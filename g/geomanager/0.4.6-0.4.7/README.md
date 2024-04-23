# Comparing `tmp/geomanager-0.4.6.tar.gz` & `tmp/geomanager-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomanager-0.4.6.tar", last modified: Thu Feb 29 08:15:27 2024, max compression
+gzip compressed data, was "geomanager-0.4.7.tar", last modified: Tue Apr 23 14:09:39 2024, max compression
```

## Comparing `geomanager-0.4.6.tar` & `geomanager-0.4.7.tar`

### file list

```diff
@@ -1,266 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.588713 geomanager-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-29 08:15:19.000000 geomanager-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-29 08:15:19.000000 geomanager-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-29 08:15:27.588713 geomanager-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-02-29 08:15:19.000000 geomanager-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.556713 geomanager-0.4.6/geomanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/mbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/raster_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/raster_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/raster_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/vector_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/vector_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin/wms.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    39310 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/geomanager_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/raster_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/raster_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/vector_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/forms/vector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    63619 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    63608 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    54622 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.560713 geomanager-0.4.6/geomanager/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    58148 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.564713 geomanager-0.4.6/geomanager/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    59319 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.564713 geomanager-0.4.6/geomanager/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    56680 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.564713 geomanager-0.4.6/geomanager/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.564713 geomanager-0.4.6/geomanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/management/commands/ingest_geomanager_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/management/commands/initialize_geomanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/management/commands/process_geomanager_layer_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.572713 geomanager-0.4.6/geomanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    50526 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)    79453 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0001_squashed_0024_rastertilelayer_get_time_from_tile_json_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0004_alter_dataset_can_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0005_delete_countryboundary_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0006_stationsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0008_stationsettings_name_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0009_stationsettings_popup_props.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0010_remove_stationsettings_popup_props.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0011_vectorlayericon.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0015_wmslayer_request_time_from_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0016_wmslayer_date_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0017_wmslayer_more_info_alter_wmslayer_date_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0018_wmslayer_custom_get_capabilities_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0019_wmslayer_get_capabilities_layer_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0020_tmslayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0021_rasterfilelayer_rastertilelayer_vectorfilelayer_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0022_alter_rastertilelayer_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0023_vectortilelayericon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0024_rastertilelayer_get_time_from_tile_json_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)    25095 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0025_alter_areaofinterest_options_alter_category_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0026_layerrasterfile_raster_metadata_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0027_alter_layerrasterfile_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0028_alter_pgvectortable_options_alter_dataset_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0029_rasterfilelayer_auto_ingest_from_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0030_delete_stationsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0031_remove_geomanagersettings_cap_auto_refresh_interval_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0032_rasterfilelayer_auto_ingest_nc_data_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0033_alter_layerrasterfile_file_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0034_rastertilelayer_time_parameter_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0035_vectortilelayer_render_layers_json_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0036_vectortilelayer_popup_config_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0037_dataset_enable_all_multi_layers_on_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0038_rasterfilelayer_legend_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0039_rasterfilelayer_order_rastertilelayer_order_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0040_alter_rasterfilelayer_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0041_dataset_order_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0042_alter_dataset_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0043_additionalmapboundarydata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0044_alter_additionalmapboundarydata_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0045_additionalmapboundarydata_active_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/0046_colorvalue_show_on_legend_rasterstyle_legend_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.572713 geomanager-0.4.6/geomanager/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/geomanager_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/geostore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/raster_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/raster_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/raster_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/tile_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/vector_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/vector_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/models/wms.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.572713 geomanager-0.4.6/geomanager/samples/basemaps/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/samples/basemaps/basemaps.json
--rw-r--r--   0 runner    (1001) docker     (127)    26170 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/samples/basemaps/style.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.576713 geomanager-0.4.6/geomanager/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/geostore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/raster_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/raster_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/vector_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/vector_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/serializers/wms.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/static/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/static/django_large_image/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/static/django_large_image/js/geojs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.576713 geomanager-0.4.6/geomanager/static/django_large_image/js/geojs/1.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.548713 geomanager-0.4.6/geomanager/static/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.576713 geomanager-0.4.6/geomanager/static/geomanager/css/
--rw-r--r--   0 runner    (1001) docker     (127)    35100 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/css/bulma-navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/css/preview-map.css
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/css/stations_preview.css
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/css/upload.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.576713 geomanager-0.4.6/geomanager/static/geomanager/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    70412 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/css/vendor/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.576713 geomanager-0.4.6/geomanager/static/geomanager/images/
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/images/geomapviewer-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/static/geomanager/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/add-multiple.js
--rw-r--r--   0 runner    (1001) docker     (127)    29056 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/colorbrewer.js
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/dataset-form-conditional.js
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/mbt_source_extra.js
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/raster-file-conditional.js
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/raster-file-preview.js
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/raster-tile-preview.js
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/raster_style_extra.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/raster_tile_layer_form.js
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vector-file-preview.js
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vector-tile-conditional.js
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vector-tile-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/static/geomanager/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vendor/d3-format.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   745424 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vendor/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   542509 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/vendor/ol.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/static/geomanager/js/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/widgets/icon_chooser.js
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/widgets/raster_style_widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/static/geomanager/js/wms-preview.js
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.552713 geomanager-0.4.6/geomanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.552713 geomanager-0.4.6/geomanager/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.552713 geomanager-0.4.6/geomanager/templates/admin/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/templates/admin/geomanager/layerrasterfile/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/templates/django_nextjs/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/django_nextjs/mapviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/templates/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.580713 geomanager-0.4.6/geomanager/templates/geomanager/boundary/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/boundary/additional_boundary_create.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/boundary/additional_boundary_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/boundary/additional_boundary_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/boundary/boundary_landing.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/create.html
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/index_without_custom_create.html
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/raster_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_layer_preview.html
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_upload.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/raster_tile/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/raster_tile/raster_tile_layer_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/shared/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/vector_file/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_layer_preview.html
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_upload.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/vector_tile/
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/vector_tile/vector_tile_layer_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/widgets/raster_style_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templates/geomanager/wms/
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templates/geomanager/wms/wms_layer_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/templatetags/geomanager_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.584713 geomanager-0.4.6/geomanager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/raster_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/utils/vector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.588713 geomanager-0.4.6/geomanager/views/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/nextjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    28051 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/raster_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/raster_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16349 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/vector_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/vector_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/views/wms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.588713 geomanager-0.4.6/geomanager/viewsets/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/viewsets/aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/viewsets/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/viewsets/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/viewsets/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-29 08:15:19.000000 geomanager-0.4.6/geomanager/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:15:27.588713 geomanager-0.4.6/geomanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-29 08:15:27.000000 geomanager-0.4.6/geomanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-02-29 08:15:27.000000 geomanager-0.4.6/geomanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 08:15:27.000000 geomanager-0.4.6/geomanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-29 08:15:27.000000 geomanager-0.4.6/geomanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 08:15:27.000000 geomanager-0.4.6/geomanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-29 08:15:19.000000 geomanager-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-29 08:15:27.588713 geomanager-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.834496 geomanager-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 14:09:35.000000 geomanager-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-23 14:09:35.000000 geomanager-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-23 14:09:39.834496 geomanager-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-23 14:09:35.000000 geomanager-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.798495 geomanager-0.4.7/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/mbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/raster_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/raster_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/raster_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/vector_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/vector_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39310 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/geomanager_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/raster_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/raster_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/vector_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/forms/vector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.786495 geomanager-0.4.7/geomanager/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    63619 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    63608 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    54622 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    58148 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    59319 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    56680 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.802496 geomanager-0.4.7/geomanager/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.806496 geomanager-0.4.7/geomanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/management/commands/ingest_geomanager_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/management/commands/initialize_geomanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/management/commands/process_geomanager_layer_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.814496 geomanager-0.4.7/geomanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    50526 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79453 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0001_squashed_0024_rastertilelayer_get_time_from_tile_json_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0004_alter_dataset_can_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0005_delete_countryboundary_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0006_stationsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0008_stationsettings_name_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0009_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0010_remove_stationsettings_popup_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0011_vectorlayericon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0015_wmslayer_request_time_from_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0016_wmslayer_date_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0017_wmslayer_more_info_alter_wmslayer_date_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0018_wmslayer_custom_get_capabilities_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0019_wmslayer_get_capabilities_layer_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0020_tmslayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0021_rasterfilelayer_rastertilelayer_vectorfilelayer_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0022_alter_rastertilelayer_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0023_vectortilelayericon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0024_rastertilelayer_get_time_from_tile_json_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25095 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0025_alter_areaofinterest_options_alter_category_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0026_layerrasterfile_raster_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0027_alter_layerrasterfile_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0028_alter_pgvectortable_options_alter_dataset_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0029_rasterfilelayer_auto_ingest_from_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0030_delete_stationsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0031_remove_geomanagersettings_cap_auto_refresh_interval_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0032_rasterfilelayer_auto_ingest_nc_data_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0033_alter_layerrasterfile_file_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0034_rastertilelayer_time_parameter_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0035_vectortilelayer_render_layers_json_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0036_vectortilelayer_popup_config_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0037_dataset_enable_all_multi_layers_on_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0038_rasterfilelayer_legend_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0039_rasterfilelayer_order_rastertilelayer_order_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0040_alter_rasterfilelayer_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0041_dataset_order_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0042_alter_dataset_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0043_additionalmapboundarydata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0044_alter_additionalmapboundarydata_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0045_additionalmapboundarydata_active_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0046_colorvalue_show_on_legend_rasterstyle_legend_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0047_geomanagersettings_map_disclaimer_page_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0048_alter_geomanagersettings_map_disclaimer_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0049_geomanagersettings_allow_signups_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/0050_geomanagersettings_contact_us_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.814496 geomanager-0.4.7/geomanager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20596 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/geomanager_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/geostore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/raster_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/raster_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/raster_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/tile_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/vector_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/vector_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/models/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.814496 geomanager-0.4.7/geomanager/samples/basemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/samples/basemaps/basemaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26170 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/samples/basemaps/style.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.818496 geomanager-0.4.7/geomanager/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/geostore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/raster_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/raster_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/vector_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/vector_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/serializers/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/static/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/static/django_large_image/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/static/django_large_image/js/geojs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.818496 geomanager-0.4.7/geomanager/static/django_large_image/js/geojs/1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/static/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.818496 geomanager-0.4.7/geomanager/static/geomanager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    35100 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/css/bulma-navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/css/preview-map.css
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/css/stations_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/css/upload.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.818496 geomanager-0.4.7/geomanager/static/geomanager/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    70412 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/css/vendor/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.818496 geomanager-0.4.7/geomanager/static/geomanager/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/images/geomapviewer-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.822496 geomanager-0.4.7/geomanager/static/geomanager/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/add-multiple.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29056 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/colorbrewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/dataset-form-conditional.js
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/mbt_source_extra.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster-file-conditional.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster-file-preview.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster-tile-preview.js
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster_style_extra.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster_style_index_extra.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/raster_tile_layer_form.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vector-file-preview.js
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vector-tile-conditional.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vector-tile-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.822496 geomanager-0.4.7/geomanager/static/geomanager/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vendor/d3-format.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   279633 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vendor/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   745424 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vendor/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   542509 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/vendor/ol.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/static/geomanager/js/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/widgets/icon_chooser.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/widgets/raster_style_widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/static/geomanager/js/wms-preview.js
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.790495 geomanager-0.4.7/geomanager/templates/admin/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/admin/geomanager/layerrasterfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/adminsortable/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/adminsortable/index_without_create_button.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/django_nextjs/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/django_nextjs/mapviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/boundary/additional_boundary_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/boundary/additional_boundary_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/boundary/additional_boundary_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/boundary/boundary_landing.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/create.html
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/index_without_custom_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/raster_style_legend_preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/raster_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_layer_preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_upload.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/raster_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/raster_tile/raster_tile_layer_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/shared/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/vector_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_layer_preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_upload.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.826496 geomanager-0.4.7/geomanager/templates/geomanager/vector_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/vector_tile/vector_tile_layer_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.830496 geomanager-0.4.7/geomanager/templates/geomanager/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/widgets/raster_style_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.830496 geomanager-0.4.7/geomanager/templates/geomanager/wms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templates/geomanager/wms/wms_layer_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.830496 geomanager-0.4.7/geomanager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/templatetags/geomanager_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.830496 geomanager-0.4.7/geomanager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/raster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/utils/vector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.830496 geomanager-0.4.7/geomanager/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/nextjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28051 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/raster_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/raster_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16349 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/vector_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/vector_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/views/wms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.834496 geomanager-0.4.7/geomanager/viewsets/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/viewsets/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/viewsets/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/viewsets/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/viewsets/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 14:09:35.000000 geomanager-0.4.7/geomanager/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:39.834496 geomanager-0.4.7/geomanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-23 14:09:39.000000 geomanager-0.4.7/geomanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-23 14:09:39.000000 geomanager-0.4.7/geomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:09:39.000000 geomanager-0.4.7/geomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 14:09:39.000000 geomanager-0.4.7/geomanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 14:09:39.000000 geomanager-0.4.7/geomanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 14:09:35.000000 geomanager-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-23 14:09:39.834496 geomanager-0.4.7/setup.cfg
```

### Comparing `geomanager-0.4.6/LICENSE` & `geomanager-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/PKG-INFO` & `geomanager-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.4.6
+Version: 0.4.7
 Summary: Wagtail based Geospatial Data Manager
