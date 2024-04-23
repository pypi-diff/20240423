# Comparing `tmp/gemd-2.1.1.tar.gz` & `tmp/gemd-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemd-2.1.1.tar", last modified: Wed Apr 17 18:09:26 2024, max compression
+gzip compressed data, was "gemd-2.1.3.tar", last modified: Tue Apr 23 17:32:41 2024, max compression
```

## Comparing `gemd-2.1.1.tar` & `gemd-2.1.3.tar`

### file list

```diff
@@ -1,130 +1,135 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.441172 gemd-2.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-04-17 18:08:09.000000 gemd-2.1.1/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)     1007 2024-04-17 18:09:26.437172 gemd-2.1.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2024-04-17 18:08:09.000000 gemd-2.1.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.333165 gemd-2.1.1/gemd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.341165 gemd-2.1.1/gemd/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14906 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/builders/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.357166 gemd-2.1.1/gemd/demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38891 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/cake.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4689 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/material_run_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/measurement_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  1541363 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)    19946 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   235566 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook_small.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/table_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/toothpick.jpg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.365167 gemd-2.1.1/gemd/entity/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.369167 gemd-2.1.1/gemd/entity/attribute/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/base_attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/condition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2577 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/property_and_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8895 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/base_entity.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.377168 gemd-2.1.1/gemd/entity/bounds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2650 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/base_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5128 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/categorical_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5247 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/composition_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5768 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/integer_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3872 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/molecular_structure_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7709 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/real_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds_validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6326 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/case_insensitive_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7173 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/dict_serializable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/file_link.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/has_dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2598 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/link_by_uid.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.393169 gemd-2.1.1/gemd/entity/object/
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2589 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/base_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1536 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_quantities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      802 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1805 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1582 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4290 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_template_check_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/ingredient_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5967 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/ingredient_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4596 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/material_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5540 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/material_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/measurement_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/measurement_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4614 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/process_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4730 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/process_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/setters.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.393169 gemd-2.1.1/gemd/entity/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/source/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/source/performed_source.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.401170 gemd-2.1.1/gemd/entity/template/
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/attribute_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3322 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/base_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/condition_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_condition_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_parameter_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4127 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_property_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1932 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/material_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/measurement_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/parameter_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3887 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/process_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1000 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/property_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4037 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5686 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/valid_list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.417171 gemd-2.1.1/gemd/entity/value/
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/base_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      736 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/categorical_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/composition_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/continuous_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2263 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/discrete_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/empirical_formula.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/inchi_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      642 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/integer_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/molecular_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1282 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_composition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/normal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/smiles_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2907 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/uniform_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1712 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/uniform_real.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.421171 gemd-2.1.1/gemd/enumeration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5108 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/base_enumeration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      390 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/origin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/sample_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.425171 gemd-2.1.1/gemd/json/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/gemd_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7922 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/gemd_json.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.425171 gemd-2.1.1/gemd/units/
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35636 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/citrine_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6701 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/constants_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    15746 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/gemd/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17810 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/util/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/gemd.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     1007 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      207 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-17 18:09:26.441172 gemd-2.1.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1990 2024-04-17 18:08:09.000000 gemd-2.1.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6320 2024-04-17 18:08:09.000000 gemd-2.1.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.159029 gemd-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 17:32:38.000000 gemd-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 17:32:41.159029 gemd-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-23 17:32:38.000000 gemd-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.143029 gemd-2.1.3/gemd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.143029 gemd-2.1.3/gemd/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/builders/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.147029 gemd-2.1.3/gemd/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38891 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/cake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/material_run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/measurement_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1541363 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/strehlow_and_cook.pif
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/strehlow_and_cook.py
+-rw-r--r--   0 runner    (1001) docker     (127)   235566 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/strehlow_and_cook_small.pif
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/table_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/demo/toothpick.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.147029 gemd-2.1.3/gemd/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.147029 gemd-2.1.3/gemd/entity/attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/base_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/attribute/property_and_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/base_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.151029 gemd-2.1.3/gemd/entity/bounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/base_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/categorical_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/composition_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/integer_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/molecular_structure_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds/real_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/bounds_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/dict_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/file_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/has_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/link_by_uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.151029 gemd-2.1.3/gemd/entity/object/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/has_template_check_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/ingredient_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/ingredient_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/material_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/material_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/measurement_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/measurement_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/process_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/object/process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/setters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.151029 gemd-2.1.3/gemd/entity/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/source/performed_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.155029 gemd-2.1.3/gemd/entity/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/attribute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/condition_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/has_condition_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/has_parameter_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/has_property_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/material_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/measurement_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/parameter_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/process_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/template/property_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/valid_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.155029 gemd-2.1.3/gemd/entity/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/base_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/categorical_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/composition_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/continuous_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/discrete_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/empirical_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/inchi_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/integer_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/molecular_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/nominal_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/nominal_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/nominal_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/nominal_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/normal_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/smiles_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/uniform_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/entity/value/uniform_real.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.155029 gemd-2.1.3/gemd/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/enumeration/base_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/enumeration/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/enumeration/sample_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.155029 gemd-2.1.3/gemd/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/json/gemd_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/json/gemd_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.155029 gemd-2.1.3/gemd/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35636 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/units/citrine_en.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/units/constants_en.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/units/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.159029 gemd-2.1.3/gemd/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17810 2024-04-23 17:32:38.000000 gemd-2.1.3/gemd/util/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.143029 gemd-2.1.3/gemd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 17:32:41.000000 gemd-2.1.3/gemd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-23 17:32:41.000000 gemd-2.1.3/gemd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:32:41.000000 gemd-2.1.3/gemd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 17:32:41.000000 gemd-2.1.3/gemd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:32:41.000000 gemd-2.1.3/gemd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:32:41.159029 gemd-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-23 17:32:38.000000 gemd-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.159029 gemd-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:38.000000 gemd-2.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-23 17:32:38.000000 gemd-2.1.3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:41.159029 gemd-2.1.3/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:32:38.000000 gemd-2.1.3/tests/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-23 17:32:38.000000 gemd-2.1.3/tests/units/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 17:32:38.000000 gemd-2.1.3/tests/units/test_units.txt
```

### Comparing `gemd-2.1.1/LICENSE` & `gemd-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/README.md` & `gemd-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GEMD-python 
-Python binding for Citrine's nextgen data model, GEMD. 
+Python binding for Citrine's data model, GEMD. 
 
 This package provides a framework for storing information about the processes that create materials, the materials themselves, and measurements performed on those materials. 
 
 ## Usage
 
 To install `gemd`, you can simply:
 ```bash
```

