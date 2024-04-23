# Comparing `tmp/kibot-1.6.5.tar.gz` & `tmp/kibot-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibot-1.6.5.tar", last modified: Sun Mar 31 15:05:15 2024, max compression
+gzip compressed data, was "kibot-1.7.0.tar", last modified: Tue Apr 23 16:16:20 2024, max compression
```

## Comparing `kibot-1.6.5.tar` & `kibot-1.7.0.tar`

### file list

```diff
@@ -1,381 +1,392 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/
--rw-rw-r--   0 root         (0) root         (0)    34523 2024-03-31 14:44:11.000000 kibot-1.6.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1000 2024-03-31 14:44:11.000000 kibot-1.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2522 2024-03-31 15:05:15.790088 kibot-1.6.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1571 2024-03-31 14:44:11.000000 kibot-1.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.750088 kibot-1.6.5/kibot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.754088 kibot-1.6.5/kibot/EasyEDA/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/EasyEDA/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13852 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/EasyEDA/easyeda_3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.754088 kibot-1.6.5/kibot/PcbDraw/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1297 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/eda_angle.py
--rw-rw-r--   0 root         (0) root         (0)     5998 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/mdrenderer.py
--rw-rw-r--   0 root         (0) root         (0)     1279 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/mistune_shim.py
--rw-rw-r--   0 root         (0) root         (0)      923 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/np.py
--rw-rw-r--   0 root         (0) root         (0)     9128 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pcbnew_transition.py
--rw-rw-r--   0 root         (0) root         (0)    55962 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/plot.py
--rw-rw-r--   0 root         (0) root         (0)    15370 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/populate.py
--rw-rw-r--   0 root         (0) root         (0)     7573 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.754088 kibot-1.6.5/kibot/PcbDraw/pybars/
--rw-rw-r--   0 root         (0) root         (0)     1706 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31100 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/_compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.754088 kibot-1.6.5/kibot/PcbDraw/pybars/_templates/
--rw-rw-r--   0 root         (0) root         (0)       77 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/_templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.758088 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    33589 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/boot.py
--rw-rw-r--   0 root         (0) root         (0)     9269 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/builder.py
--rw-rw-r--   0 root         (0) root         (0)    11467 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/grammar.py
--rw-rw-r--   0 root         (0) root         (0)    16895 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/runtime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.758088 kibot-1.6.5/kibot/PcbDraw/svgpathtools/
--rw-rw-r--   0 root         (0) root         (0)     1086 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14309 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/bezier.py
--rw-rw-r--   0 root         (0) root         (0)    17910 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/document.py
--rw-rw-r--   0 root         (0) root         (0)     2026 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/misctools.py
--rw-rw-r--   0 root         (0) root         (0)     3939 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/parser.py
--rw-rw-r--   0 root         (0) root         (0)   124423 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/path.py
--rw-rw-r--   0 root         (0) root         (0)    18064 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/paths2svg.py
--rw-rw-r--   0 root         (0) root         (0)     2473 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/polytools.py
--rw-rw-r--   0 root         (0) root         (0)     7642 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/smoothing.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/svg_io_sax.py
--rw-rw-r--   0 root         (0) root         (0)     8755 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/svgpathtools/svg_to_paths.py
--rw-rw-r--   0 root         (0) root         (0)      448 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PcbDraw/unit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.762088 kibot-1.6.5/kibot/PyPDF2/
--rw-rw-r--   0 root         (0) root         (0)      210 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       23 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/_version.py
--rw-rw-r--   0 root         (0) root         (0)    13148 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/filters.py
--rw-rw-r--   0 root         (0) root         (0)    45236 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/generic.py
--rw-rw-r--   0 root         (0) root         (0)    21296 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/merger.py
--rw-rw-r--   0 root         (0) root         (0)     5534 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/pagerange.py
--rw-rw-r--   0 root         (0) root         (0)   125850 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/pdf.py
--rw-rw-r--   0 root         (0) root         (0)     7044 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/utils.py
--rw-rw-r--   0 root         (0) root         (0)    13598 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/PyPDF2/xmp.py
--rw-rw-r--   0 root         (0) root         (0)      430 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    24049 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     5601 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/banner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.762088 kibot-1.6.5/kibot/blender_scripts/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/blender_scripts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16406 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/blender_scripts/blender_export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.762088 kibot-1.6.5/kibot/bom/
--rw-rw-r--   0 root         (0) root         (0)       57 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20712 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/bom.py
--rw-rw-r--   0 root         (0) root         (0)     1860 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/bom_writer.py
--rw-rw-r--   0 root         (0) root         (0)     4126 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/columnlist.py
--rw-rw-r--   0 root         (0) root         (0)     6737 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/csv_writer.py
--rw-rw-r--   0 root         (0) root         (0)     5467 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/electro_grammar.py
--rw-rw-r--   0 root         (0) root         (0)    22067 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/html_writer.py
--rw-rw-r--   0 root         (0) root         (0)    45883 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/kibot_logo.py
--rw-rw-r--   0 root         (0) root         (0)     9437 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/units.py
--rw-rw-r--   0 root         (0) root         (0)    34124 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/xlsx_writer.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/bom/xml_writer.py
--rw-rw-r--   0 root         (0) root         (0)    57419 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/config_reader.py
--rw-rw-r--   0 root         (0) root         (0)     1302 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/create_pdf.py
--rw-rw-r--   0 root         (0) root         (0)    37635 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/dep_downloader.py
--rw-rw-r--   0 root         (0) root         (0)    20715 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/docopt.py
--rw-rw-r--   0 root         (0) root         (0)     1698 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/drill_marks.py
--rw-rw-r--   0 root         (0) root         (0)      466 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/error.py
--rw-rw-r--   0 root         (0) root         (0)    15870 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_base.py
--rw-rw-r--   0 root         (0) root         (0)     1866 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_expand_text_vars.py
--rw-rw-r--   0 root         (0) root         (0)     2632 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_field_modify.py
--rw-rw-r--   0 root         (0) root         (0)     1498 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_field_rename.py
--rw-rw-r--   0 root         (0) root         (0)    10388 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_generic.py
--rw-rw-r--   0 root         (0) root         (0)    16203 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_rot_footprint.py
--rw-rw-r--   0 root         (0) root         (0)    11385 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_spec_to_field.py
--rw-rw-r--   0 root         (0) root         (0)    11853 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_subparts.py
--rw-rw-r--   0 root         (0) root         (0)     1449 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_urlify.py
--rw-rw-r--   0 root         (0) root         (0)     5630 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_value_split.py
--rw-rw-r--   0 root         (0) root         (0)     2429 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_var_rename.py
--rw-rw-r--   0 root         (0) root         (0)     3841 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/fil_var_rename_kicost.py
--rw-rw-r--   0 root         (0) root         (0)    28229 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/globals.py
--rw-rw-r--   0 root         (0) root         (0)    31317 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/gs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.766088 kibot-1.6.5/kibot/kicad/
--rw-rw-r--   0 root         (0) root         (0)       57 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3913 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/color_theme.py
--rw-rw-r--   0 root         (0) root         (0)    28058 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/config.py
--rw-rw-r--   0 root         (0) root         (0)      568 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/error.py
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/patch_svg.py
--rw-rw-r--   0 root         (0) root         (0)     2448 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/pcb.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/sexp_helpers.py
--rw-rw-r--   0 root         (0) root         (0)    19499 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/sexpdata.py
--rw-rw-r--   0 root         (0) root         (0)    80616 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/v5_sch.py
--rw-rw-r--   0 root         (0) root         (0)    92651 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/v6_sch.py
--rw-rw-r--   0 root         (0) root         (0)    20587 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kicad/worksheet.py
--rw-rw-r--   0 root         (0) root         (0)    43575 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/kiplot.py
--rw-rw-r--   0 root         (0) root         (0)    15187 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/layer.py
--rw-rw-r--   0 root         (0) root         (0)     9130 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/log.py
--rw-rw-r--   0 root         (0) root         (0)     6521 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/macros.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.770088 kibot-1.6.5/kibot/mcpyrate/
--rw-rw-r--   0 root         (0) root         (0)      681 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2385 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/activate.py
--rw-rw-r--   0 root         (0) root         (0)     2616 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/ansi.py
--rw-rw-r--   0 root         (0) root         (0)     3228 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/astdumper.py
--rw-rw-r--   0 root         (0) root         (0)     7096 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/astfixers.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/bunch.py
--rw-rw-r--   0 root         (0) root         (0)     6900 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/colorizer.py
--rw-rw-r--   0 root         (0) root         (0)    26173 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/compiler.py
--rw-rw-r--   0 root         (0) root         (0)    18663 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/core.py
--rw-rw-r--   0 root         (0) root         (0)    13791 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/coreutils.py
--rw-rw-r--   0 root         (0) root         (0)    11186 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/debug.py
--rw-rw-r--   0 root         (0) root         (0)    20782 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/dialects.py
--rw-rw-r--   0 root         (0) root         (0)    29602 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/expander.py
--rw-rw-r--   0 root         (0) root         (0)    10837 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/importer.py
--rw-rw-r--   0 root         (0) root         (0)     3418 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/markers.py
--rw-rw-r--   0 root         (0) root         (0)    23744 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/metatools.py
--rw-rw-r--   0 root         (0) root         (0)    17282 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/multiphase.py
--rwxrwxr-x   0 root         (0) root         (0)     1648 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/pycachecleaner.py
--rw-rw-r--   0 root         (0) root         (0)    56157 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/quotes.py
--rw-rw-r--   0 root         (0) root         (0)    12323 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/splicing.py
--rw-rw-r--   0 root         (0) root         (0)    38292 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/unparser.py
--rw-rw-r--   0 root         (0) root         (0)    12379 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/utils.py
--rw-rw-r--   0 root         (0) root         (0)     8029 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/mcpyrate/walkers.py
--rw-rw-r--   0 root         (0) root         (0)    15014 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/misc.py
--rw-rw-r--   0 root         (0) root         (0)    26347 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/optionable.py
--rw-rw-r--   0 root         (0) root         (0)     4351 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_diff.py
--rw-rw-r--   0 root         (0) root         (0)     8153 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_drill.py
--rw-rw-r--   0 root         (0) root         (0)    15301 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_layer.py
--rw-rw-r--   0 root         (0) root         (0)     4651 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_pcb_print.py
--rw-rw-r--   0 root         (0) root         (0)     2977 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)     5709 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_any_stencil.py
--rw-rw-r--   0 root         (0) root         (0)    49092 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_base.py
--rw-rw-r--   0 root         (0) root         (0)    28761 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_base_3d.py
--rw-rw-r--   0 root         (0) root         (0)    32825 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_blender_export.py
--rw-rw-r--   0 root         (0) root         (0)     6685 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_boardview.py
--rw-rw-r--   0 root         (0) root         (0)    53429 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_bom.py
--rw-rw-r--   0 root         (0) root         (0)    11742 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_compress.py
--rw-rw-r--   0 root         (0) root         (0)    18197 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_copy_files.py
--rw-rw-r--   0 root         (0) root         (0)    28308 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_diff.py
--rw-rw-r--   0 root         (0) root         (0)     7329 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_download_datasheets.py
--rw-rw-r--   0 root         (0) root         (0)     2500 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_dxf.py
--rw-rw-r--   0 root         (0) root         (0)     1576 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_dxf_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)     3032 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_excellon.py
--rw-rw-r--   0 root         (0) root         (0)     2821 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_gencad.py
--rw-rw-r--   0 root         (0) root         (0)     1603 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_gerb_drill.py
--rw-rw-r--   0 root         (0) root         (0)     6668 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_gerber.py
--rw-rw-r--   0 root         (0) root         (0)     2211 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_hpgl.py
--rw-rw-r--   0 root         (0) root         (0)     1948 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_hpgl_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)    13303 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_ibom.py
--rw-rw-r--   0 root         (0) root         (0)     2669 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_info.py
--rw-rw-r--   0 root         (0) root         (0)    19404 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_kibom.py
--rw-rw-r--   0 root         (0) root         (0)     9913 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_kicanvas.py
--rw-rw-r--   0 root         (0) root         (0)    10307 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_kicost.py
--rw-rw-r--   0 root         (0) root         (0)    19392 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_kikit_present.py
--rw-rw-r--   0 root         (0) root         (0)    18976 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_kiri.py
--rw-rw-r--   0 root         (0) root         (0)    31708 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_navigate_results.py
--rw-rw-r--   0 root         (0) root         (0)     3023 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_netlist.py
--rw-rw-r--   0 root         (0) root         (0)    40932 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_panelize.py
--rw-rw-r--   0 root         (0) root         (0)    16667 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pcb2blender_tools.py
--rw-rw-r--   0 root         (0) root         (0)    65105 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pcb_print.py
--rw-rw-r--   0 root         (0) root         (0)     2225 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pcb_variant.py
--rw-rw-r--   0 root         (0) root         (0)    24613 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pcbdraw.py
--rw-rw-r--   0 root         (0) root         (0)     2080 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pdf.py
--rw-rw-r--   0 root         (0) root         (0)     1918 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pdf_pcb_print.py
--rw-rw-r--   0 root         (0) root         (0)     1652 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pdf_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)     6190 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_pdfunite.py
--rw-rw-r--   0 root         (0) root         (0)     7631 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_populate.py
--rw-rw-r--   0 root         (0) root         (0)    16617 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_position.py
--rw-rw-r--   0 root         (0) root         (0)     3058 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_ps.py
--rw-rw-r--   0 root         (0) root         (0)     1554 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_ps_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)    25162 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_qr_lib.py
--rw-rw-r--   0 root         (0) root         (0)    15029 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_render_3d.py
--rw-rw-r--   0 root         (0) root         (0)    42017 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_report.py
--rw-rw-r--   0 root         (0) root         (0)     2133 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_sch_variant.py
--rw-rw-r--   0 root         (0) root         (0)     5798 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_stencil_3d.py
--rw-rw-r--   0 root         (0) root         (0)     6151 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_stencil_for_jig.py
--rw-rw-r--   0 root         (0) root         (0)     3877 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_step.py
--rw-rw-r--   0 root         (0) root         (0)     4734 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_svg.py
--rw-rw-r--   0 root         (0) root         (0)     2647 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_svg_pcb_print.py
--rw-rw-r--   0 root         (0) root         (0)     1626 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_svg_sch_print.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/out_vrml.py
--rw-rw-r--   0 root         (0) root         (0)     9708 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_annotate_pcb.py
--rw-rw-r--   0 root         (0) root         (0)     2666 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_annotate_power.py
--rw-rw-r--   0 root         (0) root         (0)     5465 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_any_replace.py
--rw-rw-r--   0 root         (0) root         (0)     6376 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_base.py
--rw-rw-r--   0 root         (0) root         (0)      935 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_check_zone_fills.py
--rw-rw-r--   0 root         (0) root         (0)      920 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_erc_warnings.py
--rw-rw-r--   0 root         (0) root         (0)     1151 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_fill_zones.py
--rw-rw-r--   0 root         (0) root         (0)     4163 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_filters.py
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_ignore_unconnected.py
--rw-rw-r--   0 root         (0) root         (0)     2025 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_pcb_replace.py
--rw-rw-r--   0 root         (0) root         (0)     4687 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_run_drc.py
--rw-rw-r--   0 root         (0) root         (0)     4279 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_run_erc.py
--rw-rw-r--   0 root         (0) root         (0)     2513 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_sch_replace.py
--rw-rw-r--   0 root         (0) root         (0)     7087 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_set_text_variables.py
--rw-rw-r--   0 root         (0) root         (0)     1170 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_update_qr.py
--rw-rw-r--   0 root         (0) root         (0)    10229 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/pre_update_xml.py
--rw-rw-r--   0 root         (0) root         (0)     7383 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/registrable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.730088 kibot-1.6.5/kibot/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.774088 kibot-1.6.5/kibot/resources/config_templates/
--rw-rw-r--   0 root         (0) root         (0)      717 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/3DRender.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      196 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/3DRender_bottom.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      157 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/3DRender_bottom_straight.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      163 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/3DRender_top.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      125 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/3DRender_top_straight.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      821 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/CheckZoneFill.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     2337 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/Elecrow.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      132 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/Elecrow_stencil.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     2406 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/FusionPCB.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      134 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/FusionPCB_stencil.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     4571 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/JLCPCB.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      299 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/JLCPCB_stencil.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      104 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/JLCPCB_stencil_with_THT.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)       96 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/JLCPCB_with_THT.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     1401 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/MacroFab_XYRS.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     3215 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/P-Ban.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      130 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/P-Ban_stencil.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     1567 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_1.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     1072 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_1_haschtl.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     1687 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_7.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     2612 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PCBWay.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)      131 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PCBWay_stencil.kibot.yaml
--rw-rw-r--   0 root         (0) root         (0)     1410 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/config_templates/PanelDemo_4x4.kibot.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.778088 kibot-1.6.5/kibot/resources/images/
--rw-rw-r--   0 root         (0) root         (0)     3577 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/3d.svg
--rw-rw-r--   0 root         (0) root         (0)     6278 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/assembly_simple.svg
--rw-rw-r--   0 root         (0) root         (0)     3982 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/back.svg
--rw-rw-r--   0 root         (0) root         (0)     5773 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/bom.svg
--rw-rw-r--   0 root         (0) root         (0)     7222 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/eeschema.svg
--rw-rw-r--   0 root         (0) root         (0)     1820 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/export.svg
--rw-rw-r--   0 root         (0) root         (0)     2833 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/fabrication.svg
--rw-rw-r--   0 root         (0) root         (0)     4286 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/favicon.ico
--rw-rw-r--   0 root         (0) root         (0)    10332 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_blend.svg
--rw-rw-r--   0 root         (0) root         (0)     9125 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_brd.svg
--rw-rw-r--   0 root         (0) root         (0)     5394 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_bz2.svg
--rw-rw-r--   0 root         (0) root         (0)     7388 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_cad.svg
--rw-rw-r--   0 root         (0) root         (0)     4991 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_css.svg
--rw-rw-r--   0 root         (0) root         (0)     7199 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_csv.svg
--rw-rw-r--   0 root         (0) root         (0)     4080 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_drl.svg
--rw-rw-r--   0 root         (0) root         (0)     4826 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_dxf.svg
--rw-rw-r--   0 root         (0) root         (0)     7137 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_eps.svg
--rw-rw-r--   0 root         (0) root         (0)     6964 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_gbr.svg
--rw-rw-r--   0 root         (0) root         (0)     8756 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_gerber_job.svg
--rw-rw-r--   0 root         (0) root         (0)     4603 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_gz.svg
--rw-rw-r--   0 root         (0) root         (0)     4384 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_html.svg
--rw-rw-r--   0 root         (0) root         (0)     4795 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_jpg.svg
--rw-rw-r--   0 root         (0) root         (0)    11418 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_pcb3d.svg
--rw-rw-r--   0 root         (0) root         (0)     7488 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_pdf.svg
--rw-rw-r--   0 root         (0) root         (0)     5744 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_plt.svg
--rw-rw-r--   0 root         (0) root         (0)     4610 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_png.svg
--rw-rw-r--   0 root         (0) root         (0)     6299 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_pos.svg
--rw-rw-r--   0 root         (0) root         (0)     4761 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_ps.svg
--rw-rw-r--   0 root         (0) root         (0)     5726 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_rar.svg
--rw-rw-r--   0 root         (0) root         (0)     8380 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_scad.svg
--rw-rw-r--   0 root         (0) root         (0)     7131 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_stl.svg
--rw-rw-r--   0 root         (0) root         (0)     7581 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_stp.svg
--rw-rw-r--   0 root         (0) root         (0)     7778 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_svg.svg
--rw-rw-r--   0 root         (0) root         (0)     5436 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_tar.svg
--rw-rw-r--   0 root         (0) root         (0)     7107 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_tsv.svg
--rw-rw-r--   0 root         (0) root         (0)     4466 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_txt.svg
--rw-rw-r--   0 root         (0) root         (0)     7133 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_wrl.svg
--rw-rw-r--   0 root         (0) root         (0)     6988 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_xlsx.svg
--rw-rw-r--   0 root         (0) root         (0)     3830 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_xml.svg
--rw-rw-r--   0 root         (0) root         (0)    10186 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_xyrs.svg
--rw-rw-r--   0 root         (0) root         (0)     3912 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_xz.svg
--rw-rw-r--   0 root         (0) root         (0)     4841 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/file_zip.svg
--rw-rw-r--   0 root         (0) root         (0)     2884 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/folder.svg
--rw-rw-r--   0 root         (0) root         (0)    19304 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/gerber.svg
--rw-rw-r--   0 root         (0) root         (0)     5056 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/home.svg
--rw-rw-r--   0 root         (0) root         (0)     8080 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/ibom.svg
--rw-rw-r--   0 root         (0) root         (0)     9238 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/load_drill.svg
--rw-rw-r--   0 root         (0) root         (0)    11424 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/pcbnew.svg
--rw-rw-r--   0 root         (0) root         (0)     4445 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/project.svg
--rw-rw-r--   0 root         (0) root         (0)     2240 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/repair.svg
--rw-rw-r--   0 root         (0) root         (0)     3958 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/unknown.svg
--rw-rw-r--   0 root         (0) root         (0)     2563 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/images/zip.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.782088 kibot-1.6.5/kibot/resources/kicad_colors/
--rw-rw-r--   0 root         (0) root         (0)     6954 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kicad_colors/_builtin_classic.json
--rw-rw-r--   0 root         (0) root         (0)     7124 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kicad_colors/_builtin_default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.782088 kibot-1.6.5/kibot/resources/kicad_layouts/
--rw-rw-r--   0 root         (0) root         (0)     2027 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kicad_layouts/default.kicad_wks
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.782088 kibot-1.6.5/kibot/resources/kicanvas/
--rw-rw-r--   0 root         (0) root         (0)     8636 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kicanvas/kicanvas.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.782088 kibot-1.6.5/kibot/resources/kiri/
--rw-rw-r--   0 root         (0) root         (0)      486 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/blank.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.782088 kibot-1.6.5/kibot/resources/kiri/images/
--rw-rw-r--   0 root         (0) root         (0)      310 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/center-to-fit.svg
--rw-rw-r--   0 root         (0) root         (0)      500 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/circuit-board.svg
--rw-rw-r--   0 root         (0) root         (0)      893 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/code-branch-solid.svg
--rw-rw-r--   0 root         (0) root         (0)      194 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/commit.svg
--rw-rw-r--   0 root         (0) root         (0)     2929 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/icon.svg
--rw-rw-r--   0 root         (0) root         (0)      301 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/info.svg
--rw-rw-r--   0 root         (0) root         (0)      410 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/layers-solid.svg
--rw-rw-r--   0 root         (0) root         (0)      283 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/next-page.svg
--rw-rw-r--   0 root         (0) root         (0)      240 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/pages.svg
--rw-rw-r--   0 root         (0) root         (0)      506 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/schematics.svg
--rw-rw-r--   0 root         (0) root         (0)      224 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/square-solid.svg
--rw-rw-r--   0 root         (0) root         (0)      269 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/x.svg
--rw-rw-r--   0 root         (0) root         (0)      279 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/zoom-in.svg
--rw-rw-r--   0 root         (0) root         (0)      250 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/images/zoom-out.svg
--rw-rw-r--   0 root         (0) root         (0)    15283 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/index.html
--rwxrwxr-x   0 root         (0) root         (0)     5545 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/kiri-server
--rw-rw-r--   0 root         (0) root         (0)    10089 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/kiri.css
--rw-rw-r--   0 root         (0) root         (0)    45441 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/kiri.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.786088 kibot-1.6.5/kibot/resources/kiri/utils/
--rw-rw-r--   0 root         (0) root         (0)    83253 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/utils/bootstrap.bundle.min.js
--rw-rw-r--   0 root         (0) root         (0)   162017 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/utils/bootstrap.min.css
--rw-rw-r--   0 root         (0) root         (0)    89501 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/utils/jquery-3.6.0.min.js
--rw-rw-r--   0 root         (0) root         (0)    29768 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/kiri/utils/svg-pan-zoom.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.786088 kibot-1.6.5/kibot/resources/parsers/
--rw-rw-r--   0 root         (0) root         (0)     7179 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/parsers/electro.lark
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.730088 kibot-1.6.5/kibot/resources/pcbdraw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.730088 kibot-1.6.5/kibot/resources/pcbdraw/present/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.730088 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.786088 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.786088 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/css/
--rw-rw-r--   0 root         (0) root         (0)     4006 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/css/styles.css
--rw-rw-r--   0 root         (0) root         (0)     1882 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/index.html
--rw-rw-r--   0 root         (0) root         (0)    81945 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/package-lock.json
--rw-rw-r--   0 root         (0) root         (0)      443 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/package.json
--rw-rw-r--   0 root         (0) root         (0)      358 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/postcss.config.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.786088 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/src/
--rw-rw-r--   0 root         (0) root         (0)      819 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/src/styles.css
--rw-rw-r--   0 root         (0) root         (0)       84 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/tailwind.config.js
--rw-rw-r--   0 root         (0) root         (0)       62 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/template.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/kibot/resources/pcbdraw/styles/
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/gatema-green.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/jlcpcb-green-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/jlcpcb-green-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/mayer-yellow-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/oshpark-afterdark.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/oshpark-purple.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-black-cu.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-black-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-black-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-blue-cu.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-blue-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-blue-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-red-cu.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-red-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-red-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-white-cu.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-white-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-white-hasl.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-yellow-cu.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-yellow-enig.json
--rw-rw-r--   0 root         (0) root         (0)      321 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/styles/set-yellow-hasl.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/kibot/resources/pcbdraw/templates/
--rw-rw-r--   0 root         (0) root         (0)     1508 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/pcbdraw/templates/simple.handlebars
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/kibot/resources/report_templates/
--rw-rw-r--   0 root         (0) root         (0)     3658 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/report_templates/report_full.txt
--rw-rw-r--   0 root         (0) root         (0)     3658 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/report_templates/report_full_svg.txt
--rw-rw-r--   0 root         (0) root         (0)     1459 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/resources/report_templates/report_simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/kibot/svgutils/
--rw-rw-r--   0 root         (0) root         (0)       48 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/svgutils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11209 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/svgutils/compose.py
--rw-rw-r--   0 root         (0) root         (0)     2048 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/svgutils/templates.py
--rw-rw-r--   0 root         (0) root         (0)    12513 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/svgutils/transform.py
--rw-rw-r--   0 root         (0) root         (0)    18208 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/var_base.py
--rw-rw-r--   0 root         (0) root         (0)     3434 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/var_ibom.py
--rw-rw-r--   0 root         (0) root         (0)     4981 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/var_kibom.py
--rw-rw-r--   0 root         (0) root         (0)     3908 2024-03-31 14:44:11.000000 kibot-1.6.5/kibot/var_kicost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.754088 kibot-1.6.5/kibot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2522 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11320 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-31 15:05:15.000000 kibot-1.6.5/kibot.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      936 2024-03-31 15:05:15.790088 kibot-1.6.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1621 2024-03-31 14:44:11.000000 kibot-1.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:05:15.790088 kibot-1.6.5/src/
--rwxrwxr-x   0 root         (0) root         (0)    59043 2024-03-31 14:44:11.000000 kibot-1.6.5/src/kibot-check
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.852519 kibot-1.7.0/
+-rw-rw-r--   0 root         (0) root         (0)    34523 2024-04-23 16:14:28.000000 kibot-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1000 2024-04-23 16:14:28.000000 kibot-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-04-23 16:16:20.852519 kibot-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1571 2024-04-23 16:14:28.000000 kibot-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot/EasyEDA/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/EasyEDA/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13852 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/EasyEDA/easyeda_3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot/PcbDraw/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1297 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/eda_angle.py
+-rw-rw-r--   0 root         (0) root         (0)     5998 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/mdrenderer.py
+-rw-rw-r--   0 root         (0) root         (0)     1279 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/mistune_shim.py
+-rw-rw-r--   0 root         (0) root         (0)      923 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/np.py
+-rw-rw-r--   0 root         (0) root         (0)     9128 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pcbnew_transition.py
+-rw-rw-r--   0 root         (0) root         (0)    56059 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/plot.py
+-rw-rw-r--   0 root         (0) root         (0)    15370 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/populate.py
+-rw-rw-r--   0 root         (0) root         (0)     7573 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot/PcbDraw/pybars/
+-rw-rw-r--   0 root         (0) root         (0)     1706 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31100 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/_compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot/PcbDraw/pybars/_templates/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/_templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.816519 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    33589 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/boot.py
+-rw-rw-r--   0 root         (0) root         (0)     9269 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/builder.py
+-rw-rw-r--   0 root         (0) root         (0)    11467 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)    16895 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/runtime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.816519 kibot-1.7.0/kibot/PcbDraw/svgpathtools/
+-rw-rw-r--   0 root         (0) root         (0)     1086 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14309 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/bezier.py
+-rw-rw-r--   0 root         (0) root         (0)    17910 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/document.py
+-rw-rw-r--   0 root         (0) root         (0)     2026 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/misctools.py
+-rw-rw-r--   0 root         (0) root         (0)     3939 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/parser.py
+-rw-rw-r--   0 root         (0) root         (0)   124423 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/path.py
+-rw-rw-r--   0 root         (0) root         (0)    18064 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/paths2svg.py
+-rw-rw-r--   0 root         (0) root         (0)     2473 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/polytools.py
+-rw-rw-r--   0 root         (0) root         (0)     7642 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/smoothing.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/svg_io_sax.py
+-rw-rw-r--   0 root         (0) root         (0)     8755 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/svgpathtools/svg_to_paths.py
+-rw-rw-r--   0 root         (0) root         (0)      448 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PcbDraw/unit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.820519 kibot-1.7.0/kibot/PyPDF2/
+-rw-rw-r--   0 root         (0) root         (0)      210 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       23 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/_version.py
+-rw-rw-r--   0 root         (0) root         (0)    13148 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/filters.py
+-rw-rw-r--   0 root         (0) root         (0)    45236 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/generic.py
+-rw-rw-r--   0 root         (0) root         (0)    21296 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/merger.py
+-rw-rw-r--   0 root         (0) root         (0)     5534 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/pagerange.py
+-rw-rw-r--   0 root         (0) root         (0)   125850 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/pdf.py
+-rw-rw-r--   0 root         (0) root         (0)     7044 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    13598 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/PyPDF2/xmp.py
+-rw-rw-r--   0 root         (0) root         (0)      430 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    24187 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     5601 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/banner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.820519 kibot-1.7.0/kibot/blender_scripts/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/blender_scripts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16406 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/blender_scripts/blender_export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.820519 kibot-1.7.0/kibot/bom/
+-rw-rw-r--   0 root         (0) root         (0)       57 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    20712 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/bom.py
+-rw-rw-r--   0 root         (0) root         (0)     1860 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/bom_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     4126 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/columnlist.py
+-rw-rw-r--   0 root         (0) root         (0)     6737 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/csv_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     5467 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/electro_grammar.py
+-rw-rw-r--   0 root         (0) root         (0)    19759 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/html_writer.py
+-rw-rw-r--   0 root         (0) root         (0)    60265 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/kibot_logo.py
+-rw-rw-r--   0 root         (0) root         (0)     9437 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/units.py
+-rw-rw-r--   0 root         (0) root         (0)    35261 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/xlsx_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/bom/xml_writer.py
+-rw-rw-r--   0 root         (0) root         (0)    57419 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/config_reader.py
+-rw-rw-r--   0 root         (0) root         (0)     1302 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/create_pdf.py
+-rw-rw-r--   0 root         (0) root         (0)    37635 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/dep_downloader.py
+-rw-rw-r--   0 root         (0) root         (0)    20715 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/docopt.py
+-rw-rw-r--   0 root         (0) root         (0)     1698 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/drill_marks.py
+-rw-rw-r--   0 root         (0) root         (0)      466 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/error.py
+-rw-rw-r--   0 root         (0) root         (0)    15870 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_base.py
+-rw-rw-r--   0 root         (0) root         (0)     1866 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_expand_text_vars.py
+-rw-rw-r--   0 root         (0) root         (0)     2632 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_field_modify.py
+-rw-rw-r--   0 root         (0) root         (0)     1498 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_field_rename.py
+-rw-rw-r--   0 root         (0) root         (0)    10388 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_generic.py
+-rw-rw-r--   0 root         (0) root         (0)    16203 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_rot_footprint.py
+-rw-rw-r--   0 root         (0) root         (0)    11385 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_spec_to_field.py
+-rw-rw-r--   0 root         (0) root         (0)    11853 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_subparts.py
+-rw-rw-r--   0 root         (0) root         (0)     1449 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_urlify.py
+-rw-rw-r--   0 root         (0) root         (0)     5630 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_value_split.py
+-rw-rw-r--   0 root         (0) root         (0)     3122 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_var_rename.py
+-rw-rw-r--   0 root         (0) root         (0)     4721 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/fil_var_rename_kicost.py
+-rw-rw-r--   0 root         (0) root         (0)    28539 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/globals.py
+-rw-rw-r--   0 root         (0) root         (0)    34588 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/gs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.824519 kibot-1.7.0/kibot/kicad/
+-rw-rw-r--   0 root         (0) root         (0)       57 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3913 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/color_theme.py
+-rw-rw-r--   0 root         (0) root         (0)    30644 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/config.py
+-rw-rw-r--   0 root         (0) root         (0)      568 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/error.py
+-rw-rw-r--   0 root         (0) root         (0)     1798 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/patch_svg.py
+-rw-rw-r--   0 root         (0) root         (0)     6353 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/pcb.py
+-rw-rw-r--   0 root         (0) root         (0)     5906 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/sexp_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)    19499 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/sexpdata.py
+-rw-rw-r--   0 root         (0) root         (0)    80749 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/v5_sch.py
+-rw-rw-r--   0 root         (0) root         (0)    92651 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/v6_sch.py
+-rw-rw-r--   0 root         (0) root         (0)    20809 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kicad/worksheet.py
+-rw-rw-r--   0 root         (0) root         (0)    45124 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/kiplot.py
+-rw-rw-r--   0 root         (0) root         (0)    15187 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/layer.py
+-rw-rw-r--   0 root         (0) root         (0)     9130 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/log.py
+-rw-rw-r--   0 root         (0) root         (0)     6521 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/macros.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.828519 kibot-1.7.0/kibot/mcpyrate/
+-rw-rw-r--   0 root         (0) root         (0)      681 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2385 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/activate.py
+-rw-rw-r--   0 root         (0) root         (0)     2616 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/ansi.py
+-rw-rw-r--   0 root         (0) root         (0)     3228 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/astdumper.py
+-rw-rw-r--   0 root         (0) root         (0)     7096 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/astfixers.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/bunch.py
+-rw-rw-r--   0 root         (0) root         (0)     6900 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/colorizer.py
+-rw-rw-r--   0 root         (0) root         (0)    26173 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/compiler.py
+-rw-rw-r--   0 root         (0) root         (0)    18663 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/core.py
+-rw-rw-r--   0 root         (0) root         (0)    13791 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/coreutils.py
+-rw-rw-r--   0 root         (0) root         (0)    11186 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/debug.py
+-rw-rw-r--   0 root         (0) root         (0)    20782 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/dialects.py
+-rw-rw-r--   0 root         (0) root         (0)    29602 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/expander.py
+-rw-rw-r--   0 root         (0) root         (0)    10837 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/importer.py
+-rw-rw-r--   0 root         (0) root         (0)     3418 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/markers.py
+-rw-rw-r--   0 root         (0) root         (0)    23744 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/metatools.py
+-rw-rw-r--   0 root         (0) root         (0)    17282 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/multiphase.py
+-rwxrwxr-x   0 root         (0) root         (0)     1648 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/pycachecleaner.py
+-rw-rw-r--   0 root         (0) root         (0)    56157 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/quotes.py
+-rw-rw-r--   0 root         (0) root         (0)    12323 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/splicing.py
+-rw-rw-r--   0 root         (0) root         (0)    38292 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/unparser.py
+-rw-rw-r--   0 root         (0) root         (0)    12379 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8029 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/mcpyrate/walkers.py
+-rw-rw-r--   0 root         (0) root         (0)    19080 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    26347 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/optionable.py
+-rw-rw-r--   0 root         (0) root         (0)     4191 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_diff.py
+-rw-rw-r--   0 root         (0) root         (0)     8153 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_drill.py
+-rw-rw-r--   0 root         (0) root         (0)    15301 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_layer.py
+-rw-rw-r--   0 root         (0) root         (0)     4780 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_pcb_print.py
+-rw-rw-r--   0 root         (0) root         (0)     5010 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)     5709 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_any_stencil.py
+-rw-rw-r--   0 root         (0) root         (0)    49706 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_base.py
+-rw-rw-r--   0 root         (0) root         (0)    28761 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_base_3d.py
+-rw-rw-r--   0 root         (0) root         (0)    32825 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_blender_export.py
+-rw-rw-r--   0 root         (0) root         (0)     6685 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_boardview.py
+-rw-rw-r--   0 root         (0) root         (0)    55021 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_bom.py
+-rw-rw-r--   0 root         (0) root         (0)    12837 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_compress.py
+-rw-rw-r--   0 root         (0) root         (0)    18719 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_copy_files.py
+-rw-rw-r--   0 root         (0) root         (0)    28329 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_diff.py
+-rw-rw-r--   0 root         (0) root         (0)     7329 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_download_datasheets.py
+-rw-rw-r--   0 root         (0) root         (0)     2500 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_dxf.py
+-rw-rw-r--   0 root         (0) root         (0)     1576 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_dxf_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)     3032 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_excellon.py
+-rw-rw-r--   0 root         (0) root         (0)     2821 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_gencad.py
+-rw-rw-r--   0 root         (0) root         (0)     1603 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_gerb_drill.py
+-rw-rw-r--   0 root         (0) root         (0)     6668 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_gerber.py
+-rw-rw-r--   0 root         (0) root         (0)     2211 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_hpgl.py
+-rw-rw-r--   0 root         (0) root         (0)     1948 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_hpgl_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)    13259 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_ibom.py
+-rw-rw-r--   0 root         (0) root         (0)     2669 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_info.py
+-rw-rw-r--   0 root         (0) root         (0)    19147 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_kibom.py
+-rw-rw-r--   0 root         (0) root         (0)     9913 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_kicanvas.py
+-rw-rw-r--   0 root         (0) root         (0)    10263 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_kicost.py
+-rw-rw-r--   0 root         (0) root         (0)    19327 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_kikit_present.py
+-rw-rw-r--   0 root         (0) root         (0)    18965 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_kiri.py
+-rw-rw-r--   0 root         (0) root         (0)    32298 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_navigate_results.py
+-rw-rw-r--   0 root         (0) root         (0)     3023 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_netlist.py
+-rw-rw-r--   0 root         (0) root         (0)    40767 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_panelize.py
+-rw-rw-r--   0 root         (0) root         (0)    16667 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pcb2blender_tools.py
+-rw-rw-r--   0 root         (0) root         (0)    65627 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pcb_print.py
+-rw-rw-r--   0 root         (0) root         (0)     2225 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pcb_variant.py
+-rw-rw-r--   0 root         (0) root         (0)    24847 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pcbdraw.py
+-rw-rw-r--   0 root         (0) root         (0)     2080 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pdf.py
+-rw-rw-r--   0 root         (0) root         (0)     1918 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pdf_pcb_print.py
+-rw-rw-r--   0 root         (0) root         (0)     1652 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pdf_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)     6190 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_pdfunite.py
+-rw-rw-r--   0 root         (0) root         (0)     7457 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_populate.py
+-rw-rw-r--   0 root         (0) root         (0)    16617 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_position.py
+-rw-rw-r--   0 root         (0) root         (0)     3058 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_ps.py
+-rw-rw-r--   0 root         (0) root         (0)     1554 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_ps_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)    23412 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_qr_lib.py
+-rw-rw-r--   0 root         (0) root         (0)    18192 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_render_3d.py
+-rw-rw-r--   0 root         (0) root         (0)    40766 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_report.py
+-rw-rw-r--   0 root         (0) root         (0)     2133 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_sch_variant.py
+-rw-rw-r--   0 root         (0) root         (0)     5798 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_stencil_3d.py
+-rw-rw-r--   0 root         (0) root         (0)     6151 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_stencil_for_jig.py
+-rw-rw-r--   0 root         (0) root         (0)     3877 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_step.py
+-rw-rw-r--   0 root         (0) root         (0)     4734 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_svg.py
+-rw-rw-r--   0 root         (0) root         (0)     2647 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_svg_pcb_print.py
+-rw-rw-r--   0 root         (0) root         (0)     1626 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_svg_sch_print.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/out_vrml.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_annotate_pcb.py
+-rw-rw-r--   0 root         (0) root         (0)     2490 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_annotate_power.py
+-rw-rw-r--   0 root         (0) root         (0)     5465 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_any_replace.py
+-rw-rw-r--   0 root         (0) root         (0)    13613 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_any_xrc.py
+-rw-rw-r--   0 root         (0) root         (0)     8106 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_base.py
+-rw-rw-r--   0 root         (0) root         (0)      757 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_check_zone_fills.py
+-rw-rw-r--   0 root         (0) root         (0)    15705 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_draw_stackup.py
+-rw-rw-r--   0 root         (0) root         (0)     7920 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_drc.py
+-rw-rw-r--   0 root         (0) root         (0)     7605 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_erc.py
+-rw-rw-r--   0 root         (0) root         (0)     1003 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_erc_warnings.py
+-rw-rw-r--   0 root         (0) root         (0)      975 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_fill_zones.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_filters.py
+-rw-rw-r--   0 root         (0) root         (0)     1123 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_ignore_unconnected.py
+-rw-rw-r--   0 root         (0) root         (0)     2082 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_pcb_replace.py
+-rw-rw-r--   0 root         (0) root         (0)     4855 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_run_drc.py
+-rw-rw-r--   0 root         (0) root         (0)     4380 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_run_erc.py
+-rw-rw-r--   0 root         (0) root         (0)     2570 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_sch_replace.py
+-rw-rw-r--   0 root         (0) root         (0)     7144 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_set_text_variables.py
+-rw-rw-r--   0 root         (0) root         (0)     1552 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_update_footprint.py
+-rw-rw-r--   0 root         (0) root         (0)     3625 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_update_pcb_characteristics.py
+-rw-rw-r--   0 root         (0) root         (0)      994 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_update_qr.py
+-rw-rw-r--   0 root         (0) root         (0)     9990 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_update_stackup.py
+-rw-rw-r--   0 root         (0) root         (0)    10414 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/pre_update_xml.py
+-rw-rw-r--   0 root         (0) root         (0)     7383 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/registrable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.788519 kibot-1.7.0/kibot/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.832519 kibot-1.7.0/kibot/resources/config_templates/
+-rw-rw-r--   0 root         (0) root         (0)      717 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/3DRender.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      196 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/3DRender_bottom.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      157 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/3DRender_bottom_straight.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      163 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/3DRender_top.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      125 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/3DRender_top_straight.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      821 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/CheckZoneFill.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     2337 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/Elecrow.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      132 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/Elecrow_stencil.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      707 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/ExportProject.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     2406 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/FusionPCB.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      134 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/FusionPCB_stencil.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     4571 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/JLCPCB.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      299 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/JLCPCB_stencil.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      104 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/JLCPCB_stencil_with_THT.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)       96 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/JLCPCB_with_THT.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1401 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/MacroFab_XYRS.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     3215 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/P-Ban.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      130 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/P-Ban_stencil.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1567 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_1.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1072 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_1_haschtl.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1687 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_7.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     2612 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PCBWay.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)      131 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PCBWay_stencil.kibot.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1410 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/config_templates/PanelDemo_4x4.kibot.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.840519 kibot-1.7.0/kibot/resources/images/
+-rw-rw-r--   0 root         (0) root         (0)     3577 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/3d.svg
+-rw-rw-r--   0 root         (0) root         (0)     6278 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/assembly_simple.svg
+-rw-rw-r--   0 root         (0) root         (0)     3982 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/back.svg
+-rw-rw-r--   0 root         (0) root         (0)     5773 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/bom.svg
+-rw-rw-r--   0 root         (0) root         (0)     5957 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/drc.svg
+-rw-rw-r--   0 root         (0) root         (0)     7222 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/eeschema.svg
+-rw-rw-r--   0 root         (0) root         (0)     4303 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/erc.svg
+-rw-rw-r--   0 root         (0) root         (0)     1820 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/export.svg
+-rw-rw-r--   0 root         (0) root         (0)     2833 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/fabrication.svg
+-rw-rw-r--   0 root         (0) root         (0)     4286 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/favicon.ico
+-rw-rw-r--   0 root         (0) root         (0)    10332 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_blend.svg
+-rw-rw-r--   0 root         (0) root         (0)     9125 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_brd.svg
+-rw-rw-r--   0 root         (0) root         (0)     5394 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_bz2.svg
+-rw-rw-r--   0 root         (0) root         (0)     7388 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_cad.svg
+-rw-rw-r--   0 root         (0) root         (0)     4991 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_css.svg
+-rw-rw-r--   0 root         (0) root         (0)     7199 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_csv.svg
+-rw-rw-r--   0 root         (0) root         (0)     4080 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_drl.svg
+-rw-rw-r--   0 root         (0) root         (0)     4826 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_dxf.svg
+-rw-rw-r--   0 root         (0) root         (0)     7137 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_eps.svg
+-rw-rw-r--   0 root         (0) root         (0)     6964 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_gbr.svg
+-rw-rw-r--   0 root         (0) root         (0)     8756 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_gerber_job.svg
+-rw-rw-r--   0 root         (0) root         (0)     4603 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_gz.svg
+-rw-rw-r--   0 root         (0) root         (0)     4384 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_html.svg
+-rw-rw-r--   0 root         (0) root         (0)     4795 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_jpg.svg
+-rw-rw-r--   0 root         (0) root         (0)     3774 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_json.svg
+-rw-rw-r--   0 root         (0) root         (0)    11418 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_pcb3d.svg
+-rw-rw-r--   0 root         (0) root         (0)     7488 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_pdf.svg
+-rw-rw-r--   0 root         (0) root         (0)     5744 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_plt.svg
+-rw-rw-r--   0 root         (0) root         (0)     4610 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_png.svg
+-rw-rw-r--   0 root         (0) root         (0)     6299 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_pos.svg
+-rw-rw-r--   0 root         (0) root         (0)     4761 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_ps.svg
+-rw-rw-r--   0 root         (0) root         (0)     5726 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_rar.svg
+-rw-rw-r--   0 root         (0) root         (0)     8380 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_scad.svg
+-rw-rw-r--   0 root         (0) root         (0)     7131 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_stl.svg
+-rw-rw-r--   0 root         (0) root         (0)     7581 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_stp.svg
+-rw-rw-r--   0 root         (0) root         (0)     7778 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_svg.svg
+-rw-rw-r--   0 root         (0) root         (0)     5436 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_tar.svg
+-rw-rw-r--   0 root         (0) root         (0)     7107 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_tsv.svg
+-rw-rw-r--   0 root         (0) root         (0)     4466 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_txt.svg
+-rw-rw-r--   0 root         (0) root         (0)     7133 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_wrl.svg
+-rw-rw-r--   0 root         (0) root         (0)     6988 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_xlsx.svg
+-rw-rw-r--   0 root         (0) root         (0)     3830 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_xml.svg
+-rw-rw-r--   0 root         (0) root         (0)    10186 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_xyrs.svg
+-rw-rw-r--   0 root         (0) root         (0)     3912 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_xz.svg
+-rw-rw-r--   0 root         (0) root         (0)     4841 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/file_zip.svg
+-rw-rw-r--   0 root         (0) root         (0)     2884 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/folder.svg
+-rw-rw-r--   0 root         (0) root         (0)    19304 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/gerber.svg
+-rw-rw-r--   0 root         (0) root         (0)     5056 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/home.svg
+-rw-rw-r--   0 root         (0) root         (0)     8080 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/ibom.svg
+-rw-rw-r--   0 root         (0) root         (0)     9238 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/load_drill.svg
+-rw-rw-r--   0 root         (0) root         (0)    11424 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/pcbnew.svg
+-rw-rw-r--   0 root         (0) root         (0)     4445 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/project.svg
+-rw-rw-r--   0 root         (0) root         (0)     2240 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/repair.svg
+-rw-rw-r--   0 root         (0) root         (0)     3958 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/unknown.svg
+-rw-rw-r--   0 root         (0) root         (0)     2563 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/images/zip.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.840519 kibot-1.7.0/kibot/resources/kicad_colors/
+-rw-rw-r--   0 root         (0) root         (0)     6954 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kicad_colors/_builtin_classic.json
+-rw-rw-r--   0 root         (0) root         (0)     7124 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kicad_colors/_builtin_default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.840519 kibot-1.7.0/kibot/resources/kicad_layouts/
+-rw-rw-r--   0 root         (0) root         (0)     2027 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kicad_layouts/default.kicad_wks
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.840519 kibot-1.7.0/kibot/resources/kicanvas/
+-rw-rw-r--   0 root         (0) root         (0)     8636 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kicanvas/kicanvas.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.840519 kibot-1.7.0/kibot/resources/kiri/
+-rw-rw-r--   0 root         (0) root         (0)      486 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/blank.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.844519 kibot-1.7.0/kibot/resources/kiri/images/
+-rw-rw-r--   0 root         (0) root         (0)      310 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/center-to-fit.svg
+-rw-rw-r--   0 root         (0) root         (0)      500 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/circuit-board.svg
+-rw-rw-r--   0 root         (0) root         (0)      893 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/code-branch-solid.svg
+-rw-rw-r--   0 root         (0) root         (0)      194 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/commit.svg
+-rw-rw-r--   0 root         (0) root         (0)     2929 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/icon.svg
+-rw-rw-r--   0 root         (0) root         (0)      301 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/info.svg
+-rw-rw-r--   0 root         (0) root         (0)      410 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/layers-solid.svg
+-rw-rw-r--   0 root         (0) root         (0)      283 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/next-page.svg
+-rw-rw-r--   0 root         (0) root         (0)      240 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/pages.svg
+-rw-rw-r--   0 root         (0) root         (0)      506 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/schematics.svg
+-rw-rw-r--   0 root         (0) root         (0)      224 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/square-solid.svg
+-rw-rw-r--   0 root         (0) root         (0)      269 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/x.svg
+-rw-rw-r--   0 root         (0) root         (0)      279 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/zoom-in.svg
+-rw-rw-r--   0 root         (0) root         (0)      250 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/images/zoom-out.svg
+-rw-rw-r--   0 root         (0) root         (0)    15283 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/index.html
+-rwxrwxr-x   0 root         (0) root         (0)     5545 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/kiri-server
+-rw-rw-r--   0 root         (0) root         (0)    10089 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/kiri.css
+-rw-rw-r--   0 root         (0) root         (0)    45441 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/kiri.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.844519 kibot-1.7.0/kibot/resources/kiri/utils/
+-rw-rw-r--   0 root         (0) root         (0)    83253 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/utils/bootstrap.bundle.min.js
+-rw-rw-r--   0 root         (0) root         (0)   162017 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/utils/bootstrap.min.css
+-rw-rw-r--   0 root         (0) root         (0)    89501 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/utils/jquery-3.6.0.min.js
+-rw-rw-r--   0 root         (0) root         (0)    29768 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/kiri/utils/svg-pan-zoom.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.844519 kibot-1.7.0/kibot/resources/parsers/
+-rw-rw-r--   0 root         (0) root         (0)     7179 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/parsers/electro.lark
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.788519 kibot-1.7.0/kibot/resources/pcbdraw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.788519 kibot-1.7.0/kibot/resources/pcbdraw/present/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.788519 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.848519 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.848519 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/css/
+-rw-rw-r--   0 root         (0) root         (0)     4006 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/css/styles.css
+-rw-rw-r--   0 root         (0) root         (0)     1882 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/index.html
+-rw-rw-r--   0 root         (0) root         (0)    81945 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/package-lock.json
+-rw-rw-r--   0 root         (0) root         (0)      443 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/package.json
+-rw-rw-r--   0 root         (0) root         (0)      358 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/postcss.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.848519 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/src/
+-rw-rw-r--   0 root         (0) root         (0)      819 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/src/styles.css
+-rw-rw-r--   0 root         (0) root         (0)       84 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/tailwind.config.js
+-rw-rw-r--   0 root         (0) root         (0)       62 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.848519 kibot-1.7.0/kibot/resources/pcbdraw/styles/
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/gatema-green.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/jlcpcb-green-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/jlcpcb-green-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/mayer-yellow-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/oshpark-afterdark.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/oshpark-purple.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-black-cu.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-black-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-black-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-blue-cu.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-blue-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-blue-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-red-cu.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-red-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-red-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-white-cu.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-white-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-white-hasl.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-yellow-cu.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-yellow-enig.json
+-rw-rw-r--   0 root         (0) root         (0)      321 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/styles/set-yellow-hasl.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.848519 kibot-1.7.0/kibot/resources/pcbdraw/templates/
+-rw-rw-r--   0 root         (0) root         (0)     1508 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/pcbdraw/templates/simple.handlebars
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.852519 kibot-1.7.0/kibot/resources/report_templates/
+-rw-rw-r--   0 root         (0) root         (0)     3658 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/report_templates/report_full.txt
+-rw-rw-r--   0 root         (0) root         (0)     3658 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/report_templates/report_full_svg.txt
+-rw-rw-r--   0 root         (0) root         (0)     1459 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/resources/report_templates/report_simple.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.852519 kibot-1.7.0/kibot/svgutils/
+-rw-rw-r--   0 root         (0) root         (0)       48 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/svgutils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11209 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/svgutils/compose.py
+-rw-rw-r--   0 root         (0) root         (0)     2048 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/svgutils/templates.py
+-rw-rw-r--   0 root         (0) root         (0)    12513 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/svgutils/transform.py
+-rw-rw-r--   0 root         (0) root         (0)    18208 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/var_base.py
+-rw-rw-r--   0 root         (0) root         (0)     3434 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/var_ibom.py
+-rw-rw-r--   0 root         (0) root         (0)     4981 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/var_kibom.py
+-rw-rw-r--   0 root         (0) root         (0)     3908 2024-04-23 16:14:28.000000 kibot-1.7.0/kibot/var_kicost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.812519 kibot-1.7.0/kibot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11656 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-23 16:16:20.000000 kibot-1.7.0/kibot.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      960 2024-04-23 16:16:20.852519 kibot-1.7.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1621 2024-04-23 16:14:28.000000 kibot-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 16:16:20.852519 kibot-1.7.0/src/
+-rwxrwxr-x   0 root         (0) root         (0)    59962 2024-04-23 16:14:28.000000 kibot-1.7.0/src/kibot-check
```

### Comparing `kibot-1.6.5/LICENSE` & `kibot-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/MANIFEST.in` & `kibot-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/PKG-INFO` & `kibot-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kibot
-Version: 1.6.5
+Version: 1.7.0
 Summary: KiCad automation tool for documents generation
 Home-page: https://github.com/INTI-CMNB/KiBot/
 Author: Salvador E. Tropea, John Beard
 Author-email: stropea@inti.gob.ar
 License: GPL-3.0
 Description: 
         # KiBot (formerly KiPlot)