-Home-page: https://github.com/wmo-raf/geomanager
+Home-page: https://github.com/erick-otenyo/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -212,7 +212,19 @@
 # Including the Map Viewer
 
 This package is the backend component to the frontend [geomapviewer](https://github.com/wmo-raf/geomapviewer).
 
 # Documentation
 
 TODO
+
+# Maintainer ✨
+
+**GeoManager** is built with 💛 by [Erick Otenyo](https://github.com/erick-otenyo).
+
+Your support and feedback are valuable in maintaining and improving the package.
+
+<a href="https://www.linkedin.com/in/erick-otenyo" target="_blank"><img src="images/linkedin.png" alt="logo" width="150"></a>
+<a href="https://www.buymeacoffee.com/erick_otenyo" target="_blank"><img src="images/buymeacoffe.png" alt="logo" width="150"></a>
+<a href="https://twitter.com/erick_otenyo" target="_blank"><img src="images/twitter.png" alt="logo" width="150"></a>
+
+<a href="https://www.buymeacoffee.com/erick_otenyo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geomanager-0.4.6/geomanager/admin/__init__.py` & `geomanager-0.4.7/geomanager/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/base.py` & `geomanager-0.4.7/geomanager/admin/base.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/boundary.py` & `geomanager-0.4.7/geomanager/admin/boundary.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/category.py` & `geomanager-0.4.7/geomanager/admin/category.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/dataset.py` & `geomanager-0.4.7/geomanager/admin/dataset.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/raster_file.py` & `geomanager-0.4.7/geomanager/admin/raster_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 class RasterFileLayerModelAdmin(BaseModelAdmin, SortableAdminMixin, ModelAdminCanHide):
     model = RasterFileLayer
     hidden = True
     exclude_from_explorer = True
     menu_label = _("File Layers")
     button_helper_class = RasterFileLayerButtonHelper
     list_display = ("title",)
-    list_filter = ("dataset",)
-    index_template_name = 'adminsortable/index.html'
+    list_filter = ("dataset__category",)
+    index_template_name = 'adminsortable/index_without_create_button.html'
     list_display_add_buttons = "title"
 
     create_view_class = RasterFileLayerCreateView
     edit_view_class = RasterFileLayerEditView
 
     form_view_extra_js = ["geomanager/js/raster-file-conditional.js"]
```

### Comparing `geomanager-0.4.6/geomanager/admin/raster_style.py` & `geomanager-0.4.7/geomanager/admin/raster_style.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django import forms
+from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from wagtail_modeladmin.views import CreateView
 
 from geomanager.admin.base import BaseModelAdmin, ModelAdminCanHide
 from geomanager.models import RasterFileLayer, RasterStyle
 
@@ -50,20 +51,29 @@
     list_display = ("__str__", "min", "max")
     form_view_extra_js = ["geomanager/js/raster_style_extra.js"]
     menu_icon = "palette"
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.list_display = (list(self.list_display) or []) + ["preview"]
-        self.preview.__func__.short_description = _("Color Preview")
+        self.preview.__func__.short_description = _("Legend Preview")
+
+    def get_index_view_extra_js(self):
+        js = [
+            "geomanager/js/vendor/d3.min.js",
+            "geomanager/js/raster_style_index_extra.js",
+        ]
+
+        return js
 
     def preview(self, obj):
-        if obj.use_custom_colors:
-            return None
-        color_list = [f"<li style='background-color:{color};height:20px;flex:1;'><li/>" for color in
-                      obj.palette.split(",")]
-        html = f"""
-            <ul style='display:flex;width:200px;box-shadow: 0 1px 6px rgba(0, 0, 0, 0.12), 0 1px 4px rgba(0, 0, 0, 0.12);'>
-                {''.join(color_list)}
-            </ul>
-        """
+        legend_config = obj.get_legend_config()
+
+        colors_str = ",".join([item.get("color") for item in legend_config.get("items")])
+        context = {
+            "legend_config": legend_config,
+            "raster_style": obj,
+            "colors_str": colors_str,
+        }
+        html = render_to_string("geomanager/modeladmin/raster_style_legend_preview.html", context=context)
+
         return mark_safe(html)
```

### Comparing `geomanager-0.4.6/geomanager/admin/raster_tile.py` & `geomanager-0.4.7/geomanager/admin/raster_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/vector_file.py` & `geomanager-0.4.7/geomanager/admin/vector_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/vector_tile.py` & `geomanager-0.4.7/geomanager/admin/vector_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/admin/wms.py` & `geomanager-0.4.7/geomanager/admin/wms.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/blocks.py` & `geomanager-0.4.7/geomanager/blocks.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/constants.py` & `geomanager-0.4.7/geomanager/constants.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/decorators.py` & `geomanager-0.4.7/geomanager/decorators.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/errors.py` & `geomanager-0.4.7/geomanager/errors.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/fields.py` & `geomanager-0.4.7/geomanager/fields.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/forms/boundary.py` & `geomanager-0.4.7/geomanager/forms/boundary.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/forms/raster_file.py` & `geomanager-0.4.7/geomanager/forms/raster_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/forms/raster_style.py` & `geomanager-0.4.7/geomanager/forms/raster_style.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/forms/vector_file.py` & `geomanager-0.4.7/geomanager/forms/vector_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/helpers.py` & `geomanager-0.4.7/geomanager/helpers.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/am/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/ar/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/en/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/es/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/fr/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/locale/sw/LC_MESSAGES/django.po` & `geomanager-0.4.7/geomanager/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/management/commands/ingest_geomanager_raster.py` & `geomanager-0.4.7/geomanager/management/commands/ingest_geomanager_raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/management/commands/initialize_geomanager.py` & `geomanager-0.4.7/geomanager/management/commands/initialize_geomanager.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/management/commands/process_geomanager_layer_directory.py` & `geomanager-0.4.7/geomanager/management/commands/process_geomanager_layer_directory.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0001_initial.py` & `geomanager-0.4.7/geomanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0001_squashed_0024_rastertilelayer_get_time_from_tile_json_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0001_squashed_0024_rastertilelayer_get_time_from_tile_json_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0002_geomanagersettings_logo_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0002_geomanagersettings_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0004_alter_dataset_can_clip.py` & `geomanager-0.4.7/geomanager/migrations/0004_alter_dataset_can_clip.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0005_delete_countryboundary_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0005_delete_countryboundary_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0006_stationsettings.py` & `geomanager-0.4.7/geomanager/migrations/0006_stationsettings.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0007_remove_stationsettings_id_field_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0011_vectorlayericon.py` & `geomanager-0.4.7/geomanager/migrations/0011_vectorlayericon.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py` & `geomanager-0.4.7/geomanager/migrations/0012_geomanagersettings_crop_raster_to_country.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0013_geomanagersettings_logo_external_link_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0014_geomanagersettings_privacy_policy_page_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0015_wmslayer_request_time_from_capabilities.py` & `geomanager-0.4.7/geomanager/migrations/0015_wmslayer_request_time_from_capabilities.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0016_wmslayer_date_format.py` & `geomanager-0.4.7/geomanager/migrations/0016_wmslayer_date_format.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0017_wmslayer_more_info_alter_wmslayer_date_format.py` & `geomanager-0.4.7/geomanager/migrations/0017_wmslayer_more_info_alter_wmslayer_date_format.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0018_wmslayer_custom_get_capabilities_url.py` & `geomanager-0.4.7/geomanager/migrations/0018_wmslayer_custom_get_capabilities_url.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0019_wmslayer_get_capabilities_layer_name_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0019_wmslayer_get_capabilities_layer_name_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0020_tmslayer.py` & `geomanager-0.4.7/geomanager/migrations/0020_tmslayer.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0021_rasterfilelayer_rastertilelayer_vectorfilelayer_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0021_rasterfilelayer_rastertilelayer_vectorfilelayer_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0022_alter_rastertilelayer_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0022_alter_rastertilelayer_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0023_vectortilelayericon.py` & `geomanager-0.4.7/geomanager/migrations/0023_vectortilelayericon.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0024_rastertilelayer_get_time_from_tile_json_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0024_rastertilelayer_get_time_from_tile_json_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0025_alter_areaofinterest_options_alter_category_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0025_alter_areaofinterest_options_alter_category_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0026_layerrasterfile_raster_metadata_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0026_layerrasterfile_raster_metadata_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0027_alter_layerrasterfile_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0027_alter_layerrasterfile_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0028_alter_pgvectortable_options_alter_dataset_category.py` & `geomanager-0.4.7/geomanager/migrations/0028_alter_pgvectortable_options_alter_dataset_category.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0031_remove_geomanagersettings_cap_auto_refresh_interval_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0031_remove_geomanagersettings_cap_auto_refresh_interval_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0032_rasterfilelayer_auto_ingest_nc_data_variable.py` & `geomanager-0.4.7/geomanager/migrations/0032_rasterfilelayer_auto_ingest_nc_data_variable.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0033_alter_layerrasterfile_file_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0033_alter_layerrasterfile_file_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0034_rastertilelayer_time_parameter_name_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0034_rastertilelayer_time_parameter_name_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0035_vectortilelayer_render_layers_json_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0035_vectortilelayer_render_layers_json_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0036_vectortilelayer_popup_config_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0036_vectortilelayer_popup_config_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0037_dataset_enable_all_multi_layers_on_add.py` & `geomanager-0.4.7/geomanager/migrations/0037_dataset_enable_all_multi_layers_on_add.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0038_rasterfilelayer_legend_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0038_rasterfilelayer_legend_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0039_rasterfilelayer_order_rastertilelayer_order_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0039_rasterfilelayer_order_rastertilelayer_order_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0040_alter_rasterfilelayer_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0040_alter_rasterfilelayer_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0041_dataset_order_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0041_dataset_order_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0042_alter_dataset_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0042_alter_dataset_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0043_additionalmapboundarydata.py` & `geomanager-0.4.7/geomanager/migrations/0043_additionalmapboundarydata.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0044_alter_additionalmapboundarydata_options_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0044_alter_additionalmapboundarydata_options_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0045_additionalmapboundarydata_active_and_more.py` & `geomanager-0.4.7/geomanager/migrations/0045_additionalmapboundarydata_active_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/migrations/0046_colorvalue_show_on_legend_rasterstyle_legend_type.py` & `geomanager-0.4.7/geomanager/migrations/0046_colorvalue_show_on_legend_rasterstyle_legend_type.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/__init__.py` & `geomanager-0.4.7/geomanager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/aoi.py` & `geomanager-0.4.7/geomanager/models/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/boundary.py` & `geomanager-0.4.7/geomanager/models/boundary.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/core.py` & `geomanager-0.4.7/geomanager/models/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     panels = [
         FieldPanel("title"),
         FieldPanel("active"),
         FieldPanel("public"),
     ]
 
     def __str__(self):
-        return self.title
+        return f"{self.title} - {self.category.title}"
 
 
 class Dataset(TimeStampedModel, AdminSortable):
     DATASET_TYPE_CHOICES = (
         ("raster_file", _("Raster File - NetCDF/GeoTiff")),
         ("vector_file", _("Vector File - Shapefile, Geojson")),
         ("wms", _("Web Map Service - WMS Layer")),
@@ -308,14 +308,29 @@
     def has_layers(self):
         layers = self.get_layers_rel()
         if layers:
             return layers.exists()
 
         return False
 
+    @property
+    def requires_file_upload(self):
+        return self.layer_type in ["raster_file", "vector_file"]
+
+    @property
+    def has_files(self):
+        if self.requires_file_upload:
+            if self.layer_type == "raster_file":
+                return self.has_raster_files()
+
+            if self.layer_type == "vector_file":
+                return self.has_vector_tables()
+
+        return False
+
     def can_preview(self):
         layers_check = [
             self.has_raster_files(),
             self.has_vector_tables(),
             self.has_wms_layers(),
             self.has_raster_tile_layers(),
             self.has_vector_tile_layers()
@@ -474,9 +489,7 @@
                 self.dataset.layers.filter(default=True).exclude(pk=self.pk).update(default=False)
             else:
                 if not self.dataset.layers.filter(default=True).exclude(pk=self.pk).exists():
                     self.default = True
                     self.dataset.layers.filter(default=True).exclude(pk=self.pk).update(default=False)
 
         super().save(*args, **kwargs)
-
-
```

### Comparing `geomanager-0.4.6/geomanager/models/geomanager_settings.py` & `geomanager-0.4.7/geomanager/models/geomanager_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from django import forms
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from modelcluster.models import ClusterableModel
 from wagtail import blocks
 from wagtail.admin.panels import (
     FieldPanel,
     TabbedInterface,
-    ObjectList
+    ObjectList, MultiFieldPanel
 )
 from wagtail.api.v2.utils import get_full_url
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 from wagtail.fields import StreamField
 from wagtail.images.blocks import ImageChooserBlock
 from wagtail.models import Page
@@ -71,21 +72,51 @@
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name='+',
         verbose_name=_("Privacy Policy Page"),
         help_text=_("MapViewer Privacy Policy Page")
     )
+    contact_us_page = models.ForeignKey(
+        Page,
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='+',
+        verbose_name=_("Contact Us Page")
+    )
 
     navigation = StreamField([
         ('menu_items', blocks.ListBlock(NavigationItemsBlock(max_num=8))),
     ], block_counts={
         'menu_items': {'max_num': 1},
     }, use_json_field=True, null=True, blank=True)
 
+    map_disclaimer_text = models.CharField(max_length=350, blank=True, null=True,
+                                           default="The boundaries and names shown and the designations used on this "
+                                                   "map do not imply the expression of any opinion whatsoever "
+                                                   "concerning the legal status of any country, territory, city or "
+                                                   "area or of its authorities, or concerning the delimitation of its "
+                                                   "frontiers or boundaries",
+                                           verbose_name=_("Map Disclaimer Text"),
+                                           help_text=_("MapViewer Map disclaimer text. Maximum of 350 characters. "
+                                                       "Add more details in the Map Disclaimer Page and link it below"))
+    map_disclaimer_page = models.ForeignKey(
+        Page,
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='+',
+        verbose_name=_("Map Disclaimer Page"),
+        help_text=_("MapViewer Map disclaimer page for more details")
+    )
+
+    enable_my_account = models.BooleanField(default=False, verbose_name=_("Enable My Account"))
+    allow_signups = models.BooleanField(default=False, verbose_name=_("Allow user signups"))
+
     base_maps = StreamField([
         ('basemap', blocks.StructBlock([
             ('label', blocks.CharBlock(label=_("label"))),
             ('backgroundColor', blocks.CharBlock(label=_("background color"))),
             ('image', ImageChooserBlock(required=False, label=_("image"))),
             ('basemapGroup', blocks.CharBlock(label=_("basemap group"))),
             ('labelsGroup', blocks.CharBlock(label=_("labels group"))),
@@ -109,16 +140,27 @@
         ], heading=_("Basemap TileServer Settings")),
         ObjectList([
             FieldPanel("logo"),
             FieldPanel("logo_page"),
             FieldPanel("logo_external_link"),
             FieldPanel("terms_of_service_page"),
             FieldPanel("privacy_policy_page"),
+            FieldPanel("contact_us_page"),
             FieldPanel("navigation"),
+
+            MultiFieldPanel([
+                FieldPanel("map_disclaimer_text", widget=forms.Textarea(attrs={'rows': 3})),
+                FieldPanel("map_disclaimer_page")
+            ], heading=_("Map Disclaimer Settings")),
+
         ], heading=_("Navigation Settings")),
+        ObjectList([
+            FieldPanel("enable_my_account"),
+            FieldPanel("allow_signups"),
+        ], heading=_("My Account Settings")),
     ])
 
     @property
     def max_upload_size_bytes(self):
         return self.max_upload_size_mb * 1024 * 1024
 
     @property
```

### Comparing `geomanager-0.4.6/geomanager/models/geostore.py` & `geomanager-0.4.7/geomanager/models/geostore.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/profile.py` & `geomanager-0.4.7/geomanager/models/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/raster_file.py` & `geomanager-0.4.7/geomanager/models/raster_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,18 @@
         }
 
         if self.date_format:
             if self.date_format == "pentadal":
                 time_config.update({
                     "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "pentadal"},
                 })
+            elif self.date_format == "dekadal":
+                time_config.update({
+                    "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "dekadal"},
+                })
             else:
                 time_config.update({
                     "dateFormat": {"currentTime": self.date_format},
                 })
         else:
             time_config.update({
                 "dateFormat": {"currentTime": "yyyy-MM-dd HH:mm"},
@@ -361,9 +365,7 @@
     panels = [
         FieldPanel("layer"),
         FieldPanel("file"),
     ]
 
     def __str__(self):
         return f"{self.dataset} - {self.created}"
-
-
```

### Comparing `geomanager-0.4.6/geomanager/models/raster_style.py` & `geomanager-0.4.7/geomanager/models/raster_style.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from modelcluster.models import ClusterableModel
 from wagtail.admin.panels import FieldPanel, FieldRowPanel, MultiFieldPanel, InlinePanel
 from wagtail.models import Orderable
 from wagtail_color_panel.edit_handlers import NativeColorPanel
 from wagtail_color_panel.fields import ColorField
 
 from geomanager.forms import RasterStyleModelForm
+from geomanager.utils import significant_digits, round_to_precision
 from geomanager.widgets import RasterStyleWidget
 
 
 class RasterStyle(TimeStampedModel, ClusterableModel):
     LEGEND_TYPE_CHOICES = (
         ("basic", _("Basic")),
-        ("choropleth", _("Choropleth")),
-        ("gradient", _("Gradient")),
+        ("choropleth", _("Choropleth Horizontal")),
+        ("choropleth_vertical", _("Choropleth Vertical")),
+        ("gradient", _("Gradient Horizontal")),
+        ("gradient_vertical", _("Gradient Vertical")),
     )
 
     base_form_class = RasterStyleModelForm
 
     name = models.CharField(max_length=256, verbose_name=_("name"),
                             help_text=_("Style name for identification"))
     unit = models.CharField(max_length=100, blank=True, null=True, verbose_name=_("data unit"),
@@ -29,15 +32,15 @@
     min = models.IntegerField(default=0, verbose_name=_("minimum value"), help_text=_("minimum value"))
     max = models.IntegerField(default=100, verbose_name=_("maximum value"), help_text=_("maximum value"))
     steps = models.IntegerField(default=5, validators=[MinValueValidator(3), MaxValueValidator(20), ], null=True,
                                 blank=True, verbose_name=_("steps"), help_text=_("Number of steps"))
     use_custom_colors = models.BooleanField(default=False, verbose_name=_("Use Custom Colors"))
     palette = models.TextField(blank=True, null=True, verbose_name=_("Color Palette"))
     interpolate = models.BooleanField(default=False, verbose_name=_("interpolate"), help_text="Interpolate colorscale")
-    legend_type = models.CharField(max_length=100, choices=LEGEND_TYPE_CHOICES, default="choropleth",
+    legend_type = models.CharField(max_length=100, choices=LEGEND_TYPE_CHOICES, default="choropleth_vertical",
                                    verbose_name=_("Legend Type"))
     custom_color_for_rest = ColorField(blank=True, null=True, default="#ff0000",
                                        verbose_name=_("Color for the rest of values"),
                                        help_text=_(
                                            "Color for values greater than the values defined above, "
                                            "as well as values greater than the maximum defined value"))
 
@@ -93,27 +96,73 @@
     def offset_value(self):
         return -self.min_value
 
     @property
     def clip_value(self):
         return self.max_value + self.offset_value
 
+    @property
+    def palette_legend_values(self):
+        if self.use_custom_colors:
+            return None
+
+        colors = self.get_palette_list()
+        step = (self.max - self.min) / (len(colors) - (2 if self.min > 0 else 1))
+        precision = significant_digits(step, self.max)
+        value_format = round_to_precision(precision)
+
+        val_from = self.min
+        val_to = value_format(self.min + step)
+
+        items = []
+
+        for i, color in enumerate(colors):
+            item = {"color": color}
+
+            if i == 0 and self.min > 0:
+                item.update({
+                    "from": 0,
+                    "to": self.min,
+                    "name": "< {}".format(self.min)
+                })
+                val_to = self.min
+
+            elif val_from < self.max:
+                item.update({
+                    "from": round(val_from, 1),
+                    "to": round(val_to, 1),
+                    "name": "{} - {}".format(val_from, val_to)
+                })
+            else:
+                item.update({
+                    "from": val_from,
+                    "name": "> {}".format(val_from)
+                })
+
+            val_from = val_to
+            val_to = value_format(self.min + step * (i + (1 if self.min > 0 else 2)))
+
+            items.append(item)
+
+        return items
+
     def get_custom_color_values(self):
         values = []
         color_values = self.color_values.order_by('threshold')
 
         for i, c_value in enumerate(color_values):
             value = c_value.value
             # if not the first one, add prev value for later comparison
             if i == 0:
                 value["min_value"] = None
             else:
                 value["min_value"] = color_values[i - 1].threshold
             value["max_value"] = value["threshold"]
             values.append(value)
+
         return values
 
     def get_custom_palette(self):
         colors = []
         for i in range(256):
             color = self.get_color_for_index(i)
             colors.append(color)
@@ -167,34 +216,46 @@
                 }
             ]
         }
         return style
 
     def get_legend_config(self):
         items = []
+        legend_type = self.legend_type
         if self.use_custom_colors:
             values = self.get_custom_color_values()
             count = len(values)
 
-            if count > 1:
+            if count > 0:
                 for value in values:
                     item = {
                         "name": "",
                         "color": value['color']
                     }
                     if value.get("show_on_legend"):
                         item.update({
                             "name": value['label'] if value.get('label') else value['threshold'],
                         })
-
                     items.append(item)
-                rest_item = {"name": "", "color": self.custom_color_for_rest}
-                items.append(rest_item)
 
-        return {"type": self.legend_type, "items": items}
+                # if only one item and it is the custom color for rest, then show it as basic legend
+                # no matter what the legend type was set
+                if count == 1 and items[0].get("color") == self.custom_color_for_rest:
+                    legend_type = "basic"
+                else:
+                    rest_item = {"name": "", "color": self.custom_color_for_rest}
+                    items.append(rest_item)
+        else:
+            items = self.palette_legend_values
+
+        config = {"type": legend_type, "items": items, }
+
+        if self.unit:
+            config["units"] = self.unit
+        return config
 
 
 class ColorValue(TimeStampedModel, Orderable):
     layer = ParentalKey(RasterStyle, related_name='color_values')
     threshold = models.FloatField(verbose_name=_("Threshold value"), help_text=_(
         "Values less than or equal to the input value, will be assigned the chosen color"))
     color = ColorField(default="#ff0000", verbose_name=_("color"))
```

### Comparing `geomanager-0.4.6/geomanager/models/raster_tile.py` & `geomanager-0.4.7/geomanager/models/raster_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/tile_base.py` & `geomanager-0.4.7/geomanager/models/tile_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,14 +179,18 @@
             }
 
             if self.date_format:
                 if self.date_format == "pentadal":
                     time_config.update({
                         "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "pentadal"},
                     })
+                elif self.date_format == "dekadal":
+                    time_config.update({
+                        "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "dekadal"},
+                    })
                 else:
                     time_config.update({
                         "dateFormat": {"currentTime": self.date_format},
                     })
             else:
                 time_config.update({
                     "dateFormat": {"currentTime": "yyyy-MM-dd HH:mm"},
```

### Comparing `geomanager-0.4.6/geomanager/models/tile_gl.py` & `geomanager-0.4.7/geomanager/models/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/vector_file.py` & `geomanager-0.4.7/geomanager/models/vector_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/vector_tile.py` & `geomanager-0.4.7/geomanager/models/vector_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/models/wms.py` & `geomanager-0.4.7/geomanager/models/wms.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,14 +252,18 @@
             }
 
             if self.date_format:
                 if self.date_format == "pentadal":
                     time_config.update({
                         "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "pentadal"},
                     })
+                elif self.date_format == "dekadal":
+                    time_config.update({
+                        "dateFormat": {"currentTime": "MMM yyyy", "asPeriod": "dekadal"},
+                    })
                 else:
                     time_config.update({
                         "dateFormat": {"currentTime": self.date_format},
                     })
             else:
                 time_config.update({
                     "dateFormat": {"currentTime": "yyyy-MM-dd HH:mm"},
```

### Comparing `geomanager-0.4.6/geomanager/samples/basemaps/basemaps.json` & `geomanager-0.4.7/geomanager/samples/basemaps/basemaps.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/samples/basemaps/style.json` & `geomanager-0.4.7/geomanager/samples/basemaps/style.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/aoi.py` & `geomanager-0.4.7/geomanager/serializers/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/auth.py` & `geomanager-0.4.7/geomanager/serializers/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/core.py` & `geomanager-0.4.7/geomanager/serializers/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/geostore.py` & `geomanager-0.4.7/geomanager/serializers/geostore.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/profile.py` & `geomanager-0.4.7/geomanager/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/raster_file.py` & `geomanager-0.4.7/geomanager/serializers/raster_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/raster_tile.py` & `geomanager-0.4.7/geomanager/serializers/raster_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/vector_file.py` & `geomanager-0.4.7/geomanager/serializers/vector_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/vector_tile.py` & `geomanager-0.4.7/geomanager/serializers/vector_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/serializers/wms.py` & `geomanager-0.4.7/geomanager/serializers/wms.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/css/bulma-navbar.css` & `geomanager-0.4.7/geomanager/static/geomanager/css/bulma-navbar.css`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/css/vendor/maplibre-gl.css` & `geomanager-0.4.7/geomanager/static/geomanager/css/vendor/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/images/geomapviewer-logo.png` & `geomanager-0.4.7/geomanager/static/geomanager/images/geomapviewer-logo.png`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/add-multiple.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/colorbrewer.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/colorbrewer.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/dataset-form-conditional.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/dataset-form-conditional.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/mbt_source_extra.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/mbt_source_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/raster-file-conditional.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/raster-file-conditional.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/raster-file-preview.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/raster-file-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/raster-tile-preview.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/raster-tile-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/raster_style_extra.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/raster_style_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/raster_tile_layer_form.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/raster_tile_layer_form.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vector-file-preview.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vector-file-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vector-tile-conditional.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vector-tile-conditional.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vector-tile-preview.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vector-tile-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vendor/d3-format.min.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vendor/d3-format.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vendor/maplibre-gl.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vendor/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/vendor/ol.min.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/vendor/ol.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/widgets/icon_chooser.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/widgets/icon_chooser.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/widgets/raster_style_widget.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/widgets/raster_style_widget.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/static/geomanager/js/wms-preview.js` & `geomanager-0.4.7/geomanager/static/geomanager/js/wms-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/boundary/additional_boundary_create.html` & `geomanager-0.4.7/geomanager/templates/geomanager/boundary/additional_boundary_create.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/boundary/boundary_landing.html` & `geomanager-0.4.7/geomanager/templates/geomanager/boundary/boundary_landing.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/modeladmin/index_without_custom_create.html` & `geomanager-0.4.7/geomanager/templates/geomanager/modeladmin/index_without_custom_create.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/navbar.html` & `geomanager-0.4.7/geomanager/templates/geomanager/navbar.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_edit_form.html` & `geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_layer_preview.html` & `geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_layer_preview.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% block content %}
     {% if navigation_items %}
         {% breadcrumbs_component navigation_items %}
     {% endif %}
 
     {% translate "Preview" as preview_str %}
 
-    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
+    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:selected_layer.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
         <div class="w-field__input" data-field-input="" style="display: none">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 {% translate "Select Layer" %}
             </label>
             <select name="select" id="layer_select">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 wagtailadmin_tags wagtailimages_tags static geomanager_tags %} {% block
 titletag %} {% blocktranslate trimmed with title=page.get_admin_display_title
 %} Preview Layer {{ title }} {% endblocktranslate %} {% endblock %} {% block
 extra_css %} {{ block.super }} {{ form_media.css }}
 {% endblock %} {% block content %} {% if navigation_items %} {%
 breadcrumbs_component navigation_items %} {% endif %} {% translate "Preview" as
 preview_str %} {% include "wagtailadmin/shared/header.html" with
-title=preview_str|add:" - "|add:dataset.title
+title=preview_str|add:" - "|add:selected_layer.title
 subtitle=page.get_admin_display_title icon="view" %}
 {% for layer in dataset.raster_file_layers.all %}
 % if layer.style %}data-hasstyle="1"{% endif %} {% if selected_layer and
 selected_layer.pk == layer.pk %}selected{% endif %}>{{ layer.title }}
 {% endfor %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }}
 {% endblock %}
```

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/raster_file/raster_file_upload.html` & `geomanager-0.4.7/geomanager/templates/geomanager/raster_file/raster_file_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/raster_tile/raster_tile_layer_preview.html` & `geomanager-0.4.7/geomanager/templates/geomanager/raster_tile/raster_tile_layer_preview.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     {% if navigation_items %}
         {% breadcrumbs_component navigation_items %}
     {% endif %}
 
 
     {% trans "Preview" as preview_str %}
 
-    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
+    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:selected_layer.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
         <div class="w-field__input" data-field-input="" style="display: none">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 {% translate "Select Layer" %}
             </label>
             <select name="select" id="layer_select">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 wagtailadmin_tags wagtailimages_tags static geomanager_tags %} {% block
 titletag %} {% blocktranslate trimmed with title=page.get_admin_display_title
 %} Preview Layers {{ title }} {% endblocktranslate %} {% endblock %} {% block
 extra_css %} {{ block.super }} {{ form_media.css }}
 {% endblock %} {% block content %} {% if navigation_items %} {%
 breadcrumbs_component navigation_items %} {% endif %} {% trans "Preview" as
 preview_str %} {% include "wagtailadmin/shared/header.html" with
-title=preview_str|add:" - "|add:dataset.title
+title=preview_str|add:" - "|add:selected_layer.title
 subtitle=page.get_admin_display_title icon="view" %}
 {% for layer in dataset.raster_tile_layers.all %}
 % if selected_layer and selected_layer.pk == layer.pk %}selected{% endif %}>{
 { layer.title }}
 {% endfor %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }}
 {% endblock %}
```

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/shared/breadcrumbs.html` & `geomanager-0.4.7/geomanager/templates/geomanager/shared/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_edit_form.html` & `geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_layer_preview.html` & `geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_layer_preview.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 {% block content %}
     {% if navigation_items %}
         {% breadcrumbs_component navigation_items %}
     {% endif %}
 
     {% translate "Preview" as preview_str %}
 
-    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
+    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:selected_layer.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
         <div class="w-field__input" data-field-input="" style="display: none">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 {% translate "Select Layer" %}
             </label>
             <select name="select" id="layer_select">
```

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/vector_file/vector_file_upload.html` & `geomanager-0.4.7/geomanager/templates/geomanager/vector_file/vector_file_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/vector_tile/vector_tile_layer_preview.html` & `geomanager-0.4.7/geomanager/templates/geomanager/vector_tile/vector_tile_layer_preview.html`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 {% block content %}
     {% if navigation_items %}
         {% breadcrumbs_component navigation_items %}
     {% endif %}
 
     {% trans "Preview" as preview_str %}
 
-    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
+    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:selected_layer.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
         <div class="w-field__input" data-field-input="" style="display: none">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 {% translate "Select Layer" %}
             </label>
             <select name="select" id="layer_select">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 wagtailadmin_tags wagtailimages_tags static geomanager_tags %} {% block
 titletag %} {% blocktranslate trimmed with title=page.get_admin_display_title
 %} Preview Layers {{ title }} {% endblocktranslate %} {% endblock %} {% block
 extra_css %} {{ block.super }} {{ form_media.css }}
 {% endblock %} {% block content %} {% if navigation_items %} {%
 breadcrumbs_component navigation_items %} {% endif %} {% trans "Preview" as
 preview_str %} {% include "wagtailadmin/shared/header.html" with
-title=preview_str|add:" - "|add:dataset.title
+title=preview_str|add:" - "|add:selected_layer.title
 subtitle=page.get_admin_display_title icon="view" %}
 {% for layer in dataset.vector_tile_layers.all %}
 % if selected_layer and selected_layer.pk == layer.pk %}selected{% endif %}>{
 { layer.title }}
 {% endfor %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }}
 {% endblock %}