### Comparing `gemd-2.1.1/gemd/__init__.py` & `gemd-2.1.3/gemd/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/builders/impl.py` & `gemd-2.1.3/gemd/builders/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/cake.py` & `gemd-2.1.3/gemd/demo/cake.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/material_run_example.py` & `gemd-2.1.3/gemd/demo/material_run_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/measurement_example.py` & `gemd-2.1.3/gemd/demo/measurement_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/strehlow_and_cook.pif` & `gemd-2.1.3/gemd/demo/strehlow_and_cook.pif`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/strehlow_and_cook.py` & `gemd-2.1.3/gemd/demo/strehlow_and_cook.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/strehlow_and_cook_small.pif` & `gemd-2.1.3/gemd/demo/strehlow_and_cook_small.pif`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/table_example.py` & `gemd-2.1.3/gemd/demo/table_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/demo/toothpick.jpg` & `gemd-2.1.3/gemd/demo/toothpick.jpg`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/__init__.py` & `gemd-2.1.3/gemd/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/attribute/base_attribute.py` & `gemd-2.1.3/gemd/entity/attribute/base_attribute.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/attribute/condition.py` & `gemd-2.1.3/gemd/entity/attribute/condition.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/attribute/parameter.py` & `gemd-2.1.3/gemd/entity/attribute/parameter.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/attribute/property.py` & `gemd-2.1.3/gemd/entity/attribute/property.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/attribute/property_and_conditions.py` & `gemd-2.1.3/gemd/entity/attribute/property_and_conditions.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/base_entity.py` & `gemd-2.1.3/gemd/entity/base_entity.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/base_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/base_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/categorical_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/categorical_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/composition_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/composition_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/integer_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/integer_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/molecular_structure_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/molecular_structure_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds/real_bounds.py` & `gemd-2.1.3/gemd/entity/bounds/real_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/bounds_validation.py` & `gemd-2.1.3/gemd/entity/bounds_validation.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/case_insensitive_dict.py` & `gemd-2.1.3/gemd/entity/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/dict_serializable.py` & `gemd-2.1.3/gemd/entity/dict_serializable.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/file_link.py` & `gemd-2.1.3/gemd/entity/file_link.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/has_dependencies.py` & `gemd-2.1.3/gemd/entity/has_dependencies.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/link_by_uid.py` & `gemd-2.1.3/gemd/entity/link_by_uid.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/__init__.py` & `gemd-2.1.3/gemd/entity/object/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/base_object.py` & `gemd-2.1.3/gemd/entity/object/base_object.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_conditions.py` & `gemd-2.1.3/gemd/entity/object/has_conditions.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_material.py` & `gemd-2.1.3/gemd/entity/object/has_material.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_parameters.py` & `gemd-2.1.3/gemd/entity/object/has_parameters.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_process.py` & `gemd-2.1.3/gemd/entity/object/has_process.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_properties.py` & `gemd-2.1.3/gemd/entity/object/has_properties.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_quantities.py` & `gemd-2.1.3/gemd/entity/object/has_quantities.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_source.py` & `gemd-2.1.3/gemd/entity/object/has_source.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_spec.py` & `gemd-2.1.3/gemd/entity/object/has_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_template.py` & `gemd-2.1.3/gemd/entity/object/has_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/has_template_check_generator.py` & `gemd-2.1.3/gemd/entity/object/has_template_check_generator.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/ingredient_run.py` & `gemd-2.1.3/gemd/entity/object/ingredient_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/ingredient_spec.py` & `gemd-2.1.3/gemd/entity/object/ingredient_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/material_run.py` & `gemd-2.1.3/gemd/entity/object/material_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/material_spec.py` & `gemd-2.1.3/gemd/entity/object/material_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/measurement_run.py` & `gemd-2.1.3/gemd/entity/object/measurement_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/measurement_spec.py` & `gemd-2.1.3/gemd/entity/object/measurement_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/process_run.py` & `gemd-2.1.3/gemd/entity/object/process_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/object/process_spec.py` & `gemd-2.1.3/gemd/entity/object/process_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/setters.py` & `gemd-2.1.3/gemd/entity/setters.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/source/performed_source.py` & `gemd-2.1.3/gemd/entity/source/performed_source.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/attribute_template.py` & `gemd-2.1.3/gemd/entity/template/attribute_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/base_template.py` & `gemd-2.1.3/gemd/entity/template/base_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/condition_template.py` & `gemd-2.1.3/gemd/entity/template/condition_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/has_condition_templates.py` & `gemd-2.1.3/gemd/entity/template/has_condition_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/has_parameter_templates.py` & `gemd-2.1.3/gemd/entity/template/has_parameter_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/has_property_templates.py` & `gemd-2.1.3/gemd/entity/template/has_property_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/material_template.py` & `gemd-2.1.3/gemd/entity/template/material_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/measurement_template.py` & `gemd-2.1.3/gemd/entity/template/measurement_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/parameter_template.py` & `gemd-2.1.3/gemd/entity/template/parameter_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/process_template.py` & `gemd-2.1.3/gemd/entity/template/process_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/template/property_template.py` & `gemd-2.1.3/gemd/entity/template/property_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/util.py` & `gemd-2.1.3/gemd/entity/util.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/valid_list.py` & `gemd-2.1.3/gemd/entity/valid_list.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/__init__.py` & `gemd-2.1.3/gemd/entity/value/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/base_value.py` & `gemd-2.1.3/gemd/entity/value/base_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/categorical_value.py` & `gemd-2.1.3/gemd/entity/value/categorical_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/composition_value.py` & `gemd-2.1.3/gemd/entity/value/composition_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/continuous_value.py` & `gemd-2.1.3/gemd/entity/value/continuous_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/discrete_categorical.py` & `gemd-2.1.3/gemd/entity/value/discrete_categorical.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/empirical_formula.py` & `gemd-2.1.3/gemd/entity/value/empirical_formula.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/inchi_value.py` & `gemd-2.1.3/gemd/entity/value/inchi_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/integer_value.py` & `gemd-2.1.3/gemd/entity/value/integer_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/molecular_value.py` & `gemd-2.1.3/gemd/entity/value/molecular_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/nominal_categorical.py` & `gemd-2.1.3/gemd/entity/value/nominal_categorical.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/nominal_composition.py` & `gemd-2.1.3/gemd/entity/value/nominal_composition.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/nominal_integer.py` & `gemd-2.1.3/gemd/entity/value/nominal_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/nominal_real.py` & `gemd-2.1.3/gemd/entity/value/nominal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/normal_real.py` & `gemd-2.1.3/gemd/entity/value/normal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/smiles_value.py` & `gemd-2.1.3/gemd/entity/value/smiles_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/uniform_integer.py` & `gemd-2.1.3/gemd/entity/value/uniform_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/entity/value/uniform_real.py` & `gemd-2.1.3/gemd/entity/value/uniform_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/enumeration/base_enumeration.py` & `gemd-2.1.3/gemd/enumeration/base_enumeration.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/json/__init__.py` & `gemd-2.1.3/gemd/json/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/json/gemd_json.py` & `gemd-2.1.3/gemd/json/gemd_json.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/units/citrine_en.txt` & `gemd-2.1.3/gemd/units/citrine_en.txt`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/units/constants_en.txt` & `gemd-2.1.3/gemd/units/constants_en.txt`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/units/impl.py` & `gemd-2.1.3/gemd/units/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd/util/impl.py` & `gemd-2.1.3/gemd/util/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-2.1.1/gemd.egg-info/SOURCES.txt` & `gemd-2.1.3/gemd.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -104,8 +104,12 @@
 gemd/json/gemd_json.py
 gemd/units/__init__.py
 gemd/units/citrine_en.txt
 gemd/units/constants_en.txt
 gemd/units/impl.py
 gemd/util/__init__.py
 gemd/util/impl.py
