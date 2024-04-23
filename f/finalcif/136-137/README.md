# Comparing `tmp/finalcif-136.tar.gz` & `tmp/finalcif-137.tar.gz`

## Comparing `finalcif-136.tar` & `finalcif-137.tar`

### file list

```diff
@@ -1,147 +1,148 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 finalcif-136/.gitattributes
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 finalcif-136/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 finalcif-136/CONTRIBUTING.md
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 finalcif-136/Finalcif_installer_win.spec
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 finalcif-136/Finalcif_linux_onefile.spec
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 finalcif-136/Finalcif_mac.spec
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 finalcif-136/Hydrogen_solution_type.cif
--rw-r--r--   0        0        0   255400 2020-02-02 00:00:00.000000 finalcif-136/finalcif.exe
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 finalcif-136/install_requirements
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 finalcif-136/install_requirements.bat
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 finalcif-136/requirements.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 finalcif-136/requirements_devel.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 finalcif-136/requirements_doku.txt
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 finalcif-136/run_finalcif
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 finalcif-136/run_finalcif.bat
--rw-r--r--   0        0        0  8839016 2020-02-02 00:00:00.000000 finalcif-136/update.exe
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 finalcif-136/.run/Make Documentation MAC.run.xml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 finalcif-136/.run/compile_ui_files.run.xml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 finalcif-136/.run/make documentation Windows.run.xml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-136/finalcif/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 finalcif-136/finalcif/app_path.py
--rw-r--r--   0        0        0    96459 2020-02-02 00:00:00.000000 finalcif-136/finalcif/appwindow.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 finalcif-136/finalcif/finalcif_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/all_cif_dicts.py
--rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/atoms.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cif_dict_foo.py
--rw-r--r--   0        0        0    40128 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cif_file_io.py
--rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cif_order.py
--rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/core_dict.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/hkl.py
--rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/modulation_dict.py
--rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/powder_dict.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/reference.py
--rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/restraints_dict.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/text.py
--rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/twin_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/checkcif/__init__.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/checkcif/checkcif.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/__init__.py
--rw-r--r--   0        0        0    18834 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/deposit.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/deposit_check.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/deposition_list.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/doi.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/upload.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-136/finalcif/cif/cod/website_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/__init__.py
--rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/bruker_data.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/bruker_frame.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/ccdc_mail.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/data.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/p4p_reader.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/sadabs.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/saint.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/shelx_lst.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-136/finalcif/datafiles/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/displaymol/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 finalcif-136/finalcif/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-136/finalcif/displaymol/sdm.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-136/finalcif/displaymol/vtk_molecule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/equip_property/__init__.py
--rw-r--r--   0        0        0    21663 2020-02-02 00:00:00.000000 finalcif-136/finalcif/equip_property/author_loop_templates.py
--rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 finalcif-136/finalcif/equip_property/equipment.py
--rw-r--r--   0        0        0    14732 2020-02-02 00:00:00.000000 finalcif-136/finalcif/equip_property/properties.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 finalcif-136/finalcif/equip_property/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/__init__.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/combobox.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/custom_classes.py
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/dialogs.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/edit_button.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/equipmenttable.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/file_editor.py
--rw-r--r--   0        0        0   159875 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/finalcif_gui_ui.py
--rw-r--r--   0        0        0   183169 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/finalcif_gui_ui.ui
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/import_selector.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/import_selector_ui.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/import_selector_ui.ui
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/loop_creator.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/loop_creator_ui.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/loop_creator_ui.ui
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/loops.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/mainstackwidget.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/mixins.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/new_key_dialog.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/new_key_dialog_ui.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/new_key_dialog_ui.ui
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/plaintextedit.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/playground.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/propertytable.py
--rw-r--r--   0        0        0    13000 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/spell_check_edit.py
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/text_templates_ui.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/text_templates_ui.ui
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/text_value_editor.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 finalcif-136/finalcif/gui/vrf_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/__init__.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/finalcif.png
--rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/finalcif2.ico
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/finalcif2.png
--rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/multitable.ico
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/multitable.png
--rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-136/finalcif/icon/multitable.xcf
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/archive_report.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/mtools.py
--rw-r--r--   0        0        0    19893 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/references.py
--rw-r--r--   0        0        0    24640 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/report_text.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/symm.py
--rw-r--r--   0        0        0    38718 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/tables.py
--rw-r--r--   0        0        0    38803 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/templated_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/gui/__init__.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/gui/mainwindow.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-136/finalcif/report/gui/mainwindow.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/__init__.py
--rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/mathml2omml.xsl
--rw-r--r--   0        0        0    20387 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/report.tmpl
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/template1.docx
--rw-r--r--   0        0        0    26744 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/template_for_multitable.docx
--rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/template_text.docx
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/template_without_text.docx
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/templates.py
--rw-r--r--   0        0        0   163873 2020-02-02 00:00:00.000000 finalcif-136/finalcif/template/bootstrap/bootstrap.min.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/__init__.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/download.py
--rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/dsrmath.py
--rw-r--r--   0        0        0    29727 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/misc.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/options.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/platon.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/pupdate.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/settings.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/shred.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/space_groups.py
--rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/spgr_format.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/statusbar.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-136/finalcif/tools/sumformula.py
--rw-r--r--   0        0        0    96403 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_checkcif.png
--rw-r--r--   0        0        0   132682 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_details.png
--rw-r--r--   0        0        0    52874 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_loops.png
--rw-r--r--   0        0        0    71252 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_loops2.png
--rw-r--r--   0        0        0    84495 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_main.png
--rw-r--r--   0        0        0   111861 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_report.png
--rw-r--r--   0        0        0    75057 2020-02-02 00:00:00.000000 finalcif-136/screenshots/finalcif_responses.png
--rw-r--r--   0        0        0   163873 2020-02-02 00:00:00.000000 finalcif-136/work/bootstrap.min.css
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 finalcif-136/.gitignore
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-136/LICENSE
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 finalcif-136/README.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 finalcif-136/pyproject.toml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 finalcif-136/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 finalcif-137/.gitattributes
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 finalcif-137/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 finalcif-137/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 finalcif-137/Finalcif_installer_win.spec
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 finalcif-137/Finalcif_linux_onefile.spec
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 finalcif-137/Finalcif_mac.spec
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 finalcif-137/Hydrogen_solution_type.cif
+-rw-r--r--   0        0        0   255400 2020-02-02 00:00:00.000000 finalcif-137/finalcif.exe
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 finalcif-137/install_requirements
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 finalcif-137/install_requirements.bat
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 finalcif-137/requirements.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 finalcif-137/requirements_devel.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 finalcif-137/requirements_doku.txt
+-rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 finalcif-137/run_finalcif
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 finalcif-137/run_finalcif.bat
+-rw-r--r--   0        0        0  8839016 2020-02-02 00:00:00.000000 finalcif-137/update.exe
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 finalcif-137/.run/Make Documentation MAC.run.xml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 finalcif-137/.run/compile_ui_files.run.xml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 finalcif-137/.run/make documentation Windows.run.xml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-137/finalcif/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 finalcif-137/finalcif/app_path.py
+-rw-r--r--   0        0        0    97566 2020-02-02 00:00:00.000000 finalcif-137/finalcif/appwindow.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 finalcif-137/finalcif/finalcif_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/all_cif_dicts.py
+-rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/atoms.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cif_dict_foo.py
+-rw-r--r--   0        0        0    40127 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cif_file_io.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cif_order.py
+-rw-r--r--   0        0        0   558364 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/core_dict.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/hkl.py
+-rw-r--r--   0        0        0  1071510 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/modulation_dict.py
+-rw-r--r--   0        0        0   243970 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/powder_dict.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/reference.py
+-rw-r--r--   0        0        0   121599 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/restraints_dict.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/text.py
+-rw-r--r--   0        0        0    23604 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/twin_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/checkcif/__init__.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/checkcif/checkcif.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/__init__.py
+-rw-r--r--   0        0        0    18834 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/deposit.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/deposit_check.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/deposition_list.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/doi.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/upload.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-137/finalcif/cif/cod/website_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/__init__.py
+-rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/bruker_data.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/bruker_frame.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/ccdc_mail.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/data.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/p4p_reader.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/sadabs.py
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/saint.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/shelx_lst.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-137/finalcif/datafiles/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/displaymol/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 finalcif-137/finalcif/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-137/finalcif/displaymol/sdm.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-137/finalcif/displaymol/vtk_molecule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/equip_property/__init__.py
+-rw-r--r--   0        0        0    21663 2020-02-02 00:00:00.000000 finalcif-137/finalcif/equip_property/author_loop_templates.py
+-rw-r--r--   0        0        0    14058 2020-02-02 00:00:00.000000 finalcif-137/finalcif/equip_property/equipment.py
+-rw-r--r--   0        0        0    14732 2020-02-02 00:00:00.000000 finalcif-137/finalcif/equip_property/properties.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 finalcif-137/finalcif/equip_property/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/__init__.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/combobox.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/custom_classes.py
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/dialogs.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/edit_button.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/equipmenttable.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/file_editor.py
+-rw-r--r--   0        0        0   159875 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/finalcif_gui_ui.py
+-rw-r--r--   0        0        0   183169 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/finalcif_gui_ui.ui
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/import_selector.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/import_selector_ui.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/import_selector_ui.ui
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/loop_creator.py
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/loop_creator_ui.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/loop_creator_ui.ui
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/loops.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/mainstackwidget.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/mixins.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/new_key_dialog.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/new_key_dialog_ui.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/new_key_dialog_ui.ui
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/plaintextedit.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/playground.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/propertytable.py
+-rw-r--r--   0        0        0    13000 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/spell_check_edit.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/text_templates_ui.py
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/text_templates_ui.ui
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/text_value_editor.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/validators.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 finalcif-137/finalcif/gui/vrf_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/__init__.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/finalcif.png
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/finalcif2.ico
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/finalcif2.png
+-rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/multitable.ico
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/multitable.png
+-rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-137/finalcif/icon/multitable.xcf
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/archive_report.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/mtools.py
+-rw-r--r--   0        0        0    19893 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/references.py
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/report_text.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/symm.py
+-rw-r--r--   0        0        0    38620 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/tables.py
+-rw-r--r--   0        0        0    39080 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/templated_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/gui/__init__.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/gui/mainwindow.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-137/finalcif/report/gui/mainwindow.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/__init__.py
+-rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/mathml2omml.xsl
+-rw-r--r--   0        0        0    20497 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/report.tmpl
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/template1.docx
+-rw-r--r--   0        0        0    26744 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/template_for_multitable.docx
+-rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/template_text.docx
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/template_without_text.docx
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/templates.py
+-rw-r--r--   0        0        0   163873 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/bootstrap/bootstrap.min.css
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 finalcif-137/finalcif/template/machines/D8_VENTURE.cif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/__init__.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/download.py
+-rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/dsrmath.py
+-rw-r--r--   0        0        0    29783 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/misc.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/options.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/platon.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/pupdate.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/settings.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/shred.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/space_groups.py
+-rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/spgr_format.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/statusbar.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-137/finalcif/tools/sumformula.py
+-rw-r--r--   0        0        0    96403 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_checkcif.png
+-rw-r--r--   0        0        0   132682 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_details.png
+-rw-r--r--   0        0        0    52874 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_loops.png
+-rw-r--r--   0        0        0    71252 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_loops2.png
+-rw-r--r--   0        0        0    84495 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_main.png
+-rw-r--r--   0        0        0   111861 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_report.png
+-rw-r--r--   0        0        0    75057 2020-02-02 00:00:00.000000 finalcif-137/screenshots/finalcif_responses.png
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 finalcif-137/.gitignore
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-137/LICENSE
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 finalcif-137/README.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 finalcif-137/pyproject.toml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 finalcif-137/PKG-INFO
```

### Comparing `finalcif-136/Finalcif_installer_win.spec` & `finalcif-137/Finalcif_installer_win.spec`

 * *Files identical despite different names*

### Comparing `finalcif-136/Finalcif_linux_onefile.spec` & `finalcif-137/Finalcif_linux_onefile.spec`

 * *Files identical despite different names*

### Comparing `finalcif-136/Finalcif_mac.spec` & `finalcif-137/Finalcif_mac.spec`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif.exe` & `finalcif-137/finalcif.exe`

 * *Files identical despite different names*

### Comparing `finalcif-136/update.exe` & `finalcif-137/update.exe`

 * *Files identical despite different names*

### Comparing `finalcif-136/.run/Make Documentation MAC.run.xml` & `finalcif-137/.run/Make Documentation MAC.run.xml`

 * *Files identical despite different names*

### Comparing `finalcif-136/.run/compile_ui_files.run.xml` & `finalcif-137/.run/compile_ui_files.run.xml`

 * *Files identical despite different names*

### Comparing `finalcif-136/.run/make documentation Windows.run.xml` & `finalcif-137/.run/make documentation Windows.run.xml`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/app_path.py` & `finalcif-137/finalcif/app_path.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/appwindow.py` & `finalcif-137/finalcif/appwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 import sys
 import threading
 import time
 from contextlib import suppress
 from datetime import datetime
 from math import sin, radians
 from pathlib import Path, WindowsPath
-from shutil import which
 from typing import Union, Dict, Tuple, List, Optional
 
 import gemmi.cif
 import requests  # type: ignore
-from PyQt5 import QtCore, QtGui, QtWebEngineWidgets
+from PyQt5 import QtCore, QtGui, QtWebEngineWidgets, QtWidgets
 from PyQt5.QtCore import Qt, QEvent
 from PyQt5.QtWidgets import QMainWindow, QShortcut, QCheckBox, QListWidgetItem, QApplication, \
     QPlainTextEdit, QFileDialog, QMessageBox, QScrollBar
 from gemmi import cif
 
 from finalcif import VERSION
 from finalcif.cif.cif_file_io import CifContainer, GemmiError
@@ -57,14 +56,16 @@
 from finalcif.tools.platon import PlatonRunner
 from finalcif.tools.settings import FinalCifSettings
 from finalcif.tools.shred import ShredCIF
 from finalcif.tools.space_groups import SpaceGroups
 from finalcif.tools.statusbar import StatusBar
 from finalcif.tools.sumformula import formula_str_to_dict, sum_formula_to_html
 
+# QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling)
+
 DEBUG = False
 app = QApplication.instance()
 if app is None:
     app = QApplication([])
 with suppress(ImportError):
     import qtawesome as qta
 from finalcif.cif.checkcif.checkcif import MyHTMLParser, AlertHelp, CheckCif
@@ -629,18 +630,17 @@
         # Not necessary here, it is done in MyCifTable
         # threading.Thread(target=self.ui.cif_main_table.resizeRowsToContents).start()
         # QtCore.QTimer(self).singleShot(0, self.ui.cif_main_table.resizeRowsToContents)
         self.setTextEditSizes()
 
     def setTextEditSizes(self):
         for ui in [self.ui.Spacegroup_top_LineEdit, self.ui.CCDCNumLineEdit, self.ui.SumFormMainLineEdit]:
-            ui.setFixedHeight(self.ui.appendCifPushButton.height() + 6)
-            ui.setFixedHeight(self.ui.appendCifPushButton.height() + 6)
-            ui.setFixedHeight(self.ui.appendCifPushButton.height() + 6)
+            ui.setFixedHeight(self.ui.appendCifPushButton.height())
             vScrollBar = ui.verticalScrollBar()
+            # Scroll down a bit, or text will not be in the vertical center:
             vScrollBar.triggerAction(QScrollBar.SliderSingleStepAdd)
 
     def moveEvent(self, a0: QtGui.QMoveEvent) -> None:
         """Is called when the main window moves."""
         super(AppWindow, self).moveEvent(a0)
         with suppress(AttributeError):
             self._savesize()
@@ -1031,15 +1031,15 @@
             return None
         self.load_cif_file(self.cif.finalcif_file, block=self.ui.datanameComboBox.currentIndex(), load_changes=False)
         self.ui.MainStackedWidget.go_to_checkcif_page()
         runner = PlatonRunner(parent=self,
                               log_widget=self.ui.CheckCifLogPlainTextEdit,
                               output_widget=self.ui.CheckcifPlaintextEdit,
                               cif_file=self.cif.fileobj)
-        if not Path(which(runner.platon_exe)).exists():
+        if runner.platon_exe is not None and not Path(runner.platon_exe).exists():
             self.ui.CheckCifLogPlainTextEdit.setPlainText('\nPlaton executable not found!')
             self.ui.CheckCifLogPlainTextEdit.appendPlainText(
                 'You can download Platon at http://www.platonsoft.nl/platon/\n')
         runner.tick.connect(self.append_to_ciflog_without_newline)
         runner.finished.connect(lambda: self.ui.CheckcifButton.setEnabled(True))
         runner.run_process()
         runner.formula.connect(self.add_moiety_furmula)
@@ -1131,20 +1131,28 @@
                 print('Report without templates')
                 make_report_from(options=self.options, cif=self.cif,
                                  output_filename=str(report_filename), picfile=picfile)
                 if self.cif.is_multi_cif and self.cif.doc[0].name != 'global':
                     make_multi_tables(cif=self.cif, output_filename=str(multi_table_document))
             else:
                 print('Report with templates')
-                t = TemplatedReport(format=ReportFormat.RICHTEXT, options=self.options, cif=self.cif)
-                ok = t.make_templated_docx_report(output_filename=str(report_filename),
-                                                  picfile=picfile,
-                                                  template_path=Path(self.get_checked_templates_list_text()))
-                # t = TemplatedReport(format=ReportFormat.HTML, options=self.options, cif=self.cif)
-                # t.make_templated_html_report(options=self.options, picfile=picfile)
+                template_path = Path(self.get_checked_templates_list_text())
+                ok = False
+                if template_path.suffix in ('.docx',):
+                    t = TemplatedReport(format=ReportFormat.RICHTEXT, options=self.options, cif=self.cif)
+                    ok = t.make_templated_docx_report(output_filename=str(report_filename),
+                                                      picfile=picfile,
+                                                      template_path=Path(self.get_checked_templates_list_text()))
+                elif template_path.suffix in ('.html', '.tmpl'):
+                    t = TemplatedReport(format=ReportFormat.HTML, options=self.options, cif=self.cif)
+                    report_filename = report_filename.with_suffix('.html')
+                    ok = t.make_templated_html_report(output_filename=str(report_filename),
+                                                      picfile=picfile,
+                                                      template_path=template_path.parent,
+                                                      template_file=template_path.name)
                 if not ok:
                     return None
         except FileNotFoundError as e:
             if DEBUG:
                 raise
             print('Unable to make report from cif file.')
             not_ok = e
@@ -1509,14 +1517,15 @@
         except Exception as e:
             not_ok = e
             print(e)
             # if DEBUG:
             raise
             # unable_to_open_message(Path(self.cif.filename), not_ok)
         self.load_recent_cifs_list()
+        self.set_vertical_header_width()
         if self.options.track_changes and load_changes:
             changes_exist = False
             if self.changes_cif_has_zero_size():
                 self.finalcif_changes_filename.unlink(missing_ok=True)
             elif self.finalcif_changes_filename.exists() and self.changes_cif_has_values():
                 changes_exist = True
             if changes_exist and not self.running_inside_unit_test and self.changes_answer == 0 and not self.cif.is_multi_cif:
@@ -1553,14 +1562,24 @@
                 self.ui.cif_main_table.vheaderitems.insert(row_number, vhead_key)
             if self.ui.MainStackedWidget.on_info_page():
                 self.show_residuals()
                 self.redraw_molecule()
             t = QtCore.QTimer(self)
             t.singleShot(1000, self.check_cecksums)
 
+    def set_vertical_header_width(self):
+        """
+        Sets the width of the vertical header to the length of the longest string in the list.
+        """
+        vheader: QtWidgets.QHeaderView = self.ui.cif_main_table.verticalHeader()
+        fm = QtGui.QFontMetrics(vheader.font(), self)
+        # noinspection PyTypeChecker
+        longest_string: str = max(self.ui.cif_main_table.vheaderitems, key=len)
+        vheader.setMaximumWidth(fm.width(longest_string + 'O'))
+
     def changes_cif_has_values(self) -> bool:
         try:
             return not self.get_changes_cif(self.finalcif_changes_filename).is_empty()
         except IndexError:
             return False
 
     def fill_sum_formula_lineedit(self) -> None:
```

### Comparing `finalcif-136/finalcif/finalcif_start.py` & `finalcif-137/finalcif/finalcif_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         sys.excepthook = my_exception_hook
     # windows_style = QStyleFactory.create('Fusion')
     # app.setStyle(windows_style)
     file = None
     if len(sys.argv) > 1:
         file = Path(sys.argv[1])
         if not file.is_file():
-            show_general_warning(parent=None, warn_text=f'The file {file.resolve().absolute()} \nyou tried to open does not exist.',
+            show_general_warning(parent=None,
+                                 warn_text=f'The file {file.resolve().absolute()} \nyou tried to open does not exist.',
                                  window_title='File not found')
             file = None
     app.setQuitOnLastWindowClosed(True)
     w = AppWindow(file=file)
     from PyQt5.QtGui import QIcon
     app.setWindowIcon(QIcon(str(application_path / r'icon/finalcif2.png')))
     w.setWindowTitle('FinalCif v{}'.format(VERSION))
```

### Comparing `finalcif-136/finalcif/cif/all_cif_dicts.py` & `finalcif-137/finalcif/cif/all_cif_dicts.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/atoms.py` & `finalcif-137/finalcif/cif/atoms.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cif_dict_foo.py` & `finalcif-137/finalcif/cif/cif_dict_foo.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,23 @@
                 line = line[padding + 1:]
             else:
                 line = line[padding:]
         newdef += line
     return newdef
 
 
+formats = {
+    'char' : 'string',
+    'uchar': 'case-insensitive string',
+    'numb' : 'number (int or float)',
+    'null' : '? (unknown)' or '. (not applicable)',
+    ''     : '--'
+}
+
+
 def process_cif_dict(cdic):
     """
     Creates a dictionary with cif keywords as key and help text as value.
     """
     alldic = {}
     for x in cdic.keys():
         if '_name' in cdic[x]:
@@ -32,14 +41,15 @@
             name = item['_name']
             if isinstance(item, dict) and not '[]' in name:
                 definition = escape(item['_definition'])
                 example = item.get('_example', '')
                 example_detail = item.get('_example_detail', '')
                 enumeration = item.get('_enumeration', '')
                 enumeration_detail = item.get('_enumeration_detail', '')
+                default = item.get('_enumeration_default', '')
                 if example:
                     if isinstance(example, list) and not enumeration_detail:
                         example = '\n'.join([str(x) for x in example])
                     if isinstance(example, list) and enumeration_detail:
                         example = '\n'.join(
                             ["{}\t\t{}\n".format(str(x), str(y)) for x, y in zip(example, example_detail)])
                     example = format_definition(escape(str(example)))
@@ -48,23 +58,37 @@
                     if isinstance(enumeration, list) and not enumeration_detail:
                         enumeration = '\n'.join([str(x) for x in enumeration])
                     if isinstance(enumeration, list) and enumeration_detail:
                         enumeration = '\n'.join(
                             ["{}\n\t{}\n".format(str(x), str(y)) for x, y in zip(enumeration, enumeration_detail)])
                     enumeration = format_definition(escape(str(enumeration)))
                     definition = '{}\n\n<h3>Example:</h3>\n{}'.format(definition, enumeration)
+                type_format = item.get("_type", "")
+                enum_range = item.get('_enumeration_range', '')
                 if isinstance(name, list):
                     for n in name:
                         # For keys like 'atom_site_aniso_b_[]' where the name has several subnames:
-                        alldic[n] = '<pre><h2>{}</h2>{}</pre>'.format(n, format_definition(definition))
+                        alldic[n] = help_text(definition, n, type_format, enum_range, default)
                 else:
-                    alldic[name] = '<pre><h2>{}</h2>{}</pre>'.format(name, format_definition(definition))
+                    alldic[name] = help_text(definition, name, type_format, enum_range, default)
     return alldic
 
 
+def help_text(definition: str, name: str, type_format: str, enum_range: str, enum_default) -> str:
+    if enum_range.endswith(':'):
+        enum_range = enum_range + '∞'
+    limits = f'\n<br><p><h4>Limits:</h4> {enum_range} </p>'
+    default = f'\n<br><p><h4>Default:</h4> {enum_default} </p>'
+    return (f'<pre><h2>{name}</h2>{format_definition(definition)}</pre>'
+            f'\n<br><p><h4>Type:</h4> {formats.get(type_format, "")}</p>'
+            f'{limits if enum_range else ""}'
+            f'{default if enum_default else ""}'
+            )
+
+
 def load_cif_as_dictionary(link, path_to_cif):
     if not path_to_cif.exists():
         get_dictionary_cif(link, path_to_cif)
     c = gemmi.cif.read_file(str(path_to_cif))
     cdic = json.loads(c.as_json())
     return cdic
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finalcif-136/finalcif/cif/cif_file_io.py` & `finalcif-137/finalcif/cif/cif_file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def finalcif_file_prefixed(self, prefix: str, suffix: str = '-finalcif.cif', force_strip=True) -> Path:
         """
         The full path of the file with a prefix and '-finalcif.cif' attached to the end.
         The suffix needs '-finalcif' in order to contain the finalcif ending.
         "foo/bar/baz-finalcif.cif"
 
-        :param forece_strip: Forces to strip the filename also after the '-finalcif' string.
+        :param force_strip: Forces to strip the filename also after the '-finalcif' string.
         """
         file_witout_finalcif = strip_finalcif_of_name(Path(self.filename).stem, till_name_ends=force_strip)
         filename = self.path_base.joinpath(Path(prefix + file_witout_finalcif + suffix))
         return filename
 
     def get_line_numbers_of_bad_characters(self, filepath: Path):
         line_numbers = []
```

### Comparing `finalcif-136/finalcif/cif/cif_order.py` & `finalcif-137/finalcif/cif/cif_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,21 @@
                 '_refln_F_sigma',
                 '_refln_F_squared_sigma',
                 '_refln_F_calc',
                 '_refln_F_squared_calc',
                 ]
 
 order = [
+    '_audit_update_record',
+    '_audit_contact_author',
+    '_audit_contact_author_name',
+    '_audit_contact_author_phone',
+    '_audit_contact_author_email',
+    '_audit_contact_author_fax',
+    '_audit_contact_author_address',
     '_audit_author_id',
     '_audit_author_id_audit',
     '_audit_author_name',
     '_audit_author_address',
     '_audit_author_email',
     '_audit_author_phone',
     '_audit_author_fax',
@@ -124,15 +131,14 @@
     '_publ_contact_author_email',
     '_publ_contact_author_phone',
     '_publ_contact_author_fax',
     '_publ_contact_author_id_iucr',
     '_publ_contact_author_id_orcid',
     '_publ_contact_author_footnote',
 
-
     '_shelx_SHELXL_version_number',
     '_chemical_name_systematic',
     '_chemical_name_common',
     '_chemical_formula_sum',
     '_chemical_formula_moiety',
     '_chemical_formula_structural',
     '_chemical_formula_analytical',
@@ -337,8 +343,21 @@
     '_atom_type_scat_dispersion_real',
     '_atom_type_scat_dispersion_imag',
     '_atom_type_scat_source',
 
     '_geom_details',
     '_geom_special_details',
 
+    '_bruker_diffrn_runs_wavelength',
+    '_bruker_diffrn_runs_temperature',
+    '_bruker_diffrn_runs_current',
+    '_bruker_diffrn_runs_voltage',
+    '_bruker_diffrn_runs_images',
+    '_bruker_diffrn_runs_time',
+    '_bruker_diffrn_runs_width',
+    '_bruker_diffrn_runs_axis',
+    '_bruker_diffrn_runs_chi',
+    '_bruker_diffrn_runs_phi',
+    '_bruker_diffrn_runs_omega',
+    '_bruker_diffrn_runs_theta',
+    '_bruker_diffrn_runs_distance',
 ]
```

### Comparing `finalcif-136/finalcif/cif/hkl.py` & `finalcif-137/finalcif/cif/hkl.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/modulation_dict.py` & `finalcif-137/finalcif/cif/modulation_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,20 @@
                                                'A description of the linear combination involved '
                                                'in a given\n'
                                                ' Fourier wave vector used to describe the atomic '
                                                'modulation\n'
                                                ' functions.\n'
                                                '\n'
                                                '<h3>Example:</h3>\n'
-                                               'q(4)=q(1)+q(2)</pre>',
+                                               'q(4)=q(1)+q(2)</pre>\n'
+                                               '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_Fourier_wave_vector_seq_id': '<pre><h2>_atom_site_Fourier_wave_vector_seq_id</h2> A '
                                           'numeric code identifying the wave vectors defined in\n'
-                                          ' _atom_site_Fourier_wave_vector_.</pre>',
+                                          ' _atom_site_Fourier_wave_vector_.</pre>\n'
+                                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_Fourier_wave_vector_x': '<pre><h2>_atom_site_Fourier_wave_vector_x</h2> Wave vectors '
                                      'of the Fourier terms used in the structural model\n'
                                      ' to describe the atomic modulation functions, expressed '
                                      'with\n'
                                      ' respect to the three-dimensional reciprocal basis that '
                                      'spans\n'
                                      ' the lattice of main reflections. They are linear '
@@ -24,15 +26,16 @@
                                      'Fourier wave\n'
                                      ' vector is expressed as k=n(1)q(1)+...+n(p)q(p), where p is '
                                      'given\n'
                                      ' by _cell_modulation_dimension. In the case of composites\n'
                                      ' described in a single data block, these wave vectors are\n'
                                      ' expressed with respect to the three-dimensional reciprocal\n'
                                      ' basis of each subsystem (see '
-                                     '_cell_subsystem_matrix_W_).</pre>',
+                                     '_cell_subsystem_matrix_W_).</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_Fourier_wave_vector_y': '<pre><h2>_atom_site_Fourier_wave_vector_y</h2> Wave vectors '
                                      'of the Fourier terms used in the structural model\n'
                                      ' to describe the atomic modulation functions, expressed '
                                      'with\n'
                                      ' respect to the three-dimensional reciprocal basis that '
                                      'spans\n'
                                      ' the lattice of main reflections. They are linear '
@@ -43,15 +46,16 @@
                                      'Fourier wave\n'
                                      ' vector is expressed as k=n(1)q(1)+...+n(p)q(p), where p is '
                                      'given\n'
                                      ' by _cell_modulation_dimension. In the case of composites\n'
                                      ' described in a single data block, these wave vectors are\n'
                                      ' expressed with respect to the three-dimensional reciprocal\n'
                                      ' basis of each subsystem (see '
-                                     '_cell_subsystem_matrix_W_).</pre>',
+                                     '_cell_subsystem_matrix_W_).</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_Fourier_wave_vector_z': '<pre><h2>_atom_site_Fourier_wave_vector_z</h2> Wave vectors '
                                      'of the Fourier terms used in the structural model\n'
                                      ' to describe the atomic modulation functions, expressed '
                                      'with\n'
                                      ' respect to the three-dimensional reciprocal basis that '
                                      'spans\n'
                                      ' the lattice of main reflections. They are linear '
@@ -62,15 +66,16 @@
                                      'Fourier wave\n'
                                      ' vector is expressed as k=n(1)q(1)+...+n(p)q(p), where p is '
                                      'given\n'
                                      ' by _cell_modulation_dimension. In the case of composites\n'
                                      ' described in a single data block, these wave vectors are\n'
                                      ' expressed with respect to the three-dimensional reciprocal\n'
                                      ' basis of each subsystem (see '
-                                     '_cell_subsystem_matrix_W_).</pre>',
+                                     '_cell_subsystem_matrix_W_).</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_U_Fourier_atom_site_label': '<pre><h2>_atom_site_U_Fourier_atom_site_label</h2> '
                                          'Modulation parameters are usually looped in separate '
                                          'lists.\n'
                                          ' Modulated parameters are the atom positions '
                                          '(displacive\n'
                                          ' modulation), the atomic occupation (occupational '
                                          'modulation)\n'
@@ -85,18 +90,20 @@
                                          ' identifies an atom in a loop in which the Fourier '
                                          'components of\n'
                                          ' its thermal-parameters modulation are listed.  This '
                                          'code must\n'
                                          ' match the _atom_site_label of the associated coordinate '
                                          'list\n'
                                          ' and conform to the rules described in '
-                                         '_atom_site_label.</pre>',
+                                         '_atom_site_label.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_U_Fourier_id': '<pre><h2>_atom_site_U_Fourier_id</h2> A code identifying each Fourier '
                             'component used to describe the\n'
-                            ' modulation of the atomic thermal parameters.</pre>',
+                            ' modulation of the atomic thermal parameters.</pre>\n'
+                            '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_U_Fourier_param_cos': '<pre><h2>_atom_site_U_Fourier_param_cos</h2> The modulation of '
                                    'the atomic thermal parameters is usually\n'
                                    ' parameterized by Fourier series. Each term of the series\n'
                                    ' commonly adopts two different representations: the '
                                    'sine-cosine\n'
                                    ' form,\n'
                                    '          U(ij)c cos(2\\p k r)+U(ij)s sin(2\\p k r),\n'
@@ -105,21 +112,23 @@
                                    ' where k is the wave vector of the term and r is the atomic\n'
                                    ' average position. _atom_site_U_Fourier_param_cos is the '
                                    'cosine\n'
                                    ' coefficient [U(ij)c], in angstroms squared, corresponding to\n'
                                    ' the Fourier term defined by\n'
                                    ' _atom_site_U_Fourier_atom_site_label,\n'
                                    ' _atom_site_U_Fourier_tens_elem and\n'
-                                   ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>',
+                                   ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_U_Fourier_param_id': '<pre><h2>_atom_site_U_Fourier_param_id</h2> A code identifying '
                                   'the (in general complex) coefficient of each\n'
                                   ' term present in the Fourier series describing the modulation '
                                   'of\n'
                                   ' the atomic thermal parameters. This code must match\n'
-                                  ' _atom_site_U_Fourier_id.</pre>',
+                                  ' _atom_site_U_Fourier_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_U_Fourier_param_modulus': '<pre><h2>_atom_site_U_Fourier_param_modulus</h2> The '
                                        'modulation of the atomic thermal parameters is usually\n'
                                        ' parameterized by Fourier series. Each term of the series\n'
                                        ' commonly adopts two different representations: the '
                                        'sine-cosine\n'
                                        ' form,\n'
                                        '          U(ij)c cos(2\\p k r)+U(ij)s sin(2\\p k r),\n'
@@ -129,15 +138,17 @@
                                        'atomic\n'
                                        ' average position. _atom_site_U_Fourier_param_modulus is '
                                        'the\n'
                                        ' modulus [|U(ij)|], in angstroms squared, of the complex\n'
                                        ' amplitudes corresponding to the Fourier term defined by\n'
                                        ' _atom_site_U_Fourier_atom_site_label,\n'
                                        ' _atom_site_U_Fourier_tens_elem and\n'
-                                       ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>',
+                                       ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_atom_site_U_Fourier_param_phase': '<pre><h2>_atom_site_U_Fourier_param_phase</h2> The '
                                      'modulation of the atomic thermal parameters is usually\n'
                                      ' parameterized by Fourier series. Each term of the series\n'
                                      ' commonly adopts two different representations: the '
                                      'sine-cosine\n'
                                      ' form,\n'
                                      '          U(ij)c cos(2\\p k r)+U(ij)s sin(2\\p k r),\n'
@@ -147,15 +158,17 @@
                                      ' average position. _atom_site_U_Fourier_param_phase is the '
                                      'phase\n'
                                      ' (\\c/2\\p), in cycles, of the complex amplitude '
                                      'corresponding to\n'
                                      ' the Fourier term defined by '
                                      '_atom_site_U_Fourier_atom_site_label,\n'
                                      ' _atom_site_U_Fourier_tens_elem and\n'
-                                     ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>',
+                                     ' _atom_site_U_Fourier_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                     '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_site_U_Fourier_param_sin': '<pre><h2>_atom_site_U_Fourier_param_sin</h2> The modulation of '
                                    'the atomic thermal parameters is usually\n'
                                    ' parameterized by Fourier series. Each term of the series\n'
                                    ' commonly adopts two different representations: the '
                                    'sine-cosine\n'
                                    ' form,\n'
                                    '          U(ij)c cos(2\\p k r)+U(ij)s sin(2\\p k r),\n'
@@ -163,15 +176,16 @@
                                    '          |U(ij)| cos(2\\p k r+\\c),\n'
                                    ' where k is the wave vector of the term and r is the atomic\n'
                                    ' average position. _atom_site_U_Fourier_param_sin is the sine\n'
                                    ' coefficient [U(ij)s], in angstroms squared, corresponding to\n'
                                    ' the Fourier term defined by\n'
                                    ' _atom_site_U_Fourier_atom_site_label,\n'
                                    ' _atom_site_U_Fourier_tens_elem\n'
-                                   ' and _atom_site_U_Fourier_wave_vector_seq_id.</pre>',
+                                   ' and _atom_site_U_Fourier_wave_vector_seq_id.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_U_Fourier_tens_elem': '<pre><h2>_atom_site_U_Fourier_tens_elem</h2> A label '
                                    'identifying the temperature tensor element U(ij) of a\n'
                                    ' given atom or rigid group whose modulation is being '
                                    'parameterized\n'
                                    ' by Fourier series.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
@@ -191,23 +205,25 @@
                                    '\tmodulation of U23\n'
                                    '\n'
                                    'U33\n'
                                    '\tmodulation of U33\n'
                                    '\n'
                                    'Uiso\n'
                                    '\tmodulation of U~isotropic~\n'
-                                   '</pre>',
+                                   '</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_U_Fourier_wave_vector_seq_id': '<pre><h2>_atom_site_U_Fourier_wave_vector_seq_id</h2> '
                                             'A numeric code identifying the wave vectors of the '
                                             'Fourier terms\n'
                                             ' used to describe the modulation functions '
                                             'corresponding to the\n'
                                             ' temperature factors of an atom or rigid group. This '
                                             'code must\n'
-                                            ' match _atom_site_Fourier_wave_vector_seq_id.</pre>',
+                                            ' match _atom_site_Fourier_wave_vector_seq_id.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_U_modulation_flag': '<pre><h2>_atom_site_U_modulation_flag</h2> A code that signals '
                                  'whether the structural model includes the\n'
                                  ' modulation of the thermal parameters of a given atom\n'
                                  ' site.\n'
                                  '\n'
                                  '<h3>Example:</h3>\n'
                                  'yes\n'
@@ -217,22 +233,25 @@
                                  '\tabbreviation for "yes"\n'
                                  '\n'
                                  'no\n'
                                  '\tno modulation of thermal parameters\n'
                                  '\n'
                                  'n\n'
                                  '\tabbreviation for "no"\n'
-                                 '</pre>',
+                                 '</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>\n'
+                                 '<br><p><h4>Default:</h4> no </p>',
  '_atom_site_[ms]': '<pre><h2>_atom_site_[ms]</h2> Data items in the ATOM_SITE category record '
                     'details about\n'
                     ' the atom sites in a crystal structure, such as the positional\n'
                     ' coordinates, atomic displacement parameters, and magnetic moments\n'
                     ' and directions. This category exists in the core CIF dictionary\n'
                     ' but is extended in this dictionary by the addition of some items\n'
-                    ' that may appear in the main looped list of atom-site information.</pre>',
+                    ' that may appear in the main looped list of atom-site information.</pre>\n'
+                    '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_atom_site_displace_Fourier_atom_site_label': '<pre><h2>_atom_site_displace_Fourier_atom_site_label</h2> '
                                                 'Modulation parameters are usually looped in '
                                                 'separate lists.\n'
                                                 ' Modulated parameters are the atom positions '
                                                 '(displacive\n'
                                                 ' modulation), the atomic occupation (occupational '
                                                 'modulation)\n'
@@ -256,15 +275,16 @@
                                                 ' part (if any) would appear in a separate list '
                                                 '(see\n'
                                                 ' _atom_site_rot_Fourier_atom_site_label). This '
                                                 'code must match\n'
                                                 ' the _atom_site_label of the associated '
                                                 'coordinate list and\n'
                                                 ' conform to the rules described in '
-                                                '_atom_site_label.</pre>',
+                                                '_atom_site_label.</pre>\n'
+                                                '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_displace_Fourier_axis': '<pre><h2>_atom_site_displace_Fourier_axis</h2> A label '
                                      'identifying the displacement component of a given atom\n'
                                      ' or rigid group that is being parameterized by Fourier '
                                      'series. a,\n'
                                      ' b and c are the basic lattice vectors of the reference '
                                      'structure.\n'
                                      ' For composites they refer to the reference structure of '
@@ -286,22 +306,24 @@
                                      '\tdisplacement along an arbitrary a1 axis\n'
                                      '\n'
                                      'a2\n'
                                      '\tdisplacement along an arbitrary a2 axis\n'
                                      '\n'
                                      'a3\n'
                                      '\tdisplacement along an arbitrary a3 axis\n'
-                                     '</pre>',
+                                     '</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_displace_Fourier_id': '<pre><h2>_atom_site_displace_Fourier_id</h2> A code '
                                    'identifying each component of the displacive modulation of\n'
                                    ' a given atom or rigid group when the modulation is expressed '
                                    'in\n'
                                    ' terms of Fourier series. In the case of a rigid group, it\n'
                                    ' applies only to the translational part of the '
-                                   'distortion.</pre>',
+                                   'distortion.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_displace_Fourier_param_cos': '<pre><h2>_atom_site_displace_Fourier_param_cos</h2> The '
                                           'displacive distortion of a given atom or rigid group '
                                           '(see\n'
                                           ' also _atom_site_rot_Fourier_param_cos) is usually '
                                           'parameterized\n'
                                           ' by Fourier series. Each term of the series commonly '
                                           'adopts two\n'
@@ -320,26 +342,28 @@
                                           ' _atom_site_displace_Fourier_wave_vector_seq_id. Atomic '
                                           'or rigid-\n'
                                           ' group displacements must be expressed as fractions of '
                                           'the unit\n'
                                           ' cell or in angstroms if the modulations are referred '
                                           'to some\n'
                                           ' special axes defined by\n'
-                                          ' _atom_sites_displace_Fourier_axes_description.</pre>',
+                                          ' _atom_sites_displace_Fourier_axes_description.</pre>\n'
+                                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_Fourier_param_id': '<pre><h2>_atom_site_displace_Fourier_param_id</h2> A '
                                          'code identifying the (in general complex) coefficient of '
                                          'each\n'
                                          ' term present in the Fourier series describing the '
                                          'displacive\n'
                                          ' modulation of a given atom or rigid group. In the case '
                                          'of a rigid\n'
                                          ' group, it applies only to the translational part of '
                                          'the\n'
                                          ' distortion. This code must match '
-                                         '_atom_site_displace_Fourier_id.</pre>',
+                                         '_atom_site_displace_Fourier_id.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_displace_Fourier_param_modulus': '<pre><h2>_atom_site_displace_Fourier_param_modulus</h2> '
                                               'The displacive distortion of a given atom or rigid '
                                               'group (see\n'
                                               ' also _atom_site_rot_Fourier_param_modulus) is '
                                               'usually\n'
                                               ' parameterized by Fourier series. Each term of the '
                                               'series commonly\n'
@@ -361,15 +385,17 @@
                                               'Atomic or rigid-\n'
                                               ' group displacements must be expressed as fractions '
                                               'of the unit\n'
                                               ' cell or in angstroms if the modulations are '
                                               'referred to some\n'
                                               ' special axes defined by\n'
                                               ' '
-                                              '_atom_sites_displace_Fourier_axes_description.</pre>',
+                                              '_atom_sites_displace_Fourier_axes_description.</pre>\n'
+                                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                              '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_atom_site_displace_Fourier_param_phase': '<pre><h2>_atom_site_displace_Fourier_param_phase</h2> '
                                             'The displacive distortion of a given atom or rigid '
                                             'group (see\n'
                                             ' also _atom_site_rot_Fourier_param_phase) is usually '
                                             'parameterized\n'
                                             ' by Fourier series. Each term of the series commonly '
                                             'adopts two\n'
@@ -383,15 +409,17 @@
                                             '_atom_site_displace_Fourier_param_phase is the\n'
                                             ' phase (\\f/2\\p) in cycles of the complex amplitude '
                                             'corresponding\n'
                                             ' to the Fourier term defined by\n'
                                             ' _atom_site_displace_Fourier_atom_site_label,\n'
                                             ' _atom_site_displace_Fourier_axis and\n'
                                             ' '
-                                            '_atom_site_displace_Fourier_wave_vector_seq_id.</pre>',
+                                            '_atom_site_displace_Fourier_wave_vector_seq_id.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_site_displace_Fourier_param_sin': '<pre><h2>_atom_site_displace_Fourier_param_sin</h2> The '
                                           'displacive distortion of a given atom or rigid group '
                                           '(see\n'
                                           ' also _atom_site_rot_Fourier_param_sin) is usually '
                                           'parameterized\n'
                                           ' by Fourier series. Each term of the series commonly '
                                           'adopts two\n'
@@ -410,26 +438,29 @@
                                           ' _atom_site_displace_Fourier_wave_vector_seq_id. Atomic '
                                           'or rigid-\n'
                                           ' group displacements must be expressed as fractions of '
                                           'the unit\n'
                                           ' cell or in angstroms if the modulations are referred '
                                           'to some\n'
                                           ' special axes defined by\n'
-                                          ' _atom_sites_displace_Fourier_axes_description.</pre>',
+                                          ' _atom_sites_displace_Fourier_axes_description.</pre>\n'
+                                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_Fourier_wave_vector_seq_id': '<pre><h2>_atom_site_displace_Fourier_wave_vector_seq_id</h2> '
                                                    'A numeric code identifying the wave vectors of '
                                                    'the Fourier terms\n'
                                                    ' used in the structural model to describe the '
                                                    'displacive\n'
                                                    ' modulation of an atom or rigid group. In the '
                                                    'case of a rigid\n'
                                                    ' group, it applies only to the translational '
                                                    'part of the\n'
                                                    ' distortion. This code must match\n'
-                                                   ' _atom_site_Fourier_wave_vector_seq_id.</pre>',
+                                                   ' _atom_site_Fourier_wave_vector_seq_id.</pre>\n'
+                                                   '<br><p><h4>Type:</h4> number (int or '
+                                                   'float)</p>',
  '_atom_site_displace_modulation_flag': '<pre><h2>_atom_site_displace_modulation_flag</h2> A code '
                                         'that signals whether the structural model includes the\n'
                                         ' modulation of the positional coordinates of a given '
                                         'atom\n'
                                         ' site.\n'
                                         '\n'
                                         '<h3>Example:</h3>\n'
@@ -440,25 +471,28 @@
                                         '\tabbreviation for "yes"\n'
                                         '\n'
                                         'no\n'
                                         '\tno displacive modulation\n'
                                         '\n'
                                         'n\n'
                                         '\tabbreviation for "no"\n'
-                                        '</pre>',
+                                        '</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>\n'
+                                        '<br><p><h4>Default:</h4> no </p>',
  '_atom_site_displace_special_func_atom_site_label': '<pre><h2>_atom_site_displace_special_func_atom_site_label</h2> '
                                                      'The code that identifies an atom in a loop '
                                                      'in which the special\n'
                                                      ' function that describes its displacive '
                                                      'modulation is being\n'
                                                      ' defined. This code must match the '
                                                      '_atom_site_label of the\n'
                                                      ' associated coordinate list and conform to '
                                                      'the rules described in\n'
-                                                     ' _atom_site_label.</pre>',
+                                                     ' _atom_site_label.</pre>\n'
+                                                     '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_displace_special_func_sawtooth_ax': '<pre><h2>_atom_site_displace_special_func_sawtooth_ax</h2>  '
                                                  '_atom_site_displace_special_func_sawtooth_ items '
                                                  'are the\n'
                                                  '  adjustable parameters of a sawtooth function.\n'
                                                  '\n'
                                                  '  A displacive sawtooth function along the '
                                                  'internal space is\n'
@@ -486,15 +520,16 @@
                                                  '2000).\n'
                                                  '\n'
                                                  '  Reference: Petricek, V. &amp; Dusek, M. '
                                                  '(2000). JANA2000. The\n'
                                                  '  crystallographic computing system. Institute '
                                                  'of Physics, Prague,\n'
                                                  '  Czech Republic.\n'
-                                                 '</pre>',
+                                                 '</pre>\n'
+                                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_special_func_sawtooth_ay': '<pre><h2>_atom_site_displace_special_func_sawtooth_ay</h2>  '
                                                  '_atom_site_displace_special_func_sawtooth_ items '
                                                  'are the\n'
                                                  '  adjustable parameters of a sawtooth function.\n'
                                                  '\n'
                                                  '  A displacive sawtooth function along the '
                                                  'internal space is\n'
@@ -522,15 +557,16 @@
                                                  '2000).\n'
                                                  '\n'
                                                  '  Reference: Petricek, V. &amp; Dusek, M. '
                                                  '(2000). JANA2000. The\n'
                                                  '  crystallographic computing system. Institute '
                                                  'of Physics, Prague,\n'
                                                  '  Czech Republic.\n'
-                                                 '</pre>',
+                                                 '</pre>\n'
+                                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_special_func_sawtooth_az': '<pre><h2>_atom_site_displace_special_func_sawtooth_az</h2>  '
                                                  '_atom_site_displace_special_func_sawtooth_ items '
                                                  'are the\n'
                                                  '  adjustable parameters of a sawtooth function.\n'
                                                  '\n'
                                                  '  A displacive sawtooth function along the '
                                                  'internal space is\n'
@@ -558,15 +594,16 @@
                                                  '2000).\n'
                                                  '\n'
                                                  '  Reference: Petricek, V. &amp; Dusek, M. '
                                                  '(2000). JANA2000. The\n'
                                                  '  crystallographic computing system. Institute '
                                                  'of Physics, Prague,\n'
                                                  '  Czech Republic.\n'
-                                                 '</pre>',
+                                                 '</pre>\n'
+                                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_special_func_sawtooth_c': '<pre><h2>_atom_site_displace_special_func_sawtooth_c</h2>  '
                                                 '_atom_site_displace_special_func_sawtooth_ items '
                                                 'are the\n'
                                                 '  adjustable parameters of a sawtooth function.\n'
                                                 '\n'
                                                 '  A displacive sawtooth function along the '
                                                 'internal space is\n'
@@ -594,15 +631,16 @@
                                                 '2000).\n'
                                                 '\n'
                                                 '  Reference: Petricek, V. &amp; Dusek, M. (2000). '
                                                 'JANA2000. The\n'
                                                 '  crystallographic computing system. Institute of '
                                                 'Physics, Prague,\n'
                                                 '  Czech Republic.\n'
-                                                '</pre>',
+                                                '</pre>\n'
+                                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_displace_special_func_sawtooth_w': '<pre><h2>_atom_site_displace_special_func_sawtooth_w</h2>  '
                                                 '_atom_site_displace_special_func_sawtooth_ items '
                                                 'are the\n'
                                                 '  adjustable parameters of a sawtooth function.\n'
                                                 '\n'
                                                 '  A displacive sawtooth function along the '
                                                 'internal space is\n'
@@ -630,15 +668,16 @@
                                                 '2000).\n'
                                                 '\n'
                                                 '  Reference: Petricek, V. &amp; Dusek, M. (2000). '
                                                 'JANA2000. The\n'
                                                 '  crystallographic computing system. Institute of '
                                                 'Physics, Prague,\n'
                                                 '  Czech Republic.\n'
-                                                '</pre>',
+                                                '</pre>\n'
+                                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_occ_Fourier_atom_site_label': '<pre><h2>_atom_site_occ_Fourier_atom_site_label</h2> '
                                            'Modulation parameters are usually looped in separate '
                                            'lists.\n'
                                            ' Modulated parameters are the atom positions '
                                            '(displacive\n'
                                            ' modulation), the atomic occupation (occupational '
                                            'modulation)\n'
@@ -653,19 +692,21 @@
                                            ' identifies an atom in a loop in which the Fourier '
                                            'components of\n'
                                            ' its occupational modulation are listed. This code '
                                            'must\n'
                                            ' match the _atom_site_label of the associated '
                                            'coordinate list and\n'
                                            ' conform to the rules described in '
-                                           '_atom_site_label.</pre>',
+                                           '_atom_site_label.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_occ_Fourier_id': '<pre><h2>_atom_site_occ_Fourier_id</h2> A code identifying each '
                               'component of the occupational modulation\n'
                               ' of a given atom or rigid group when the modulation is\n'
-                              ' expressed in terms of Fourier series.</pre>',
+                              ' expressed in terms of Fourier series.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_occ_Fourier_param_cos': '<pre><h2>_atom_site_occ_Fourier_param_cos</h2> The '
                                      'occupational distortion of a given atom or rigid group is\n'
                                      ' usually parameterized by Fourier series. Each term of the '
                                      'series\n'
                                      ' commonly adopts two different representations: the '
                                      'sine-cosine\n'
                                      ' form,\n'
@@ -674,22 +715,24 @@
                                      '          |P| cos(2\\p k r+\\d),\n'
                                      ' where k is the wave vector of the term and r is the atomic\n'
                                      ' average position. _atom_site_occ_Fourier_param_cos is the '
                                      'cosine\n'
                                      ' coefficient (Pc) corresponding to the Fourier term defined '
                                      'by\n'
                                      ' _atom_site_occ_Fourier_atom_site_label and\n'
-                                     ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>',
+                                     ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_occ_Fourier_param_id': '<pre><h2>_atom_site_occ_Fourier_param_id</h2> A code '
                                     'identifying the (in general complex) coefficient of each\n'
                                     ' term present in the Fourier series describing the '
                                     'occupational\n'
                                     ' modulation of a given atom or rigid group. This code must '
                                     'match\n'
-                                    ' _atom_site_occ_Fourier_id.</pre>',
+                                    ' _atom_site_occ_Fourier_id.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_occ_Fourier_param_modulus': '<pre><h2>_atom_site_occ_Fourier_param_modulus</h2> The '
                                          'occupational distortion of a given atom or rigid group '
                                          'is\n'
                                          ' usually parameterized by Fourier series. Each term of '
                                          'the series\n'
                                          ' commonly adopts two different representations: the '
                                          'sine-cosine\n'
@@ -701,15 +744,17 @@
                                          'atomic\n'
                                          ' average position. _atom_site_occ_Fourier_param_modulus '
                                          'is the\n'
                                          ' modulus (|P|) of the complex amplitude corresponding to '
                                          'the\n'
                                          ' Fourier term defined by '
                                          '_atom_site_occ_Fourier_atom_site_label\n'
-                                         ' and _atom_site_occ_Fourier_wave_vector_seq_id.</pre>',
+                                         ' and _atom_site_occ_Fourier_wave_vector_seq_id.</pre>\n'
+                                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                         '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_atom_site_occ_Fourier_param_phase': '<pre><h2>_atom_site_occ_Fourier_param_phase</h2> The '
                                        'occupational distortion of a given atom or rigid group is\n'
                                        ' usually parameterized by Fourier series. Each term of the '
                                        'series\n'
                                        ' commonly adopts two different representations: the '
                                        'sine-cosine\n'
                                        ' form,\n'
@@ -719,15 +764,17 @@
                                        ' where k is the wave vector of the term and r is the '
                                        'atomic\n'
                                        ' average position. _atom_site_occ_Fourier_param_phase is '
                                        'the phase\n'
                                        ' (\\d/2\\p) in cycles corresponding to the Fourier term '
                                        'defined by\n'
                                        ' _atom_site_occ_Fourier_atom_site_label and\n'
-                                       ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>',
+                                       ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                       '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_site_occ_Fourier_param_sin': '<pre><h2>_atom_site_occ_Fourier_param_sin</h2> The '
                                      'occupational distortion of a given atom or rigid group is\n'
                                      ' usually parameterized by Fourier series. Each term of the '
                                      'series\n'
                                      ' commonly adopts two different representations: the '
                                      'sine-cosine\n'
                                      ' form,\n'
@@ -736,24 +783,26 @@
                                      '          |P| cos(2\\p k r+\\d),\n'
                                      ' where k is the wave vector of the term and r is the atomic\n'
                                      ' average position. _atom_site_occ_Fourier_param_sin is the '
                                      'sine\n'
                                      ' coefficient (Ps) corresponding to the Fourier term defined '
                                      'by\n'
                                      ' _atom_site_occ_Fourier_atom_site_label and\n'
-                                     ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>',
+                                     ' _atom_site_occ_Fourier_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_occ_Fourier_wave_vector_seq_id': '<pre><h2>_atom_site_occ_Fourier_wave_vector_seq_id</h2> '
                                               'A numeric code identifying the wave vectors of the '
                                               'Fourier terms\n'
                                               ' used in the structural model to describe the '
                                               'modulation functions\n'
                                               ' corresponding to the occupational part of the '
                                               'distortion. This\n'
                                               ' code must match '
-                                              '_atom_site_Fourier_wave_vector_seq_id.</pre>',
+                                              '_atom_site_Fourier_wave_vector_seq_id.</pre>\n'
+                                              '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_occ_modulation_flag': '<pre><h2>_atom_site_occ_modulation_flag</h2> A code that '
                                    'signals whether the structural model includes the\n'
                                    ' modulation of the occupation of a given atom site.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'yes\n'
                                    '\toccupational modulation\n'
@@ -762,26 +811,29 @@
                                    '\tabbreviation for "yes"\n'
                                    '\n'
                                    'no\n'
                                    '\tno occupational modulation\n'
                                    '\n'
                                    'n\n'
                                    '\tabbreviation for "no"\n'
-                                   '</pre>',
+                                   '</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> no </p>',
  '_atom_site_occ_special_func_atom_site_label': '<pre><h2>_atom_site_occ_special_func_atom_site_label</h2> '
                                                 'The code that identifies an atom or rigid group '
                                                 'in a loop in\n'
                                                 ' which the parameters of the special function '
                                                 'that describes its\n'
                                                 ' occupational modulation are listed. This code '
                                                 'must match\n'
                                                 ' the _atom_site_label of the associated '
                                                 'coordinate list and\n'
                                                 ' conform to the rules described in '
-                                                '_atom_site_label.</pre>',
+                                                '_atom_site_label.</pre>\n'
+                                                '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_occ_special_func_crenel_c': '<pre><h2>_atom_site_occ_special_func_crenel_c</h2>  '
                                          '_atom_site_occ_special_func_crenel_ items are the '
                                          'adjustable\n'
                                          '  parameters of a crenel function.\n'
                                          '\n'
                                          '  An occupational crenel function along the internal '
                                          'space is\n'
@@ -801,15 +853,16 @@
                                          '  For more details, see the manual for JANA2000\n'
                                          '  (Petricek &amp; Dusek, 2000).\n'
                                          '\n'
                                          '  Reference: Petricek, V. &amp; Dusek, M. (2000). '
                                          'JANA2000. The\n'
                                          '  crystallographic computing system. Institute of '
                                          'Physics, Prague,\n'
-                                         '  Czech Republic.</pre>',
+                                         '  Czech Republic.</pre>\n'
+                                         '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_occ_special_func_crenel_w': '<pre><h2>_atom_site_occ_special_func_crenel_w</h2>  '
                                          '_atom_site_occ_special_func_crenel_ items are the '
                                          'adjustable\n'
                                          '  parameters of a crenel function.\n'
                                          '\n'
                                          '  An occupational crenel function along the internal '
                                          'space is\n'
@@ -829,15 +882,16 @@
                                          '  For more details, see the manual for JANA2000\n'
                                          '  (Petricek &amp; Dusek, 2000).\n'
                                          '\n'
                                          '  Reference: Petricek, V. &amp; Dusek, M. (2000). '
                                          'JANA2000. The\n'
                                          '  crystallographic computing system. Institute of '
                                          'Physics, Prague,\n'
-                                         '  Czech Republic.</pre>',
+                                         '  Czech Republic.</pre>\n'
+                                         '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_phason_atom_site_label': '<pre><h2>_atom_site_phason_atom_site_label</h2> The code '
                                       'that identifies an atom or rigid group in a loop in\n'
                                       ' which the phason coefficients are listed. Although this '
                                       'kind of\n'
                                       ' correction is intended to be overall, some refinement '
                                       'programs\n'
                                       ' (for example, JANA2000) allow an independent phason '
@@ -845,38 +899,42 @@
                                       ' for each atom or rigid group. In this case,\n'
                                       ' _atom_site_phason_formula and _atom_site_phason_coeff '
                                       'should be\n'
                                       ' used (see also _refine_ls_mod_overall_phason_). This code '
                                       'must\n'
                                       ' match the _atom_site_label of the associated coordinate '
                                       'list and\n'
-                                      ' conform to the rules described in _atom_site_label.</pre>',
+                                      ' conform to the rules described in _atom_site_label.</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_phason_coeff': '<pre><h2>_atom_site_phason_coeff</h2> The phason coefficient used to '
                             'calculate (with the appropriate\n'
                             ' expression given in _atom_site_phason_formula) the atomic phason\n'
                             ' correction. Although this kind of correction is intended to be\n'
                             ' overall, some refinement programs (for example, JANA2000) allow\n'
                             ' an independent phason correction for each atom or rigid group. In\n'
                             ' this case, _atom_site_phason_formula and _atom_site_phason_coeff\n'
-                            ' should be used (see also _refine_ls_mod_overall_phason_).</pre>',
+                            ' should be used (see also _refine_ls_mod_overall_phason_).</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_atom_site_phason_formula': '<pre><h2>_atom_site_phason_formula</h2> The formula used for the '
                               'phason correction. Although both kinds\n'
                               ' of corrections are intended to be overall, some refinement\n'
                               ' programs (for example, JANA2000) allow an independent phason\n'
                               ' correction for each atom or rigid group. In this case,\n'
                               ' _atom_site_phason_formula and _atom_site_phason_coeff should\n'
                               ' be used (see also _refine_ls_mod_overall_phason_).\n'
                               '\n'
                               '<h3>Example:</h3>\n'
                               'Axe\n'
                               '\tAxe, J. D. (1980). Phys. Rev. B, 21, 4181-4190.\n'
                               '\n'
                               'Ovr\n'
                               '\tOverhauser, A. W. (1971). Phys. Rev. B, 3, 3173-3182.\n'
-                              '</pre>',
+                              '</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_rot_Fourier_atom_site_label': '<pre><h2>_atom_site_rot_Fourier_atom_site_label</h2> '
                                            'Modulation parameters are usually looped in separate '
                                            'lists.\n'
                                            ' Modulated parameters are the atom positions '
                                            '(displacive\n'
                                            ' modulation), the atomic occupation (occupational '
                                            'modulation)\n'
@@ -896,15 +954,16 @@
                                            'appear in a\n'
                                            ' separate list (see '
                                            '_atom_site_displace_Fourier_atom_site_label).\n'
                                            ' This code must match the _atom_site_label of the '
                                            'associated\n'
                                            ' coordinate list and conform to the rules described '
                                            'in\n'
-                                           ' _atom_site_label.</pre>',
+                                           ' _atom_site_label.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_rot_Fourier_axis': '<pre><h2>_atom_site_rot_Fourier_axis</h2> A label identifying the '
                                 'rotation component around a fixed point\n'
                                 ' of a given rigid group whose modulation is being parameterized '
                                 'by\n'
                                 ' Fourier series. a, b and c are the basic lattice vectors of the\n'
                                 ' reference structure. For composites they refer to the reference\n'
                                 ' structure of each subsystem. a~1~, a~2~ and a~3~ are defined by\n'
@@ -924,19 +983,21 @@
                                 '\trotation around an arbitrary a1 axis\n'
                                 '\n'
                                 'a2\n'
                                 '\trotation around an arbitrary a2 axis\n'
                                 '\n'
                                 'a3\n'
                                 '\trotation around an arbitrary a3 axis\n'
-                                '</pre>',
+                                '</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_rot_Fourier_id': '<pre><h2>_atom_site_rot_Fourier_id</h2> A code identifying each '
                               'component of the rotational modulation of\n'
                               ' a given rigid group when the modulation is expressed in terms of\n'
-                              ' Fourier series.</pre>',
+                              ' Fourier series.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_rot_Fourier_param_cos': '<pre><h2>_atom_site_rot_Fourier_param_cos</h2> The '
                                      'displacive distortion of a given rigid group is not\n'
                                      ' completely described by _atom_site_displace_Fourier_. The '
                                      'rigid\n'
                                      ' rotation of the group around a given axis passing through a '
                                      'fixed\n'
                                      ' point (for example, the centre of mass of the group) is '
@@ -951,22 +1012,24 @@
                                      ' where k is the wave vector of the term and r is the atomic\n'
                                      ' average position. _atom_site_rot_Fourier_param_cos is the '
                                      'cosine\n'
                                      ' coefficient (Rc) in degrees corresponding to the Fourier '
                                      'term\n'
                                      ' defined by _atom_site_rot_Fourier_atom_site_label,\n'
                                      ' _atom_site_rot_Fourier_axis and\n'
-                                     ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>',
+                                     ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_rot_Fourier_param_id': '<pre><h2>_atom_site_rot_Fourier_param_id</h2> A code '
                                     'identifying the (in general complex) coefficient of each\n'
                                     ' term present in the Fourier series describing the rotational '
                                     'part\n'
                                     ' of the displacive modulation of a given rigid group. This '
                                     'code\n'
-                                    ' must match _atom_site_rot_Fourier_id.</pre>',
+                                    ' must match _atom_site_rot_Fourier_id.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_atom_site_rot_Fourier_param_modulus': '<pre><h2>_atom_site_rot_Fourier_param_modulus</h2> The '
                                          'displacive distortion of a given rigid group is not\n'
                                          ' completely described by _atom_site_displace_Fourier_. '
                                          'The rigid\n'
                                          ' rotation of the group around a given axis passing '
                                          'through a fixed\n'
                                          ' point (for example, the centre of mass of the group) is '
@@ -984,15 +1047,17 @@
                                          ' average position. _atom_site_rot_Fourier_param_modulus '
                                          'is the\n'
                                          ' modulus (|R|) in degrees of the complex amplitude '
                                          'corresponding\n'
                                          ' to the Fourier term defined by\n'
                                          ' _atom_site_rot_Fourier_atom_site_label,\n'
                                          ' _atom_site_rot_Fourier_axis and\n'
-                                         ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>',
+                                         ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>\n'
+                                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                         '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_atom_site_rot_Fourier_param_phase': '<pre><h2>_atom_site_rot_Fourier_param_phase</h2> The '
                                        'displacive distortion of a given rigid group is not\n'
                                        ' completely described by _atom_site_displace_Fourier_. The '
                                        'rigid\n'
                                        ' rotation of the group around a given axis passing through '
                                        'a fixed\n'
                                        ' point (for example, the centre of mass of the group) is '
@@ -1009,15 +1074,17 @@
                                        ' average position. _atom_site_rot_Fourier_param_phase is '
                                        'the phase\n'
                                        ' (\\y/2\\p) in cycles of the complex amplitude '
                                        'corresponding to the\n'
                                        ' Fourier term defined by '
                                        '_atom_site_rot_Fourier_atom_site_label,\n'
                                        ' _atom_site_rot_Fourier_axis and\n'
-                                       ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>',
+                                       ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                       '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_site_rot_Fourier_param_sin': '<pre><h2>_atom_site_rot_Fourier_param_sin</h2> The '
                                      'displacive distortion of a given rigid group is not\n'
                                      ' completely described by _atom_site_displace_Fourier_. The '
                                      'rigid\n'
                                      ' rotation of the group around a given axis passing through a '
                                      'fixed\n'
                                      ' point (for example, the centre of mass of the group) is '
@@ -1032,43 +1099,47 @@
                                      ' where k is the wave vector of the term and r is the atomic\n'
                                      ' average position. _atom_site_rot_Fourier_param_sin is the '
                                      'sine\n'
                                      ' coefficient (Rs) in degrees corresponding to the Fourier '
                                      'term\n'
                                      ' defined by _atom_site_rot_Fourier_atom_site_label,\n'
                                      ' _atom_site_rot_Fourier_axis and\n'
-                                     ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>',
+                                     ' _atom_site_rot_Fourier_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_rot_Fourier_wave_vector_seq_id': '<pre><h2>_atom_site_rot_Fourier_wave_vector_seq_id</h2> '
                                               'A numeric code identifying the wave vectors of the '
                                               'Fourier terms\n'
                                               ' used in the structural model to describe the '
                                               'modulation functions\n'
                                               ' corresponding to the rotational distortion of a '
                                               'rigid group. This\n'
                                               ' code must match '
-                                              '_atom_site_Fourier_wave_vector_seq_id.</pre>',
+                                              '_atom_site_Fourier_wave_vector_seq_id.</pre>\n'
+                                              '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_atom_site_subsystem_code': '<pre><h2>_atom_site_subsystem_code</h2> A code that links a given '
                               'atom or rigid-group site to one of the\n'
                               ' subsystems present in a composite. This code provides an\n'
                               ' alternative description for composites which is less explicit\n'
                               ' than that based on linked data blocks (see the description in\n'
                               ' this dictionary of _audit_link_[ms]). It must match one of\n'
-                              ' the labels specified for _cell_subsystem_code.</pre>',
+                              ' the labels specified for _cell_subsystem_code.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_atom_sites_displace_Fourier_axes_description': '<pre><h2>_atom_sites_displace_Fourier_axes_description</h2> '
                                                   'The definition of the axes used for describing '
                                                   'the displacive\n'
                                                   ' modulation, parameterized by Fourier series, '
                                                   'when they are other\n'
                                                   ' than the crystallographic axes.\n'
                                                   '\n'
                                                   '<h3>Example:</h3>\n'
                                                   ' a1 and a2 are respectively the long molecular '
                                                   'axis\n'
                                                   ' and the axis normal to the mean molecular '
-                                                  'plane.</pre>',
+                                                  'plane.</pre>\n'
+                                                  '<br><p><h4>Type:</h4> string</p>',
  '_atom_sites_modulation_global_phase_t_1': '<pre><h2>_atom_sites_modulation_global_phase_t_1</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1088,15 +1159,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_2': '<pre><h2>_atom_sites_modulation_global_phase_t_2</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1116,15 +1189,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_3': '<pre><h2>_atom_sites_modulation_global_phase_t_3</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1144,15 +1219,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_4': '<pre><h2>_atom_sites_modulation_global_phase_t_4</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1172,15 +1249,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_5': '<pre><h2>_atom_sites_modulation_global_phase_t_5</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1200,15 +1279,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_6': '<pre><h2>_atom_sites_modulation_global_phase_t_6</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1228,15 +1309,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_7': '<pre><h2>_atom_sites_modulation_global_phase_t_7</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1256,15 +1339,17 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_modulation_global_phase_t_8': '<pre><h2>_atom_sites_modulation_global_phase_t_8</h2> '
                                             'The initial phases, in cycles, of the modulation '
                                             'waves. For\n'
                                             ' incommensurate structures they are irrelevant. '
                                             'However, they are\n'
                                             ' essential for the description of commensurate '
                                             'structures within\n'
@@ -1284,28 +1369,31 @@
                                             'information can\n'
                                             ' be found in van Smaalen (1995).\n'
                                             '\n'
                                             ' Ref: Perez-Mato, J. M., Madariaga, G., Zu\\~niga, F. '
                                             'J. &amp; Garcia\n'
                                             ' Arribas, A. (1987). Acta Cryst. A43, 216-226. '
                                             'Smaalen, S. van\n'
-                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                            ' (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                            '<br><p><h4>Limits:</h4> -1.0:1.0 </p>',
  '_atom_sites_rot_Fourier_axes_description': '<pre><h2>_atom_sites_rot_Fourier_axes_description</h2> '
                                              'The definition of the axes used for describing the '
                                              'rotational\n'
                                              ' part of the displacive modulation of a given rigid '
                                              'group,\n'
                                              ' parameterized by Fourier series, when they are '
                                              'other than the\n'
                                              ' crystallographic axes.\n'
                                              '\n'
                                              '<h3>Example:</h3>\n'
                                              ' a1 and a2 are respectively the long molecular axis\n'
                                              ' and the axis normal to the mean molecular '
-                                             'plane.</pre>',
+                                             'plane.</pre>\n'
+                                             '<br><p><h4>Type:</h4> string</p>',
  '_audit_link_[ms]': '<pre><h2>_audit_link_[ms]</h2> This category description does NOT introduce '
                      'a new category;\n'
                      ' instead, it describes the recommended practice for using\n'
                      ' block codes as described in the core AUDIT_LINK category for\n'
                      ' descriptions of modulated structures.\n'
                      '\n'
                      ' The value of _audit_block_code may be associated with a data\n'
@@ -1354,23 +1442,27 @@
                      '    _audit_link_block_code\n'
                      '    _audit_link_block_description\n'
                      "       .               'publication details'\n"
                      "       K2SEO4_COM      'experimental data common to ref./mod. structures'\n"
                      "       K2SEO4_REFRNCE  'reference structure'\n"
                      "       K2SEO4_MOD      'modulated structure'\n"
                      '\n'
-                     "    _audit_link_block_code      'PbSVS2_MOD_VS2'</pre>",
+                     "    _audit_link_block_code      'PbSVS2_MOD_VS2'</pre>\n"
+                     '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_[ms]': '<pre><h2>_cell_[ms]</h2> Data items in the CELL category record details about\n'
                ' the crystallographic cell parameters and their measurement.\n'
                ' This category is already defined in the core CIF dictionary\n'
                ' but is extended in this dictionary by the addition of some items\n'
-               ' that are specific for modulated and composite structures.</pre>',
+               ' that are specific for modulated and composite structures.</pre>\n'
+               '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_modulation_dimension': '<pre><h2>_cell_modulation_dimension</h2> Number of additional '
                                'reciprocal vectors needed to index the\n'
-                               ' whole diffraction pattern using integer Miller indices.</pre>',
+                               ' whole diffraction pattern using integer Miller indices.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 1:8 </p>',
  '_cell_reciprocal_basis_description': '<pre><h2>_cell_reciprocal_basis_description</h2> '
                                        'Definition of the higher-dimensional basis with respect to '
                                        'which\n'
                                        ' the Miller indices are defined. The three-dimensional '
                                        'basis used\n'
                                        ' to index the additional wave vectors should be clearly '
                                        'indicated.\n'
@@ -1381,15 +1473,16 @@
                                        'a*,b*,c*)\n'
                                        'The diffraction pattern can be indexed with four integers '
                                        'based\n'
                                        ' on the reciprocal vectors a*~1~=a*~11~, a*~2~=a*~12~,\n'
                                        ' a*~3~=a*~13~, a*~4~=a*~21~. a*~1j~ (j=1,2,3) index the\n'
                                        ' main reflections of the 1st subsystem. a*~21~ is '
                                        'incommensurate\n'
-                                       ' with a*~11~.</pre>',
+                                       ' with a*~11~.</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>',
  '_cell_subsystem_[ms]': '<pre><h2>_cell_subsystem_[ms]</h2> Data items in the CELL_SUBSYSTEM '
                          'category record details about\n'
                          ' the crystallographic cell parameters of each subsystem present in\n'
                          ' a composite.\n'
                          '\n'
                          '<h3>Example:</h3>\n'
                          '\n'
@@ -1400,29 +1493,32 @@
                          '         _cell_subsystem_matrix_W_1_1\n'
                          '         _cell_subsystem_matrix_W_1_4\n'
                          '         _cell_subsystem_matrix_W_2_2\n'
                          '         _cell_subsystem_matrix_W_3_3\n'
                          '         _cell_subsystem_matrix_W_4_1\n'
                          '         _cell_subsystem_matrix_W_4_4\n'
                          "   NbS2            '1st subsystem'  1 0 1 1 0 1\n"
-                         "   LaS             '2nd subsystem'  0 1 1 1 1 0</pre>",
+                         "   LaS             '2nd subsystem'  0 1 1 1 1 0</pre>\n"
+                         '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_subsystem_code': '<pre><h2>_cell_subsystem_code</h2> The code identifying uniquely a '
                          'certain composite subsystem.\n'
                          ' This code is used to identify the data blocks that contain\n'
                          ' the structural information associated with the subsystem.\n'
                          '\n'
                          '<h3>Example:</h3>\n'
-                         'NbS2</pre>',
+                         'NbS2</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_cell_subsystem_description': '<pre><h2>_cell_subsystem_description</h2> Description of each '
                                 'subsystem defining a composite structurally.\n'
                                 ' The number of definitions must match the number given in\n'
                                 ' _cell_subsystems_number.\n'
                                 '\n'
                                 '<h3>Example:</h3>\n'
-                                'NbS2 part of the layer compound (LaS)~1.14~NbS~2~</pre>',
+                                'NbS2 part of the layer compound (LaS)~1.14~NbS~2~</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_cell_subsystem_matrix_W_10_1': '<pre><h2>_cell_subsystem_matrix_W_10_1</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -1504,15 +1600,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_10': '<pre><h2>_cell_subsystem_matrix_W_10_10</h2> In the case of '
                                    'composites, for each subsystem the matrix W as\n'
                                    ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                    ' Its dimension must match\n'
                                    ' '
                                    '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                    '\n'
@@ -1599,15 +1696,16 @@
                                    'in a\n'
                                    ' multiblock CIF or should be calculated (with the appropriate '
                                    'W\n'
                                    ' matrix) in the case of a single block description of the\n'
                                    ' composite.\n'
                                    '\n'
                                    ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_11': '<pre><h2>_cell_subsystem_matrix_W_10_11</h2> In the case of '
                                    'composites, for each subsystem the matrix W as\n'
                                    ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                    ' Its dimension must match\n'
                                    ' '
                                    '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                    '\n'
@@ -1694,15 +1792,16 @@
                                    'in a\n'
                                    ' multiblock CIF or should be calculated (with the appropriate '
                                    'W\n'
                                    ' matrix) in the case of a single block description of the\n'
                                    ' composite.\n'
                                    '\n'
                                    ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_2': '<pre><h2>_cell_subsystem_matrix_W_10_2</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -1784,15 +1883,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_3': '<pre><h2>_cell_subsystem_matrix_W_10_3</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -1874,15 +1974,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_4': '<pre><h2>_cell_subsystem_matrix_W_10_4</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -1964,15 +2065,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_5': '<pre><h2>_cell_subsystem_matrix_W_10_5</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2054,15 +2156,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_6': '<pre><h2>_cell_subsystem_matrix_W_10_6</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2144,15 +2247,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_7': '<pre><h2>_cell_subsystem_matrix_W_10_7</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2234,15 +2338,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_8': '<pre><h2>_cell_subsystem_matrix_W_10_8</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2324,15 +2429,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_10_9': '<pre><h2>_cell_subsystem_matrix_W_10_9</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2414,15 +2520,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_1': '<pre><h2>_cell_subsystem_matrix_W_11_1</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2504,15 +2611,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_10': '<pre><h2>_cell_subsystem_matrix_W_11_10</h2> In the case of '
                                    'composites, for each subsystem the matrix W as\n'
                                    ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                    ' Its dimension must match\n'
                                    ' '
                                    '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                    '\n'
@@ -2599,15 +2707,16 @@
                                    'in a\n'
                                    ' multiblock CIF or should be calculated (with the appropriate '
                                    'W\n'
                                    ' matrix) in the case of a single block description of the\n'
                                    ' composite.\n'
                                    '\n'
                                    ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_11': '<pre><h2>_cell_subsystem_matrix_W_11_11</h2> In the case of '
                                    'composites, for each subsystem the matrix W as\n'
                                    ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                    ' Its dimension must match\n'
                                    ' '
                                    '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                    '\n'
@@ -2694,15 +2803,16 @@
                                    'in a\n'
                                    ' multiblock CIF or should be calculated (with the appropriate '
                                    'W\n'
                                    ' matrix) in the case of a single block description of the\n'
                                    ' composite.\n'
                                    '\n'
                                    ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                   ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_2': '<pre><h2>_cell_subsystem_matrix_W_11_2</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2784,15 +2894,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_3': '<pre><h2>_cell_subsystem_matrix_W_11_3</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2874,15 +2985,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_4': '<pre><h2>_cell_subsystem_matrix_W_11_4</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -2964,15 +3076,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_5': '<pre><h2>_cell_subsystem_matrix_W_11_5</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3054,15 +3167,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_6': '<pre><h2>_cell_subsystem_matrix_W_11_6</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3144,15 +3258,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_7': '<pre><h2>_cell_subsystem_matrix_W_11_7</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3234,15 +3349,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_8': '<pre><h2>_cell_subsystem_matrix_W_11_8</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3324,15 +3440,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_11_9': '<pre><h2>_cell_subsystem_matrix_W_11_9</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3414,15 +3531,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_1': '<pre><h2>_cell_subsystem_matrix_W_1_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -3497,15 +3615,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_10': '<pre><h2>_cell_subsystem_matrix_W_1_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3587,15 +3706,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_11': '<pre><h2>_cell_subsystem_matrix_W_1_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -3677,15 +3797,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_2': '<pre><h2>_cell_subsystem_matrix_W_1_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -3760,15 +3881,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_3': '<pre><h2>_cell_subsystem_matrix_W_1_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -3843,15 +3965,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_4': '<pre><h2>_cell_subsystem_matrix_W_1_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -3926,15 +4049,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_5': '<pre><h2>_cell_subsystem_matrix_W_1_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4009,15 +4133,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_6': '<pre><h2>_cell_subsystem_matrix_W_1_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4092,15 +4217,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_7': '<pre><h2>_cell_subsystem_matrix_W_1_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4175,15 +4301,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_8': '<pre><h2>_cell_subsystem_matrix_W_1_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4258,15 +4385,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_1_9': '<pre><h2>_cell_subsystem_matrix_W_1_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4341,15 +4469,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_1': '<pre><h2>_cell_subsystem_matrix_W_2_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4424,15 +4553,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_10': '<pre><h2>_cell_subsystem_matrix_W_2_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -4514,15 +4644,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_11': '<pre><h2>_cell_subsystem_matrix_W_2_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -4604,15 +4735,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_2': '<pre><h2>_cell_subsystem_matrix_W_2_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4687,15 +4819,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_3': '<pre><h2>_cell_subsystem_matrix_W_2_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4770,15 +4903,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_4': '<pre><h2>_cell_subsystem_matrix_W_2_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4853,15 +4987,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_5': '<pre><h2>_cell_subsystem_matrix_W_2_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -4936,15 +5071,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_6': '<pre><h2>_cell_subsystem_matrix_W_2_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5019,15 +5155,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_7': '<pre><h2>_cell_subsystem_matrix_W_2_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5102,15 +5239,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_8': '<pre><h2>_cell_subsystem_matrix_W_2_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5185,15 +5323,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_2_9': '<pre><h2>_cell_subsystem_matrix_W_2_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5268,15 +5407,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_1': '<pre><h2>_cell_subsystem_matrix_W_3_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5351,15 +5491,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_10': '<pre><h2>_cell_subsystem_matrix_W_3_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -5441,15 +5582,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_11': '<pre><h2>_cell_subsystem_matrix_W_3_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -5531,15 +5673,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_2': '<pre><h2>_cell_subsystem_matrix_W_3_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5614,15 +5757,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_3': '<pre><h2>_cell_subsystem_matrix_W_3_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5697,15 +5841,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_4': '<pre><h2>_cell_subsystem_matrix_W_3_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5780,15 +5925,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_5': '<pre><h2>_cell_subsystem_matrix_W_3_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5863,15 +6009,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_6': '<pre><h2>_cell_subsystem_matrix_W_3_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -5946,15 +6093,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_7': '<pre><h2>_cell_subsystem_matrix_W_3_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6029,15 +6177,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_8': '<pre><h2>_cell_subsystem_matrix_W_3_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6112,15 +6261,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_3_9': '<pre><h2>_cell_subsystem_matrix_W_3_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6195,15 +6345,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_1': '<pre><h2>_cell_subsystem_matrix_W_4_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6278,15 +6429,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_10': '<pre><h2>_cell_subsystem_matrix_W_4_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -6368,15 +6520,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_11': '<pre><h2>_cell_subsystem_matrix_W_4_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -6458,15 +6611,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_2': '<pre><h2>_cell_subsystem_matrix_W_4_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6541,15 +6695,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_3': '<pre><h2>_cell_subsystem_matrix_W_4_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6624,15 +6779,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_4': '<pre><h2>_cell_subsystem_matrix_W_4_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6707,15 +6863,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_5': '<pre><h2>_cell_subsystem_matrix_W_4_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6790,15 +6947,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_6': '<pre><h2>_cell_subsystem_matrix_W_4_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6873,15 +7031,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_7': '<pre><h2>_cell_subsystem_matrix_W_4_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -6956,15 +7115,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_8': '<pre><h2>_cell_subsystem_matrix_W_4_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7039,15 +7199,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_4_9': '<pre><h2>_cell_subsystem_matrix_W_4_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7122,15 +7283,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_1': '<pre><h2>_cell_subsystem_matrix_W_5_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7205,15 +7367,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_10': '<pre><h2>_cell_subsystem_matrix_W_5_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -7295,15 +7458,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_11': '<pre><h2>_cell_subsystem_matrix_W_5_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -7385,15 +7549,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_2': '<pre><h2>_cell_subsystem_matrix_W_5_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7468,15 +7633,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_3': '<pre><h2>_cell_subsystem_matrix_W_5_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7551,15 +7717,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_4': '<pre><h2>_cell_subsystem_matrix_W_5_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7634,15 +7801,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_5': '<pre><h2>_cell_subsystem_matrix_W_5_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7717,15 +7885,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_6': '<pre><h2>_cell_subsystem_matrix_W_5_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7800,15 +7969,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_7': '<pre><h2>_cell_subsystem_matrix_W_5_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7883,15 +8053,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_8': '<pre><h2>_cell_subsystem_matrix_W_5_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -7966,15 +8137,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_5_9': '<pre><h2>_cell_subsystem_matrix_W_5_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8049,15 +8221,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_1': '<pre><h2>_cell_subsystem_matrix_W_6_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8132,15 +8305,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_10': '<pre><h2>_cell_subsystem_matrix_W_6_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -8222,15 +8396,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_11': '<pre><h2>_cell_subsystem_matrix_W_6_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -8312,15 +8487,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_2': '<pre><h2>_cell_subsystem_matrix_W_6_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8395,15 +8571,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_3': '<pre><h2>_cell_subsystem_matrix_W_6_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8478,15 +8655,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_4': '<pre><h2>_cell_subsystem_matrix_W_6_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8561,15 +8739,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_5': '<pre><h2>_cell_subsystem_matrix_W_6_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8644,15 +8823,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_6': '<pre><h2>_cell_subsystem_matrix_W_6_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8727,15 +8907,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_7': '<pre><h2>_cell_subsystem_matrix_W_6_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8810,15 +8991,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_8': '<pre><h2>_cell_subsystem_matrix_W_6_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8893,15 +9075,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_6_9': '<pre><h2>_cell_subsystem_matrix_W_6_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -8976,15 +9159,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_1': '<pre><h2>_cell_subsystem_matrix_W_7_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9059,15 +9243,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_10': '<pre><h2>_cell_subsystem_matrix_W_7_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -9149,15 +9334,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_11': '<pre><h2>_cell_subsystem_matrix_W_7_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -9239,15 +9425,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_2': '<pre><h2>_cell_subsystem_matrix_W_7_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9322,15 +9509,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_3': '<pre><h2>_cell_subsystem_matrix_W_7_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9405,15 +9593,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_4': '<pre><h2>_cell_subsystem_matrix_W_7_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9488,15 +9677,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_5': '<pre><h2>_cell_subsystem_matrix_W_7_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9571,15 +9761,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_6': '<pre><h2>_cell_subsystem_matrix_W_7_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9654,15 +9845,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_7': '<pre><h2>_cell_subsystem_matrix_W_7_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9737,15 +9929,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_8': '<pre><h2>_cell_subsystem_matrix_W_7_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9820,15 +10013,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_7_9': '<pre><h2>_cell_subsystem_matrix_W_7_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9903,15 +10097,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_1': '<pre><h2>_cell_subsystem_matrix_W_8_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -9986,15 +10181,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_10': '<pre><h2>_cell_subsystem_matrix_W_8_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -10076,15 +10272,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_11': '<pre><h2>_cell_subsystem_matrix_W_8_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -10166,15 +10363,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_2': '<pre><h2>_cell_subsystem_matrix_W_8_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10249,15 +10447,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_3': '<pre><h2>_cell_subsystem_matrix_W_8_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10332,15 +10531,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_4': '<pre><h2>_cell_subsystem_matrix_W_8_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10415,15 +10615,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_5': '<pre><h2>_cell_subsystem_matrix_W_8_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10498,15 +10699,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_6': '<pre><h2>_cell_subsystem_matrix_W_8_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10581,15 +10783,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_7': '<pre><h2>_cell_subsystem_matrix_W_8_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10664,15 +10867,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_8': '<pre><h2>_cell_subsystem_matrix_W_8_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10747,15 +10951,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_8_9': '<pre><h2>_cell_subsystem_matrix_W_8_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10830,15 +11035,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_1': '<pre><h2>_cell_subsystem_matrix_W_9_1</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -10913,15 +11119,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_10': '<pre><h2>_cell_subsystem_matrix_W_9_10</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -11003,15 +11210,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_11': '<pre><h2>_cell_subsystem_matrix_W_9_11</h2> In the case of '
                                   'composites, for each subsystem the matrix W as\n'
                                   ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                   ' Its dimension must match\n'
                                   ' '
                                   '(_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                   '\n'
@@ -11093,15 +11301,16 @@
                                   'a\n'
                                   ' multiblock CIF or should be calculated (with the appropriate '
                                   'W\n'
                                   ' matrix) in the case of a single block description of the\n'
                                   ' composite.\n'
                                   '\n'
                                   ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                  ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_2': '<pre><h2>_cell_subsystem_matrix_W_9_2</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11176,15 +11385,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_3': '<pre><h2>_cell_subsystem_matrix_W_9_3</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11259,15 +11469,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_4': '<pre><h2>_cell_subsystem_matrix_W_9_4</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11342,15 +11553,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_5': '<pre><h2>_cell_subsystem_matrix_W_9_5</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11425,15 +11637,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_6': '<pre><h2>_cell_subsystem_matrix_W_9_6</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11508,15 +11721,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_7': '<pre><h2>_cell_subsystem_matrix_W_9_7</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11591,15 +11805,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_8': '<pre><h2>_cell_subsystem_matrix_W_9_8</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11674,15 +11889,16 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystem_matrix_W_9_9': '<pre><h2>_cell_subsystem_matrix_W_9_9</h2> In the case of '
                                  'composites, for each subsystem the matrix W as\n'
                                  ' defined in van Smaalen (1991); see also van Smaalen (1995).\n'
                                  ' Its dimension must match\n'
                                  ' (_cell_modulation_dimension+3)*(_cell_modulation_dimension+3).\n'
                                  '\n'
                                  ' Intergrowth compounds are composed of several periodic\n'
@@ -11757,44 +11973,50 @@
                                  ' particular subsystem. Such a basis will be explicitly given in '
                                  'a\n'
                                  ' multiblock CIF or should be calculated (with the appropriate W\n'
                                  ' matrix) in the case of a single block description of the\n'
                                  ' composite.\n'
                                  '\n'
                                  ' Ref: Smaalen, S. van (1991). Phys. Rev. B, 43, 11330-11341.\n'
-                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>',
+                                 ' Smaalen, S. van (1995). Crystallogr. Rev. 4, 79-202.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_subsystems_[ms]': '<pre><h2>_cell_subsystems_[ms]</h2> Data items in the CELL_SUBSYSTEMS '
                           'category describe the gross\n'
                           ' structure of the subsystems present in a composite.\n'
                           '\n'
                           '<h3>Example:</h3>\n'
                           '\n'
-                          '     _cell_subsystems_number                  2</pre>',
+                          '     _cell_subsystems_number                  2</pre>\n'
+                          '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_subsystems_number': '<pre><h2>_cell_subsystems_number</h2> The number of subsystems used '
                             'to define the structural model of\n'
-                            ' a composite structure.</pre>',
+                            ' a composite structure.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 2:∞ </p>',
  '_cell_wave_vector_[ms]': '<pre><h2>_cell_wave_vector_[ms]</h2> Data items in the '
                            'CELL_WAVE_VECTOR category list the\n'
                            ' independent modulation wave vectors q~i~. The diffraction\n'
                            ' vectors are indexed in the form\n'
                            ' ha*+kb*+lc*+sum~i~ (m~i~q~i~). sum~i~ is taken\n'
                            ' over all wave vectors. In this version of the dictionary, the\n'
                            ' index i has been restricted to be less than 9.\n'
                            '\n'
                            '<h3>Example:</h3>\n'
                            '\n'
                            '     loop_\n'
                            '         _cell_wave_vector_seq_id\n'
                            '         _cell_wave_vector_x\n'
-                           '  1       0.318(5)</pre>',
+                           '  1       0.318(5)</pre>\n'
+                           '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_wave_vector_seq_id': '<pre><h2>_cell_wave_vector_seq_id</h2> A numeric code to identify '
                              'each independent wave vector. These\n'
                              ' codes define uniquely the reciprocal basis and, therefore,\n'
                              ' force the order of the Miller indices assigned to\n'
-                             ' intensities, crystal faces etc.</pre>',
+                             ' intensities, crystal faces etc.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_wave_vector_x': '<pre><h2>_cell_wave_vector_x</h2> Independent modulation wave vector(s) '
                         'with which the whole\n'
                         ' diffraction pattern is indexed, expressed as fractions of the\n'
                         ' three reciprocal basis vectors of the reference structure. In\n'
                         ' the case of composites, the modulation wave vectors of each\n'
                         ' subsystem are expressed in terms of the reciprocal basis of its\n'
                         ' corresponding reference structure. Their number must match\n'
@@ -11804,15 +12026,16 @@
                         ' reference in _cell_reciprocal_basis_description, which would\n'
                         ' correspond to the subsystem (if any) whose W matrix is the\n'
                         ' {(_cell_modulation_dimension + 3)*\n'
                         ' (_cell_modulation_dimension + 3)} unit matrix. In this case,\n'
                         ' the wave vectors used to describe the modulation of each\n'
                         ' subsystem are referred to their own reciprocal basis via the W\n'
                         ' matrices (for details see _cell_subsystem_matrix_W_ and\n'
-                        ' _atom_site_Fourier_wave_vector_).</pre>',
+                        ' _atom_site_Fourier_wave_vector_).</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_wave_vector_y': '<pre><h2>_cell_wave_vector_y</h2> Independent modulation wave vector(s) '
                         'with which the whole\n'
                         ' diffraction pattern is indexed, expressed as fractions of the\n'
                         ' three reciprocal basis vectors of the reference structure. In\n'
                         ' the case of composites, the modulation wave vectors of each\n'
                         ' subsystem are expressed in terms of the reciprocal basis of its\n'
                         ' corresponding reference structure. Their number must match\n'
@@ -11822,15 +12045,16 @@
                         ' reference in _cell_reciprocal_basis_description, which would\n'
                         ' correspond to the subsystem (if any) whose W matrix is the\n'
                         ' {(_cell_modulation_dimension + 3)*\n'
                         ' (_cell_modulation_dimension + 3)} unit matrix. In this case,\n'
                         ' the wave vectors used to describe the modulation of each\n'
                         ' subsystem are referred to their own reciprocal basis via the W\n'
                         ' matrices (for details see _cell_subsystem_matrix_W_ and\n'
-                        ' _atom_site_Fourier_wave_vector_).</pre>',
+                        ' _atom_site_Fourier_wave_vector_).</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_wave_vector_z': '<pre><h2>_cell_wave_vector_z</h2> Independent modulation wave vector(s) '
                         'with which the whole\n'
                         ' diffraction pattern is indexed, expressed as fractions of the\n'
                         ' three reciprocal basis vectors of the reference structure. In\n'
                         ' the case of composites, the modulation wave vectors of each\n'
                         ' subsystem are expressed in terms of the reciprocal basis of its\n'
                         ' corresponding reference structure. Their number must match\n'
@@ -11840,518 +12064,576 @@
                         ' reference in _cell_reciprocal_basis_description, which would\n'
                         ' correspond to the subsystem (if any) whose W matrix is the\n'
                         ' {(_cell_modulation_dimension + 3)*\n'
                         ' (_cell_modulation_dimension + 3)} unit matrix. In this case,\n'
                         ' the wave vectors used to describe the modulation of each\n'
                         ' subsystem are referred to their own reciprocal basis via the W\n'
                         ' matrices (for details see _cell_subsystem_matrix_W_ and\n'
-                        ' _atom_site_Fourier_wave_vector_).</pre>',
+                        ' _atom_site_Fourier_wave_vector_).</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_cell_wave_vectors_[ms]': '<pre><h2>_cell_wave_vectors_[ms]</h2> Data items in the '
                             'CELL_WAVE_VECTORS category record details\n'
                             ' about the set of independent modulation wave vectors q~i~ and\n'
                             ' their measurement. The diffraction vectors are indexed in\n'
                             ' the form ha*+kb*+lc*+sum~i~ (m~i~q~i~). sum~i~ is taken\n'
                             ' over all wave vectors. In this version of the dictionary, the\n'
                             ' index i has been restricted to be less than 9.\n'
                             '\n'
                             '<h3>Example:</h3>\n'
                             '\n'
                             "     _cell_wave_vectors_meas_details          'Determined from "
-                            "profiles along q'</pre>",
+                            "profiles along q'</pre>\n"
+                            '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_cell_wave_vectors_meas_details': '<pre><h2>_cell_wave_vectors_meas_details</h2> Details about '
                                     'the method used to determine the independent\n'
-                                    ' modulation wave vector(s).</pre>',
+                                    ' modulation wave vector(s).</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_cell_wave_vectors_pressure_max': '<pre><h2>_cell_wave_vectors_pressure_max</h2> The maximum and '
                                     'minimum values of the pressure in kilopascals\n'
                                     ' defining the interval within which the modulation wave '
                                     'vector(s)\n'
-                                    ' were measured.</pre>',
+                                    ' were measured.</pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                    '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_cell_wave_vectors_pressure_min': '<pre><h2>_cell_wave_vectors_pressure_min</h2> The maximum and '
                                     'minimum values of the pressure in kilopascals\n'
                                     ' defining the interval within which the modulation wave '
                                     'vector(s)\n'
-                                    ' were measured.</pre>',
+                                    ' were measured.</pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                    '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_cell_wave_vectors_temp_max': '<pre><h2>_cell_wave_vectors_temp_max</h2> The maximum and minimum '
                                 'values of the temperature in kelvins\n'
                                 ' defining the interval within which the modulation wave '
                                 'vector(s)\n'
-                                ' were measured.</pre>',
+                                ' were measured.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_cell_wave_vectors_temp_min': '<pre><h2>_cell_wave_vectors_temp_min</h2> The maximum and minimum '
                                 'values of the temperature in kelvins\n'
                                 ' defining the interval within which the modulation wave '
                                 'vector(s)\n'
-                                ' were measured.</pre>',
+                                ' were measured.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_cell_wave_vectors_variation': '<pre><h2>_cell_wave_vectors_variation</h2> Details concerning '
                                  'the behaviour (and its experimental\n'
                                  ' detection) of the wave vector(s) with temperature and/or\n'
                                  ' pressure within the ranges specified by\n'
                                  ' _cell_wave_vectors_pressure_max, '
                                  '_cell_wave_vectors_pressure_min,\n'
                                  ' _cell_wave_vectors_temp_max and '
-                                 '_cell_wave_vectors_temp_min.</pre>',
+                                 '_cell_wave_vectors_temp_min.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_diffrn_refln_[ms]': '<pre><h2>_diffrn_refln_[ms]</h2> Data items in the DIFFRN_REFLN category '
                        'record details about\n'
                        ' the intensities measured in the diffraction experiment. The\n'
                        ' DIFFRN_REFLN data items refer to individual intensity\n'
                        ' measurements and must be included in looped lists. (The\n'
                        ' DIFFRN_REFLNS data items specify the parameters that apply\n'
                        ' to all intensity measurements. The DIFFRN_REFLNS data items\n'
                        ' are not looped.) Data items in this category are extensions\n'
                        ' of the core CIF dictionary definitions to the indexing of\n'
-                       ' diffraction intensities by higher-dimensional components.</pre>',
+                       ' diffraction intensities by higher-dimensional components.</pre>\n'
+                       '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_diffrn_refln_index_m_1': '<pre><h2>_diffrn_refln_index_m_1</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_2': '<pre><h2>_diffrn_refln_index_m_2</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_3': '<pre><h2>_diffrn_refln_index_m_3</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_4': '<pre><h2>_diffrn_refln_index_m_4</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_5': '<pre><h2>_diffrn_refln_index_m_5</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_6': '<pre><h2>_diffrn_refln_index_m_6</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_7': '<pre><h2>_diffrn_refln_index_m_7</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_refln_index_m_8': '<pre><h2>_diffrn_refln_index_m_8</h2> Additional Miller indices '
                             'needed to write the reciprocal vector\n'
                             ' of a certain reflection in the basis described in\n'
                             ' _cell_reciprocal_basis_description. Following the usual\n'
                             ' convention, such a vector would be expressed as\n'
                             '          H=h*a*+k*b*+l*c*+m1*q(1)+...+m8*q(8),\n'
                             ' where h,k,l are the usual _diffrn_refln_index_, and q(1)...q(8)\n'
                             ' represent the independent wave vectors given by\n'
                             ' _cell_wave_vector_ and identified by _cell_wave_vector_seq_id.\n'
                             ' Therefore, the total number of indices of a given reflection must\n'
                             ' match (_cell_modulation_dimension + 3) and the order of the\n'
                             ' additional indices must be consistent with the codes given in\n'
                             ' _cell_wave_vector_seq_id. These indices need not match\n'
                             ' _refln_index_m_ values if a transformation of the original\n'
-                            ' measured cell has occurred.</pre>',
+                            ' measured cell has occurred.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_[ms]': '<pre><h2>_diffrn_reflns_[ms]</h2> Data items in the DIFFRN_REFLNS '
                         'category record details about\n'
                         ' the set of intensities measured in the diffraction experiment.\n'
                         ' The DIFFRN_REFLNS data items specify the parameters that apply to\n'
                         ' all intensity measurements. The DIFFRN_REFLNS data items are\n'
                         ' not looped. (The DIFFRN_REFLN data items refer to individual\n'
                         ' intensity measurements and must be included in looped lists.)\n'
                         ' Data items in this category extend the core CIF dictionary\n'
                         ' definitions providing independent checks on the range of values\n'
                         ' recorded for each of the additional Miller indices given in\n'
-                        ' the DIFFRN_REFLN category.</pre>',
+                        ' the DIFFRN_REFLN category.</pre>\n'
+                        '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_diffrn_reflns_limit_index_m_1_max': '<pre><h2>_diffrn_reflns_limit_index_m_1_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_1_min': '<pre><h2>_diffrn_reflns_limit_index_m_1_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_2_max': '<pre><h2>_diffrn_reflns_limit_index_m_2_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_2_min': '<pre><h2>_diffrn_reflns_limit_index_m_2_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_3_max': '<pre><h2>_diffrn_reflns_limit_index_m_3_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_3_min': '<pre><h2>_diffrn_reflns_limit_index_m_3_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_4_max': '<pre><h2>_diffrn_reflns_limit_index_m_4_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_4_min': '<pre><h2>_diffrn_reflns_limit_index_m_4_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_5_max': '<pre><h2>_diffrn_reflns_limit_index_m_5_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_5_min': '<pre><h2>_diffrn_reflns_limit_index_m_5_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_6_max': '<pre><h2>_diffrn_reflns_limit_index_m_6_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_6_min': '<pre><h2>_diffrn_reflns_limit_index_m_6_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_7_max': '<pre><h2>_diffrn_reflns_limit_index_m_7_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_7_min': '<pre><h2>_diffrn_reflns_limit_index_m_7_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_8_max': '<pre><h2>_diffrn_reflns_limit_index_m_8_max</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_limit_index_m_8_min': '<pre><h2>_diffrn_reflns_limit_index_m_8_min</h2> Maximum '
                                        'and minimum values of the additional Miller indices\n'
                                        ' appearing in _diffrn_refln_index_m_. The number of ranges '
                                        'must\n'
                                        ' match _cell_modulation_dimension. The order of the '
                                        'additional\n'
                                        ' indices must be consistent with the codes given in\n'
-                                       ' _cell_wave_vector_seq_id.</pre>',
+                                       ' _cell_wave_vector_seq_id.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_reflns_satellite_order_max': '<pre><h2>_diffrn_reflns_satellite_order_max</h2> Maximum '
-                                       'order of observed satellites.</pre>',
+                                       'order of observed satellites.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_[ms]': '<pre><h2>_diffrn_standard_refln_[ms]</h2> Data items in the '
                                 'DIFFRN_STANDARD_REFLN category record\n'
                                 ' details about the reflections treated as standards during the\n'
                                 ' measurement of diffraction intensities. Note that these are the\n'
                                 ' individual standard reflections, not the results of the '
                                 'analysis\n'
                                 ' of the standard reflections. Data items in this category are\n'
                                 ' extensions of  the core CIF dictionary definitions\n'
                                 ' to the indexing of standard reflections by\n'
-                                ' higher-dimensional components.</pre>',
+                                ' higher-dimensional components.</pre>\n'
+                                '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_diffrn_standard_refln_index_m_1': '<pre><h2>_diffrn_standard_refln_index_m_1</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_2': '<pre><h2>_diffrn_standard_refln_index_m_2</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_3': '<pre><h2>_diffrn_standard_refln_index_m_3</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_4': '<pre><h2>_diffrn_standard_refln_index_m_4</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_5': '<pre><h2>_diffrn_standard_refln_index_m_5</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_6': '<pre><h2>_diffrn_standard_refln_index_m_6</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_7': '<pre><h2>_diffrn_standard_refln_index_m_7</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_diffrn_standard_refln_index_m_8': '<pre><h2>_diffrn_standard_refln_index_m_8</h2> Additional '
                                      'Miller indices needed to write the reciprocal vectors\n'
                                      ' of the standard intensities used in the diffraction '
                                      'measurement\n'
                                      ' process, in the basis described in\n'
                                      ' _cell_reciprocal_basis_description. The total number of '
                                      'indices\n'
                                      ' of a given standard reflection must match\n'
                                      ' (_cell_modulation_dimension + 3) and the order of the\n'
                                      ' additional indices must be consistent with the codes given '
                                      'in\n'
-                                     ' _cell_wave_vector_seq_id.</pre>',
+                                     ' _cell_wave_vector_seq_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_[ms]': '<pre><h2>_exptl_crystal_[ms]</h2> Data items in the EXPTL_CRYSTAL '
                         'category record\n'
                         ' details about experimental measurements on the crystal or\n'
                         ' crystals used, such as shape, size and density. The new\n'
                         ' data item added to this category specifies whether the structure\n'
-                        ' is crystalline, modulated or composite.</pre>',
+                        ' is crystalline, modulated or composite.</pre>\n'
+                        '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_exptl_crystal_face_[ms]': '<pre><h2>_exptl_crystal_face_[ms]</h2> Data items in the '
                              'EXPTL_CRYSTAL_FACE category record\n'
                              ' details of the crystal faces. Data items in this category are\n'
                              ' extensions of the core CIF dictionary definitions to the\n'
-                             ' indexing of crystal faces by higher-dimensional components.</pre>',
+                             ' indexing of crystal faces by higher-dimensional components.</pre>\n'
+                             '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_exptl_crystal_face_index_m_1': '<pre><h2>_exptl_crystal_face_index_m_1</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_2': '<pre><h2>_exptl_crystal_face_index_m_2</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_3': '<pre><h2>_exptl_crystal_face_index_m_3</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_4': '<pre><h2>_exptl_crystal_face_index_m_4</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_5': '<pre><h2>_exptl_crystal_face_index_m_5</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_6': '<pre><h2>_exptl_crystal_face_index_m_6</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_7': '<pre><h2>_exptl_crystal_face_index_m_7</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_face_index_m_8': '<pre><h2>_exptl_crystal_face_index_m_8</h2> Additional Miller '
                                   'indices of the crystal face associated with the\n'
                                   ' value _exptl_crystal_face_perp_dist when the face is indexed\n'
                                   ' using a multidimensional scheme. The total number of indices '
                                   'must\n'
                                   ' match (_cell_modulation_dimension + 3). The order of the '
                                   'indices\n'
                                   ' must be consistent with the codes given in\n'
-                                  ' _cell_wave_vector_seq_id.</pre>',
+                                  ' _cell_wave_vector_seq_id.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_exptl_crystal_type_of_structure': '<pre><h2>_exptl_crystal_type_of_structure</h2>       The '
                                      'type of structure. This is used to check the consistency of '
                                      'a\n'
                                      '        CIF: the data blocks that are expected and/or '
                                      'certain characteristic\n'
                                      '        parameters depend on whether the material is '
                                      'classified as crystalline\n'
@@ -12363,34 +12645,40 @@
                                      '\tcrystalline structure\n'
                                      '\n'
                                      'mod\n'
                                      '\tmodulated structure\n'
                                      '\n'
                                      'comp\n'
                                      '\tcomposite (misfit) structure\n'
-                                     '</pre>',
+                                     '</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>\n'
+                                     '<br><p><h4>Default:</h4> cryst </p>',
  '_geom_angle_[ms]': '<pre><h2>_geom_angle_[ms]</h2> Data items in the GEOM_ANGLE category record\n'
                      ' details about the bond angles, as calculated from the\n'
                      ' ATOM, CELL and SYMMETRY data. These extensions\n'
                      ' to the core CIF dictionary definitions record the maximum,\n'
                      ' minimum and average values of angles and extend the\n'
                      ' symmetry-operation code used in angle listings to the\n'
-                     ' higher-dimensional superspace form.</pre>',
+                     ' higher-dimensional superspace form.</pre>\n'
+                     '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_geom_angle_av': '<pre><h2>_geom_angle_av</h2> Maximum, minimum and average angles in degrees '
                    'bounded by\n'
                    ' _geom_angle_atom_site_label_1, *_2, and *_3. The site at *_2\n'
-                   ' is at the apex of the angle.</pre>',
+                   ' is at the apex of the angle.</pre>\n'
+                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_angle_max': '<pre><h2>_geom_angle_max</h2> Maximum, minimum and average angles in degrees '
                     'bounded by\n'
                     ' _geom_angle_atom_site_label_1, *_2, and *_3. The site at *_2\n'
-                    ' is at the apex of the angle.</pre>',
+                    ' is at the apex of the angle.</pre>\n'
+                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_angle_min': '<pre><h2>_geom_angle_min</h2> Maximum, minimum and average angles in degrees '
                     'bounded by\n'
                     ' _geom_angle_atom_site_label_1, *_2, and *_3. The site at *_2\n'
-                    ' is at the apex of the angle.</pre>',
+                    ' is at the apex of the angle.</pre>\n'
+                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_angle_site_ssg_symmetry_1': '<pre><h2>_geom_angle_site_ssg_symmetry_1</h2> The symmetry '
                                     'code of each atom site as the symmetry operation\n'
                                     " number 'n' and the higher-dimensional translation "
                                     "'m1...mp'.\n"
                                     " These numbers are combined to form the code 'n m1...mp' or\n"
                                     ' n_m1...mp. The character string n_m1...mp is composed as '
                                     'follows:\n'
@@ -12412,15 +12700,16 @@
                                     ' symmetry operations or translations are applicable, then a '
                                     'single\n'
                                     " full stop '.' is used.\n"
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_6455</pre>',
+                                    '7_6455</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_geom_angle_site_ssg_symmetry_2': '<pre><h2>_geom_angle_site_ssg_symmetry_2</h2> The symmetry '
                                     'code of each atom site as the symmetry operation\n'
                                     " number 'n' and the higher-dimensional translation "
                                     "'m1...mp'.\n"
                                     " These numbers are combined to form the code 'n m1...mp' or\n"
                                     ' n_m1...mp. The character string n_m1...mp is composed as '
                                     'follows:\n'
@@ -12442,15 +12731,16 @@
                                     ' symmetry operations or translations are applicable, then a '
                                     'single\n'
                                     " full stop '.' is used.\n"
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_6455</pre>',
+                                    '7_6455</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_geom_angle_site_ssg_symmetry_3': '<pre><h2>_geom_angle_site_ssg_symmetry_3</h2> The symmetry '
                                     'code of each atom site as the symmetry operation\n'
                                     " number 'n' and the higher-dimensional translation "
                                     "'m1...mp'.\n"
                                     " These numbers are combined to form the code 'n m1...mp' or\n"
                                     ' n_m1...mp. The character string n_m1...mp is composed as '
                                     'follows:\n'
@@ -12472,31 +12762,39 @@
                                     ' symmetry operations or translations are applicable, then a '
                                     'single\n'
                                     " full stop '.' is used.\n"
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_6455</pre>',
+                                    '7_6455</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_geom_bond_[ms]': '<pre><h2>_geom_bond_[ms]</h2> Data items in the GEOM_BOND category record\n'
                     ' details about bonds, as calculated from the\n'
                     ' ATOM, CELL and SYMMETRY data. These extensions\n'
                     ' to the core CIF dictionary definitions record the maximum,\n'
                     ' minimum and average lengths of bonds and extend the\n'
                     ' symmetry-operation code used in bond listings to the\n'
-                    ' higher-dimensional superspace form.</pre>',
+                    ' higher-dimensional superspace form.</pre>\n'
+                    '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_geom_bond_distance_av': '<pre><h2>_geom_bond_distance_av</h2> Maximum, minimum and average '
                            'values of the intramolecular bond\n'
-                           ' distance in angstroms.</pre>',
+                           ' distance in angstroms.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_bond_distance_max': '<pre><h2>_geom_bond_distance_max</h2> Maximum, minimum and average '
                             'values of the intramolecular bond\n'
-                            ' distance in angstroms.</pre>',
+                            ' distance in angstroms.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_bond_distance_min': '<pre><h2>_geom_bond_distance_min</h2> Maximum, minimum and average '
                             'values of the intramolecular bond\n'
-                            ' distance in angstroms.</pre>',
+                            ' distance in angstroms.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_bond_site_ssg_symmetry_1': '<pre><h2>_geom_bond_site_ssg_symmetry_1</h2> The symmetry code '
                                    'of each atom site as the symmetry operation\n'
                                    " number 'n' and the higher-dimensional translation 'm1...mp'.\n"
                                    " These numbers are combined to form the code 'n m1...mp' or\n"
                                    ' n_m1...mp. The character string n_m1...mp is composed as '
                                    'follows:\n'
                                    " 'n' refers to the symmetry operation that is applied to the\n"
@@ -12517,15 +12815,16 @@
                                    ' symmetry operations or translations are applicable then a '
                                    'single\n'
                                    " full stop '.' is used.\n"
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_6455</pre>',
+                                   '7_6455</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_geom_bond_site_ssg_symmetry_2': '<pre><h2>_geom_bond_site_ssg_symmetry_2</h2> The symmetry code '
                                    'of each atom site as the symmetry operation\n'
                                    " number 'n' and the higher-dimensional translation 'm1...mp'.\n"
                                    " These numbers are combined to form the code 'n m1...mp' or\n"
                                    ' n_m1...mp. The character string n_m1...mp is composed as '
                                    'follows:\n'
                                    " 'n' refers to the symmetry operation that is applied to the\n"
@@ -12546,32 +12845,40 @@
                                    ' symmetry operations or translations are applicable then a '
                                    'single\n'
                                    " full stop '.' is used.\n"
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_6455</pre>',
+                                   '7_6455</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_geom_contact_[ms]': '<pre><h2>_geom_contact_[ms]</h2> Data items in the GEOM_CONTACT category '
                        'record\n'
                        ' details about interatomic contacts, as calculated from the\n'
                        ' ATOM, CELL and SYMMETRY data. These extensions\n'
                        ' to the core CIF dictionary definitions record the maximum,\n'
                        ' minimum and average values of contact distances and extend the\n'
                        ' symmetry-operation code used in contact-distance listings to the\n'
-                       ' higher-dimensional superspace form.</pre>',
+                       ' higher-dimensional superspace form.</pre>\n'
+                       '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_geom_contact_distance_av': '<pre><h2>_geom_contact_distance_av</h2> Maximum, minimum and '
                               'average values of the interatomic contact\n'
-                              ' distance in angstroms.</pre>',
+                              ' distance in angstroms.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_contact_distance_max': '<pre><h2>_geom_contact_distance_max</h2> Maximum, minimum and '
                                'average values of the interatomic contact\n'
-                               ' distance in angstroms.</pre>',
+                               ' distance in angstroms.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_contact_distance_min': '<pre><h2>_geom_contact_distance_min</h2> Maximum, minimum and '
                                'average values of the interatomic contact\n'
-                               ' distance in angstroms.</pre>',
+                               ' distance in angstroms.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_geom_contact_site_ssg_symmetry_1': '<pre><h2>_geom_contact_site_ssg_symmetry_1</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12597,15 +12904,16 @@
                                       ' symmetry operations or translations are applicable, then a '
                                       'single\n'
                                       " full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_geom_contact_site_ssg_symmetry_2': '<pre><h2>_geom_contact_site_ssg_symmetry_2</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12631,47 +12939,52 @@
                                       ' symmetry operations or translations are applicable, then a '
                                       'single\n'
                                       " full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_geom_torsion_[ms]': '<pre><h2>_geom_torsion_[ms]</h2> Data items in the GEOM_TORSION category '
                        'record\n'
                        ' details about torsion angles, as calculated from the\n'
                        ' ATOM, CELL and SYMMETRY data. These extensions\n'
                        ' to the core CIF dictionary definitions record the maximum,\n'
                        ' minimum and average values of torsion angles and extend the\n'
                        ' symmetry-operation code used in torsion-angle listings to the\n'
-                       ' higher-dimensional superspace form.</pre>',
+                       ' higher-dimensional superspace form.</pre>\n'
+                       '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_geom_torsion_av': '<pre><h2>_geom_torsion_av</h2> Maximum, minimum and average torsion angles '
                      'in degrees bounded\n'
                      ' by the four atom sites identified by the\n'
                      ' _geom_torsion_atom_site_label_ codes. These must match labels\n'
                      ' specified as _atom_site_label in the atom list. The torsion-\n'
                      ' angle definition should be that of Klyne and Prelog (1960).\n'
                      '\n'
-                     ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>',
+                     ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_torsion_max': '<pre><h2>_geom_torsion_max</h2> Maximum, minimum and average torsion angles '
                       'in degrees bounded\n'
                       ' by the four atom sites identified by the\n'
                       ' _geom_torsion_atom_site_label_ codes. These must match labels\n'
                       ' specified as _atom_site_label in the atom list. The torsion-\n'
                       ' angle definition should be that of Klyne and Prelog (1960).\n'
                       '\n'
-                      ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>',
+                      ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>\n'
+                      '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_torsion_min': '<pre><h2>_geom_torsion_min</h2> Maximum, minimum and average torsion angles '
                       'in degrees bounded\n'
                       ' by the four atom sites identified by the\n'
                       ' _geom_torsion_atom_site_label_ codes. These must match labels\n'
                       ' specified as _atom_site_label in the atom list. The torsion-\n'
                       ' angle definition should be that of Klyne and Prelog (1960).\n'
                       '\n'
-                      ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>',
+                      ' Ref: Klyne, W. &amp; Prelog, V. (1960). Experientia, 16, 521-523.</pre>\n'
+                      '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_geom_torsion_site_ssg_symmetry_1': '<pre><h2>_geom_torsion_site_ssg_symmetry_1</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12695,15 +13008,16 @@
                                       'omitted.\n'
                                       ' If no symmetry operations or translations are applicable,\n'
                                       " then a single full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_geom_torsion_site_ssg_symmetry_2': '<pre><h2>_geom_torsion_site_ssg_symmetry_2</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12727,15 +13041,16 @@
                                       'omitted.\n'
                                       ' If no symmetry operations or translations are applicable,\n'
                                       " then a single full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_geom_torsion_site_ssg_symmetry_3': '<pre><h2>_geom_torsion_site_ssg_symmetry_3</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12759,15 +13074,16 @@
                                       'omitted.\n'
                                       ' If no symmetry operations or translations are applicable,\n'
                                       " then a single full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_geom_torsion_site_ssg_symmetry_4': '<pre><h2>_geom_torsion_site_ssg_symmetry_4</h2> The '
                                       'symmetry code of each atom site as the symmetry operation\n'
                                       " number 'n' and the higher-dimensional translation "
                                       "'m1...mp'.\n"
                                       " These numbers are combined to form the code 'n m1...mp' "
                                       'or\n'
                                       ' n_m1...mp. The character string n_m1...mp is composed as '
@@ -12791,28 +13107,31 @@
                                       'omitted.\n'
                                       ' If no symmetry operations or translations are applicable,\n'
                                       " then a single full stop '.' is used.\n"
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'None\n'
                                       '4\n'
-                                      '7_6455</pre>',
+                                      '7_6455</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_refine_[ms]': '<pre><h2>_refine_[ms]</h2> Data items in the REFINE category record\n'
                  ' details about the structure refinement parameters. The\n'
                  ' new items in this category extend those of the core CIF\n'
                  ' dictionary and are specific to the refinement of\n'
-                 ' modulated structures.</pre>',
+                 ' modulated structures.</pre>\n'
+                 '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_refine_ls_mod_func_description': '<pre><h2>_refine_ls_mod_func_description</h2> Types of '
                                     'modulation present in the structural model and their\n'
                                     ' parameterization.\n'
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'Only displacive modulation. Fourier series.\n'
                                     'Modulation of atom S(1) described by a non-standard\n'
-                                    ' linear sawtooth function</pre>',
+                                    ' linear sawtooth function</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_refine_ls_mod_hydrogen_treatment': '<pre><h2>_refine_ls_mod_hydrogen_treatment</h2> Treatment '
                                       'of hydrogen-atom modulation parameters in the\n'
                                       ' refinement.\n'
                                       '\n'
                                       '<h3>Example:</h3>\n'
                                       'refA\n'
                                       '\trefined H-atom displacive modulation parameters only\n'
@@ -12826,231 +13145,266 @@
                                       '\n'
                                       'refUP\n'
                                       '\trefined H-atom U and occupational modulation parameters '
                                       'only\n'
                                       '\n'
                                       'nomod\n'
                                       '\tno modulation of H-atom parameters\n'
-                                      '</pre>',
+                                      '</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>\n'
+                                      '<br><p><h4>Default:</h4> nomod </p>',
  '_refine_ls_mod_overall_phason_coeff': '<pre><h2>_refine_ls_mod_overall_phason_coeff</h2> The '
                                         'phason coefficient used to calculate the overall phason\n'
-                                        ' correction.</pre>',
+                                        ' correction.</pre>\n'
+                                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                        '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_refine_ls_mod_overall_phason_formula': '<pre><h2>_refine_ls_mod_overall_phason_formula</h2> The '
                                           'expression for the overall phason correction, if used.\n'
                                           '\n'
                                           '<h3>Example:</h3>\n'
                                           'Axe\n'
                                           '\tAxe, J. D. (1980). Phys. Rev. B, 21, 4181-4190.\n'
                                           '\n'
                                           'Ovr\n'
                                           '\tOverhauser, A. W. (1971). Phys. Rev. B, 3, '
                                           '3173-3182.\n'
-                                          '</pre>',
+                                          '</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>',
  '_refln_[ms]': '<pre><h2>_refln_[ms]</h2> Data items in the REFLN category record details about '
                 'the\n'
                 ' reflections used to determine the ATOM_SITE data items.\n'
                 ' The REFLN data items refer to individual reflections and\n'
                 ' must be included in looped lists. The REFLNS data items\n'
                 ' specify the parameters that apply to all reflections. The\n'
                 ' REFLNS data items are not looped. Data items in this category\n'
                 ' are extensions of the core CIF dictionary definitions to the\n'
                 ' indexing of reflections used in the refinement by\n'
-                ' higher-dimensional components.</pre>',
+                ' higher-dimensional components.</pre>\n'
+                '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_refln_index_m_1': '<pre><h2>_refln_index_m_1</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_2': '<pre><h2>_refln_index_m_2</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_3': '<pre><h2>_refln_index_m_3</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_4': '<pre><h2>_refln_index_m_4</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_5': '<pre><h2>_refln_index_m_5</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_6': '<pre><h2>_refln_index_m_6</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_7': '<pre><h2>_refln_index_m_7</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_refln_index_m_8': '<pre><h2>_refln_index_m_8</h2> Additional Miller indices of a particular '
                      'reflection in the basis\n'
                      ' described in _cell_reciprocal_basis_description. The total number\n'
                      ' of indices must match (_cell_modulation_dimension + 3). The\n'
                      ' order of the additional indices must be consistent with the codes\n'
-                     ' given in _cell_wave_vector_seq_id.</pre>',
+                     ' given in _cell_wave_vector_seq_id.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_[ms]': '<pre><h2>_reflns_[ms]</h2> Data items in the REFLNS category record details '
                  'about the\n'
                  ' reflections used to determine the ATOM_SITE data items.\n'
                  ' The REFLN data items refer to individual reflections and\n'
                  ' must be included in looped lists. The REFLNS data items\n'
                  ' specify the parameters that apply to all reflections. The\n'
                  ' REFLNS data items are not looped. Data items in this category\n'
                  ' extend the core CIF dictionary definitions providing independent\n'
                  ' checks on the range of values recorded for each of the\n'
-                 ' additional Miller indices given in the REFLN category.</pre>',
+                 ' additional Miller indices given in the REFLN category.</pre>\n'
+                 '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_reflns_limit_index_m_1_max': '<pre><h2>_reflns_limit_index_m_1_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_1_min': '<pre><h2>_reflns_limit_index_m_1_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_2_max': '<pre><h2>_reflns_limit_index_m_2_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_2_min': '<pre><h2>_reflns_limit_index_m_2_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_3_max': '<pre><h2>_reflns_limit_index_m_3_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_3_min': '<pre><h2>_reflns_limit_index_m_3_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_4_max': '<pre><h2>_reflns_limit_index_m_4_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_4_min': '<pre><h2>_reflns_limit_index_m_4_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_5_max': '<pre><h2>_reflns_limit_index_m_5_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_5_min': '<pre><h2>_reflns_limit_index_m_5_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_6_max': '<pre><h2>_reflns_limit_index_m_6_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_6_min': '<pre><h2>_reflns_limit_index_m_6_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_7_max': '<pre><h2>_reflns_limit_index_m_7_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_7_min': '<pre><h2>_reflns_limit_index_m_7_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_8_max': '<pre><h2>_reflns_limit_index_m_8_max</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_reflns_limit_index_m_8_min': '<pre><h2>_reflns_limit_index_m_8_min</h2> Maximum and minimum '
                                 'values of the additional Miller indices\n'
                                 ' appearing in _refln_index_m_. The number of ranges must match\n'
                                 ' _cell_modulation_dimension. The order of the additional indices\n'
                                 ' must be consistent with the codes given in\n'
                                 ' _cell_wave_vector_seq_id. These need not be the same as\n'
-                                ' the _diffrn_reflns_limit_index_m_.</pre>',
+                                ' the _diffrn_reflns_limit_index_m_.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_space_group_[ms]': '<pre><h2>_space_group_[ms]</h2> The SPACE_GROUP category introduced in the '
                       'symmetry CIF\n'
                       ' dictionary (cif_sym.dic) is intended to replace the original\n'
                       ' core SYMMETRY category. For modulated structures, superspace-\n'
                       ' group descriptions may be included in the same category, but\n'
-                      ' include the _ssg_ flag to indicate their dimensionality of &gt; 3.</pre>',
+                      ' include the _ssg_ flag to indicate their dimensionality of &gt; 3.</pre>\n'
+                      '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_space_group_ssg_IT_number': '<pre><h2>_space_group_ssg_IT_number</h2> Superspace-group number '
                                'from International Tables for\n'
                                ' Crystallography, Vol. C (2004). Valid only for one-dimensional\n'
                                ' modulated structures.\n'
                                '\n'
                                ' Ref: International Tables for Crystallography (2004). Vol. C,\n'
-                               '      Chapter 9.8. Dordrecht: Kluwer Academic Publishers.</pre>',
+                               '      Chapter 9.8. Dordrecht: Kluwer Academic Publishers.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 1.1:∞ </p>',
  '_space_group_ssg_WJJ_code': '<pre><h2>_space_group_ssg_WJJ_code</h2> Superspace-group code as '
                               'given by de Wolff, Janssen &amp; Janner\n'
                               ' (1981). Valid only for one-dimensional modulated structures.\n'
                               '\n'
                               ' Ref: Wolff, P. M. de, Janssen, T. &amp; Janner, A. (1981).\n'
                               '      Acta Cryst. A37, 625-636.\n'
                               '\n'
                               '<h3>Example:</h3>\n'
-                              '28a.10.1/2</pre>',
+                              '28a.10.1/2</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_space_group_ssg_name': '<pre><h2>_space_group_ssg_name</h2> Superspace-group symbol conforming '
                           'to an alternative definition\n'
                           ' from that given in _space_group_ssg_name_IT and\n'
                           ' _space_group_ssg_name_WJJ for one-dimensional modulated\n'
                           ' structures or to the superspace-group name for higher dimensions.\n'
                           ' When necessary, indicate the origin and the setting. Use a colon\n'
                           " ':' as a separator between the different parts of the\n"
@@ -13061,15 +13415,16 @@
                           ' _space_group_ssg_name_IT and _space_group_ssg_name_WJJ.\n'
                           ' For composites described in a single data block, the superspace\n'
                           ' group describes the symmetry of the whole structure. The\n'
                           ' symmetry of each subsystem can be derived using the\n'
                           ' appropriate W matrices.\n'
                           '\n'
                           '<h3>Example:</h3>\n'
-                          "Hall's notation W:-P -2xb -2ya:q q</pre>",
+                          "Hall's notation W:-P -2xb -2ya:q q</pre>\n"
+                          '<br><p><h4>Type:</h4> string</p>',
  '_space_group_ssg_name_IT': '<pre><h2>_space_group_ssg_name_IT</h2> Superspace-group symbol as '
                              'given in International Tables for\n'
                              ' Crystallography, Vol. C (2004). Valid only for one-dimensional\n'
                              ' modulated structures. The symbol is divided into three parts:\n'
                              ' the Hermann-Mauguin space-group symbol of the reference\n'
                              ' structure, the modulation wave vector  and the phase shift\n'
                              ' (or internal translation) associated with each component of\n'
@@ -13083,15 +13438,16 @@
                              ' of each subsystem can be derived using the appropriate W\n'
                              ' matrices.\n'
                              '\n'
                              ' Ref: International Tables for Crystallography (2004). Vol. C,\n'
                              '      Chapter 9.8. Dordrecht: Kluwer Academic Publishers.\n'
                              '\n'
                              '<h3>Example:</h3>\n'
-                             'P n m a (0 0 \\g) 0 s 0</pre>',
+                             'P n m a (0 0 \\g) 0 s 0</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_space_group_ssg_name_WJJ': '<pre><h2>_space_group_ssg_name_WJJ</h2> Superspace-group symbol as '
                               'given by de Wolff, Janssen &amp; Janner\n'
                               ' (1981). Valid only for one-dimensional modulated structures.\n'
                               " The symbol is divided into three parts separated by colons ':':\n"
                               ' the superspace lattice symbol, the Hermann-Mauguin space-group\n'
                               ' symbol of the reference structure and the phase shift (or\n'
                               ' internal translation) associated with each component of the\n'
@@ -13103,15 +13459,16 @@
                               ' whole structure. The symmetry of each subsystem can be derived\n'
                               ' using the appropriate W matrices.\n'
                               '\n'
                               ' Ref: Wolff, P. M. de, Janssen, T. &amp; Janner, A. (1981).\n'
                               '      Acta Cryst. A37, 625-636.\n'
                               '\n'
                               '<h3>Example:</h3>\n'
-                              'P:P c m n:s s -1</pre>',
+                              'P:P c m n:s s -1</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_space_group_symop_[ms]': '<pre><h2>_space_group_symop_[ms]</h2> The SPACE_GROUP_SYMOP category '
                             'introduced in the symmetry CIF\n'
                             ' dictionary (cif_sym.dic) is intended to replace the original\n'
                             ' core SYMMETRY_EQUIV category. It contains information about the\n'
                             ' symmetry operations of the space group. For modulated structures,\n'
                             ' superspace-group descriptions may be included in the same\n'
                             ' category, but include the _ssg_ flag to indicate their\n'
@@ -13125,18 +13482,20 @@
                             '  1                       x1,x2,x3,x4\n'
                             '  2                       1/2+x1,1/2-x2,1/2-x3,x4\n'
                             '  3                       1/2-x1,1/2+x2,-x3,1/2-x4\n'
                             '  4                       -x1,-x2,1/2+x3,1/2-x4\n'
                             '  5                       -x1,-x2,-x3,-x4\n'
                             '  6                       1/2-x1,1/2+x2,1/2+x3,-x4\n'
                             '  7                       1/2+x1,1/2-x2,x3,1/2+x4\n'
-                            '  8                       x1,x2,1/2-x3,1/2+x4</pre>',
+                            '  8                       x1,x2,1/2-x3,1/2+x4</pre>\n'
+                            '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_space_group_symop_ssg_id': '<pre><h2>_space_group_symop_ssg_id</h2> A numeric code identifying '
                               'each entry in the\n'
-                              ' _space_group_symop_ssg_operation_algebraic list.</pre>',
+                              ' _space_group_symop_ssg_operation_algebraic list.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_space_group_symop_ssg_operation_algebraic': '<pre><h2>_space_group_symop_ssg_operation_algebraic</h2> '
                                                'A parsable string giving one of the symmetry '
                                                'operations of the\n'
                                                ' superspace group in algebraic form. These data '
                                                'will generally be\n'
                                                ' repeated in a loop. Use symbols as necessary '
                                                'according to\n'
@@ -13152,8 +13511,9 @@
                                                ' as x1,x2,x3,...,xn.\n'
                                                '\n'
                                                ' _space_group_symop_ssg_operation_algebraic must '
                                                'always be present\n'
                                                ' in a CIF corresponding to a modulated structure.\n'
                                                '\n'
                                                '<h3>Example:</h3>\n'
-                                               'x1,-x2,x3,1/2+x4</pre>'}
+                                               'x1,-x2,x3,1/2+x4</pre>\n'
+                                               '<br><p><h4>Type:</h4> string</p>'}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finalcif-136/finalcif/cif/powder_dict.py` & `finalcif-137/finalcif/cif/powder_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,26 @@
                    ' The ID code assigned to each data block should be unique with\n'
                    ' respect to an ID code assigned for any other data block in the\n'
                    ' world. The naming scheme chosen for the block-ID format is\n'
                    ' designed to ensure uniqueness.\n'
                    '\n'
                    ' It is the responsibility of a data archive site or local\n'
                    " laboratory to create a catalogue of block ID's if that site\n"
-                   ' wishes to resolve these references.</pre>',
+                   ' wishes to resolve these references.</pre>\n'
+                   '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_block_diffractogram_id': '<pre><h2>_pd_block_diffractogram_id</h2> A block ID code (see '
                                '_pd_block_id) that identifies\n'
                                ' diffraction data contained in a data block other\n'
                                ' than the current block. This will occur most frequently\n'
                                ' when more than one set of diffraction data\n'
                                ' is used for a structure determination. The data\n'
                                ' block containing the diffraction data will contain\n'
                                ' a _pd_block_id code matching the code in\n'
-                               ' _pd_block_diffractogram_id.</pre>',
+                               ' _pd_block_diffractogram_id.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_block_id': '<pre><h2>_pd_block_id</h2> Used to assign a unique character string to a block.\n'
                  ' Note that this code is not intended to be parsed; the\n'
                  ' concatenation of several strings is used in order to\n'
                  ' generate a string that can reasonably be expected to\n'
                  ' be unique.\n'
                  '\n'
                  ' This code is assigned by the originator of the data set and\n'
@@ -96,20 +98,22 @@
                  ' appropriate block for the final two sections of the ID\n'
                  ' (&lt;creator_name&gt; and &lt;instr_name&gt;). Note that this should\n'
                  ' not be done unless the archive site is prepared to keep the\n'
                  ' file available online indefinitely.\n'
                  '\n'
                  '<h3>Example:</h3>\n'
                  '1991-15-09T16:54|Si-std|B.Toby|D500#1234-987\n'
-                 '1991-15-09T16:54|SEPD7234|B.Toby|SEPD.IPNS.ANL.GOV</pre>',
+                 '1991-15-09T16:54|SEPD7234|B.Toby|SEPD.IPNS.ANL.GOV</pre>\n'
+                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_calc_[pd]': '<pre><h2>_pd_calc_[pd]</h2> This section is used for storing a computed '
                   'diffractogram trace.\n'
                   ' This may be a simulated powder pattern for a material from a\n'
                   ' program such as LAZY/PULVERIX or the computed intensities from a\n'
-                  ' Rietveld refinement.</pre>',
+                  ' Rietveld refinement.</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_calc_intensity_net': '<pre><h2>_pd_calc_intensity_net</h2> Intensity values for a computed '
                            'diffractogram at\n'
                            ' each angle setting. Values should be computed at the\n'
                            ' same locations as the processed diffractogram, and thus\n'
                            ' the numbers of points will be defined by\n'
                            ' _pd_proc_number_of_points and point positions may\n'
                            ' be defined using _pd_proc_2theta_range_ or\n'
@@ -123,15 +127,17 @@
                            ' Use _pd_calc_intensity_total if the computed diffraction\n'
                            ' pattern includes background or normalization corrections\n'
                            ' (or both) and thus is specified on the same scale as the\n'
                            ' observed intensities (_pd_meas_counts_ or _pd_meas_intensity_).\n'
                            '\n'
                            ' If an observed pattern is included, _pd_calc_intensity_\n'
                            ' should be looped with either _pd_proc_intensity_net,\n'
-                           ' _pd_meas_counts_ or _pd_meas_intensity_.</pre>',
+                           ' _pd_meas_counts_ or _pd_meas_intensity_.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_calc_intensity_total': '<pre><h2>_pd_calc_intensity_total</h2> Intensity values for a '
                              'computed diffractogram at\n'
                              ' each angle setting. Values should be computed at the\n'
                              ' same locations as the processed diffractogram, and thus\n'
                              ' the numbers of points will be defined by\n'
                              ' _pd_proc_number_of_points and point positions may\n'
                              ' be defined using _pd_proc_2theta_range_ or\n'
@@ -145,83 +151,95 @@
                              ' Use _pd_calc_intensity_total if the computed diffraction\n'
                              ' pattern includes background or normalization corrections\n'
                              ' (or both) and thus is specified on the same scale as the\n'
                              ' observed intensities (_pd_meas_counts_ or _pd_meas_intensity_).\n'
                              '\n'
                              ' If an observed pattern is included, _pd_calc_intensity_\n'
                              ' should be looped with either _pd_proc_intensity_net,\n'
-                             ' _pd_meas_counts_ or _pd_meas_intensity_.</pre>',
+                             ' _pd_meas_counts_ or _pd_meas_intensity_.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_calc_method': '<pre><h2>_pd_calc_method</h2> A description of the method used for the '
                     'calculation of\n'
                     ' the intensities in _pd_calc_intensity_. If the pattern was\n'
                     ' calculated from crystal structure data, the atom coordinates\n'
                     ' and other crystallographic information should be included\n'
-                    ' using the core CIF _atom_site_ and _cell_ data items.</pre>',
+                    ' using the core CIF _atom_site_ and _cell_ data items.</pre>\n'
+                    '<br><p><h4>Type:</h4> string</p>',
  '_pd_calc_point_id': '<pre><h2>_pd_calc_point_id</h2> Arbitrary label identifying a calculated '
                       'data point. Used to\n'
                       ' identify a specific entry in a list of values forming the\n'
                       ' calculated diffractogram. The role of this identifier may\n'
                       ' be adopted by _pd_data_point_id if measured, processed and\n'
-                      ' calculated intensity values are combined in a single list.</pre>',
+                      ' calculated intensity values are combined in a single list.</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_calib_2theta_off_max': '<pre><h2>_pd_calib_2theta_off_max</h2> _pd_calib_2theta_offset '
                              'defines an offset angle (in degrees)\n'
                              ' used to calibrate 2\\q (as defined in _pd_meas_2theta_).\n'
                              ' Calibration is done by adding the offset:\n'
                              '\n'
                              '      2\\q~calibrated~ = 2\\q~measured~ + 2\\q~offset~\n'
                              '\n'
                              ' For cases where the _pd_calib_2theta_offset value is\n'
                              ' not a constant, but rather varies with 2\\q, a set\n'
                              ' of offset values can be supplied in a loop. In this case,\n'
                              ' the value where the offset has been determined can be\n'
                              ' specified as _pd_calib_2theta_off_point. Alternatively, a\n'
                              ' range where the offset is applicable can be specified using\n'
-                             ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>',
+                             ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_calib_2theta_off_min': '<pre><h2>_pd_calib_2theta_off_min</h2> _pd_calib_2theta_offset '
                              'defines an offset angle (in degrees)\n'
                              ' used to calibrate 2\\q (as defined in _pd_meas_2theta_).\n'
                              ' Calibration is done by adding the offset:\n'
                              '\n'
                              '      2\\q~calibrated~ = 2\\q~measured~ + 2\\q~offset~\n'
                              '\n'
                              ' For cases where the _pd_calib_2theta_offset value is\n'
                              ' not a constant, but rather varies with 2\\q, a set\n'
                              ' of offset values can be supplied in a loop. In this case,\n'
                              ' the value where the offset has been determined can be\n'
                              ' specified as _pd_calib_2theta_off_point. Alternatively, a\n'
                              ' range where the offset is applicable can be specified using\n'
-                             ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>',
+                             ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_calib_2theta_off_point': '<pre><h2>_pd_calib_2theta_off_point</h2> _pd_calib_2theta_offset '
                                'defines an offset angle (in degrees)\n'
                                ' used to calibrate 2\\q (as defined in _pd_meas_2theta_).\n'
                                ' Calibration is done by adding the offset:\n'
                                '\n'
                                '      2\\q~calibrated~ = 2\\q~measured~ + 2\\q~offset~\n'
                                '\n'
                                ' For cases where the _pd_calib_2theta_offset value is\n'
                                ' not a constant, but rather varies with 2\\q, a set\n'
                                ' of offset values can be supplied in a loop. In this case,\n'
                                ' the value where the offset has been determined can be\n'
                                ' specified as _pd_calib_2theta_off_point. Alternatively, a\n'
                                ' range where the offset is applicable can be specified using\n'
-                               ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>',
+                               ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_calib_2theta_offset': '<pre><h2>_pd_calib_2theta_offset</h2> _pd_calib_2theta_offset defines '
                             'an offset angle (in degrees)\n'
                             ' used to calibrate 2\\q (as defined in _pd_meas_2theta_).\n'
                             ' Calibration is done by adding the offset:\n'
                             '\n'
                             '      2\\q~calibrated~ = 2\\q~measured~ + 2\\q~offset~\n'
                             '\n'
                             ' For cases where the _pd_calib_2theta_offset value is\n'
                             ' not a constant, but rather varies with 2\\q, a set\n'
                             ' of offset values can be supplied in a loop. In this case,\n'
                             ' the value where the offset has been determined can be\n'
                             ' specified as _pd_calib_2theta_off_point. Alternatively, a\n'
                             ' range where the offset is applicable can be specified using\n'
-                            ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>',
+                            ' _pd_calib_2theta_off_min and _pd_calib_2theta_off_max.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_calib_[pd]': '<pre><h2>_pd_calib_[pd]</h2> This section defines the parameters used for the '
                    'calibration \n'
                    ' of the instrument that are used directly or indirectly in the \n'
                    ' interpretation of this data set. The information in this \n'
                    ' section of the CIF should generally be written when the \n'
                    ' intensities are first measured, but from then on should remain \n'
                    ' unchanged. Loops may be used for calibration information that \n'
@@ -234,104 +252,120 @@
                    ' QuartzPlate|D500#1234-987|B.Toby|91-15-09|14:02\n'
                    '   _pd_calib_std_external_name\n'
                    " 'Arkansas Stone quartz plate'\n"
                    '\n'
                    '    _pd_calibration_conversion_eqn\n'
                    '    ; 2\\q~actual~ = 2\\q~setting~ + arctan(\n'
                    '      cos(P~1~)/{1/[P~0~ (CC - CH~0~ - P~2~ CC^2^)] - sin(P~1~)})\n'
-                   '    ;</pre>',
+                   '    ;</pre>\n'
+                   '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_calib_detector_id': '<pre><h2>_pd_calib_detector_id</h2> A code which identifies the '
                           'detector or channel number in a\n'
                           ' position-sensitive, energy-dispersive or other multiple-detector\n'
                           ' instrument. Note that this code should match the code name used\n'
-                          ' for _pd_meas_detector_id.</pre>',
+                          ' for _pd_meas_detector_id.</pre>\n'
+                          '<br><p><h4>Type:</h4> string</p>',
  '_pd_calib_detector_response': '<pre><h2>_pd_calib_detector_response</h2> A value that indicates '
                                 'the relative sensitivity of each\n'
                                 ' detector. This can compensate for differences in electronics,\n'
                                 ' size and collimation. Usually, one detector or the mean for\n'
-                                ' all detectors will be assigned the value of 1.</pre>',
+                                ' all detectors will be assigned the value of 1.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_calib_std_external_block_id': '<pre><h2>_pd_calib_std_external_block_id</h2> Identifies the '
                                     'data set used as an external standard for\n'
                                     ' the diffraction angle or the intensity calibrations.\n'
                                     ' *_name specifies the name of the material and\n'
                                     ' *_id the _pd_block_id for the CIF containing calibration\n'
                                     ' measurements. If more than one data set is used for\n'
-                                    ' calibration, these fields may be looped.</pre>',
+                                    ' calibration, these fields may be looped.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_pd_calib_std_external_name': '<pre><h2>_pd_calib_std_external_name</h2> Identifies the data set '
                                 'used as an external standard for\n'
                                 ' the diffraction angle or the intensity calibrations.\n'
                                 ' *_name specifies the name of the material and\n'
                                 ' *_id the _pd_block_id for the CIF containing calibration\n'
                                 ' measurements. If more than one data set is used for\n'
-                                ' calibration, these fields may be looped.</pre>',
+                                ' calibration, these fields may be looped.</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_calib_std_internal_mass_%': '<pre><h2>_pd_calib_std_internal_mass_%</h2> Per cent presence '
                                   'of the internal standard specified by the\n'
                                   ' data item _pd_calib_std_internal_name expressed as 100 times\n'
                                   ' the ratio of the amount of standard added to the original\n'
-                                  ' sample mass.</pre>',
+                                  ' sample mass.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:100.0 </p>',
  '_pd_calib_std_internal_name': '<pre><h2>_pd_calib_std_internal_name</h2> Identity of material(s) '
                                 'used as an internal intensity standard.\n'
                                 '\n'
                                 '<h3>Example:</h3>\n'
                                 'NIST 640a Silicon standard\n'
-                                'Al2O3</pre>',
+                                'Al2O3</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_calibration_conversion_eqn': '<pre><h2>_pd_calibration_conversion_eqn</h2> The calibration '
                                    'function for converting a channel number\n'
                                    ' supplied in _pd_meas_detector_id for a position-sensitive\n'
                                    ' or energy-dispersive detector or the distance supplied in\n'
                                    ' _pd_meas_position to Q, energy, angle etc.\n'
                                    ' Use _pd_calib_std_external_ to define a pointer\n'
                                    ' to the file or data block containing the information used\n'
                                    ' to define this function.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    ' 2\\q~actual~ = 2\\q~setting~ + arctan(\n'
                                    'os(P~1~) / {1/[P~0~ (CC - CH~0~ - P~2~ CC^2^)] - sin(P~1~)} '
-                                   ')</pre>',
+                                   ')</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_pd_calibration_special_details': '<pre><h2>_pd_calibration_special_details</h2> Description of '
                                     'how the instrument was\n'
                                     ' calibrated, particularly for instruments where\n'
                                     ' calibration information is used to make hardware\n'
                                     ' settings that would otherwise be invisible once data\n'
                                     ' collection is completed. Do not use this item to specify\n'
                                     ' information that can be specified using other _pd_calib_\n'
-                                    ' items.</pre>',
+                                    ' items.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_pd_char_[pd]': '<pre><h2>_pd_char_[pd]</h2>   This section contains experimental '
                   '(non-diffraction) information\n'
-                  '    relevant to the chemical and physical nature of the material.</pre>',
+                  '    relevant to the chemical and physical nature of the material.</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_char_atten_coef_mu_calc': '<pre><h2>_pd_char_atten_coef_mu_calc</h2> The observed and '
                                 'calculated linear attenuation coefficient,\n'
                                 ' \\m, in units of inverse millimetres. Note that this quantity\n'
                                 ' is sometimes referred to as the mass absorption coefficient;\n'
                                 ' however, this term accounts for other potentially significant\n'
                                 ' losses of incident radiation, for example incoherent\n'
                                 ' scattering of neutrons.\n'
                                 '\n'
                                 ' The calculated \\m will be obtained from the atomic content of\n'
                                 ' the cell, the average density (allowing for specimen packing)\n'
                                 ' and the radiation wavelength. The observed \\m will be\n'
                                 ' determined by a transmission measurement.\n'
                                 ' Note that _pd_char_atten_coef_mu_calc will differ from\n'
                                 ' _exptl_absorpt_coefficient_mu if the packing density is\n'
-                                ' not unity.</pre>',
+                                ' not unity.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_char_atten_coef_mu_obs': '<pre><h2>_pd_char_atten_coef_mu_obs</h2> The observed and '
                                'calculated linear attenuation coefficient,\n'
                                ' \\m, in units of inverse millimetres. Note that this quantity\n'
                                ' is sometimes referred to as the mass absorption coefficient;\n'
                                ' however, this term accounts for other potentially significant\n'
                                ' losses of incident radiation, for example incoherent\n'
                                ' scattering of neutrons.\n'
                                '\n'
                                ' The calculated \\m will be obtained from the atomic content of\n'
                                ' the cell, the average density (allowing for specimen packing)\n'
                                ' and the radiation wavelength. The observed \\m will be\n'
                                ' determined by a transmission measurement.\n'
                                ' Note that _pd_char_atten_coef_mu_calc will differ from\n'
                                ' _exptl_absorpt_coefficient_mu if the packing density is\n'
-                               ' not unity.</pre>',
+                               ' not unity.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_char_colour': '<pre><h2>_pd_char_colour</h2> The colour of the material used for the '
                     'measurement.\n'
                     ' To facilitate more standardized use of names, the\n'
                     ' following guidelines for colour naming developed by\n'
                     ' Peter Bayliss for the International Centre for \n'
                     ' Diffraction Data (ICDD) should be followed. Note that\n'
                     ' combinations of descriptors are separated by an\n'
@@ -355,24 +389,27 @@
                     ' that occur with ranges of colours; however this usage is\n'
                     ' not appropriate for the description of a single sample.\n'
                     '\n'
                     '<h3>Example:</h3>\n'
                     'dark_green\n'
                     'orange_red\n'
                     'brownish_red\n'
-                    'yellow_metallic</pre>',
+                    'yellow_metallic</pre>\n'
+                    '<br><p><h4>Type:</h4> string</p>',
  '_pd_char_particle_morphology': '<pre><h2>_pd_char_particle_morphology</h2> A description of the '
                                  'sample morphology and estimates for\n'
                                  ' particle sizes (before grinding/sieving, if noted by\n'
                                  ' _pd_spec_preparation). Include the method used for\n'
-                                 ' these estimates (SEM, visual estimate etc.).</pre>',
+                                 ' these estimates (SEM, visual estimate etc.).</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_char_special_details': '<pre><h2>_pd_char_special_details</h2> Additional characterization '
                              'information relevant to the sample\n'
                              ' or documentation of non-routine processing steps used\n'
-                             ' for characterization.</pre>',
+                             ' for characterization.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_pd_data_[pd]': '<pre><h2>_pd_data_[pd]</h2> The PD_DATA category contains raw, processed and '
                   'calculated\n'
                   ' data points in a diffraction data set. In many cases, it is\n'
                   ' convenient to tabulate calculated values against the\n'
                   ' raw and processed measurements, and so the various\n'
                   ' _pd_meas_, _pd_proc_ and _pd_calc_ data items belonging\n'
                   ' to this category may be looped together. In some instances,\n'
@@ -432,26 +469,32 @@
                   '     _pd_calc_point_id\n'
                   '     _pd_proc_2theta_corrected\n'
                   '     _pd_calc_intensity_total\n'
                   '            1   21.0  26\n'
                   '            1a  21.3  56\n'
                   '            4   21.6  76\n'
                   '            4a  21.9  90\n'
-                  '</pre>',
+                  '</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_data_point_id': '<pre><h2>_pd_data_point_id</h2> Arbitrary label identifying an entry in the '
                       'table of\n'
-                      ' diffractogram intensity values.</pre>',
+                      ' diffractogram intensity values.</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_2theta_monochr_post': '<pre><h2>_pd_instr_2theta_monochr_post</h2> The 2\\q angle for '
                                   'a pre-specimen or post-specimen\n'
                                   ' monochromator (see _pd_instr_monochr_pre_spec and\n'
-                                  ' _pd_instr_monochr_post_spec).</pre>',
+                                  ' _pd_instr_monochr_post_spec).</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_instr_2theta_monochr_pre': '<pre><h2>_pd_instr_2theta_monochr_pre</h2> The 2\\q angle for a '
                                  'pre-specimen or post-specimen\n'
                                  ' monochromator (see _pd_instr_monochr_pre_spec and\n'
-                                 ' _pd_instr_monochr_post_spec).</pre>',
+                                 ' _pd_instr_monochr_post_spec).</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_instr_[pd]': '<pre><h2>_pd_instr_[pd]</h2> This section contains information relevant to the '
                    'instrument\n'
                    ' used for the diffraction measurement. For most laboratories,\n'
                    ' very little of this information will change, so a standard file\n'
                    ' may be prepared and included with each data set.\n'
                    '\n'
                    ' Note that several definitions in the core CIF dictionary\n'
@@ -492,50 +535,58 @@
                    '<h3>Example:</h3>\n'
                    '\n'
                    '    _pd_instr_slit_eq_src/spec       1.\n'
                    '    _pd_instr_slit_eq_anal/detc      0.2\n'
                    '\n'
                    '    _pd_instr_geometry              Bragg-Brentano\n'
                    "    _pd_instr_monochr_post_spec     'graphite (0001)'\n"
-                   '    _pd_instr_cons_illum_flag       no</pre>',
+                   '    _pd_instr_cons_illum_flag       no</pre>\n'
+                   '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_instr_beam_size_ax': '<pre><h2>_pd_instr_beam_size_ax</h2> Axial and equatorial dimensions '
                            'of the radiation beam\n'
                            ' at the specimen position (in millimetres).\n'
                            ' The perpendicular to the plane containing the incident\n'
-                           ' and scattered beam is the axial (*_ax) direction.</pre>',
+                           ' and scattered beam is the axial (*_ax) direction.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_beam_size_eq': '<pre><h2>_pd_instr_beam_size_eq</h2> Axial and equatorial dimensions '
                            'of the radiation beam\n'
                            ' at the specimen position (in millimetres).\n'
                            ' The perpendicular to the plane containing the incident\n'
-                           ' and scattered beam is the axial (*_ax) direction.</pre>',
+                           ' and scattered beam is the axial (*_ax) direction.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_cons_illum_flag': "<pre><h2>_pd_instr_cons_illum_flag</h2> Use 'yes' for instruments "
                               'where the divergence slit is\n'
                               ' \\q-compensated to yield a constant illumination length\n'
                               ' (also see _pd_instr_cons_illum_len).\n'
                               '\n'
                               ' For other flat-plate instruments, where the illumination\n'
                               " length changes with 2\\q, specify 'no'. Note that\n"
                               ' if the length is known, it may be specified using\n'
                               ' _pd_instr_var_illum_len.\n'
                               '\n'
                               '<h3>Example:</h3>\n'
                               'yes\n'
-                              'no</pre>',
+                              'no</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_cons_illum_len': '<pre><h2>_pd_instr_cons_illum_len</h2> Length of the specimen that '
                              'is illuminated by the radiation\n'
                              ' source (in millimetres).\n'
                              '\n'
                              ' Use _pd_instr_cons_illum_len for instruments where\n'
                              ' the illumination length does not vary with 2\\q, by\n'
                              ' adjustment of the divergence slits (sometimes known\n'
                              ' as \\q-compensated slits).\n'
                              ' Use _pd_instr_var_illum_len for instruments where\n'
                              ' the illuminated length of the specimen has been \n'
                              ' characterized as a function of 2\\q, most commonly true\n'
-                             ' with a fixed divergence slit.</pre>',
+                             ' with a fixed divergence slit.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_anal/detc': '<pre><h2>_pd_instr_dist_anal/detc</h2> Specifies distances in '
                              'millimetres for the instrument geometry:\n'
                              '   *_src/mono, the distance from the radiation source\n'
                              '       to the monochromator;\n'
                              '   *_mono/spec, the distance from the monochromator to\n'
                              '       the specimen;\n'
                              '   *_src/spec, the distance from the radiation source\n'
@@ -546,15 +597,17 @@
                              '       detector;\n'
                              '   *_spec/detc, the distance from the specimen to the\n'
                              '       detector.\n'
                              '\n'
                              ' Note that *_src/spec is used in place of *_src/mono and \n'
                              ' *_mono/spec if there is no monochromator in use, and \n'
                              ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                             ' if there is no analyser in use.</pre>',
+                             ' if there is no analyser in use.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_mono/spec': '<pre><h2>_pd_instr_dist_mono/spec</h2> Specifies distances in '
                              'millimetres for the instrument geometry:\n'
                              '   *_src/mono, the distance from the radiation source\n'
                              '       to the monochromator;\n'
                              '   *_mono/spec, the distance from the monochromator to\n'
                              '       the specimen;\n'
                              '   *_src/spec, the distance from the radiation source\n'
@@ -565,15 +618,17 @@
                              '       detector;\n'
                              '   *_spec/detc, the distance from the specimen to the\n'
                              '       detector.\n'
                              '\n'
                              ' Note that *_src/spec is used in place of *_src/mono and \n'
                              ' *_mono/spec if there is no monochromator in use, and \n'
                              ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                             ' if there is no analyser in use.</pre>',
+                             ' if there is no analyser in use.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_spec/anal': '<pre><h2>_pd_instr_dist_spec/anal</h2> Specifies distances in '
                              'millimetres for the instrument geometry:\n'
                              '   *_src/mono, the distance from the radiation source\n'
                              '       to the monochromator;\n'
                              '   *_mono/spec, the distance from the monochromator to\n'
                              '       the specimen;\n'
                              '   *_src/spec, the distance from the radiation source\n'
@@ -584,15 +639,17 @@
                              '       detector;\n'
                              '   *_spec/detc, the distance from the specimen to the\n'
                              '       detector.\n'
                              '\n'
                              ' Note that *_src/spec is used in place of *_src/mono and \n'
                              ' *_mono/spec if there is no monochromator in use, and \n'
                              ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                             ' if there is no analyser in use.</pre>',
+                             ' if there is no analyser in use.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_spec/detc': '<pre><h2>_pd_instr_dist_spec/detc</h2> Specifies distances in '
                              'millimetres for the instrument geometry:\n'
                              '   *_src/mono, the distance from the radiation source\n'
                              '       to the monochromator;\n'
                              '   *_mono/spec, the distance from the monochromator to\n'
                              '       the specimen;\n'
                              '   *_src/spec, the distance from the radiation source\n'
@@ -603,15 +660,17 @@
                              '       detector;\n'
                              '   *_spec/detc, the distance from the specimen to the\n'
                              '       detector.\n'
                              '\n'
                              ' Note that *_src/spec is used in place of *_src/mono and \n'
                              ' *_mono/spec if there is no monochromator in use, and \n'
                              ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                             ' if there is no analyser in use.</pre>',
+                             ' if there is no analyser in use.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_src/mono': '<pre><h2>_pd_instr_dist_src/mono</h2> Specifies distances in '
                             'millimetres for the instrument geometry:\n'
                             '   *_src/mono, the distance from the radiation source\n'
                             '       to the monochromator;\n'
                             '   *_mono/spec, the distance from the monochromator to\n'
                             '       the specimen;\n'
                             '   *_src/spec, the distance from the radiation source\n'
@@ -622,15 +681,17 @@
                             '       detector;\n'
                             '   *_spec/detc, the distance from the specimen to the\n'
                             '       detector.\n'
                             '\n'
                             ' Note that *_src/spec is used in place of *_src/mono and \n'
                             ' *_mono/spec if there is no monochromator in use, and \n'
                             ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                            ' if there is no analyser in use.</pre>',
+                            ' if there is no analyser in use.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_dist_src/spec': '<pre><h2>_pd_instr_dist_src/spec</h2> Specifies distances in '
                             'millimetres for the instrument geometry:\n'
                             '   *_src/mono, the distance from the radiation source\n'
                             '       to the monochromator;\n'
                             '   *_mono/spec, the distance from the monochromator to\n'
                             '       the specimen;\n'
                             '   *_src/spec, the distance from the radiation source\n'
@@ -641,15 +702,17 @@
                             '       detector;\n'
                             '   *_spec/detc, the distance from the specimen to the\n'
                             '       detector.\n'
                             '\n'
                             ' Note that *_src/spec is used in place of *_src/mono and \n'
                             ' *_mono/spec if there is no monochromator in use, and \n'
                             ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                            ' if there is no analyser in use.</pre>',
+                            ' if there is no analyser in use.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_anal/detc': '<pre><h2>_pd_instr_divg_ax_anal/detc</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument.\n'
                                 ' Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -665,15 +728,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_mono/spec': '<pre><h2>_pd_instr_divg_ax_mono/spec</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument.\n'
                                 ' Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -689,15 +754,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_spec/anal': '<pre><h2>_pd_instr_divg_ax_spec/anal</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument.\n'
                                 ' Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -713,15 +780,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_spec/detc': '<pre><h2>_pd_instr_divg_ax_spec/detc</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument.\n'
                                 ' Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -737,15 +806,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_src/mono': '<pre><h2>_pd_instr_divg_ax_src/mono</h2> Describes collimation in '
                                'the axial direction\n'
                                ' (perpendicular to the plane containing the incident\n'
                                ' and diffracted beams) for the instrument.\n'
                                ' Values are the maximum divergence angles in\n'
                                ' degrees, as limited by slits or beamline optics\n'
                                ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -761,15 +832,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_ax_src/spec': '<pre><h2>_pd_instr_divg_ax_src/spec</h2> Describes collimation in '
                                'the axial direction\n'
                                ' (perpendicular to the plane containing the incident\n'
                                ' and diffracted beams) for the instrument.\n'
                                ' Values are the maximum divergence angles in\n'
                                ' degrees, as limited by slits or beamline optics\n'
                                ' other than Soller slits (see _pd_instr_soller_ax_):\n'
@@ -785,15 +858,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_anal/detc': '<pre><h2>_pd_instr_divg_eq_anal/detc</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for\n'
                                 ' the instrument. Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -808,15 +883,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_mono/spec': '<pre><h2>_pd_instr_divg_eq_mono/spec</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for\n'
                                 ' the instrument. Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -831,15 +908,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_spec/anal': '<pre><h2>_pd_instr_divg_eq_spec/anal</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for\n'
                                 ' the instrument. Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -854,15 +933,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_spec/detc': '<pre><h2>_pd_instr_divg_eq_spec/detc</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for\n'
                                 ' the instrument. Values are the maximum divergence angles in\n'
                                 ' degrees, as limited by slits or beamline optics\n'
                                 ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -877,15 +958,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_src/mono': '<pre><h2>_pd_instr_divg_eq_src/mono</h2> Describes collimation in '
                                'the equatorial plane (the plane\n'
                                ' containing the incident and diffracted beams) for\n'
                                ' the instrument. Values are the maximum divergence angles in\n'
                                ' degrees, as limited by slits or beamline optics\n'
                                ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                '   *_src/mono, collimation between the radiation source\n'
@@ -900,15 +983,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_divg_eq_src/spec': '<pre><h2>_pd_instr_divg_eq_src/spec</h2> Describes collimation in '
                                'the equatorial plane (the plane\n'
                                ' containing the incident and diffracted beams) for\n'
                                ' the instrument. Values are the maximum divergence angles in\n'
                                ' degrees, as limited by slits or beamline optics\n'
                                ' other than Soller slits (see _pd_instr_soller_eq_):\n'
                                '   *_src/mono, collimation between the radiation source\n'
@@ -923,32 +1008,36 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_geometry': '<pre><h2>_pd_instr_geometry</h2> A description of the diffractometer type '
                        'or geometry.\n'
                        '\n'
                        '<h3>Example:</h3>\n'
                        'Bragg-Brentano\n'
                        'Guinier\n'
                        '           Parallel-beam non-focusing optics with\n'
                        '            channel-cut monochromator and linear\n'
-                       '            position-sensitive detector</pre>',
+                       '            position-sensitive detector</pre>\n'
+                       '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_location': '<pre><h2>_pd_instr_location</h2> The name and location of the instrument '
                        'where measurements\n'
                        ' were made. This is used primarily to identify data sets\n'
                        " measured away from the author's home facility, at shared\n"
                        ' resources such as a reactor or spallation source.\n'
                        '\n'
                        '<h3>Example:</h3>\n'
-                       'SEPD diffractometer, IPNS, Argonne National Lab (USA)</pre>',
+                       'SEPD diffractometer, IPNS, Argonne National Lab (USA)</pre>\n'
+                       '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_monochr_post_spec': '<pre><h2>_pd_instr_monochr_post_spec</h2> Indicates the method '
                                 'used to obtain monochromatic radiation.\n'
                                 ' Use _pd_instr_monochr_pre_spec to describe the primary beam\n'
                                 ' monochromator (pre-specimen monochromation). Use\n'
                                 ' _pd_instr_monochr_post_spec to specify the\n'
                                 ' post-diffraction analyser (post-specimen monochromation).\n'
                                 '\n'
@@ -969,15 +1058,16 @@
                                 ' pp. 164-165. New York: Wiley.\n'
                                 '\n'
                                 '<h3>Example:</h3>\n'
                                 'Zr filter\n'
                                 'Ge 220\n'
                                 'none\n'
                                 'equatorial mounted graphite (0001)\n'
-                                'Si (111), antiparallel</pre>',
+                                'Si (111), antiparallel</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_monochr_pre_spec': '<pre><h2>_pd_instr_monochr_pre_spec</h2> Indicates the method used '
                                'to obtain monochromatic radiation.\n'
                                ' Use _pd_instr_monochr_pre_spec to describe the primary beam\n'
                                ' monochromator (pre-specimen monochromation). Use\n'
                                ' _pd_instr_monochr_post_spec to specify the\n'
                                ' post-diffraction analyser (post-specimen monochromation).\n'
                                '\n'
@@ -998,15 +1088,16 @@
                                ' pp. 164-165. New York: Wiley.\n'
                                '\n'
                                '<h3>Example:</h3>\n'
                                'Zr filter\n'
                                'Ge 220\n'
                                'none\n'
                                'equatorial mounted graphite (0001)\n'
-                               'Si (111), antiparallel</pre>',
+                               'Si (111), antiparallel</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_slit_ax_anal/detc': '<pre><h2>_pd_instr_slit_ax_anal/detc</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument as a slit width\n'
                                 ' (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -1021,15 +1112,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_ax_mono/spec': '<pre><h2>_pd_instr_slit_ax_mono/spec</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument as a slit width\n'
                                 ' (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -1044,15 +1137,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_ax_spec/anal': '<pre><h2>_pd_instr_slit_ax_spec/anal</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument as a slit width\n'
                                 ' (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -1067,15 +1162,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_ax_spec/detc': '<pre><h2>_pd_instr_slit_ax_spec/detc</h2> Describes collimation '
                                 'in the axial direction\n'
                                 ' (perpendicular to the plane containing the incident\n'
                                 ' and diffracted beams) for the instrument as a slit width\n'
                                 ' (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
@@ -1090,15 +1187,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                                ' if there is no analyser in use.</pre>',
+                                ' if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_ax_src/mono': '<pre><h2>_pd_instr_slit_ax_src/mono</h2> Describes collimation in '
                                'the axial direction\n'
                                ' (perpendicular to the plane containing the incident\n'
                                ' and diffracted beams) for the instrument as a slit width\n'
                                ' (as opposed to a divergence angle).\n'
                                ' Values are the width of the slit (in millimetres) defining:\n'
                                '   *_src/mono, collimation between the radiation source\n'
@@ -1113,15 +1212,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_ax_src/spec': '<pre><h2>_pd_instr_slit_ax_src/spec</h2> Describes collimation in '
                                'the axial direction\n'
                                ' (perpendicular to the plane containing the incident\n'
                                ' and diffracted beams) for the instrument as a slit width\n'
                                ' (as opposed to a divergence angle).\n'
                                ' Values are the width of the slit (in millimetres) defining:\n'
                                '   *_src/mono, collimation between the radiation source\n'
@@ -1136,15 +1237,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and *_anal/detc \n'
-                               ' if there is no analyser in use.</pre>',
+                               ' if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_anal/detc': '<pre><h2>_pd_instr_slit_eq_anal/detc</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for the\n'
                                 ' instrument as a slit width (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
                                 '       and the monochromator;\n'
@@ -1158,15 +1261,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and \n'
-                                ' *_anal/detc if there is no analyser in use.</pre>',
+                                ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_mono/spec': '<pre><h2>_pd_instr_slit_eq_mono/spec</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for the\n'
                                 ' instrument as a slit width (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
                                 '       and the monochromator;\n'
@@ -1180,15 +1285,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and \n'
-                                ' *_anal/detc if there is no analyser in use.</pre>',
+                                ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_spec/anal': '<pre><h2>_pd_instr_slit_eq_spec/anal</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for the\n'
                                 ' instrument as a slit width (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
                                 '       and the monochromator;\n'
@@ -1202,15 +1309,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and \n'
-                                ' *_anal/detc if there is no analyser in use.</pre>',
+                                ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_spec/detc': '<pre><h2>_pd_instr_slit_eq_spec/detc</h2> Describes collimation '
                                 'in the equatorial plane (the plane\n'
                                 ' containing the incident and diffracted beams) for the\n'
                                 ' instrument as a slit width (as opposed to a divergence angle).\n'
                                 ' Values are the width of the slit (in millimetres) defining:\n'
                                 '   *_src/mono, collimation between the radiation source\n'
                                 '       and the monochromator;\n'
@@ -1224,15 +1333,17 @@
                                 '       detector;\n'
                                 '   *_spec/detc, collimation between the specimen and the\n'
                                 '       detector.\n'
                                 '\n'
                                 ' Note that *_src/spec is used in place of *_src/mono and \n'
                                 ' *_mono/spec if there is no monochromator in use, and \n'
                                 ' *_spec/detc is used in place of *_spec/anal and \n'
-                                ' *_anal/detc if there is no analyser in use.</pre>',
+                                ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_src/mono': '<pre><h2>_pd_instr_slit_eq_src/mono</h2> Describes collimation in '
                                'the equatorial plane (the plane\n'
                                ' containing the incident and diffracted beams) for the\n'
                                ' instrument as a slit width (as opposed to a divergence angle).\n'
                                ' Values are the width of the slit (in millimetres) defining:\n'
                                '   *_src/mono, collimation between the radiation source\n'
                                '       and the monochromator;\n'
@@ -1246,15 +1357,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and \n'
-                               ' *_anal/detc if there is no analyser in use.</pre>',
+                               ' *_anal/detc if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_slit_eq_src/spec': '<pre><h2>_pd_instr_slit_eq_src/spec</h2> Describes collimation in '
                                'the equatorial plane (the plane\n'
                                ' containing the incident and diffracted beams) for the\n'
                                ' instrument as a slit width (as opposed to a divergence angle).\n'
                                ' Values are the width of the slit (in millimetres) defining:\n'
                                '   *_src/mono, collimation between the radiation source\n'
                                '       and the monochromator;\n'
@@ -1268,15 +1381,17 @@
                                '       detector;\n'
                                '   *_spec/detc, collimation between the specimen and the\n'
                                '       detector.\n'
                                '\n'
                                ' Note that *_src/spec is used in place of *_src/mono and \n'
                                ' *_mono/spec if there is no monochromator in use, and \n'
                                ' *_spec/detc is used in place of *_spec/anal and \n'
-                               ' *_anal/detc if there is no analyser in use.</pre>',
+                               ' *_anal/detc if there is no analyser in use.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_anal/detc': '<pre><h2>_pd_instr_soller_ax_anal/detc</h2> Describes '
                                   'collimation in the axial direction\n'
                                   ' (perpendicular to the plane containing the incident\n'
                                   ' and diffracted beams) for the instrument.\n'
                                   ' Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
@@ -1291,15 +1406,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_mono/spec': '<pre><h2>_pd_instr_soller_ax_mono/spec</h2> Describes '
                                   'collimation in the axial direction\n'
                                   ' (perpendicular to the plane containing the incident\n'
                                   ' and diffracted beams) for the instrument.\n'
                                   ' Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
@@ -1314,15 +1431,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_spec/anal': '<pre><h2>_pd_instr_soller_ax_spec/anal</h2> Describes '
                                   'collimation in the axial direction\n'
                                   ' (perpendicular to the plane containing the incident\n'
                                   ' and diffracted beams) for the instrument.\n'
                                   ' Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
@@ -1337,15 +1456,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_spec/detc': '<pre><h2>_pd_instr_soller_ax_spec/detc</h2> Describes '
                                   'collimation in the axial direction\n'
                                   ' (perpendicular to the plane containing the incident\n'
                                   ' and diffracted beams) for the instrument.\n'
                                   ' Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
@@ -1360,15 +1481,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_src/mono': '<pre><h2>_pd_instr_soller_ax_src/mono</h2> Describes collimation '
                                  'in the axial direction\n'
                                  ' (perpendicular to the plane containing the incident\n'
                                  ' and diffracted beams) for the instrument.\n'
                                  ' Values are the maximum divergence angles in\n'
                                  ' degrees, as limited by Soller slits located thus:\n'
                                  '   *_src/mono, collimation between the radiation source\n'
@@ -1383,15 +1506,17 @@
                                  '       detector;\n'
                                  '   *_spec/detc, collimation between the specimen and the\n'
                                  '       detector.\n'
                                  '\n'
                                  ' Note that *_src/spec is used in place of *_src/mono and \n'
                                  ' *_mono/spec if there is no monochromator in use, and \n'
                                  ' *_spec/detc is used in place of *_spec/anal and \n'
-                                 ' *_anal/detc if there is no analyser in use.</pre>',
+                                 ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_ax_src/spec': '<pre><h2>_pd_instr_soller_ax_src/spec</h2> Describes collimation '
                                  'in the axial direction\n'
                                  ' (perpendicular to the plane containing the incident\n'
                                  ' and diffracted beams) for the instrument.\n'
                                  ' Values are the maximum divergence angles in\n'
                                  ' degrees, as limited by Soller slits located thus:\n'
                                  '   *_src/mono, collimation between the radiation source\n'
@@ -1406,15 +1531,17 @@
                                  '       detector;\n'
                                  '   *_spec/detc, collimation between the specimen and the\n'
                                  '       detector.\n'
                                  '\n'
                                  ' Note that *_src/spec is used in place of *_src/mono and \n'
                                  ' *_mono/spec if there is no monochromator in use, and \n'
                                  ' *_spec/detc is used in place of *_spec/anal and \n'
-                                 ' *_anal/detc if there is no analyser in use.</pre>',
+                                 ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_anal/detc': '<pre><h2>_pd_instr_soller_eq_anal/detc</h2> Describes '
                                   'collimation in the equatorial plane (the plane\n'
                                   ' containing the incident and diffracted beams) for\n'
                                   ' the instrument. Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
                                   '       and the monochromator;\n'
@@ -1428,15 +1555,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_mono/spec': '<pre><h2>_pd_instr_soller_eq_mono/spec</h2> Describes '
                                   'collimation in the equatorial plane (the plane\n'
                                   ' containing the incident and diffracted beams) for\n'
                                   ' the instrument. Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
                                   '       and the monochromator;\n'
@@ -1450,15 +1579,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_spec/anal': '<pre><h2>_pd_instr_soller_eq_spec/anal</h2> Describes '
                                   'collimation in the equatorial plane (the plane\n'
                                   ' containing the incident and diffracted beams) for\n'
                                   ' the instrument. Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
                                   '       and the monochromator;\n'
@@ -1472,15 +1603,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_spec/detc': '<pre><h2>_pd_instr_soller_eq_spec/detc</h2> Describes '
                                   'collimation in the equatorial plane (the plane\n'
                                   ' containing the incident and diffracted beams) for\n'
                                   ' the instrument. Values are the maximum divergence angles in\n'
                                   ' degrees, as limited by Soller slits located thus:\n'
                                   '   *_src/mono, collimation between the radiation source\n'
                                   '       and the monochromator;\n'
@@ -1494,15 +1627,17 @@
                                   '       detector;\n'
                                   '   *_spec/detc, collimation between the specimen and the\n'
                                   '       detector.\n'
                                   '\n'
                                   ' Note that *_src/spec is used in place of *_src/mono and \n'
                                   ' *_mono/spec if there is no monochromator in use, and \n'
                                   ' *_spec/detc is used in place of *_spec/anal and \n'
-                                  ' *_anal/detc if there is no analyser in use.</pre>',
+                                  ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_src/mono': '<pre><h2>_pd_instr_soller_eq_src/mono</h2> Describes collimation '
                                  'in the equatorial plane (the plane\n'
                                  ' containing the incident and diffracted beams) for\n'
                                  ' the instrument. Values are the maximum divergence angles in\n'
                                  ' degrees, as limited by Soller slits located thus:\n'
                                  '   *_src/mono, collimation between the radiation source\n'
                                  '       and the monochromator;\n'
@@ -1516,15 +1651,17 @@
                                  '       detector;\n'
                                  '   *_spec/detc, collimation between the specimen and the\n'
                                  '       detector.\n'
                                  '\n'
                                  ' Note that *_src/spec is used in place of *_src/mono and \n'
                                  ' *_mono/spec if there is no monochromator in use, and \n'
                                  ' *_spec/detc is used in place of *_spec/anal and \n'
-                                 ' *_anal/detc if there is no analyser in use.</pre>',
+                                 ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_soller_eq_src/spec': '<pre><h2>_pd_instr_soller_eq_src/spec</h2> Describes collimation '
                                  'in the equatorial plane (the plane\n'
                                  ' containing the incident and diffracted beams) for\n'
                                  ' the instrument. Values are the maximum divergence angles in\n'
                                  ' degrees, as limited by Soller slits located thus:\n'
                                  '   *_src/mono, collimation between the radiation source\n'
                                  '       and the monochromator;\n'
@@ -1538,60 +1675,77 @@
                                  '       detector;\n'
                                  '   *_spec/detc, collimation between the specimen and the\n'
                                  '       detector.\n'
                                  '\n'
                                  ' Note that *_src/spec is used in place of *_src/mono and \n'
                                  ' *_mono/spec if there is no monochromator in use, and \n'
                                  ' *_spec/detc is used in place of *_spec/anal and \n'
-                                 ' *_anal/detc if there is no analyser in use.</pre>',
+                                 ' *_anal/detc if there is no analyser in use.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_source_size_ax': '<pre><h2>_pd_instr_source_size_ax</h2> Axial and equatorial '
                              'intrinsic dimensions\n'
                              ' of the radiation source (in millimetres).\n'
                              ' The perpendicular to the plane containing the incident\n'
-                             ' and scattered beam is the axial (*_ax) direction.</pre>',
+                             ' and scattered beam is the axial (*_ax) direction.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_source_size_eq': '<pre><h2>_pd_instr_source_size_eq</h2> Axial and equatorial '
                              'intrinsic dimensions\n'
                              ' of the radiation source (in millimetres).\n'
                              ' The perpendicular to the plane containing the incident\n'
-                             ' and scattered beam is the axial (*_ax) direction.</pre>',
+                             ' and scattered beam is the axial (*_ax) direction.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_instr_special_details': '<pre><h2>_pd_instr_special_details</h2> A brief description of the '
                               'instrument giving\n'
                               ' details that cannot be given in other\n'
-                              ' _pd_instr_ entries.</pre>',
+                              ' _pd_instr_ entries.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_pd_instr_var_illum_len': '<pre><h2>_pd_instr_var_illum_len</h2> Length of the specimen that is '
                             'illuminated by the radiation\n'
                             ' source (in millimetres) for instruments where\n'
                             ' the illumination length varies with 2\\q (fixed\n'
                             ' divergence slits). The _pd_instr_var_illum_len\n'
                             ' values should be included in the same loop as the\n'
                             ' intensity measurements (_pd_meas_).\n'
                             '\n'
                             ' See _pd_instr_cons_illum_len for instruments where\n'
                             ' the divergence slit is \\q-compensated to yield a\n'
-                            ' constant illumination length.</pre>',
+                            ' constant illumination length.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_meas_2theta_fixed': '<pre><h2>_pd_meas_2theta_fixed</h2> The 2\\q diffraction angle in '
                           'degrees for measurements\n'
                           ' in a white-beam fixed-angle experiment. For measurements\n'
                           ' where 2\\q is scanned, see _pd_meas_2theta_scan or\n'
-                          ' _pd_meas_2theta_range_.</pre>',
+                          ' _pd_meas_2theta_range_.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_2theta_range_inc': '<pre><h2>_pd_meas_2theta_range_inc</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_meas_2theta_scan values for data sets measured with a\n'
-                              ' constant step size.</pre>',
+                              ' constant step size.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_2theta_range_max': '<pre><h2>_pd_meas_2theta_range_max</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_meas_2theta_scan values for data sets measured with a\n'
-                              ' constant step size.</pre>',
+                              ' constant step size.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_2theta_range_min': '<pre><h2>_pd_meas_2theta_range_min</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_meas_2theta_scan values for data sets measured with a\n'
-                              ' constant step size.</pre>',
+                              ' constant step size.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_2theta_scan': '<pre><h2>_pd_meas_2theta_scan</h2> 2\\q diffraction angle (in degrees) '
                          'for intensity\n'
                          ' points measured in a scanning method. The scan method used\n'
                          ' (e.g. continuous or step scan) should be specified in\n'
                          ' the item _pd_meas_scan_method. For fixed 2\\q (white-beam)\n'
                          ' experiments, use _pd_meas_2theta_fixed. In the case of\n'
                          ' continuous-scan data sets, the 2\\q value should be the\n'
@@ -1600,15 +1754,17 @@
                          ' _pd_meas_counts_ items. The 2\\q values should\n'
                          ' not be corrected for nonlinearity,\n'
                          ' zero offset etc. Corrected values may be specified\n'
                          ' using _pd_proc_2theta_corrected.\n'
                          '\n'
                          ' Note that for data sets collected with constant step size,\n'
                          ' _pd_meas_2theta_range_ (*_min, *_max and *_inc) may be\n'
-                         ' used instead of _pd_meas_2theta_scan.</pre>',
+                         ' used instead of _pd_meas_2theta_scan.</pre>\n'
+                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                         '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_[pd]': '<pre><h2>_pd_meas_[pd]</h2> This section contains the measured diffractogram '
                   'and information\n'
                   ' about the conditions used for the measurement of the diffraction \n'
                   ' data set, prior to processing and application of correction\n'
                   ' terms. While additional information may be added to the CIF\n'
                   ' as data are processed and transported between laboratories\n'
                   ' (possibly with the addition of a new _pd_block_id entry), the\n'
@@ -1634,35 +1790,44 @@
                   '    _pd_meas_info_author_address     ?\n'
                   '    _pd_meas_datetime_initiated      1992-03-23T17:20\n'
                   '\n'
                   '    _pd_meas_scan_method             step\n'
                   '    _pd_meas_2theta_range_min        6.0\n'
                   '    _pd_meas_2theta_range_max        164.0\n'
                   '    _pd_meas_2theta_range_inc        0.025\n'
-                  '    _pd_meas_step_count_time         2.0</pre>',
+                  '    _pd_meas_step_count_time         2.0</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_meas_angle_2theta': '<pre><h2>_pd_meas_angle_2theta</h2> The diffractometer angles in '
                           'degrees for an instrument with a\n'
                           ' Euler circle. The definitions for these angles follow the\n'
                           ' convention of International Tables for X-ray Crystallography\n'
-                          ' (1974), Vol. IV, p. 276.</pre>',
+                          ' (1974), Vol. IV, p. 276.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_angle_chi': '<pre><h2>_pd_meas_angle_chi</h2> The diffractometer angles in degrees for '
                        'an instrument with a\n'
                        ' Euler circle. The definitions for these angles follow the\n'
                        ' convention of International Tables for X-ray Crystallography\n'
-                       ' (1974), Vol. IV, p. 276.</pre>',
+                       ' (1974), Vol. IV, p. 276.</pre>\n'
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_angle_omega': '<pre><h2>_pd_meas_angle_omega</h2> The diffractometer angles in degrees '
                          'for an instrument with a\n'
                          ' Euler circle. The definitions for these angles follow the\n'
                          ' convention of International Tables for X-ray Crystallography\n'
-                         ' (1974), Vol. IV, p. 276.</pre>',
+                         ' (1974), Vol. IV, p. 276.</pre>\n'
+                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                         '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_angle_phi': '<pre><h2>_pd_meas_angle_phi</h2> The diffractometer angles in degrees for '
                        'an instrument with a\n'
                        ' Euler circle. The definitions for these angles follow the\n'
                        ' convention of International Tables for X-ray Crystallography\n'
-                       ' (1974), Vol. IV, p. 276.</pre>',
+                       ' (1974), Vol. IV, p. 276.</pre>\n'
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> -180.0:360.0 </p>',
  '_pd_meas_counts_background': '<pre><h2>_pd_meas_counts_background</h2> Counts measured at the '
                                'measurement point as a function of\n'
                                ' angle, time, channel or some other variable (see\n'
                                ' _pd_meas_2theta_ etc.).\n'
                                '\n'
                                ' The defined fields are:\n'
                                '   _pd_meas_counts_total, scattering from the specimen\n'
@@ -1684,15 +1849,17 @@
                                ' Note that counts-per-second values should be converted to\n'
                                ' total counts. If the counting time varies for different\n'
                                ' points, it may be included in the loop using\n'
                                ' _pd_meas_step_count_time.\n'
                                '\n'
                                ' Standard uncertainties should not be quoted for these values.\n'
                                ' If the standard uncertainties differ from the square root of\n'
-                               ' the number of counts, _pd_meas_intensity_ should be used.</pre>',
+                               ' the number of counts, _pd_meas_intensity_ should be used.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_meas_counts_container': '<pre><h2>_pd_meas_counts_container</h2> Counts measured at the '
                               'measurement point as a function of\n'
                               ' angle, time, channel or some other variable (see\n'
                               ' _pd_meas_2theta_ etc.).\n'
                               '\n'
                               ' The defined fields are:\n'
                               '   _pd_meas_counts_total, scattering from the specimen\n'
@@ -1714,15 +1881,17 @@
                               ' Note that counts-per-second values should be converted to\n'
                               ' total counts. If the counting time varies for different\n'
                               ' points, it may be included in the loop using\n'
                               ' _pd_meas_step_count_time.\n'
                               '\n'
                               ' Standard uncertainties should not be quoted for these values.\n'
                               ' If the standard uncertainties differ from the square root of\n'
-                              ' the number of counts, _pd_meas_intensity_ should be used.</pre>',
+                              ' the number of counts, _pd_meas_intensity_ should be used.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_meas_counts_monitor': '<pre><h2>_pd_meas_counts_monitor</h2> Counts measured at the '
                             'measurement point as a function of\n'
                             ' angle, time, channel or some other variable (see\n'
                             ' _pd_meas_2theta_ etc.).\n'
                             '\n'
                             ' The defined fields are:\n'
                             '   _pd_meas_counts_total, scattering from the specimen\n'
@@ -1744,15 +1913,17 @@
                             ' Note that counts-per-second values should be converted to\n'
                             ' total counts. If the counting time varies for different\n'
                             ' points, it may be included in the loop using\n'
                             ' _pd_meas_step_count_time.\n'
                             '\n'
                             ' Standard uncertainties should not be quoted for these values.\n'
                             ' If the standard uncertainties differ from the square root of\n'
-                            ' the number of counts, _pd_meas_intensity_ should be used.</pre>',
+                            ' the number of counts, _pd_meas_intensity_ should be used.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_meas_counts_total': '<pre><h2>_pd_meas_counts_total</h2> Counts measured at the measurement '
                           'point as a function of\n'
                           ' angle, time, channel or some other variable (see\n'
                           ' _pd_meas_2theta_ etc.).\n'
                           '\n'
                           ' The defined fields are:\n'
                           '   _pd_meas_counts_total, scattering from the specimen\n'
@@ -1774,62 +1945,71 @@
                           ' Note that counts-per-second values should be converted to\n'
                           ' total counts. If the counting time varies for different\n'
                           ' points, it may be included in the loop using\n'
                           ' _pd_meas_step_count_time.\n'
                           '\n'
                           ' Standard uncertainties should not be quoted for these values.\n'
                           ' If the standard uncertainties differ from the square root of\n'
-                          ' the number of counts, _pd_meas_intensity_ should be used.</pre>',
+                          ' the number of counts, _pd_meas_intensity_ should be used.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_meas_datetime_initiated': '<pre><h2>_pd_meas_datetime_initiated</h2> The date and time of '
                                 'the data-set measurement. Entries follow\n'
                                 " the standard CIF format 'yyyy-mm-ddThh:mm:ss+zz'. Use\n"
                                 ' of seconds and a time zone is optional, but use of hours\n'
                                 ' and minutes is strongly encouraged. Where possible, give the\n'
                                 ' time when the measurement was started rather than when\n'
                                 ' it was completed.\n'
                                 '\n'
                                 '<h3>Example:</h3>\n'
-                                '1990-07-13T14:40</pre>',
+                                '1990-07-13T14:40</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_detector_id': '<pre><h2>_pd_meas_detector_id</h2> A code or number which identifies the '
                          'measuring detector or\n'
                          ' channel number in a position-sensitive, energy-dispersive\n'
                          ' or other multiple-detector instrument.\n'
                          '\n'
                          ' Calibration information, such as angle offsets or\n'
                          ' a calibration function to convert channel numbers\n'
                          ' to Q, energy, wavelength, angle etc. should\n'
                          ' be described with _pd_calib_ values. If\n'
                          " _pd_calibration_conversion_eqn is used, the detector ID's\n"
-                         ' should be the number to be used in the equation.</pre>',
+                         ' should be the number to be used in the equation.</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_info_author_address': '<pre><h2>_pd_meas_info_author_address</h2> The address of the '
                                  'person who measured the data set. If there\n'
                                  ' is more than one person, this will be looped with\n'
-                                 ' _pd_meas_info_author_name.</pre>',
+                                 ' _pd_meas_info_author_name.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_info_author_email': '<pre><h2>_pd_meas_info_author_email</h2> The e-mail address of the '
                                'person who measured the data set. If\n'
                                ' there is more than one person, this will be looped with\n'
-                               ' _pd_meas_info_author_name.</pre>',
+                               ' _pd_meas_info_author_name.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_info_author_fax': '<pre><h2>_pd_meas_info_author_fax</h2> The fax number of the person '
                              'who measured the data set. If\n'
                              ' there is more than one person, this will be looped with\n'
                              ' _pd_meas_info_author_name. The recommended style is\n'
                              ' the international dialing prefix, followed by the area code in\n'
-                             ' parentheses, followed by the local number with no spaces.</pre>',
+                             ' parentheses, followed by the local number with no spaces.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_info_author_name': '<pre><h2>_pd_meas_info_author_name</h2> The name of the person who '
                               'measured the data set. The family\n'
                               ' name(s), followed by a comma and including any dynastic\n'
                               ' components, precedes the first name(s) or initial(s).\n'
                               ' For more than one person use a loop to specify multiple '
-                              'values.</pre>',
+                              'values.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_info_author_phone': '<pre><h2>_pd_meas_info_author_phone</h2> The telephone number of '
                                'the person who measured the data set.\n'
                                ' If there is more than one person, this will be looped with\n'
                                ' _pd_meas_info_author_name. The recommended style is\n'
                                ' the international dialing prefix, followed by the area code in\n'
-                               ' parentheses, followed by the local number with no spaces.</pre>',
+                               ' parentheses, followed by the local number with no spaces.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_intensity_background': '<pre><h2>_pd_meas_intensity_background</h2> Intensity '
                                   'measurements at the measurement point (see\n'
                                   ' the definition of _pd_meas_2theta_).\n'
                                   '\n'
                                   ' The defined fields are:\n'
                                   '   _pd_meas_intensity_total, scattering from the specimen\n'
                                   '     (with background, specimen mounting or container\n'
@@ -1850,15 +2030,16 @@
                                   ' estimated as the square root of the number of counts).\n'
                                   '\n'
                                   ' Corrections for background, detector dead time etc.,\n'
                                   ' should not have been made to these values. Instead use\n'
                                   ' _pd_proc_intensity_ for corrected diffractograms.\n'
                                   '\n'
                                   ' _pd_meas_units_of_intensity should be used to specify\n'
-                                  ' the units of the intensity measurements.</pre>',
+                                  ' the units of the intensity measurements.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_meas_intensity_container': '<pre><h2>_pd_meas_intensity_container</h2> Intensity '
                                  'measurements at the measurement point (see\n'
                                  ' the definition of _pd_meas_2theta_).\n'
                                  '\n'
                                  ' The defined fields are:\n'
                                  '   _pd_meas_intensity_total, scattering from the specimen\n'
                                  '     (with background, specimen mounting or container\n'
@@ -1878,15 +2059,16 @@
                                  ' estimated as the square root of the number of counts).\n'
                                  '\n'
                                  ' Corrections for background, detector dead time etc.,\n'
                                  ' should not have been made to these values. Instead use\n'
                                  ' _pd_proc_intensity_ for corrected diffractograms.\n'
                                  '\n'
                                  ' _pd_meas_units_of_intensity should be used to specify\n'
-                                 ' the units of the intensity measurements.</pre>',
+                                 ' the units of the intensity measurements.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_meas_intensity_monitor': '<pre><h2>_pd_meas_intensity_monitor</h2> Intensity measurements at '
                                'the measurement point (see\n'
                                ' the definition of _pd_meas_2theta_).\n'
                                '\n'
                                ' The defined fields are:\n'
                                '   _pd_meas_intensity_total, scattering from the specimen\n'
                                '     (with background, specimen mounting or container\n'
@@ -1905,15 +2087,16 @@
                                ' estimated as the square root of the number of counts).\n'
                                '\n'
                                ' Corrections for background, detector dead time etc.,\n'
                                ' should not have been made to these values. Instead use\n'
                                ' _pd_proc_intensity_ for corrected diffractograms.\n'
                                '\n'
                                ' _pd_meas_units_of_intensity should be used to specify\n'
-                               ' the units of the intensity measurements.</pre>',
+                               ' the units of the intensity measurements.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_meas_intensity_total': '<pre><h2>_pd_meas_intensity_total</h2> Intensity measurements at the '
                              'measurement point (see\n'
                              ' the definition of _pd_meas_2theta_).\n'
                              '\n'
                              ' The defined fields are:\n'
                              '   _pd_meas_intensity_total, scattering from the specimen\n'
                              '     (with background, specimen mounting or container\n'
@@ -1932,24 +2115,28 @@
                              ' estimated as the square root of the number of counts).\n'
                              '\n'
                              ' Corrections for background, detector dead time etc.,\n'
                              ' should not have been made to these values. Instead use\n'
                              ' _pd_proc_intensity_ for corrected diffractograms.\n'
                              '\n'
                              ' _pd_meas_units_of_intensity should be used to specify\n'
-                             ' the units of the intensity measurements.</pre>',
+                             ' the units of the intensity measurements.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_meas_number_of_points': '<pre><h2>_pd_meas_number_of_points</h2> The total number of points '
                               'in the measured\n'
-                              ' diffractogram.</pre>',
+                              ' diffractogram.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 1:∞ </p>',
  '_pd_meas_point_id': '<pre><h2>_pd_meas_point_id</h2> Arbitrary label identifying a measured data '
                       'point. Used to\n'
                       ' identify a specific entry in a list of measured intensities.\n'
                       ' The role of this identifier may be adopted by\n'
                       ' _pd_data_point_id if measured, processed and calculated\n'
-                      ' intensity values are combined in a single list.</pre>',
+                      ' intensity values are combined in a single list.</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_position': '<pre><h2>_pd_meas_position</h2> A linear distance in millimetres '
                       'corresponding to the\n'
                       ' location where an intensity measurement is made.\n'
                       ' Used for detectors where a distance measurement is made\n'
                       ' as a direct observable, such as from a microdensitometer\n'
                       ' trace from film or a strip chart recorder. This is an\n'
                       ' alternative to _pd_meas_2theta_scan, which should only be\n'
@@ -1959,28 +2146,32 @@
                       ' be used to record positions.\n'
                       '\n'
                       ' Calibration information, such as angle offsets or a\n'
                       ' function to convert this distance to a 2\\q angle\n'
                       ' or d-space, should be supplied with the _pd_calib_ values.\n'
                       '\n'
                       ' Do not confuse this with the instrument geometry\n'
-                      ' descriptions given by _pd_instr_dist_.</pre>',
+                      ' descriptions given by _pd_instr_dist_.</pre>\n'
+                      '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_meas_rocking_angle': '<pre><h2>_pd_meas_rocking_angle</h2> The angular range in degrees '
                            'through which a sample is rotated\n'
                            ' or oscillated during a measurement step\n'
-                           ' (see _pd_meas_rocking_axis).</pre>',
+                           ' (see _pd_meas_rocking_axis).</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0:360.0 </p>',
  '_pd_meas_rocking_axis': '<pre><h2>_pd_meas_rocking_axis</h2> Description of the axis (or axes) '
                           'used to rotate or rock the\n'
                           ' specimen for better randomization of crystallites\n'
                           ' (see _pd_meas_rocking_angle).\n'
                           '\n'
                           '<h3>Example:</h3>\n'
                           'chi\n'
                           'omega\n'
-                          'phi</pre>',
+                          'phi</pre>\n'
+                          '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_scan_method': '<pre><h2>_pd_meas_scan_method</h2> Code identifying the method for '
                          'scanning reciprocal space.\n'
                          " The designation `fixed' should be used for measurements where\n"
                          ' film, a stationary position-sensitive or area detector\n'
                          ' or other non-moving detection mechanism is used to\n'
                          ' measure diffraction intensities.\n'
                          '\n'
@@ -1995,245 +2186,309 @@
                          '\ttime of flight\n'
                          '\n'
                          'disp\n'
                          '\tenergy dispersive\n'
                          '\n'
                          'fixed\n'
                          '\tstationary detector\n'
-                         '</pre>',
+                         '</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_special_details': '<pre><h2>_pd_meas_special_details</h2> Special details of the '
                              'diffraction measurement process.\n'
                              ' Include information about source instability, degradation etc.\n'
                              ' However, this item should not be used to record information\n'
-                             ' that can be specified in other _pd_meas_ entries.</pre>',
+                             ' that can be specified in other _pd_meas_ entries.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_pd_meas_step_count_time': '<pre><h2>_pd_meas_step_count_time</h2> The count time in seconds for '
                              'each intensity measurement.\n'
                              ' If this value varies for different intensity measurements,\n'
                              ' then this item will be placed in the loop with the\n'
                              ' diffraction measurements. If a single fixed value is used,\n'
-                             ' it may be recorded outside the loop.</pre>',
+                             ' it may be recorded outside the loop.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_meas_time_of_flight': '<pre><h2>_pd_meas_time_of_flight</h2> Measured time in microseconds '
                             'for time-of-flight neutron\n'
                             ' measurements. Note that the flight distance may be\n'
-                            ' specified using _pd_instr_dist_ values.</pre>',
+                            ' specified using _pd_instr_dist_ values.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_meas_units_of_intensity': '<pre><h2>_pd_meas_units_of_intensity</h2> Units for intensity '
                                 'measurements when _pd_meas_intensity_\n'
                                 " is used. Note that use of 'counts' or 'counts per second'\n"
                                 ' here is strongly discouraged: convert the intensity\n'
                                 ' measurements to counts and use _pd_meas_counts_ and\n'
                                 ' _pd_meas_step_count_time instead of _pd_meas_intensity_.\n'
                                 '\n'
                                 '<h3>Example:</h3>\n'
                                 'estimated from strip chart\n'
                                 'arbitrary, from film density\n'
-                                'counts, with automatic dead-time correction applied</pre>',
+                                'counts, with automatic dead-time correction applied</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_peak_2theta_centroid': '<pre><h2>_pd_peak_2theta_centroid</h2> Position of the centroid and '
                              'maximum of a peak as a\n'
-                             ' 2\\q angle in degrees.</pre>',
+                             ' 2\\q angle in degrees.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:180.0 </p>',
  '_pd_peak_2theta_maximum': '<pre><h2>_pd_peak_2theta_maximum</h2> Position of the centroid and '
                             'maximum of a peak as a\n'
-                            ' 2\\q angle in degrees.</pre>',
+                            ' 2\\q angle in degrees.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:180.0 </p>',
  '_pd_peak_[pd]': '<pre><h2>_pd_peak_[pd]</h2> This section contains peak information extracted '
                   'from the\n'
                   ' measured or, if present, the processed diffractogram. Each\n'
                   ' peak in this table will have a unique label (see _pd_peak_id).\n'
                   ' The reflections and phases associated with each peak will be\n'
                   ' specified in other sections (see the _pd_refln_ and\n'
                   ' _pd_phase_ sections).\n'
                   '\n'
                   ' Note that peak positions are customarily determined from the\n'
                   ' processed diffractogram and thus corrections for position\n'
-                  ' and intensity will have been previously applied.</pre>',
+                  ' and intensity will have been previously applied.</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_peak_d_spacing': '<pre><h2>_pd_peak_d_spacing</h2> Peak position as a d-spacing in '
-                       'angstroms.</pre>',
+                       'angstroms.</pre>\n'
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_peak_id': '<pre><h2>_pd_peak_id</h2> An arbitrary code is assigned to each peak. Used to '
                 'link with\n'
                 ' _pd_refln_peak_id so that multiple hkl and/or phase\n'
                 ' identifications can be assigned to a single peak.\n'
                 ' Each peak will have a unique code. In cases\n'
                 ' where two peaks are severely overlapped, it may be\n'
                 ' desirable to list them as a single peak.\n'
                 '\n'
-                ' A peak ID must be included for every peak.</pre>',
+                ' A peak ID must be included for every peak.</pre>\n'
+                '<br><p><h4>Type:</h4> string</p>',
  '_pd_peak_intensity': '<pre><h2>_pd_peak_intensity</h2> Integrated area for the peak, with the '
                        'same scaling as\n'
                        ' the _pd_proc_intensity_ values. It is good practice to\n'
-                       " include s.u.'s for these values.</pre>",
+                       " include s.u.'s for these values.</pre>\n"
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_peak_pk_height': '<pre><h2>_pd_peak_pk_height</h2> The maximum intensity of the peak, either '
                        'extrapolated\n'
                        ' or the highest observed intensity value. The same\n'
                        ' scaling is used for the _pd_proc_intensity_ values.\n'
-                       " It is good practice to include s.u.'s for these values.</pre>",
+                       " It is good practice to include s.u.'s for these values.</pre>\n"
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_peak_special_details': '<pre><h2>_pd_peak_special_details</h2> Detailed description of any '
                              'non-routine processing steps\n'
                              ' used for peak determination or other comments\n'
-                             ' related to the peak table that cannot be given elsewhere.</pre>',
+                             ' related to the peak table that cannot be given elsewhere.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_pd_peak_wavelength_id': '<pre><h2>_pd_peak_wavelength_id</h2> Code identifying the wavelength '
                            'appropriate for this peak\n'
                            ' from the wavelengths in the _diffrn_radiation_ list.\n'
                            ' (See _diffrn_radiation_wavelength_id.) Most commonly used\n'
                            ' to distinguish K\\a~1~ peaks from K\\a~2~ or to designate\n'
                            ' where K\\a~1~ and K\\a~2~ peaks cannot be resolved. For\n'
                            ' complex peak tables with multiple superimposed peaks,\n'
                            ' specify wavelengths in the reflection table using\n'
                            ' _pd_refln_wavelength_id rather than identifying peaks by\n'
-                           ' wavelength.</pre>',
+                           ' wavelength.</pre>\n'
+                           '<br><p><h4>Type:</h4> string</p>',
  '_pd_peak_width_2theta': '<pre><h2>_pd_peak_width_2theta</h2> Peak width as full-width at '
                           'half-maximum expressed as\n'
-                          ' a 2\\q value in degrees.</pre>',
+                          ' a 2\\q value in degrees.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> 0.0:180.0 </p>',
  '_pd_peak_width_d_spacing': '<pre><h2>_pd_peak_width_d_spacing</h2> Peak width as full-width at '
                              'half-maximum expressed as\n'
-                             ' a d-spacing in angstroms.</pre>',
+                             ' a d-spacing in angstroms.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_phase_[pd]': '<pre><h2>_pd_phase_[pd]</h2> This section contains a description of the '
                    'crystalline phases\n'
                    ' contributing to the powder diffraction data set. Note that if\n'
                    ' multiple-phase Rietveld or other structural analysis is\n'
                    ' performed, the structural results will be placed in different\n'
                    ' data blocks, using CIF entries from the core CIF dictionary.\n'
                    '\n'
                    ' The _pd_phase_block_id entry points to the CIF block with\n'
                    ' structural parameters for each crystalline phase. The\n'
                    ' _pd_phase_id serves to link to _pd_refln_phase_id, which is\n'
-                   ' used to label peaks by phase.</pre>',
+                   ' used to label peaks by phase.</pre>\n'
+                   '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_phase_block_id': '<pre><h2>_pd_phase_block_id</h2> A block ID code identifying the phase '
                        'contributing to\n'
                        ' the diffraction peak. The data block containing the\n'
                        ' crystallographic information for this phase will be\n'
                        ' identified with a _pd_block_id code matching the\n'
-                       ' code in _pd_phase_block_id.</pre>',
+                       ' code in _pd_phase_block_id.</pre>\n'
+                       '<br><p><h4>Type:</h4> string</p>',
  '_pd_phase_id': '<pre><h2>_pd_phase_id</h2> A code for each crystal phase used to link with\n'
-                 ' _pd_refln_phase_id.</pre>',
+                 ' _pd_refln_phase_id.</pre>\n'
+                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_phase_mass_%': '<pre><h2>_pd_phase_mass_%</h2> Per cent composition of the specified crystal '
                      'phase\n'
                      ' expressed as the total mass of the component\n'
-                     ' with respect to the total mass of the specimen.</pre>',
+                     ' with respect to the total mass of the specimen.</pre>\n'
+                     '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                     '<br><p><h4>Limits:</h4> 0.0:100.0 </p>',
  '_pd_phase_name': '<pre><h2>_pd_phase_name</h2> The name of the crystal phase identified by '
                    '_pd_phase_id.\n'
-                   ' It may be designated as unknown or by a structure type etc.</pre>',
+                   ' It may be designated as unknown or by a structure type etc.</pre>\n'
+                   '<br><p><h4>Type:</h4> string</p>',
  '_pd_prep_[pd]': '<pre><h2>_pd_prep_[pd]</h2> This section contains descriptive information about '
                   'how the\n'
-                  ' sample was prepared.</pre>',
+                  ' sample was prepared.</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_prep_conditions': '<pre><h2>_pd_prep_conditions</h2> A description of how the material was '
                         'prepared\n'
-                        ' (reaction conditions etc.)</pre>',
+                        ' (reaction conditions etc.)</pre>\n'
+                        '<br><p><h4>Type:</h4> string</p>',
  '_pd_prep_cool_rate': '<pre><h2>_pd_prep_cool_rate</h2> Cooling rate in kelvins per minute for '
                        'samples prepared\n'
                        ' at high temperatures. If the cooling rate is not linear\n'
                        ' or is unknown (e.g. quenched samples), it should be\n'
-                       ' described in _pd_prep_conditions instead.</pre>',
+                       ' described in _pd_prep_conditions instead.</pre>\n'
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_prep_pressure': '<pre><h2>_pd_prep_pressure</h2> Preparation pressure of the sample in '
                       'kilopascals. This\n'
                       ' is particularly important for materials which are metastable\n'
-                      ' at the measurement pressure, _diffrn_ambient_pressure.</pre>',
+                      ' at the measurement pressure, _diffrn_ambient_pressure.</pre>\n'
+                      '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                      '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_prep_temperature': '<pre><h2>_pd_prep_temperature</h2> Preparation temperature of the sample '
                          'in kelvins. This is\n'
                          ' particularly important for materials which are metastable\n'
-                         ' at the measurement temperature, _diffrn_ambient_temperature.</pre>',
+                         ' at the measurement temperature, _diffrn_ambient_temperature.</pre>\n'
+                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                         '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_2theta_corrected': '<pre><h2>_pd_proc_2theta_corrected</h2> The 2\\q diffraction angle '
                               'in degrees of an intensity\n'
                               ' measurement where 2\\q is not constant. Used if\n'
                               ' corrections such as for nonlinearity, zero offset etc.\n'
                               ' have been applied to the _pd_meas_2theta_ values or if\n'
                               ' 2\\q values are computed. If the 2\\q values\n'
                               ' are evenly spaced, _pd_proc_2theta_range_min,\n'
                               ' _pd_proc_2theta_range_max and _pd_proc_2theta_range_inc\n'
-                              ' may be used to specify the 2\\q values.</pre>',
+                              ' may be used to specify the 2\\q values.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_proc_2theta_range_inc': '<pre><h2>_pd_proc_2theta_range_inc</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_proc_2theta_corrected values, or in the case of white-beam\n'
-                              ' experiments it will define the fixed 2\\q value.</pre>',
+                              ' experiments it will define the fixed 2\\q value.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_proc_2theta_range_max': '<pre><h2>_pd_proc_2theta_range_max</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_proc_2theta_corrected values, or in the case of white-beam\n'
-                              ' experiments it will define the fixed 2\\q value.</pre>',
+                              ' experiments it will define the fixed 2\\q value.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_proc_2theta_range_min': '<pre><h2>_pd_proc_2theta_range_min</h2> The range of 2\\q '
                               'diffraction angles in degrees for the\n'
                               ' measurement of intensities. These may be used in place of the\n'
                               ' _pd_proc_2theta_corrected values, or in the case of white-beam\n'
-                              ' experiments it will define the fixed 2\\q value.</pre>',
+                              ' experiments it will define the fixed 2\\q value.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> -180.0:180.0 </p>',
  '_pd_proc_[pd]': '<pre><h2>_pd_proc_[pd]</h2> This section contains the diffraction data set '
                   'after processing\n'
                   ' and application of correction terms. If the data set is\n'
                   ' reprocessed, this section may be replaced (with the addition of\n'
-                  ' a new _pd_block_id entry).</pre>',
+                  ' a new _pd_block_id entry).</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_proc_d_spacing': '<pre><h2>_pd_proc_d_spacing</h2> d-spacing corresponding to an intensity '
                        'point\n'
-                       " from Bragg's law, d = \\l/(2 sin\\q), in units of angstroms.</pre>",
+                       " from Bragg's law, d = \\l/(2 sin\\q), in units of angstroms.</pre>\n"
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_energy_detection': '<pre><h2>_pd_proc_energy_detection</h2> Incident energy in '
                               'electronvolts of the source computed\n'
                               ' from secondary calibration information (time-of-flight\n'
                               ' and synchrotron data).\n'
                               ' Detection energy in electronvolts selected by the analyser,\n'
                               ' if not the same as the incident energy (triple-axis or \n'
                               ' energy-dispersive data). This may be a single value or may \n'
                               ' vary for each data point (triple-axis and time-of-flight '
-                              'data).</pre>',
+                              'data).</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_energy_incident': '<pre><h2>_pd_proc_energy_incident</h2> Incident energy in '
                              'electronvolts of the source computed\n'
                              ' from secondary calibration information (time-of-flight\n'
                              ' and synchrotron data).\n'
                              ' Detection energy in electronvolts selected by the analyser,\n'
                              ' if not the same as the incident energy (triple-axis or \n'
                              ' energy-dispersive data). This may be a single value or may \n'
                              ' vary for each data point (triple-axis and time-of-flight '
-                             'data).</pre>',
+                             'data).</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_info_author_address': '<pre><h2>_pd_proc_info_author_address</h2>  The address of the '
                                  'person who processed the data.\n'
                                  '  If there is more than one person, this will be looped with\n'
-                                 '  _pd_proc_info_author_name.</pre>',
+                                 '  _pd_proc_info_author_name.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_author_email': '<pre><h2>_pd_proc_info_author_email</h2>  The e-mail address of '
                                'the person who processed the\n'
                                '  data.  If there is more than one person, this will be looped\n'
-                               '  with _pd_proc_info_author_name.</pre>',
+                               '  with _pd_proc_info_author_name.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_author_fax': '<pre><h2>_pd_proc_info_author_fax</h2>  The fax number of the person '
                              'who processed the data.\n'
                              '  If there is more than one person, this will be looped with\n'
                              '  _pd_proc_info_author_name. The recommended style is\n'
                              '  the international dialing prefix, followed by the area code in\n'
-                             '  parentheses, followed by the local number with no spaces.</pre>',
+                             '  parentheses, followed by the local number with no spaces.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_author_name': '<pre><h2>_pd_proc_info_author_name</h2>  The name of the person who '
                               'processed the data, if different\n'
                               '  from the person(s) who measured the data set. The family\n'
                               '  name(s), followed by a comma and including any dynastic\n'
                               '  components, precedes the first name(s) or initial(s). For\n'
-                              '  more than one person use a loop to specify multiple values.</pre>',
+                              '  more than one person use a loop to specify multiple '
+                              'values.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_author_phone': '<pre><h2>_pd_proc_info_author_phone</h2>  The telephone number of '
                                'the person who processed the data.\n'
                                '  If there is more than one person, this will be looped\n'
                                '  with _pd_proc_info_author_name. The recommended style is\n'
                                '  the international dialing prefix, followed by the area code in\n'
-                               '  parentheses, followed by the local number with no spaces.</pre>',
+                               '  parentheses, followed by the local number with no spaces.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_data_reduction': '<pre><h2>_pd_proc_info_data_reduction</h2> Description of the '
                                  'processing steps applied in the data-reduction\n'
                                  ' process (background subtraction, \\a-2 stripping, smoothing\n'
-                                 ' etc.). Include details of the program(s) used etc.</pre>',
+                                 ' etc.). Include details of the program(s) used etc.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_datetime': '<pre><h2>_pd_proc_info_datetime</h2> Date(s) and time(s) when the data '
                            'set was processed.\n'
                            ' May be looped if multiple processing steps were used.\n'
                            '\n'
                            ' Dates and times should be specified in the standard CIF\n'
                            " format 'yyyy-mm-ddThh:mm:ss+zz'. Use of seconds and a\n"
                            ' time zone is optional, but use of hours and minutes is\n'
                            ' strongly encouraged.\n'
                            '\n'
                            '<h3>Example:</h3>\n'
-                           '1990-07-13T14:40</pre>',
+                           '1990-07-13T14:40</pre>\n'
+                           '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_excluded_regions': '<pre><h2>_pd_proc_info_excluded_regions</h2> Description of '
                                    'regions in the diffractogram excluded\n'
                                    ' from processing along with a justification of why the\n'
                                    ' data points were not used.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
-                                   '20 to 21 degrees unreliable due to beam dump</pre>',
+                                   '20 to 21 degrees unreliable due to beam dump</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_info_special_details': '<pre><h2>_pd_proc_info_special_details</h2> Detailed '
                                   'description of any non-routine processing steps\n'
                                   ' applied due to any irregularities in this particular data '
-                                  'set.</pre>',
+                                  'set.</pre>\n'
+                                  '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_intensity_bkg_calc': '<pre><h2>_pd_proc_intensity_bkg_calc</h2> _pd_proc_intensity_net '
                                 'contains intensity values for the\n'
                                 ' processed diffractogram for each data point (see\n'
                                 ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                                 ' correction and normalization factors have been applied\n'
                                 ' (in contrast to _pd_meas_counts_ values, which are\n'
                                 ' uncorrected).\n'
@@ -2278,15 +2533,17 @@
                                 ' _pd_proc_intensity_incident values should increase as the\n'
                                 ' incident flux is increased.\n'
                                 '\n'
                                 ' The other normalization factors applied to the data set (for\n'
                                 ' example, Lp corrections, compensation for variation in\n'
                                 ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                                 ' The function should be specified as the one used to divide the\n'
-                                ' measured intensities.</pre>',
+                                ' measured intensities.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_intensity_bkg_fix': '<pre><h2>_pd_proc_intensity_bkg_fix</h2> _pd_proc_intensity_net '
                                'contains intensity values for the\n'
                                ' processed diffractogram for each data point (see\n'
                                ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                                ' correction and normalization factors have been applied\n'
                                ' (in contrast to _pd_meas_counts_ values, which are\n'
                                ' uncorrected).\n'
@@ -2331,15 +2588,17 @@
                                ' _pd_proc_intensity_incident values should increase as the\n'
                                ' incident flux is increased.\n'
                                '\n'
                                ' The other normalization factors applied to the data set (for\n'
                                ' example, Lp corrections, compensation for variation in\n'
                                ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                                ' The function should be specified as the one used to divide the\n'
-                               ' measured intensities.</pre>',
+                               ' measured intensities.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_intensity_incident': '<pre><h2>_pd_proc_intensity_incident</h2> _pd_proc_intensity_net '
                                 'contains intensity values for the\n'
                                 ' processed diffractogram for each data point (see\n'
                                 ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                                 ' correction and normalization factors have been applied\n'
                                 ' (in contrast to _pd_meas_counts_ values, which are\n'
                                 ' uncorrected).\n'
@@ -2384,15 +2643,17 @@
                                 ' _pd_proc_intensity_incident values should increase as the\n'
                                 ' incident flux is increased.\n'
                                 '\n'
                                 ' The other normalization factors applied to the data set (for\n'
                                 ' example, Lp corrections, compensation for variation in\n'
                                 ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                                 ' The function should be specified as the one used to divide the\n'
-                                ' measured intensities.</pre>',
+                                ' measured intensities.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_intensity_net': '<pre><h2>_pd_proc_intensity_net</h2> _pd_proc_intensity_net contains '
                            'intensity values for the\n'
                            ' processed diffractogram for each data point (see\n'
                            ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                            ' correction and normalization factors have been applied\n'
                            ' (in contrast to _pd_meas_counts_ values, which are\n'
                            ' uncorrected).\n'
@@ -2436,15 +2697,17 @@
                            ' _pd_proc_intensity_incident values should increase as the\n'
                            ' incident flux is increased.\n'
                            '\n'
                            ' The other normalization factors applied to the data set (for\n'
                            ' example, Lp corrections, compensation for variation in\n'
                            ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                            ' The function should be specified as the one used to divide the\n'
-                           ' measured intensities.</pre>',
+                           ' measured intensities.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                           '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_intensity_norm': '<pre><h2>_pd_proc_intensity_norm</h2> _pd_proc_intensity_net contains '
                             'intensity values for the\n'
                             ' processed diffractogram for each data point (see\n'
                             ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                             ' correction and normalization factors have been applied\n'
                             ' (in contrast to _pd_meas_counts_ values, which are\n'
                             ' uncorrected).\n'
@@ -2488,15 +2751,17 @@
                             ' _pd_proc_intensity_incident values should increase as the\n'
                             ' incident flux is increased.\n'
                             '\n'
                             ' The other normalization factors applied to the data set (for\n'
                             ' example, Lp corrections, compensation for variation in\n'
                             ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                             ' The function should be specified as the one used to divide the\n'
-                            ' measured intensities.</pre>',
+                            ' measured intensities.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                            '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_intensity_total': '<pre><h2>_pd_proc_intensity_total</h2> _pd_proc_intensity_net '
                              'contains intensity values for the\n'
                              ' processed diffractogram for each data point (see\n'
                              ' _pd_proc_2theta_, _pd_proc_wavelength etc.) after\n'
                              ' correction and normalization factors have been applied\n'
                              ' (in contrast to _pd_meas_counts_ values, which are\n'
                              ' uncorrected).\n'
@@ -2540,27 +2805,30 @@
                              ' _pd_proc_intensity_incident values should increase as the\n'
                              ' incident flux is increased.\n'
                              '\n'
                              ' The other normalization factors applied to the data set (for\n'
                              ' example, Lp corrections, compensation for variation in\n'
                              ' counting time) may be specified in _pd_proc_intensity_norm.\n'
                              ' The function should be specified as the one used to divide the\n'
-                             ' measured intensities.</pre>',
+                             ' measured intensities.</pre>\n'
+                             '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                             '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_ls_[pd]': '<pre><h2>_pd_proc_ls_[pd]</h2> This section is used to define parameters '
                      'relevant to a\n'
                      ' least-squares fit to a powder diffractogram, using a Rietveld\n'
                      ' or other full-profile (e.g. Pawley or Le Bail methods) fit.\n'
                      '\n'
                      ' Note that values in this section refer to full-pattern fitting.\n'
                      ' Use the appropriate items for single-crystal analyses from the\n'
                      ' core CIF dictionary for structure refinements using diffraction\n'
                      ' intensities estimated from a powder diffractogram by \n'
                      ' pattern-decomposition methods. Also note that many entries in \n'
                      ' the core _refine_ls_ entries may also be useful (for example\n'
-                     ' _refine_ls_shift/su_*).</pre>',
+                     ' _refine_ls_shift/su_*).</pre>\n'
+                     '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_proc_ls_background_function': '<pre><h2>_pd_proc_ls_background_function</h2> Description of '
                                     'the background treatment mechanism used to\n'
                                     ' fit the data set.\n'
                                     '\n'
                                     ' For refinements where the background is computed as a\n'
                                     ' function that is fitted to minimize the difference between \n'
                                     ' the observed and calculated patterns, it is\n'
@@ -2581,31 +2849,34 @@
                                     ' extrapolation method (linear extrapolation, spline etc.).\n'
                                     ' _pd_proc_ls_background_function should also indicate how '
                                     'the\n'
                                     ' points were determined (automatically, by visual estimation\n'
                                     ' etc.) and whether the values were refined to improve the\n'
                                     ' agreement. The extrapolated background intensity value for\n'
                                     ' each data point should be specified in\n'
-                                    ' _pd_proc_intensity_bkg_calc.</pre>',
+                                    ' _pd_proc_intensity_bkg_calc.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_ls_peak_cutoff': '<pre><h2>_pd_proc_ls_peak_cutoff</h2> Describes where peak-intensity '
                             'computation is\n'
                             ' discontinued as a fraction of the intensity of the\n'
                             ' peak at maximum. Thus for a value of 0.005, the\n'
                             ' tails of a diffraction peak are neglected\n'
                             ' after the intensity has dropped below 0.5% of the\n'
-                            ' diffraction intensity at the maximum.</pre>',
+                            ' diffraction intensity at the maximum.</pre>\n'
+                            '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_pd_proc_ls_pref_orient_corr': '<pre><h2>_pd_proc_ls_pref_orient_corr</h2> Description of the '
                                  'preferred-orientation correction if\n'
                                  ' such a correction is used. Omitting this entry\n'
                                  ' implies that no preferred-orientation correction\n'
                                  ' has been used. If a function form is used, it is\n'
                                  ' recommended that the actual equation in TeX, or a\n'
                                  ' programming language, is used to specify the function as\n'
                                  ' well as a giving a description. Include the value(s) used \n'
-                                 " for the correction with s.u.'s.</pre>",
+                                 " for the correction with s.u.'s.</pre>\n"
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_ls_prof_R_factor': '<pre><h2>_pd_proc_ls_prof_R_factor</h2> Rietveld/profile fit R '
                               'factors.\n'
                               '\n'
                               ' Note that the R factor computed for Rietveld refinements\n'
                               ' using the extracted reflection intensity values (often\n'
                               ' called the Rietveld or Bragg R factor, R~B~) is not properly\n'
                               ' a profile R factor. This R factor may be specified using\n'
@@ -2650,15 +2921,17 @@
                               '          point with background and other corrections\n'
                               '          applied to match the scale of the observed data set,\n'
                               '          sometimes referred to as y~i~(calc) or\n'
                               '          y~ci~. (See _pd_calc_intensity_total.)\n'
                               '     n is the total number of data points (see\n'
                               '          _pd_proc_number_of_points) less the number of\n'
                               '          data points excluded from the refinement.\n'
-                              '     p is the total number of refined parameters.</pre>',
+                              '     p is the total number of refined parameters.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_ls_prof_wR_expected': '<pre><h2>_pd_proc_ls_prof_wR_expected</h2> Rietveld/profile fit '
                                  'R factors.\n'
                                  '\n'
                                  ' Note that the R factor computed for Rietveld refinements\n'
                                  ' using the extracted reflection intensity values (often\n'
                                  ' called the Rietveld or Bragg R factor, R~B~) is not properly\n'
                                  ' a profile R factor. This R factor may be specified using\n'
@@ -2705,15 +2978,17 @@
                                  '          point with background and other corrections\n'
                                  '          applied to match the scale of the observed data set,\n'
                                  '          sometimes referred to as y~i~(calc) or\n'
                                  '          y~ci~. (See _pd_calc_intensity_total.)\n'
                                  '     n is the total number of data points (see\n'
                                  '          _pd_proc_number_of_points) less the number of\n'
                                  '          data points excluded from the refinement.\n'
-                                 '     p is the total number of refined parameters.</pre>',
+                                 '     p is the total number of refined parameters.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_ls_prof_wR_factor': '<pre><h2>_pd_proc_ls_prof_wR_factor</h2> Rietveld/profile fit R '
                                'factors.\n'
                                '\n'
                                ' Note that the R factor computed for Rietveld refinements\n'
                                ' using the extracted reflection intensity values (often\n'
                                ' called the Rietveld or Bragg R factor, R~B~) is not properly\n'
                                ' a profile R factor. This R factor may be specified using\n'
@@ -2759,104 +3034,125 @@
                                '          point with background and other corrections\n'
                                '          applied to match the scale of the observed data set,\n'
                                '          sometimes referred to as y~i~(calc) or\n'
                                '          y~ci~. (See _pd_calc_intensity_total.)\n'
                                '     n is the total number of data points (see\n'
                                '          _pd_proc_number_of_points) less the number of\n'
                                '          data points excluded from the refinement.\n'
-                               '     p is the total number of refined parameters.</pre>',
+                               '     p is the total number of refined parameters.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                               '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_ls_profile_function': '<pre><h2>_pd_proc_ls_profile_function</h2> Description of the '
                                  'profile function used to\n'
                                  ' fit the data set. If a function form is used, it is\n'
                                  ' recommended that the actual equation in TeX, or a\n'
                                  ' programming language, is used to specify the function as\n'
                                  ' well as giving a description. Include the values used \n'
-                                 " for the profile-function coefficients and their s.u.'s.</pre>",
+                                 " for the profile-function coefficients and their s.u.'s.</pre>\n"
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_ls_special_details': '<pre><h2>_pd_proc_ls_special_details</h2> Additional '
                                 'characterization information relevant to\n'
                                 ' non-routine steps used for refinement of a structural model\n'
-                                ' that cannot be specified elsewhere.</pre>',
+                                ' that cannot be specified elsewhere.</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_ls_weight': '<pre><h2>_pd_proc_ls_weight</h2> Weight applied to each profile point. '
                        'These values\n'
                        ' may be omitted if the weights are 1/u^2^, where\n'
                        ' u is the s.u. for the _pd_proc_intensity_net values.\n'
                        '\n'
                        ' A weight value of zero is used to indicate a data\n'
                        ' point not used for refinement (see\n'
-                       ' _pd_proc_info_excluded_regions).</pre>',
+                       ' _pd_proc_info_excluded_regions).</pre>\n'
+                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                       '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_pd_proc_number_of_points': '<pre><h2>_pd_proc_number_of_points</h2> The total number of data '
-                              'points in the processed diffractogram.</pre>',
+                              'points in the processed diffractogram.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 1:∞ </p>',
  '_pd_proc_point_id': '<pre><h2>_pd_proc_point_id</h2> Arbitrary label identifying a processed '
                       'data point. Used to\n'
                       ' identify a specific entry in a list of processed intensities.\n'
                       ' The role of this identifier may be adopted by\n'
                       ' _pd_data_point_id if measured, processed and calculated\n'
                       ' intensity values are combined in a single list, or by\n'
                       ' _pd_meas_point_id if measured and processed lists are\n'
-                      ' combined.</pre>',
+                      ' combined.</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_proc_recip_len_Q': '<pre><h2>_pd_proc_recip_len_Q</h2> Length in reciprocal space (|Q|= '
                          '2\\p/d) corresponding to\n'
-                         ' an intensity point. Units are inverse angstroms.</pre>',
+                         ' an intensity point. Units are inverse angstroms.</pre>\n'
+                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                         '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_proc_wavelength': '<pre><h2>_pd_proc_wavelength</h2> Wavelength in angstroms for the '
                         'incident radiation as\n'
                         ' computed from secondary calibration information. This will\n'
                         ' be most appropriate for time-of-flight and synchrotron\n'
                         ' measurements. This will be a single value for\n'
                         ' continuous-wavelength methods or may vary for each data point\n'
                         ' and be looped with the intensity values for energy-dispersive\n'
-                        ' measurements.</pre>',
+                        ' measurements.</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                        '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_refln_[pd]': '<pre><h2>_pd_refln_[pd]</h2> This section provides a mechanism to identify '
                    'each peak in the\n'
                    ' peak-table section (_pd_peak_) with the phase(s) (_pd_phase_id)\n'
                    ' and the reflection indices (_refln_index_) associated with the\n'
                    ' peak.  There are no restrictions on the number of phases or\n'
                    ' reflections associated with an observed peak. Reflections may\n'
                    " also be included that are not observed; use '.' for the\n"
-                   ' _pd_refln_peak_id.</pre>',
+                   ' _pd_refln_peak_id.</pre>\n'
+                   '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_refln_peak_id': '<pre><h2>_pd_refln_peak_id</h2> Code which identifies the powder '
                       'diffraction peak that\n'
                       ' contains the current reflection. This code must match a\n'
-                      ' _pd_peak_id code.</pre>',
+                      ' _pd_peak_id code.</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_refln_phase_id': '<pre><h2>_pd_refln_phase_id</h2> Code which identifies the crystal phase '
                        'associated with this\n'
-                       ' reflection. This code must match a _pd_phase_id code.</pre>',
+                       ' reflection. This code must match a _pd_phase_id code.</pre>\n'
+                       '<br><p><h4>Type:</h4> string</p>',
  '_pd_refln_wavelength_id': '<pre><h2>_pd_refln_wavelength_id</h2> Code which identifies the '
                             'wavelength associated with the\n'
                             ' reflection and the peak pointed to by _pd_refln_peak_id.\n'
-                            ' This code must match a _diffrn_radiation_wavelength_id code.</pre>',
+                            ' This code must match a _diffrn_radiation_wavelength_id code.</pre>\n'
+                            '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_[pd]': '<pre><h2>_pd_spec_[pd]</h2> This section contains information about the '
                   'specimen used\n'
                   ' for measurement of the diffraction data set. Note that \n'
                   ' information about the sample (the batch of material from which \n'
                   ' the specimen was obtained) is specified in _pd_prep_.\n'
                   '\n'
                   '<h3>Example:</h3>\n'
                   '\n'
                   '    _pd_spec_mounting               ?\n'
                   '    _pd_spec_mount_mode             transmission\n'
                   '    _pd_spec_orientation            horizontal\n'
-                  '    _pd_spec_preparation            ?</pre>',
+                  '    _pd_spec_preparation            ?</pre>\n'
+                  '<br><p><h4>Type:</h4> ? (unknown)</p>',
  '_pd_spec_description': '<pre><h2>_pd_spec_description</h2>  A description of the specimen, such '
                          'as the source of the\n'
-                         '  specimen, identification of standards, mixtures etc.</pre>',
+                         '  specimen, identification of standards, mixtures etc.</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_mount_mode': '<pre><h2>_pd_spec_mount_mode</h2> A code describing the beam path through '
                         'the specimen.\n'
                         '\n'
                         '<h3>Example:</h3>\n'
                         'reflection\n'
-                        'transmission</pre>',
+                        'transmission</pre>\n'
+                        '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_mounting': '<pre><h2>_pd_spec_mounting</h2> A description of how the specimen is '
                       'mounted.\n'
                       '\n'
                       '<h3>Example:</h3>\n'
                       'vanadium can with He exchange gas\n'
                       'quartz capillary\n'
                       'packed powder pellet\n'
                       'drifted powder on off-cut Si\n'
-                      'drifted powder on Kapton film</pre>',
+                      'drifted powder on Kapton film</pre>\n'
+                      '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_orientation': '<pre><h2>_pd_spec_orientation</h2> The orientation of the \\w (\\q) and '
                          '2\\q axis.\n'
                          ' Note that this axis is parallel to the specimen axial axis\n'
                          ' and perpendicular to the plane containing the incident and\n'
                          ' scattered beams.\n'
                          '\n'
                          ' Thus for a horizontal orientation, scattering\n'
@@ -2867,55 +3163,65 @@
                          " is perpendicular to the ground). `Both' is appropriate for\n"
                          ' experiments where measurements are made in both planes,\n'
                          ' for example using two-dimensional detectors.\n'
                          '\n'
                          '<h3>Example:</h3>\n'
                          'horizontal\n'
                          'vertical\n'
-                         'both</pre>',
+                         'both</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_preparation': '<pre><h2>_pd_spec_preparation</h2> A description of the preparation '
                          'steps for producing the\n'
                          ' diffraction specimen from the sample. Include any procedures\n'
                          ' related to grinding, sieving, spray drying etc. For\n'
                          ' information relevant to how the sample is synthesized, use\n'
                          ' the _pd_prep_ entries.\n'
                          '\n'
                          '<h3>Example:</h3>\n'
                          'wet grinding in acetone\n'
                          'sieved through a 44 micron (325 mesh/inch) sieve\n'
-                         'spray dried in water with 1% clay</pre>',
+                         'spray dried in water with 1% clay</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_shape': '<pre><h2>_pd_spec_shape</h2> A code describing the specimen shape.\n'
                    '\n'
                    '<h3>Example:</h3>\n'
                    'cylinder\n'
                    'flat_sheet\n'
-                   'irregular</pre>',
+                   'irregular</pre>\n'
+                   '<br><p><h4>Type:</h4> string</p>',
  '_pd_spec_size_axial': '<pre><h2>_pd_spec_size_axial</h2> The size of the specimen in three '
                         'mutually perpendicular\n'
                         ' directions in millimetres.\n'
                         ' The perpendicular to the plane containing the incident\n'
                         ' and scattered beam is the *_axial direction.\n'
                         ' In transmission geometry, the scattering vector is parallel\n'
                         ' to *_equat and in reflection geometry the scattering vector is\n'
                         ' parallel to *_thick.\n'
-                        '</pre>',
+                        '</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                        '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_spec_size_equat': '<pre><h2>_pd_spec_size_equat</h2> The size of the specimen in three '
                         'mutually perpendicular\n'
                         ' directions in millimetres.\n'
                         ' The perpendicular to the plane containing the incident\n'
                         ' and scattered beam is the *_axial direction.\n'
                         ' In transmission geometry, the scattering vector is parallel\n'
                         ' to *_equat and in reflection geometry the scattering vector is\n'
                         ' parallel to *_thick.\n'
-                        '</pre>',
+                        '</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                        '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_spec_size_thick': '<pre><h2>_pd_spec_size_thick</h2> The size of the specimen in three '
                         'mutually perpendicular\n'
                         ' directions in millimetres.\n'
                         ' The perpendicular to the plane containing the incident\n'
                         ' and scattered beam is the *_axial direction.\n'
                         ' In transmission geometry, the scattering vector is parallel\n'
                         ' to *_equat and in reflection geometry the scattering vector is\n'
                         ' parallel to *_thick.\n'
-                        '</pre>',
+                        '</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                        '<br><p><h4>Limits:</h4> 0.0:∞ </p>',
  '_pd_spec_special_details': '<pre><h2>_pd_spec_special_details</h2> Descriptive information about '
                              'the specimen that cannot be\n'
-                             ' included in other data items.</pre>'}
+                             ' included in other data items.</pre>\n'
+                             '<br><p><h4>Type:</h4> string</p>'}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finalcif-136/finalcif/cif/reference.py` & `finalcif-137/finalcif/cif/reference.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/restraints_dict.py` & `finalcif-137/finalcif/cif/restraints_dict.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 restraints_dict = {'_restr_U_iso_atom_site_label': '<pre><h2>_restr_U_iso_atom_site_label</h2> Label of the atom '
                                  'whose atomic displacement parameters\n'
-                                 ' are restrained.</pre>',
+                                 ' are restrained.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_iso_weight_param': '<pre><h2>_restr_U_iso_weight_param</h2> The expectation value of '
                               'the difference between\n'
                               ' the refined and the isotropic equivalent of the\n'
                               ' anisotropic atomic displacement parameters.\n'
-                              ' The default value of zero indicates a constraint.</pre>',
+                              ' The default value of zero indicates a constraint.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_U_rigid_U_parallel': '<pre><h2>_restr_U_rigid_U_parallel</h2> The average value of the '
                               'components parallel to the bond\n'
                               ' of the atomic displacement parameters of the two atoms\n'
-                              ' that define the bond.</pre>',
+                              ' that define the bond.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_U_rigid_atom_site_label_1': '<pre><h2>_restr_U_rigid_atom_site_label_1</h2> The atom-site '
-                                     'labels of the two atoms that define the rigid bond.</pre>',
+                                     'labels of the two atoms that define the rigid bond.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_rigid_atom_site_label_2': '<pre><h2>_restr_U_rigid_atom_site_label_2</h2> The atom-site '
-                                     'labels of the two atoms that define the rigid bond.</pre>',
+                                     'labels of the two atoms that define the rigid bond.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_rigid_details': '<pre><h2>_restr_U_rigid_details</h2> Free-text information about the '
-                           'rigid-bond restraint.</pre>',
+                           'rigid-bond restraint.</pre>\n'
+                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_rigid_diff': '<pre><h2>_restr_U_rigid_diff</h2> The difference between the components '
                         'along the bond direction\n'
-                        ' of the atomic displacement parameters, U, of the two atoms.</pre>',
+                        ' of the atomic displacement parameters, U, of the two atoms.</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_U_rigid_site_symmetry_1': '<pre><h2>_restr_U_rigid_site_symmetry_1</h2> The site '
                                    'symmetries of the two atoms that define the rigid bond.\n'
                                    '\n'
                                    ' The symmetry code of each atom site is given as the \n'
                                    "\t       symmetry-equivalent position number 'n' and the \n"
                                    "\t       cell translation number 'klm'. These numbers are \n"
                                    '\t       combined to form the code n_klm. The character '
@@ -45,15 +53,17 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_U_rigid_site_symmetry_2': '<pre><h2>_restr_U_rigid_site_symmetry_2</h2> The site '
                                    'symmetries of the two atoms that define the rigid bond.\n'
                                    '\n'
                                    ' The symmetry code of each atom site is given as the \n'
                                    "\t       symmetry-equivalent position number 'n' and the \n"
                                    "\t       cell translation number 'klm'. These numbers are \n"
                                    '\t       combined to form the code n_klm. The character '
@@ -76,65 +86,78 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_U_rigid_target_weight_param': '<pre><h2>_restr_U_rigid_target_weight_param</h2>        '
                                        'The weighting parameter = sqrt(1/weight).\n'
                                        '         The expectation value of the difference between '
                                        'the components\n'
                                        '         of the atomic displacement parameter, U,\n'
                                        '         along the bond direction of the two atoms that '
                                        'define the bond.\n'
                                        '         This number is used to assign a weight during '
                                        'refinement.\n'
                                        '         A value of zero causes the restraint to become a '
                                        'constraint.\n'
-                                       '         This item has a default value of zero.</pre>',
+                                       '         This item has a default value of zero.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_U_similar_atom_site_label_1': '<pre><h2>_restr_U_similar_atom_site_label_1</h2> '
                                        '_restr_U_similar_atom_site_label_1 is the atom-site label '
                                        'of  \n'
                                        ' the atom whose atomic displacement parameters are used \n'
                                        '\t       as the target. _restr_U_similar_atom_site_label_2 '
                                        'is the \n'
                                        '\t       atom-site label of the atom whose atomic '
                                        'displacement \n'
                                        '\t       parameters are restrained to be the same as atom '
-                                       '1.</pre>',
+                                       '1.</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_similar_atom_site_label_2': '<pre><h2>_restr_U_similar_atom_site_label_2</h2> '
                                        '_restr_U_similar_atom_site_label_1 is the atom-site label '
                                        'of  \n'
                                        ' the atom whose atomic displacement parameters are used \n'
                                        '\t       as the target. _restr_U_similar_atom_site_label_2 '
                                        'is the \n'
                                        '\t       atom-site label of the atom whose atomic '
                                        'displacement \n'
                                        '\t       parameters are restrained to be the same as atom '
-                                       '1.</pre>',
+                                       '1.</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>',
  '_restr_U_similar_weight_param': '<pre><h2>_restr_U_similar_weight_param</h2> The expectation '
                                   'value of the difference between the\n'
                                   ' anisotropic atomic displacement parameters\n'
                                   ' of the two atoms.\n'
-                                  ' The default value of zero represents a constraint.</pre>',
+                                  ' The default value of zero represents a constraint.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                  '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_angle_atom_site_label_1': '<pre><h2>_restr_angle_atom_site_label_1</h2> The atom-site '
                                    'labels used to define the angle. Atom 2\n'
-                                   ' is at the apex of the angle.</pre>',
+                                   ' is at the apex of the angle.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_restr_angle_atom_site_label_2': '<pre><h2>_restr_angle_atom_site_label_2</h2> The atom-site '
                                    'labels used to define the angle. Atom 2\n'
-                                   ' is at the apex of the angle.</pre>',
+                                   ' is at the apex of the angle.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_restr_angle_atom_site_label_3': '<pre><h2>_restr_angle_atom_site_label_3</h2> The atom-site '
                                    'labels used to define the angle. Atom 2\n'
-                                   ' is at the apex of the angle.</pre>',
+                                   ' is at the apex of the angle.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_restr_angle_details': '<pre><h2>_restr_angle_details</h2> A free-text description of the '
-                         'restraint.</pre>',
+                         'restraint.</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_angle_diff': '<pre><h2>_restr_angle_diff</h2> The difference between the target and the '
-                      'refined angle.</pre>',
+                      'refined angle.</pre>\n'
+                      '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                      '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_angle_site_symmetry_1': '<pre><h2>_restr_angle_site_symmetry_1</h2> The symmetry '
                                  'transformation needed to generate the coordinates\n'
                                  ' of the three atoms that define the angle.\n'
                                  '\n'
                                  ' The symmetry code of each atom site is given as the \n'
                                  "\t       symmetry-equivalent position number 'n' and the cell \n"
                                  "\t       translation number 'klm'. These numbers are combined \n"
@@ -155,15 +178,17 @@
                                  '      m = 5 + z\n'
                                  ' By adding 5 to the translations, the use of negative numbers\n'
                                  ' is avoided.\n'
                                  '\n'
                                  '<h3>Example:</h3>\n'
                                  'None\n'
                                  '4\n'
-                                 '7_645</pre>',
+                                 '7_645</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>\n'
+                                 '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_angle_site_symmetry_2': '<pre><h2>_restr_angle_site_symmetry_2</h2> The symmetry '
                                  'transformation needed to generate the coordinates\n'
                                  ' of the three atoms that define the angle.\n'
                                  '\n'
                                  ' The symmetry code of each atom site is given as the \n'
                                  "\t       symmetry-equivalent position number 'n' and the cell \n"
                                  "\t       translation number 'klm'. These numbers are combined \n"
@@ -184,15 +209,17 @@
                                  '      m = 5 + z\n'
                                  ' By adding 5 to the translations, the use of negative numbers\n'
                                  ' is avoided.\n'
                                  '\n'
                                  '<h3>Example:</h3>\n'
                                  'None\n'
                                  '4\n'
-                                 '7_645</pre>',
+                                 '7_645</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>\n'
+                                 '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_angle_site_symmetry_3': '<pre><h2>_restr_angle_site_symmetry_3</h2> The symmetry '
                                  'transformation needed to generate the coordinates\n'
                                  ' of the three atoms that define the angle.\n'
                                  '\n'
                                  ' The symmetry code of each atom site is given as the \n'
                                  "\t       symmetry-equivalent position number 'n' and the cell \n"
                                  "\t       translation number 'klm'. These numbers are combined \n"
@@ -213,37 +240,47 @@
                                  '      m = 5 + z\n'
                                  ' By adding 5 to the translations, the use of negative numbers\n'
                                  ' is avoided.\n'
                                  '\n'
                                  '<h3>Example:</h3>\n'
                                  'None\n'
                                  '4\n'
-                                 '7_645</pre>',
+                                 '7_645</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>\n'
+                                 '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_angle_target': '<pre><h2>_restr_angle_target</h2> The expectation angle defined by the '
                         'three atoms.\n'
-                        ' This is the target angle for the restrained refinement.</pre>',
+                        ' This is the target angle for the restrained refinement.</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                        '<br><p><h4>Limits:</h4> 0:180 </p>',
  '_restr_angle_target_weight_param': '<pre><h2>_restr_angle_target_weight_param</h2> Weighting '
                                      'parameter = sqrt(1/weight).\n'
                                      ' It is the expectation value of the difference between\n'
                                      ' the refined value and the target.\n'
                                      ' If this parameter is set to zero, the angle will be '
                                      'constrained\n'
                                      ' to refine to the target value.\n'
                                      ' If this item is absent, its value will be taken as zero\n'
-                                     ' and the distance will be constrained.</pre>',
+                                     ' and the distance will be constrained.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                     '<br><p><h4>Limits:</h4> 0:180 </p>',
  '_restr_distance_atom_site_label_1': '<pre><h2>_restr_distance_atom_site_label_1</h2> The '
                                       'atom-site labels of the two atoms defining\n'
-                                      ' the distance restrained.</pre>',
+                                      ' the distance restrained.</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_atom_site_label_2': '<pre><h2>_restr_distance_atom_site_label_2</h2> The '
                                       'atom-site labels of the two atoms defining\n'
-                                      ' the distance restrained.</pre>',
+                                      ' the distance restrained.</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_details': '<pre><h2>_restr_distance_details</h2> A free-text description of the '
-                            'restraint.</pre>',
+                            'restraint.</pre>\n'
+                            '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_diff': '<pre><h2>_restr_distance_diff</h2> The difference between the target and '
-                         'the refined distance.</pre>',
+                         'the refined distance.</pre>\n'
+                         '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_min_A': '<pre><h2>_restr_distance_min_A</h2> The weight associated with the '
                           'difference between the\n'
                           ' refined distance D and the prescribed minimum distance\n'
                           ' (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -253,15 +290,17 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0.  In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target distance\n'
-                          ' of F so as to avoid division by zero.</pre>',
+                          ' of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_distance_min_B': '<pre><h2>_restr_distance_min_B</h2> The weight associated with the '
                           'difference between the\n'
                           ' refined distance D and the prescribed minimum distance\n'
                           ' (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -271,15 +310,17 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0. In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target\n'
-                          ' distance of F so as to avoid division by zero.</pre>',
+                          ' distance of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_distance_min_C': '<pre><h2>_restr_distance_min_C</h2> The weight associated with the '
                           'difference between the\n'
                           ' refined distance D and the prescribed minimum distance\n'
                           ' (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -289,15 +330,16 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0.  In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target\n'
-                          ' distance of F so as to avoid division by zero.</pre>',
+                          ' distance of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_min_E': '<pre><h2>_restr_distance_min_E</h2> The weight associated with the '
                           'difference between the\n'
                           ' refined distance D and the prescribed minimum distance\n'
                           ' (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -307,15 +349,16 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0.  In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target\n'
-                          ' distance of F so as to avoid division by zero.</pre>',
+                          ' distance of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_min_F': '<pre><h2>_restr_distance_min_F</h2> The weight associated with the '
                           'difference between the\n'
                           ' refined distance D and the prescribed minimum distance\n'
                           ' (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -325,15 +368,17 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0.  In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target\n'
-                          ' distance of F so as to avoid division by zero.</pre>',
+                          ' distance of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                          '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_distance_min_G': '<pre><h2>_restr_distance_min_G</h2> The weight associated with the '
                           'difference between\n'
                           ' the refined distance D and the prescribed minimum\n'
                           ' distance (B or F) is given by the expression\n'
                           '\n'
                           ' w = A*(B/D)^C^ + E*exp((D-F)/G)\n'
                           '\n'
@@ -343,31 +388,38 @@
                           '\n'
                           ' If A=0, B and C are undefined; if E=0, F and G are undefined.\n'
                           '\n'
                           ' A hard-sphere contact can be generated by setting E=1,\n'
                           ' F=prescribed minimum distance and G=0.  In this case G\n'
                           ' (combined with a non-zero E) should be treated as a flag\n'
                           ' indicating a hard-sphere interaction with a target\n'
-                          ' distance of F so as to avoid division by zero.</pre>',
+                          ' distance of F so as to avoid division by zero.</pre>\n'
+                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_min_atom_site_label_1': '<pre><h2>_restr_distance_min_atom_site_label_1</h2> The '
                                           'atom-site labels for the two atoms that are kept '
-                                          'apart.</pre>',
+                                          'apart.</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_min_atom_site_label_2': '<pre><h2>_restr_distance_min_atom_site_label_2</h2> The '
                                           'atom-site labels for the two atoms that are kept '
-                                          'apart.</pre>',
+                                          'apart.</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_min_details': '<pre><h2>_restr_distance_min_details</h2> A text description of '
                                 'the restraint giving details not\n'
-                                ' given elsewhere.</pre>',
+                                ' given elsewhere.</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_min_difference': '<pre><h2>_restr_distance_min_difference</h2> The difference in '
                                    'angstroms between the refined distance\n'
                                    ' of approach of the two atoms and the target distance B or F:\n'
                                    '\n'
-                                   ' difference = D - B or D - F</pre>',
+                                   ' difference = D - B or D - F</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_min_distance': '<pre><h2>_restr_distance_min_distance</h2> The refined distance, '
-                                 'D, between the two atoms.</pre>',
+                                 'D, between the two atoms.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_distance_min_site_symmetry_1': '<pre><h2>_restr_distance_min_site_symmetry_1</h2> The '
                                         'site symmetries of the two atoms kept apart.\n'
                                         '\n'
                                         ' The symmetry code of each atom site is given as the \n'
                                         "\t       symmetry-equivalent position number 'n' and the "
                                         'cell \n'
                                         "\t       translation number 'klm'. These numbers are "
@@ -391,15 +443,16 @@
                                         ' the atoms that are kept apart.  These translations\n'
                                         ' (x,y,z) are related to (k,l,m) by the relations\n'
                                         '      k = 5 + x\n'
                                         '      l = 5 + y\n'
                                         '      m = 5 + z\n'
                                         ' By adding 5 to the translations, the use of negative '
                                         'numbers\n'
-                                        ' is avoided.</pre>',
+                                        ' is avoided.</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_min_site_symmetry_2': '<pre><h2>_restr_distance_min_site_symmetry_2</h2> The '
                                         'site symmetries of the two atoms kept apart.\n'
                                         '\n'
                                         ' The symmetry code of each atom site is given as the \n'
                                         "\t       symmetry-equivalent position number 'n' and the "
                                         'cell \n'
                                         "\t       translation number 'klm'. These numbers are "
@@ -423,15 +476,16 @@
                                         ' the atoms that are kept apart.  These translations\n'
                                         ' (x,y,z) are related to (k,l,m) by the relations\n'
                                         '      k = 5 + x\n'
                                         '      l = 5 + y\n'
                                         '      m = 5 + z\n'
                                         ' By adding 5 to the translations, the use of negative '
                                         'numbers\n'
-                                        ' is avoided.</pre>',
+                                        ' is avoided.</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>',
  '_restr_distance_site_symmetry_1': '<pre><h2>_restr_distance_site_symmetry_1</h2> The symmetry '
                                     'transformation needed to generate the coordinates\n'
                                     ' of the two atoms that define the distance.\n'
                                     '\n'
                                     ' The symmetry code of each atom site is given as the \n'
                                     "\t       symmetry-equivalent position number 'n' and the "
                                     'cell \n'
@@ -459,15 +513,17 @@
                                     ' By adding 5 to the translations, the use of negative '
                                     'numbers\n'
                                     ' is avoided.\n'
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_645</pre>',
+                                    '7_645</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>\n'
+                                    '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_distance_site_symmetry_2': '<pre><h2>_restr_distance_site_symmetry_2</h2> The symmetry '
                                     'transformation needed to generate the coordinates\n'
                                     ' of the two atoms that define the distance.\n'
                                     '\n'
                                     ' The symmetry code of each atom site is given as the \n'
                                     "\t       symmetry-equivalent position number 'n' and the "
                                     'cell \n'
@@ -495,72 +551,93 @@
                                     ' By adding 5 to the translations, the use of negative '
                                     'numbers\n'
                                     ' is avoided.\n'
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_645</pre>',
+                                    '7_645</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>\n'
+                                    '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_distance_target': '<pre><h2>_restr_distance_target</h2> The expectation distance between '
                            'the two atoms.\n'
-                           ' This is the target distance for the restrained refinement.</pre>',
+                           ' This is the target distance for the restrained refinement.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_distance_target_weight_param': '<pre><h2>_restr_distance_target_weight_param</h2> '
                                         'Weighting parameter = sqrt(1/weight).\n'
                                         ' It is the expectation value of the difference between\n'
                                         ' the refined value and the target.\n'
                                         ' If this parameter is set to zero, the distance will be\n'
                                         ' constrained to refine to the target value.\n'
                                         ' If this item is absent, its value will be taken as zero\n'
-                                        ' and the distance will be constrained.</pre>',
+                                        ' and the distance will be constrained.</pre>\n'
+                                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_equal_angle_atom_site_label_1': '<pre><h2>_restr_equal_angle_atom_site_label_1</h2> The '
                                          'atom-site labels of the three atoms that define one of\n'
                                          ' the angles restrained to be equal to other angles in\n'
-                                         ' the same class.</pre>',
+                                         ' the same class.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_angle_atom_site_label_2': '<pre><h2>_restr_equal_angle_atom_site_label_2</h2> The '
                                          'atom-site labels of the three atoms that define one of\n'
                                          ' the angles restrained to be equal to other angles in\n'
-                                         ' the same class.</pre>',
+                                         ' the same class.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_angle_atom_site_label_3': '<pre><h2>_restr_equal_angle_atom_site_label_3</h2> The '
                                          'atom-site labels of the three atoms that define one of\n'
                                          ' the angles restrained to be equal to other angles in\n'
-                                         ' the same class.</pre>',
+                                         ' the same class.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_angle_class_average': '<pre><h2>_restr_equal_angle_class_average</h2> The average '
                                      'angle in the class of angles restrained to\n'
-                                     ' be the same after refinement.</pre>',
+                                     ' be the same after refinement.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                     '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_angle_class_class_id': '<pre><h2>_restr_equal_angle_class_class_id</h2> A character '
                                       'string that identifies the class of angles\n'
-                                      ' whose properties are described.</pre>',
+                                      ' whose properties are described.</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>\n'
+                                      '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_angle_class_detail': '<pre><h2>_restr_equal_angle_class_detail</h2> A text '
                                     'description giving details of the class of angles that\n'
-                                    ' are restrained to be equal.</pre>',
+                                    ' are restrained to be equal.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_angle_class_diff_max': '<pre><h2>_restr_equal_angle_class_diff_max</h2> The maximum '
                                       'deviation of an angle in the class from the\n'
-                                      ' class average after refinement.</pre>',
+                                      ' class average after refinement.</pre>\n'
+                                      '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                      '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_angle_class_esd': '<pre><h2>_restr_equal_angle_class_esd</h2> The actual estimated '
                                  'standard deviation of the angles in the\n'
                                  ' class from their average after refinement.\n'
                                  ' This number is expected to be similar to the value set for\n'
-                                 ' _restr_equal_angle_class_target_weight_param.</pre>',
+                                 ' _restr_equal_angle_class_target_weight_param.</pre>\n'
+                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                 '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_angle_class_id': '<pre><h2>_restr_equal_angle_class_id</h2> A character string '
                                 'identifying the class of equal angles\n'
-                                ' to which this angle belongs.</pre>',
+                                ' to which this angle belongs.</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>\n'
+                                '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_angle_class_target_weight_param': '<pre><h2>_restr_equal_angle_class_target_weight_param</h2> '
                                                  'The weighting parameter = sqrt(1/weight).\n'
                                                  ' The expectation value of the estimated standard '
                                                  'deviation of\n'
                                                  ' the angles in the class from their average '
                                                  'after refinement.\n'
                                                  ' This value determines the weight assigned to '
                                                  'the restraint.\n'
                                                  ' If it is zero the angles are constrained to be '
                                                  'equal.\n'
-                                                 ' The default value is zero.</pre>',
+                                                 ' The default value is zero.</pre>\n'
+                                                 '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                                 '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_angle_detail': '<pre><h2>_restr_equal_angle_detail</h2> A text description giving '
                               'details of an angle in\n'
-                              ' a class of angles that are restrained to be equal.</pre>',
+                              ' a class of angles that are restrained to be equal.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_angle_site_symmetry_1': '<pre><h2>_restr_equal_angle_site_symmetry_1</h2> The site '
                                        'symmetries of the three atoms that define an angle\n'
                                        ' restrained to be equal to other angles in the same '
                                        'class.\n'
                                        '\n'
                                        ' The symmetry code of each atom site is given as the \n'
                                        "\t       symmetry-equivalent position number 'n' and the "
@@ -592,15 +669,17 @@
                                        ' By adding 5 to the translations, the use of negative '
                                        'numbers\n'
                                        ' is avoided.\n'
                                        '\n'
                                        '<h3>Example:</h3>\n'
                                        'None\n'
                                        '4\n'
-                                       '7_645</pre>',
+                                       '7_645</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>\n'
+                                       '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_angle_site_symmetry_2': '<pre><h2>_restr_equal_angle_site_symmetry_2</h2> The site '
                                        'symmetries of the three atoms that define an angle\n'
                                        ' restrained to be equal to other angles in the same '
                                        'class.\n'
                                        '\n'
                                        ' The symmetry code of each atom site is given as the \n'
                                        "\t       symmetry-equivalent position number 'n' and the "
@@ -632,15 +711,17 @@
                                        ' By adding 5 to the translations, the use of negative '
                                        'numbers\n'
                                        ' is avoided.\n'
                                        '\n'
                                        '<h3>Example:</h3>\n'
                                        'None\n'
                                        '4\n'
-                                       '7_645</pre>',
+                                       '7_645</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>\n'
+                                       '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_angle_site_symmetry_3': '<pre><h2>_restr_equal_angle_site_symmetry_3</h2> The site '
                                        'symmetries of the three atoms that define an angle\n'
                                        ' restrained to be equal to other angles in the same '
                                        'class.\n'
                                        '\n'
                                        ' The symmetry code of each atom site is given as the \n'
                                        "\t       symmetry-equivalent position number 'n' and the "
@@ -672,62 +753,81 @@
                                        ' By adding 5 to the translations, the use of negative '
                                        'numbers\n'
                                        ' is avoided.\n'
                                        '\n'
                                        '<h3>Example:</h3>\n'
                                        'None\n'
                                        '4\n'
-                                       '7_645</pre>',
+                                       '7_645</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>\n'
+                                       '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_distance_atom_site_label_1': '<pre><h2>_restr_equal_distance_atom_site_label_1</h2> '
                                             'The atom-site labels of the two atoms that define one '
                                             'of the\n'
                                             ' distances restrained to be equal to other distances '
                                             'in\n'
-                                            ' the same class.</pre>',
+                                            ' the same class.</pre>\n'
+                                            '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_distance_atom_site_label_2': '<pre><h2>_restr_equal_distance_atom_site_label_2</h2> '
                                             'The atom-site labels of the two atoms that define one '
                                             'of the\n'
                                             ' distances restrained to be equal to other distances '
                                             'in\n'
-                                            ' the same class.</pre>',
+                                            ' the same class.</pre>\n'
+                                            '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_distance_class_average': '<pre><h2>_restr_equal_distance_class_average</h2> The '
                                         'average distance in the class of distances restrained to\n'
-                                        ' be the same after refinement.</pre>',
+                                        ' be the same after refinement.</pre>\n'
+                                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                        '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_distance_class_class_id': '<pre><h2>_restr_equal_distance_class_class_id</h2> A '
                                          'character string that identifies the class of distances\n'
-                                         ' whose properties are described.</pre>',
+                                         ' whose properties are described.</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>\n'
+                                         '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_distance_class_details': '<pre><h2>_restr_equal_distance_class_details</h2> A text '
                                         'description giving details of the class of distances '
                                         'that\n'
-                                        ' are restrained to be equal.</pre>',
+                                        ' are restrained to be equal.</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_distance_class_diff_max': '<pre><h2>_restr_equal_distance_class_diff_max</h2> The '
                                          'maximum deviation of a distance in the class from the\n'
-                                         ' class average after refinement.</pre>',
+                                         ' class average after refinement.</pre>\n'
+                                         '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                         '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_distance_class_esd': '<pre><h2>_restr_equal_distance_class_esd</h2> The actual '
                                     'estimated standard deviation of the distances in the\n'
                                     ' class from their average after refinement.\n'
                                     ' This number is expected to be similar to the value set for\n'
-                                    ' _restr_equal_distance_class_target_weight_param.</pre>',
+                                    ' _restr_equal_distance_class_target_weight_param.</pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                    '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_distance_class_id': '<pre><h2>_restr_equal_distance_class_id</h2> A character '
                                    'string identifying the class of equal distances\n'
-                                   ' to which this distance belongs.</pre>',
+                                   ' to which this distance belongs.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_distance_class_target_weight_param': '<pre><h2>_restr_equal_distance_class_target_weight_param</h2> '
                                                     'The weighting parameter = sqrt(1/weight).\n'
                                                     ' The expectation value of the estimated '
                                                     'standard deviation of the\n'
                                                     ' distances in the class from their average '
                                                     'after refinement.\n'
                                                     ' This value determines the weight assigned to '
                                                     'the restraint.\n'
                                                     ' If it is zero the distances are constrained '
                                                     'to be equal.\n'
-                                                    ' The default value is zero.</pre>',
+                                                    ' The default value is zero.</pre>\n'
+                                                    '<br><p><h4>Type:</h4> number (int or '
+                                                    'float)</p>\n'
+                                                    '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_distance_details': '<pre><h2>_restr_equal_distance_details</h2> A text description '
                                   'giving details of a distance in\n'
-                                  ' a class of distances that are restrained to be equal.</pre>',
+                                  ' a class of distances that are restrained to be equal.</pre>\n'
+                                  '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_distance_site_symmetry_1': '<pre><h2>_restr_equal_distance_site_symmetry_1</h2> The '
                                           'site symmetries of the two atoms that define a '
                                           'distance\n'
                                           ' restrained to be equal to other distances in the same\n'
                                           ' class.\n'
                                           '\n'
                                           ' The symmetry code of each atom site is given as the \n'
@@ -761,15 +861,17 @@
                                           ' By adding 5 to the translations, the use of negative '
                                           'numbers\n'
                                           ' is avoided.\n'
                                           '\n'
                                           '<h3>Example:</h3>\n'
                                           'None\n'
                                           '4\n'
-                                          '7_645</pre>',
+                                          '7_645</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>\n'
+                                          '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_distance_site_symmetry_2': '<pre><h2>_restr_equal_distance_site_symmetry_2</h2> The '
                                           'site symmetries of the two atoms that define a '
                                           'distance\n'
                                           ' restrained to be equal to other distances in the same\n'
                                           ' class.\n'
                                           '\n'
                                           ' The symmetry code of each atom site is given as the \n'
@@ -803,93 +905,114 @@
                                           ' By adding 5 to the translations, the use of negative '
                                           'numbers\n'
                                           ' is avoided.\n'
                                           '\n'
                                           '<h3>Example:</h3>\n'
                                           'None\n'
                                           '4\n'
-                                          '7_645</pre>',
+                                          '7_645</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>\n'
+                                          '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_torsion_atom_site_label_1': '<pre><h2>_restr_equal_torsion_atom_site_label_1</h2> '
                                            'The atom-site labels of the four atoms that define one '
                                            'of the\n'
                                            ' torsion angles restrained to be equal to other '
                                            'torsion\n'
                                            ' angles in the same class.  The torsion angle is the '
                                            'dihedral\n'
                                            ' angle between the plane defined by atoms 1, 2 and 3, '
                                            'and\n'
-                                           ' the plane defined by atoms 2, 3 and 4.</pre>',
+                                           ' the plane defined by atoms 2, 3 and 4.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_atom_site_label_2': '<pre><h2>_restr_equal_torsion_atom_site_label_2</h2> '
                                            'The atom-site labels of the four atoms that define one '
                                            'of the\n'
                                            ' torsion angles restrained to be equal to other '
                                            'torsion\n'
                                            ' angles in the same class.  The torsion angle is the '
                                            'dihedral\n'
                                            ' angle between the plane defined by atoms 1, 2 and 3, '
                                            'and\n'
-                                           ' the plane defined by atoms 2, 3 and 4.</pre>',
+                                           ' the plane defined by atoms 2, 3 and 4.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_atom_site_label_3': '<pre><h2>_restr_equal_torsion_atom_site_label_3</h2> '
                                            'The atom-site labels of the four atoms that define one '
                                            'of the\n'
                                            ' torsion angles restrained to be equal to other '
                                            'torsion\n'
                                            ' angles in the same class.  The torsion angle is the '
                                            'dihedral\n'
                                            ' angle between the plane defined by atoms 1, 2 and 3, '
                                            'and\n'
-                                           ' the plane defined by atoms 2, 3 and 4.</pre>',
+                                           ' the plane defined by atoms 2, 3 and 4.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_atom_site_label_4': '<pre><h2>_restr_equal_torsion_atom_site_label_4</h2> '
                                            'The atom-site labels of the four atoms that define one '
                                            'of the\n'
                                            ' torsion angles restrained to be equal to other '
                                            'torsion\n'
                                            ' angles in the same class.  The torsion angle is the '
                                            'dihedral\n'
                                            ' angle between the plane defined by atoms 1, 2 and 3, '
                                            'and\n'
-                                           ' the plane defined by atoms 2, 3 and 4.</pre>',
+                                           ' the plane defined by atoms 2, 3 and 4.</pre>\n'
+                                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_class_average': '<pre><h2>_restr_equal_torsion_class_average</h2> The '
                                        'average torsion angle in the class of torsion angles\n'
-                                       ' restrained to be the same after refinement.</pre>',
+                                       ' restrained to be the same after refinement.</pre>\n'
+                                       '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                       '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_torsion_class_class_id': '<pre><h2>_restr_equal_torsion_class_class_id</h2> A '
                                         'character string that identifies the class of torsion\n'
-                                        ' angles whose properties are described.</pre>',
+                                        ' angles whose properties are described.</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>\n'
+                                        '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_torsion_class_details': '<pre><h2>_restr_equal_torsion_class_details</h2> A text '
                                        'description giving details of the class of torsion\n'
-                                       ' angles that are restrained to be equal.</pre>',
+                                       ' angles that are restrained to be equal.</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_class_diff_max': '<pre><h2>_restr_equal_torsion_class_diff_max</h2> The '
                                         'maximum deviation of a torsion angle in the class\n'
-                                        ' from the class average after refinement.</pre>',
+                                        ' from the class average after refinement.</pre>\n'
+                                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                        '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_torsion_class_esd': '<pre><h2>_restr_equal_torsion_class_esd</h2> The actual '
                                    'estimated standard deviation of the torsion\n'
                                    ' angles in the class from their average after refinement.\n'
                                    ' This number is expected to be similar to the value set for\n'
-                                   ' _restr_equal_torsion_class_target_weight_param.</pre>',
+                                   ' _restr_equal_torsion_class_target_weight_param.</pre>\n'
+                                   '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                   '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_torsion_class_id': '<pre><h2>_restr_equal_torsion_class_id</h2> A character string '
                                   'identifying the class of equal torsion\n'
-                                  ' angles to which this torsion angle belongs.</pre>',
+                                  ' angles to which this torsion angle belongs.</pre>\n'
+                                  '<br><p><h4>Type:</h4> string</p>\n'
+                                  '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_equal_torsion_class_target_weight_param': '<pre><h2>_restr_equal_torsion_class_target_weight_param</h2> '
                                                    'The weighting parameter = sqrt(1/weight).\n'
                                                    ' This is the expectation value of the '
                                                    'estimated\n'
                                                    ' standard deviation (given in '
                                                    '_restr_equal_torsion_class_esd)\n'
                                                    ' of the torsion angles in the class from '
                                                    'their\n'
                                                    ' average after refinement.\n'
                                                    ' This value determines the weight assigned to '
                                                    'the target.\n'
                                                    ' If it is zero the torsion angles are '
                                                    'constrained to be equal.\n'
-                                                   ' The default value is zero.</pre>',
+                                                   ' The default value is zero.</pre>\n'
+                                                   '<br><p><h4>Type:</h4> number (int or '
+                                                   'float)</p>\n'
+                                                   '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_equal_torsion_details': '<pre><h2>_restr_equal_torsion_details</h2> A text description '
                                  'giving details of a torsion angle in\n'
                                  ' a class of torsion angles that are restrained to be '
-                                 'equal.</pre>',
+                                 'equal.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_restr_equal_torsion_site_symmetry_1': '<pre><h2>_restr_equal_torsion_site_symmetry_1</h2> The '
                                          'site symmetries of the four atoms that define a torsion '
                                          'angle\n'
                                          ' restrained to be equal to other torsion angles in the\n'
                                          ' same class.\n'
                                          '\n'
                                          ' The symmetry code of each atom site is given as the \n'
@@ -923,15 +1046,17 @@
                                          ' By adding 5 to the translations, the use of negative '
                                          'numbers\n'
                                          ' is avoided.\n'
                                          '\n'
                                          '<h3>Example:</h3>\n'
                                          'None\n'
                                          '4\n'
-                                         '7_645</pre>',
+                                         '7_645</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>\n'
+                                         '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_torsion_site_symmetry_2': '<pre><h2>_restr_equal_torsion_site_symmetry_2</h2> The '
                                          'site symmetries of the four atoms that define a torsion '
                                          'angle\n'
                                          ' restrained to be equal to other torsion angles in the\n'
                                          ' same class.\n'
                                          '\n'
                                          ' The symmetry code of each atom site is given as the \n'
@@ -965,15 +1090,17 @@
                                          ' By adding 5 to the translations, the use of negative '
                                          'numbers\n'
                                          ' is avoided.\n'
                                          '\n'
                                          '<h3>Example:</h3>\n'
                                          'None\n'
                                          '4\n'
-                                         '7_645</pre>',
+                                         '7_645</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>\n'
+                                         '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_torsion_site_symmetry_3': '<pre><h2>_restr_equal_torsion_site_symmetry_3</h2> The '
                                          'site symmetries of the four atoms that define a torsion '
                                          'angle\n'
                                          ' restrained to be equal to other torsion angles in the\n'
                                          ' same class.\n'
                                          '\n'
                                          ' The symmetry code of each atom site is given as the \n'
@@ -1007,15 +1134,17 @@
                                          ' By adding 5 to the translations, the use of negative '
                                          'numbers\n'
                                          ' is avoided.\n'
                                          '\n'
                                          '<h3>Example:</h3>\n'
                                          'None\n'
                                          '4\n'
-                                         '7_645</pre>',
+                                         '7_645</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>\n'
+                                         '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_equal_torsion_site_symmetry_4': '<pre><h2>_restr_equal_torsion_site_symmetry_4</h2> The '
                                          'site symmetries of the four atoms that define a torsion '
                                          'angle\n'
                                          ' restrained to be equal to other torsion angles in the\n'
                                          ' same class.\n'
                                          '\n'
                                          ' The symmetry code of each atom site is given as the \n'
@@ -1049,27 +1178,37 @@
                                          ' By adding 5 to the translations, the use of negative '
                                          'numbers\n'
                                          ' is avoided.\n'
                                          '\n'
                                          '<h3>Example:</h3>\n'
                                          'None\n'
                                          '4\n'
-                                         '7_645</pre>',
+                                         '7_645</pre>\n'
+                                         '<br><p><h4>Type:</h4> string</p>\n'
+                                         '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_parameter_atom_coefficient': '<pre><h2>_restr_parameter_atom_coefficient</h2> A parameter '
                                       'that scales the quantity being restrained.\n'
                                       ' It can be used to convert a constraint on occupancy to\n'
-                                      ' a constraint on ionic charge.</pre>',
+                                      ' a constraint on ionic charge.</pre>\n'
+                                      '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                      '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_parameter_atom_site_label': '<pre><h2>_restr_parameter_atom_site_label</h2> The atom-site '
-                                     'label for an atom in this class.</pre>',
+                                     'label for an atom in this class.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_parameter_class_class_id': '<pre><h2>_restr_parameter_class_class_id</h2> The class ID of '
-                                    'the restraint described in this category.</pre>',
+                                    'the restraint described in this category.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>\n'
+                                    '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_parameter_class_details': '<pre><h2>_restr_parameter_class_details</h2> A text '
-                                   'description of the restraint.</pre>',
+                                   'description of the restraint.</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>',
  '_restr_parameter_class_id': '<pre><h2>_restr_parameter_class_id</h2> The identifier of the class '
-                              'of restraint applied to the atoms.</pre>',
+                              'of restraint applied to the atoms.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>\n'
+                              '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_parameter_class_parameter_type': '<pre><h2>_restr_parameter_class_parameter_type</h2> A '
                                           'flag that indicates the nature of the value\n'
                                           ' that is being restrained.\n'
                                           '\n'
                                           '<h3>Example:</h3>\n'
                                           'occupancy\n'
                                           '\t_atom_site_occupancy\n'
@@ -1078,51 +1217,65 @@
                                           '\t_atom_site_fract_x\n'
                                           '\n'
                                           'position_y\n'
                                           '\t_atom_site_fract_y\n'
                                           '\n'
                                           'position_z\n'
                                           '\t_atom_site_fract_z\n'
-                                          '</pre>',
+                                          '</pre>\n'
+                                          '<br><p><h4>Type:</h4> string</p>',
  '_restr_parameter_class_target': '<pre><h2>_restr_parameter_class_target</h2> The target value '
                                   'for the sum of values of the appropriate\n'
-                                  ' parameter type multiplied by the _*_target_weight_param.</pre>',
+                                  ' parameter type multiplied by the '
+                                  '_*_target_weight_param.</pre>\n'
+                                  '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_parameter_class_target_weight_param': '<pre><h2>_restr_parameter_class_target_weight_param</h2> '
                                                'Weighting parameter = sqrt(1/weight).\n'
                                                ' It is the expectation value of the difference '
                                                'between\n'
                                                ' the refined value of the '
                                                'sum(parameter*coefficient)\n'
                                                ' and the _*_target.\n'
                                                ' If this parameter is set to zero, the sum will be '
                                                'constrained\n'
                                                ' to refine to the target value.\n'
                                                ' If this item is absent, its value will be taken '
                                                'as zero\n'
-                                               ' and the distance will be constrained.</pre>',
+                                               ' and the distance will be constrained.</pre>\n'
+                                               '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_parameter_id': '<pre><h2>_restr_parameter_id</h2> A unique identifier for each line in a '
-                        'loop.</pre>',
+                        'loop.</pre>\n'
+                        '<br><p><h4>Type:</h4> string</p>',
  '_restr_plane_atom_site_label': '<pre><h2>_restr_plane_atom_site_label</h2> An atom-site label of '
-                                 'one of the atoms that form the plane.</pre>',
+                                 'one of the atoms that form the plane.</pre>\n'
+                                 '<br><p><h4>Type:</h4> string</p>',
  '_restr_plane_class_class_id': '<pre><h2>_restr_plane_class_class_id</h2>       The class '
-                                'identifier for the plane whose properties are described.</pre>',
+                                'identifier for the plane whose properties are described.</pre>\n'
+                                '<br><p><h4>Type:</h4> string</p>\n'
+                                '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_plane_class_details': '<pre><h2>_restr_plane_class_details</h2>        Text describing '
-                               'any special features of the restraint.</pre>',
+                               'any special features of the restraint.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>',
  '_restr_plane_class_displacement_esd': '<pre><h2>_restr_plane_class_displacement_esd</h2> The '
                                         'observed estimated standard deviation of the\n'
-                                        ' atoms from this plane.</pre>',
+                                        ' atoms from this plane.</pre>\n'
+                                        '<br><p><h4>Type:</h4> string</p>\n'
+                                        '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_plane_class_displacement_max': '<pre><h2>_restr_plane_class_displacement_max</h2> The '
                                         'distance in angstroms from the plane to the atom '
                                         'furthest\n'
-                                        ' removed from the plane.</pre>',
+                                        ' removed from the plane.</pre>\n'
+                                        '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                        '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_plane_class_displacement_max_atom_site_label': '<pre><h2>_restr_plane_class_displacement_max_atom_site_label</h2> '
                                                         'The atom-site label of the atom that lies '
                                                         'furthest\n'
                                                         ' from the plane defined by this '
-                                                        'class.</pre>',
+                                                        'class.</pre>\n'
+                                                        '<br><p><h4>Type:</h4> string</p>',
  '_restr_plane_class_displacement_max_site_symmetry': '<pre><h2>_restr_plane_class_displacement_max_site_symmetry</h2> '
                                                       'The site symmetry of the atom lying '
                                                       'furthest from the plane\n'
                                                       ' to which it is restrained.\n'
                                                       '\n'
                                                       ' The symmetry code of each atom site is '
                                                       'given as the \n'
@@ -1157,25 +1310,34 @@
                                                       ' By adding 5 to the translations, the use '
                                                       'of negative numbers\n'
                                                       ' is avoided.\n'
                                                       '\n'
                                                       '<h3>Example:</h3>\n'
                                                       'None\n'
                                                       '4\n'
-                                                      '7_645</pre>',
+                                                      '7_645</pre>\n'
+                                                      '<br><p><h4>Type:</h4> string</p>\n'
+                                                      '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_plane_class_id': '<pre><h2>_restr_plane_class_id</h2> A character string that identifies '
                           'the plane\n'
-                          ' to which this atom is constrained.</pre>',
+                          ' to which this atom is constrained.</pre>\n'
+                          '<br><p><h4>Type:</h4> string</p>\n'
+                          '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_plane_details': '<pre><h2>_restr_plane_details</h2> A text string giving details not '
-                         'described elsewhere.</pre>',
+                         'described elsewhere.</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_plane_displacement': '<pre><h2>_restr_plane_displacement</h2> The distance between this '
                               'atom and the best plane through\n'
-                              ' all the atoms.</pre>',
+                              ' all the atoms.</pre>\n'
+                              '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                              '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_plane_id': '<pre><h2>_restr_plane_id</h2> A unique identifier for each line in the '
-                    'list.</pre>',
+                    'list.</pre>\n'
+                    '<br><p><h4>Type:</h4> string</p>\n'
+                    '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_plane_site_symmetry': '<pre><h2>_restr_plane_site_symmetry</h2> The site symmetry of the '
                                'atom that helps to define the plane\n'
                                ' to which it is restrained.\n'
                                '\n'
                                ' The symmetry code of each atom site is given as the \n'
                                "\t       symmetry-equivalent position number 'n' and the cell \n"
                                "\t       translation number 'klm'. These numbers are combined \n"
@@ -1196,36 +1358,48 @@
                                '      m = 5 + z\n'
                                ' By adding 5 to the translations, the use of negative numbers\n'
                                ' is avoided.\n'
                                '\n'
                                '<h3>Example:</h3>\n'
                                'None\n'
                                '4\n'
-                               '7_645</pre>',
+                               '7_645</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>\n'
+                               '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_plane_target_weight_param': '<pre><h2>_restr_plane_target_weight_param</h2> The weighting '
                                      'parameter = sqrt(1/weight).\n'
                                      ' The expectation value of the distance in angstroms\n'
                                      ' between this atom and the best plane through all\n'
-                                     ' the atoms of the class.</pre>',
+                                     ' the atoms of the class.</pre>\n'
+                                     '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                     '<br><p><h4>Limits:</h4> 0:∞ </p>',
  '_restr_rigid_body_atom_site_label': '<pre><h2>_restr_rigid_body_atom_site_label</h2> The '
-                                      'atom-site labels of an atom in a rigid body.</pre>',
+                                      'atom-site labels of an atom in a rigid body.</pre>\n'
+                                      '<br><p><h4>Type:</h4> string</p>',
  '_restr_rigid_body_class_class_id': '<pre><h2>_restr_rigid_body_class_class_id</h2> A character '
                                      'string that identifies the rigid body.\n'
                                      ' It must match one of the values of '
-                                     '_restr_rigid_body_class_id.</pre>',
+                                     '_restr_rigid_body_class_id.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>\n'
+                                     '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_rigid_body_class_details': '<pre><h2>_restr_rigid_body_class_details</h2> A text '
-                                    'description giving details of a rigid body.</pre>',
+                                    'description giving details of a rigid body.</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>',
  '_restr_rigid_body_class_id': '<pre><h2>_restr_rigid_body_class_id</h2> A character string '
-                               'identifying a rigid body.</pre>',
+                               'identifying a rigid body.</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>\n'
+                               '<br><p><h4>Default:</h4> 1 </p>',
  '_restr_rigid_body_details': '<pre><h2>_restr_rigid_body_details</h2> A text description giving '
                               'details of a rigid body in\n'
-                              ' a class of rigid bodies that are constrained to be equal.</pre>',
+                              ' a class of rigid bodies that are constrained to be equal.</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_restr_rigid_body_id': '<pre><h2>_restr_rigid_body_id</h2> A unique identifier for each atom in '
                          'the list of atoms in the\n'
-                         ' RESTR_RIGID_BODY category.</pre>',
+                         ' RESTR_RIGID_BODY category.</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_restr_rigid_body_site_symmetry': '<pre><h2>_restr_rigid_body_site_symmetry</h2> The site '
                                     'symmetry of an atom in a rigid body.\n'
                                     '\n'
                                     ' The symmetry code of each atom site is given as the \n'
                                     "\t       symmetry-equivalent position number 'n' and the "
                                     'cell \n'
                                     "\t       translation number 'klm'. These numbers are "
@@ -1252,45 +1426,56 @@
                                     ' By adding 5 to the translations, the use of negative '
                                     'numbers\n'
                                     ' is avoided.\n'
                                     '\n'
                                     '<h3>Example:</h3>\n'
                                     'None\n'
                                     '4\n'
-                                    '7_645</pre>',
+                                    '7_645</pre>\n'
+                                    '<br><p><h4>Type:</h4> string</p>\n'
+                                    '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_special_details': '<pre><h2>_restr_special_details</h2> Text describing any restraint or '
                            'constraint that cannot be\n'
                            ' described using any of the the other restraint items.\n'
-                           ' See also _atom_site_restraints.</pre>',
+                           ' See also _atom_site_restraints.</pre>\n'
+                           '<br><p><h4>Type:</h4> string</p>',
  '_restr_torsion_angle_target': '<pre><h2>_restr_torsion_angle_target</h2> The angle in degrees to '
                                 'which the torsion angle is restrained.\n'
                                 ' The torsion angle is the dihedral angle between the plane '
                                 'defined\n'
                                 ' by atoms 1, 2 and 3, and the plane defined by atoms 2, 3 and '
-                                '4.</pre>',
+                                '4.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> -180:180 </p>',
  '_restr_torsion_atom_site_label_1': '<pre><h2>_restr_torsion_atom_site_label_1</h2> The atom-site '
                                      'labels of the atoms in the sequence in which\n'
                                      ' they are linked by the bonds whose torsion angle is to\n'
-                                     ' be restrained.</pre>',
+                                     ' be restrained.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_torsion_atom_site_label_2': '<pre><h2>_restr_torsion_atom_site_label_2</h2> The atom-site '
                                      'labels of the atoms in the sequence in which\n'
                                      ' they are linked by the bonds whose torsion angle is to\n'
-                                     ' be restrained.</pre>',
+                                     ' be restrained.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_torsion_atom_site_label_3': '<pre><h2>_restr_torsion_atom_site_label_3</h2> The atom-site '
                                      'labels of the atoms in the sequence in which\n'
                                      ' they are linked by the bonds whose torsion angle is to\n'
-                                     ' be restrained.</pre>',
+                                     ' be restrained.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_torsion_atom_site_label_4': '<pre><h2>_restr_torsion_atom_site_label_4</h2> The atom-site '
                                      'labels of the atoms in the sequence in which\n'
                                      ' they are linked by the bonds whose torsion angle is to\n'
-                                     ' be restrained.</pre>',
+                                     ' be restrained.</pre>\n'
+                                     '<br><p><h4>Type:</h4> string</p>',
  '_restr_torsion_details': '<pre><h2>_restr_torsion_details</h2> A free-text description of the '
-                           'restraint.</pre>',
+                           'restraint.</pre>\n'
+                           '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_torsion_diff': '<pre><h2>_restr_torsion_diff</h2> The difference between the target and '
-                        'the refined torsion angle.</pre>',
+                        'the refined torsion angle.</pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_restr_torsion_site_symmetry_1': '<pre><h2>_restr_torsion_site_symmetry_1</h2> The symmetry '
                                    'transformations needed to generate the coordinates\n'
                                    ' of the four atoms that define the torsion angle.\n'
                                    '\n'
                                    'The symmetry code of each atom site is given as the \n'
                                    "\t      symmetry-equivalent position number 'n' and the cell \n"
                                    "\t      translation number 'klm'. These numbers are combined \n"
@@ -1313,15 +1498,17 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_torsion_site_symmetry_2': '<pre><h2>_restr_torsion_site_symmetry_2</h2> The symmetry '
                                    'transformations needed to generate the coordinates\n'
                                    ' of the four atoms that define the torsion angle.\n'
                                    '\n'
                                    'The symmetry code of each atom site is given as the \n'
                                    "\t      symmetry-equivalent position number 'n' and the cell \n"
                                    "\t      translation number 'klm'. These numbers are combined \n"
@@ -1344,15 +1531,17 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_torsion_site_symmetry_3': '<pre><h2>_restr_torsion_site_symmetry_3</h2> The symmetry '
                                    'transformations needed to generate the coordinates\n'
                                    ' of the four atoms that define the torsion angle.\n'
                                    '\n'
                                    'The symmetry code of each atom site is given as the \n'
                                    "\t      symmetry-equivalent position number 'n' and the cell \n"
                                    "\t      translation number 'klm'. These numbers are combined \n"
@@ -1375,15 +1564,17 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_torsion_site_symmetry_4': '<pre><h2>_restr_torsion_site_symmetry_4</h2> The symmetry '
                                    'transformations needed to generate the coordinates\n'
                                    ' of the four atoms that define the torsion angle.\n'
                                    '\n'
                                    'The symmetry code of each atom site is given as the \n'
                                    "\t      symmetry-equivalent position number 'n' and the cell \n"
                                    "\t      translation number 'klm'. These numbers are combined \n"
@@ -1406,16 +1597,20 @@
                                    '      m = 5 + z\n'
                                    ' By adding 5 to the translations, the use of negative numbers\n'
                                    ' is avoided.\n'
                                    '\n'
                                    '<h3>Example:</h3>\n'
                                    'None\n'
                                    '4\n'
-                                   '7_645</pre>',
+                                   '7_645</pre>\n'
+                                   '<br><p><h4>Type:</h4> string</p>\n'
+                                   '<br><p><h4>Default:</h4> 1_555 </p>',
  '_restr_torsion_weight_param': '<pre><h2>_restr_torsion_weight_param</h2> Weighting parameter = '
                                 'sqrt(1/weight).\n'
                                 ' It is the expectation value of the difference between\n'
                                 ' the refined value and the target.\n'
                                 ' If this parameter is set to zero, the angle will be constrained\n'
                                 ' to refine to the target value.\n'
                                 ' If this item is absent, its value will be taken as zero\n'
-                                ' and the angle will be constrained.</pre>'}
+                                ' and the angle will be constrained.</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                '<br><p><h4>Limits:</h4> 0:∞ </p>'}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finalcif-136/finalcif/cif/text.py` & `finalcif-137/finalcif/cif/text.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/twin_dict.py` & `finalcif-137/finalcif/cif/twin_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,39 +12,44 @@
                          '\tcommon lattice in three dimensions\n'
                          '\n'
                          'diperiodic\n'
                          '\tcommon lattice in two dimensions\n'
                          '\n'
                          'monoperiodic\n'
                          '\tcommon lattice in one dimension\n'
-                         '</pre>',
+                         '</pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_twin_formation_mechanism': '<pre><h2>_twin_formation_mechanism</h2>\n'
                               '     A description of the method of twin formation.\n'
                               '\n'
                               '<h3>Example:</h3>\n'
                               'gt\n'
                               '\tgrowth twin formed during crystal growth\n'
                               '\n'
                               'tt\n'
                               '\ttransformation twin formed during phase transition\n'
                               '\n'
                               'mt\n'
                               '\tmechanical twin formed as a result of mechanical action\n'
-                              '</pre>',
+                              '</pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_twin_individual_id': '<pre><h2>_twin_individual_id</h2>\n'
                         '      The unique identifier for this twin individual. \n'
                         '      The twin for which _twin_individual_twin_matrix_\n'
                         '      is the identity matrix is called the reference twin.  \n'
-                        "      It is recommended that the reference twin be labelled '1'. </pre>",
+                        "      It is recommended that the reference twin be labelled '1'. </pre>\n"
+                        '<br><p><h4>Type:</h4> string</p>',
  '_twin_individual_mass_fraction_refined': '<pre><h2>_twin_individual_mass_fraction_refined</h2>\n'
                                            '      The refined mass fraction of this twin '
                                            'individual; the sum\n'
                                            '      of all mass fractions must equal unity within '
                                            'the limits of \n'
-                                           '      experimental uncertainty.</pre>',
+                                           '      experimental uncertainty.</pre>\n'
+                                           '<br><p><h4>Type:</h4> number (int or float)</p>\n'
+                                           '<br><p><h4>Limits:</h4> 0:1.0 </p>',
  '_twin_individual_twin_lattice_type': '<pre><h2>_twin_individual_twin_lattice_type</h2>\n'
                                        '       Identification of the symmetry relationships '
                                        'between the \n'
                                        '       twin lattices as described in International '
                                        'Tables \n'
                                        '       for Crystallography (2004), Vol. C, Chapter 1.3.  \n'
                                        '       The twin with the identity matrix should be denoted '
@@ -70,114 +75,124 @@
                                        '\tpseudo-merohedral\n'
                                        '\n'
                                        'rpmt\n'
                                        '\treticular pseudo-merohedral\n'
                                        '\n'
                                        'nmt\n'
                                        '\tnon-merohedral\n'
-                                       '</pre>',
+                                       '</pre>\n'
+                                       '<br><p><h4>Type:</h4> string</p>',
  '_twin_individual_twin_matrix_11': '<pre><h2>_twin_individual_twin_matrix_11</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_12': '<pre><h2>_twin_individual_twin_matrix_12</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_13': '<pre><h2>_twin_individual_twin_matrix_13</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_21': '<pre><h2>_twin_individual_twin_matrix_21</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_22': '<pre><h2>_twin_individual_twin_matrix_22</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_23': '<pre><h2>_twin_individual_twin_matrix_23</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_31': '<pre><h2>_twin_individual_twin_matrix_31</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_32': '<pre><h2>_twin_individual_twin_matrix_32</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_individual_twin_matrix_33': '<pre><h2>_twin_individual_twin_matrix_33</h2>\n'
                                     '     Elements of the matrix U that multiplies the Miller '
                                     'indices h,k,l \n'
                                     '     of the reference twin to give the Miller indices '
                                     "h',k',l', \n"
                                     '     of the twin specified by _twin_individual_id \n'
                                     '\n'
                                     "           (h' k' l') = U (h k l )\n"
                                     '\n'
                                     '     It follows that the reference twin must have U = I, the '
-                                    'identity matrix. </pre>',
+                                    'identity matrix. </pre>\n'
+                                    '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_morphology': '<pre><h2>_twin_morphology</h2>\n'
                      ' The physical relationship of the different twins to one another.\n'
                      '\n'
                      '<h3>Example:</h3>\n'
                      'contact\n'
                      '\tseparated by a surface\n'
                      '\n'
@@ -188,15 +203,16 @@
                      '\tindividuals are not repeated\n'
                      '\n'
                      'polysynthetic\n'
                      '\tindividuals repeat in approximately linear arrangement\n'
                      '\n'
                      'cyclic\n'
                      '\tindividuals repeat in closed edifice\n'
-                     '</pre>',
+                     '</pre>\n'
+                     '<br><p><h4>Type:</h4> string</p>',
  '_twin_refln_F_squared_calc': '<pre><h2>_twin_refln_F_squared_calc</h2> \n'
                                '\n'
                                '        Calculated value for the overall squared structure factors '
                                '(in\n'
                                '        electrons squared for X-ray diffraction) arising from '
                                'all \n'
                                '        the twin contributions to the peak defined by '
@@ -214,53 +230,58 @@
                                '        mf is the mass fraction,\n'
                                '        and the sum is taken over all the twin components that '
                                'contribute\n'
                                '        to this diffraction peak.\n'
                                '\n'
                                '        Reference: Pratt, C. S., Coyle, B. A. &amp; Ibers, J. A. '
                                '(1971).\n'
-                               '        J. Chem. Soc. A, pp. 2146-2151.</pre>',
+                               '        J. Chem. Soc. A, pp. 2146-2151.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_F_squared_calc_individual': '<pre><h2>_twin_refln_F_squared_calc_individual</h2> \n'
                                           '\n'
                                           '        Contribution of the twin identified by '
                                           '_twin_refln_individual_id \n'
                                           '        to _twin_refln_F_squared_calc. \n'
                                           '\n'
                                           '        _twin_refln_F_squared_calc_individual = osf * '
                                           'mf * _refln_F_squared_calc\n'
                                           '\n'
                                           '        where osf is the overall scale factor, mf is '
                                           'the mass factor.\n'
                                           '        For X-ray diffraction the units are electrons '
                                           'squared.\n'
-                                          '</pre>',
+                                          '</pre>\n'
+                                          '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_F_squared_meas': '<pre><h2>_twin_refln_F_squared_meas</h2>\n'
                                '         The observed value F^2^ of the peak referenced by \n'
                                '         _twin_refln_datum_id. This is typically the observed '
                                'peak\n'
                                '         intensity after Lorentz and polarization '
-                               'corrections.</pre>',
+                               'corrections.</pre>\n'
+                               '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_F_squared_sigma': '<pre><h2>_twin_refln_F_squared_sigma</h2>\n'
                                 '            Standard uncertainty of '
-                                '_twin_refln_F_squared_meas</pre>',
+                                '_twin_refln_F_squared_meas</pre>\n'
+                                '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_datum_id': '<pre><h2>_twin_refln_datum_id</h2>\n'
                          '     This item serves to identify an observed diffraction peak. \n'
                          '     It may include contributions from one or more twin components\n'
                          '     and so may appear more than once in the list.  \n'
                          '     The values of _twin_refln_F_squared_calc and \n'
                          '     _twin_refln_F_squared_meas indexed by\n'
                          '     _twin_refln_datum_id include the contributions from all the '
                          'twins.  \n'
                          '     The diffraction peak is indexed by \n'
                          '     _twin_refln_index_h, *_k and *_l referred to the cell of \n'
                          '     the twin component identified by _twin_refln_individual_id.  \n'
                          '     \n'
                          '     The list reference includes both _twin_refln_datum_id and \n'
                          '     _twin_refln_individual_id.  The combination of these two items \n'
-                         '     may only appear once in a list. </pre>',
+                         '     may only appear once in a list. </pre>\n'
+                         '<br><p><h4>Type:</h4> string</p>',
  '_twin_refln_include_status': '<pre><h2>_twin_refln_include_status</h2>\n'
                                '    A symbol indicating how the reflection is treated during '
                                'refinement.\n'
                                '\n'
                                '<h3>Example:</h3>\n'
                                'o\n'
                                "lower-case letter o for 'observed')\n"
@@ -283,41 +304,48 @@
                                '\tremoved from the refinement for other reasons\n'
                                '\n'
                                'h\n'
                                '\tdoes not satisfy _refine_ls_d_res_high\n'
                                '\n'
                                'l\n'
                                '\tdoes not satisfy _refine_ls_d_res_low\n'
-                               '</pre>',
+                               '</pre>\n'
+                               '<br><p><h4>Type:</h4> string</p>\n'
+                               '<br><p><h4>Default:</h4> o </p>',
  '_twin_refln_index_h': '<pre><h2>_twin_refln_index_h</h2>\n'
                         '     Miller indices of a reflection from the twin component \n'
                         '     labelled by _twin_refln_individual_id. \n'
                         '     The values of the Miller indices must correspond \n'
-                        '     to the cell defined for this twin component.  </pre>',
+                        '     to the cell defined for this twin component.  </pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_index_k': '<pre><h2>_twin_refln_index_k</h2>\n'
                         '     Miller indices of a reflection from the twin component \n'
                         '     labelled by _twin_refln_individual_id. \n'
                         '     The values of the Miller indices must correspond \n'
-                        '     to the cell defined for this twin component.  </pre>',
+                        '     to the cell defined for this twin component.  </pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_index_l': '<pre><h2>_twin_refln_index_l</h2>\n'
                         '     Miller indices of a reflection from the twin component \n'
                         '     labelled by _twin_refln_individual_id. \n'
                         '     The values of the Miller indices must correspond \n'
-                        '     to the cell defined for this twin component.  </pre>',
+                        '     to the cell defined for this twin component.  </pre>\n'
+                        '<br><p><h4>Type:</h4> number (int or float)</p>',
  '_twin_refln_individual_id': '<pre><h2>_twin_refln_individual_id</h2>\n'
                               '      The unique identifier of the twin individual \n'
                               '      whose Miller indices are given in _twin_refln_index_.  \n'
                               '      The ID must match a _twin_individual_id in the \n'
                               '      TWIN_INDIVIDUAL category.  \n'
                               '\n'
                               '     The list reference includes both _twin_refln_datum_id and \n'
                               '     _twin_refln_individual_id.  The combination of these two '
                               'items \n'
-                              '     may only appear once in a list. </pre>',
+                              '     may only appear once in a list. </pre>\n'
+                              '<br><p><h4>Type:</h4> string</p>',
  '_twin_special_details': '<pre><h2>_twin_special_details</h2>\n'
                           '    Information about twinning in the sample not contained in other '
                           'data items.\n'
                           '\n'
                           '<h3>Example:</h3>\n'
                           '   Individuals 3 and 4 arise from form (I) following an\n'
                           '    enantiotropic phase transition by sudden cooling in\n'
-                          '    a cryostat to 173K. </pre>'}
+                          '    a cryostat to 173K. </pre>\n'
+                          '<br><p><h4>Type:</h4> string</p>'}
```

### Comparing `finalcif-136/finalcif/cif/checkcif/checkcif.py` & `finalcif-137/finalcif/cif/checkcif/checkcif.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/deposit.py` & `finalcif-137/finalcif/cif/cod/deposit.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/deposit_check.py` & `finalcif-137/finalcif/cif/cod/deposit_check.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/deposition_list.py` & `finalcif-137/finalcif/cif/cod/deposition_list.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/doi.py` & `finalcif-137/finalcif/cif/cod/doi.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/upload.py` & `finalcif-137/finalcif/cif/cod/upload.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/cif/cod/website_parser.py` & `finalcif-137/finalcif/cif/cod/website_parser.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/bruker_data.py` & `finalcif-137/finalcif/datafiles/bruker_data.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/bruker_frame.py` & `finalcif-137/finalcif/datafiles/bruker_frame.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/ccdc_mail.py` & `finalcif-137/finalcif/datafiles/ccdc_mail.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/data.py` & `finalcif-137/finalcif/datafiles/data.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/p4p_reader.py` & `finalcif-137/finalcif/datafiles/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/sadabs.py` & `finalcif-137/finalcif/datafiles/sadabs.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/saint.py` & `finalcif-137/finalcif/datafiles/saint.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/shelx_lst.py` & `finalcif-137/finalcif/datafiles/shelx_lst.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/datafiles/utils.py` & `finalcif-137/finalcif/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/displaymol/molecule2D.py` & `finalcif-137/finalcif/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/displaymol/sdm.py` & `finalcif-137/finalcif/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/displaymol/vtk_molecule.py` & `finalcif-137/finalcif/displaymol/vtk_molecule.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/equip_property/author_loop_templates.py` & `finalcif-137/finalcif/equip_property/author_loop_templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/equip_property/equipment.py` & `finalcif-137/finalcif/equip_property/equipment.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import List, Dict
 from typing import TYPE_CHECKING
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QListWidgetItem
 from gemmi import cif
 
+from finalcif.app_path import application_path
 from finalcif.cif.cif_file_io import CifContainer
 from finalcif.cif.text import retranslate_delimiter, string_to_utf8
 from finalcif.equip_property.tools import read_document_from_cif_file
 from finalcif.gui.custom_classes import Column, light_green
 from finalcif.gui.dialogs import show_general_warning, cif_file_open_dialog, cif_file_save_dialog
 from finalcif.tools import misc
 from finalcif.tools.misc import include_equipment_imports
@@ -119,14 +120,28 @@
         self.settings.save_key_value(name='deleted_templates', item=deleted)
         self.show_equipment()
 
     def load_default_equipment(self):
         self.store_predefined_templates()
         self.show_equipment()
 
+    def load_equipment_files(self):
+        template_path = Path(application_path).joinpath('template/machines').resolve()
+        files = template_path.glob('*.cif')
+        for file in files:
+            try:
+                doc = read_document_from_cif_file(file.__str__())
+                block = doc.sole_block()
+            except Exception as e:
+                print(f'DBG> Could not load equipment templates: {e.__str__()}')
+                continue
+            if file.stem.replace('_', ' ') in self.settings.deleted_equipment:
+                continue
+            self._import_block(block, filename=str(file.resolve()))
+
     def store_predefined_templates(self):
         equipment_list = self.settings.get_equipment_list() or []
         for item in misc.predefined_equipment_templates:
             if item['name'] not in equipment_list:
                 self.settings.save_settings_list('equipment', item['name'], item['items'])
 
     def edit_equipment_template(self) -> None:
@@ -179,51 +194,56 @@
         # Local import for faster startup
         from finalcif.cif.all_cif_dicts import cif_all_dict
         table_data = self.get_equipment_entry_data()
         # warn if key is not official:
         for key, _ in table_data:
             if key not in cif_all_dict.keys():
                 if not key.startswith('_'):
-                    show_general_warning(self.app, '"{}" is not a valid keyword! '
-                                                   '\nChange the name in order to save.\n'
-                                                   'Keys must start with an underscore.'.format(key))
+                    show_general_warning(self.app,
+                                         f'"{key}" is not a valid keyword! \n'
+                                         f'Change the name in order to save.\n'
+                                         f'Keys must start with an underscore.')
                     return
                 show_general_warning(self.app, '"{}" is not an official CIF keyword!'.format(key))
         self.settings.save_settings_list('equipment', self.selected_template_name(), table_data)
         self.app.ui.EquipmentTemplatesStackedWidget.setCurrentIndex(0)
-        print('saved')
+        self.load_default_equipment()
 
     def import_equipment_from_file(self, filename: Path | str = '') -> None:
         """
         Import an equipment entry from a cif file.
         """
         if isinstance(filename, Path):
             filename = str(filename)
         if not filename:
-            filename = cif_file_open_dialog(filter="CIF file (*.cif  *.cif_od *.cfx)")
+            filename = cif_file_open_dialog(filter="CIF file (*.pcf *.cif  *.cif_od *.cfx)")
         if not filename:
             print('No file given')
             return
         doc = read_document_from_cif_file(filename)
         if not doc:
             return
         for block in doc:
             self._import_block(block, filename)
-        self.show_equipment()
+        self.load_default_equipment()
 
     def _import_block(self, block: cif.Block, filename: str) -> None:
         table_data = []
         for item in block:
             if item.pair is not None:
                 key, value = item.pair
                 if filename.endswith('.cif_od') and key not in include_equipment_imports:
                     continue
                 table_data.append([key, retranslate_delimiter(cif.as_string(value).strip('\n\r ;'))])
         if filename.endswith('.cif_od'):
             name = Path(filename).stem
+        elif filename.endswith('.pcf'):
+            name = Path(filename).stem.replace('_', ' ')
+        elif block.name == 'site_settings':
+            name = Path(filename).stem.replace('_', ' ')
         else:
             name = block.name.replace('__', ' ')
         self.undelete_equipment(equipment_name=name)
         self.settings.save_settings_list('equipment', name, table_data)
 
     def get_equipment_entry_data(self) -> list:
         """
@@ -279,13 +299,14 @@
         """
         Cancel Equipment editing.
         """
         table = self.app.ui.EquipmentEditTableWidget
         table.clearContents()
         table.setRowCount(0)
         self.app.ui.EquipmentTemplatesStackedWidget.setCurrentIndex(0)
+        self.load_default_equipment()
 
 
 if __name__ == '__main__':
     l = Equipment(None, FinalCifSettings())
     for line in l.export_raw_data():
         print(f"{line}")
```

### Comparing `finalcif-136/finalcif/equip_property/properties.py` & `finalcif-137/finalcif/equip_property/properties.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/equip_property/tools.py` & `finalcif-137/finalcif/equip_property/tools.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/combobox.py` & `finalcif-137/finalcif/gui/combobox.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/custom_classes.py` & `finalcif-137/finalcif/gui/custom_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         # Clear current selection.
         self.setCurrentItem(None)
         if not searchtext:
             # Empty string, don't search and set all unhidden:
             for row in range(self.rowCount()):
                 self.setRowHidden(row, False)
             return
-
+        searchtext = searchtext.replace('.', '_')
         searchpattern = re.compile(f'.*{searchtext}.*', re.IGNORECASE)
         searched = [x for x in self.vheaderitems if searchpattern.match(x)]
 
         for row in range(self.rowCount()):
             if self.vheaderitems[row] in searched:
                 self.setRowHidden(row, False)
             else:
@@ -175,14 +175,15 @@
             pass
         return QObject.eventFilter(self, widget, event)
 
     def setText(self, key: str, column: int, txt: str, row: int = None, color=None):
         """
         Set text in current table cell regardless of the containing item.
         """
+        self.color = color
         txt = retranslate_delimiter(txt)
         if row is None and key in self.vheaderitems:
             row = self.vheaderitems.index(key)
         elif row is None and key not in self.vheaderitems:
             row = 0
             raise IndexError
         if isinstance(self.cellWidget(row, column), MyComboBox):
@@ -191,14 +192,15 @@
         if isinstance(self.cellWidget(row, column), MyQPlainTextEdit):
             widget = self.cellWidget(row, column)
             widget.setText(txt, color=color)
             # setting the CIF key here is important for the finding of row e.g. for clipboard copy
             widget.cif_key = key
         else:
             textedit = MyQPlainTextEdit(self)
+            textedit.color = self.color
             textedit.cif_key = key
             textedit.templateRequested.connect(self.goto_template_page)
             textedit.new_key.connect(lambda x: self.new_key.emit(x))
             self.setCellWidget(row, column, textedit)
             textedit.setText(txt, color=color, column=column)
             if (column == Column.CIF) or (column == Column.DATA):
                 textedit.setUneditable()
```

### Comparing `finalcif-136/finalcif/gui/dialogs.py` & `finalcif-137/finalcif/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/edit_button.py` & `finalcif-137/finalcif/gui/edit_button.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/equipmenttable.py` & `finalcif-137/finalcif/gui/equipmenttable.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/file_editor.py` & `finalcif-137/finalcif/gui/file_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/finalcif_gui_ui.py` & `finalcif-137/finalcif/gui/finalcif_gui_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/finalcif_gui_ui.ui` & `finalcif-137/finalcif/gui/finalcif_gui_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/import_selector.py` & `finalcif-137/finalcif/gui/import_selector.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/import_selector_ui.py` & `finalcif-137/finalcif/gui/import_selector_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/import_selector_ui.ui` & `finalcif-137/finalcif/gui/import_selector_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/loop_creator.py` & `finalcif-137/finalcif/gui/loop_creator.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/loop_creator_ui.py` & `finalcif-137/finalcif/gui/loop_creator_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,14 @@
         self.label.setObjectName("label")
         self.horizontalLayout.addWidget(self.label)
         self.searchLineEdit = QtWidgets.QLineEdit(LoopCreator)
         self.searchLineEdit.setObjectName("searchLineEdit")
         self.horizontalLayout.addWidget(self.searchLineEdit)
         self.verticalLayout_2.addLayout(self.horizontalLayout)
         self.availableKeysListWidget = QtWidgets.QListWidget(LoopCreator)
-        font = QtGui.QFont()
-        font.setPointSize(13)
-        self.availableKeysListWidget.setFont(font)
         self.availableKeysListWidget.setObjectName("availableKeysListWidget")
         self.verticalLayout_2.addWidget(self.availableKeysListWidget)
         self.horizontalLayout_2.addLayout(self.verticalLayout_2)
         self.verticalLayout = QtWidgets.QVBoxLayout()
         self.verticalLayout.setContentsMargins(0, -1, -1, -1)
         self.verticalLayout.setObjectName("verticalLayout")
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
@@ -56,17 +53,14 @@
         self.label_3 = QtWidgets.QLabel(LoopCreator)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_3.addWidget(self.label_3)
         self.label_4 = QtWidgets.QLabel(LoopCreator)
         self.label_4.setObjectName("label_4")
         self.verticalLayout_3.addWidget(self.label_4)
         self.newLoopKeysListWidget = QtWidgets.QListWidget(LoopCreator)
-        font = QtGui.QFont()
-        font.setPointSize(13)
-        self.newLoopKeysListWidget.setFont(font)
         self.newLoopKeysListWidget.setObjectName("newLoopKeysListWidget")
         self.verticalLayout_3.addWidget(self.newLoopKeysListWidget)
         self.saveLoopPushButton = QtWidgets.QPushButton(LoopCreator)
         self.saveLoopPushButton.setObjectName("saveLoopPushButton")
         self.verticalLayout_3.addWidget(self.saveLoopPushButton)
         self.horizontalLayout_2.addLayout(self.verticalLayout_3)
```

### Comparing `finalcif-136/finalcif/gui/loop_creator_ui.ui` & `finalcif-137/finalcif/gui/loop_creator_ui.ui`

 * *Files 14% similar despite different names*

#### Comparing `finalcif-136/finalcif/gui/loop_creator_ui.ui` & `finalcif-137/finalcif/gui/loop_creator_ui.ui`

```diff
@@ -34,21 +34,15 @@
               </item>
               <item>
                 <widget class="QLineEdit" name="searchLineEdit"/>
               </item>
             </layout>
           </item>
           <item>
-            <widget class="QListWidget" name="availableKeysListWidget">
-              <property name="font">
-                <font>
-                  <pointsize>13</pointsize>
-                </font>
-              </property>
-            </widget>
+            <widget class="QListWidget" name="availableKeysListWidget"/>
           </item>
         </layout>
       </item>
       <item>
         <layout class="QVBoxLayout" name="verticalLayout">
           <property name="leftMargin">
             <number>0</number>
@@ -108,21 +102,15 @@
             <widget class="QLabel" name="label_4">
               <property name="text">
                 <string>Add CIF keys in order to create a new loop</string>
               </property>
             </widget>
           </item>
           <item>
-            <widget class="QListWidget" name="newLoopKeysListWidget">
-              <property name="font">
-                <font>
-                  <pointsize>13</pointsize>
-                </font>
-              </property>
-            </widget>
+            <widget class="QListWidget" name="newLoopKeysListWidget"/>
           </item>
           <item>
             <widget class="QPushButton" name="saveLoopPushButton">
               <property name="text">
                 <string>Save new Loop</string>
               </property>
             </widget>
```

### Comparing `finalcif-136/finalcif/gui/loops.py` & `finalcif-137/finalcif/gui/loops.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/mainstackwidget.py` & `finalcif-137/finalcif/gui/mainstackwidget.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/mixins.py` & `finalcif-137/finalcif/gui/mixins.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/new_key_dialog.py` & `finalcif-137/finalcif/gui/new_key_dialog.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/new_key_dialog_ui.py` & `finalcif-137/finalcif/gui/new_key_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/new_key_dialog_ui.ui` & `finalcif-137/finalcif/gui/new_key_dialog_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/plaintextedit.py` & `finalcif-137/finalcif/gui/plaintextedit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import dataclasses
 from enum import IntEnum
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
-from PyQt5 import QtCore
+from PyQt5 import QtCore, QtGui
 from PyQt5.QtCore import pyqtSignal, Qt, QObject, QEvent, QSize
 from PyQt5.QtGui import QTextOption, QFontMetrics, QContextMenuEvent, QFont, QColor
 from PyQt5.QtWidgets import QPlainTextEdit, QFrame, QAbstractScrollArea
 
 from finalcif.gui.edit_button import FloatingButtonWidget
 from finalcif.gui.new_key_dialog import NewKey
+from finalcif.gui.validators import validators
 
 if TYPE_CHECKING:
     from finalcif.gui.custom_classes import MyCifTable
 
 
 class Column(IntEnum):
     CIF = 0
@@ -24,19 +26,20 @@
     A special plaintextedit with convenient methods to set the background color and other things.
     """
     templateRequested = pyqtSignal(int)
     new_key = pyqtSignal(str)
     to_be_shortened = {'_shelx_hkl_file', '_shelx_res_file', '_shelx_fab_file', '_shelx_fcf_file',
                        '_iucr_refine_instructions_details', '_iucr_refine_fcf_details'}
 
-    def __init__(self, parent=None, *args, **kwargs):
+    def __init__(self, parent=None, *args):
         """
         Plaintext edit field for most of the table cells.
         """
-        super().__init__(parent=parent, *args, **kwargs)
+        super().__init__(*args, parent)
+        self.color = None
         self.cif_key = ''
         self.edit_button = None
         font = QFont()
         font.setPointSize(self.document().defaultFont().pointSize() + 1)
         self.setFont(font)
         self.parent: 'MyCifTable' = parent
         self.setFocusPolicy(Qt.StrongFocus)
@@ -97,18 +100,14 @@
         return self.parent.indexAt(self.pos()).column()
 
     def setBackground(self, color: QColor) -> None:
         """
         Set background color of the text field.
         """
         self.setStyleSheet("background-color: {};".format(str(color.name())))
-        # No idea why this does not work
-        # pal = self.palette()
-        # pal.setColor(QPalette.Base, color)
-        # self.setPalette(pal)
 
     def setUneditable(self):
         self.setReadOnly(True)
 
     def setText(self, text: str, color: QColor = None, column: int = None):
         """
         Set text of a Plaintextfield with lines wrapped at newline characters.
@@ -146,14 +145,31 @@
             self.edit_button.show()
 
     def event(self, e: QtCore.QEvent):
         if e.type() == QtCore.QEvent.InputMethodQuery:
             self.parent.setCurrentCell(self.row, self.column)
         return super().event(e)
 
+    def keyPressEvent(self, event: QtGui.QKeyEvent):
+        super().keyPressEvent(event)
+        if self.column == Column.EDIT:
+            self.validate_text(self.toPlainText())
+
+    def validate_text(self, text: str):
+        validator = validators.get(self.cif_key, None)
+        if validator and not validator.valid(text):
+            self.setBackground(QColor(254, 191, 189))
+            self.setToolTip(validator.help_text)
+        else:
+            self.setToolTip('')
+            if self.color:
+                self.setBackground(self.color)
+            else:
+                self.setStyleSheet("")
+
     def leaveEvent(self, a0: QEvent) -> None:
         super().leaveEvent(a0)
         if self.edit_button and self.column == Column.EDIT:
             self.edit_button.hide()
 
     def getText(self):
         return self.toPlainText()
```

### Comparing `finalcif-136/finalcif/gui/playground.py` & `finalcif-137/finalcif/gui/playground.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/propertytable.py` & `finalcif-137/finalcif/gui/propertytable.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/spell_check_edit.py` & `finalcif-137/finalcif/gui/spell_check_edit.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/gui/text_templates_ui.py` & `finalcif-137/finalcif/gui/text_templates_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self.cifKeyLineEdit = QtWidgets.QLineEdit(TextTemplatesWidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(40)
         sizePolicy.setHeightForWidth(self.cifKeyLineEdit.sizePolicy().hasHeightForWidth())
         self.cifKeyLineEdit.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
-        font.setPointSize(12)
         font.setBold(True)
         font.setWeight(75)
         self.cifKeyLineEdit.setFont(font)
         self.cifKeyLineEdit.setText("")
         self.cifKeyLineEdit.setReadOnly(True)
         self.cifKeyLineEdit.setObjectName("cifKeyLineEdit")
         self.horizontalLayout.addWidget(self.cifKeyLineEdit)
@@ -84,17 +83,14 @@
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.plainTextEdit = SpellTextEdit(self.combinedTestGroupBox)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.plainTextEdit.sizePolicy().hasHeightForWidth())
         self.plainTextEdit.setSizePolicy(sizePolicy)
-        font = QtGui.QFont()
-        font.setPointSize(10)
-        self.plainTextEdit.setFont(font)
         self.plainTextEdit.setFrameShadow(QtWidgets.QFrame.Plain)
         self.plainTextEdit.setLineWidth(0)
         self.plainTextEdit.setBackgroundVisible(False)
         self.plainTextEdit.setObjectName("plainTextEdit")
         self.verticalLayout_4.addWidget(self.plainTextEdit)
         self.horizontalLayout_2.addWidget(self.combinedTestGroupBox)
         self.verticalLayout_3.addLayout(self.horizontalLayout_2)
```

### Comparing `finalcif-136/finalcif/gui/text_templates_ui.ui` & `finalcif-137/finalcif/gui/text_templates_ui.ui`

 * *Files 2% similar despite different names*

#### Comparing `finalcif-136/finalcif/gui/text_templates_ui.ui` & `finalcif-137/finalcif/gui/text_templates_ui.ui`

```diff
@@ -47,15 +47,14 @@
                 <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                   <horstretch>0</horstretch>
                   <verstretch>40</verstretch>
                 </sizepolicy>
               </property>
               <property name="font">
                 <font>
-                  <pointsize>12</pointsize>
                   <weight>75</weight>
                   <bold>true</bold>
                 </font>
               </property>
               <property name="text">
                 <string/>
               </property>
@@ -170,19 +169,14 @@
                   <widget class="SpellTextEdit" name="plainTextEdit">
                     <property name="sizePolicy">
                       <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                         <horstretch>0</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
                     </property>
-                    <property name="font">
-                      <font>
-                        <pointsize>10</pointsize>
-                      </font>
-                    </property>
                     <property name="frameShadow">
                       <enum>QFrame::Plain</enum>
                     </property>
                     <property name="lineWidth">
                       <number>0</number>
                     </property>
                     <property name="backgroundVisible">
```

### Comparing `finalcif-136/finalcif/gui/text_value_editor.py` & `finalcif-137/finalcif/gui/text_value_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 from typing import Tuple, List, Union
 
+from PyQt5 import QtGui
 from PyQt5.QtCore import QSize, Qt, pyqtSignal
 from PyQt5.QtWidgets import QWidget, QHBoxLayout, QCheckBox, QListWidgetItem, QVBoxLayout, QLabel
 
 from finalcif.gui import text_templates_ui
 from finalcif.gui.spell_check_edit import SpellTextEdit
 
 
@@ -20,24 +21,27 @@
         layout = QHBoxLayout(self)
         self.vlayout = QVBoxLayout()
         self.vlayout.setAlignment(Qt.AlignVCenter)
         self.checkbox = QCheckBox()
         self.number_label = QLabel()
         self.vlayout.addWidget(self.number_label)
         self.textfield = SpellTextEdit(self)
-        font = self.textfield.font()
-        font.setPixelSize(12)
-        self.textfield.setFont(font)
+        self.set_font_size()
         self.vlayout.addWidget(self.checkbox)
         layout.addLayout(self.vlayout)
         layout.addWidget(self.textfield)
         layout.setContentsMargins(12, 8, 30, 8)
         self.setAutoFillBackground(False)
         self.checkbox.clicked.connect(self.on_checkbox_clicked)
 
+    def set_font_size(self):
+        font: QtGui.QFont = self.textfield.font()
+        font.setPointSize(font.pointSize() + 2)
+        self.textfield.setFont(font)
+
     @property
     def text(self) -> str:
         return self.textfield.toPlainText()
 
     def on_checkbox_clicked(self, checked: bool) -> None:
         if checked:
             self.checkbox_clicked.emit(self.textfield.toPlainText())
@@ -61,14 +65,23 @@
         super().__init__(*args, **kwargs)
         self.cif_key: str = ''
         self.ui = text_templates_ui.Ui_TextTemplatesWidget()
         self.ui.setupUi(self)
         self.ui.cancelTextPushButton.clicked.connect(self._on_backbutton_clicked)
         if not self.ui.templatesListWidget.count():
             self.add_more_fiels()
+        self.set_font_size()
+
+    def set_font_size(self):
+        textedit_font: QtGui.QFont = self.ui.plainTextEdit.font()
+        textedit_font.setPointSize(textedit_font.pointSize() + 3)
+        self.ui.plainTextEdit.setFont(textedit_font)
+        cif_key_font = self.ui.cifKeyLineEdit.font()
+        cif_key_font.setPointSize(textedit_font.pointSize())
+        self.ui.cifKeyLineEdit.setFont(cif_key_font)
 
     def _on_backbutton_clicked(self) -> None:
         self.ui.templatesListWidget.clear()
         TextEditItem._num = 1
 
     def add_textfields(self, text_list: Union[List, Tuple]) -> None:
         self.ui.templatesListWidget.clear()
```

### Comparing `finalcif-136/finalcif/gui/vrf_classes.py` & `finalcif-137/finalcif/gui/vrf_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/finalcif.png` & `finalcif-137/finalcif/icon/finalcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/finalcif2.ico` & `finalcif-137/finalcif/icon/finalcif2.ico`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/finalcif2.png` & `finalcif-137/finalcif/icon/finalcif2.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/multitable.ico` & `finalcif-137/finalcif/icon/multitable.ico`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/multitable.png` & `finalcif-137/finalcif/icon/multitable.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/icon/multitable.xcf` & `finalcif-137/finalcif/icon/multitable.xcf`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/archive_report.py` & `finalcif-137/finalcif/report/archive_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/mtools.py` & `finalcif-137/finalcif/report/mtools.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/references.py` & `finalcif-137/finalcif/report/references.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/report_text.py` & `finalcif-137/finalcif/report/report_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
 class DataReduction():
     def __init__(self, cif: CifContainer, paragraph: Paragraph, ref: references.ReferenceList):
         integration = gstr(cif['_computing_data_reduction']) or '??'
         abstype = gstr(cif['_exptl_absorpt_correction_type']) or '??'
         abs_details = gstr(cif['_exptl_absorpt_process_details']) or '??'
         data_reduct_ref = references.DummyReference()
         absorpt_ref = references.DummyReference()
-        integration_prog = '[unknown integration program]'
-        scale_prog = '[unknown program]'
+        integration_prog = '[No _computing_data_reduction given]'
+        scale_prog = '[Unknown scaling program]'
         if 'SAINT' in integration:
             data_reduct_ref, integration_prog = self.add_saint_reference(integration)
         if 'XDS' in integration:
             data_reduct_ref = references.XDSReference()
             integration_prog = 'XDS'
         if 'CrysAlisPro'.lower() in integration.lower():
             data_reduct_ref, absorpt_ref, integration_prog = self.add_crysalispro_reference(integration)
@@ -209,15 +209,16 @@
         xredversion = 'unknown version'
         # if len(integration.split()) > 1:
         #    xredversion = integration.split()[1]
         integration_prog = 'STOE X-RED'
         data_reduct_ref = references.XRedReference('X-RED', xredversion)
         return data_reduct_ref, integration_prog
 
-    def add_crysalispro_reference(self, integration: str) -> Tuple[references.CrysalisProReference, references.CrysalisProReference, str]:
+    def add_crysalispro_reference(self, integration: str) -> Tuple[
+        references.CrysalisProReference, references.CrysalisProReference, str]:
         """
         CrysAlisPro, Agilent Technologies,Version 1.171.37.31h (release 21-03-2014 CrysAlis171 .NET)
             (compiled Mar 21 2014,18:13:45)
         CrysAlisPro 1.171.42.58a (Rigaku OD, 2022)
         """
         year = 'unknown version'
         version = 'unknown year'
@@ -496,15 +497,18 @@
 
 
 class RefinementDetails():
     def __init__(self, cif: CifContainer, document: Document):
         ph = document.add_paragraph(style='Heading 2')
         ph.add_run(text=fr"Refinement details for {cif.block.name}")
         p = document.add_paragraph()
-        p.style = document.styles['fliesstext']
+        try:
+            p.style = document.styles['fliesstext']
+        except KeyError:
+            print('DBG> Text style not found')
         text = ' '.join(cif['_refine_special_details'].splitlines(keepends=False))
         if cif['_olex2_refine_details']:
             text += ' '.join(cif['_olex2_refine_details'].splitlines(keepends=False))
         # Replacing semicolon, because it can damage the CIF:
         text = text.replace(';', '.')
         p.add_run(string_to_utf8(text).strip())
 
@@ -523,15 +527,18 @@
         return radtype
     else:
         return radtype
 
 
 def make_report_text(cif, document: Document) -> references.ReferenceList:
     paragr = document.add_paragraph()
-    paragr.style = document.styles['fliesstext']
+    try:
+        paragr.style = document.styles['fliesstext']
+    except KeyError:
+        print('DBG> Text style not found')
     ref = references.ReferenceList(paragr)
     # -- The main text:
     paragr.add_run('The following text is only a suggestion: ').font.bold = True
     Crystallization(cif, paragr)
     CrystalSelection(cif, paragr)
     DataCollection(cif, paragr)
     SpaceChar(paragr).regular()
```

### Comparing `finalcif-136/finalcif/report/symm.py` & `finalcif-137/finalcif/report/symm.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/tables.py` & `finalcif-137/finalcif/report/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,14 @@
     document.save(output_filename)
     return output_filename
 
 
 def make_report_from(options: Options, cif: CifContainer, output_filename: str = None, picfile: Path = None) -> str:
     """
     Creates a tabular cif report.
-    :param file_obj: Input cif file.
-    :param output_filename: the table is saved to this file.
     """
     document = create_document()
     references: Union[ReferenceList, None] = None
 
     if not options.report_text:
         document.add_heading(f'Structure Tables for {cif.block.name}', 1)
     else:
```

### Comparing `finalcif-136/finalcif/report/templated_report.py` & `finalcif-137/finalcif/report/templated_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,23 @@
 
     def hkl_index_limits(self, cif: CifContainer) -> str:
         raise NotImplementedError
 
     def make_3d(self, cif: CifContainer, options: Options) -> str:
         raise NotImplementedError
 
+    def space_group_subdoc(self, cif: CifContainer, tpl_doc: DocxTemplate):
+        raise NotImplementedError
+
+    def make_picture(self, options: Options, picfile: Path, tpl_doc: DocxTemplate):
+        raise NotImplementedError
+
+    def format_sum_formula(self, sum_formula: str) -> str:
+        raise NotImplementedError
+
     @staticmethod
     def get_from_to_theta_range(cif: CifContainer) -> str:
         theta_min = cif['_diffrn_reflns_theta_min']
         theta_max = cif['_diffrn_reflns_theta_max']
         radiation_wavelength = cif['_diffrn_radiation_wavelength']
         try:
             d_max = f' ({float(radiation_wavelength) / (2 * sin(radians(float(theta_max)))):.2f}' \
@@ -729,19 +738,19 @@
                                        autoescape=False)
         jinja_env.filters['inv_article'] = get_inf_article
         template = jinja_env.get_template(template_file)
         try:
             with open(output_filename, encoding='utf-8', mode='w+t') as f:
                 outputText = template.render(context)
                 f.write(outputText)
-            return True
         except Exception as e:
             show_general_warning(parent=None, window_title='Warning', warn_text='Document generation failed',
                                  info_text=str(e))
             return False
+        return True
 
     def prepare_report_data(self, cif: CifContainer,
                             options: Options,
                             picfile: Path,
                             tpl_doc: DocxTemplate | None) -> tuple[dict[str, Any], DocxTemplate]:
         maincontext = {}
         if not cif.is_multi_cif:
@@ -831,15 +840,15 @@
                    'angles'                 : self.text_formatter.get_angles(),
                    'ba_symminfo'            : self.text_formatter.get_bonds_angles_symminfo(),
                    'torsions'               : self.text_formatter.get_torsion_angles(),
                    'torsion_symminfo'       : self.text_formatter.get_torsion_symminfo(),
                    'hydrogen_bonds'         : self.text_formatter.get_hydrogen_bonds(),
                    'hydrogen_symminfo'      : self.text_formatter.get_hydrogen_symminfo(),
                    'literature'             : self.text_formatter.literature,
-                   'css'                    : Path('finalcif/template/bootstrap/bootstrap.min.css').read_text(
+                   'bootstrap_css'          : Path('finalcif/template/bootstrap/bootstrap.min.css').read_text(
                        encoding='utf-8'),
                    }
         return context
 
 
 if __name__ == '__main__':
     import subprocess
@@ -854,19 +863,19 @@
     options = Options()
     # Set options with leading underscore without settings parameter in Options:
     # options._bonds_table = True
     # options._report_adp = True
     # options._without_h = True
     # options._report_text = False
     # options._hydrogen_bonds = True
+    # options._picture_width = '300'
 
     t = TemplatedReport(format=ReportFormat.HTML, options=options, cif=cif)
     work = Path('work').resolve()
     work.mkdir(exist_ok=True)
-    # shutil.copy2(Path('finalcif/template/bootstrap/bootstrap.min.css'), work)
     output = work / 'test.html'
     template_path = app_path.application_path / 'template'
     ok = t.make_templated_html_report(output_filename=str(output), picfile=pic, template_path=template_path)
     if ok:
         print('HTML report successfully generated')
     else:
         print('HTML report failed')
```

### Comparing `finalcif-136/finalcif/report/gui/mainwindow.py` & `finalcif-137/finalcif/report/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/report/gui/mainwindow.ui` & `finalcif-137/finalcif/report/gui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/mathml2omml.xsl` & `finalcif-137/finalcif/template/mathml2omml.xsl`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/report.tmpl` & `finalcif-137/finalcif/template/report.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -33,33 +33,34 @@
 
         img {
             border-radius: 6px;
         / / padding: 1 px;
         }
     </style>
     <style>
-        {{ css }}
+        {{ bootstrap_css }}
     </style>
 </head>
 
 <body>
 <div class="container">
 
     <div class="row">
         {% if options.report_text %}
             <div class="col">
         {% else %}
             <div class="col-5">
         {% endif %}
 
-        <h2>Structure Tables</h2>
+        <h2>Crystal Structure Report for {{ cif.block.name }}</h2>
         {% if options.report_text %}
 
             {% if structure_figure %}
                 <div class="card w-90 mt-4 mb-4">
+                    <!--suppress HtmlUnknownTarget -->
                     <img alt="Structure Figure" src="{{ structure_figure }}" width="100%">
                 </div>
             {% endif %}
 
             <p id="report_text">
                 A {{ crystal_colour }}, {{ crystal_shape }} shaped crystal was mounted on
                 a {{ cif._diffrn_measurement_specimen_support }}
@@ -72,16 +73,16 @@
                 {% if lowtemp_dev %}was equipped with {{ lowtemp_dev|inv_article }} {{ lowtemp_dev }}
                     low temperature device and
                 {% endif %}
                 used {{ radiation }} radiation {% if wavelength %}(λ = {{ wavelength }} Å){% endif %}.
                 All data were integrated with {{ integration_progr }} yielding {{ cif._diffrn_reflns_number }}
                 reflections of which {{ cif._reflns_number_total }} where independent and
                 {{ '%0.1f'| format((cif._reflns_number_gt|float() / cif._reflns_number_total|float()) * 100) }} %
-                were greater than 2σ(<i>F</i><sup>2</sup>). A
-                {{ abstype }} absorption correction using {{ abs_details }} was applied.<sup>[1,2]</sup>
+                were greater than 2σ(<i>F</i><sup>2</sup>).<sup>[1]</sup> A
+                {{ abstype }} absorption correction using {{ abs_details }} was applied.<sup>[2]</sup>
                 The structure was solved by
                 {{ solution_method }} methods with {{ solution_program }} and refined by full-matrix
                 least-squares methods against
                 <i>F</i><sup>2</sup> using {{ refinement_prog }}.<sup>[3,4]</sup> All non-hydrogen atoms
                 were refined with anisotropic displacement parameters.
                 {% if cif.hydrogen_atoms_present %}The hydrogen atoms were refined isotropically on
                     calculated positions using a riding model with their <i>U</i><sub>iso</sub> values
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {#
 #}
 {% if options.report_text %}
 {% else %}
 {% endif %}
-********** SSttrruuccttuurree TTaabblleess **********
+********** CCrryyssttaall SSttrruuccttuurree RReeppoorrtt ffoorr {{{{ cciiff..bblloocckk..nnaammee }}}} **********
 {% if options.report_text %} {% if structure_figure %}
 [Structure Figure]
 {% endif %}
 A {{ crystal_colour }}, {{ crystal_shape }} shaped crystal was mounted on a {
 { cif._diffrn_measurement_specimen_support }} with perfluoroether oil. {
 { crystallization_method }}. Data for {{ cif.block.name }} were collected from
 a shock-cooled single crystal at {{ cif._diffrn_ambient_temperature }} K on {
@@ -16,26 +16,26 @@
 monochromator and {{ detector|inv_article }} {{ detector }} detector. The
 diffractometer {% if lowtemp_dev %}was equipped with {{ lowtemp_dev|inv_article
 }} {{ lowtemp_dev }} low temperature device and {% endif %} used {{ radiation
 }} radiation {% if wavelength %}(λ = {{ wavelength }} Å){% endif %}. All data
 were integrated with {{ integration_progr }} yielding {
 { cif._diffrn_reflns_number }} reflections of which {{ cif._reflns_number_total
 }} where independent and {{ '%0.1f'| format((cif._reflns_number_gt|float() /
-cif._reflns_number_total|float()) * 100) }} % were greater than 2σ(F2). A {
-{ abstype }} absorption correction using {{ abs_details }} was applied.[1,2]
-The structure was solved by {{ solution_method }} methods with {
-{ solution_program }} and refined by full-matrix least-squares methods against
-F2 using {{ refinement_prog }}.[3,4] All non-hydrogen atoms were refined with
-anisotropic displacement parameters. {% if cif.hydrogen_atoms_present %}The
-hydrogen atoms were refined isotropically on calculated positions using a
-riding model with their Uiso values constrained to 1.5 times the Ueq of their
-pivot atoms for terminal sp3 carbon atoms and 1.2 times for all other carbon
-atoms. {% endif %} Crystallographic data for the structures reported in this
-paper have been deposited with the Cambridge Crystallographic Data Centre.[5]
-CCDC {% if cif._database_code_depnum_ccdc_archive %} {
+cif._reflns_number_total|float()) * 100) }} % were greater than 2σ(F2).[1] A {
+{ abstype }} absorption correction using {{ abs_details }} was applied.[2] The
+structure was solved by {{ solution_method }} methods with {{ solution_program
+}} and refined by full-matrix least-squares methods against F2 using {
+{ refinement_prog }}.[3,4] All non-hydrogen atoms were refined with anisotropic
+displacement parameters. {% if cif.hydrogen_atoms_present %}The hydrogen atoms
+were refined isotropically on calculated positions using a riding model with
+their Uiso values constrained to 1.5 times the Ueq of their pivot atoms for
+terminal sp3 carbon atoms and 1.2 times for all other carbon atoms. {% endif %}
+Crystallographic data for the structures reported in this paper have been
+deposited with the Cambridge Crystallographic Data Centre.[5] CCDC {% if
+cif._database_code_depnum_ccdc_archive %} {
 { cif._database_code_depnum_ccdc_archive|replace('CCDC ', '') }}{% else %}
 ?????? {% endif %} contain the supplementary crystallographic data for this
 paper. These data can be obtained free of charge from The Cambridge
 Crystallographic Data Centre via _w_w_w_._c_c_d_c_._c_a_m_._a_c_._u_k_/_s_t_r_u_c_t_u_r_e_s. This report and
 the CIF file were generated using FinalCif.[6]
 {% if refinement_details %}
 ****** RReeffiinneemmeenntt ddeettaaiillss ffoorr {{{{ cciiff..bblloocckk..nnaammee }}}} ******
```

### Comparing `finalcif-136/finalcif/template/template1.docx` & `finalcif-137/finalcif/template/template1.docx`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/template_for_multitable.docx` & `finalcif-137/finalcif/template/template_for_multitable.docx`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/template_text.docx` & `finalcif-137/finalcif/template/template_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/template_without_text.docx` & `finalcif-137/finalcif/template/template_without_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/template/templates.py` & `finalcif-137/finalcif/template/templates.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
+from __future__ import annotations
 from contextlib import suppress
 from pathlib import Path
 from typing import List
+from typing import TYPE_CHECKING
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QColor
 from PyQt5.QtWidgets import QFileDialog, QListWidgetItem
 
-from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from finalcif.appwindow import AppWindow
-
-from finalcif.tools.settings import FinalCifSettings
+    from finalcif.tools.settings import FinalCifSettings
 
 
 class ReportTemplates:
     """
     Displays the list of report templates in the options menu.
     """
 
-    def __init__(self, app: 'AppWindow', settings: FinalCifSettings):
+    def __init__(self, app: AppWindow, settings: FinalCifSettings):
         self.app = app
         self.settings = settings
         self.lw = self.app.ui.docxTemplatesListWidget
         self.load_templates_list()
         self.app.ui.AddNewTemplPushButton.clicked.connect(self.add_new_template)
         self.app.ui.RemoveTemplPushButton.clicked.connect(self.remove_current_template)
         self.app.ui.docxTemplatesListWidget.currentItemChanged.connect(self.template_changed)
         self.app.ui.docxTemplatesListWidget.itemChanged.connect(self.template_changed)
         self.app.ui.docxTemplatesListWidget.setCurrentItem(
             self.app.ui.docxTemplatesListWidget.item(self.app.options.current_template))
 
     def add_new_template(self, templ_path: str = '') -> None:
         if not templ_path:
-            templ_path, _ = QFileDialog.getOpenFileName(filter="DOCX file (*.docx)", initialFilter="DOCX file (*.docx)",
-                                                        caption='Open a Report Template File')
+            templ_path, _ = QFileDialog.getOpenFileName(filter="DOCX file (*.docx);; html file (*.html *.tmpl)",
+                                                        initialFilter="DOCX file (*.docx)",
+                                                        caption='Open a Report Template File', parent=self.app)
         itemslist = self.get_templates_list_from_widget()
         self.app.status_bar.show_message('')
         if templ_path in itemslist:
             self.app.status_bar.show_message('This templates is already in the list.', 10)
             print('This templates is already in the list.')
             return
-        if not Path(templ_path).exists() or not Path(templ_path).is_file() \
-                or not Path(templ_path).name.endswith('.docx'):
+        if (not Path(templ_path).exists() or not Path(templ_path).is_file()
+                or not Path(templ_path).suffix in ('.docx', '.html', '.tmpl')):
             self.app.status_bar.show_message('This template does not exist or is unreadable.', 10)
             print('This template does not exist or is unreadable.', Path(templ_path).resolve())
             return
         item = QListWidgetItem(templ_path)
         item.setCheckState(Qt.Unchecked)
         self.app.ui.docxTemplatesListWidget.addItem(item)
         self.settings.save_template_list('report_templates_list', self.get_templates_list_from_widget())
```

### Comparing `finalcif-136/finalcif/template/bootstrap/bootstrap.min.css` & `finalcif-137/finalcif/template/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/download.py` & `finalcif-137/finalcif/tools/download.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/dsrmath.py` & `finalcif-137/finalcif/tools/dsrmath.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/misc.py` & `finalcif-137/finalcif/tools/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,16 @@
 def make_numbered(items):
     items.insert(0, '')
     return [(x, y) for x, y in enumerate(items)]
 
 
 # '_space_group_centring_type',  # seems to be used nowere
 # '_exptl_absorpt_special_details',   # This is not official?!?
+
+# These keywords will end up in the CIF in any case:
 essential_keys = (
     # '_atom_sites_solution_secondary'
     # '_diffrn_measurement_specimen_adhesive'
     # '_diffrn_source_power'
     # '_diffrn_source_target'
     # '_olex2_diffrn_ambient_temperature_device'
     '_diffrn_measurement_ambient_temperature_device_make',
@@ -294,18 +296,18 @@
     '_chemical_melting_point',
     '_chemical_name_common',
     '_chemical_name_systematic',
     '_computing_cell_refinement',
     '_computing_data_collection',
     '_computing_data_reduction',
     '_computing_molecular_graphics',
-    '_computing_publication_material',
+    #'_computing_publication_material',
     '_computing_structure_refinement',
     '_computing_structure_solution',
-    '_diffrn_ambient_environment',
+    #'_diffrn_ambient_environment',
     '_diffrn_ambient_temperature',
     '_diffrn_detector',
     '_diffrn_detector_area_resol_mean',
     '_diffrn_detector_type',
     '_diffrn_measured_fraction_theta_full',
     '_diffrn_measured_fraction_theta_max',
     '_diffrn_measurement_device',
```

### Comparing `finalcif-136/finalcif/tools/options.py` & `finalcif-137/finalcif/tools/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 
 class Options:
     def __init__(self, ui: Ui_FinalCifWindow = None, settings: FinalCifSettings = None):
         """
         :param ui: UI of FinalCif
         :param settings: Settings of FinalCif
-        :param debug: If turned on, this object can set and get attributes without using the settings.
         """
         self.ui = ui
         self.settings = settings
         # initial default, otherwise we have width=0.0 and no picture visible:
         if ui:
             self.ui.PictureWidthDoubleSpinBox.setValue(7.5)
             self._connect_signal_and_slots()
```

### Comparing `finalcif-136/finalcif/tools/platon.py` & `finalcif-137/finalcif/tools/platon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import subprocess
 import sys
 import threading
 import time
 from contextlib import suppress
 from pathlib import Path
+from shutil import which
 
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton, QVBoxLayout, QWidget, QLabel, \
     QPlainTextEdit
 
 
 class PlatonRunner(QtCore.QObject):
@@ -26,29 +27,29 @@
         self.log_widget = log_widget
         self.formula_moiety = ''
         self.Z = ''
         self.chk_file_text = ''
 
     def run_process(self):
         self._origdir = os.curdir
-        #os.chdir(self.cif_file.parent)
+        # os.chdir(self.cif_file.parent)
         self.formula_moiety = ''
         self.Z = ''
         self.process = QtCore.QProcess()
         self.output_widget.clear()
         threading.Thread(target=self._monitor_output_log).start()
         # self.process.readyReadStandardOutput.connect(self.on_ready_read)
         self.process.finished.connect(self._onfinished)
         self.process.setWorkingDirectory(str(self.cif_file.parent))
         self.cif_file.with_suffix('.chk').unlink(missing_ok=True)
         self.process.start(self.platon_exe, ["-U", str(self.cif_file.name)])
 
     def _onfinished(self):
         self._on_ready_read()
-        #os.chdir(self._origdir)
+        # os.chdir(self._origdir)
         self._parse_chk_file()
         self.output_widget.setPlainText(self.chk_file_text)
         self.finished.emit(True)
         self.delete_orphaned_files()
 
     def _on_ready_read(self):
         output = self.process.readAllStandardOutput().data().decode()
@@ -65,15 +66,15 @@
                 if '! Congratulations !' in log_file:
                     self._stop_program()
             except FileNotFoundError:
                 break
 
     def _stop_program(self):
         self.is_stopped = True
-        #if self.process and self.process.state() == QProcess.Running:
+        # if self.process and self.process.state() == QProcess.Running:
         self.process.terminate()
         self.finished.emit(True)
 
     def _parse_chk_file(self):
         try:
             self.chk_file_text = self.cif_file.with_suffix('.chk').read_text(encoding='latin1', errors='ignore')
         except FileNotFoundError as e:
@@ -83,21 +84,23 @@
             if line.startswith('# MoietyFormula'):
                 self.formula_moiety = ' '.join(line.split(' ')[2:])
                 self.formula.emit(self.formula_moiety)
             if line.startswith('# Z'):
                 self.Z = line[19:24].strip(' ')
 
     @property
-    def platon_exe(self):
+    def platon_exe(self) -> str:
         if sys.platform.startswith('win'):
             in_pwt = r'C:\pwt\platon.exe'
         else:
             in_pwt = 'platon'
         if Path(in_pwt).exists():
             return in_pwt
+        elif which('platon'):
+            return which('platon')
         else:
             return 'platon'
 
     def kill(self):
         if sys.platform.startswith('win'):
             with suppress(FileNotFoundError):
                 subprocess.run(["taskkill", "/f", "/im", "platon.exe"], shell=False)
```

### Comparing `finalcif-136/finalcif/tools/pupdate.py` & `finalcif-137/finalcif/tools/pupdate.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/settings.py` & `finalcif-137/finalcif/tools/settings.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/shred.py` & `finalcif-137/finalcif/tools/shred.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/space_groups.py` & `finalcif-137/finalcif/tools/space_groups.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/spgr_format.py` & `finalcif-137/finalcif/tools/spgr_format.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/statusbar.py` & `finalcif-137/finalcif/tools/statusbar.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/finalcif/tools/sumformula.py` & `finalcif-137/finalcif/tools/sumformula.py`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_checkcif.png` & `finalcif-137/screenshots/finalcif_checkcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_details.png` & `finalcif-137/screenshots/finalcif_details.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_loops.png` & `finalcif-137/screenshots/finalcif_loops.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_loops2.png` & `finalcif-137/screenshots/finalcif_loops2.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_main.png` & `finalcif-137/screenshots/finalcif_main.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_report.png` & `finalcif-137/screenshots/finalcif_report.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/screenshots/finalcif_responses.png` & `finalcif-137/screenshots/finalcif_responses.png`

 * *Files identical despite different names*

### Comparing `finalcif-136/.gitignore` & `finalcif-137/.gitignore`

 * *Files identical despite different names*

### Comparing `finalcif-136/README.md` & `finalcif-137/README.md`

 * *Files identical despite different names*

### Comparing `finalcif-136/pyproject.toml` & `finalcif-137/pyproject.toml`

 * *Files identical despite different names*

### Comparing `finalcif-136/PKG-INFO` & `finalcif-137/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: finalcif
-Version: 136
+Version: 137
 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/FinalCif/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalcif Version: 136 Summary: CIF file editor
+Metadata-Version: 2.3 Name: finalcif Version: 137 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL: Bug
 Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
 Kratzert
 gmx.de> License-File: LICENSE Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-Python: >=3.9
```

