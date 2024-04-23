# Comparing `tmp/openepd-3.1.1.tar.gz` & `tmp/openepd-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.1.1.tar", max compression
+gzip compressed data, was "openepd-3.1.2.tar", max compression
```

## Comparing `openepd-3.1.1.tar` & `openepd-3.1.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    11357 2024-04-22 15:11:03.128442 openepd-3.1.1/LICENSE
--rw-r--r--   0        0        0     6786 2024-04-22 15:11:03.128442 openepd-3.1.1/README.md
--rw-r--r--   0        0        0     3132 2024-04-22 15:11:03.132442 openepd-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-04-22 15:11:03.132442 openepd-3.1.1/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     5176 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     2271 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/aluminium.py
--rw-r--r--   0        0        0     3549 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0    15961 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1934 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/accessories.py
--rw-r--r--   0        0        0     3161 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/aggregates.py
--rw-r--r--   0        0        0     2440 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/aluminium.py
--rw-r--r--   0        0        0     3837 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/asphalt.py
--rw-r--r--   0        0        0     1034 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/bulk_materials.py
--rw-r--r--   0        0        0     1058 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
--rw-r--r--   0        0        0     6939 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/cladding.py
--rw-r--r--   0        0        0     2324 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/cmu.py
--rw-r--r--   0        0        0     1117 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/common.py
--rw-r--r--   0        0        0     6617 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/concrete.py
--rw-r--r--   0        0        0     2422 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/conveying_equipment.py
--rw-r--r--   0        0        0    10457 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/electrical.py
--rw-r--r--   0        0        0     2117 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
--rw-r--r--   0        0        0     1029 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/electricity.py
--rw-r--r--   0        0        0    57079 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/enums.py
--rw-r--r--   0        0        0    22337 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/finishes.py
--rw-r--r--   0        0        0     2801 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/fire_and_smoke_protection.py
--rw-r--r--   0        0        0     3076 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/furnishings.py
--rw-r--r--   0        0        0     1023 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/grouting.py
--rw-r--r--   0        0        0     4599 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/manufacturing_inputs.py
--rw-r--r--   0        0        0     3177 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/masonry.py
--rw-r--r--   0        0        0     1225 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/material_handling.py
--rw-r--r--   0        0        0    11561 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/mechanical.py
--rw-r--r--   0        0        0     1900 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/mechanical_insulation.py
--rw-r--r--   0        0        0     8644 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/network_infrastructure.py
--rw-r--r--   0        0        0    17100 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/openings.py
--rw-r--r--   0        0        0     1057 2024-04-22 15:11:03.136442 openepd-3.1.1/src/openepd/model/specs/generated/other_electrical_equipment.py
--rw-r--r--   0        0        0     3453 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/other_materials.py
--rw-r--r--   0        0        0     5439 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/plumbing.py
--rw-r--r--   0        0        0     2690 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/precast_concrete.py
--rw-r--r--   0        0        0     3516 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/sheathing.py
--rw-r--r--   0        0        0     8102 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/steel.py
--rw-r--r--   0        0        0     7963 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/thermal_moisture_protection.py
--rw-r--r--   0        0        0     2768 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/utility_piping.py
--rw-r--r--   0        0        0     6199 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/wood.py
--rw-r--r--   0        0        0     1880 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/generated/wood_joists.py
--rw-r--r--   0        0        0    13664 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/glass.py
--rw-r--r--   0        0        0     6367 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/steel.py
--rw-r--r--   0        0        0     5144 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/specs/wood.py
--rw-r--r--   0        0        0     1535 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     5287 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2024-04-22 15:11:03.140442 openepd-3.1.1/src/openepd/py.typed
--rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 openepd-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 17:16:43.101493 openepd-3.1.2/LICENSE
+-rw-r--r--   0        0        0     6786 2024-04-23 17:16:43.101493 openepd-3.1.2/README.md
+-rw-r--r--   0        0        0     3147 2024-04-23 17:16:43.105493 openepd-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-04-23 17:16:43.105493 openepd-3.1.2/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     2271 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/aluminium.py
+-rw-r--r--   0        0        0     3549 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0    15961 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1934 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2440 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3837 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1034 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1058 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6939 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2324 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     8324 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     2422 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0    10457 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2117 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1029 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    58482 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    22337 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     2801 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     3076 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1023 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     4599 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3177 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1225 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0    11561 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1900 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     8644 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    19729 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1057 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3453 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     5439 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     2690 2024-04-23 17:16:43.109493 openepd-3.1.2/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3516 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0    10255 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     7963 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2768 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6199 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     1880 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0    13664 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/glass.py
+-rw-r--r--   0        0        0     6367 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/steel.py
+-rw-r--r--   0        0        0     5144 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/specs/wood.py
+-rw-r--r--   0        0        0     1535 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     5287 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:16:43.113493 openepd-3.1.2/src/openepd/py.typed
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.1.2/PKG-INFO
```

### Comparing `openepd-3.1.1/LICENSE` & `openepd-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/README.md` & `openepd-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/pyproject.toml` & `openepd-3.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.1.1"
+version = "3.1.2"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -20,29 +20,30 @@
 exclude = ["**/test_*.py", "**/tests/**"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = ">=1.10,<3.0"
 email-validator = ">=1.3.1"
 requests = { version = ">=2.0", optional = true }
+idna = ">=3.7"
 
 # Optional dependencies
 # lxml = { version = "~=4.9.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
 pytest = "~=7.2"
 pytest-subtests = "~=0.4"
 pytest-cov = "~=4.0"
 teamcity-messages = ">=1.31"
 wheel = "~=0.40.0"
 
 # Dev tools
-black = "~=22.3"
+black = "~=24.3"
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
 flake8-import-graph = "~=0.1.3"
 flake8-docstrings = "~=1.7.0"
 isort = "~=5.11"
 mypy = ">=1.0.1"
 pre-commit = "~=2.19"
```

### Comparing `openepd-3.1.1/src/openepd/__init__.py` & `openepd-3.1.2/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/__version__.py` & `openepd-3.1.2/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.1.1"
+VERSION = "3.1.2"
```

### Comparing `openepd-3.1.1/src/openepd/api/__init__.py` & `openepd-3.1.2/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/base_sync_client.py` & `openepd-3.1.2/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/category/__init__.py` & `openepd-3.1.2/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/category/dto.py` & `openepd-3.1.2/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/category/sync_api.py` & `openepd-3.1.2/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/common.py` & `openepd-3.1.2/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/__init__.py` & `openepd-3.1.2/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/base.py` & `openepd-3.1.2/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/common.py` & `openepd-3.1.2/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/meta.py` & `openepd-3.1.2/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/mf.py` & `openepd-3.1.2/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/dto/params.py` & `openepd-3.1.2/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/epd/__init__.py` & `openepd-3.1.2/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/epd/dto.py` & `openepd-3.1.2/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/epd/sync_api.py` & `openepd-3.1.2/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/errors.py` & `openepd-3.1.2/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/pcr/__init__.py` & `openepd-3.1.2/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/pcr/dto.py` & `openepd-3.1.2/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/pcr/sync_api.py` & `openepd-3.1.2/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/sync_client.py` & `openepd-3.1.2/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/api/test/__init__.py` & `openepd-3.1.2/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/bundle/__init__.py` & `openepd-3.1.2/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/bundle/base.py` & `openepd-3.1.2/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/bundle/model.py` & `openepd-3.1.2/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/bundle/reader.py` & `openepd-3.1.2/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/bundle/writer.py` & `openepd-3.1.2/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/compat/__init__.py` & `openepd-3.1.2/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/compat/pydantic.py` & `openepd-3.1.2/src/openepd/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/__init__.py` & `openepd-3.1.2/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/base.py` & `openepd-3.1.2/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/category.py` & `openepd-3.1.2/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/common.py` & `openepd-3.1.2/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/epd.py` & `openepd-3.1.2/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/factory.py` & `openepd-3.1.2/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/lcia.py` & `openepd-3.1.2/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/org.py` & `openepd-3.1.2/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/pcr.py` & `openepd-3.1.2/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/README.md` & `openepd-3.1.2/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/__init__.py` & `openepd-3.1.2/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/aluminium.py` & `openepd-3.1.2/src/openepd/model/specs/aluminium.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/asphalt.py` & `openepd-3.1.2/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/base.py` & `openepd-3.1.2/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/concrete.py` & `openepd-3.1.2/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/accessories.py` & `openepd-3.1.2/src/openepd/model/specs/generated/accessories.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/aggregates.py` & `openepd-3.1.2/src/openepd/model/specs/generated/aggregates.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/aluminium.py` & `openepd-3.1.2/src/openepd/model/specs/generated/aluminium.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/asphalt.py` & `openepd-3.1.2/src/openepd/model/specs/generated/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/bulk_materials.py` & `openepd-3.1.2/src/openepd/model/specs/generated/bulk_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/cast_decks_and_underlayment.py` & `openepd-3.1.2/src/openepd/model/specs/generated/cast_decks_and_underlayment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/cladding.py` & `openepd-3.1.2/src/openepd/model/specs/generated/cladding.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/cmu.py` & `openepd-3.1.2/src/openepd/model/specs/generated/cmu.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/common.py` & `openepd-3.1.2/src/openepd/model/specs/generated/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/concrete.py` & `openepd-3.1.2/src/openepd/model/specs/generated/wood.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,139 +13,155 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Literal
-
 from openepd.compat.pydantic import pyd
+from openepd.model.org import OrgRef
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.specs.concrete import Cementitious, ConcreteTypicalApplication
-from openepd.model.specs.generated.enums import AciExposureClass, CsaExposureClass, EnExposureClass
-from openepd.model.validation.numbers import RatioFloat
-from openepd.model.validation.quantity import (
-    LengthInchStr,
-    LengthMmStr,
-    MassKgStr,
-    PressureMPaStr,
-    validate_unit_factory,
+from openepd.model.specs.generated.common import HasForestPracticesCertifiers
+from openepd.model.specs.generated.enums import (
+    AllFabrication,
+    AllTimberSpecies,
+    CompositeLumberFabrication,
+    EngineeredTimberSpecies,
+    MassTimberFabrication,
+    SawnTimberSpecies,
+    SheathingPanelsFabrication,
 )
+from openepd.model.validation.numbers import RatioFloat
+from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
 
 
-class CementGroutV1(BaseOpenEpdHierarchicalSpec):
-    """Cement grout performance specification."""
+class WoodDeckingV1(BaseOpenEpdHierarchicalSpec):
+    """Wood used for decking."""
 
     _EXT_VERSION = "1.0"
 
 
-class ConcretePavingV1(BaseOpenEpdHierarchicalSpec):
-    """Concrete paving performance specification."""
+class WoodFramingV1(BaseOpenEpdHierarchicalSpec):
+    """Lumber for framing, typically softwood."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-    flexion_strength: PressureMPaStr | None = pyd.Field(
-        default=None, description="Paving flexion strength", example="30 MPa"
-    )
 
-    _concrete_flexion_strength_is_quantity_validator = pyd.validator("flexion_strength", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
+class PrefabricatedWoodInsulatedPanelsV1(BaseOpenEpdHierarchicalSpec):
+    """Prefabricated wood insulated panels performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+
+class PrefabricatedWoodTrussV1(BaseOpenEpdHierarchicalSpec):
+    """Prefabricated wood truss performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+
+class CompositeLumberV1(BaseOpenEpdHierarchicalSpec):
+    """Composite lumber performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+    fabrication: CompositeLumberFabrication | None = pyd.Field(default=None, description="", example="LVL")
+    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+
+
+class DimensionLumberV1(BaseOpenEpdHierarchicalSpec):
+    """Dimension lumber performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+    # Nested specs:
+    timber_species: SawnTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+    WoodDecking: WoodDeckingV1 | None = None
+    WoodFraming: WoodFramingV1 | None = None
 
 
-class FlowableFillV1(BaseOpenEpdHierarchicalSpec):
-    """Flowable fill performance specification."""
+class HeavyTimberV1(BaseOpenEpdHierarchicalSpec):
+    """Large format natural timber."""
 
     _EXT_VERSION = "1.0"
 
 
-class OilPatchV1(BaseOpenEpdHierarchicalSpec):
-    """Oil patch performance specification."""
+class MassTimberV1(BaseOpenEpdHierarchicalSpec):
+    """Manufactured structural wood elements, such a CLT and LVL."""
 
     _EXT_VERSION = "1.0"
 
+    fabrication: MassTimberFabrication | None = pyd.Field(default=None, description="", example="CLT")
+    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+
 
-class ReadyMixV1(BaseOpenEpdHierarchicalSpec):
-    """Concretes that are mixed just before use, and then poured on-site into forms."""
+class NonStructuralWoodV1(BaseOpenEpdHierarchicalSpec):
+    """Wood products that are not meant for structural use."""
 
     _EXT_VERSION = "1.0"
 
 
-class ShotcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Shotcrete performance specification."""
+class PrefabricatedWoodV1(BaseOpenEpdHierarchicalSpec):
+    """Prefabricated wood performance specification."""
 
     _EXT_VERSION = "1.0"
 
+    # Nested specs:
+    PrefabricatedWoodInsulatedPanels: PrefabricatedWoodInsulatedPanelsV1 | None = None
+    PrefabricatedWoodTruss: PrefabricatedWoodTrussV1 | None = None
+
 
-class ConcreteV1(BaseOpenEpdHierarchicalSpec):
-    """Concrete performance specification."""
+class SheathingPanelsV1(BaseOpenEpdHierarchicalSpec):
+    """Structural Wood Panels."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    lightweight: bool | None = pyd.Field(default=None, description="Lightweight", example=True)
+    fabrication: SheathingPanelsFabrication | None = pyd.Field(default=None, description="", example="Plywood")
+    wood_board_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
+    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
 
-    strength_28d: PressureMPaStr | None = pyd.Field(
-        default=None, description="Concrete strength after 28 days", example="1 MPa"
-    )
-    strength_other: PressureMPaStr | None = pyd.Field(
-        default=None,
-        description="A strength spec which is to be reached later other 28 days (e.g. 42d)",
-        example="30 MPa",
-    )
-    strength_other_d: Literal[3, 7, 14, 42, 56, 72, 96, 120] | None = pyd.Field(
-        default=None, description="Test Day for the Late Strength", example=42
+    _wood_board_thickness_is_quantity_validator = pyd.validator("wood_board_thickness", allow_reuse=True)(
+        validate_unit_factory("m")
     )
 
-    slump: LengthInchStr | None = pyd.Field(default=None, description="", example="2 in")
-    min_slump: LengthInchStr | None = pyd.Field(default=None, description="Minimum test slump", example="2 in")
-    max_slump: LengthInchStr | None = pyd.Field(default=None, description="", example="2 in")
-
-    min_pipeline_size: LengthMmStr | None = pyd.Field(default=None, description="", example="200 mm")
-    w_c_ratio: RatioFloat | None = pyd.Field(
-        default=None, description="Ratio of water to cement", example=0.5, ge=0, le=1
-    )
-    air_entrain: bool | None = pyd.Field(default=None, description="Air Entrainment", example=True)
-    co2_entrain: bool | None = pyd.Field(default=None, description="CO2 Curing", example=True)
-    self_consolidating: bool | None = pyd.Field(default=None, description="Self Compacting", example=True)
-    white_cement: bool | None = pyd.Field(default=None, description="White Cement", example=True)
-    plc: bool | None = pyd.Field(default=None, description="Portland Limestone Cement", example=True)
-    finishable: bool | None = pyd.Field(default=None, description="Finishable", example=True)
-    fiber_reinforced: bool | None = pyd.Field(default=None, description="fiber_reinforced", example=True)
-
-    cementitious: Cementitious | None = pyd.Field(default=None, description="")
-
-    aggregate_size_max: LengthMmStr | None = pyd.Field(default=None, description="", example="0.0254 m")
-    cement_content: MassKgStr | None = pyd.Field(default=None, description="", example="1 kg")
-    aci_exposure_classes: list[AciExposureClass] | None = pyd.Field(default=None, description="", example=["aci.F0"])
-    csa_exposure_classes: list[CsaExposureClass] | None = pyd.Field(default=None, description="", example=["csa.C-2"])
-    en_exposure_classes: list[EnExposureClass] | None = pyd.Field(default=None, description="", example=["en206.X0"])
-    typical_application: ConcreteTypicalApplication | None = pyd.Field(default=None, description="Typical Application")
 
-    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator("strength_28d", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _concrete_compressive_strength_other_is_quantity_validator = pyd.validator("strength_other", allow_reuse=True)(
-        validate_unit_factory("MPa")
+class UnfinishedWoodV1(BaseOpenEpdHierarchicalSpec):
+    """Unfinished or 'green' timber."""
+
+    _EXT_VERSION = "1.0"
+
+
+class WoodV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
+    """Wood performance specification."""
+
+    _EXT_VERSION = "1.0"
+
+    # Own fields:
+    timber_species: AllTimberSpecies | None = pyd.Field(
+        default=None, description="Timber species", example="Alaska Cedar"
     )
-    _concrete_slump_is_quantity_validator = pyd.validator("slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_min_slump_is_quantity_validator = pyd.validator("min_slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_max_slump_is_quantity_validator = pyd.validator("max_slump", allow_reuse=True)(validate_unit_factory("m"))
-    _concrete_min_pipeline_size_is_quantity_validator = pyd.validator("min_pipeline_size", allow_reuse=True)(
-        validate_unit_factory("m")
+    fabrication: AllFabrication | None = pyd.Field(default=None, description="Timber fabrication", example="LVL")
+    forest_practices_certifiers: list[OrgRef] | None = pyd.Field(
+        default=None, description="List of organizations that certify forest practices."
     )
-    _concrete_aggregate_size_max_is_quantity_validator = pyd.validator("aggregate_size_max", allow_reuse=True)(
-        validate_unit_factory("m")
+    weather_exposed: bool | None = pyd.Field(default=None, description="Weather exposed", example=True)
+    fire_retardant: bool | None = pyd.Field(default=None, description="Fire retardant", example=True)
+    decay_resistant: bool | None = pyd.Field(default=None, description="Decay resistant", example=True)
+    fsc_certified: RatioFloat | None = pyd.Field(
+        default=None, description="Forest Stewardship Council certified proportion", example=0.3, ge=0, le=1
     )
-    _concrete_cement_content_is_quantity_validator = pyd.validator("cement_content", allow_reuse=True)(
-        validate_unit_factory("kg")
+    fsc_certified_z: float | None = pyd.Field(default=None, description="", example=0.7)
+
+    recycled_content: RatioFloat | None = pyd.Field(
+        default=None, description="Recycled content", example=0.3, ge=0, le=1
     )
+    recycled_content_z: float | None = pyd.Field(default=None, description="", example=0.7)
 
     # Nested specs:
-    CementGrout: CementGroutV1 | None = None
-    ConcretePaving: ConcretePavingV1 | None = None
-    FlowableFill: FlowableFillV1 | None = None
-    OilPatch: OilPatchV1 | None = None
-    ReadyMix: ReadyMixV1 | None = None
-    Shotcrete: ShotcreteV1 | None = None
+    CompositeLumber: CompositeLumberV1 | None = None
+    DimensionLumber: DimensionLumberV1 | None = None
+    HeavyTimber: HeavyTimberV1 | None = None
+    MassTimber: MassTimberV1 | None = None
+    NonStructuralWood: NonStructuralWoodV1 | None = None
+    PrefabricatedWood: PrefabricatedWoodV1 | None = None
+    SheathingPanels: SheathingPanelsV1 | None = None
+    UnfinishedWood: UnfinishedWoodV1 | None = None
```

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/conveying_equipment.py` & `openepd-3.1.2/src/openepd/model/specs/generated/conveying_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/electrical.py` & `openepd-3.1.2/src/openepd/model/specs/generated/electrical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py` & `openepd-3.1.2/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/electricity.py` & `openepd-3.1.2/src/openepd/model/specs/generated/electricity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/enums.py` & `openepd-3.1.2/src/openepd/model/specs/generated/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,22 +368,22 @@
     CLOSED_CELL = "Closed-Cell"
 
 
 class FrameMaterial(StrEnum):
     """
     Frame material.
 
-     - Vinyl: Vinyl
-     - Aluminium: Aluminium
-     - Steel: Steel
-     - Wood: Wood
-     - Fiberglass: Fiberglass
-     - Composite: Composite
-     - None: None
-     - Other: Other
+     - Vinyl: PVC and similar polymer frames
+     - Aluminium: Aluminium, with optional thermal improvement. Does not include aluminium clad.
+     - Steel: Steel, with optional thermal improvement
+     - Wood: Wood with optional cladding
+     - Fiberglass: Fiber reinforced plastic
+     - Composite: Plastic and Wood Fiber composite.
+     - None: This EPD does not cover the frame.
+     - Other: Other framing material not listed
 
     """
 
     VINYL = "Vinyl"
     ALUMINIUM = "Aluminium"
     STEEL = "Steel"
     WOOD = "Wood"
@@ -1789,20 +1789,20 @@
     YELLOW_POPLAR = "Yellow Poplar"
 
 
 class HardwareFunction(StrEnum):
     """
     Hardware function.
 
-     - Lock: Lock
-     - Hinge: Hinge
-     - Handle: Handle
-     - Operator: Operator
-     - Balance: Balance
-     - Other: Other
+     - Lock: Locks, Keepers, and similar items that resist opening.
+     - Hinge: Hinges, Pivots, and similar items that secure glazing to the frame while it moves.
+     - Handle: Handles, knobs, and similar items for directly manipulating a window.
+     - Operator: Arms, Cranks, and other hardware that moves a window.
+     - Balance: Springs, Sash Balances, and other items that counter the weight of an operable sash.
+     - Other: Other hardware not described above.
 
     """
 
     LOCK = "Lock"
     HINGE = "Hinge"
     HANDLE = "Handle"
     OPERATOR = "Operator"
@@ -1971,19 +1971,25 @@
     OTHER = "Other"
 
 
 class ThermalSeparation(StrEnum):
     """
     Thermal separation.
 
-     - Aluminium: Aluminium
-     - Steel: Steel
-     - Thermally Improved Metal: Thermally Improved Metal
-     - Thermally Broken Metal: Thermally Broken Metal
-     - Nonmetal: Nonmetal
+     - Aluminium: Aluminium System members with less than 1.6 mm (0.062 in) or no separation between metal or system
+       members to provide a resistance heat transfer path from exterior to interior.
+     - Steel: Steel System members with less than 1.6 mm (0.062 in) or no separation between metal or system members to
+       provide a resistance heat transfer path from exterior to interior.
+     - Thermally Improved Metal: Metal System members with a separation ≥ 1.60 mm (0.062 in) provided by either a
+       thermal break or open air space that may be interrupted by short thermal bridges between the interior and
+       exterior surfaces.
+     - Thermally Broken Metal: Aluminium System members with a minimum of 5.30 mm (0.210 in) separation provided by
+       a thermal break.
+     - Nonmetal: Nonmetal material where the path from inside to outside inherently has low thermal conductivity,
+       such as wood, vinyl, and fiberglass. Aluminium-clad or split windows fall in this category.
 
     """
 
     ALUMINIUM = "Aluminium"
     STEEL = "Steel"
     THERMALLY_IMPROVED_METAL = "Thermally Improved Metal"
     THERMALLY_BROKEN_METAL = "Thermally Broken Metal"
@@ -2372,15 +2378,15 @@
     MM_10 = "10 mm"
     MM_12 = "12 mm"
     MM_16 = "16 mm"
     MM_19 = "19 mm"
 
 
 class NAFSPerformanceGrade(StrEnum):
-    """NAFS Performance Grade enum."""
+    """NAFS Performance Grade."""
 
     GRADE_15_PSF = "15 psf"
     GRADE_20_PSF = "20 psf"
     GRADE_25_PSF = "25 psf"
     GRADE_30_PSF = "30 psf"
     GRADE_35_PSF = "35 psf"
     GRADE_40_PSF = "40 psf"
```

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/finishes.py` & `openepd-3.1.2/src/openepd/model/specs/generated/finishes.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/fire_and_smoke_protection.py` & `openepd-3.1.2/src/openepd/model/specs/generated/fire_and_smoke_protection.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/furnishings.py` & `openepd-3.1.2/src/openepd/model/specs/generated/furnishings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/grouting.py` & `openepd-3.1.2/src/openepd/model/specs/generated/grouting.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/manufacturing_inputs.py` & `openepd-3.1.2/src/openepd/model/specs/generated/manufacturing_inputs.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/masonry.py` & `openepd-3.1.2/src/openepd/model/specs/generated/masonry.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/material_handling.py` & `openepd-3.1.2/src/openepd/model/specs/generated/material_handling.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/mechanical.py` & `openepd-3.1.2/src/openepd/model/specs/generated/mechanical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/mechanical_insulation.py` & `openepd-3.1.2/src/openepd/model/specs/generated/mechanical_insulation.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/network_infrastructure.py` & `openepd-3.1.2/src/openepd/model/specs/generated/network_infrastructure.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/other_electrical_equipment.py` & `openepd-3.1.2/src/openepd/model/specs/generated/other_electrical_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/other_materials.py` & `openepd-3.1.2/src/openepd/model/specs/generated/other_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/plumbing.py` & `openepd-3.1.2/src/openepd/model/specs/generated/plumbing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/precast_concrete.py` & `openepd-3.1.2/src/openepd/model/specs/generated/precast_concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/sheathing.py` & `openepd-3.1.2/src/openepd/model/specs/generated/sheathing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/steel.py` & `openepd-3.1.2/src/openepd/model/specs/generated/thermal_moisture_protection.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,211 +14,220 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.compat.pydantic import pyd
-from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec, BaseOpenEpdSpec
-from openepd.model.specs.generated.enums import SteelComposition, SteelRebarGrade
-from openepd.model.specs.steel import SteelMakingRoute
-from openepd.model.standard import Standard
+from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from openepd.model.specs.generated.enums import (
+    FoamType,
+    InsulatingMaterial,
+    InsulationIntendedApplication,
+    MembraneRoofingReinforcement,
+    RoofCoverBoardsFacing,
+    RoofCoverBoardsMaterial,
+)
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, PressureMPaStr, validate_unit_factory
 
 
-class SteelFabricatedMixin(BaseOpenEpdSpec):
-    """Class with fabricated property used in different parts of steel hierarchy."""
+class BituminousRoofingV1(BaseOpenEpdHierarchicalSpec):
+    """Bituminous roofing performance specification."""
 
-    fabricated: bool | None = pyd.Field(default=None, description="", example=True)
+    _EXT_VERSION = "1.0"
 
 
-class ColdFormedFramingV1(BaseOpenEpdHierarchicalSpec):
-    """Cold formed framing performance specification."""
+class SinglePlyEPDMV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply e p d m performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class DeckingSteelV1(BaseOpenEpdHierarchicalSpec):
-    """Cold Formed Steel Decking."""
+class SinglePlyKEEV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply k e e performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class SteelSuspensionAssemblyV1(BaseOpenEpdHierarchicalSpec):
-    """Steel suspension assembly performance specification."""
+class SinglePlyOtherV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply other performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class HollowSectionsV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
-    """Hollow sections performance specification."""
+class SinglePlyPolyurethaneV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply polyurethane performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-
 
-class HotRolledSectionsV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
-    """Hot rolled sections performance specification."""
+class SinglePlyPVCV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply p v c performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-
 
-class PlateSteelV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
-    """Plate Steels."""
+class SinglePlyTPOV1(BaseOpenEpdHierarchicalSpec):
+    """Single ply t p o performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-
 
-class MetalRailingsV1(BaseOpenEpdHierarchicalSpec):
-    """Metal railings performance specification."""
+class BlanketInsulationV1(BaseOpenEpdHierarchicalSpec):
+    """Blanket insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class MetalStairsV1(BaseOpenEpdHierarchicalSpec):
-    """Metal stairs performance specification."""
+class BlownInsulationV1(BaseOpenEpdHierarchicalSpec):
+    """Blown insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class MiscMetalFabricationV1(BaseOpenEpdHierarchicalSpec):
-    """Misc metal fabrication performance specification."""
+class BoardInsulationV1(BaseOpenEpdHierarchicalSpec):
+    """Board insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
+    # Own fields:
+    compressive_strength: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
+
+    _compressive_strength_is_quantity_validator = pyd.validator("compressive_strength", allow_reuse=True)(
+        validate_unit_factory("MPa")
+    )
 
-class OpenWebMembranesV1(BaseOpenEpdHierarchicalSpec):
-    """Open web membranes performance specification."""
+
+class FoamedInPlaceV1(BaseOpenEpdHierarchicalSpec):
+    """Foamed in place performance specification."""
 
     _EXT_VERSION = "1.0"
 
+    # Own fields:
+    foam_type: FoamType | None = pyd.Field(default=None, description="", example="Open-Cell")
+
 
-class MBQSteelV1(BaseOpenEpdHierarchicalSpec):
-    """M b q steel performance specification."""
+class SprayedInsulationV1(BaseOpenEpdHierarchicalSpec):
+    """Sprayed insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class CoilSteelV1(BaseOpenEpdHierarchicalSpec):
-    """Coil steel performance specification."""
+class AirBarriersV1(BaseOpenEpdHierarchicalSpec):
+    """Air barriers performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class ColdFormedSteelV1(BaseOpenEpdHierarchicalSpec):
-    """Cold Formed Structural Steel."""
+class MembraneRoofingV1(BaseOpenEpdHierarchicalSpec):
+    """Membrane roofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
+    # Own fields:
+    thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
+    sri: float | None = pyd.Field(default=None, description="", example=2.3)
+    total_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
+    post_consumer_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
+    reinforcement: MembraneRoofingReinforcement | None = pyd.Field(default=None, description="", example="Polyester")
+    felt_backing: bool | None = pyd.Field(default=None, description="", example=True)
+    nsf347: bool | None = pyd.Field(default=None, description="", example=True)
+    vantage_vinyl: bool | None = pyd.Field(default=None, description="", example=True)
+
+    _thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(validate_unit_factory("m"))
+
     # Nested specs:
-    ColdFormedFraming: ColdFormedFramingV1 | None = None
-    DeckingSteel: DeckingSteelV1 | None = None
-    SteelSuspensionAssembly: SteelSuspensionAssemblyV1 | None = None
+    BituminousRoofing: BituminousRoofingV1 | None = None
+    SinglePlyEPDM: SinglePlyEPDMV1 | None = None
+    SinglePlyKEE: SinglePlyKEEV1 | None = None
+    SinglePlyOther: SinglePlyOtherV1 | None = None
+    SinglePlyPolyurethane: SinglePlyPolyurethaneV1 | None = None
+    SinglePlyPVC: SinglePlyPVCV1 | None = None
+    SinglePlyTPO: SinglePlyTPOV1 | None = None
 
 
-class StructuralSteelV1(BaseOpenEpdHierarchicalSpec):
-    """Structural Steel."""
+class InsulationV1(BaseOpenEpdHierarchicalSpec):
+    """Insulation performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    modulus_of_elasticity: PressureMPaStr | None = pyd.Field(default=None, description="", example="1.0 MPa")
-    thermal_expansion: str | None = pyd.Field(default=None, description="", example="1 / K")
-    thermal_conductivity: str | None = pyd.Field(default=None, description="", example="1 W / (m * K)")
-
-    _steel_modulus_of_elasticity_is_quantity_validator = pyd.validator("modulus_of_elasticity", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
-    _steel_thermal_expansion_is_quantity_validator = pyd.validator("thermal_expansion", allow_reuse=True)(
-        validate_unit_factory("1 / K")
+    r_value: float | None = pyd.Field(default=None, description="", example=2.3)
+    material: InsulatingMaterial | None = pyd.Field(default=None, description="", example="Mineral Wool")
+    intended_application: list[InsulationIntendedApplication] | None = pyd.Field(
+        default=None, description="", example=["Wall & General"]
     )
-    _steel_thermal_conductivity_is_quantity_validator = pyd.validator("thermal_conductivity", allow_reuse=True)(
-        validate_unit_factory("W / (m * K)")
+    thickness_per_declared_unit: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
+
+    _thickness_per_declared_unit_is_quantity_validator = pyd.validator("thickness_per_declared_unit", allow_reuse=True)(
+        validate_unit_factory("m")
     )
 
     # Nested specs:
-    HollowSections: HollowSectionsV1 | None = None
-    HotRolledSections: HotRolledSectionsV1 | None = None
-    PlateSteel: PlateSteelV1 | None = None
+    BlanketInsulation: BlanketInsulationV1 | None = None
+    BlownInsulation: BlownInsulationV1 | None = None
+    BoardInsulation: BoardInsulationV1 | None = None
+    FoamedInPlace: FoamedInPlaceV1 | None = None
+    SprayedInsulation: SprayedInsulationV1 | None = None
 
 
-class PrefabricatedSteelAssembliesV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated steel assemblies performance specification."""
+class DampproofingAndWaterproofingV1(BaseOpenEpdHierarchicalSpec):
+    """Dampproofing and waterproofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    # Nested specs:
-    MetalRailings: MetalRailingsV1 | None = None
-    MetalStairs: MetalStairsV1 | None = None
-    MiscMetalFabrication: MiscMetalFabricationV1 | None = None
-    OpenWebMembranes: OpenWebMembranesV1 | None = None
+
+class FlashingAndSheetMetalV1(BaseOpenEpdHierarchicalSpec):
+    """Flashing and sheet metal performance specification."""
+
+    _EXT_VERSION = "1.0"
 
 
-class PostTensioningSteelV1(BaseOpenEpdHierarchicalSpec):
-    """Post-Tensioning Steels, per https://www.concretenetwork.com/post-tension/industry.html."""
+class JointProtectionV1(BaseOpenEpdHierarchicalSpec):
+    """Joint protection performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class RebarSteelV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
-    """Bar steels, such as rebar for concrete reinforcement."""
+class RoofCoverBoardsV1(BaseOpenEpdHierarchicalSpec):
+    """Roof cover boards performance specification."""
 
     _EXT_VERSION = "1.0"
 
     # Own fields:
-    grade: SteelRebarGrade | None = pyd.Field(default=None, description="", example="60 ksi")
-    diameter_min: LengthMmStr | None = pyd.Field(default=None, description="", example="8 mm")
-    bending_pin_max: float | None = pyd.Field(default=None, description="", example=2.3)
-    ts_ys_ratio_max: float | None = pyd.Field(default=None, description="", example=2.3)
-    epoxy_coated: bool | None = pyd.Field(default=None, description="", example=True)
+    material: RoofCoverBoardsMaterial | None = pyd.Field(default=None, description="", example="Gypsum Fiber")
+    facing: list[RoofCoverBoardsFacing] | None = pyd.Field(default=None, description="", example=["Paper"])
+    thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="1 m")
 
-    _steel_rebar_diameter_min_is_quantity_validator = pyd.validator("diameter_min", allow_reuse=True)(
+    _roof_cover_boards_thickness_is_quantity_validator = pyd.validator("thickness", allow_reuse=True)(
         validate_unit_factory("m")
     )
 
 
-class WireMeshSteelV1(BaseOpenEpdHierarchicalSpec, SteelFabricatedMixin):
-    """Mild steel wire for reinforcement, connections, and meshes."""
+class SteepSlopeRoofingV1(BaseOpenEpdHierarchicalSpec):
+    """Steep slope roofing performance specification."""
 
     _EXT_VERSION = "1.0"
 
 
-class SteelV1(BaseOpenEpdHierarchicalSpec):
-    """Steel performance specification."""
+class WeatherBarriersV1(BaseOpenEpdHierarchicalSpec):
+    """Weather barriers performance specification."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-    yield_tensile_str: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
-    bar_elongation: float | None = pyd.Field(default=None, description="", example=2.3)
-    recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
-    post_consumer_recycled_content: RatioFloat | None = pyd.Field(default=None, description="", example=0.5, ge=0, le=1)
-    astm_marking: str | None = pyd.Field(default=None, description="")
-    euro_marking: str | None = pyd.Field(default=None, description="")
-    composition: SteelComposition | None = pyd.Field(default=None, description="", example="Carbon")
-    cold_finished: bool | None = pyd.Field(default=None, description="", example=True)
-    galvanized: bool | None = pyd.Field(default=None, description="", example=True)
-    stainless: bool | None = pyd.Field(default=None, description="", example=True)
-    making_route: SteelMakingRoute | None = pyd.Field(default=None)
-    astm_standards: list[Standard] | None = pyd.Field(default=None, description="")
-    sae_standards: list[Standard] | None = pyd.Field(default=None, description="")
-    en_standards: list[Standard] | None = pyd.Field(default=None, description="")
 
-    _steel_yield_tensile_str_is_quantity_validator = pyd.validator("yield_tensile_str", allow_reuse=True)(
-        validate_unit_factory("MPa")
-    )
+class ThermalMoistureProtectionV1(BaseOpenEpdHierarchicalSpec):
+    """Thermal moisture protection performance specification."""
+
+    _EXT_VERSION = "1.0"
 
     # Nested specs:
-    MBQSteel: MBQSteelV1 | None = None
-    CoilSteel: CoilSteelV1 | None = None
-    ColdFormedSteel: ColdFormedSteelV1 | None = None
-    StructuralSteel: StructuralSteelV1 | None = None
-    PrefabricatedSteelAssemblies: PrefabricatedSteelAssembliesV1 | None = None
-    PostTensioningSteel: PostTensioningSteelV1 | None = None
-    RebarSteel: RebarSteelV1 | None = None
-    WireMeshSteel: WireMeshSteelV1 | None = None
+    AirBarriers: AirBarriersV1 | None = None
+    MembraneRoofing: MembraneRoofingV1 | None = None
+    Insulation: InsulationV1 | None = None
+    DampproofingAndWaterproofing: DampproofingAndWaterproofingV1 | None = None
+    FlashingAndSheetMetal: FlashingAndSheetMetalV1 | None = None
+    JointProtection: JointProtectionV1 | None = None
+    RoofCoverBoards: RoofCoverBoardsV1 | None = None
+    SteepSlopeRoofing: SteepSlopeRoofingV1 | None = None
+    WeatherBarriers: WeatherBarriersV1 | None = None
```

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/utility_piping.py` & `openepd-3.1.2/src/openepd/model/specs/generated/utility_piping.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/wood.py` & `openepd-3.1.2/src/openepd/model/specs/steel.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,155 +13,172 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
+from enum import StrEnum
+
 from openepd.compat.pydantic import pyd
-from openepd.model.org import OrgRef
+from openepd.model.base import BaseOpenEpdSchema
+from openepd.model.common import OpenEPDUnit
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
-from openepd.model.specs.generated.common import HasForestPracticesCertifiers
-from openepd.model.specs.generated.enums import (
-    AllFabrication,
-    AllTimberSpecies,
-    CompositeLumberFabrication,
-    EngineeredTimberSpecies,
-    MassTimberFabrication,
-    SawnTimberSpecies,
-    SheathingPanelsFabrication,
-)
+from openepd.model.specs.generated.enums import SteelComposition
+from openepd.model.standard import Standard
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
 
 
-class WoodDeckingV1(BaseOpenEpdHierarchicalSpec):
-    """Wood used for decking."""
+class SteelMakingRoute(BaseOpenEpdSchema):
+    """Steel making route."""
 
-    _EXT_VERSION = "1.0"
+    bof: bool | None = pyd.Field(default=None, description="Basic oxygen furnace")
+    eaf: bool | None = pyd.Field(default=None, description="Electric arc furnace")
+    ohf: bool | None = pyd.Field(default=None, description="Open hearth furnace")
 
 
-class WoodFramingV1(BaseOpenEpdHierarchicalSpec):
-    """Lumber for framing, typically softwood."""
+class FabricatedOptionsMixin(pyd.BaseModel):
+    """Fabricated options mixin."""
 
     _EXT_VERSION = "1.0"
 
+    fabricated: bool | None = pyd.Field(default=None, description="Fabricated")
+
 
-class PrefabricatedWoodInsulatedPanelsV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood insulated panels performance specification."""
+class WireMeshSteelV1(BaseOpenEpdHierarchicalSpec):
+    """Spec for wire mesh steel."""
 
     _EXT_VERSION = "1.0"
 
+    class Options(BaseOpenEpdSchema, FabricatedOptionsMixin):
+        """Wire Mesh Options."""
 
-class PrefabricatedWoodTrussV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood truss performance specification."""
+        pass
 
-    _EXT_VERSION = "1.0"
+    options: Options = pyd.Field(description="Rebar Steel options", default_factory=Options)
 
 
-class CompositeLumberV1(BaseOpenEpdHierarchicalSpec):
-    """Composite lumber performance specification."""
+class RebarGrade(StrEnum):
+    """Rebar grade enum."""
 
-    _EXT_VERSION = "1.0"
+    USA_60_KSI = "60 ksi"
+    USA_75_KIS = "75 ksi"
+    USA_80_KSI = "80 ksi"
+    USA_90_KSI = "90 ksi"
+    USA_100_KSI = "100 ksi"
+    USA_120_KSI = "120 ksi"
+    USA_40_KSI = "40 ksi"
+    USA_50_KSI = "50 ksi"
 
-    fabrication: CompositeLumberFabrication | None = pyd.Field(default=None, description="", example="LVL")
-    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+    METRIC_420_MPA = "420 Mpa"
+    METRIC_520_MPA = "520 Mpa"
+    METRIC_550_MPA = "550 Mpa"
+    METRIC_620_MPA = "620 Mpa"
+    METRIC_690_MPA = "690 MPa"
+    METRIC_830_MPA = "830 Mpa"
+    METRIC_280_MPA = "280 MPa"
+    METRIC_350_MPA = "350 Mpa"
 
 
-class DimensionLumberV1(BaseOpenEpdHierarchicalSpec):
-    """Dimension lumber performance specification."""
+class RebarSteelV1(BaseOpenEpdHierarchicalSpec):
+    """Rebar steel spec."""
 
     _EXT_VERSION = "1.0"
 
-    # Nested specs:
-    timber_species: SawnTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
-    WoodDecking: WoodDeckingV1 | None = None
-    WoodFraming: WoodFramingV1 | None = None
+    class Options(BaseOpenEpdSchema, FabricatedOptionsMixin):
+        """Rebar Steel Options."""
 
+        epoxy: bool | None = pyd.Field(default=None, description="Epoxy Coated")
 
-class HeavyTimberV1(BaseOpenEpdHierarchicalSpec):
-    """Large format natural timber."""
+    options: Options = pyd.Field(description="Rebar Steel options", default_factory=Options)
 
-    _EXT_VERSION = "1.0"
+    steel_rebar_grade: RebarGrade | None = pyd.Field(default=None, description="Rebar steel grade")
+    steel_rebar_diameter_min: LengthMmStr | None = pyd.Field(default=None, description="Minimum rebar diameter")
+    _steel_rebar_diameter_min = pyd.validator("steel_rebar_diameter_min", allow_reuse=True)(
+        validate_unit_factory(OpenEPDUnit.m)
+    )
+
+    steel_rebar_bending_pin_max: float | None = pyd.Field(
+        default=None, description="Maximum rebar bending pin in diameters of this rebar", example=6.2
+    )
+    steel_rebar_ts_ys_ratio_max: float | None = pyd.Field(
+        default=None, description="Max ratio of ultimate tensile to yield tensile strength"
+    )
 
 
-class MassTimberV1(BaseOpenEpdHierarchicalSpec):
-    """Manufactured structural wood elements, such a CLT and LVL."""
+class PlateSteelV1(BaseOpenEpdHierarchicalSpec):
+    """Plate Steel Spec."""
 
     _EXT_VERSION = "1.0"
 
-    fabrication: MassTimberFabrication | None = pyd.Field(default=None, description="", example="CLT")
-    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
-
+    class Options(BaseOpenEpdSchema, FabricatedOptionsMixin):
+        """Plate Steel Options."""
 
-class NonStructuralWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Wood products that are not meant for structural use."""
+        pass
 
-    _EXT_VERSION = "1.0"
+    options: Options = pyd.Field(description="Plate Steel options", default_factory=Options)
 
 
-class PrefabricatedWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Prefabricated wood performance specification."""
+class HollowV1(BaseOpenEpdHierarchicalSpec):
+    """Hollow Sections Spec."""
 
     _EXT_VERSION = "1.0"
 
-    # Nested specs:
-    PrefabricatedWoodInsulatedPanels: PrefabricatedWoodInsulatedPanelsV1 | None = None
-    PrefabricatedWoodTruss: PrefabricatedWoodTrussV1 | None = None
+    class Options(FabricatedOptionsMixin, BaseOpenEpdSchema):
+        """Hollow Sections Options."""
 
+        pass
 
-class SheathingPanelsV1(BaseOpenEpdHierarchicalSpec):
-    """Structural Wood Panels."""
+    options: Options = pyd.Field(description="Hollow Steel options", default_factory=Options)
 
-    _EXT_VERSION = "1.0"
 
-    # Own fields:
-    fabrication: SheathingPanelsFabrication | None = pyd.Field(default=None, description="", example="Plywood")
-    wood_board_thickness: LengthMmStr | None = pyd.Field(default=None, description="", example="10 mm")
-    timber_species: EngineeredTimberSpecies | None = pyd.Field(default=None, description="", example="Alaska Cedar")
+class HotRolledV1(BaseOpenEpdHierarchicalSpec):
+    """Hot Rolled spec."""
 
-    _wood_board_thickness_is_quantity_validator = pyd.validator("wood_board_thickness", allow_reuse=True)(
-        validate_unit_factory("m")
-    )
+    _EXT_VERSION = "1.0"
 
+    class Options(FabricatedOptionsMixin, BaseOpenEpdSchema):
+        """Hot Rolled options."""
 
-class UnfinishedWoodV1(BaseOpenEpdHierarchicalSpec):
-    """Unfinished or 'green' timber."""
+        pass
 
-    _EXT_VERSION = "1.0"
+    options: Options = pyd.Field(description="Hollow Steel options", default_factory=Options)
 
 
-class WoodV1(BaseOpenEpdHierarchicalSpec, HasForestPracticesCertifiers):
-    """Wood performance specification."""
+class SteelV1(BaseOpenEpdHierarchicalSpec):
+    """Steel spec."""
 
     _EXT_VERSION = "1.0"
 
-    # Own fields:
-    timber_species: AllTimberSpecies | None = pyd.Field(
-        default=None, description="Timber species", example="Alaska Cedar"
-    )
-    fabrication: AllFabrication | None = pyd.Field(default=None, description="Timber fabrication", example="LVL")
-    forest_practices_certifiers: list[OrgRef] | None = pyd.Field(
-        default=None, description="List of organizations that certify forest practices."
-    )
-    weather_exposed: bool | None = pyd.Field(default=None, description="Weather exposed", example=True)
-    fire_retardant: bool | None = pyd.Field(default=None, description="Fire retardant", example=True)
-    decay_resistant: bool | None = pyd.Field(default=None, description="Decay resistant", example=True)
-    fsc_certified: RatioFloat | None = pyd.Field(
-        default=None, description="Forest Stewardship Council certified proportion", example=0.3, ge=0, le=1
-    )
-    fsc_certified_z: float | None = pyd.Field(default=None, description="", example=0.7)
+    class Options(BaseOpenEpdSchema):
+        """Steel spec options."""
+
+        galvanized: bool | None = pyd.Field(default=None, description="Galvanized")
+        cold_finished: bool | None = pyd.Field(default=None, description="Cold Finished")
 
+    form_factor: str | None = pyd.Field(description="Product's form factor", example="Steel >> RebarSteel")
+    steel_composition: SteelComposition | None = pyd.Field(default=None, description="Basic chemical composition")
     recycled_content: RatioFloat | None = pyd.Field(
-        default=None, description="Recycled content", example=0.3, ge=0, le=1
+        default=None,
+        example=0.3,
+        description="Scrap steel inputs from other processes.  Includes "
+        "Post-Consumer content, if any.  This percentage may be "
+        "used to evaluate the EPD w.r.t. targets or limits that are"
+        " different for primary and recycled content.",
+    )
+    ASTM: list[Standard] = pyd.Field(description="ASTM standard to which this product complies", default_factory=list)
+    SAE: list[Standard] = pyd.Field(
+        description="AISA/SAE standard to which this product complies", default_factory=list
     )
-    recycled_content_z: float | None = pyd.Field(default=None, description="", example=0.7)
+    EN: list[Standard] = pyd.Field(description="EN 10027 number(s)", default_factory=list)
+
+    options: Options | None = pyd.Field(description="Steel options", default_factory=Options)
+    making_route: SteelMakingRoute | None = pyd.Field(default=None, description="Steel making route")
+
+    # Nested specs
 
-    # Nested specs:
-    CompositeLumber: CompositeLumberV1 | None = None
-    DimensionLumber: DimensionLumberV1 | None = None
-    HeavyTimber: HeavyTimberV1 | None = None
-    MassTimber: MassTimberV1 | None = None
-    NonStructuralWood: NonStructuralWoodV1 | None = None
-    PrefabricatedWood: PrefabricatedWoodV1 | None = None
-    SheathingPanels: SheathingPanelsV1 | None = None
-    UnfinishedWood: UnfinishedWoodV1 | None = None
+    WireMeshSteel: WireMeshSteelV1 | None = None
+    RebarSteel: RebarSteelV1 | None = None
+    PlateSteel: PlateSteelV1 | None = None
+    Hollow: HollowV1 | None = None
+    HotRolled: HotRolledV1 | None = None
```

### Comparing `openepd-3.1.1/src/openepd/model/specs/generated/wood_joists.py` & `openepd-3.1.2/src/openepd/model/specs/generated/wood_joists.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/glass.py` & `openepd-3.1.2/src/openepd/model/specs/glass.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/specs/wood.py` & `openepd-3.1.2/src/openepd/model/specs/wood.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/standard.py` & `openepd-3.1.2/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/validation/__init__.py` & `openepd-3.1.2/src/openepd/model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/validation/common.py` & `openepd-3.1.2/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/validation/numbers.py` & `openepd-3.1.2/src/openepd/model/validation/numbers.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/validation/quantity.py` & `openepd-3.1.2/src/openepd/model/validation/quantity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/src/openepd/model/versioning.py` & `openepd-3.1.2/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.1.1/PKG-INFO` & `openepd-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: api-client
 Requires-Dist: email-validator (>=1.3.1)
+Requires-Dist: idna (>=3.7)
 Requires-Dist: pydantic (>=1.10,<3.0)
 Requires-Dist: requests (>=2.0) ; extra == "api-client"
 Project-URL: Repository, https://github.com/cchangelabs/openepd
 Description-Content-Type: text/markdown
 
 # Python Library to work with OpenEPD format
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.1.1 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.1.2 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Provides-Extra: api-client Requires-
-Dist: email-validator (>=1.3.1) Requires-Dist: pydantic (>=1.10,<3.0) Requires-
-Dist: requests (>=2.0) ; extra == "api-client" Project-URL: Repository, https:/
-/github.com/cchangelabs/openepd Description-Content-Type: text/markdown #
-Python Library to work with OpenEPD format
+Dist: email-validator (>=1.3.1) Requires-Dist: idna (>=3.7) Requires-Dist:
+pydantic (>=1.10,<3.0) Requires-Dist: requests (>=2.0) ; extra == "api-client"
+Project-URL: Repository, https://github.com/cchangelabs/openepd Description-
+Content-Type: text/markdown # Python Library to work with OpenEPD format
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
      _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_S_t_y_l_e_-_b_l_a_c_k_-_b_l_a_c_k_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
                         _d_m_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_c_c_h_a_n_g_e_l_a_b_s_/_o_p_e_n_e_p_d_/
    _s_a_n_i_t_y_-_c_h_e_c_k_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-
```