-tests/test_examples.py
+tests/__init__.py
+tests/test_examples.py
+tests/units/__init__.py
+tests/units/test_parser.py
+tests/units/test_units.txt
```

### Comparing `gemd-2.1.1/setup.py` & `gemd-2.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
-from os import path
-from packaging.version import Version
+from pathlib import Path
 import re
 
 packages = find_packages()
 
-this_directory = path.abspath(path.dirname(__file__))
-version_file = path.join(this_directory, 'gemd', '__version__.py')
-version_re = r'''^__version__\s*=\s*(['"])([\w\.]+)\1$'''
-with open(version_file, 'r') as f:
-    mo = re.search(version_re, f.read(), re.M)
-    if mo:
-        version = Version(mo.group(2))
-    else:
-        raise RuntimeError(f"Unable to find version string in {version_file}")
+this_directory = Path(__file__).parent.absolute()
+version_file = this_directory / 'gemd' / '__version__.py'
+version_re = r'''^\s*__version__\s*=\s*(['"])([\w\.]+)\1$'''
+if mo := re.search(version_re, version_file.read_text(), re.M):
+    version = mo.group(2)
+else:
+    raise RuntimeError(f"Unable to find version string in {version_file}")
 
 setup(name='gemd',
       # Update this in gemd/__version__.py
-      version=str(version),
+      version=version,
       python_requires='>=3.8',
       url='http://github.com/CitrineInformatics/gemd-python',
       description="Python binding for Citrine's GEMD data model",
       author='Citrine Informatics',
       packages=packages,
       package_data={
           'gemd.demo': [
@@ -38,14 +35,20 @@
       install_requires=[
           "pint>=0.20,<0.24",
           "deprecation>=2.1.0,<3",
           "typing_extensions>=4.8,<5",
           "importlib-resources>=5.3,<7"
       ],
       extras_require={
+          "scripts": [
+              "packaging"
+              "sphinx==5.0.0",
+              "sphinx-rtd-theme==1.0.0",
+              "sphinxcontrib-apidoc==0.3.0",
+          ],
           "tests": [
               "pytest>=8.0.0,<9"
           ],
           "tests.demo": [
               "pandas>=2.0.3,<3"
           ],
           "tests.entity.bounds": [
```

### Comparing `gemd-2.1.1/tests/test_examples.py` & `gemd-2.1.3/tests/test_examples.py`

 * *Files identical despite different names*