```

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/widgets/raster_style_widget.html` & `geomanager-0.4.7/geomanager/templates/geomanager/widgets/raster_style_widget.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         display: inline-block;
         height: 100%;
         width: 100%
     }
 
     #legend-content table tr td {
         padding-left: 8px;
-        line-height: 24px;
         font-size: 14px;
     }
 
 </style>
 
 <script>
     const instanceColorPalette = "{% if widget.value != None %}{{ widget.value|stringformat:'s' }}{% endif %}"
```

### Comparing `geomanager-0.4.6/geomanager/templates/geomanager/wms/wms_layer_preview.html` & `geomanager-0.4.7/geomanager/templates/geomanager/wms/wms_layer_preview.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {% block content %}
     {% if navigation_items %}
         {% breadcrumbs_component navigation_items %}
     {% endif %}
 
     {% trans "Preview" as preview_str %}
 
-    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:dataset.title subtitle=page.get_admin_display_title icon="view" %}
+    {% include "wagtailadmin/shared/header.html" with title=preview_str|add:" - "|add:selected_layer.title subtitle=page.get_admin_display_title icon="view" %}
 
     <div class="nice-padding">
 
         <div class="w-field__input" data-field-input="">
             <label class="w-field__label" for="layer_select" id="layer_select-label">
                 {% translate "Select Layer" %}
             </label>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 wagtailadmin_tags wagtailimages_tags static geomanager_tags %} {% block
 titletag %} {% blocktranslate trimmed with title=page.get_admin_display_title
 %} Preview Layers {{ title }} {% endblocktranslate %} {% endblock %} {% block
 extra_css %} {{ block.super }} {{ form_media.css }}
 {% endblock %} {% block content %} {% if navigation_items %} {%
 breadcrumbs_component navigation_items %} {% endif %} {% trans "Preview" as
 preview_str %} {% include "wagtailadmin/shared/header.html" with
-title=preview_str|add:" - "|add:dataset.title
+title=preview_str|add:" - "|add:selected_layer.title
 subtitle=page.get_admin_display_title icon="view" %}
 {% for layer in dataset.wms_layers.all %}
 % if selected_layer and selected_layer.pk == layer.pk %}selected{% endif %}>{
 { layer.title }}
 {% endfor %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }}
 {% endblock %}