```

### Comparing `kibot-1.6.5/README.md` & `kibot-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/EasyEDA/easyeda_3d.py` & `kibot-1.7.0/kibot/EasyEDA/easyeda_3d.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/eda_angle.py` & `kibot-1.7.0/kibot/PcbDraw/eda_angle.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/mdrenderer.py` & `kibot-1.7.0/kibot/PcbDraw/mdrenderer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/mistune_shim.py` & `kibot-1.7.0/kibot/PcbDraw/mistune_shim.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/np.py` & `kibot-1.7.0/kibot/PcbDraw/np.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pcbnew_transition.py` & `kibot-1.7.0/kibot/PcbDraw/pcbnew_transition.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/plot.py` & `kibot-1.7.0/kibot/PcbDraw/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # Author: Jan Mrázek
 # License: MIT
 
 from __future__ import annotations
 
+from copy import deepcopy
 import json
 import math
 import os
 import re
 import sysconfig
 import tempfile
 from dataclasses import dataclass, field
@@ -125,23 +126,27 @@
 
     def __str__(self) -> str:
         return f"{self.start} - {self.end} {self.type}"
 
 def matrix(data: List[List[Numeric]]) -> Matrix:
     return np.array(data, dtype=np.float32)
 
-def pseudo_distance(a: Point, b: Point) -> Numeric:
-    return (a[0] - b[0])**2 + (a[1] - b[1])**2
+# def distance(a: Point, b: Point) -> Numeric:
+#     return math.sqrt((a[0] - b[0])**2 + (a[1] - b[1])**2)
 
-def distance(a: Point, b: Point) -> Numeric:
-    return math.sqrt((a[0] - b[0])**2 + (a[1] - b[1])**2)
+def pseudo_distance(a: Point, b: Point) -> Numeric:
+    a0 = a[0] - b[0]
+    a1 = a[1] - b[1]
+    return a0*a0 + a1*a1
 
 def get_closest(reference: Point, elems: List[Point]) -> int:
-    distances = [pseudo_distance(reference, x) for x in elems]
-    return int(np.argmin(distances))
+    try:
+        return elems.index(reference)
+    except ValueError:
+        return int(np.argmin([pseudo_distance(reference, x) for x in elems]))
 
 def extract_arg(args: List[Any], index: int, default: Any=None) -> Any:
     """
     Return n-th element of array or default if out of range
     """
     if index >= len(args):
         return default
@@ -713,25 +718,22 @@
             el = etree.SubElement(layer, "path")
             el.attrib["d"] = hole.get_svg_path_d(self._plotter.ki2svg)
             el.attrib["transform"] = "translate({} {}) rotate({})".format(
                 position[0], position[1], -hole.orientation.AsDegrees())
 
     def _process_baselayer(self, name: str, source_filename: str) -> None:
         clipPath = self._plotter.get_def_slot(tag_name="clipPath", id="cut-off")
-        clipPath.append(
-            get_board_polygon(
-                extract_svg_content(
-                    read_svg_unique(source_filename, self._plotter.unique_prefix()))))
+        board_polygon = get_board_polygon(extract_svg_content(read_svg_unique(source_filename, self._plotter.unique_prefix())))
+        clipPath.append(board_polygon)
         style = self._plotter.get_style(name)
         layer = etree.SubElement(self._container, "g", id="substrate-"+name,
             style="fill:{0}; stroke:{0};".format(style))
-        layer.append(
-            get_board_polygon(
-                extract_svg_content(
-                    read_svg_unique(source_filename, self._plotter.unique_prefix()))))
+        # This call is here just for debug purposes, I want to get the same result as the reference file
+        self._plotter.unique_prefix()
+        layer.append(deepcopy(board_polygon))
         for element in extract_svg_content(read_svg_unique(source_filename, self._plotter.unique_prefix())):
             # Forbidden colors = workaround - KiCAD plots vias white
             # See https://gitlab.com/kicad/code/kicad/-/issues/10491
             if not strip_style_svg(element, keys=["fill", "stroke"],
                                   forbidden_colors=["#ffffff"], new_val=style):
                 layer.append(element)
```

### Comparing `kibot-1.6.5/kibot/PcbDraw/populate.py` & `kibot-1.7.0/kibot/PcbDraw/populate.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/present.py` & `kibot-1.7.0/kibot/PcbDraw/present.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/__init__.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/__init__.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/_compiler.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/_compiler.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/boot.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/boot.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/builder.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/builder.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/grammar.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/grammar.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/pybars/pymeta/runtime.py` & `kibot-1.7.0/kibot/PcbDraw/pybars/pymeta/runtime.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/__init__.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/bezier.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/document.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/misctools.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/parser.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/path.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/paths2svg.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/polytools.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/smoothing.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/svg_io_sax.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PcbDraw/svgpathtools/svg_to_paths.py` & `kibot-1.7.0/kibot/PcbDraw/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/filters.py` & `kibot-1.7.0/kibot/PyPDF2/filters.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/generic.py` & `kibot-1.7.0/kibot/PyPDF2/generic.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/merger.py` & `kibot-1.7.0/kibot/PyPDF2/merger.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/pagerange.py` & `kibot-1.7.0/kibot/PyPDF2/pagerange.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/pdf.py` & `kibot-1.7.0/kibot/PyPDF2/pdf.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/utils.py` & `kibot-1.7.0/kibot/PyPDF2/utils.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/PyPDF2/xmp.py` & `kibot-1.7.0/kibot/PyPDF2/xmp.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/__main__.py` & `kibot-1.7.0/kibot/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,16 @@
     def __init__(self, num, regex=''):
         self.number = num
         self.regex = re.compile(regex)
         self.error = ''
 
 
 def detect_ci_env():
-    return os.path.isfile('/etc/kiauto_tag') or ('GITLAB_CI' in os.environ) or ('GITHUB_RUN_ID' in os.environ)
+    GS.ci_cd_detected = os.path.isfile('/etc/kiauto_tag') or ('GITLAB_CI' in os.environ) or ('GITHUB_RUN_ID' in os.environ)
+    return GS.ci_cd_detected
 
 
 def apply_warning_filter(args):
     if args.no_warn:
         try:
             log.set_filters([SimpleFilter(int(n)) for n in args.no_warn.split(',')])
         except ValueError:
@@ -425,14 +426,16 @@
     # Now we have the debug level set we can check (and optionally inform) KiCad info
     detect_kicad()
     detect_windows()
     debug_arguments(args)
 
     # Force iBoM to avoid the use of graphical stuff
     os.environ['INTERACTIVE_HTML_BOM_NO_DISPLAY'] = 'True'
+    # Tell git that we don't want interactive stuff
+    os.environ['GIT_TERMINAL_PROMPT'] = '0'
 
     # Parse global overwrite options
     parse_global_redef(args)
 
     # Disable auto-download if needed
     if args.no_auto_download:
         dep_downloader.disable_auto_download = True
```

### Comparing `kibot-1.6.5/kibot/banner.py` & `kibot-1.7.0/kibot/banner.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/blender_scripts/blender_export.py` & `kibot-1.7.0/kibot/blender_scripts/blender_export.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/bom.py` & `kibot-1.7.0/kibot/bom/bom.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/bom_writer.py` & `kibot-1.7.0/kibot/bom/bom_writer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/columnlist.py` & `kibot-1.7.0/kibot/bom/columnlist.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/csv_writer.py` & `kibot-1.7.0/kibot/bom/csv_writer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/electro_grammar.py` & `kibot-1.7.0/kibot/bom/electro_grammar.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/html_writer.py` & `kibot-1.7.0/kibot/bom/html_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,79 +8,20 @@
 """
 HTML Writer: Generates a HTML BoM file.
 """
 import os
 from base64 import b64encode
 from .columnlist import ColumnList, BoMError
 from .kibot_logo import KIBOT_LOGO, KIBOT_LOGO_W, KIBOT_LOGO_H
-from ..misc import read_png
+from ..misc import (read_png, STYLE_COMMON, TABLE_MODERN, TABLE_CLASSIC, HEAD_COLOR_R, HEAD_COLOR_R_L, HEAD_COLOR_G,
+                    HEAD_COLOR_G_L, HEAD_COLOR_B, HEAD_COLOR_B_L)
+from .. import log
+logger = log.get_logger()
+
 
-BG_GEN = "#DCF5E4"
-BG_KICAD = "#F5DCA9"
-BG_USER = "#DCEFF5"
-BG_EMPTY = "#F57676"
-BG_GEN_L = "#E6FFEE"
-BG_KICAD_L = "#FFE6B3"
-BG_USER_L = "#E6F9FF"
-BG_EMPTY_L = "#FF8080"
-HEAD_COLOR_R = "#982020"
-HEAD_COLOR_R_L = "#c85050"
-HEAD_COLOR_G = "#009879"
-HEAD_COLOR_G_L = "#30c8a9"
-HEAD_COLOR_B = "#0e4e8e"
-HEAD_COLOR_B_L = "#3e7ebe"
-STYLE_COMMON = (" .cell-title { vertical-align: bottom; }\n"
-                " .cell-info { vertical-align: top; padding: 1em;}\n"
-                " .cell-extra-info { vertical-align: top; padding: 1em;}\n"
-                " .cell-stats { vertical-align: top; padding: 1em;}\n"
-                " .title { font-size:2.5em; font-weight: bold; }\n"
-                " .subtitle { font-size:1.5em; font-weight: bold; }\n"
-                " .h2 { font-size:1.5em; font-weight: bold; }\n"
-                " .td-empty0 { text-align: center; background-color: "+BG_EMPTY+";}\n"
-                " .td-gen0 { text-align: center; background-color: "+BG_GEN+";}\n"
-                " .td-kicad0 { text-align: center; background-color: "+BG_KICAD+";}\n"
-                " .td-user0 { text-align: center; background-color: "+BG_USER+";}\n"
-                " .td-empty1 { text-align: center; background-color: "+BG_EMPTY_L+";}\n"
-                " .td-gen1 { text-align: center; background-color: "+BG_GEN_L+";}\n"
-                " .td-kicad1 { text-align: center; background-color: "+BG_KICAD_L+";}\n"
-                " .td-user1 { text-align: center; background-color: "+BG_USER_L+";}\n"
-                " .color-ref { margin: 25px 0; }\n"
-                " .color-ref th { text-align: left }\n"
-                " .color-ref td { padding: 5px 20px; }\n"
-                " .head-table { margin-bottom: 2em; }\n"
-                # Table sorting cursor. 60% transparent when disabled. Solid white when enabled.
-                " .tg-sort-header::-moz-selection{background:0 0}\n"
-                " .tg-sort-header::selection{background:0 0}.tg-sort-header{cursor:pointer}\n"
-                " .tg-sort-header:after{content:'';float:right;border-width:0 5px 5px;border-style:solid;\n"
-                "                       border-color:#ffffff transparent;visibility:hidden;opacity:.6}\n"
-                " .tg-sort-header:hover:after{visibility:visible}\n"
-                " .tg-sort-asc:after,.tg-sort-asc:hover:after,.tg-sort-desc:after{visibility:visible;opacity:1}\n"
-                " .tg-sort-desc:after{border-bottom:none;border-width:5px 5px 0}\n")
-TABLE_MODERN = """
- .content-table {
-   border-collapse:
-   collapse;
-   margin-top: 5px;
-   margin-bottom: 4em;
-   font-size: 0.9em;
-   font-family: sans-serif;
-   min-width: 400px;
-   border-radius: 5px 5px 0 0;
-   overflow: hidden;
-   box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
- }
- .content-table thead tr { background-color: @bg@; color: #ffffff; text-align: left; }
- .content-table th, .content-table td { padding: 12px 15px; }
- .content-table tbody tr { border-bottom: 1px solid #dddddd; }
- .content-table tbody tr:nth-of-type(even) { background-color: #f3f3f3; }
- .content-table tbody tr:last-of-type { border-bottom: 2px solid @bg@; }
- .content-table * tr:hover > td { background-color: @bgl@ !important }
-"""
-TABLE_CLASSIC = (" .content-table, .content-table th, .content-table td { border: 1px solid black; }\n"
-                 " .content-table * tr:hover > td { background-color: #B0B0B0 !important }\n")
 # JavaScript table sorter. Is floating around internet, i.e.:
 # - Stack Overflow: https://stackoverflow.com/questions/61122696/addeventlistener-after-change-event
 # - pimpmykicadbom: https://gitlab.com/antto/pimpmykicadbom
 # - Table Generator: https://www.tablesgenerator.com/
 SORT_CODE = ('<script charset="utf-8">\n'
              '  var TGSort = window.TGSort || function(n) {\n'
              '    "use strict";\n'
@@ -214,15 +155,15 @@
     for t in ["http", "https", "ftp", "www"]:
         if text.startswith(t):
             return '<a href="{t}">{t}</a>'.format(t=text)
     return text
 
 
 def content_table(html, groups, headings, head_names, cfg, link_datasheet, link_digikey, link_mouser, link_lcsc, col_colors,
-                  dnf=False):
+                  row_colors, dnf=False):
     cl = ''
     # Table start
     html.write('<table class="content-table">\n')
     # Row titles:
     html.write(" <thead>\n")
     html.write("  <tr>\n")
     for i, h in enumerate(head_names):
@@ -235,14 +176,21 @@
 
     html.write(" <tbody>\n")
     rc = 0
     hl_empty = cfg.html.highlight_empty
     for i, group in enumerate(groups):
         if (cfg.ignore_dnf and not group.is_fitted()) != dnf:
             continue
+        # Check if the user wants a color for this row
+        row_color = None
+        for r_color in row_colors:
+            c = group.components[0]
+            if r_color.filter.filter(c):
+                row_color = r_color.color
+                break
         row = group.get_row(headings)
         if link_datasheet != -1:
             datasheet = group.get_field(ColumnList.COL_DATASHEET_L)
         html.write('  <tr id="{}">\n'.format(i))
         for n, r in enumerate(row):
             # A link to Digi-Key?
             if link_digikey and headings[n] in link_digikey:
@@ -257,14 +205,18 @@
             if col_colors:
                 # Empty cell?
                 if hl_empty and (len(r) == 0 or r.strip() == "~"):
                     cl = 'empty'
                 else:
                     cl = cell_class(headings[n])
                 cl = ' class="td-{}{}"'.format(cl, rc % 2)
+            else:
+                cl = ' class="td-nocolor"'
+            if row_color is not None:
+                cl += f' style="background-color: {row_color}"'
             if headings[n] == ColumnList.COL_REFERENCE_L:
                 for ref in r.split(cfg.ref_separator):
                     r = '<div id="{}"></div>'.format(ref)+r
             html.write('   <td{}>{}</td>\n'.format(cl, link(r)))
         html.write("  </tr>\n")
         rc += 1
     html.write(" </tbody>\n")
@@ -371,14 +323,15 @@
     link_datasheet = -1
     if cfg.html.datasheet_as_link and cfg.html.datasheet_as_link in headings:
         link_datasheet = headings.index(cfg.html.datasheet_as_link)
     link_digikey = cfg.html.digikey_link
     link_mouser = cfg.html.mouser_link
     link_lcsc = cfg.html.lcsc_link
     col_colors = cfg.html.col_colors
+    row_colors = cfg.html.row_colors
     # Compute the CSS
     style_name = cfg.html.style
     if os.path.isfile(style_name):
         with open(style_name, 'rt') as f:
             style = f.read()
     else:
         # Common stuff
@@ -444,30 +397,38 @@
             write_extra_info(html, cfg)
             write_stats(html, cfg)
             html.write('</table>\n')
 
         # Fitted groups
         html.write("<h2>Component Groups</h2>\n")
         content_table(html, groups, headings, head_names, cfg, link_datasheet, link_digikey, link_mouser, link_lcsc,
-                      col_colors)
+                      col_colors, row_colors)
 
         # DNF component groups
         if cfg.html.generate_dnf and cfg.n_total != cfg.n_fitted:
             html.write("<h2>Optional components (DNF=Do Not Fit)</h2>\n")
             content_table(html, groups, headings, head_names, cfg, link_datasheet, link_digikey, link_mouser, link_lcsc,
-                          col_colors, True)
+                          col_colors, row_colors, True)
 
         # Color reference
         if col_colors:
             html.write('<table class="color-ref">\n')
-            html.write('<tr><th>Color reference:</th></tr>\n')
+            html.write('<tr><th>Color reference for columns:</th></tr>\n')
             html.write('<tr><td class="td-kicad0">KiCad Fields (default)</td></tr>\n')
             html.write('<tr><td class="td-gen0">Generated Fields</td></tr>\n')
             html.write('<tr><td class="td-user0">User Fields</td></tr>\n')
             if cfg.html.highlight_empty:
                 html.write('<tr><td class="td-empty0">Empty Fields</td></tr>\n')
             html.write('</table>\n')
 
+        if row_colors:
+            html.write('<table class="color-ref">\n')
+            html.write('<tr><th>Color reference for rows:</th></tr>\n')
+            for r_color in row_colors:
+                html.write('<tr><td style="background-color: '
+                           f'{r_color.color}">{r_color.description}</td></tr>\n')
+            html.write('</table>\n')
+
         html.write(SORT_CODE)
         html.write("</body></html>")
 
     return True
```

### Comparing `kibot-1.6.5/kibot/bom/units.py` & `kibot-1.7.0/kibot/bom/units.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/bom/xlsx_writer.py` & `kibot-1.7.0/kibot/bom/xlsx_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,22 @@
         for _ in col_fields:
             col_fmt.append(fmt_cols[0])
     # Empty color
     col_fmt.append(fmt_cols[-1])
     return col_fmt
 
 
+def create_row_fmt(workbook, row_colors):
+    """ Assign a color to each highlighted row """
+    for r in row_colors:
+        fmt = workbook.add_format(DEFAULT_FMT)
+        fmt.set_bg_color(r.color)
+        r.xlsx_fmt = fmt
+
+
 def create_fmt_info(workbook, cfg):
     """ Formats for the PCB and stats info """
     if cfg.xlsx.hide_pcb_info and cfg.xlsx.hide_stats_info and not cfg.xlsx.extra_info:
         return None
     # Data left justified
     fmt_data = workbook.add_format({'align': 'left'})
     fmt_name = workbook.add_format(DEFAULT_FMT)
@@ -235,32 +243,45 @@
                    'object_position': 1,
                    'decorative': True}
         worksheet.insert_image('A1', 'logo.png', options)
         return 2
     return 0
 
 
-def create_color_ref(workbook, col_colors, hl_empty, fmt_cols, do_kicost, kicost_colors):
+def create_color_ref(workbook, col_colors, hl_empty, fmt_cols, do_kicost, kicost_colors, row_colors):
     if not (col_colors or do_kicost):
         return
     row = 0
     worksheet = workbook.add_worksheet('Colors')
-    worksheet.set_column(0, 0, 50)
+    max_w = 50
     if col_colors:
-        worksheet.write_string(0, 0, 'KiCad Fields (default)', fmt_cols[1][0])
-        worksheet.write_string(1, 0, 'Generated Fields', fmt_cols[0][0])
-        worksheet.write_string(2, 0, 'User Fields', fmt_cols[2][0])
-        if hl_empty:
-            worksheet.write_string(3, 0, 'Empty Fields', fmt_cols[3][0])
+        worksheet.write_string(0, 0, 'Columns colors')
+        worksheet.write_string(1, 0, 'KiCad Fields (default)', fmt_cols[1][0])
+        worksheet.write_string(2, 0, 'Generated Fields', fmt_cols[0][0])
+        worksheet.write_string(3, 0, 'User Fields', fmt_cols[2][0])
         row = 5
+        if hl_empty:
+            worksheet.write_string(4, 0, 'Empty Fields', fmt_cols[3][0])
+            row = 6
+        max_w = 22
+    if row_colors:
+        worksheet.write_string(row, 0, 'Row colors')
+        row += 1
+        for r in row_colors:
+            worksheet.write_string(row, 0, r.description, r.xlsx_fmt)
+            max_w = max(max_w, len(r.description))
+            row += 1
+        row += 1
     if do_kicost:
-        worksheet.write_string(row, 0, 'Costs sheet')
+        worksheet.write_string(row, 0, 'Costs sheet colors')
         for label, format in kicost_colors.items():
             row += 1
             worksheet.write_string(row, 0, label, format)
+            max_w = max(max_w, len(label))
+    worksheet.set_column(0, 0, max_w)
 
 
 def get_spec(part, name):
     if name[0] != '_':
         return part.specs.get(name, ['', ''])
     name = name[1:]
     for v in part.dd.values():
@@ -748,14 +769,15 @@
     # #######################
     # Headings
     # Column names format
     fmt_head = create_fmt_head(workbook, cfg.xlsx.style)
     # Column formats
     fmt_cols = create_fmt_cols(workbook, cfg.xlsx.col_colors)
     col_fmt = create_col_fmt(col_fields, cfg.xlsx.col_colors, fmt_cols)
+    create_row_fmt(workbook, cfg.xlsx.row_colors)
     # Page head
     # Logo
     image_data = get_logo_data(cfg.xlsx.logo)
     # Title
     fmt_title = create_fmt_title(workbook, cfg.xlsx.title)
     fmt_subtitle = create_fmt_subtitle(workbook)
     # Info
@@ -792,18 +814,27 @@
             if (cfg.ignore_dnf and not group.is_fitted()) != dnf:
                 continue
             # Get the data row
             row = group.get_row(col_fields)
             rows.append(row)
             if link_datasheet != -1:
                 datasheet = group.get_field(ColumnList.COL_DATASHEET_L)
+            # Check if the user wants a color for this row
+            row_fmt = None
+            for r_color in cfg.xlsx.row_colors:
+                c = group.components[0]
+                if r_color.filter.filter(c):
+                    row_fmt = r_color.xlsx_fmt
+                    break
             # Fill the row
             for i in range(len(row)):
                 cell = row[i]
-                if hl_empty and (len(cell) == 0 or cell.strip() == "~"):
+                if row_fmt is not None:
+                    fmt = row_fmt
+                elif hl_empty and (len(cell) == 0 or cell.strip() == "~"):
                     fmt = col_fmt[-1][row_count % 2]
                 else:
                     fmt = col_fmt[i][row_count % 2]
                 # Link this column to the datasheet?
                 if link_datasheet == i and datasheet.startswith('http'):
                     worksheet.write_url(row_count, i, datasheet, fmt, cell)
                 # A link to Digi-Key?
@@ -843,12 +874,13 @@
 
     # Optionally add KiCost information
     kicost_colors = None
     if cfg.xlsx.kicost:
         kicost_colors = create_kicost_sheet(workbook, groups, image_data, fmt_title, fmt_info, fmt_subtitle, fmt_head,
                                             fmt_cols, cfg)
     # Add a sheet for the color references
-    create_color_ref(workbook, cfg.xlsx.col_colors, hl_empty, fmt_cols, cfg.xlsx.kicost and KICOST_SUPPORT, kicost_colors)
+    create_color_ref(workbook, cfg.xlsx.col_colors, hl_empty, fmt_cols, cfg.xlsx.kicost and KICOST_SUPPORT, kicost_colors,
+                     cfg.xlsx.row_colors)
 
     workbook.close()
 
     return True
```

### Comparing `kibot-1.6.5/kibot/bom/xml_writer.py` & `kibot-1.7.0/kibot/bom/xml_writer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/config_reader.py` & `kibot-1.7.0/kibot/config_reader.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/create_pdf.py` & `kibot-1.7.0/kibot/create_pdf.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/dep_downloader.py` & `kibot-1.7.0/kibot/dep_downloader.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/docopt.py` & `kibot-1.7.0/kibot/docopt.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/drill_marks.py` & `kibot-1.7.0/kibot/drill_marks.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_base.py` & `kibot-1.7.0/kibot/fil_base.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_expand_text_vars.py` & `kibot-1.7.0/kibot/fil_expand_text_vars.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_field_modify.py` & `kibot-1.7.0/kibot/fil_field_modify.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_field_rename.py` & `kibot-1.7.0/kibot/fil_field_rename.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_generic.py` & `kibot-1.7.0/kibot/fil_generic.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_rot_footprint.py` & `kibot-1.7.0/kibot/fil_rot_footprint.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_spec_to_field.py` & `kibot-1.7.0/kibot/fil_spec_to_field.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_subparts.py` & `kibot-1.7.0/kibot/fil_subparts.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_urlify.py` & `kibot-1.7.0/kibot/fil_urlify.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_value_split.py` & `kibot-1.7.0/kibot/fil_value_split.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/fil_var_rename.py` & `kibot-1.7.0/kibot/var_ibom.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020-2021 Salvador E. Tropea
-# Copyright (c) 2020-2021 Instituto Nacional de Tecnología Industrial
+# Copyright (c) 2020 Salvador E. Tropea
+# Copyright (c) 2020 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
-# Description: Implements the VARIANT:FIELD=VALUE renamer to get FIELD=VALUE when VARIANT is in use.
+# Description: Implements the IBoM variants mechanism.
+from .optionable import Optionable
 from .gs import GS
-from .macros import macros, document, filter_class  # noqa: F401
+from .misc import IFILT_MECHANICAL
+from .fil_base import BaseFilter
+from .macros import macros, document, variant_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
 
 
-@filter_class
-class Var_Rename(BaseFilter):  # noqa: F821
-    """ Variant Renamer
-        This filter implements the VARIANT:FIELD=VALUE renamer to get FIELD=VALUE when VARIANT is in use """
+@variant_class
+class IBoM(BaseVariant):  # noqa: F821
+    """ IBoM variant style
+        The Config field (configurable) contains a value.
+        If this value matches with a value in the whitelist is included.
+        If this value matches with a value in the blacklist is excluded """
     def __init__(self):
         super().__init__()
-        self._is_transform = True
         with document:
-            self.separator = ':'
-            """ Separator used between the variant and the field name """
-            self.variant_to_value = False
-            """ Rename fields matching the variant to the value of the component """
-            self.force_variant = ''
-            """ Use this variant instead of the current variant. Useful for IBoM variants """
+            self.variant_field = 'Config'
+            """ Name of the field that stores board variant for component """
+            self.variants_blacklist = Optionable
+            """ [string|list(string)=''] List of board variants to exclude from the BOM """
+            self.variants_whitelist = Optionable
+            """ [string|list(string)=''] List of board variants to include in the BOM """
+
+    def get_variant_field(self):
+        """ Returns the name of the field used to determine if the component belongs to the variant """
+        return self.variant_field
 
     def config(self, parent):
         super().config(parent)
-        if not self.separator:
-            self.separator = ':'
+        self.pre_transform = BaseFilter.solve_filter(self.pre_transform, 'pre_transform', is_transform=True)
+        self.exclude_filter = BaseFilter.solve_filter(self.exclude_filter, 'exclude_filter', IFILT_MECHANICAL)
+        self.dnf_filter = BaseFilter.solve_filter(self.dnf_filter, 'dnf_filter')
+        self.dnc_filter = BaseFilter.solve_filter(self.dnc_filter, 'dnc_filter')
+        self.variants_blacklist = self.force_list(self.variants_blacklist)
+        self.variants_whitelist = self.force_list(self.variants_whitelist)
+
+    def skip_component(self, c):
+        """ Skip components that doesn't belong to this variant. """
+        # Apply variants white/black lists
+        if self.variant_field:
+            ref_variant = c.get_field_value(self.variant_field).lower()
+            # skip components with wrong variant field
+            if self.variants_whitelist and ref_variant not in self.variants_whitelist:
+                return True
+            if self.variants_blacklist and ref_variant and ref_variant in self.variants_blacklist:
+                return True
+        return False
 
-    def filter(self, comp):
-        """ Look for fields containing VARIANT:FIELD used to change fields according to the variant """
-        if self.force_variant:
-            variants = [self.force_variant]
-        else:
-            variants = GS.variant
-            if not variants:
-                # No variant in use, nothing to do
-                return
-        for variant in variants:
-            for name, value in comp.get_user_fields():
-                res = name.strip().split(self.separator)
-                if len(res) == 2:
-                    f_variant = res[0].lower()
-                    f_field = res[1].lower()
-                    if f_variant == variant:
-                        if GS.debug_level > 2:
-                            logger.debug('ref: {} {}: {} -> {}'.
-                                         format(comp.ref, f_field, comp.get_field_value(f_field), value))
-                        comp.set_field(f_field, value)
-                elif self.variant_to_value and name.lower() == variant:
-                    if GS.debug_level > 2:
-                        logger.debug('ref: {} value: {} -> {}'.format(comp.ref, comp.value, value))
-                    comp.set_field('value', value)
+    def filter(self, comps):
+        GS.variant = self.variants_whitelist
+        comps = super().filter(comps)
+        logger.debug("Applying IBoM style variants `{}`".format(self.name))
+        # Make black/white lists case insensitive
+        self.variants_whitelist = [v.lower() for v in self.variants_whitelist]
+        self.variants_blacklist = [v.lower() for v in self.variants_blacklist]
+        # Apply to all the components
+        for c in comps:
+            logger.debug("{} {} {}".format(c.ref, c.fitted, c.included))
+            if not (c.fitted and c.included):
+                # Don't check if we already discarded it
+                continue
+            c.fitted = not self.skip_component(c)
+            if not c.fitted and GS.debug_level > 2:
+                logger.debug('ref: {} value: {} -> False'.format(c.ref, c.value))
+        return comps
```

### Comparing `kibot-1.6.5/kibot/fil_var_rename_kicost.py` & `kibot-1.7.0/kibot/fil_var_rename_kicost.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020-2021 Salvador E. Tropea
-# Copyright (c) 2020-2021 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2020-2024 Salvador E. Tropea
+# Copyright (c) 2020-2024 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 # The algorithm is from KiCost project (https://github.com/xesscorp/KiCost)
 # Description: Implements the kicost.VARIANT:FIELD=VALUE renamer to get FIELD=VALUE when VARIANT is in use.
 #              It applies the KiCost concept of variants (a regex to match the VARIANT)
 #              Can be configured, by default is what KiCost does.
 import re
 from .gs import GS
@@ -16,15 +16,22 @@
 
 
 @filter_class
 class Var_Rename_KiCost(BaseFilter):  # noqa: F821
     """ Variant Renamer KiCost style
         This filter implements the kicost.VARIANT:FIELD=VALUE renamer to get FIELD=VALUE when VARIANT is in use.
         It applies the KiCost concept of variants (a regex to match the VARIANT).
-        The internal `_var_rename_kicost` filter emulates the KiCost behavior """
+        As an example: a field named *kicost.V1:MPN* with value *1N4001* will change the field *MPN* to be
+        *1N4001* when a variant in use matches the *V1* string.
+        Note that this mechanism can be used to change a footprint, i.e. *kicost.VARIANT:Footprint* assigned
+        with *Diode_SMD:D_0805_2012Metric* will change the footprint when *VARIANT* is matched. Of course the
+        footprints should be similar, or your PCB will become invalid.
+        The internal `_var_rename_kicost` filter is configured to emulate the KiCost behavior. You can create
+        other filters to fine-tune the behavior, i.e. you can make the mechanism to be triggered by fields
+        like *kibot.VARIANT|FIELD* """
     def __init__(self):
         super().__init__()
         self._is_transform = True
         with document:
             self.prefix = 'kicost.'
             """ A mandatory prefix. Is not case sensitive """
             self.separator = ':'
@@ -71,16 +78,20 @@
                 # Successfully separated
                 f_variant = res[0].lower()
                 f_field = res[1].lower()
                 if GS.debug_level > 3:
                     logger.debug(' Checking `{}` | `{}`'.format(f_variant, f_field))
                 if var_re.match(f_variant):
                     # Variant matched
+                    old_value = comp.get_field_value(f_field)
                     if GS.debug_level > 2:
                         logger.debug(' ref: {} {}: {} -> {}'.
-                                     format(comp.ref, f_field, comp.get_field_value(f_field), value))
+                                     format(comp.ref, f_field, old_value, value))
                     comp.set_field(f_field, value)
+                    if f_field == 'footprint' and old_value != value:
+                        # Ok, this is crazy, but we can change the footprint
+                        comp._footprint_variant = True
             elif self.variant_to_value and var_re.match(name):
                 # The field matches the variant and the user wants to change the value
                 if GS.debug_level > 2:
                     logger.debug(' ref: {} value: {} -> {}'.format(comp.ref, comp.value, value))
                 comp.set_field('value', value)
```

### Comparing `kibot-1.6.5/kibot/globals.py` & `kibot-1.7.0/kibot/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,16 +268,16 @@
                 Read `solder_mask_color` help """
             self.time_format = '%H-%M-%S'
             """ Format used for the time we started the script. Uses the `strftime` format """
             self.time_reformat = True
             """ Tries to reformat the PCB/SCH date using the `date_format`.
                 This assumes you let KiCad fill this value and hence the time is in ISO format (YY-MM-DD) """
             self.units = ''
-            """ [millimeters,inches,mils] Default units. Affects `position`, `bom` and `panelize` outputs.
-                Also KiCad 6 dimensions """
+            """ [millimeters,inches,mils] Default units. Affects `position`, `bom` and `panelize` outputs and
+                the `erc` and `drc` preflights. Also KiCad 6 dimensions """
             self.use_dir_for_preflights = True
             """ Use the global `dir` as subdir for the preflights """
             self.variant = ''
             """ Default variant to apply to all outputs """
             self.out_dir = ''
             """ Base output dir, same as command line `--out-dir` """
             self.environment = Environment
@@ -357,14 +357,18 @@
                 Note that the name for the layer must match exactly, no aliases """
             self.include_components_from_pcb = True
             """ Include components that are only in the PCB, not in the schematic, for filter and variants processing.
                 Note that version 1.6.3 and older ignored them """
             self.allow_component_ranges = True
             """ Allow using ranges like *R5-R20* in the `show_components` and `highlight` options.
                 If you have references that looks like a range you should disable this option """
+            self.str_yes = 'yes'
+            """ String used for *yes*. Currently used by the **update_pcb_characteristics** preflight """
+            self.str_no = 'no'
+            """ String used for *no*. Currently used by the **update_pcb_characteristics** preflight """
         self.set_doc('filters', " [list(dict)] KiBot warnings to be ignored ")
         self._filter_what = 'KiBot warnings'
         self.filters = FilterOptionsKiBot
         self._unknown_is_error = True
         self._error_context = 'global '
 
     def set_global(self, opt):
```

### Comparing `kibot-1.6.5/kibot/gs.py` & `kibot-1.7.0/kibot/gs.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     class pcbnew(object):
         IU_PER_MM = 1
         IU_PER_MILS = 1
 from datetime import datetime
 import shlex
 from shutil import copy2
 from sys import exit, exc_info
+import tempfile
 from traceback import extract_stack, format_list, print_tb
 from .misc import EXIT_BAD_ARGS, W_DATEFORMAT, W_UNKVAR, WRONG_INSTALL, CORRUPTED_PRO
 from .log import get_logger
 
 logger = get_logger(__name__)
 if hasattr(pcbnew, 'IU_PER_MM'):
     IU_PER_MM = pcbnew.IU_PER_MM
@@ -71,15 +72,17 @@
     pro_fname = None     # file.kicad_pro (or .pro)
     pro_ext = '.pro'
     pro_variables = None  # KiCad 6 text variables defined in the project
     vars_regex = re.compile(r'\$\{([^\}]+)\}')
     # Main output dir
     out_dir = None
     out_dir_in_cmd_line = False
+    # Content of the "filters" preflight
     filter_file = None
+    filters = None
     board = None
     sch = None
     debug_enabled = False
     debug_level = 0
     kibot_version = None
     n = datetime.now()
     on_windows = False
@@ -116,14 +119,15 @@
     test_number = 5
     stackup = None
     # Preprocessor definitions
     cli_defines = {}
     kikit_units_to_kicad = {'mm': IU_PER_MM, 'cm': 10*IU_PER_MM, 'dm': 100*IU_PER_MM,
                             'm': 1000*IU_PER_MM, 'mil': IU_PER_MILS, 'inch': 1000*IU_PER_MILS,
                             'in': 1000*IU_PER_MILS}
+    ci_cd_detected = False
     # Maximum recursive replace
     MAXDEPTH = 20
     #
     # Global defaults
     #
     # Options from command line
     cli_global_defs = {}
@@ -181,14 +185,16 @@
     global_set_text_variables_before_output = None
     global_silk_screen_color = None
     global_silk_screen_color_bottom = None
     global_silk_screen_color_top = None
     global_solder_mask_color = None
     global_solder_mask_color_bottom = None
     global_solder_mask_color_top = None
+    global_str_yes = None
+    global_str_no = None
     global_time_format = None
     global_time_reformat = None
     global_units = None
     global_use_dir_for_preflights = None
     global_use_os_env_for_expand = None
     global_variant = None
     # Only for v7+
@@ -387,26 +393,40 @@
         if units == 'millimeters':
             return 1.0/IU_PER_MM
         if units == 'mils':
             return 1.0/IU_PER_MILS
         # Inches
         return 0.001/IU_PER_MILS
 
+#     @staticmethod
+#     def unit_name_to_abrev(units):
+#         if units == 'millimeters':
+#             return 'mm'
+#         if units == 'mils':
+#             return 'mils'
+#         # Inches
+#         return 'in'
+
     @staticmethod
     def to_mm(val):
         return float(val)/IU_PER_MM
 
     @staticmethod
     def from_mm(val):
         return int(val*IU_PER_MM)
 
     @staticmethod
     def to_mils(val):
         return val/IU_PER_MILS
 
+#     @staticmethod
+#     def to_global_units(val):
+#         scale = GS.unit_name_to_scale_factor(GS.global_units)
+#         return str(val*scale)+' '+GS.unit_name_to_abrev(GS.global_units)
+
     @staticmethod
     def make_bkp(fname):
         bkp = fname+'-bak'
         os.replace(fname, bkp)
 
     @staticmethod
     def zones():
@@ -886,7 +906,75 @@
         if GS.ki8:  # 8
             return obj.GetShownText(allow_extra_text, a_depth)
         if GS.ki7:  # 7
             return obj.GetShownText()
         if GS.ki6:  # 6
             return obj.GetShownText(a_depth, allow_extra_text)
         return obj.GetShownText()  # 5
+
+    @staticmethod
+    def compute_group_boundary(g):
+        x1 = y1 = x2 = y2 = None
+        for item in g.GetItems():
+            bb = GS.get_shape_bbox(item) if hasattr(item, 'GetWidth') else item.GetBoundingBox()
+            start = bb.GetOrigin()
+            end = bb.GetEnd()
+            if x1 is None:
+                x1 = x2 = start.x
+                y1 = y2 = start.y
+            for p in [start, end]:
+                x2 = max(x2, p.x)
+                y2 = max(y2, p.y)
+                x1 = min(x1, p.x)
+                y1 = min(y1, p.y)
+        return x1, y1, x2, y2
+
+    @staticmethod
+    def compute_pcb_boundary(board):
+        edge_layer = board.GetLayerID('Edge.Cuts')
+        x1 = y1 = x2 = y2 = None
+        for d in board.GetDrawings():
+            if d.GetClass() == GS.board_gr_type and d.GetLayer() == edge_layer:
+                bb = GS.get_shape_bbox(d)
+                start = bb.GetOrigin()
+                end = bb.GetEnd()
+                if x1 is None:
+                    x1 = x2 = start.x
+                    y1 = y2 = start.y
+                for p in [start, end]:
+                    x2 = max(x2, p.x)
+                    y2 = max(y2, p.y)
+                    x1 = min(x1, p.x)
+                    y1 = min(y1, p.y)
+        # This is a special case: the PCB edges are in a footprint
+        for m in GS.get_modules():
+            for gi in m.GraphicalItems():
+                if gi.GetClass() == GS.footprint_gr_type and gi.GetLayer() == edge_layer:
+                    bb = GS.get_shape_bbox(gi)
+                    start = bb.GetOrigin()
+                    end = bb.GetEnd()
+                    if x1 is None:
+                        x1 = x2 = start.x
+                        y1 = y2 = start.y
+                    for p in [start, end]:
+                        x2 = max(x2, p.x)
+                        y2 = max(y2, p.y)
+                        x1 = min(x1, p.x)
+                        y1 = min(y1, p.y)
+        return x1, y1, x2, y2
+
+    @staticmethod
+    def tmp_file(content=None, prefix=None, suffix=None, dir=None, what=None, a_logger=None, binary=False, indent=False):
+        mode = 'wb' if binary else 'wt'
+        prefix = 'kibot_'+(prefix if prefix is not None else '')
+        with tempfile.NamedTemporaryFile(mode=mode, delete=False, suffix=suffix, prefix=prefix, dir=dir) as f:
+            if what is not None:
+                if a_logger is None:
+                    a_logger = logger
+                a_logger.debug(('- ' if indent else '')+f'Writing {what} to {f.name}')
+            if content:
+                f.write(content)
+        return f.name
+
+    @staticmethod
+    def mkdtemp(mod):
+        return tempfile.mkdtemp(prefix='tmp-kibot-'+mod+'-')
```

### Comparing `kibot-1.6.5/kibot/kicad/color_theme.py` & `kibot-1.7.0/kibot/kicad/color_theme.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/kicad/config.py` & `kibot-1.7.0/kibot/kicad/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 - kicad_common to know about the 'environment' variables
 - The `sym-lib-table` files to map library aliases
 
 Notes about coverage:
 I'm excluding all the Darwin and Windows code from coverage.
 I'm not even sure the values are correct.
 """