```

### Comparing `geomanager-0.4.6/geomanager/urls.py` & `geomanager-0.4.7/geomanager/urls.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/boundary.py` & `geomanager-0.4.7/geomanager/utils/boundary.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/ingest.py` & `geomanager-0.4.7/geomanager/utils/ingest.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/raster_utils.py` & `geomanager-0.4.7/geomanager/utils/raster_utils.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/svg.py` & `geomanager-0.4.7/geomanager/utils/svg.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/tile_gl.py` & `geomanager-0.4.7/geomanager/utils/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/tiles.py` & `geomanager-0.4.7/geomanager/utils/tiles.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/utils/vector_utils.py` & `geomanager-0.4.7/geomanager/utils/vector_utils.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/validators.py` & `geomanager-0.4.7/geomanager/validators.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/__init__.py` & `geomanager-0.4.7/geomanager/views/__init__.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/auth.py` & `geomanager-0.4.7/geomanager/views/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/boundary.py` & `geomanager-0.4.7/geomanager/views/boundary.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/core.py` & `geomanager-0.4.7/geomanager/views/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,48 @@
     gm_settings = GeomanagerSettings.for_request(request)
     abm_settings = AdminBoundarySettings.for_request(request)
 
     categories = Category.objects.all()
     categories_data = CategorySerializer(categories, many=True).data
     response = {
         "categories": categories_data,
+        "enableMyAccount": False,
+        "allowSignups": False,
     }
 
+    if gm_settings.enable_my_account:
+        response.update({
+            "enableMyAccount": True,
+        })
+
+    if gm_settings.allow_signups:
+        response.update({
+            "allowSignups": True,
+        })
+
+    if gm_settings.map_disclaimer_text:
+        response.update({"disclaimerText": gm_settings.map_disclaimer_text})
+
     links = {
         "mapViewerBaseUrl": get_full_url(request, (reverse("mapview"))),
     }
 
     if gm_settings.terms_of_service_page:
-        links.update({"termsOfServicePageUrl": get_full_url(request, gm_settings.terms_of_service_page.url)})
+        links.update(
+            {"termsOfServicePageUrl": get_full_url(request, gm_settings.terms_of_service_page.get_full_url(request))})
 
     if gm_settings.privacy_policy_page:
-        links.update({"privacyPolicyPageUrl": get_full_url(request, gm_settings.privacy_policy_page.url)})
+        links.update(
+            {"privacyPolicyPageUrl": get_full_url(request, gm_settings.privacy_policy_page.get_full_url(request))})
+
+    if gm_settings.map_disclaimer_page:
+        links.update({"disclaimerPageUrl": gm_settings.map_disclaimer_page.get_full_url(request)})
+
+    if gm_settings.contact_us_page:
+        links.update({"contactUsPageUrl": gm_settings.contact_us_page.get_full_url(request)})
 
     response.update({"links": links})
 
     icon_images = []
     for icon in VectorLayerIcon.objects.all():
         icon_images.append({"name": icon.name, "url": get_full_url(request, icon.file.url)})