+import atexit
 import csv
 from glob import glob
 from io import StringIO
 import json
 import os
 import platform
 import re
 from shutil import copy2
 import sys
 import sysconfig
 from ..error import KiPlotConfigurationError
 from ..gs import GS
 from .. import log
 from ..misc import (W_NOCONFIG, W_NOKIENV, W_NOLIBS, W_NODEFSYMLIB, MISSING_WKS, W_MAXDEPTH, W_3DRESVER, W_LIBTVERSION,
-                    W_LIBTUNK)
+                    W_LIBTUNK, W_MISLIBTAB)
 from .sexpdata import load, SExpData, Symbol, dumps, Sep
 from .sexp_helpers import _check_is_symbol_list, _check_integer, _check_relaxed
 
 # Check python version to determine which version of ConfirParser to import
 if sys.version_info.major >= 3:
     import configparser as ConfigParser
 else:  # pragma: no cover (Py2)
@@ -543,14 +544,44 @@
         if KiConf.fp_aliases is None:
             if fname is None:
                 fname = GS.pcb_file
             KiConf.init(fname)
             KiConf.fp_aliases = KiConf.load_all_lib_aliases(FP_LIB_TABLE, KiConf.footprint_dir, '*.pretty')
         return KiConf.fp_aliases
 
+    def check_fp_lib_table(fname=None):
+        if fname is None:
+            fname = GS.pcb_file
+        KiConf.check_lib_table(fname, FP_LIB_TABLE)
+
+    def check_sym_lib_table(fname=None):
+        if fname is None:
+            fname = GS.sch_file
+        KiConf.check_lib_table(fname, SYM_LIB_TABLE)
+
+    def check_lib_table(fname, table_name):
+        KiConf.init(fname)
+        if KiConf.config_dir:
+            fp_name = os.path.join(KiConf.config_dir, table_name)
+            if not os.path.isfile(fp_name):
+                # No global fp lib table
+                global_fp_name = os.path.join(KiConf.template_dir, table_name) if KiConf.template_dir else None
+                if global_fp_name and os.path.isfile(global_fp_name):
+                    # Try to copy the template
+                    if not GS.ci_cd_detected:
+                        logger.warning(f'{W_MISLIBTAB}Missing default system symbol table {table_name}, copying the template')
+                    logger.debug(f'Copying {global_fp_name} to {fp_name}')
+                    copy2(global_fp_name, fp_name)
+                    atexit.register(KiConf.remove_lib_table, fp_name)
+
+    def remove_lib_table(fname):
+        if os.path.isfile(fname):
+            logger.debug('Removing '+fname)
+            os.remove(fname)
+
     def save_fp_lib_aliases(fname, aliases, is_fp=True):
         logger.debug(f'Writing lib table `{fname}`')
         table = [Symbol('fp_lib_table' if is_fp else 'sym_lib_table'), Sep()]
         for name in sorted(aliases.keys(), key=str.casefold):
             alias = aliases[name]
             cnt = [[Symbol('name'), alias.name],
                    [Symbol('type'), alias.type],
@@ -590,93 +621,110 @@
                 name = parse_len_str(r[0])
                 value = parse_len_str(r[1])
                 # Discard the comment (2)
                 logger.debugl(1, '- {}={}'.format(name, value))
                 KiConf.aliases_3D[name] = value
         logger.debugl(1, 'Finished loading 3D aliases')
 
-    def fix_page_layout_k6_key(key, data, dest_dir):
+    def fix_page_layout_k6_key(key, data, dest_dir, forced):
         if key in data:
             section = data[key]
             pl = section.get('page_layout_descr_file', None)
             if pl:
-                fname = KiConf.expand_env(pl)
-                if os.path.isfile(fname):
-                    dest = os.path.join(dest_dir, key+'.kicad_wks')
-                    logger.debug('Copying {} -> {}'.format(fname, dest))
-                    copy2(fname, dest)
-                    data[key]['page_layout_descr_file'] = key+'.kicad_wks'
-                    return dest
+                if forced:
+                    data[key]['page_layout_descr_file'] = forced
+                    logger.debug(f'Replacing page layout {pl} -> {forced}')
                 else:
-                    GS.exit_with_error('Missing page layout file: '+fname, MISSING_WKS)
+                    fname = KiConf.expand_env(pl)
+                    if os.path.isfile(fname):
+                        dest = os.path.join(dest_dir, key+'.kicad_wks')
+                        logger.debug('Copying {} -> {}'.format(fname, dest))
+                        copy2(fname, dest)
+                        data[key]['page_layout_descr_file'] = key+'.kicad_wks'
+                        logger.debug(f'Replacing page layout {pl} -> {key}.kicad_wks')
+                        return dest
+                    else:
+                        GS.exit_with_error('Missing page layout file: '+fname, MISSING_WKS)
         return None
 
-    def fix_page_layout_k6(project, dry):
+    def fix_page_layout_k6(project, dry, force_sch, force_pcb):
         # Get the current definitions
         dest_dir = os.path.dirname(project)
         with open(project, 'rt') as f:
             pro_text = f.read()
         data = json.loads(pro_text)
         layouts = [None, None]
         if not dry:
-            layouts[1] = KiConf.fix_page_layout_k6_key('pcbnew', data, dest_dir)
-            layouts[0] = KiConf.fix_page_layout_k6_key('schematic', data, dest_dir)
+            layouts[1] = KiConf.fix_page_layout_k6_key('pcbnew', data, dest_dir, force_pcb)
+            layouts[0] = KiConf.fix_page_layout_k6_key('schematic', data, dest_dir, force_sch)
+            logger.debug(f'Saving modified project to {project}')
             with open(project, 'wt') as f:
                 f.write(json.dumps(data, sort_keys=True, indent=2))
         else:
             aux = data.get('schematic', None)
             if aux:
                 layouts[0] = KiConf.expand_env(aux.get('page_layout_descr_file', None), ref_dir=dest_dir)
             aux = data.get('pcbnew', None)
             if aux:
                 layouts[1] = KiConf.expand_env(aux.get('page_layout_descr_file', None), ref_dir=dest_dir)
         return layouts
 
-    def fix_page_layout_k5(project, dry):
+    def fix_page_layout_k5(project, dry, force_sch, force_pcb):
         order = 1
         dest_dir = os.path.dirname(project)
         with open(project, 'rt') as f:
             lns = f.readlines()
         is_pcb_new = False
         layouts = [None, None]
         for c, line in enumerate(lns):
             if line.startswith('[pcbnew]'):
                 is_pcb_new = True
             if line.startswith('[schematic'):
                 is_pcb_new = False
             if line.startswith('PageLayoutDescrFile='):
                 fname = line[20:].strip()
-                if fname:
+                if force_sch and not is_pcb_new:
+                    dest = force_sch
+                elif force_pcb and is_pcb_new:
+                    dest = force_pcb
+                elif fname:
                     fname = KiConf.expand_env(fname)
                     if os.path.isfile(fname):
                         dest = os.path.join(dest_dir, str(order)+'.kicad_wks')
                         if not dry:
                             copy2(fname, dest)
                             layouts[is_pcb_new] = dest
                         else:
                             layouts[is_pcb_new] = fname
                         dest = str(order)+'.kicad_wks'
                         order = order+1
                     else:
                         GS.exit_with_error('Missing page layout file: '+fname, MISSING_WKS)
                 else:
                     dest = ''
+                if dest or fname:
+                    logger.debug(f'Replacing page layout {fname} -> {dest}')
                 lns[c] = f'PageLayoutDescrFile={dest}\n'
         if not dry:
+            logger.debug(f'Saving modified project to {project}')
             with open(project, 'wt') as f:
                 lns = f.writelines(lns)
         return layouts
 
-    def fix_page_layout(project, dry=False):
+    def fix_page_layout(project, dry=False, force_sch=None, force_pcb=None):
+        """ When we copy the project the page layouts must be also copied.
+            After copying the project to another destination we have wrong relative references to the WKSs.
+            We copy these files and patch the project so the files are named in a simple way.
+            In addition we can use this function to force the names of the page layouts. """
         if not project:
             return None, None
-        KiConf.init(GS.pcb_file)
+        KiConf.init(GS.pcb_file or GS.sch_file)
         if GS.ki5:
-            return KiConf.fix_page_layout_k5(project, dry)
-        return KiConf.fix_page_layout_k6(project, dry)
+            return KiConf.fix_page_layout_k5(project, dry, force_sch, force_pcb)
+        return KiConf.fix_page_layout_k6(project, dry, force_sch, force_pcb)
 
     def expand_env(name, used_extra=None, ref_dir=None):
         if used_extra is None:
             used_extra = [False]
         if not name:
             return name
         expanded = expand_env(un_quote(name), KiConf.kicad_env, GS.load_pro_variables(), used_extra)
```

### Comparing `kibot-1.6.5/kibot/kicad/error.py` & `kibot-1.7.0/kibot/kicad/error.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/kicad/patch_svg.py` & `kibot-1.7.0/kibot/kicad/patch_svg.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/kicad/sexp_helpers.py` & `kibot-1.7.0/kibot/kicad/sexp_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2021-2023 Salvador E. Tropea
-# Copyright (c) 2021-2023 Instituto Nacional de Tecnología Industrial
+# Copyright (c) 2021-2024 Salvador E. Tropea
+# Copyright (c) 2021-2024 Instituto Nacional de Tecnología Industrial
 # License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 from .error import SchError
-from .sexpdata import Symbol
+from ..error import KiPlotConfigurationError
+from .sexpdata import Symbol, Sep, SExpData, load
+TO_SEPARATE = {'kicad_pcb', 'general', 'title_block', 'layers', 'setup', 'pcbplotparams', 'net_class', 'module',
+               'kicad_sch', 'lib_symbols', 'symbol', 'sheet', 'sheet_instances', 'symbol_instances'}
 
 
 class Point(object):
     def __init__(self, items):
         super().__init__()
         self.x = _check_float(items, 1, 'x coord')
         self.y = _check_float(items, 2, 'y coord')
 
     @staticmethod
     def parse(items):
         return Point(items)
 
 
+def make_separated(sexp):
+    """ Add separators to make the file more readable """
+    if not isinstance(sexp, list):
+        return sexp
+    if not isinstance(sexp[0], Symbol) or sexp[0].value() not in TO_SEPARATE:
+        return sexp
+    separated = []
+    for s in sexp:
+        separated.append(make_separated(s))
+        if isinstance(s, list):
+            separated.append(Sep())
+    return separated
+
+
+def load_sexp_file(fname):
+    with open(fname, 'rt') as fh:
+        error = None
+        try:
+            ki_file = load(fh)
+        except SExpData as e:
+            error = str(e)
+        if error:
+            raise KiPlotConfigurationError(error)
+    return ki_file
+
+
 def _check_is_symbol_list(e, allow_orphan_symbol=()):
     # Each entry is a list
     if not isinstance(e, list):
         if isinstance(e, Symbol):
             name = e.value()
             if name in allow_orphan_symbol:
                 return name
@@ -155,7 +184,12 @@
             raise SchError('Unknown points attribute `{}`'.format(i))
     return points
 
 
 def _get_size(items, pos, name):
     value = _check_symbol_value(items, pos, name, 'size')
     return _get_xy(value)
+
+
+def _get_symbol_name(items):
+    """ Check if items is a list and starts with a symbol, return its name, otherwise None """
+    return None if not isinstance(items, list) or not isinstance(items[0], Symbol) else items[0].value()
```

### Comparing `kibot-1.6.5/kibot/kicad/sexpdata.py` & `kibot-1.7.0/kibot/kicad/sexpdata.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/kicad/v5_sch.py` & `kibot-1.7.0/kibot/kicad/v5_sch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1970,17 +1970,19 @@
                         continue
                     fld = SubElement(comp, 'property')
                     fld.set('name', fname)
                     fld.set('value', fvalue)
                 prop = SubElement(comp, 'property')
                 prop.set('name', 'Sheetname')
                 prop.set('value', os.path.basename(c.sheet_path_h))
-                prop = SubElement(comp, 'property')
-                prop.set('name', 'Sheetfile')
-                prop.set('value', os.path.basename(c.parent_sheet.fname))
+                if hasattr(c, 'parent_sheet'):
+                    # Components from the PCB doesn't have "parent_sheet"
+                    prop = SubElement(comp, 'property')
+                    prop.set('name', 'Sheetfile')
+                    prop.set('value', os.path.basename(c.parent_sheet.fname))
             shp = SubElement(comp, 'sheetpath')
             shp.set('names', _path(c.sheet_path_h))
             shp.set('tstamps', _path(c.sheet_path))
             if self.netlist_version == 'D':
                 SubElement(comp, 'tstamp').text = tstamps[c.ref].split()[0]
             else:
                 SubElement(comp, 'tstamps').text = tstamps[c.ref]
```

### Comparing `kibot-1.6.5/kibot/kicad/v6_sch.py` & `kibot-1.7.0/kibot/kicad/v6_sch.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/kicad/worksheet.py` & `kibot-1.7.0/kibot/kicad/worksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2022-2023 Salvador E. Tropea
-# Copyright (c) 2022-2023 Instituto Nacional de Tecnología Industrial
+# Copyright (c) 2022-2024 Salvador E. Tropea
+# Copyright (c) 2022-2024 Instituto Nacional de Tecnología Industrial
 # License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 # KiCad bugs:
 # - Text bold doesn't work
 # - Shape Line and Rect swapped
 """
-KiCad v5/6 Worksheet format.
+KiCad v5/6/7/8 Worksheet format.
 A basic implementation of the .kicad_wks file format.
 Documentation: https://dev-docs.kicad.org/en/file-formats/sexpr-worksheet/
 """
 import io
 from struct import unpack
 from pcbnew import (wxPoint, wxSize, FromMM, wxPointMM)
 from ..gs import GS
@@ -48,15 +48,16 @@
 from ..misc import W_WKSVERSION
 from .. import log
 
 logger = log.get_logger()
 setup = None
 # The version of "kicad_wks" used for all tests is 20210606
 # 20220228 seems to be fully supported
-SUP_VERSION = 20220228
+# And now 20231118, but the documentation is from 2023-04-13 ...
+SUP_VERSION = 20231118
 # Hash to convert KiCad 5 "%X" markers to KiCad 6 "${XXX}" text variables
 KI5_2_KI6 = {'K': 'KICAD_VERSION', 'S': '#', 'N': '##', 'C0': 'COMMENT1', 'C1': 'COMMENT2', 'C2': 'COMMENT3',
              'C3': 'COMMENT4', 'C4': 'COMMENT5', 'C5': 'COMMENT6', 'C6': 'COMMENT7', 'C7': 'COMMENT8',
              'C8': 'COMMENT9', 'Y': 'COMPANY', 'F': 'FILENAME', 'D': 'ISSUE_DATE', 'Z': 'PAPER', 'R': 'REVISION',
              'P': 'SHEETNAME', 'T': 'TITLE'}
 
 
@@ -469,15 +470,15 @@
                 raise WksError(error)
         if not isinstance(wks, list) or (wks[0].value() != 'page_layout' and wks[0].value() != 'kicad_wks'):
             raise WksError('No kicad_wks signature')
         elements = []
         global setup
         setup = WksSetup()
         version = 0
-        generator = ''
+        generator_version = generator = ''
         has_images = False
         for e in wks[1:]:
             e_type = _check_is_symbol_list(e)
             if e_type == 'setup':
                 setup = WksSetup.parse(e)
             elif e_type == 'rect':
                 elements.append(WksRect.parse(e))
@@ -494,18 +495,20 @@
                 elements.append(WksBitmap.parse(e))
                 has_images = True
             elif e_type == 'version':
                 version = _check_integer(e, 1, e_type)
                 if version > SUP_VERSION:
                     logger.warning(W_WKSVERSION+"Unsupported worksheet version, loading could fail")
             elif e_type == 'generator':
-                generator = _check_symbol(e, 1, e_type)
+                generator = _check_relaxed(e, 1, e_type)
+            elif e_type == 'generator_version':
+                generator_version = ' v'+_check_str(e, 1, e_type)
             else:
                 raise WksError('Unknown worksheet attribute `{}`'.format(e_type))
-        return Worksheet(setup, elements, version, generator, has_images)
+        return Worksheet(setup, elements, version, generator+generator_version, has_images)
 
     def set_page(self, pw, ph):
         pw = FromMM(pw)
         ph = FromMM(ph)
         self.pw = pw
         self.ph = ph
         self.lm = self.setup.left_margin
```

### Comparing `kibot-1.6.5/kibot/kiplot.py` & `kibot-1.7.0/kibot/kiplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 from .gs import GS
 from .registrable import RegOutput
 from .misc import (PLOT_ERROR, CORRUPTED_PCB, EXIT_BAD_ARGS, CORRUPTED_SCH, version_str2tuple,
                    EXIT_BAD_CONFIG, WRONG_INSTALL, UI_SMD, UI_VIRTUAL, TRY_INSTALL_CHECK, MOD_SMD, MOD_THROUGH_HOLE,
                    MOD_VIRTUAL, W_PCBNOSCH, W_NONEEDSKIP, W_WRONGCHAR, name2make, W_TIMEOUT, W_KIAUTO, W_VARSCH,
                    NO_SCH_FILE, NO_PCB_FILE, W_VARPCB, NO_YAML_MODULE, WRONG_ARGUMENTS, FAILED_EXECUTE, W_VALMISMATCH,
-                   MOD_EXCLUDE_FROM_POS_FILES, MOD_EXCLUDE_FROM_BOM, MOD_BOARD_ONLY, hide_stderr, W_MAXDEPTH, DONT_STOP)
+                   MOD_EXCLUDE_FROM_POS_FILES, MOD_EXCLUDE_FROM_BOM, MOD_BOARD_ONLY, hide_stderr, W_MAXDEPTH, DONT_STOP,
+                   W_BADREF)
 from .error import PlotError, KiPlotConfigurationError, config_error, KiPlotError
 from .config_reader import CfgYamlReader
 from .pre_base import BasePreFlight
 from .dep_downloader import register_deps
 import kibot.dep_downloader as dep_downloader
 from .kicad.v5_sch import Schematic, SchFileError, SchError, SchematicField
 from .kicad.v6_sch import SchematicV6, SchematicComponentV6
@@ -272,15 +273,15 @@
     GS.sch = load_any_sch(GS.sch_file, GS.sch_basename)
 
 
 def create_component_from_footprint(m, ref):
     c = SchematicComponentV6()
     c.f_ref = c.ref = ref
     c.name = m.GetValue()
-    c.sheet_path_h = c.lib = ''
+    c.sheet_path_h = c.sheet_path = c.lib = ''
     c.project = GS.sch_basename
     c.id = m.m_Uuid.AsString() if hasattr(m, 'm_Uuid') else ''
     # Basic fields
     # Reference
     f = SchematicField()
     f.name = 'Reference'
     f.value = ref
@@ -310,15 +311,20 @@
         f = SchematicField()
         f.name = name
         f.value = val
         f.number = -1
         f.visible(False)
         c.add_field(f)
     c._solve_fields(None)
-    c.split_ref()
+    try:
+        c.split_ref()
+    except SchError:
+        # Unusable ref, discard it
+        logger.warning(f'{W_BADREF}Not including component `{ref}` in filters because it has a malformed reference')
+        c = None
     return c
 
 
 def get_board_comps_data(comps):
     """ Add information from the PCB to the list of components from the schematic.
         Note that we do it every time the function is called to reset transformation filters like rot_footprint. """
     if not GS.pcb_file:
@@ -338,14 +344,16 @@
             if not (attrs & MOD_BOARD_ONLY) and not ref.startswith('KiKit_'):
                 logger.warning(W_PCBNOSCH + '`{}` component in board, but not in schematic'.format(ref))
             if not GS.global_include_components_from_pcb:
                 # v1.6.3 behavior
                 continue
             # Create a component for this so we can include/exclude it using filters
             c = create_component_from_footprint(m, ref)
+            if c is None:
+                continue
             comps_hash[ref] = [c]
             comps.append(c)
         for c in comps_hash[ref]:
             new_value = m.GetValue()
             if new_value != c.value and '${' not in c.value:
                 logger.warning(f"{W_VALMISMATCH}Value field mismatch for `{ref}` (SCH: `{c.value}` PCB: `{new_value}`)")
             c.value = new_value
@@ -400,24 +408,25 @@
 
 
 def expand_fields(comps, dont_copy=False):
     if not dont_copy:
         new_comps = deepcopy(comps)
         for n_c, c in zip(new_comps, comps):
             n_c.original_copy = c
+    KiConf.init(GS.sch_file)
     env = KiConf.kicad_env
     env.update(GS.load_pro_variables())
     for c in comps:
         expand_comp_fields(c, env)
     return comps
 
 
 def preflight_checks(skip_pre, targets):
     logger.debug("Preflight checks")
-
+    BasePreFlight.configure_all()
     if skip_pre is not None:
         if skip_pre == 'all':
             logger.debug("Skipping all preflight actions")
             return
         else:
             skip_list = skip_pre.split(',')
             for skip in skip_list:
@@ -494,15 +503,15 @@
         out._done = True
     except KiPlotConfigurationError as e:
         msg = "In section '"+out.name+"' ("+out.type+"): "+str(e)
         if dont_stop:
             logger.error(msg)
         else:
             config_error(msg)
-    except (PlotError, KiPlotError) as e:
+    except (PlotError, KiPlotError, SchError) as e:
         msg = "In output `"+str(out)+"`: "+str(e)
         GS.exit_with_error(msg, DONT_STOP if dont_stop else PLOT_ERROR)
     except KiConfError as e:
         ki_conf_error(e)
     except SystemExit:
         if not dont_stop:
             raise
@@ -631,14 +640,15 @@
         f.write('{}:{}\n\n'.format(all, tg))
         extra_targets.append(all)
     return extra_targets
 
 
 def get_pre_targets(targets, dependencies, is_pre):
     pcb_targets = sch_targets = ''
+    BasePreFlight.configure_all()
     prefs = BasePreFlight.get_in_use_objs()
     try:
         for pre in prefs:
             tg = pre.get_targets()
             if not tg:
                 continue
             name = pre._name
@@ -948,14 +958,22 @@
 def register_xmp_import(name, definitions=None):
     """ Register an import we need for an example """
     global needed_imports
     assert name not in needed_imports
     needed_imports[name] = definitions
 
 
+def check_we_cant_use(o):
+    """ Check if the output doesn't have what it needs, i.e. no PCB and this is PCB related """
+    return ((not (o.is_pcb() and GS.pcb_file) and
+             not (o.is_sch() and GS.sch_file) and
+             not (o.is_any() and (GS.pcb_file or GS.sch_file))) or
+            ((o.is_pcb() and o.is_sch()) and (not GS.pcb_file or not GS.sch_file)))
+
+
 def generate_one_example(dest_dir, types):
     """ Generate a example config for dest_dir """
     fname = discover_files(dest_dir)
     # Abort if none
     if not GS.pcb_file and not GS.sch_file:
         return None
     # Reset the board and schematic
@@ -976,31 +994,46 @@
             layers = look_for_used_layers()
         if GS.sch_file:
             load_sch()
         # Filter some warnings
         fil = [{'number': 1007},  # No information for a component in a distributor
                {'number': 1015},  # More than one component in a search for a distributor
                {'number': 58},    # Missing project file
+               {'number': 107},   # Stencil.side auto, we always use it for the example
                ]
         glb = {'filters': fil}
         yaml_dump(f, {'global': glb})
         f.write('\n')
         # A helper for the internal templates
         global needed_imports
         needed_imports = {}
+        # All the preflights
+        preflights = {}
+        for n, cls in OrderedDict(sorted(BasePreFlight.get_registered().items())).items():
+            o = cls(n, None)
+            if types and n not in types:
+                logger.debug('- {}, not selected (PCB: {} SCH: {})'.format(n, o.is_pcb(), o.is_sch()))
+                continue
+            if check_we_cant_use(o):
+                logger.debug('- {}, skipped (PCB: {} SCH: {})'.format(n, o.is_pcb(), o.is_sch()))
+                continue
+            tree = cls.get_conf_examples(n, layers)
+            if tree:
+                logger.debug('- {}, generated'.format(n))
+                preflights.update(tree)
+            else:
+                logger.debug('- {}, nothing to do'.format(n))
         # All the outputs
         outputs = []
         for n, cls in OrderedDict(sorted(outs.items())).items():
             o = cls()
             if types and n not in types:
                 logger.debug('- {}, not selected (PCB: {} SCH: {})'.format(n, o.is_pcb(), o.is_sch()))
                 continue
-            if ((not (o.is_pcb() and GS.pcb_file) and not (o.is_sch() and GS.sch_file) and
-                 not (o.is_any() and (GS.pcb_file or GS.sch_file))) or
-               ((o.is_pcb() and o.is_sch()) and (not GS.pcb_file or not GS.sch_file))):
+            if check_we_cant_use(o):
                 logger.debug('- {}, skipped (PCB: {} SCH: {})'.format(n, o.is_pcb(), o.is_sch()))
                 continue
             tree = cls.get_conf_examples(n, layers)
             if tree:
                 logger.debug('- {}, generated'.format(n))
                 outputs.extend(tree)
             else:
@@ -1014,14 +1047,17 @@
                     continue
                 content = {'file': n}
                 if d:
                     content['definitions'] = d
                 imports.append(content)
             yaml_dump(f, {'import': imports})
             f.write('\n')
+        if preflights:
+            yaml_dump(f, {'preflight': preflights})
+            f.write('\n')
         if outputs:
             yaml_dump(f, {'outputs': outputs})
         else:
             return None
         if global_defaults:
             f.write('\n...\n')
             yaml_dump(f, {'definitions': global_defaults})
@@ -1029,16 +1065,17 @@
 
 
 def generate_targets(config_file):
     """ Generate all possible targets for the configuration file """
     # Reset the board and schematic
     GS.board = None
     GS.sch = None
-    # Reset the list of outputs
+    # Reset the list of outputs and preflights
     RegOutput.reset()
+    BasePreFlight.reset()
     # Read the config file
     cr = CfgYamlReader()
     with open(config_file) as cf_file:
         outputs = cr.read(cf_file)
     # Do all the job
     generate_outputs(outputs, [], False, None, False, False, dont_stop=True)
```

### Comparing `kibot-1.6.5/kibot/layer.py` & `kibot-1.7.0/kibot/layer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/log.py` & `kibot-1.7.0/kibot/log.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/macros.py` & `kibot-1.7.0/kibot/macros.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/__init__.py` & `kibot-1.7.0/kibot/mcpyrate/__init__.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/activate.py` & `kibot-1.7.0/kibot/mcpyrate/activate.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/ansi.py` & `kibot-1.7.0/kibot/mcpyrate/ansi.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/astdumper.py` & `kibot-1.7.0/kibot/mcpyrate/astdumper.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/astfixers.py` & `kibot-1.7.0/kibot/mcpyrate/astfixers.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/bunch.py` & `kibot-1.7.0/kibot/mcpyrate/bunch.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/colorizer.py` & `kibot-1.7.0/kibot/mcpyrate/colorizer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/compiler.py` & `kibot-1.7.0/kibot/mcpyrate/compiler.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/core.py` & `kibot-1.7.0/kibot/mcpyrate/core.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/coreutils.py` & `kibot-1.7.0/kibot/mcpyrate/coreutils.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/debug.py` & `kibot-1.7.0/kibot/mcpyrate/debug.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/dialects.py` & `kibot-1.7.0/kibot/mcpyrate/dialects.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/expander.py` & `kibot-1.7.0/kibot/mcpyrate/expander.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/importer.py` & `kibot-1.7.0/kibot/mcpyrate/importer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/markers.py` & `kibot-1.7.0/kibot/mcpyrate/markers.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/metatools.py` & `kibot-1.7.0/kibot/mcpyrate/metatools.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/multiphase.py` & `kibot-1.7.0/kibot/mcpyrate/multiphase.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/pycachecleaner.py` & `kibot-1.7.0/kibot/mcpyrate/pycachecleaner.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/quotes.py` & `kibot-1.7.0/kibot/mcpyrate/quotes.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/splicing.py` & `kibot-1.7.0/kibot/mcpyrate/splicing.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/unparser.py` & `kibot-1.7.0/kibot/mcpyrate/unparser.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/utils.py` & `kibot-1.7.0/kibot/mcpyrate/utils.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/mcpyrate/walkers.py` & `kibot-1.7.0/kibot/mcpyrate/walkers.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/optionable.py` & `kibot-1.7.0/kibot/optionable.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_any_diff.py` & `kibot-1.7.0/kibot/out_any_diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2022-2024 Salvador E. Tropea
 # Copyright (c) 2022-2024 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 import os
-from tempfile import NamedTemporaryFile
 from .gs import GS
 from .kiplot import run_command
 from .out_base import VariantOptions
 from .pre_base import BasePreFlight
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 
@@ -67,16 +66,15 @@
         self.run_git(['worktree', 'remove', '--force', name])
 
     def write_empty_file(self, name, create_tmp=False):
         base, ext = os.path.splitext(name)
         kind = 'PCB' if ext == '.kicad_pcb' else 'schematic'
         if create_tmp:
             # Use a temporary file
-            with NamedTemporaryFile(mode='w', suffix=ext, delete=False) as f:
-                name = f.name
+            name = GS.tmp_file(suffix=ext)
             base = os.path.splitext(name)[0]
         to_remove = [name]
         logger.debug('Creating empty '+kind+': '+name)
         with open(name, 'w') as f:
             if ext == '.kicad_sch':
                 f.write("(kicad_sch (version 20211123) (generator eeschema))\n")
             elif ext == '.sch':
@@ -94,13 +92,13 @@
                     f.write("EESchema-LIBRARY Version 2.4\n#\n#End Library\n")
                 to_remove.append(lib_name)
         return name, to_remove
 
     def save_layers_incl(self, layers):
         self._solved_layers = layers
         logger.debug('Including layers:')
-        with NamedTemporaryFile(mode='w', suffix='.lst', delete=False) as f:
-            self.incl_file = f.name
-            for la in layers:
-                logger.debug('- {} ({})'.format(la.layer, la.id))
-                f.write(str(la.id)+'\n')
+        txt = ''
+        for la in layers:
+            logger.debug(f'- {la.layer} ({la.id})')
+            txt += str(la.id)+'\n'
+        self.incl_file = GS.tmp_file(content=txt, suffix='.lst')
         return self.incl_file
```

### Comparing `kibot-1.6.5/kibot/out_any_drill.py` & `kibot-1.7.0/kibot/out_any_drill.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_any_layer.py` & `kibot-1.7.0/kibot/out_any_layer.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_any_pcb_print.py` & `kibot-1.7.0/kibot/out_any_pcb_print.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2020-2023 Salvador E. Tropea
 # Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 import os
 from .pre_base import BasePreFlight
 from .gs import GS
-from .misc import PDF_PCB_PRINT, KICAD_VERSION_7_0_1, MISSING_TOOL
+from .misc import PDF_PCB_PRINT, KICAD_VERSION_7_0_1, MISSING_TOOL, W_DEPR
 from .out_base import VariantOptions
 from .macros import macros, document, output_class  # noqa: F401
 from .drill_marks import add_drill_marks, DRILL_MARKS_MAP
 from .layer import Layer
 from . import log
 
 logger = log.get_logger()
@@ -65,14 +65,15 @@
         return fname
 
     def get_targets(self, out_dir):
         return [self._parent.expand_filename(out_dir, self.output)]
 
     def run(self, output, svg=False):
         super().run(self._layers)
+        logger.warning(W_DEPR+'The `pdf_pcb_print` and `svg_pcb_print` outputs are deprecated, use `pcb_print` instead')
         if GS.ki7 and GS.kicad_version_n < KICAD_VERSION_7_0_1 and self.scaling != 0 and self.scaling != 1.0:
             GS.exit_with_error("Scaled printing is broken in KiCad 7.0.0\n"
                                "Please upgrade KiCad to 7.0.1 or newer", MISSING_TOOL)
         command = self.ensure_tool('KiAuto')
         # Output file name
         cmd = [command, 'export', '--output_name', output]
         if BasePreFlight.get_option('check_zone_fills'):
```

### Comparing `kibot-1.6.5/kibot/out_any_sch_print.py` & `kibot-1.7.0/kibot/out_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020-2023 Salvador E. Tropea
-# Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
+# Copyright (c) 2022 Salvador E. Tropea
+# Copyright (c) 2022 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
+"""
+Dependencies:
+  - from: KiAuto
+    role: Show KiAuto installation information
+    version: 2.0.0
+"""
 import os
-from tempfile import mkdtemp
+import sys
 from .gs import GS
-from .out_base import VariantOptions
+from .optionable import BaseOptions
+from .kiplot import run_command
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
 
 
-class Any_SCH_PrintOptions(VariantOptions):
+class InfoOptions(BaseOptions):
     def __init__(self):
         with document:
-            self.monochrome = False
-            """ Generate a monochromatic output """
-            self.frame = True
-            """ *Include the frame and title block """
-            self.all_pages = True
-            """ Generate with all hierarchical sheets """
-            self.color_theme = ''
-            """ Color theme used, this must exist in the KiCad config (KiCad 6) """
-            self.background_color = False
-            """ Use the background color from the `color_theme` (KiCad 6) """
-            self.title = ''
-            """ Text used to replace the sheet title. %VALUE expansions are allowed.
-                If it starts with `+` the text is concatenated """
+            self.output = GS.def_global_output
+            """ *Filename for the output (%i=info, %x=txt) """
+            self.environment = 'names'
+            """ [names,none,full] List environment variables.
+                IMPORTANT: Don't use `full` unless you know you are not leaking sensitive information """
         super().__init__()
-        self.add_to_doc('variant', "Not fitted components are crossed")
-        self._expand_id = 'schematic'
+        self._expand_id = 'info'
+        self._expand_ext = 'txt'
+        self._none_related = True
 
     def get_targets(self, out_dir):
-        if self.output:
-            return [self._parent.expand_filename(out_dir, self.output)]
-        return [self._parent.expand_filename(out_dir, '%f.%x')]
+        return [self._parent.expand_filename(out_dir, self.output)]
 
     def run(self, name):
-        super().run(name)
-        command = self.ensure_tool('KiAuto')
-        if self.title:
-            self.set_title(self.title, sch=True)
-        if self._comps or self.title:
-            # Save it to a temporal dir
-            sch_dir = mkdtemp(prefix='tmp-kibot-'+self._expand_ext+'_sch_print-')
-            GS.copy_project_sch(sch_dir)
-            fname = GS.sch.save_variant(sch_dir)
-            sch_file = os.path.join(sch_dir, fname)
-            self._files_to_remove.append(sch_dir)
-        else:
-            sch_file = GS.sch_file
-        fmt = 'hpgl' if self._expand_ext == 'plt' else self._expand_ext
-        cmd = [command, 'export', '--file_format', fmt, '-o', name]
-        if self.monochrome:
-            cmd.append('--monochrome')
-        if not self.frame:
-            cmd.append('--no_frame')
-        if self.all_pages:
-            cmd.append('--all_pages')
-        if self.color_theme:
-            cmd.extend(['--color_theme', self.color_theme])
-        if self.background_color:
-            cmd.append('--background_color')
-        if hasattr(self, '_origin'):
-            cmd.extend(['--hpgl_origin', str(self._origin)])
-        if hasattr(self, 'pen_size'):
-            cmd.extend(['--hpgl_pen_size', str(self.pen_size)])
-        cmd.extend([sch_file, os.path.dirname(name)])
-        self.exec_with_retry(self.add_extra_options(cmd), self._exit_error)
-        if self.title:
-            self.restore_title(sch=True)
+        dir = os.path.dirname(os.path.abspath(sys.argv[0]))
+        ret = run_command([os.path.join(dir, 'kibot-check'), '-p'])
+        with open(name, 'wt') as f:
+            f.write(ret+'\n')
+            # Environment
+            if self.environment == 'names':
+                f.write('\nEnvironment:\n')
+                for n in sorted(os.environ.keys()):
+                    f.write(n+'\n')
+            elif self.environment == 'full':
+                f.write('\nEnvironment:\n')
+                for n in sorted(os.environ.keys()):
+                    f.write(n+'='+os.environ[n]+'\n')
+            # KiAuto
+            command = self.check_tool('KiAuto')
+            if command:
+                ret = run_command([command, '--info'])
+                f.write('\nKiAuto:\n'+ret+'\n')
+
+
+@output_class
+class Info(BaseOutput):  # noqa: F821
+    """ Info
+        Records information about the current run.
+        It can be used to know more about the environment used to generate the files.
+        Please don't rely on the way things are reported, its content could change,
+        adding or removing information """
+    def __init__(self):
+        super().__init__()
+        self._category = ['PCB/docs', 'Schematic/docs']
+        with document:
+            self.options = InfoOptions
+            """ *[dict] Options for the `info` output """
+
+    @staticmethod
+    def get_conf_examples(name, layers):
+        return BaseOutput.simple_conf_examples(name, 'Information about the run', '.')  # noqa: F821
```

### Comparing `kibot-1.6.5/kibot/out_any_stencil.py` & `kibot-1.7.0/kibot/out_any_stencil.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_base.py` & `kibot-1.7.0/kibot/out_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 from copy import deepcopy
 import math
 import os
 import re
 from shutil import rmtree
-from tempfile import NamedTemporaryFile, mkdtemp
 from .gs import GS
+from .kicad.pcb import replace_footprints
 from .kiplot import load_sch, get_board_comps_data
 from .misc import Rect, W_WRONGPASTE, DISABLE_3D_MODEL_TEXT, W_NOCRTYD, MOD_ALLOW_MISSING_COURTYARD, W_MISSDIR, W_KEEPTMP
 if not GS.kicad_version_n:
     # When running the regression tests we need it
     from kibot.__main__ import detect_kicad
     detect_kicad()
 if GS.ki6:
@@ -47,15 +47,15 @@
 }
 Shape {
   geometry Box { size 1 1 1 }
   appearance Appearance {material USE RED-01 }
 }
 
 """
-comp_range_regex = re.compile(r'(\w+?)(\d+)-(\w+?)(\d+)')
+comp_range_regex = re.compile(r'([a-zA-Z]+)(\d+)-([a-zA-Z]+)(\d+)')
 
 
 class BaseOutput(RegOutput):
     def __init__(self):
         super().__init__()
         with document:
             self.name = ''
@@ -707,19 +707,17 @@
                                 break
             if not matched and default is not None:
                 self.apply_list_of_3D_models(enable, slots, m, '_default_')
 
     def create_3D_highlight_file(self):
         if self._highlight_3D_file:
             return
-        with NamedTemporaryFile(mode='w', suffix='.wrl', delete=False) as f:
-            self._highlight_3D_file = f.name
-            self._files_to_remove.append(f.name)
-            logger.debug('Creating temporal highlight file '+f.name)
-            f.write(HIGHLIGHT_3D_WRL)
+        tname = GS.tmp_file(content=HIGHLIGHT_3D_WRL, suffix='.wrl', what='temporal highlight', a_logger=logger)
+        self._highlight_3D_file = tname
+        self._files_to_remove.append(tname)
 
     def get_crtyd_bbox(self, board, m):
         fcrtyd = board.GetLayerID('F.CrtYd')
         bcrtyd = board.GetLayerID('B.CrtYd')
         bbox = Rect()
         for gi in m.GraphicalItems():
             if gi.GetClass() == GS.footprint_gr_type:
@@ -795,22 +793,40 @@
             m.Models().pop()
         self._highlighted_3D_components = None
 
     def will_filter_pcb_components(self):
         """ True if we will apply filters/variants """
         return self._comps or self._sub_pcb
 
+    def apply_footprint_variants(self, board, comps_hash):
+        """ Allows changing the footprints using variants """
+        if comps_hash is None:
+            return
+        # Check if we have footprints that needs change
+        to_change = {}
+        for m in GS.get_modules_board(board):
+            ref = m.GetReference()
+            c = comps_hash.get(ref, None)
+            if hasattr(c, '_footprint_variant') and c._footprint_variant:
+                to_change[c.ref] = c.get_field_value('footprint')
+        if not to_change:
+            return
+        # One or more needs a change
+        logger.debug(f'Replacing footprints from variant change {to_change}')
+        replace_footprints(GS.pcb_file, to_change, logger, replace_pcb=False)
+
     def filter_pcb_components(self, do_3D=False, do_2D=True, highlight=None):
         if not self.will_filter_pcb_components():
             return False
         self.comps_hash = self.get_refs_hash()
         if self._sub_pcb:
             self._sub_pcb.apply(self.comps_hash)
         if self._comps:
             if do_2D:
+                self.apply_footprint_variants(GS.board, self.comps_hash)
                 self.cross_modules(GS.board, self.comps_hash)
                 self.remove_paste_and_glue(GS.board, self.comps_hash)
                 if hasattr(self, 'hide_excluded') and self.hide_excluded:
                     self.remove_fab(GS.board, self.comps_hash)
                 # Copy any change in the schematic fields to the PCB properties
                 # I.e. the value of a component so it gets updated in the *.Fab layer
                 # Also useful for iBoM that can read the sch fields from the PCB
@@ -905,19 +921,15 @@
                     m.SetFPIDAsString(data[2])
                 GS.set_fields(m, data[1])
 
     def save_tmp_board(self, dir=None):
         """ Save the PCB to a temporal file.
             Advantage: all relative paths inside the file remains valid
             Disadvantage: the name of the file gets altered """
-        if dir is None:
-            dir = GS.pcb_dir
-        with NamedTemporaryFile(mode='w', suffix='.kicad_pcb', delete=False, dir=dir) as f:
-            fname = f.name
-        logger.debug('Storing modified PCB to `{}`'.format(fname))
+        fname = GS.tmp_file(suffix='.kicad_pcb', dir=GS.pcb_dir if dir is None else dir, what='modified PCB', a_logger=logger)
         GS.board.Save(fname)
         GS.copy_project(fname)
         self._files_to_remove.extend(GS.get_pcb_and_pro_names(fname))
         return fname
 
     def save_tmp_board_if_variant(self, new_title='', dir=None, do_3D=False):
         """ If we have a variant apply it and save the PCB to a file """
@@ -933,15 +945,15 @@
         return fname
 
     @staticmethod
     def save_tmp_dir_board(id, force_dir=None, forced_name=None):
         """ Save the PCB to a temporal dir.
             Disadvantage: all relative paths inside the file becomes useless
             Aadvantage: the name of the file remains the same """
-        pcb_dir = mkdtemp(prefix='tmp-kibot-'+id+'-') if force_dir is None else force_dir
+        pcb_dir = GS.mkdtemp(id) if force_dir is None else force_dir
         basename = forced_name if forced_name else GS.pcb_basename
         fname = os.path.join(pcb_dir, basename+'.kicad_pcb')
         logger.debug('Storing modified PCB to `{}`'.format(fname))
         GS.board.Save(fname)
         pro_name, _, _ = GS.copy_project(fname)
         KiConf.fix_page_layout(pro_name)
         return fname, pcb_dir
```

### Comparing `kibot-1.6.5/kibot/out_base_3d.py` & `kibot-1.7.0/kibot/out_base_3d.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_blender_export.py` & `kibot-1.7.0/kibot/out_blender_export.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_boardview.py` & `kibot-1.7.0/kibot/out_boardview.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_bom.py` & `kibot-1.7.0/kibot/out_bom.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     version: 1.1.2
     downloader: python
 """
 import csv
 from copy import deepcopy
 import os
 import re
-from tempfile import NamedTemporaryFile
 from .gs import GS
 from .misc import W_BADFIELD, W_NEEDSPCB, DISTRIBUTORS, W_NOPART, W_MISSREF, DISTRIBUTORS_STUBS, DISTRIBUTORS_STUBS_SEPS
 from .optionable import Optionable, BaseOptions
 from .registrable import RegOutput
 from .error import KiPlotConfigurationError
 from .kiplot import get_board_comps_data, load_any_sch, register_xmp_import, expand_fields, run_command
 from .kicad.v5_sch import SchematicComponent, SchematicField
@@ -175,14 +174,41 @@
                 if isinstance(c, str):
                     join.append(BoMJoinField(c))
                 else:
                     join.append(c)
             self.join = join
 
 
+class RowColors(Optionable):
+    """ Filters to give colors to rows """
+    def __init__(self):
+        super().__init__()
+        self._unknown_is_error = True
+        with document:
+            self.description = ''
+            """ *A description for this color, must be filled """
+            self.color = '#FF8080'
+            """ *Color used for this category """
+            self.filter = Optionable
+            """ *[string|list(string)='_none'] Name of the filter to match.
+                Be careful because this filter should be coherent with the grouping fields.
+                KiBot will assume that all the components grouped in the same group will
+                return the same value when applying this filter """
+        self._description_example = "Components that can't be replaced"
+
+    def config(self, parent):
+        super().config(parent)
+        self.validate_colors(['color'])
+        if not self.description:
+            raise KiPlotConfigurationError('You must add a description for a colored row')
+        if isinstance(self.filter, type):
+            raise KiPlotConfigurationError('You must provide a filter to match the rows')
+        self.filter = BaseFilter.solve_filter(self.filter, 'colored rows')
+
+
 class BoMLinkable(Optionable):
     """ Base class for HTML and XLSX formats """
     def __init__(self):
         super().__init__()
         with document:
             self.col_colors = True
             """ Use colors to show the field type """
@@ -208,14 +234,17 @@
                 Note that when using an SVG this is first converted to a PNG using `logo_width` """
             self.logo_width = 370
             """ Used when the logo is an SVG image. This width is used to render the SVG image """
             self.title = 'KiBot Bill of Materials'
             """ *BoM title """
             self.extra_info = Optionable
             """ [string|list(string)=''] Information to put after the title and before the pcb and stats info """
+            self.row_colors = RowColors
+            """ [list(dict)] Used to highlight rows using filters. Rows that match a filter can be colored.
+                Note that these rows won't have colored columns """
 
     def config(self, parent):
         super().config(parent)
         # *_link
         self.digikey_link = self.force_list(self.digikey_link, comma_sep=False, lower_case=True)
         self.mouser_link = self.force_list(self.mouser_link, comma_sep=False, lower_case=True)
         if isinstance(self.lcsc_link, bool):
@@ -230,14 +259,17 @@
             self.logo = os.path.abspath(self.logo)
             if not os.path.isfile(self.logo):
                 raise KiPlotConfigurationError('Missing logo file `{}`'.format(self.logo))
         # Extra info lines
         self.extra_info = Optionable.force_list(self.extra_info, comma_sep=False)
         # Datasheet as link
         self.datasheet_as_link = self.datasheet_as_link.lower()
+        # Row colors
+        if isinstance(self.row_colors, type):
+            self.row_colors = []
 
 
 class BoMHTML(BoMLinkable):
     """ HTML options """
     def __init__(self):
         super().__init__()
         with document:
@@ -465,15 +497,16 @@
             """ *Exclude DNF (Do Not Fit) components """
             self.fit_field = 'Config'
             """ Field name used for internal filters (not for variants) """
             self.use_alt = False
             """ Print grouped references in the alternate compressed style eg: R1-R7,R18 """
             self.columns = BoMColumns
             """ *[list(dict)|list(string)] List of columns to display.
-                Can be just the name of the field """
+                Can be just the name of the field.
+                In addition to all user defined fields you have various special columns, consult :ref:`bom_columns` """
             self.cost_extra_columns = BoMColumns
             """ [list(dict)|list(string)] List of columns to add to the global section of the cost.
                 Can be just the name of the field """
             self.normalize_values = False
             """ *Try to normalize the R, L and C values, producing uniform units and prefixes """
             self.normalize_locale = False
             """ When normalizing values use the locale decimal point """
@@ -908,16 +941,15 @@
         else:
             return None
         if not logo:
             return None
         ext = os.path.splitext(logo)[1]
         if ext.lower() != '.svg':
             return None
-        with NamedTemporaryFile(mode='w', suffix='.png', delete=False) as f:
-            png = f.name
+        png = GS.tmp_file(suffix='.png')
         cmd = [self.ensure_tool('RSVG'), '-w', str(w), '-f', 'png', '-o', png, logo]
         run_command(cmd)
         self._old_logo = logo
         if self.format == 'html':
             self.html.logo = png
         elif self.format == 'xlsx':
             self.xlsx.logo = png
@@ -1055,15 +1087,15 @@
     def process_templates(mpn_fields, dists):
         # Rename MPN for something we have, or just remove it
         if mpn_fields:
             defs = {'_KIBOT_MPN_FIELD': '- field: manf#'}
         elif dists:
             defs = {'_KIBOT_MPN_FIELD': '- field: '+list(dists)[0]+'#'}
         else:
-            defs = {}
+            defs = {'_KIBOT_MPN_FIELD': ''}
         register_xmp_import('MacroFab_XYRS', defs)
 
     @staticmethod
     def get_conf_examples(name, layers):
         outs = []
         # Make a list of available fields
         fld_names, extra_names = BoMOptions._get_columns()
```

### Comparing `kibot-1.6.5/kibot/out_compress.py` & `kibot-1.7.0/kibot/out_compress.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     def create_zip(self, output, files):
         extra = {}
         extra['compression'] = self.ZIP_ALGORITHMS[self.compression]
         if sys.version_info >= (3, 7):
             extra['compresslevel'] = 9
         with ZipFile(output, 'w', **extra) as zip:
             for fname, dest in files.items():
+                if dest == '/':
+                    # When we move all to / the main dir is stored as / and Python crashes
+                    continue
                 logger.debug('Adding '+fname+' as '+dest)
                 zip.write(fname, dest)
 
     def create_tar(self, output, files):
         with tar_open(output, 'w:'+self.TAR_MODE[self.compression]) as tar:
             for fname, dest in files.items():
                 logger.debug('Adding '+fname+' as '+dest)
@@ -135,28 +138,26 @@
         return ext
 
     def get_files(self, output, no_out_run=False):
         output_real = os.path.realpath(output)
         files = OrderedDict()
         out_dir_cwd = os.getcwd()
         out_dir_default = self.expand_filename_sch(GS.out_dir)
-        dirs_list = []
+        dirs_list = set()
         for f in self.files:
             # Get the list of candidates
             files_list = None
             output_out_dir = None
             if f.from_output:
                 logger.debugl(2, '- From output `{}`'.format(f.from_output))
                 files_list, out_dir, out = get_output_targets(f.from_output, self._parent)
                 if not out.run_by_default and self.skip_not_run:
                     continue
                 output_out_dir = out_dir
                 logger.debugl(2, '- List of files: {}'.format(files_list))
-                if out_dir not in dirs_list:
-                    dirs_list.append(out_dir)
                 if not no_out_run:
                     extra_files = []
                     for file in files_list:
                         if not os.path.exists(file):
                             # The target doesn't exist
                             if not out._done:
                                 # The output wasn't created in this run, try running it
@@ -164,19 +165,40 @@
                             if not os.path.exists(file):
                                 # Still missing, something is wrong
                                 GS.exit_with_error(f'Unable to generate `{file}` from {out}', INTERNAL_ERROR)
                         if os.path.isdir(file):
                             # Popultate output adds the image dirs
                             # Computing its content is complex:
                             # - We must parse the input markdown
-                            # - We must coinfigure and use the renderer output to do the file name expansion
+                            # - We must configure and use the renderer output to do the file name expansion
                             # This is almost as complex as generating the whole output, so it adds the dir
                             extra_files += glob.glob(os.path.join(file, '**'), recursive=True)
                     if extra_files:
                         files_list += extra_files
+                # Add the output dir and all its subdirs
+                dirs_list.add(out_dir)
+                for fname in files_list:
+                    dname = os.path.dirname(fname)
+                    d_rel = os.path.relpath(dname, out_dir)
+                    if d_rel == '.':
+                        # The out_dir is already there
+                        continue
+                    # Add a subdir
+                    if dname not in dirs_list:
+                        dirs_list.add(dname)
+                        logger.debugl(2, f'- Adding subdir: {dname}')
+                    # Compute the subdirs leading to this one
+                    while True:
+                        d_rel = os.path.dirname(d_rel)
+                        if not d_rel:
+                            break
+                        dname = os.path.join(out_dir, d_rel)
+                        if dname not in dirs_list:
+                            dirs_list.add(dname)
+                            logger.debugl(2, f'- Adding subdir: {dname}')
             else:
                 out_dir = out_dir_cwd if f.from_cwd else out_dir_default
                 source = f.expand_filename_both(f.source, make_safe=False)
                 files_list = glob.iglob(os.path.join(out_dir, source), recursive=True)
                 if GS.debug_level > 1:
                     files_list = list(files_list)
                     logger.debug('- Pattern {} list of files: {}'.format(source, files_list))
@@ -193,15 +215,15 @@
                 # Compute the destination directory inside the archive
                 dest = fname
                 if f.dest:
                     dest = os.path.join(f.dest, os.path.basename(fname))
                 else:
                     dest = os.path.relpath(dest, out_dir)
                 files[fname_real] = dest
-        return files, dirs_list
+        return files, list(dirs_list)
 
     def get_targets(self, out_dir):
         return [self._parent.expand_filename(out_dir, self.output)]
 
     def get_dependencies(self):
         output = self.get_targets(self.expand_filename_sch(GS.out_dir))[0]
         files, _ = self.get_files(output, no_out_run=True)
```

### Comparing `kibot-1.6.5/kibot/out_copy_files.py` & `kibot-1.7.0/kibot/out_copy_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2022-2023 Salvador E. Tropea
-# Copyright (c) 2022-2023 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2022-2024 Salvador E. Tropea
+# Copyright (c) 2022-2024 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 from copy import copy
 import fnmatch
 import glob
 import os
 import re
 from shutil import copy2
 from .error import KiPlotConfigurationError
 from .gs import GS
-from .kiplot import config_output, get_output_dir, run_output
+from .kiplot import config_output, get_output_dir, run_output, register_xmp_import
 from .kicad.config import KiConf, LibAlias, FP_LIB_TABLE, SYM_LIB_TABLE
 from .misc import WRONG_ARGUMENTS, INTERNAL_ERROR, W_COPYOVER, W_MISSLIB, W_MISSCMP
 from .optionable import Optionable
 from .out_base_3d import Base3DOptions
 from .registrable import RegOutput
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
@@ -240,16 +240,19 @@
             if prj_name:
                 extra_files.append(prj_name)
             if prl_name:
                 extra_files.append(prl_name)
             if dru_name:
                 extra_files.append(dru_name)
             # Worksheet
-            wks = GS.fix_page_layout(prj_name, dry=dry)
-            extra_files += [w for w in wks if w is not None]
+            prj_name_used = prj_name
+            if dry and prj_name_used is not None and not os.path.isfile(prj_name_used):
+                prj_name_used = GS.pro_file
+            wks = GS.fix_page_layout(prj_name_used, dry=dry)
+            extra_files += [w for w in wks if w]
             if mode_project:
                 extra_files += self.copy_footprints(f.dest, dry)
                 extra_files += self.copy_symbols(f.dest, dry)
         if not self._comps:
             # We must undo the download/rename
             self.undo_3d_models_rename(GS.board)
         else:
@@ -395,18 +398,27 @@
     def __init__(self):
         super().__init__()
         # Make it low priority so it gets created after all the other outputs
         self.priority = 11
         with document:
             self.options = Copy_FilesOptions
             """ *[dict] Options for the `copy_files` output """
-        self._none_related = True
         # The help is inherited and already mentions the default priority
         self.fix_priority_help()
+        # Mostly oriented to the project copy
+        self._category = ['PCB/docs', 'Schematic/docs']
+        self._any_related = True
 
     def get_dependencies(self):
         return self.options.get_dependencies()
 
+    @staticmethod
+    def get_conf_examples(name, layers):
+        if GS.pcb_file and GS.sch_file and GS.pro_file:
+            # Add it only when we have a full project
+            register_xmp_import('ExportProject')
+        return []
+
     def run(self, output_dir):
         # No output member, just a dir
         self.options.output_dir = output_dir
         self.options.run(output_dir)
```

### Comparing `kibot-1.6.5/kibot/out_diff.py` & `kibot-1.7.0/kibot/out_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 """
 from hashlib import sha1
 from itertools import combinations
 import os
 import re
 from shutil import rmtree, copy2
 from subprocess import CalledProcessError
-from tempfile import mkdtemp
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .kiplot import load_any_sch, run_command, config_output, get_output_dir, run_output
 from .layer import Layer
 from .misc import DIFF_TOO_BIG, FAILED_EXECUTE
 from .registrable import RegOutput
 from .out_any_diff import AnyDiffOptions
@@ -367,15 +366,15 @@
             self.file = GS.sch_file
         # Place where we know we have a repo
         self.repo_dir = os.path.dirname(os.path.abspath(self.file))
         if name:
             # Checkout the target
             name_ori = name
             name = self.solve_git_name(name)
-            git_tmp_wd = mkdtemp()
+            git_tmp_wd = GS.mkdtemp('diff-checkout')
             logger.debug('Checking out '+name+' to '+git_tmp_wd)
             self.run_git(['worktree', 'add', '--detach', '--force', git_tmp_wd, name])
             self._worktrees_to_remove.append(git_tmp_wd)
             self.run_git(['submodule', 'update', '--init', '--recursive'], cwd=git_tmp_wd)
             name_copy = self.run_git(['ls-files', '--full-name', self.file])
             name_copy = os.path.join(git_tmp_wd, name_copy)
             logger.debug('- Using temporal copy: '+name_copy)
@@ -422,15 +421,15 @@
         """ The file as we interpreted it """
         if self.pcb:
             fname, dir_name = self.save_tmp_dir_board('diff')
             self.dirs_to_remove.append(dir_name)
         else:
             if self._comps:
                 # We have a variant/filter applied
-                dir_name = mkdtemp()
+                dir_name = GS.mkdtemp('diff-variant')
                 fname = GS.sch.save_variant(dir_name)
                 GS.copy_project_sch(dir_name)
                 self.dirs_to_remove.append(dir_name)
             else:
                 # Just use the current file
                 # Note: The KiCad 7 DNP field needs some filter to be honored
                 dir_name = GS.sch_dir
@@ -505,15 +504,15 @@
             self.git_command = self.ensure_tool('Git')
         if not self.pcb:
             # We need eeschema_do for this
             self.ensure_tool('KiAuto')
         # Solve the cache dir
         self.dirs_to_remove = []
         if not self.cache_dir:
-            self.cache_dir = mkdtemp()
+            self.cache_dir = GS.mkdtemp('diff-cache')
             self.dirs_to_remove.append(self.cache_dir)
         self.incl_file = None
         name_ori = name
         try:
             # List of layers
             self.incl_file = self.create_layers_incl(self.layers)
             if self.new_type == 'multivar' and self.old_type != 'multivar':
```

### Comparing `kibot-1.6.5/kibot/out_download_datasheets.py` & `kibot-1.7.0/kibot/out_download_datasheets.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_dxf.py` & `kibot-1.7.0/kibot/out_dxf.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_dxf_sch_print.py` & `kibot-1.7.0/kibot/out_dxf_sch_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_excellon.py` & `kibot-1.7.0/kibot/out_excellon.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_gencad.py` & `kibot-1.7.0/kibot/out_gencad.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_gerb_drill.py` & `kibot-1.7.0/kibot/out_gerb_drill.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_gerber.py` & `kibot-1.7.0/kibot/out_gerber.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_hpgl.py` & `kibot-1.7.0/kibot/out_hpgl.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_hpgl_sch_print.py` & `kibot-1.7.0/kibot/out_hpgl_sch_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_ibom.py` & `kibot-1.7.0/kibot/out_ibom.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     version: 2.7.0
     downloader: pytool
     id: ibom
 """
 import os
 from subprocess import (check_output, STDOUT, CalledProcessError)
 from shutil import which, rmtree
-from tempfile import mkdtemp
 from .misc import BOM_ERROR, W_EXTNAME, W_NONETLIST
 from .gs import GS
 from .out_base import VariantOptions
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
@@ -180,15 +179,15 @@
         ori_extra_data_file = self.extra_data_file
         net_dir = None
         pcb_name = GS.pcb_file
         if self.will_filter_pcb_components():
             # Write a custom netlist to a temporal dir
             prj_name = os.path.basename(self.expand_filename('', self.forced_name, 'ibom', '')) if self.forced_name \
                        else GS.pcb_basename
-            net_dir = mkdtemp(prefix='tmp-kibot-ibom-')
+            net_dir = GS.mkdtemp('ibom')
             netlist = os.path.join(net_dir, prj_name+'.xml')
             self.extra_data_file = netlist
             logger.debug('Creating variant netlist `{}`'.format(netlist))
             with open(netlist, 'wb') as f:
                 GS.sch.save_netlist(f, self._comps)
             # Write a board with the filtered values applied
             self.filter_pcb_components()
```

### Comparing `kibot-1.6.5/kibot/out_info.py` & `kibot-1.7.0/kibot/out_svg_pcb_print.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,72 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2022 Salvador E. Tropea
-# Copyright (c) 2022 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2020-2023 Salvador E. Tropea
+# Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 """
 Dependencies:
   - from: KiAuto
-    role: Show KiAuto installation information
-    version: 2.0.0
+    role: mandatory
+    version: 1.6.7
 """
 import os
-import sys
 from .gs import GS
-from .optionable import BaseOptions
-from .kiplot import run_command
+from .out_any_pcb_print import Any_PCB_PrintOptions
+from .error import KiPlotConfigurationError
+from .kicad.patch_svg import patch_svg_file
+from .kicad.pcb import PCB
+from .misc import FONT_HELP_TEXT
 from .macros import macros, document, output_class  # noqa: F401
+from .layer import Layer
 from . import log
 
 logger = log.get_logger()
 
 
-class InfoOptions(BaseOptions):
+class SVG_PCB_PrintOptions(Any_PCB_PrintOptions):
     def __init__(self):
         with document:
             self.output = GS.def_global_output
-            """ *Filename for the output (%i=info, %x=txt) """
-            self.environment = 'names'
-            """ [names,none,full] List environment variables.
-                IMPORTANT: Don't use `full` unless you know you are not leaking sensitive information """
+            """ *Filename for the output SVG (%i=layers, %x=svg)"""
+            self.enable_ki6_page_fix = True
+            """ Enable workaround for KiCad 6 bug #11033 """
+            self.enable_ki5_page_fix = True
+            """ Enable workaround for KiCad 5 bug """
         super().__init__()
-        self._expand_id = 'info'
-        self._expand_ext = 'txt'
-        self._none_related = True
-
-    def get_targets(self, out_dir):
-        return [self._parent.expand_filename(out_dir, self.output)]
-
-    def run(self, name):
-        dir = os.path.dirname(os.path.abspath(sys.argv[0]))
-        ret = run_command([os.path.join(dir, 'kibot-check'), '-p'])
-        with open(name, 'wt') as f:
-            f.write(ret+'\n')
-            # Environment
-            if self.environment == 'names':
-                f.write('\nEnvironment:\n')
-                for n in sorted(os.environ.keys()):
-                    f.write(n+'\n')
-            elif self.environment == 'full':
-                f.write('\nEnvironment:\n')
-                for n in sorted(os.environ.keys()):
-                    f.write(n+'='+os.environ[n]+'\n')
-            # KiAuto
-            command = self.check_tool('KiAuto')
-            if command:
-                ret = run_command([command, '--info'])
-                f.write('\nKiAuto:\n'+ret+'\n')
+        self._expand_ext = 'svg'
+
+    def run(self, output):
+        super().run(output, svg=True)
+        if (GS.ki6 and self.enable_ki6_page_fix) or (GS.ki5 and self.enable_ki5_page_fix):
+            # KiCad 6.0.2 bug: https://gitlab.com/kicad/code/kicad/-/issues/11033
+            o = self._parent
+            out_files = o.get_targets(o.expand_dirname(os.path.join(GS.out_dir, o.dir)))
+            is_portrait = PCB.load(GS.pcb_file).paper_portrait
+            for file in out_files:
+                patch_svg_file(file, is_portrait=is_portrait)
 
 
 @output_class
-class Info(BaseOutput):  # noqa: F821
-    """ Info
-        Records information about the current run.
-        It can be used to know more about the environment used to generate the files.
-        Please don't rely on the way things are reported, its content could change,
-        adding or removing information """
+class SVG_PCB_Print(BaseOutput):  # noqa: F821
+    """ SVG PCB Print (Scalable Vector Graphics) *Deprecated*
+        Exports the PCB to the scalable vector graphics format.
+        This output is what you get from the 'File/Print' menu in pcbnew.
+        The `pcb_print` is usually a better alternative. """
+    __doc__ += FONT_HELP_TEXT
+
     def __init__(self):
         super().__init__()