```

### Comparing `geomanager-0.4.6/geomanager/views/nextjs.py` & `geomanager-0.4.7/geomanager/views/nextjs.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/profile.py` & `geomanager-0.4.7/geomanager/views/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/raster_file.py` & `geomanager-0.4.7/geomanager/views/raster_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/raster_tile.py` & `geomanager-0.4.7/geomanager/views/raster_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/tile_gl.py` & `geomanager-0.4.7/geomanager/views/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/vector_file.py` & `geomanager-0.4.7/geomanager/views/vector_file.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/vector_tile.py` & `geomanager-0.4.7/geomanager/views/vector_tile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/views/wms.py` & `geomanager-0.4.7/geomanager/views/wms.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/viewsets/aoi.py` & `geomanager-0.4.7/geomanager/viewsets/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/viewsets/core.py` & `geomanager-0.4.7/geomanager/viewsets/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,28 +21,36 @@
         context.update({'request': self.request})
         return context
 
     def list(self, request, *args, **kwargs):
         queryset = self.get_queryset()
         dataset_with_layers = []
 
+        datasets = []
+
+        # get datasets from registered hooks
+        for fn in hooks.get_hooks(geomanager_register_datasets_hook_name):
+            hook_datasets = fn(request)
+            if isinstance(hook_datasets, list):
+                for dataset in hook_datasets:
+                    datasets.append(dataset)
+
         # get only datasets with layers defined
         for dataset in queryset:
             if dataset.has_layers():