-        self._category = ['PCB/docs', 'Schematic/docs']
         with document:
-            self.options = InfoOptions
-            """ *[dict] Options for the `info` output """
-
-    @staticmethod
-    def get_conf_examples(name, layers):
-        return BaseOutput.simple_conf_examples(name, 'Information about the run', '.')  # noqa: F821
+            self.options = SVG_PCB_PrintOptions
+            """ *[dict] Options for the `pdf_pcb_print` output """
+            self.layers = Layer
+            """ *[list(dict)|list(string)|string] [all,selected,copper,technical,user,inners,outers]
+                List of PCB layers to include in the PDF """
+        self._category = 'PCB/docs'
+
+    def config(self, parent):
+        super().config(parent)
+        # We need layers
+        if isinstance(self.layers, type):
+            raise KiPlotConfigurationError("Missing `layers` list")
+        self.options.set_layers(self.layers)
```

### Comparing `kibot-1.6.5/kibot/out_kibom.py` & `kibot-1.7.0/kibot/out_kibom.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,34 @@
     github: INTI-CMNB/KiBoM
     command: KiBOM_CLI.py
     version: 1.8.0
     downloader: pytool
 """
 import os
 from re import search
-from tempfile import NamedTemporaryFile
 from .misc import BOM_ERROR, W_EXTNAME
 from .gs import GS
 from .kiplot import run_command
 from .optionable import Optionable, BaseOptions
 from .error import KiPlotConfigurationError
 from .bom.columnlist import ColumnList
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
 CONFIG_FILENAME = 'config.kibom.ini'
+SIMPLE_CONFIG = """[BOM_OPTIONS]
+output_file_name = %O
+hide_pcb_info = 1
+
+[IGNORE_COLUMNS]
+
+[REGEX_EXCLUDE]
+Part\t.*
+"""
 
 
 class KiBoMRegex(Optionable):
     """ Implements the pair column/regex """
     def __init__(self):
         super().__init__()
         self._unknown_is_error = True
@@ -184,38 +192,29 @@
             self.columns = KiBoMColumns
             """ *[list(dict)|list(string)] List of columns to display.
                 Can be just the name of the field """
 
     @staticmethod
     def _create_minimal_ini():
         """ KiBoM config to get only the headers """
-        with NamedTemporaryFile(mode='w', delete=False) as f:
-            f.write('[BOM_OPTIONS]\n')
-            f.write('output_file_name = %O\n')
-            f.write('hide_pcb_info = 1\n')
-            f.write('\n[IGNORE_COLUMNS]\n')
-            f.write('\n[REGEX_EXCLUDE]\n')
-            f.write('Part\t.*\n')
-            f.close()
-            return f.name
+        return GS.tmp_file(content=SIMPLE_CONFIG, what='minimal INI', a_logger=logger)
 
     @staticmethod
     def _get_columns():
         """ Create a list of valid columns """
         if not GS.sch:
             return ColumnList.COLUMNS_DEFAULT
         command = GS.ensure_tool('kibom', 'KiBoM')
         config = None
         csv = None
         columns = None
         try:
             xml = GS.sch_no_ext+'.xml'
             config = os.path.abspath(KiBoMConfig._create_minimal_ini())
-            with NamedTemporaryFile(mode='w', suffix='.csv', delete=False) as f:
-                csv = f.name
+            csv = GS.tmp_file(suffix='.csv')
             cmd = [command, '--cfg', config, '-d', os.path.dirname(csv), '-s', ',', xml, csv]
             run_command(cmd, err_msg='Failed to get the column names for `'+xml+'`, error {ret}', err_lvl=BOM_ERROR)
             with open(csv, 'rt') as f:
                 columns = f.readline().rstrip().split(',')
         finally:
             if config:
                 os.remove(config)
```

### Comparing `kibot-1.6.5/kibot/out_kicanvas.py` & `kibot-1.7.0/kibot/out_kicanvas.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_kicost.py` & `kibot-1.7.0/kibot/out_kicost.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 Dependencies:
   - from: KiCost
     role: mandatory
     version: 1.1.7
 """
 import os
 from os.path import isfile, abspath, join, dirname
-from tempfile import mkdtemp
 from shutil import rmtree
 from .misc import (BOM_ERROR, DISTRIBUTORS, W_UNKDIST, ISO_CURRENCIES, W_UNKCUR, KICOST_SUBMODULE,
                    W_KICOSTFLD, W_MIXVARIANT)
 from .error import KiPlotConfigurationError
 from .optionable import Optionable
 from .gs import GS
 from .out_base import VariantOptions
@@ -152,15 +151,15 @@
             if self.variant and self.variant.type == 'kicost' and self.variant.variant_field not in var_fields:
                 # Warning about KiCost limitations
                 logger.warning(W_KICOSTFLD+'KiCost variant `{}` defines `variant_field` as `{}`, not supported by KiCost'.
                                format(self.variant, self.variant.variant_field))
             if self.kicost_variant:
                 logger.warning(W_MIXVARIANT+'Avoid using KiCost variants and internal variants on the same output')
             # Write a custom netlist to a temporal dir
-            net_dir = mkdtemp(prefix='tmp-kibot-kicost-')
+            net_dir = GS.mkdtemp('kicost')
             netlist = os.path.join(net_dir, GS.sch_basename+'.xml')
             logger.debug('Creating variant netlist `{}`'.format(netlist))
             with open(netlist, 'wb') as f:
                 GS.sch.save_netlist(f, self._comps, no_field=var_fields)
         else:
             # Make sure the XML is there.
             # Currently we only support the XML mechanism.
```

### Comparing `kibot-1.6.5/kibot/out_kikit_present.py` & `kibot-1.7.0/kibot/out_kikit_present.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import glob
 import os
 import shutil
 import stat
 import subprocess
 import sys
-from tempfile import NamedTemporaryFile, TemporaryDirectory, mkdtemp
+from tempfile import TemporaryDirectory
 from .error import KiPlotConfigurationError
 from .misc import PCB_GENERATORS, RENDERERS, W_MORERES
 from .gs import GS
 from .kiplot import config_output, run_output, get_output_dir, load_board, run_command, configure_and_run
 from .optionable import BaseOptions, Optionable
 from .out_base import BaseOutput
 from .registrable import RegOutput
@@ -31,18 +31,17 @@
 from . import log
 
 
 logger = log.get_logger()
 
 
 def _get_tmp_name(ext):
-    with NamedTemporaryFile(mode='w', suffix='.'+ext, delete=False) as f:
-        f.close()
-    os.chmod(f.name, stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH)
-    return f.name
+    fname = GS.tmp_file(suffix='.'+ext)
+    os.chmod(fname, stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH)
+    return fname
 
 
 class PresentBoards(Optionable):
     def __init__(self):
         super().__init__()
         with document:
             self.mode = 'local'
@@ -249,15 +248,15 @@
                                            format(self.external_config, sub_dir))
         if len(res) > 1:
             logger.warning(W_MORERES+'`{}` generated more than one file at `{}`'.
                            format(self.external_config, sub_dir))
         return res[0]
 
     def solve_external(self):
-        tmp_dir = mkdtemp()
+        tmp_dir = GS.mkdtemp('kikit_present')
         self.temporals.append(tmp_dir)
         fname = self.new_pcb if self.solve_pcb(load_it=False) else GS.pcb_file
         cmd = [sys.argv[0], '-c', self.external_config, '-b', fname, '-d', tmp_dir]
         run_command(cmd)
         front_image = self.get_ext_file(tmp_dir, 'front')
         back_image = self.get_ext_file(tmp_dir, 'back')
         gerbers = self.get_ext_file(tmp_dir, 'gerbers')
```

### Comparing `kibot-1.6.5/kibot/out_kiri.py` & `kibot-1.7.0/kibot/out_kiri.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 """
 import datetime
 import glob
 import pwd
 import os
 from shutil import copy2, rmtree
 from subprocess import CalledProcessError
-from tempfile import mkdtemp
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .kicad.color_theme import load_color_theme
 from .kiplot import load_any_sch, run_command
 from .layer import Layer
 from .misc import W_NOTHCMP
 from .out_any_diff import AnyDiffOptions
@@ -288,15 +287,15 @@
                     dst_dir = os.path.join(self.cache_dir, hash[:7])
                     already_generated = os.path.isdir(dst_dir)
                     if self.keep_generated and already_generated:
                         logger.debug(f'- Images for {hash} already generated')
                         continue
                     if already_generated:
                         rmtree(dst_dir)
-                    git_tmp_wd = mkdtemp()
+                    git_tmp_wd = GS.mkdtemp('kiri-checkout')
                     logger.debug('Checking out '+hash+' to '+git_tmp_wd)
                     self.run_git(['worktree', 'add', '--detach', '--force', git_tmp_wd, hash])
                     self.run_git(['submodule', 'update', '--init', '--recursive'], cwd=git_tmp_wd)
                     # Generate SVGs for the schematic
                     name_sch = self.do_cache(self.sch_rel_name, git_tmp_wd, hash)
                     # Generate SVGs for the PCB
                     self.do_cache(self.pcb_rel_name, git_tmp_wd, hash)
```

### Comparing `kibot-1.6.5/kibot/out_navigate_results.py` & `kibot-1.7.0/kibot/out_navigate_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 import base64
 import os
 import subprocess
 import pprint
 from shutil import copy2
 from math import ceil
 from struct import unpack
-from tempfile import NamedTemporaryFile
 from .bom.kibot_logo import KIBOT_LOGO, KIBOT_LOGO_W, KIBOT_LOGO_H
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .optionable import Optionable, BaseOptions
 from .kiplot import config_output, get_output_dir, run_command
-from .misc import W_NOTYET, W_MISSTOOL, W_NOOUTPUTS, read_png
+from .misc import W_NOTYET, W_MISSTOOL, W_NOOUTPUTS, read_png, force_list
+from .pre_base import BasePreFlight
 from .registrable import RegOutput
 from .macros import macros, document, output_class  # noqa: F401
 from . import log, __version__
 
 logger = log.get_logger()
 CAT_IMAGE = {'PCB': 'pcbnew',
              'Schematic': 'eeschema',
@@ -94,15 +94,16 @@
              'gz': 'file_gz',
              'tar': 'file_tar',
              'zip': 'file_zip',
              'kicad_pcb': 'pcbnew',
              'sch': 'eeschema',
              'kicad_sch': 'eeschema',
              'blend': 'file_blend',
-             'pcb3d': 'file_pcb3d'}
+             'pcb3d': 'file_pcb3d',
+             'json': 'file_json'}
 for i in range(31):
     n = str(i)
     EXT_IMAGE['gl'+n] = 'file_gbr'
     EXT_IMAGE['g'+n] = 'file_gbr'
     EXT_IMAGE['gp'+n] = 'file_gbr'
 CAT_REP = {'PCB': ['pdf_pcb_print', 'svg_pcb_print', 'pcb_print'],
            'Schematic': ['pdf_sch_print', 'svg_sch_print']}
@@ -407,16 +408,15 @@
         fname = os.path.join(self.out_dir, 'images', out_name+'_'+bfname+'.png')
         # Full path for the icon image
         icon = os.path.join(self.out_dir, img)
         if ext == 'pdf':
             # Only page 1
             file += '[0]'
         if ext == 'svg':
-            with NamedTemporaryFile(mode='w', suffix='.png', delete=False) as f:
-                tmp_name = f.name
+            tmp_name = GS.tmp_file(suffix='.png')
             logger.debug('Temporal convert: {} -> {}'.format(file, tmp_name))
             if not self.svg_to_png(file, tmp_name, BIG_ICON):
                 return False, None, None
             file = tmp_name
         cmd = [self.convert_command, file,
                # Size for the big icons (width)
                '-resize', str(BIG_ICON)+'x']
@@ -534,27 +534,35 @@
             oname = oname[0].upper()+oname[1:]
             if out.comment:
                 oname += ': '+out.comment
             f.write('<thead><tr><th colspan="{}">{}</th></tr></thead>\n'.format(OUT_COLS, oname))
             out_dir = get_output_dir(out.dir, out, dry=True)
             f.write('<tbody><tr>\n')
             targets, icons = out.get_navigate_targets(out_dir)
+            c_targets = len(targets)
+            # Make the icons a list with same len as targets
+            if icons is None:
+                icons = [None]*c_targets
+            else:
+                c_icons = len(icons)
+                if c_icons < c_targets:
+                    icons.extend([None]*(c_targets-c_icons))
             if len(targets) == 1:
                 tg_rel = os.path.relpath(os.path.abspath(targets[0]), start=self.out_dir)
                 img, _ = self.get_image_for_file(targets[0], out_name, image=icons[0] if icons else None)
                 f.write('<td class="out-cell" colspan="{}"><a href="{}">{}</a></td>\n'.
                         format(OUT_COLS, tg_rel, img))
             else:
                 c = 0
-                for tg in targets:
+                for tg, icon in zip(targets, icons):
                     if c == OUT_COLS:
                         f.write('</tr>\n<tr>\n')
                         c = 0
                     tg_rel = os.path.relpath(os.path.abspath(tg), start=self.out_dir)
-                    img, wide = self.get_image_for_file(tg, out_name)
+                    img, wide = self.get_image_for_file(tg, out_name, image=icon)
                     # Check if we need to break this row
                     span = 1
                     if wide:
                         span = BIG_2_MID_REL
                         remain = OUT_COLS-c
                         if span > remain:
                             f.write('<td class="out-cell" colspan="{}"></td></tr>\n<tr>\n'.format(remain))
@@ -614,24 +622,30 @@
         if isinstance(list(node.values())[0], dict):
             self.get_html_names_cat(name, node, prev, category, files)
         else:
             files.append(os.path.join(self.out_dir, name))
 
     def create_tree(self):
         o_tree = {}
+        BasePreFlight.configure_all()
+        for n in BasePreFlight.get_in_use_names():
+            pre = BasePreFlight.get_preflight(n)
+            cat = force_list(pre.get_category())
+            if not cat:
+                continue
+            for c in cat:
+                self.add_to_tree(c, pre, o_tree)
         for o in RegOutput.get_outputs():
             if not o.run_by_default and self.skip_not_run:
                 # Skip outputs that aren't generated in a regular run
                 continue
             config_output(o)
-            cat = o.category
+            cat = force_list(o.category)
             if cat is None:
                 continue
-            if isinstance(cat, str):
-                cat = [cat]
             for c in cat:
                 self.add_to_tree(c, o, o_tree)
         return o_tree
 
     def generate_navbar_one(self, node, lvl, name, ext):
         """ Recursively create a menu containing all outputs.
             Using ul and li items """
```

### Comparing `kibot-1.6.5/kibot/out_netlist.py` & `kibot-1.7.0/kibot/out_netlist.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_panelize.py` & `kibot-1.7.0/kibot/out_panelize.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     version: 1.5.1
 """
 import collections
 from copy import deepcopy
 import os
 import re
 import json
-from tempfile import NamedTemporaryFile
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .kiplot import run_command, config_output, register_xmp_import
 from .layer import Layer
 from .misc import W_PANELEMPTY, KIKIT_UNIT_ALIASES, W_KEEPTMP
 from .optionable import PanelOptions
 from .out_base import VariantOptions
@@ -756,24 +755,21 @@
         for c, cfg in enumerate(self.configs):
             if isinstance(cfg, str):
                 continue
             if not cfg.name:
                 cfg.name = str(c+1)
 
     def create_config(self, cfg):
-        with NamedTemporaryFile(mode='w', delete=False, suffix='.json', prefix='kibot_panel_cfg') as f:
-            logger.debug('Writing panel config to '+f.name)
-            cfg_d = {}
-            for k, v in cfg.get_attrs_gen():
-                if isinstance(v, PanelOptions):
-                    cfg_d[k] = {ky: va for ky, va in v.get_attrs_gen() if va is not None and v.get_user_defined(ky)}
-            js = json.dumps(cfg_d, indent=4)
-            logger.debugl(1, js)
-            f.write(js)
-            return f.name
+        cfg_d = {}
+        for k, v in cfg.get_attrs_gen():
+            if isinstance(v, PanelOptions):
+                cfg_d[k] = {ky: va for ky, va in v.get_attrs_gen() if va is not None and v.get_user_defined(ky)}
+        js = json.dumps(cfg_d, indent=4)
+        logger.debugl(1, js)
+        return GS.tmp_file(content=js, suffix='.json', prefix='panel_cfg', what='panel config', a_logger=logger)
 
     def create_preview_file(self, name):
         if not self.create_preview or not os.path.isfile(name):
             return
         img_name = os.path.splitext(name)[0]+'.png'
         tree = {'name': '_temporal_pcbdraw_preview',
                 'type': 'pcbdraw',
```

### Comparing `kibot-1.6.5/kibot/out_pcb2blender_tools.py` & `kibot-1.7.0/kibot/out_pcb2blender_tools.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_pcb_print.py` & `kibot-1.7.0/kibot/out_pcb_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from copy import deepcopy
 import datetime
 import re
 import os
 import importlib
 from pcbnew import B_Cu, B_Mask, F_Cu, F_Mask, FromMM, IsCopperLayer, LSET, PLOT_CONTROLLER, PLOT_FORMAT_SVG
 from shutil import rmtree
-from tempfile import NamedTemporaryFile, mkdtemp
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .optionable import Optionable
 from .out_base import VariantOptions
 from .kicad.color_theme import load_color_theme
 from .kicad.patch_svg import patch_svg_file
 from .kicad.config import KiConf
@@ -172,18 +171,22 @@
             """ [number=0] Horizontal margin used for the autoscaling mode [mm] """
             self.autoscale_margin_y = None
             """ [number=0] Vertical margin used for the autoscaling mode [mm] """
             self.title = ''
             """ Text used to replace the sheet title. %VALUE expansions are allowed.
                 If it starts with `+` the text is concatenated """
             self.sheet = 'Assembly'
-            """ Text to use for the `sheet` in the title block.
+            """ Text to use for the `SHEET` in the title block.
                 Pattern (%*) and text variables are expanded.
+                The %ll is the list of layers included in this page.
                 In addition when you use `repeat_for_layer` the following patterns are available:
-                %ln layer name, %ls layer suffix and %ld layer description """
+                %ln layer name, %ls layer suffix and %ld layer description  """
+            self.layer_var = '%ll'
+            """ Text to use for the `LAYER` in the title block.
+                All the expansions available for `sheet` are also available here """
             self.sheet_reference_color = ''
             """ Color to use for the frame and title block """
             self.line_width = 0.1
             """ [0.02,2] For objects without width [mm] (KiCad 5) """
             self.negative_plot = False
             """ Invert black and white. Only useful for a single layer """
             self.exclude_pads_from_silkscreen = False
@@ -218,20 +221,21 @@
             self.repeat_inherit = True
             """ If we will inherit the options of the layer we are replacing.
                 Disable it if you specify the options in `repeat_layers`, which is unlikely """
         self._scaling_example = 1.0
         self._autoscale_margin_x_example = 0
         self._autoscale_margin_y_example = 0
 
-    def expand_sheet_patterns(self, parent, layer=None):
+    def expand_sheet_patterns(self, parent, sheet, layers, layer=None):
+        sheet = sheet.replace('%ll', layers)
         if layer:
-            self.sheet = self.sheet.replace('%ln', layer.layer)
-            self.sheet = self.sheet.replace('%ls', layer.suffix)
-            self.sheet = self.sheet.replace('%ld', layer.description)
-        self.sheet = self.expand_filename_pcb(self.sheet)
+            sheet = sheet.replace('%ln', layer.layer)
+            sheet = sheet.replace('%ls', layer.suffix)
+            sheet = sheet.replace('%ld', layer.description)
+        return self.expand_filename_pcb(sheet)
 
     def config(self, parent):
         super().config(parent)
         if isinstance(self.layers, type):
             raise KiPlotConfigurationError("Missing `layers` list")
         # Fill the ID member for all the layers
         self.layers = LayerOptions.solve(self.layers)
@@ -294,15 +298,15 @@
             self.frame_plot_mechanism = 'internal'
             """ [gui,internal,plot] Plotting the frame from Python is problematic.
                 This option selects a workaround strategy.
                 gui: uses KiCad GUI to do it. Is slow but you get the correct frame.
                 But it can't keep track of page numbers.
                 internal: KiBot loads the `.kicad_wks` and does the drawing work.
                 Best option, but some details are different from what the GUI generates.
-                plot: uses KiCad Python API. Only available for KiCad 6.
+                plot: uses KiCad Python API. Not available for KiCad 5.
                 You get the default frame and some substitutions doesn't work """
             self.pages = PagesOptions
             """ *[list(dict)] List of pages to include in the output document.
                 Each page contains one or more layers of the PCB """
             self.title = ''
             """ Text used to replace the sheet title. %VALUE expansions are allowed.
                 If it starts with `+` the text is concatenated """
@@ -362,31 +366,42 @@
             """ Invert the meaning of the `use_for_center` layer option.
                 This can be used to just select the edge cuts for centering, in this case enable this option
                 and disable the `use_for_center` option of the edge cuts layer """
         add_drill_marks(self)
         super().__init__()
         self._expand_id = 'assembly'
 
+    def get_layers_for_page(self, page):
+        layer = ''
+        for la in page.layers:
+            if len(layer):
+                layer += '+'
+            layer = layer+la.layer
+        return layer
+
     def config(self, parent):
         super().config(parent)
         if isinstance(self.pages, type):
             raise KiPlotConfigurationError("Missing `pages` list")
         # Expand any repeat_for_layer
         pages = []
         for page in self.pages:
+            layers_for_page = self.get_layers_for_page(page)
             if page.repeat_for_layer:
                 for la in page._repeat_layers:
                     new_page = deepcopy(page)
                     if page.repeat_inherit:
                         la.copy_extra_from(page._repeat_for_layer)
                     new_page.layers[page._repeat_for_layer_index] = la
-                    new_page.expand_sheet_patterns(parent, la)
+                    page.sheet = new_page.expand_sheet_patterns(parent, page.sheet, la.layer+'+'+layers_for_page, la)
+                    page.layer_var = new_page.expand_sheet_patterns(parent, page.layer_var, la.layer+'+'+layers_for_page, la)
                     pages.append(new_page)
             else:
-                page.expand_sheet_patterns(parent)
+                page.sheet = page.expand_sheet_patterns(parent, page.sheet, layers_for_page)
+                page.layer_var = page.expand_sheet_patterns(parent, page.layer_var, layers_for_page)
                 pages.append(page)
         self.pages = pages
         # Color theme
         self._color_theme = load_color_theme(self.color_theme)
         if self._color_theme is None:
             raise KiPlotConfigurationError("Unable to load `{}` color theme".format(self.color_theme))
         # Assign a color if none was defined
@@ -490,20 +505,15 @@
         vars['REVISION'] = GS.pcb_rev
         # The set_title member already took care of modifying the board value
         tb = GS.board.GetTitleBlock()
         vars['TITLE'] = tb.GetTitle()
         vars['FILENAME'] = GS.pcb_basename+'.kicad_pcb'
         vars['SHEETNAME'] = p.sheet
         vars['SHEETPATH'] = ''  # Only relevant for an schematic
-        layer = ''
-        for la in p.layers:
-            if len(layer):
-                layer += '+'
-            layer = layer+la.layer
-        vars['LAYER'] = layer
+        vars['LAYER'] = p.layer_var
         vars['PAPER'] = self.paper
         return vars
 
     def plot_frame_internal(self, pc, po, p, page, pages):
         """ Here we plot the frame manually """
         self.clear_layer('Edge.Cuts')
         po.SetPlotFrameRef(False)
@@ -700,17 +710,15 @@
     def add_frame_images(self, svg, monochrome):
         if (not self.plot_sheet_reference or not self.frame_plot_mechanism == 'internal' or
            not self.last_worksheet.has_images):
             return
         if monochrome:
             convert_command = self.ensure_tool('ImageMagick')
             for img in self.last_worksheet.images:
-                with NamedTemporaryFile(mode='wb', suffix='.png', delete=False) as f:
-                    f.write(img.data)
-                    fname = f.name
+                fname = GS.tmp_file(content=img.data, suffix='.png', binary=True)
                 dest = fname.replace('.png', '_gray.png')
                 _run_command([convert_command, fname, '-set', 'colorspace', 'Gray', '-separate', '-average', dest])
                 with open(dest, 'rb') as f:
                     img.data = f.read()
                 os.remove(fname)
                 os.remove(dest)
         self.last_worksheet.add_images_to_svg(svg, self.svg_precision)
@@ -1125,20 +1133,17 @@
                             g.SetHorizJustify(-g.GetHorizJustify())
 
     def generate_output(self, output):
         self.check_tools()
         # Avoid KiCad 5 complaining about fake vias diameter == drill == 0
         self.min_w = 2 if GS.ki5 else 0
         output_dir = os.path.dirname(output)
-        if self.keep_temporal_files:
-            temp_dir_base = output_dir
-        else:
-            temp_dir_base = mkdtemp(prefix='tmp-kibot-pcb_print-')
-        logger.debug('Starting to generate `{}`'.format(output))
-        logger.debug('- Temporal dir: {}'.format(temp_dir_base))
+        temp_dir_base = output_dir if self.keep_temporal_files else GS.mkdtemp('pcb_print')
+        logger.debug(f'Starting to generate `{output}`')
+        logger.debug(f'- Temporal dir: {temp_dir_base}')
         self.find_paper_size()
         if self.sheet_reference_layout:
             layout = self.sheet_reference_layout
         else:
             # Find the layout file
             layout = KiConf.fix_page_layout(GS.pro_file, dry=True)[1]
         if not layout or not os.path.isfile(layout):
```

### Comparing `kibot-1.6.5/kibot/out_pcb_variant.py` & `kibot-1.7.0/kibot/out_pcb_variant.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_pcbdraw.py` & `kibot-1.7.0/kibot/out_pcbdraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
   - name: numpy
     python_module: true
     debian: python3-numpy
     arch: python-numpy
     downloader: python
     role: Automatically adjust SVG margin
 """
+PROFILE_PLOT = False
+if PROFILE_PLOT:
+    import cProfile
 import os
-from tempfile import NamedTemporaryFile
 # Here we import the whole module to make monkeypatch work
 from .error import KiPlotConfigurationError
 from .kiplot import load_sch, get_board_comps_data, run_command
 from .misc import (PCBDRAW_ERR, PCB_MAT_COLORS, PCB_FINISH_COLORS, SOLDER_COLORS, SILK_COLORS, W_PCBDRAW)
 from .gs import GS
 from .layer import Layer
 from .optionable import Optionable
@@ -39,20 +41,14 @@
     return int(val * 1000000)
 
 
 def pcbdraw_warnings(tag, msg):
     logger.warning('{}({}) {}'.format(W_PCBDRAW, tag, msg))
 
 
-def _get_tmp_name(ext):
-    with NamedTemporaryFile(mode='w', suffix=ext, delete=False) as f:
-        f.close()
-    return f.name
-
-
 def _run_command(cmd):
     run_command(cmd, err_lvl=PCBDRAW_ERR)
 
 
 class PcbDrawStyle(Optionable):
     def __init__(self):
         super().__init__()
@@ -428,19 +424,19 @@
         svg_save_output_name = save_output_name = name
         self.rsvg_command = None
         self.convert_command = None
         # Check we have the tools needed for the output format
         if self.format != 'svg':
             # We need RSVG for anything other than SVG
             self.rsvg_command = self.ensure_tool('RSVG')
-            svg_save_output_name = _get_tmp_name('.svg')
+            svg_save_output_name = GS.tmp_file(suffix='.svg')
             # We need ImageMagick for anything other than SVG and PNG
             if self.format != 'png':
                 self.convert_command = self.ensure_tool('ImageMagick')
-                save_output_name = _get_tmp_name('.png')
+                save_output_name = GS.tmp_file(suffix='.png')
 
         try:
             plotter = PcbPlotter(board)
             # Read libs from KiBot resources
             plotter.setup_arbitrary_data_path(GS.get_resource_path('pcbdraw'))
             # Libs indicated by PCBDRAW_LIB_PATH
             plotter.setup_env_data_path()
@@ -475,16 +471,24 @@
             if self.placeholder:
                 plotter.plot_plan.append(PlotPlaceholders())
             plotter.compute_bbox = self.size_detection == 'svg_paths'
             # Make sure we can use svgpathtools
             if plotter.compute_bbox:
                 self.ensure_tool('numpy')
             plotter.kicad_bb_only_edge = self.size_detection == 'kicad_edge'
-
-            image = plotter.plot()
+            # Plot it
+            if PROFILE_PLOT:
+                logger.error('Start')
+                with cProfile.Profile() as pr:
+                    image = plotter.plot()
+                    pr.print_stats(sort='time')
+                    pr.print_stats(sort='cumulative')
+                logger.error('End')
+            else:
+                image = plotter.plot()
         # Most errors are reported as RuntimeError
         # When the PCB can't be loaded we get IOError
         # When the SVG contains errors we get SyntaxError
         except (RuntimeError, SyntaxError, IOError) as e:
             GS.exit_with_error('PcbDraw error: '+str(e), PCBDRAW_ERR)
 
         # Save the result
```

### Comparing `kibot-1.6.5/kibot/out_pdf.py` & `kibot-1.7.0/kibot/out_pdf.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_pdf_pcb_print.py` & `kibot-1.7.0/kibot/out_pdf_pcb_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_pdf_sch_print.py` & `kibot-1.7.0/kibot/out_pdf_sch_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_pdfunite.py` & `kibot-1.7.0/kibot/out_pdfunite.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_populate.py` & `kibot-1.7.0/kibot/out_populate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,30 @@
 #   - name: mistune
 #     python_module: true
 #     debian: python3-mistune
 #     arch: python-mistune
 #     role: mandatory
 # """
 import os
-from tempfile import NamedTemporaryFile
 # Here we import the whole module to make monkeypatch work
 from .error import KiPlotConfigurationError
 from .misc import W_PCBDRAW, RENDERERS
 from .gs import GS
 from .kiplot import run_output, look_for_output
 from .optionable import Optionable
 from .out_base import VariantOptions
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
-
-
 logger = log.get_logger()
 
 
 def pcbdraw_warnings(tag, msg):
     logger.warning('{}({}) {}'.format(W_PCBDRAW, tag, msg))
 
 
-def _get_tmp_name(ext):
-    with NamedTemporaryFile(mode='w', suffix=ext, delete=False) as f:
-        f.close()
-    return f.name
-
-
 class PopulateOptions(VariantOptions):
     def __init__(self):
         with document:
             self.renderer = ''
             """ *Name of the output used to render the PCB steps.
                 Currently this must be a `pcbdraw` or `render_3d` output """
             self.template = 'simple'
```

### Comparing `kibot-1.6.5/kibot/out_position.py` & `kibot-1.7.0/kibot/out_position.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_ps.py` & `kibot-1.7.0/kibot/out_ps.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_ps_sch_print.py` & `kibot-1.7.0/kibot/out_ps_sch_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_qr_lib.py` & `kibot-1.7.0/kibot/out_qr_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,51 +8,36 @@
   - name: QRCodeGen
     role: mandatory
     python_module: true
     downloader: python
     debian: python3-qrcodegen
 """
 import os
-from tempfile import NamedTemporaryFile
 from .gs import GS
 from .optionable import BaseOptions, Optionable
 from .error import KiPlotConfigurationError
-from .kicad.sexpdata import Symbol, dumps, Sep, load, SExpData, sexp_iter
+from .kicad.pcb import save_pcb_from_sexp
+from .kicad.sexpdata import Symbol, dumps, Sep, sexp_iter
+from .kicad.sexp_helpers import make_separated, load_sexp_file
 from .kicad.v6_sch import DrawRectangleV6, PointXY, Stroke, Fill, SchematicFieldV6, FontEffects
-from .kiplot import load_board
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 try:
     import qrcodegen
 except ImportError:
     qrcodegen = None
 
 logger = log.get_logger()
-TO_SEPARATE = {'kicad_pcb', 'general', 'title_block', 'layers', 'setup', 'pcbplotparams', 'net_class', 'module',
-               'kicad_sch', 'lib_symbols', 'symbol', 'sheet', 'sheet_instances', 'symbol_instances'}
 SHEET_FILE = {'Sheet file', 'Sheetfile'}
 
 
 def is_symbol(name, sexp):
     return isinstance(sexp, list) and len(sexp) >= 1 and isinstance(sexp[0], Symbol) and sexp[0].value() == name
 
 
-def make_separated(sexp):
-    if not isinstance(sexp, list):
-        return sexp
-    if not isinstance(sexp[0], Symbol) or sexp[0].value() not in TO_SEPARATE:
-        return sexp
-    separated = []
-    for s in sexp:
-        separated.append(make_separated(s))
-        if isinstance(s, list):
-            separated.append(Sep())
-    return separated
-
-
 def compute_size(qr, is_sch=True, use_mm=True):
     if is_sch:
         qrc = qr._code_sch
         full_size = qr.size_sch
     else:
         qrc = qr._code_pcb
         full_size = qr.size_pcb
@@ -376,48 +361,29 @@
                 elif s[2][0] == ' ':
                     logger.debug('- Updating text `{}`'.format(qr._text_pcb))
                     s[2] = ' '+qr._text_pcb
 
     def update_footprints(self, known_qrs):
         # Replace known QRs in the PCB
         updated = False
-        pcb = self.load_sexp_file(GS.pcb_file)
+        pcb = load_sexp_file(GS.pcb_file)
         for iter in [sexp_iter(pcb, 'kicad_pcb/module'), sexp_iter(pcb, 'kicad_pcb/footprint')]:
             for s in iter:
                 if len(s) < 2:
                     continue
                 if isinstance(s[1], Symbol):
                     name = s[1].value().lower()
                 else:
                     name = s[1].lower()
                 if name in known_qrs:
                     updated = True
                     self.update_footprint(name, s, known_qrs[name])
         # Save the resulting PCB
         if updated:
-            # Make it readable
-            separated = make_separated(pcb[0])
-            # Save it to a temporal
-            with NamedTemporaryFile(mode='wt', suffix='.kicad_pcb', delete=False) as f:
-                logger.debug('- Saving updated PCB to: '+f.name)
-                f.write(dumps(separated))
-                f.write('\n')
-                tmp_pcb = f.name
-            # Also copy the project
-            GS.copy_project(tmp_pcb)
-            # Reload it
-            logger.debug('- Loading the temporal PCB')
-            load_board(tmp_pcb, forced=True)
-            # Create a back-up and save it in the original place
-            logger.debug('- Replacing the old PCB')
-            os.remove(tmp_pcb)
-            GS.make_bkp(GS.pcb_file)
-            GS.board.Save(GS.pcb_file)
-            # After saving the file the name isn't changed, we must force it!!!
-            GS.board.SetFileName(GS.pcb_file)
+            save_pcb_from_sexp(pcb, logger)
 
     def update_symbol(self, name, c_name, sexp, qr):
         logger.debug('- Updating QR symbol: '+name)
         # Compute the size
         qrc, size, full_size, center, size_rect = compute_size(qr)
         # Create the new drawings
         sub_unit_name = c_name+"_1_1"
@@ -465,28 +431,17 @@
             # Create a back-up and save it in the original place
             logger.debug('- Replacing the old SCH')
             GS.make_bkp(fname)
             with open(fname, 'wt') as f:
                 f.write(dumps(separated))
                 f.write('\n')
 
-    def load_sexp_file(self, fname):
-        with open(fname, 'rt') as fh:
-            error = None
-            try:
-                ki_file = load(fh)
-            except SExpData as e:
-                error = str(e)
-            if error:
-                raise KiPlotConfigurationError(error)
-        return ki_file
-
     def load_k6_sheets(self, fname, sheets=None):
         logger.debug('- Loading '+fname)
-        sheet = self.load_sexp_file(fname)
+        sheet = load_sexp_file(fname)
         if sheets is None:
             sheets = {}
         sheets[fname] = sheet
         if not is_symbol('kicad_sch', sheet[0]):
             raise KiPlotConfigurationError('No kicad_sch signature in '+fname)
         path = os.path.dirname(fname)
         for s in sexp_iter(sheet, 'kicad_sch/sheet'):
```

### Comparing `kibot-1.6.5/kibot/out_render_3d.py` & `kibot-1.7.0/kibot/out_render_3d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2021-2023 Salvador E. Tropea
-# Copyright (c) 2021-2023 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2021-2024 Salvador E. Tropea
+# Copyright (c) 2021-2024 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
 # KiCad 6/6.0.1 bug: https://gitlab.com/kicad/code/kicad/-/issues/9890
 """
 Dependencies:
   - from: KiAuto
     role: mandatory
-    version: 2.0.4
+    version: 2.3.1
   - from: ImageMagick
     role: Automatically crop images
 """
 import os
+from .error import KiPlotConfigurationError
 from .misc import (RENDER_3D_ERR, PCB_MAT_COLORS, PCB_FINISH_COLORS, SOLDER_COLORS, SILK_COLORS,
-                   KICAD_VERSION_6_0_2, MISSING_TOOL)
+                   KICAD_VERSION_6_0_2, MISSING_TOOL, W_INV3DLAYER, W_NEEDSK8, W_NEEDSK6, W_DEPR)
 from .gs import GS
 from .out_base_3d import Base3DOptionsWithHL, Base3D
 from .kiplot import run_command
 from .macros import macros, document, output_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
@@ -116,21 +117,43 @@
             """ When enabled the image will be post-processed to make the background transparent.
                 In this mode the `background1` and `background2` colors are ignored """
             self.transparent_background_color = "#00ff00"
             """ Color used for the chroma key. Adjust it if some regions of the board becomes transparent """
             self.transparent_background_fuzz = 15
             """ [0,100] Chroma key tolerance (percent). Bigger values will remove more pixels """
             self.realistic = True
-            """ When disabled we use the colors of the layers used by the GUI. KiCad 6 or newer """
+            """ When disabled we use the colors of the layers used by the GUI. Needs KiCad 6 or 7.
+                Is emulated on KiCad 8 """
+            self.force_stackup_colors = False
+            """ Tell KiCad to use the colors from the stackup. They are better than the unified KiBot colors.
+                Needs KiCad 6 or newer """
             self.show_board_body = True
             """ Show the PCB core material. KiCad 6 or newer """
             self.show_comments = False
-            """ Show the content of the User.Comments layer. KiCad 6 or newer and ray tracing disabled """
+            """ Show the content of the User.Comments and User.Drawings layer for KiCad 5, 6 and 7.
+                On KiCad 8 this option controls only the User.Comments and you have a separated option for the
+                User.Drawings called `show_drawings`
+                Note that KiCad 5/6/7 doesn't show it when `realistic` is enabled, but KiCad 8 does it.
+                Also note that KiCad 5 ray tracer shows comments outside the PCB, but newer KiCad versions
+                doesn't """
+            self.show_drawings = False
+            """ Show the content of the User.Drawings layer. Only available for KiCad 8 and newer.
+                Consult `show_comments` to learn when drawings are visible """
             self.show_eco = False
-            """ Show the content of the Eco1.User/Eco2.User layers. KiCad 6 or newer and ray tracing disabled """
+            """ Show the content of the Eco1.User/Eco2.User layers.
+                For KiCad 8 `show_eco1` and `show_eco2` are available.
+                Consult `show_comments` to learn when drawings are visible """
+            self.show_eco1 = False
+            """ Show the content of the Eco1.User layer. KiCad 8 supports individual Eco layer options, for 6 and 7
+                use the `show_eco` option.
+                Consult `show_comments` to learn when drawings are visible """
+            self.show_eco2 = False
+            """ Show the content of the Eco1.User layer. KiCad 8 supports individual Eco layer options, for 6 and 7
+                use the `show_eco` option.
+                Consult `show_comments` to learn when drawings are visible """
             self.show_adhesive = False
             """ Show the content of F.Adhesive/B.Adhesive layers. KiCad 6 or newer """
         super().__init__()
         self._expand_ext = 'png'
 
     def config(self, parent):
         # Apply global defaults
@@ -239,25 +262,50 @@
             cmd.append('--hide_zones')
         if not self.clip_silk_on_via_annulus:
             cmd.append('--dont_clip_silk_on_via_annulus')
         if not self.subtract_mask_from_silk:
             cmd.append('--dont_substrack_mask_from_silk')
         if not self.realistic:
             cmd.append('--use_layer_colors')
+        if self.force_stackup_colors:
+            cmd.append('--use_stackup_colors')
+        if self.force_stackup_colors and not self.realistic:
+            raise KiPlotConfigurationError("Choose to disable `realistic` or enable `force_stackup_colors`, not both")
         if not self.show_board_body:
             cmd.append('--hide_board_body')
         if self.show_comments:
             cmd.append('--show_comments')
+        if self.show_drawings:
+            cmd.append('--show_drawings')
         if self.show_eco:
             cmd.append('--show_eco')
+        if self.show_eco1:
+            cmd.append('--show_eco1')
+        if self.show_eco2:
+            cmd.append('--show_eco2')
         if self.show_adhesive:
             cmd.append('--show_adhesive')
+        if not GS.ki8:
+            if (self.show_comments or self.show_drawings or self.show_eco) and self.realistic:
+                logger.warning(W_INV3DLAYER+"The comments, drawings and eco layers aren't visible when realistic is enabled")
+            if self.show_drawings:
+                logger.warning(W_NEEDSK8+"`show_drawings` needs KiCad 8 or newer")
+            if self.show_eco1:
+                logger.warning(W_NEEDSK8+"`show_eco1` needs KiCad 8 or newer")
+            if self.show_eco2:
+                logger.warning(W_NEEDSK8+"`show_eco2` needs KiCad 8 or newer")
+        if not GS.ki6:
+            if self.force_stackup_colors:
+                logger.warning(W_NEEDSK6+"`force_stackup_colors` needs KiCad 6 or newer")
+            if not self.realistic:
+                logger.warning(W_NEEDSK6+"disabling `realistic` needs KiCad 6 or newer")
 
     def run(self, output):
         super().run(output)
+        logger.warning(W_DEPR+'This output depends on KiCad version, use `blender_export` instead')
         if GS.ki6 and GS.kicad_version_n < KICAD_VERSION_6_0_2:
             GS.exit_with_error("3D Viewer not supported for KiCad 6.0.0/1\n"
                                "Please upgrade KiCad to 6.0.2 or newer", MISSING_TOOL)
         command = self.ensure_tool('KiAuto')
         if self.transparent_background:
             # Use the chroma key color
             self.background1 = self.background2 = self.transparent_background_color
@@ -283,15 +331,17 @@
             _run_command([convert_command, output, '-fuzz', str(self.transparent_background_fuzz)+'%', '-transparent',
                           self.color_str_to_rgb(self.transparent_background_color), output])
 
 
 @output_class
 class Render_3D(Base3D):  # noqa: F821
     """ 3D render of the PCB
-        Exports the image generated by KiCad's 3D viewer. """
+        Exports the image generated by KiCad's 3D viewer. *Deprecated*
+        Use the Blender Export output if you want something with better quality
+        and less dependent of the KiCad version """
     def __init__(self):
         super().__init__()
         with document:
             self.options = Render3DOptions
             """ *[dict] Options for the `render_3d` output """
         self._category = 'PCB/3D'
```

### Comparing `kibot-1.6.5/kibot/out_report.py` & `kibot-1.7.0/kibot/out_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -438,44 +438,15 @@
 
     def get_attr_tests(self):
         if GS.ki5:
             return self.is_pure_smd_5, self.is_not_virtual_5
         return self.is_pure_smd_6, self.is_not_virtual_6
 
     def measure_pcb(self, board):
-        edge_layer = board.GetLayerID('Edge.Cuts')
-        x1 = y1 = x2 = y2 = None
-        for d in board.GetDrawings():
-            if d.GetClass() == GS.board_gr_type and d.GetLayer() == edge_layer:
-                bb = GS.get_shape_bbox(d)
-                start = bb.GetOrigin()
-                end = bb.GetEnd()
-                if x1 is None:
-                    x1 = x2 = start.x
-                    y1 = y2 = start.y
-                for p in [start, end]:
-                    x2 = max(x2, p.x)
-                    y2 = max(y2, p.y)
-                    x1 = min(x1, p.x)
-                    y1 = min(y1, p.y)
-        # This is a special case: the PCB edges are in a footprint
-        for m in GS.get_modules():
-            for gi in m.GraphicalItems():
-                if gi.GetClass() == GS.footprint_gr_type and gi.GetLayer() == edge_layer:
-                    bb = GS.get_shape_bbox(gi)
-                    start = bb.GetOrigin()
-                    end = bb.GetEnd()
-                    if x1 is None:
-                        x1 = x2 = start.x
-                        y1 = y2 = start.y
-                    for p in [start, end]:
-                        x2 = max(x2, p.x)
-                        y2 = max(y2, p.y)
-                        x1 = min(x1, p.x)
-                        y1 = min(y1, p.y)
+        x1, y1, x2, y2 = GS.compute_pcb_boundary(board)
         if x1 is None:
             self.bb_w = self.bb_h = INF
         else:
             self.bb_w = x2-x1
             self.bb_h = y2-y1
 
     def compute_oar(self, pad, hole):
```

### Comparing `kibot-1.6.5/kibot/out_sch_variant.py` & `kibot-1.7.0/kibot/out_sch_variant.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_stencil_3d.py` & `kibot-1.7.0/kibot/out_stencil_3d.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_stencil_for_jig.py` & `kibot-1.7.0/kibot/out_stencil_for_jig.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_step.py` & `kibot-1.7.0/kibot/out_step.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_svg.py` & `kibot-1.7.0/kibot/out_svg.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_svg_pcb_print.py` & `kibot-1.7.0/kibot/pre_sch_replace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020-2023 Salvador E. Tropea
-# Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
-# License: AGPL-3.0
+# Copyright (c) 2021-2022 Salvador E. Tropea
+# Copyright (c) 2021-2022 Instituto Nacional de Tecnología Industrial
+# License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 """
 Dependencies:
-  - from: KiAuto
-    role: mandatory
-    version: 1.6.7
+  - from: Git
+    role: Find commit hash and/or date
+  - from: Bash
+    role: Run external commands to create replacement text
 """
 import os
 from .gs import GS
-from .out_any_pcb_print import Any_PCB_PrintOptions
-from .error import KiPlotConfigurationError
-from .kicad.patch_svg import patch_svg_file
-from .kicad.pcb import PCB
-from .misc import FONT_HELP_TEXT
-from .macros import macros, document, output_class  # noqa: F401
-from .layer import Layer
+from .kiplot import load_sch
+from .pre_any_replace import TagReplaceBase, Base_ReplaceOptions, Base_Replace
+from .macros import macros, document, pre_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
 
 
-class SVG_PCB_PrintOptions(Any_PCB_PrintOptions):
+class TagReplaceSCH(TagReplaceBase):
+    """ Tags to be replaced for an SCH """
     def __init__(self):
-        with document:
-            self.output = GS.def_global_output
-            """ *Filename for the output SVG (%i=layers, %x=svg)"""
-            self.enable_ki6_page_fix = True
-            """ Enable workaround for KiCad 6 bug #11033 """
-            self.enable_ki5_page_fix = True
-            """ Enable workaround for KiCad 5 bug """
         super().__init__()
-        self._expand_ext = 'svg'
+        self._help_command += (".\nKIBOT_SCH_NAME variable is the name of the current sheet."
+                               "\nKIBOT_TOP_SCH_NAME variable is the name of the top sheet")
 
-    def run(self, output):
-        super().run(output, svg=True)
-        if (GS.ki6 and self.enable_ki6_page_fix) or (GS.ki5 and self.enable_ki5_page_fix):
-            # KiCad 6.0.2 bug: https://gitlab.com/kicad/code/kicad/-/issues/11033
-            o = self._parent
-            out_files = o.get_targets(o.expand_dirname(os.path.join(GS.out_dir, o.dir)))
-            is_portrait = PCB.load(GS.pcb_file).paper_portrait
-            for file in out_files:
-                patch_svg_file(file, is_portrait=is_portrait)
-
-
-@output_class
-class SVG_PCB_Print(BaseOutput):  # noqa: F821
-    """ SVG PCB Print (Scalable Vector Graphics) *Deprecated*
-        Exports the PCB to the scalable vector graphics format.
-        This output is what you get from the 'File/Print' menu in pcbnew.
-        The `pcb_print` is usually a better alternative. """
-    __doc__ += FONT_HELP_TEXT
 
+class SCH_ReplaceOptions(Base_ReplaceOptions):
+    """ SCH replacement options """
     def __init__(self):
         super().__init__()
-        with document:
-            self.options = SVG_PCB_PrintOptions
-            """ *[dict] Options for the `pdf_pcb_print` output """
-            self.layers = Layer
-            """ *[list(dict)|list(string)|string] [all,selected,copper,technical,user,inners,outers]
-                List of PCB layers to include in the PDF """
-        self._category = 'PCB/docs'
-
-    def config(self, parent):
-        super().config(parent)
-        # We need layers
-        if isinstance(self.layers, type):
-            raise KiPlotConfigurationError("Missing `layers` list")
-        self.options.set_layers(self.layers)
+        self._help_date_command = self._help_date_command.replace('PCB', 'SCH')
+        self.replace_tags = TagReplaceSCH
+
+
+@pre_class
+class SCH_Replace(Base_Replace):  # noqa: F821
+    """ [dict] Replaces tags in the schematic. I.e. to insert the git hash or last revision date.
+        This is useful for KiCad 5, use `set_text_variables` when using KiCad 6.
+        This preflight modifies the schematics. Even when a back-up is done use it carefully """
+    _context = 'SCH'
+
+    def __init__(self, name, value):
+        super().__init__(name, value)
+
+    def config(self):
+        o = SCH_ReplaceOptions()
+        o.set_tree(self._value)
+        o.config(self)
+        self._value = o
+
+    @classmethod
+    def get_doc(cls):
+        return cls.__doc__, SCH_ReplaceOptions
+
+    def apply(self):
+        o = self._value
+        if o.date_command:
+            # Convert it into another replacement
+            t = TagReplaceSCH()
+            if GS.ki5:
+                t.tag = r'^Date ("(?:[^"]|\\")*")$'
+                t.before = 'Date "'
+                t.after = '"'
+            else:
+                t.tag = r'\(date ("(?:[^"]|\\")*")\)'
+                t.before = '(date "'
+                t.after = '")'
+            t.command = o.date_command
+            t._relax_check = True
+            o.replace_tags.append(t)
+        load_sch()
+        os.environ['KIBOT_TOP_SCH_NAME'] = GS.sch_file
+        for file in GS.sch.get_files():
+            self.replace(file)
+        # Force the schematic reload
+        GS.sch = None
```

### Comparing `kibot-1.6.5/kibot/out_svg_sch_print.py` & `kibot-1.7.0/kibot/out_svg_sch_print.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/out_vrml.py` & `kibot-1.7.0/kibot/out_vrml.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/pre_annotate_pcb.py` & `kibot-1.7.0/kibot/pre_annotate_pcb.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,21 +120,24 @@
 @pre_class
 class Annotate_PCB(BasePreFlight):  # noqa: F821
     """ [dict] Annotates the PCB according to physical coordinates.
         This preflight modifies the PCB and schematic, use it only in revision control environments.
         Used to assign references according to footprint coordinates.
         The project must be fully annotated first """
     def __init__(self, name, value):
-        o = Annotate_PCBOptions()
-        o.set_tree(value)
-        o.config(self)
-        super().__init__(name, o)
+        super().__init__(name, value)
         self._sch_related = True
         self._pcb_related = True
 
+    def config(self):
+        o = Annotate_PCBOptions()
+        o.set_tree(self._value)
+        o.config(self)
+        self._value = o
+
     @classmethod
     def get_doc(cls):
         return cls.__doc__, Annotate_PCBOptions
 
     def get_example():
         """ Returns a YAML value for the example config """
         return ("\n    top_main_axis: y"
```

### Comparing `kibot-1.6.5/kibot/pre_annotate_power.py` & `kibot-1.7.0/kibot/pre_annotate_power.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2022 Salvador E. Tropea
 # Copyright (c) 2022 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
-from .error import KiPlotConfigurationError
 from .gs import (GS)
 from .kiplot import load_sch
 from .misc import W_NOANNO
 from .macros import macros, pre_class  # noqa: F401
 from .log import get_logger
 
 logger = get_logger(__name__)
@@ -16,17 +15,14 @@
 @pre_class
 class Annotate_Power(BasePreFlight):  # noqa: F821
     """ [boolean=false] Annotates all power components.
         This preflight modifies the schematic, use it only in revision control environments.
         Used to solve ERC problems when using filters that remove power reference numbers """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
         self._sch_related = True
 
     def annotate_ki5(self):
         """ Annotate power components for KiCad 5 """
         comps = GS.sch.get_components(exclude_power=False)
         num = 1
         for c in comps:
```

### Comparing `kibot-1.6.5/kibot/pre_any_replace.py` & `kibot-1.7.0/kibot/pre_any_replace.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/pre_base.py` & `kibot-1.7.0/kibot/pre_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,48 @@
 
 
 class BasePreFlight(Registrable):
     _registered = {}
     _in_use = {}
     _options = {}
     _targets = None
+    _configured = False
 
     def __init__(self, name, value):
         super().__init__()
         self._value = value
         self._name = name
         self._sch_related = False
         self._pcb_related = False
+        self._any_related = False    # True if we need an schematic OR a PCB
         self._enabled = True
         self._expand_id = ''
         self._expand_ext = ''
         self._files_to_remove = []
+        self._category = None
+        # Compatibility with outputs
+        self.name = name
+        self.comment = ''
+
+    def config(self):
+        """ Default configuration assumes this is just a boolean """
+        if not isinstance(self._value, bool):
+            raise KiPlotConfigurationError('must be boolean')
+        self._enabled = self._value
+
+    @staticmethod
+    def reset():
+        # List of used preflights
+        BasePreFlight._in_use = {}
+        # Defined options
+        BasePreFlight._options = {}
+        # Output targets
+        BasePreFlight._targets = None
+        # No longer configured
+        BasePreFlight._configured = False
 
     @staticmethod
     def add_preflight(o_pre):
         BasePreFlight._in_use[o_pre._name] = o_pre
 
     @staticmethod
     def add_preflights(pre):
@@ -50,14 +73,18 @@
         return BasePreFlight._in_use.values()
 
     @staticmethod
     def get_in_use_names():
         return BasePreFlight._in_use.keys()
 
     @staticmethod
+    def get_registered():
+        return BasePreFlight._registered
+
+    @staticmethod
     def _set_option(name, value):
         BasePreFlight._options[name] = value
 
     @staticmethod
     def get_option(name):
         return BasePreFlight._options.get(name)
 
@@ -68,14 +95,27 @@
             del BasePreFlight._targets[BasePreFlight._targets.index(out)]
         except ValueError:
             pass
         BasePreFlight._targets.insert(0, out)
         out.priority = 90
 
     @staticmethod
+    def configure_all():
+        if BasePreFlight._configured:
+            return
+        try:
+            # Configure all of them
+            for k, v in BasePreFlight._in_use.items():
+                logger.debug('Configuring preflight '+k)
+                v.config()
+        except KiPlotConfigurationError as e:
+            GS.exit_with_error("In preflight `"+str(k)+"`: "+str(e), EXIT_BAD_CONFIG)
+        BasePreFlight._configured = True
+
+    @staticmethod
     def run_enabled(targets):
         BasePreFlight._targets = targets
         try:
             for k, v in BasePreFlight._in_use.items():
                 if v._enabled:
                     if v.is_sch():
                         GS.check_sch()
@@ -105,14 +145,18 @@
         """ True for preflights that needs the schematic """
         return self._sch_related
 
     def is_pcb(self):
         """ True for preflights that needs the PCB """
         return self._pcb_related
 
+    def is_any(self):
+        """ True for outputs that needs the schematic and/or the PCB """
+        return self._any_related
+
     def get_example():
         """ Returns a YAML value for the example config """
         return 'true'
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, None
@@ -135,14 +179,18 @@
             files.append(GS.pcb_file)
         return files
 
     def get_targets(self):
         """ Returns a list of targets generated by this preflight """
         return []
 
+    def get_navigate_targets(self, _):
+        """ Returns a list of targets suitable for the navigate results """
+        return self.get_targets(), None
+
     def expand_dirname(self, out_dir):
         return Optionable.expand_filename_both(self, out_dir, is_sch=self._sch_related)
 
     def _find_variant(self):
         # Preflights doesn't have a variant, but we could have one global default
         if hasattr(self, '_variant') and self._variant:
             return self._variant.file_id
@@ -196,7 +244,14 @@
             if os.path.isfile(f):
                 logger.debug('- File `{}`'.format(f))
                 os.remove(f)
             elif os.path.isdir(f):
                 logger.debug('- Dir `{}`'.format(f))
                 rmtree(f)
         self._files_to_remove = []
+
+    @staticmethod
+    def get_conf_examples(name, layers):
+        return None
+
+    def get_category(self):
+        return self._category
```

### Comparing `kibot-1.6.5/kibot/pre_check_zone_fills.py` & `kibot-1.7.0/kibot/pre_check_zone_fills.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020-2023 Salvador E. Tropea
 # Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
-from .error import (KiPlotConfigurationError)
 from .macros import macros, pre_class  # noqa: F401
 
 
 @pre_class
 class Check_Zone_Fills(BasePreFlight):  # noqa: F821
     """ [boolean=false] Zones are filled before doing any operation involving PCB layers.
         The original PCB remains unchanged. If you need to abort when the zone fill
         creates significant changes to a layer use the CheckZoneFill internal template """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
 
     def apply(self):
         BasePreFlight._set_option('check_zone_fills', self._enabled)  # noqa: F821
```

### Comparing `kibot-1.6.5/kibot/pre_erc_warnings.py` & `kibot-1.7.0/kibot/pre_erc_warnings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2021 Salvador E. Tropea
-# Copyright (c) 2021 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2021-2024 Salvador E. Tropea
+# Copyright (c) 2021-2024 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
+from .misc import W_DEPR
 from .macros import macros, pre_class  # noqa: F401
-from .error import (KiPlotConfigurationError)
+from .log import get_logger
+logger = get_logger(__name__)
 
 
 @pre_class
 class ERC_Warnings(BasePreFlight):  # noqa: F821
-    """ [boolean=false] **Deprecated**, use the `warnings_as_errors` option from `run_erc`.
+    """ [boolean=false] **Deprecated**, use the `warnings_as_errors` option from `run_erc`/`erc`.
         Option for `run_erc`. ERC warnings are considered errors """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
+
+    def config(self):
+        super().config()
+        logger.warning(W_DEPR+'The `erc_warnings` preflight is deprecated, use the `warnings_as_errors` option')
 
     def get_example():
         """ Returns a YAML value for the example config """
         return 'false'
 
     def apply(self):
         BasePreFlight._set_option('erc_warnings', self._enabled)  # noqa: F821
```

### Comparing `kibot-1.6.5/kibot/pre_fill_zones.py` & `kibot-1.7.0/kibot/pre_fill_zones.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2022 Salvador E. Tropea
 # Copyright (c) 2022 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 import pcbnew
-from .error import KiPlotConfigurationError
 from .gs import GS
 from .kiplot import load_board
 from .macros import macros, pre_class  # noqa: F401
 
 
 @pre_class
 class Fill_Zones(BasePreFlight):  # noqa: F821
     """ [boolean=false] Fill all zones again and save the PCB """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
         self._pcb_related = True
 
     def apply(self):
         load_board()
         pcbnew.ZONE_FILLER(GS.board).Fill(GS.board.Zones())
         GS.make_bkp(GS.pcb_file)
         # KiCad likes to write the project every time we save the PCB
```

### Comparing `kibot-1.6.5/kibot/pre_filters.py` & `kibot-1.7.0/kibot/pre_filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         parsed = None
         self.unparsed = None
         if not isinstance(self.filters, type):
             for f in self.filters:
                 where = ' (in `{}` filter)'.format(f.filter) if f.filter else ''
                 error = f.error
                 if not error:
-                    if not f.number:
+                    if not hasattr(f, 'number') or not f.number:
                         raise KiPlotConfigurationError('Missing `error`'+where)
                     error = str(f.number)
                 regex = f.regex
                 if regex == 'None':
                     raise KiPlotConfigurationError('Missing `regex`'+where)
                 comment = f.filter
                 logger.debug("Adding {} filter '{}','{}','{}'".format(self._filter_what, comment, error, regex))
@@ -82,22 +82,26 @@
         if parsed:
             self.unparsed = self.filters
         self.filters = parsed
 
 
 @pre_class
 class Filters(BasePreFlight):  # noqa: F821
-    """ [list(dict)] A list of entries to filter out ERC/DRC messages.
+    """ [list(dict)] A list of entries to filter out ERC/DRC messages when using *run_erc*/*run_drc*.
+        Avoid using it with the new *erc* and *drc* preflights.
         Note that ignored errors will become KiBot warnings (i.e. `(W058) ...`).
         To farther ignore these warnings use the `filters` option in the `global` section """
-    def __init__(self, name, value):
-        f = FiltersOptions()
-        f.set_tree({'filters': value})
-        f.config(self)
-        super().__init__(name, f.filters)
+#     def __init__(self, name, value):
+#         super().__init__(name, value)
+
+    def config(self):
+        self._filter_ops = FiltersOptions()
+        self._filter_ops.set_tree({'filters': self._value})
+        self._filter_ops.config(self)
+        self._value = self._filter_ops.filters
 
     def get_example():
         """ Returns a YAML value for the example config """
         return "\n    - filter: 'Filter description'\n      error: '10'\n      regex: 'Regular expression to match'"
 
     @classmethod
     def get_doc(cls):
@@ -105,9 +109,10 @@
 
     def apply(self):
         # Create the filters file
         if self._value:
             our_dir = GS.global_dir if GS.global_use_dir_for_preflights else ''
             o_dir = get_output_dir(our_dir, self)
             GS.filter_file = os.path.join(o_dir, 'kibot_errors.filter')
+            GS.filters = self._filter_ops.unparsed
             with open(GS.filter_file, 'w') as f:
                 f.write(self._value)
```

### Comparing `kibot-1.6.5/kibot/pre_ignore_unconnected.py` & `kibot-1.7.0/kibot/pre_ignore_unconnected.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020-2023 Salvador E. Tropea
-# Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
-# License: GPL-3.0
+# Copyright (c) 2020-2024 Salvador E. Tropea
+# Copyright (c) 2020-2024 Instituto Nacional de Tecnología Industrial
+# License: AGPL-3.0
 # Project: KiBot (formerly KiPlot)
+from .misc import W_DEPR
 from .macros import macros, pre_class  # noqa: F401
-from .error import (KiPlotConfigurationError)
+from .log import get_logger
+logger = get_logger(__name__)
 
 
 @pre_class
 class Ignore_Unconnected(BasePreFlight):  # noqa: F821
-    """ [boolean=false] **Deprecated**, use the `ignore_unconnected` option from `run_drc`.
+    """ [boolean=false] **Deprecated**, use the `ignore_unconnected` option from `run_drc`/`drc`.
         Option for `run_drc`. Ignores the unconnected nets. Useful if you didn't finish the routing.
-        It will also ignore KiCad 6 warnings """
+        It will also ignore KiCad 6 warnings when using `run_drc` """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
+
+    def config(self):
+        super().config()
+        logger.warning(W_DEPR+'The `ignore_unconnected` preflight is deprecated, use the `ignore_unconnected` option')
 
     def get_example():
         """ Returns a YAML value for the example config """
         return 'false'
 
     def apply(self):
         BasePreFlight._set_option('ignore_unconnected', self._enabled)  # noqa: F821
```

### Comparing `kibot-1.6.5/kibot/pre_pcb_replace.py` & `kibot-1.7.0/kibot/pre_pcb_replace.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,21 @@
 class PCB_Replace(Base_Replace):  # noqa: F821
     """ [dict] Replaces tags in the PCB. I.e. to insert the git hash or last revision date.
         This is useful for KiCad 5, use `set_text_variables` when using KiCad 6.
         This preflight modifies the PCB. Even when a back-up is done use it carefully """
     _context = 'PCB'
 
     def __init__(self, name, value):
+        super().__init__(name, value)
+
+    def config(self):
         o = PCB_ReplaceOptions()
-        o.set_tree(value)
+        o.set_tree(self._value)
         o.config(self)
-        super().__init__(name, o)
+        self._value = o
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, PCB_ReplaceOptions
 
     def apply(self):
         o = self._value
```

### Comparing `kibot-1.6.5/kibot/pre_run_drc.py` & `kibot-1.7.0/kibot/pre_run_drc.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 from .macros import macros, document, pre_class  # noqa: F401
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .optionable import Optionable
 from .kicad.config import KiConf
 from .kiplot import load_board
-from .misc import DRC_ERROR, KICAD_VERSION_7_0_1_1, W_DRC7BUG
+from .misc import DRC_ERROR, KICAD_VERSION_7_0_1_1, W_DRC7BUG, W_DEPR
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 
 class Run_DRCOptions(Optionable):
     """ DRC options """
@@ -44,30 +44,32 @@
         Note that the KiCad 6+ *Test for parity between PCB and schematic* option is not supported.
         If you need to check the parity use the `update_xml` preflight.
         KiCad 6 introduced `warnings` they are currently counted be the `unconnected` counter of KiBot.
         This will change in the future.
         If you use DRC exclusions please consult the `drc_exclusions_workaround` global option """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if isinstance(value, bool):
-            self._enabled = value
+        self._pcb_related = True
+        self._expand_id = 'drc'
+        self._expand_ext = 'txt'
+
+    def config(self):
+        if isinstance(self._value, bool):
+            self._enabled = self._value
             self._dir = ''
             self._ignore_unconnected = False
-        elif isinstance(value, dict):
+        elif isinstance(self._value, dict):
             f = Run_DRCOptions()
-            f.set_tree(value)
+            f.set_tree(self._value)
             f.config(self)
             self._enabled = f.enabled
             self._dir = f.dir
             self._ignore_unconnected = f.ignore_unconnected
         else:
             raise KiPlotConfigurationError('must be boolean or dict')
-        self._pcb_related = True
-        self._expand_id = 'drc'
-        self._expand_ext = 'txt'
 
     def get_targets(self):
         """ Returns a list of targets generated by this preflight """
         load_board()
         out_pattern = GS.global_output if GS.global_output is not None else GS.def_global_output
         name = Optionable.expand_filename_pcb(self, out_pattern)
         out_dir = self.expand_dirname(GS.out_dir)
@@ -76,14 +78,16 @@
         return [os.path.abspath(os.path.join(out_dir, self._dir, name))]
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, Run_DRCOptions
 
     def run(self):
+        if GS.ki8:
+            logger.warning(W_DEPR+'For KiCad 8 use the `drc` preflight instead of `run_drc`')
         command = self.ensure_tool('KiAuto')
         if GS.ki7:
             # KiCad 7 can do some library parity checks, but we need to be sure that the KICAD7* vars are defined
             KiConf.init(GS.pcb_file)
             if GS.kicad_version_n < KICAD_VERSION_7_0_1_1:
                 logger.warning(W_DRC7BUG+"KiCad 7.0.0/1 fails to load the global footprints table. "
                                "You may get a lot of `lib_footprint_issues` reports. "
```

### Comparing `kibot-1.6.5/kibot/pre_run_erc.py` & `kibot-1.7.0/kibot/pre_run_erc.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,20 @@
   - from: KiAuto
     role: mandatory
     command: eeschema_do
     version: 2.2.1
 """
 import os
 from shutil import move
-from tempfile import NamedTemporaryFile
 from .macros import macros, document, pre_class  # noqa: F401
 from .gs import GS
 from .optionable import Optionable
 from .kiplot import load_sch
 from .error import KiPlotConfigurationError
-from .misc import ERC_ERROR
+from .misc import ERC_ERROR, W_DEPR
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 
 class Run_ERCOptions(Optionable):
     """ ERC options """
@@ -36,34 +35,37 @@
             self.warnings_as_errors = False
             """ ERC warnings are considered errors """
         self._unknown_is_error = True
 
 
 @pre_class
 class Run_ERC(BasePreFlight):  # noqa: F821
-    """ [boolean=false|dict] Runs the ERC (Electrical Rules Check). To ensure the schematic is electrically correct.
+    """ [boolean=false|dict] (Deprecated for KiCad 8, use *erc*) Runs the ERC (Electrical Rules Check).
+        To ensure the schematic is electrically correct.
         The report file name is controlled by the global output pattern (%i=erc %x=txt) """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if isinstance(value, bool):
-            self._enabled = value
+        self._sch_related = True
+        self._expand_id = 'erc'
+        self._expand_ext = 'txt'
+
+    def config(self):
+        if isinstance(self._value, bool):
+            self._enabled = self._value
             self._dir = ''
             self._warnings_as_errors = False
-        elif isinstance(value, dict):
+        elif isinstance(self._value, dict):
             f = Run_ERCOptions()
-            f.set_tree(value)
+            f.set_tree(self._value)
             f.config(self)
             self._enabled = f.enabled
             self._dir = f.dir
             self._warnings_as_errors = f.warnings_as_errors
         else:
             raise KiPlotConfigurationError('must be boolean or dict')
-        self._sch_related = True
-        self._expand_id = 'erc'
-        self._expand_ext = 'txt'
 
     def get_targets(self):
         """ Returns a list of targets generated by this preflight """
         load_sch()
         out_pattern = GS.global_output if GS.global_output is not None else GS.def_global_output
         name = Optionable.expand_filename_sch(self, out_pattern)
         out_dir = self.expand_dirname(GS.out_dir)
@@ -72,20 +74,20 @@
         return [os.path.abspath(os.path.join(out_dir, self._dir, name))]
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, Run_ERCOptions
 
     def run(self):
+        if GS.ki8:
+            logger.warning(W_DEPR+'For KiCad 8 use the `erc` preflight instead of `run_erc`')
         command = self.ensure_tool('KiAuto')
         # Workaround for KiCad 7 odd behavior: it forces a file extension
         # Note: One thing is adding the extension before you enter a name, other is add something you removed on purpose
-        with NamedTemporaryFile(mode='w', delete=False, suffix='.rpt', prefix='erc_report') as f:
-            tmp_name = f.name
-        logger.debug('ERC report: '+tmp_name)
+        tmp_name = GS.tmp_file(suffix='.rpt', prefix='erc_report', what='ERC report', a_logger=logger)
         cmd = [command, 'run_erc', '-o', os.path.basename(tmp_name), '-g', str(GS.global_erc_grid)]
         if self._warnings_as_errors or BasePreFlight.get_option('erc_warnings'):  # noqa: F821
             cmd.append('-w')
         if GS.filter_file:
             cmd.extend(['-f', GS.filter_file])
         cmd.extend([GS.sch_file, os.path.dirname(tmp_name)])
         # If we are in verbose mode enable debug in the child
```

### Comparing `kibot-1.6.5/kibot/pre_set_text_variables.py` & `kibot-1.7.0/kibot/pre_set_text_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,18 +77,21 @@
 class Set_Text_Variables(BasePreFlight):  # noqa: F821
     """ [dict|list(dict)] Defines KiCad 6+ variables.
         They are expanded using `${VARIABLE}`, and stored in the project file.
         This preflight replaces `pcb_replace` and `sch_replace` when using KiCad 6.
         The KiCad project file is modified.
         Warning: don't use `-s all` or this preflight will be skipped """
     def __init__(self, name, value):
+        super().__init__(name, value)
+
+    def config(self):
         f = Set_Text_VariablesOptions()
-        f.set_tree({'variables': value})
+        f.set_tree({'variables': self._value})
         f.config(self)
-        super().__init__(name, f.variables)
+        self._value = f.variables
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, KiCadVariable
 
     @classmethod
     def get_example(cls):
```

### Comparing `kibot-1.6.5/kibot/pre_update_qr.py` & `kibot-1.7.0/kibot/pre_update_qr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020-2022 Salvador E. Tropea
 # Copyright (c) 2020-2022 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
 from .macros import macros, pre_class  # noqa: F401
-from .error import KiPlotConfigurationError
 from .registrable import RegOutput
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 
 @pre_class
 class Update_QR(BasePreFlight):  # noqa: F821
     """ [boolean=false] Update the QR codes.
         Complements the `qr_lib` output.
         The KiCad 6 files and the KiCad 5 PCB needs manual update, generating a new library isn't enough """
     def __init__(self, name, value):
         super().__init__(name, value)
-        if not isinstance(value, bool):
-            raise KiPlotConfigurationError('must be boolean')
-        self._enabled = value
         self._sch_related = True
         self._pcb_related = True
 
     def run(self):
         for o in RegOutput.get_outputs():
             if o.type == 'qr_lib':
                 BasePreFlight.insert_target(o)  # noqa: F821
```

### Comparing `kibot-1.6.5/kibot/pre_update_xml.py` & `kibot-1.7.0/kibot/pre_update_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import namedtuple
 import os
 import xml.etree.ElementTree as ET
 from .macros import macros, document, pre_class  # noqa: F401
 from .error import KiPlotConfigurationError
 from .gs import GS
 from .kiplot import load_board
-from .misc import BOM_ERROR, NETLIST_DIFF, W_PARITY, MISSING_TOOL, KICAD_VERSION_7_0_1, W_NOTINBOM, MOD_BOARD_ONLY
+from .misc import BOM_ERROR, NETLIST_DIFF, W_PARITY, MISSING_TOOL, KICAD_VERSION_7_0_1, W_NOTINBOM, MOD_BOARD_ONLY, W_DEPR
 from .log import get_logger
 from .optionable import Optionable
 import pcbnew
 
 logger = get_logger(__name__)
 Component = namedtuple("Component", "val fp props")
 
@@ -47,27 +47,29 @@
     """ [boolean=false|dict] Update the XML version of the BoM (Bill of Materials).
         To ensure our generated BoM is up to date.
         Note that this isn't needed when using the internal BoM generator (`bom`).
         You can compare the PCB and schematic netlists using it """
     def __init__(self, name, value):
         super().__init__(name, value)
         self._check_pcb_parity = False
-        if isinstance(value, bool):
-            self._enabled = value
-        elif isinstance(value, dict):
+        self._sch_related = True
+
+    def config(self):
+        if isinstance(self._value, bool):
+            self._enabled = self._value
+        elif isinstance(self._value, dict):
             f = Update_XMLOptions()
-            f.set_tree(value)
+            f.set_tree(self._value)
             f.config(self)
             self._enabled = f.enabled
             self._check_pcb_parity = f.check_pcb_parity
             self.options = f
             self._pcb_related = True
         else:
             raise KiPlotConfigurationError('must be boolean or dict')
-        self._sch_related = True
 
     @classmethod
     def get_doc(cls):
         return cls.__doc__, Update_XMLOptions
 
     def get_targets(self):
         """ Returns a list of targets generated by this preflight """
@@ -162,14 +164,16 @@
 
     def check_pcb_parity(self):
         if GS.ki5:
             GS.exit_with_error('PCB vs schematic parity only available for KiCad 6', MISSING_TOOL)
         if GS.ki7 and GS.kicad_version_n < KICAD_VERSION_7_0_1:
             GS.exit_with_error("Connectivity API is broken on KiCad 7.0.0\n"
                                "Please upgrade KiCad to 7.0.1 or newer", MISSING_TOOL)
+        if GS.ki8:
+            logger.warning(W_DEPR+'For KiCad 8 use the `drc` preflight, it supports parity checks from KiCad')
         fname = GS.sch_no_ext+'.xml'
         logger.debug('Loading XML: '+fname)
         try:
             tree = ET.parse(fname)
         except Exception as e:
             raise KiPlotConfigurationError('Errors parsing {}\n{}'.format(fname, e))
         root = tree.getroot()
```

### Comparing `kibot-1.6.5/kibot/registrable.py` & `kibot-1.7.0/kibot/registrable.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/3DRender.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/3DRender.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/CheckZoneFill.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/CheckZoneFill.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/Elecrow.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/Elecrow.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/FusionPCB.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/FusionPCB.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/JLCPCB.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/JLCPCB.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/MacroFab_XYRS.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/MacroFab_XYRS.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/P-Ban.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/P-Ban.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_1.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_1.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_1_haschtl.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_1_haschtl.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/PCB2Blender_2_7.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/PCB2Blender_2_7.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/PCBWay.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/PCBWay.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/config_templates/PanelDemo_4x4.kibot.yaml` & `kibot-1.7.0/kibot/resources/config_templates/PanelDemo_4x4.kibot.yaml`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/3d.svg` & `kibot-1.7.0/kibot/resources/images/3d.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/assembly_simple.svg` & `kibot-1.7.0/kibot/resources/images/assembly_simple.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/back.svg` & `kibot-1.7.0/kibot/resources/images/back.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/bom.svg` & `kibot-1.7.0/kibot/resources/images/bom.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/eeschema.svg` & `kibot-1.7.0/kibot/resources/images/eeschema.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/export.svg` & `kibot-1.7.0/kibot/resources/images/export.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/fabrication.svg` & `kibot-1.7.0/kibot/resources/images/fabrication.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/favicon.ico` & `kibot-1.7.0/kibot/resources/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_blend.svg` & `kibot-1.7.0/kibot/resources/images/file_blend.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_brd.svg` & `kibot-1.7.0/kibot/resources/images/file_brd.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_bz2.svg` & `kibot-1.7.0/kibot/resources/images/file_bz2.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_cad.svg` & `kibot-1.7.0/kibot/resources/images/file_cad.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_css.svg` & `kibot-1.7.0/kibot/resources/images/file_css.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_csv.svg` & `kibot-1.7.0/kibot/resources/images/file_csv.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_drl.svg` & `kibot-1.7.0/kibot/resources/images/file_drl.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_dxf.svg` & `kibot-1.7.0/kibot/resources/images/file_dxf.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_eps.svg` & `kibot-1.7.0/kibot/resources/images/file_eps.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_gbr.svg` & `kibot-1.7.0/kibot/resources/images/file_gbr.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_gerber_job.svg` & `kibot-1.7.0/kibot/resources/images/file_gerber_job.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_gz.svg` & `kibot-1.7.0/kibot/resources/images/file_gz.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_html.svg` & `kibot-1.7.0/kibot/resources/images/file_html.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_jpg.svg` & `kibot-1.7.0/kibot/resources/images/file_jpg.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_pcb3d.svg` & `kibot-1.7.0/kibot/resources/images/file_pcb3d.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_pdf.svg` & `kibot-1.7.0/kibot/resources/images/file_pdf.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_plt.svg` & `kibot-1.7.0/kibot/resources/images/file_plt.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_png.svg` & `kibot-1.7.0/kibot/resources/images/file_png.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_pos.svg` & `kibot-1.7.0/kibot/resources/images/file_pos.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_ps.svg` & `kibot-1.7.0/kibot/resources/images/file_ps.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_rar.svg` & `kibot-1.7.0/kibot/resources/images/file_rar.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_scad.svg` & `kibot-1.7.0/kibot/resources/images/file_scad.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_stl.svg` & `kibot-1.7.0/kibot/resources/images/file_stl.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_stp.svg` & `kibot-1.7.0/kibot/resources/images/file_stp.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_svg.svg` & `kibot-1.7.0/kibot/resources/images/file_svg.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_tar.svg` & `kibot-1.7.0/kibot/resources/images/file_tar.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_tsv.svg` & `kibot-1.7.0/kibot/resources/images/file_tsv.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_txt.svg` & `kibot-1.7.0/kibot/resources/images/file_txt.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_wrl.svg` & `kibot-1.7.0/kibot/resources/images/file_wrl.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_xlsx.svg` & `kibot-1.7.0/kibot/resources/images/file_xlsx.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_xml.svg` & `kibot-1.7.0/kibot/resources/images/file_xml.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_xyrs.svg` & `kibot-1.7.0/kibot/resources/images/file_xyrs.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_xz.svg` & `kibot-1.7.0/kibot/resources/images/file_xz.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/file_zip.svg` & `kibot-1.7.0/kibot/resources/images/file_zip.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/folder.svg` & `kibot-1.7.0/kibot/resources/images/folder.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/gerber.svg` & `kibot-1.7.0/kibot/resources/images/gerber.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/home.svg` & `kibot-1.7.0/kibot/resources/images/home.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/ibom.svg` & `kibot-1.7.0/kibot/resources/images/ibom.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/load_drill.svg` & `kibot-1.7.0/kibot/resources/images/load_drill.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/pcbnew.svg` & `kibot-1.7.0/kibot/resources/images/pcbnew.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/project.svg` & `kibot-1.7.0/kibot/resources/images/project.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/repair.svg` & `kibot-1.7.0/kibot/resources/images/repair.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/unknown.svg` & `kibot-1.7.0/kibot/resources/images/unknown.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/images/zip.svg` & `kibot-1.7.0/kibot/resources/images/zip.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kicad_colors/_builtin_classic.json` & `kibot-1.7.0/kibot/resources/kicad_colors/_builtin_classic.json`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kicad_colors/_builtin_default.json` & `kibot-1.7.0/kibot/resources/kicad_colors/_builtin_default.json`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kicad_layouts/default.kicad_wks` & `kibot-1.7.0/kibot/resources/kicad_layouts/default.kicad_wks`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kicanvas/kicanvas.svg` & `kibot-1.7.0/kibot/resources/kicanvas/kicanvas.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/images/code-branch-solid.svg` & `kibot-1.7.0/kibot/resources/kiri/images/code-branch-solid.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/images/icon.svg` & `kibot-1.7.0/kibot/resources/kiri/images/icon.svg`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/index.html` & `kibot-1.7.0/kibot/resources/kiri/index.html`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/kiri-server` & `kibot-1.7.0/kibot/resources/kiri/kiri-server`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/kiri.css` & `kibot-1.7.0/kibot/resources/kiri/kiri.css`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/kiri.js` & `kibot-1.7.0/kibot/resources/kiri/kiri.js`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/utils/bootstrap.bundle.min.js` & `kibot-1.7.0/kibot/resources/kiri/utils/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/utils/bootstrap.min.css` & `kibot-1.7.0/kibot/resources/kiri/utils/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/utils/jquery-3.6.0.min.js` & `kibot-1.7.0/kibot/resources/kiri/utils/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/kiri/utils/svg-pan-zoom.min.js` & `kibot-1.7.0/kibot/resources/kiri/utils/svg-pan-zoom.min.js`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/parsers/electro.lark` & `kibot-1.7.0/kibot/resources/parsers/electro.lark`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/css/styles.css` & `kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/css/styles.css`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/index.html` & `kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/index.html`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/package-lock.json` & `kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/package-lock.json`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/pcbdraw/present/templates/default/src/styles.css` & `kibot-1.7.0/kibot/resources/pcbdraw/present/templates/default/src/styles.css`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/pcbdraw/templates/simple.handlebars` & `kibot-1.7.0/kibot/resources/pcbdraw/templates/simple.handlebars`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/report_templates/report_full.txt` & `kibot-1.7.0/kibot/resources/report_templates/report_full.txt`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/report_templates/report_full_svg.txt` & `kibot-1.7.0/kibot/resources/report_templates/report_full_svg.txt`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/resources/report_templates/report_simple.txt` & `kibot-1.7.0/kibot/resources/report_templates/report_simple.txt`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/svgutils/compose.py` & `kibot-1.7.0/kibot/svgutils/compose.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/svgutils/templates.py` & `kibot-1.7.0/kibot/svgutils/templates.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/svgutils/transform.py` & `kibot-1.7.0/kibot/svgutils/transform.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/var_base.py` & `kibot-1.7.0/kibot/var_base.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot/var_ibom.py` & `kibot-1.7.0/kibot/var_kicost.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,88 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2020 Salvador E. Tropea
-# Copyright (c) 2020 Instituto Nacional de Tecnología Industrial
+# Copyright (c) 2020-2023 Salvador E. Tropea
+# Copyright (c) 2020-2023 Instituto Nacional de Tecnología Industrial
 # License: GPL-3.0
 # Project: KiBot (formerly KiPlot)
-# Description: Implements the IBoM variants mechanism.
-from .optionable import Optionable
+# The algorithm is from KiCost project (https://github.com/xesscorp/KiCost)
+# Description: Implements the KiCost variants mechanism.
+import re
 from .gs import GS
-from .misc import IFILT_MECHANICAL
+from .misc import IFILT_KICOST_RENAME, IFILT_KICOST_DNP
 from .fil_base import BaseFilter
 from .macros import macros, document, variant_class  # noqa: F401
 from . import log
 
 logger = log.get_logger()
 
 
 @variant_class
-class IBoM(BaseVariant):  # noqa: F821
-    """ IBoM variant style
-        The Config field (configurable) contains a value.
-        If this value matches with a value in the whitelist is included.
-        If this value matches with a value in the blacklist is excluded """
+class KiCost(BaseVariant):  # noqa: F821
+    """ KiCost variant style
+        The `variant` field (configurable) contains one or more values.
+        If any of these values matches the variant regex the component is included.
+        By default a pre-transform filter is applied to support kicost.VARIANT:FIELD and
+        field name aliases used by KiCost.
+        Also a default `dnf_filter` implements the KiCost DNP mechanism """
     def __init__(self):
         super().__init__()
         with document:
-            self.variant_field = 'Config'
-            """ Name of the field that stores board variant for component """
-            self.variants_blacklist = Optionable
-            """ [string|list(string)=''] List of board variants to exclude from the BOM """
-            self.variants_whitelist = Optionable
-            """ [string|list(string)=''] List of board variants to include in the BOM """
+            self.variant = ''
+            """ Variants to match (regex) """
+            self.variant_field = 'variant'
+            """ Name of the field that stores board variant/s for component.
+                Only supported internally, don't use it if you plan to use KiCost """
+            self.separators = ',;/ '
+            """ Valid separators for variants in the variant field.
+                Each character is a valid separator.
+                Only supported internally, don't use it if you plan to use KiCost """
 
     def get_variant_field(self):
         """ Returns the name of the field used to determine if the component belongs to the variant """
         return self.variant_field
 
     def config(self, parent):
         super().config(parent)
-        self.pre_transform = BaseFilter.solve_filter(self.pre_transform, 'pre_transform', is_transform=True)
-        self.exclude_filter = BaseFilter.solve_filter(self.exclude_filter, 'exclude_filter', IFILT_MECHANICAL)
-        self.dnf_filter = BaseFilter.solve_filter(self.dnf_filter, 'dnf_filter')
+        self.pre_transform = BaseFilter.solve_filter(self.pre_transform, 'pre_transform',
+                                                     ['_var_rename_kicost', IFILT_KICOST_RENAME], is_transform=True)
+        self.exclude_filter = BaseFilter.solve_filter(self.exclude_filter, 'exclude_filter')
+        self.dnf_filter = BaseFilter.solve_filter(self.dnf_filter, 'dnf_filter', IFILT_KICOST_DNP)
         self.dnc_filter = BaseFilter.solve_filter(self.dnc_filter, 'dnc_filter')
-        self.variants_blacklist = self.force_list(self.variants_blacklist)
-        self.variants_whitelist = self.force_list(self.variants_whitelist)
-
-    def skip_component(self, c):
-        """ Skip components that doesn't belong to this variant. """
-        # Apply variants white/black lists
-        if self.variant_field:
-            ref_variant = c.get_field_value(self.variant_field).lower()
-            # skip components with wrong variant field
-            if self.variants_whitelist and ref_variant not in self.variants_whitelist:
-                return True
-            if self.variants_blacklist and ref_variant and ref_variant in self.variants_blacklist:
+        if not self.separators:
+            self.separators = ' '
+        else:
+            self.separators = '['+self.separators+']'
+        if self.variant_field and self.variant:
+            self._var_re = re.compile(self.variant, flags=re.IGNORECASE)
+        else:
+            self._var_re = None
+
+    def matches_variant(self, variants):
+        if self._var_re is None or not variants:
+            return True
+        # The component belongs to one or more variant
+        for v in re.split(self.separators, variants):
+            if self._var_re.match(v):
+                # Matched, remains
                 return True
+        # None of the variants matched
         return False
 
     def filter(self, comps):
-        GS.variant = self.variants_whitelist
+        GS.variant = [self.variant]
         comps = super().filter(comps)
-        logger.debug("Applying IBoM style variants `{}`".format(self.name))
-        # Make black/white lists case insensitive
-        self.variants_whitelist = [v.lower() for v in self.variants_whitelist]
-        self.variants_blacklist = [v.lower() for v in self.variants_blacklist]
+        logger.debug("Applying KiCost style variant `{}`".format(self.name))
+        if self._var_re is None:
+            # No variant field or not variant regex
+            # Just skip the process
+            return comps
         # Apply to all the components
         for c in comps:
-            logger.debug("{} {} {}".format(c.ref, c.fitted, c.included))
+            logger.debug("{} fitted: {} included: {}".format(c.ref, c.fitted, c.included))
             if not (c.fitted and c.included):
                 # Don't check if we already discarded it
                 continue
-            c.fitted = not self.skip_component(c)
+            variants = c.get_field_value(self.variant_field)
+            c.fitted = self.matches_variant(variants)
             if not c.fitted and GS.debug_level > 2:
-                logger.debug('ref: {} value: {} -> False'.format(c.ref, c.value))
+                logger.debug('ref: {} value: {} variants: {} -> False'.format(c.ref, c.value, variants))
         return comps
```

### Comparing `kibot-1.6.5/kibot/var_kibom.py` & `kibot-1.7.0/kibot/var_kibom.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/kibot.egg-info/PKG-INFO` & `kibot-1.7.0/kibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kibot
-Version: 1.6.5
+Version: 1.7.0
 Summary: KiCad automation tool for documents generation
 Home-page: https://github.com/INTI-CMNB/KiBot/
 Author: Salvador E. Tropea, John Beard
 Author-email: stropea@inti.gob.ar
 License: GPL-3.0
 Description: 
         # KiBot (formerly KiPlot)
```

### Comparing `kibot-1.6.5/kibot.egg-info/SOURCES.txt` & `kibot-1.7.0/kibot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -87,26 +87,33 @@
 kibot/out_svg.py
 kibot/out_svg_pcb_print.py
 kibot/out_svg_sch_print.py
 kibot/out_vrml.py
 kibot/pre_annotate_pcb.py
 kibot/pre_annotate_power.py
 kibot/pre_any_replace.py
+kibot/pre_any_xrc.py
 kibot/pre_base.py
 kibot/pre_check_zone_fills.py
+kibot/pre_draw_stackup.py
+kibot/pre_drc.py
+kibot/pre_erc.py
 kibot/pre_erc_warnings.py
 kibot/pre_fill_zones.py
 kibot/pre_filters.py
 kibot/pre_ignore_unconnected.py
 kibot/pre_pcb_replace.py
 kibot/pre_run_drc.py
 kibot/pre_run_erc.py
 kibot/pre_sch_replace.py
 kibot/pre_set_text_variables.py
+kibot/pre_update_footprint.py
+kibot/pre_update_pcb_characteristics.py
 kibot/pre_update_qr.py
+kibot/pre_update_stackup.py
 kibot/pre_update_xml.py
 kibot/registrable.py
 kibot/var_base.py
 kibot/var_ibom.py
 kibot/var_kibom.py
 kibot/var_kicost.py
 kibot.egg-info/PKG-INFO
@@ -206,14 +213,15 @@
 kibot/resources/config_templates/3DRender_bottom.kibot.yaml
 kibot/resources/config_templates/3DRender_bottom_straight.kibot.yaml
 kibot/resources/config_templates/3DRender_top.kibot.yaml
 kibot/resources/config_templates/3DRender_top_straight.kibot.yaml
 kibot/resources/config_templates/CheckZoneFill.kibot.yaml
 kibot/resources/config_templates/Elecrow.kibot.yaml
 kibot/resources/config_templates/Elecrow_stencil.kibot.yaml
+kibot/resources/config_templates/ExportProject.kibot.yaml
 kibot/resources/config_templates/FusionPCB.kibot.yaml
 kibot/resources/config_templates/FusionPCB_stencil.kibot.yaml
 kibot/resources/config_templates/JLCPCB.kibot.yaml
 kibot/resources/config_templates/JLCPCB_stencil.kibot.yaml
 kibot/resources/config_templates/JLCPCB_stencil_with_THT.kibot.yaml
 kibot/resources/config_templates/JLCPCB_with_THT.kibot.yaml
 kibot/resources/config_templates/MacroFab_XYRS.kibot.yaml
@@ -225,15 +233,17 @@
 kibot/resources/config_templates/PCBWay.kibot.yaml
 kibot/resources/config_templates/PCBWay_stencil.kibot.yaml
 kibot/resources/config_templates/PanelDemo_4x4.kibot.yaml
 kibot/resources/images/3d.svg
 kibot/resources/images/assembly_simple.svg
 kibot/resources/images/back.svg
 kibot/resources/images/bom.svg
+kibot/resources/images/drc.svg
 kibot/resources/images/eeschema.svg
+kibot/resources/images/erc.svg
 kibot/resources/images/export.svg
 kibot/resources/images/fabrication.svg
 kibot/resources/images/favicon.ico
 kibot/resources/images/file_blend.svg
 kibot/resources/images/file_brd.svg
 kibot/resources/images/file_bz2.svg
 kibot/resources/images/file_cad.svg
@@ -243,14 +253,15 @@
 kibot/resources/images/file_dxf.svg
 kibot/resources/images/file_eps.svg
 kibot/resources/images/file_gbr.svg
 kibot/resources/images/file_gerber_job.svg
 kibot/resources/images/file_gz.svg
 kibot/resources/images/file_html.svg
 kibot/resources/images/file_jpg.svg
+kibot/resources/images/file_json.svg
 kibot/resources/images/file_pcb3d.svg
 kibot/resources/images/file_pdf.svg
 kibot/resources/images/file_plt.svg
 kibot/resources/images/file_png.svg
 kibot/resources/images/file_pos.svg
 kibot/resources/images/file_ps.svg
 kibot/resources/images/file_rar.svg
```

### Comparing `kibot-1.6.5/setup.cfg` & `kibot-1.7.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 recursive = True
 expand-star-imports = True
 
 [check-docstring-first]
 ignore = kibot/banner.py
 
 [codespell]
-skip = entrypoint.sh,kibot/banner.py
+skip = entrypoint.sh,kibot/banner.py,kibot/bom/kibot_logo.py
 ignore-words-list = kibot,tht
 quiet-level = 2
 
 [flake8]
 ignore = E402, E226, E126, W504
 	D1
 	D2
```

### Comparing `kibot-1.6.5/setup.py` & `kibot-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `kibot-1.6.5/src/kibot-check` & `kibot-1.7.0/src/kibot-check`

 * *Files 1% similar despite different names*

```diff
@@ -539,16 +539,16 @@
             {\
                 "desc": null,\
                 "mandatory": true,\
                 "max_version": null,\
                 "output": "render_3d",\
                 "version": [\
                     2,\
-                    0,\
-                    4\
+                    3,\
+                    1\
                 ]\
             },\
             {\
                 "desc": null,\
                 "mandatory": true,\
                 "max_version": null,\
                 "output": "step",\
@@ -1717,14 +1717,34 @@
     if 'HOME' in os.environ:
         home = os.environ['HOME']
         kicad_plugins_dirs.append(os.path.join(home, '.kicad_plugins'))
         kicad_plugins_dirs.append(os.path.join(home, '.kicad', 'scripting'))
         kicad_plugins_dirs.append(os.path.join(home, '.kicad', 'scripting', 'plugins'))
 except FileNotFoundError:
     kicad_ok = False
+except ModuleNotFoundError:
+    kicad_ok = False
+    if which('kicad'):
+        error("KiCad installed but the Python support is broken")
+        res = run_command(['find', '/usr/lib', '-name', 'pcbnew.py'])
+        if res:
+            cand = res.split('\n')
+            if cand:
+                cand = [x for x in cand if 'pcbnewTransition' not in x]
+                if cand:
+                    if len(cand) == 1:
+                        dname = os.path.dirname(cand[0])
+                        if dname in sys.path:
+                            error(f"The pcbnew module should be loadable, but fails to load")
+                        else:
+                            error(f"Broken Python support {dname} not in sys.path ({sys.path})")
+                    else:
+                        error(f'Multiple pcbnew modules found: {str(cand)}')
+    else:
+        error("KiCad not installed or not available in the path")
 kicad_version = (0, 0, 0)
 if kicad_ok:
     try:
         version = pcbnew.GetBuildVersion()
         # KiCad version
         m = re.search(r'(\d+)\.(\d+)\.(\d+)', version)
         if m is None:
```