+                # if dataset requires file upload, but has no files, skip
+                if dataset.requires_file_upload and not dataset.has_files:
+                    continue
                 dataset_with_layers.append(dataset)
 
         serializer = self.get_serializer(dataset_with_layers, many=True)
+        geomanager_datasets = serializer.data
 
-        datasets = serializer.data
-
-        # get datasets from registered hooks
-        for fn in hooks.get_hooks(geomanager_register_datasets_hook_name):
-            hook_datasets = fn(request)
-            for dataset in hook_datasets:
-                datasets.append(dataset)
+        if geomanager_datasets:
+            datasets.extend(geomanager_datasets)
 
         return Response(datasets)
 
 
 class MetadataViewSet(mixins.RetrieveModelMixin, viewsets.GenericViewSet):
     queryset = Metadata.objects.all()
     serializer_class = serializers.MetadataSerialiazer
```

### Comparing `geomanager-0.4.6/geomanager/viewsets/raster.py` & `geomanager-0.4.7/geomanager/viewsets/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager/viewsets/vector.py` & `geomanager-0.4.7/geomanager/viewsets/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,16 @@
 
 
 class GeostoreViewSet(viewsets.ViewSet):
     renderer_classes = [JSONRenderer]
 
     @action(detail=True, methods=['post'])
     def post(self, request):
-        # parse the GeoJSON from the POST data
-        payload = json.loads(request.body.decode('utf-8'))
 
+        payload = request.data
         geojson = payload.get("geojson")
 
         # extract the MultiPolygon geometry from the GeoJSON
         geometry = geojson['geometry']
         geom = GEOSGeometry(json.dumps(geometry))
 
         if geom.geom_type == "Polygon":
```

### Comparing `geomanager-0.4.6/geomanager/wagtail_hooks.py` & `geomanager-0.4.7/geomanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/geomanager.egg-info/PKG-INFO` & `geomanager-0.4.7/geomanager.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.4.6
+Version: 0.4.7
 Summary: Wagtail based Geospatial Data Manager
-Home-page: https://github.com/wmo-raf/geomanager
+Home-page: https://github.com/erick-otenyo/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -212,7 +212,19 @@
 # Including the Map Viewer
 
 This package is the backend component to the frontend [geomapviewer](https://github.com/wmo-raf/geomapviewer).
 
 # Documentation
 
 TODO
+
+# Maintainer ✨
+
+**GeoManager** is built with 💛 by [Erick Otenyo](https://github.com/erick-otenyo).
+
+Your support and feedback are valuable in maintaining and improving the package.
+
+<a href="https://www.linkedin.com/in/erick-otenyo" target="_blank"><img src="images/linkedin.png" alt="logo" width="150"></a>
+<a href="https://www.buymeacoffee.com/erick_otenyo" target="_blank"><img src="images/buymeacoffe.png" alt="logo" width="150"></a>
+<a href="https://twitter.com/erick_otenyo" target="_blank"><img src="images/twitter.png" alt="logo" width="150"></a>
+
+<a href="https://www.buymeacoffee.com/erick_otenyo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geomanager-0.4.6/geomanager.egg-info/SOURCES.txt` & `geomanager-0.4.7/geomanager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,18 @@
 geomanager/migrations/0040_alter_rasterfilelayer_options_and_more.py
 geomanager/migrations/0041_dataset_order_and_more.py
 geomanager/migrations/0042_alter_dataset_options_and_more.py
 geomanager/migrations/0043_additionalmapboundarydata.py
 geomanager/migrations/0044_alter_additionalmapboundarydata_options_and_more.py
 geomanager/migrations/0045_additionalmapboundarydata_active_and_more.py
 geomanager/migrations/0046_colorvalue_show_on_legend_rasterstyle_legend_type.py
+geomanager/migrations/0047_geomanagersettings_map_disclaimer_page_and_more.py
+geomanager/migrations/0048_alter_geomanagersettings_map_disclaimer_text.py
+geomanager/migrations/0049_geomanagersettings_allow_signups_and_more.py
+geomanager/migrations/0050_geomanagersettings_contact_us_page.py
 geomanager/migrations/__init__.py
 geomanager/models/__init__.py
 geomanager/models/aoi.py
 geomanager/models/boundary.py
 geomanager/models/core.py
 geomanager/models/geomanager_settings.py
 geomanager/models/geostore.py
@@ -144,35 +148,39 @@
 geomanager/static/geomanager/js/colorbrewer.js
 geomanager/static/geomanager/js/dataset-form-conditional.js
 geomanager/static/geomanager/js/mbt_source_extra.js
 geomanager/static/geomanager/js/raster-file-conditional.js
 geomanager/static/geomanager/js/raster-file-preview.js
 geomanager/static/geomanager/js/raster-tile-preview.js
 geomanager/static/geomanager/js/raster_style_extra.js
+geomanager/static/geomanager/js/raster_style_index_extra.js
 geomanager/static/geomanager/js/raster_tile_layer_form.js
 geomanager/static/geomanager/js/vector-file-preview.js
 geomanager/static/geomanager/js/vector-tile-conditional.js
 geomanager/static/geomanager/js/vector-tile-preview.js
 geomanager/static/geomanager/js/wms-preview.js
 geomanager/static/geomanager/js/vendor/d3-format.min.js
+geomanager/static/geomanager/js/vendor/d3.min.js
 geomanager/static/geomanager/js/vendor/maplibre-gl.js
 geomanager/static/geomanager/js/vendor/ol.min.js
 geomanager/static/geomanager/js/widgets/icon_chooser.js
 geomanager/static/geomanager/js/widgets/raster_style_widget.js
 geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
+geomanager/templates/adminsortable/index_without_create_button.html
 geomanager/templates/django_nextjs/mapviewer.html
 geomanager/templates/geomanager/navbar.html
 geomanager/templates/geomanager/boundary/additional_boundary_create.html
 geomanager/templates/geomanager/boundary/additional_boundary_delete.html
 geomanager/templates/geomanager/boundary/additional_boundary_edit.html
 geomanager/templates/geomanager/boundary/boundary_landing.html
 geomanager/templates/geomanager/modeladmin/create.html
 geomanager/templates/geomanager/modeladmin/edit.html
 geomanager/templates/geomanager/modeladmin/index.html
 geomanager/templates/geomanager/modeladmin/index_without_custom_create.html
+geomanager/templates/geomanager/modeladmin/raster_style_legend_preview.html
 geomanager/templates/geomanager/raster_file/raster_file_edit_form.html
 geomanager/templates/geomanager/raster_file/raster_file_layer_preview.html
 geomanager/templates/geomanager/raster_file/raster_file_upload.html
 geomanager/templates/geomanager/raster_tile/raster_tile_layer_preview.html
 geomanager/templates/geomanager/shared/breadcrumbs.html
 geomanager/templates/geomanager/vector_file/vector_file_edit_form.html
 geomanager/templates/geomanager/vector_file/vector_file_layer_preview.html
```

### Comparing `geomanager-0.4.6/geomanager.egg-info/requires.txt` & `geomanager-0.4.7/geomanager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geomanager-0.4.6/setup.cfg` & `geomanager-0.4.7/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = geomanager
-version = 0.4.6
+version = 0.4.7
 description = Wagtail based Geospatial Data Manager
 long_description = file:README.md
 long_description_content_type = text/markdown
-url = https://github.com/wmo-raf/geomanager
+url = https://github.com/erick-otenyo/geomanager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Intended Audience :: Developers
```

