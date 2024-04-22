# Comparing `tmp/arctrl-2.0.0a2.tar.gz` & `tmp/arctrl-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctrl-2.0.0a2.tar", max compression
+gzip compressed data, was "arctrl-2.0.0a3.tar", max compression
```

## Comparing `arctrl-2.0.0a2.tar` & `arctrl-2.0.0a3.tar`

### file list

```diff
@@ -1,382 +1,382 @@
--rw-r--r--   0        0        0        0 2024-04-05 14:00:30.507778 arctrl-2.0.0a2/arctrl/__init__.py
--rw-r--r--   0        0        0    28760 2024-04-05 14:00:30.683466 arctrl-2.0.0a2/arctrl/arc.py
--rw-r--r--   0        0        0      665 2024-04-05 14:00:32.526473 arctrl-2.0.0a2/arctrl/arctrl.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:30.411319 arctrl-2.0.0a2/arctrl/Contract/__init__.py
--rw-r--r--   0        0        0     1300 2024-04-05 14:00:30.475574 arctrl-2.0.0a2/arctrl/Contract/arc.py
--rw-r--r--   0        0        0     4937 2024-04-05 14:00:30.427391 arctrl-2.0.0a2/arctrl/Contract/arc_assay.py
--rw-r--r--   0        0        0     4463 2024-04-05 14:00:30.460030 arctrl-2.0.0a2/arctrl/Contract/arc_investigation.py
--rw-r--r--   0        0        0     5278 2024-04-05 14:00:30.443431 arctrl-2.0.0a2/arctrl/Contract/arc_study.py
--rw-r--r--   0        0        0     4312 2024-04-05 14:00:30.411319 arctrl-2.0.0a2/arctrl/Contract/contract.py
--rw-r--r--   0        0        0     4624 2024-04-05 14:00:30.475574 arctrl-2.0.0a2/arctrl/Contract/git.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:27.031210 arctrl-2.0.0a2/arctrl/Core/__init__.py
--rw-r--r--   0        0        0   125590 2024-04-05 14:00:28.991014 arctrl-2.0.0a2/arctrl/Core/arc_types.py
--rw-r--r--   0        0        0     4349 2024-04-05 14:00:27.063360 arctrl-2.0.0a2/arctrl/Core/comment.py
--rw-r--r--   0        0        0     3731 2024-04-05 14:00:27.063360 arctrl-2.0.0a2/arctrl/Core/comment_list.py
--rw-r--r--   0        0        0    59641 2024-04-05 14:00:29.048187 arctrl-2.0.0a2/arctrl/Core/conversion.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.857690 arctrl-2.0.0a2/arctrl/Core/Helper/__init__.py
--rw-r--r--   0        0        0    10402 2024-04-05 14:00:27.024692 arctrl-2.0.0a2/arctrl/Core/Helper/collections_.py
--rw-r--r--   0        0        0     1959 2024-04-05 14:00:26.991061 arctrl-2.0.0a2/arctrl/Core/Helper/hash_codes.py
--rw-r--r--   0        0        0     4311 2024-04-05 14:00:26.957940 arctrl-2.0.0a2/arctrl/Core/Helper/identifier.py
--rw-r--r--   0        0        0      234 2024-04-05 14:00:26.974500 arctrl-2.0.0a2/arctrl/Core/Helper/printer.py
--rw-r--r--   0        0        0    18730 2024-04-05 14:00:26.991061 arctrl-2.0.0a2/arctrl/Core/Helper/regex.py
--rw-r--r--   0        0        0     3316 2024-04-05 14:00:27.041231 arctrl-2.0.0a2/arctrl/Core/Helper/sem_ver.py
--rw-r--r--   0        0        0        2 2024-04-05 14:00:26.855656 arctrl-2.0.0a2/arctrl/Core/Helper/url.py
--rw-r--r--   0        0        0     1061 2024-04-05 14:00:28.557971 arctrl-2.0.0a2/arctrl/Core/identifier_setters.py
--rw-r--r--   0        0        0    10790 2024-04-05 14:00:27.141078 arctrl-2.0.0a2/arctrl/Core/ontology_annotation.py
--rw-r--r--   0        0        0     4731 2024-04-05 14:00:27.191198 arctrl-2.0.0a2/arctrl/Core/ontology_source_reference.py
--rw-r--r--   0        0        0    11558 2024-04-05 14:00:27.175685 arctrl-2.0.0a2/arctrl/Core/person.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:27.191198 arctrl-2.0.0a2/arctrl/Core/Process/__init__.py
--rw-r--r--   0        0        0    14288 2024-04-05 14:00:27.624258 arctrl-2.0.0a2/arctrl/Core/Process/column_index.py
--rw-r--r--   0        0        0     8025 2024-04-05 14:00:27.407767 arctrl-2.0.0a2/arctrl/Core/Process/component.py
--rw-r--r--   0        0        0     2393 2024-04-05 14:00:27.340973 arctrl-2.0.0a2/arctrl/Core/Process/data.py
--rw-r--r--   0        0        0     1843 2024-04-05 14:00:27.319378 arctrl-2.0.0a2/arctrl/Core/Process/data_file.py
--rw-r--r--   0        0        0     5936 2024-04-05 14:00:27.224496 arctrl-2.0.0a2/arctrl/Core/Process/factor.py
--rw-r--r--   0        0        0     6548 2024-04-05 14:00:27.257602 arctrl-2.0.0a2/arctrl/Core/Process/factor_value.py
--rw-r--r--   0        0        0      643 2024-04-05 14:00:27.191198 arctrl-2.0.0a2/arctrl/Core/Process/iproperty_value.py
--rw-r--r--   0        0        0     3703 2024-04-05 14:00:27.303279 arctrl-2.0.0a2/arctrl/Core/Process/material.py
--rw-r--r--   0        0        0     4320 2024-04-05 14:00:27.257602 arctrl-2.0.0a2/arctrl/Core/Process/material_attribute.py
--rw-r--r--   0        0        0     8009 2024-04-05 14:00:27.291227 arctrl-2.0.0a2/arctrl/Core/Process/material_attribute_value.py
--rw-r--r--   0        0        0     1270 2024-04-05 14:00:27.274658 arctrl-2.0.0a2/arctrl/Core/Process/material_type.py
--rw-r--r--   0        0        0    21546 2024-04-05 14:00:27.608091 arctrl-2.0.0a2/arctrl/Core/Process/process.py
--rw-r--r--   0        0        0     9394 2024-04-05 14:00:27.463978 arctrl-2.0.0a2/arctrl/Core/Process/process_input.py
--rw-r--r--   0        0        0     8212 2024-04-05 14:00:27.480048 arctrl-2.0.0a2/arctrl/Core/Process/process_output.py
--rw-r--r--   0        0        0     7173 2024-04-05 14:00:27.507595 arctrl-2.0.0a2/arctrl/Core/Process/process_parameter_value.py
--rw-r--r--   0        0        0    19068 2024-04-05 14:00:27.624258 arctrl-2.0.0a2/arctrl/Core/Process/process_sequence.py
--rw-r--r--   0        0        0    10509 2024-04-05 14:00:27.447867 arctrl-2.0.0a2/arctrl/Core/Process/protocol.py
--rw-r--r--   0        0        0     3889 2024-04-05 14:00:27.399740 arctrl-2.0.0a2/arctrl/Core/Process/protocol_parameter.py
--rw-r--r--   0        0        0     4117 2024-04-05 14:00:27.324395 arctrl-2.0.0a2/arctrl/Core/Process/sample.py
--rw-r--r--   0        0        0     2686 2024-04-05 14:00:27.307824 arctrl-2.0.0a2/arctrl/Core/Process/source.py
--rw-r--r--   0        0        0     6388 2024-04-05 14:00:27.207929 arctrl-2.0.0a2/arctrl/Core/Process/value.py
--rw-r--r--   0        0        0     6958 2024-04-05 14:00:27.191198 arctrl-2.0.0a2/arctrl/Core/publication.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:27.687844 arctrl-2.0.0a2/arctrl/Core/Table/__init__.py
--rw-r--r--   0        0        0    48412 2024-04-05 14:00:28.124304 arctrl-2.0.0a2/arctrl/Core/Table/arc_table.py
--rw-r--r--   0        0        0    24986 2024-04-05 14:00:27.831605 arctrl-2.0.0a2/arctrl/Core/Table/arc_table_aux.py
--rw-r--r--   0        0        0    25506 2024-04-05 14:00:28.103064 arctrl-2.0.0a2/arctrl/Core/Table/arc_tables.py
--rw-r--r--   0        0        0     6677 2024-04-05 14:00:27.687844 arctrl-2.0.0a2/arctrl/Core/Table/composite_cell.py
--rw-r--r--   0        0        0     3471 2024-04-05 14:00:27.687844 arctrl-2.0.0a2/arctrl/Core/Table/composite_column.py
--rw-r--r--   0        0        0    30828 2024-04-05 14:00:27.719664 arctrl-2.0.0a2/arctrl/Core/Table/composite_header.py
--rw-r--r--   0        0        0     8330 2024-04-05 14:00:28.424528 arctrl-2.0.0a2/arctrl/Core/template.py
--rw-r--r--   0        0        0     6294 2024-04-05 14:00:28.441069 arctrl-2.0.0a2/arctrl/Core/templates.py
--rw-r--r--   0        0        0      180 2024-04-05 14:00:27.024692 arctrl-2.0.0a2/arctrl/Core/uri.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.855656 arctrl-2.0.0a2/arctrl/CWL/__init__.py
--rw-r--r--   0        0        0        2 2024-04-05 14:00:26.855656 arctrl-2.0.0a2/arctrl/CWL/library.py
--rw-r--r--   0        0        0        4 2024-04-05 14:00:21.783636 arctrl-2.0.0a2/arctrl/fable_modules/.gitignore
--rw-r--r--   0        0        0        0 2024-03-20 08:48:34.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/__init__.py
--rw-r--r--   0        0        0    45250 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/array_.py
--rw-r--r--   0        0        0    10175 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/async_.py
--rw-r--r--   0        0        0    10722 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/async_builder.py
--rw-r--r--   0        0        0     4999 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/big_int.py
--rw-r--r--   0        0        0     3491 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/bit_converter.py
--rw-r--r--   0        0        0      607 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/boolean.py
--rw-r--r--   0        0        0     6477 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/char.py
--rw-r--r--   0        0        0     5685 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/choice.py
--rw-r--r--   0        0        0    24769 2024-03-01 08:30:20.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/date.py
--rw-r--r--   0        0        0     1945 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/date_offset.py
--rw-r--r--   0        0        0     3421 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/decimal_.py
--rw-r--r--   0        0        0     1578 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/diagnostics.py
--rw-r--r--   0        0        0     1607 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/double.py
--rw-r--r--   0        0        0     1089 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/encoding.py
--rw-r--r--   0        0        0     5357 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/event.py
--rw-r--r--   0        0        0        0 2024-03-20 08:48:34.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/__init__.py
--rw-r--r--   0        0        0     5685 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/choice.py
--rw-r--r--   0        0        0     1590 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_collections.py
--rw-r--r--   0        0        0     3731 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_core.py
--rw-r--r--   0        0        0     1652 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/global_.py
--rw-r--r--   0        0        0    63297 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/map.py
--rw-r--r--   0        0        0    13120 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/mutable_map.py
--rw-r--r--   0        0        0     8561 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/mutable_set.py
--rw-r--r--   0        0        0     3975 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/range.py
--rw-r--r--   0        0        0     4780 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/result.py
--rw-r--r--   0        0        0    64235 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/seq.py
--rw-r--r--   0        0        0     7439 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/seq2.py
--rw-r--r--   0        0        0    89044 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/set.py
--rw-r--r--   0        0        0    13519 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/system_collections_generic.py
--rw-r--r--   0        0        0     7292 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/system_text.py
--rw-r--r--   0        0        0     2779 2024-02-29 11:27:16.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/file.py
--rw-r--r--   0        0        0     1590 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fsharp_collections.py
--rw-r--r--   0        0        0     3731 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fsharp_core.py
--rw-r--r--   0        0        0     1652 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/global_.py
--rw-r--r--   0        0        0      727 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/guid.py
--rw-r--r--   0        0        0     1962 2024-02-29 11:27:16.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/int32.py
--rw-r--r--   0        0        0    55445 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/list.py
--rw-r--r--   0        0        0     5014 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/long.py
--rw-r--r--   0        0        0     5267 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mailbox_processor.py
--rw-r--r--   0        0        0    63297 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/map.py
--rw-r--r--   0        0        0     3489 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/map_util.py
--rw-r--r--   0        0        0    13120 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mutable_map.py
--rw-r--r--   0        0        0     8561 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mutable_set.py
--rw-r--r--   0        0        0     1104 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/native.py
--rw-r--r--   0        0        0      997 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/numeric.py
--rw-r--r--   0        0        0     6437 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/observable.py
--rw-r--r--   0        0        0     2913 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/option.py
--rw-r--r--   0        0        0     1265 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/path.py
--rw-r--r--   0        0        0     3975 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/range.py
--rw-r--r--   0        0        0    12890 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/reflection.py
--rw-r--r--   0        0        0     3424 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/reg_exp.py
--rw-r--r--   0        0        0      762 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/resize_array.py
--rw-r--r--   0        0        0     4780 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/result.py
--rw-r--r--   0        0        0    64235 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/seq.py
--rw-r--r--   0        0        0     7439 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/seq2.py
--rw-r--r--   0        0        0    89044 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/set.py
--rw-r--r--   0        0        0     1160 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/singleton_local_time_zone.py
--rw-r--r--   0        0        0    16949 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/string_.py
--rw-r--r--   0        0        0    13519 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/system_collections_generic.py
--rw-r--r--   0        0        0     7292 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/system_text.py
--rw-r--r--   0        0        0     2533 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/task.py
--rw-r--r--   0        0        0     3636 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/task_builder.py
--rw-r--r--   0        0        0       90 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/thread.py
--rw-r--r--   0        0        0     7435 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/time_span.py
--rw-r--r--   0        0        0      563 2024-03-20 08:48:38.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/timer.py
--rw-r--r--   0        0        0     8974 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/types.py
--rw-r--r--   0        0        0     3036 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/uri.py
--rw-r--r--   0        0        0    77185 2024-02-20 20:29:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_library/util.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:24.907760 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/cognite-sdk/__init__.py
--rw-r--r--   0        0        0      563 2024-04-05 14:00:24.907760 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/cognite-sdk/cognite_sdk.py
--rw-r--r--   0        0        0      538 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/cognite-sdk/CogniteSdk.fs
--rw-r--r--   0        0        0     1799 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/Fable.Python.fsproj
--rw-r--r--   0        0        0        0 2024-04-05 14:00:24.907760 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/flask/__init__.py
--rw-r--r--   0        0        0      887 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/flask/Flask.fs
--rw-r--r--   0        0        0      628 2024-04-05 14:00:24.907760 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/flask/flask.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:24.917792 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/__init__.py
--rw-r--r--   0        0        0      772 2024-04-05 14:00:24.924423 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/ipy_widgets.py
--rw-r--r--   0        0        0      400 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/IPython.fs
--rw-r--r--   0        0        0      259 2024-04-05 14:00:24.917792 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/ipython.py
--rw-r--r--   0        0        0     1052 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/IPyWidgets.fs
--rw-r--r--   0        0        0      362 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:00:24.507982 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/__init__.py
--rw-r--r--   0        0        0     3183 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Ast.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.524611 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/ast.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:24.183213 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/__init__.py
--rw-r--r--   0        0        0      200 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/Events.fs
--rw-r--r--   0        0        0      355 2024-04-05 14:00:24.183213 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/events.py
--rw-r--r--   0        0        0      674 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/Futures.fs
--rw-r--r--   0        0        0     1062 2024-04-05 14:00:24.183213 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/futures.py
--rw-r--r--   0        0        0     1164 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/Tasks.fs
--rw-r--r--   0        0        0      820 2024-04-05 14:00:24.278257 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/tasks.py
--rw-r--r--   0        0        0     1188 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Base64.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.507982 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/base64_.py
--rw-r--r--   0        0        0     5639 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Builtins.fs
--rw-r--r--   0        0        0      831 2024-04-05 14:00:24.824642 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/builtins_.py
--rw-r--r--   0        0        0      302 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Html.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.680422 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/html.py
--rw-r--r--   0        0        0      235 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Json.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.680422 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/json.py
--rw-r--r--   0        0        0     1335 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Math.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.680422 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/math_.py
--rw-r--r--   0        0        0      736 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Os.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.680422 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/os_.py
--rw-r--r--   0        0        0     4896 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Queue.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.790992 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/queue_.py
--rw-r--r--   0        0        0      214 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/String.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.790992 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/string_.py
--rw-r--r--   0        0        0      716 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Sys.fs
--rw-r--r--   0        0        0      503 2024-04-05 14:00:24.805505 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/sys_.py
--rw-r--r--   0        0        0      572 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Time.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.805505 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/time_.py
--rw-r--r--   0        0        0        2 2024-04-05 14:00:24.885498 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/tk_inter.py
--rw-r--r--   0        0        0     1669 2023-10-19 07:05:32.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/TkInter.fs
--rw-r--r--   0        0        0        0 2024-04-05 14:00:25.093722 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/__init__.py
--rw-r--r--   0        0        0     1158 2022-08-19 12:26:48.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Fable.SimpleHttp.fsproj
--rw-r--r--   0        0        0    14549 2022-08-04 11:00:56.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Http.fs
--rw-r--r--   0        0        0    16867 2024-04-05 14:00:25.588713 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/http.py
--rw-r--r--   0        0        0     1023 2022-06-12 21:10:06.000000 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Types.fs
--rw-r--r--   0        0        0     4631 2024-04-05 14:00:25.093722 arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/types.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:25.588713 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:25.732422 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/__init__.py
--rw-r--r--   0        0        0    16722 2024-04-05 14:00:25.732422 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cell.py
--rw-r--r--   0        0        0    21064 2024-04-05 14:00:25.797495 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cells_collection.py
--rw-r--r--   0        0        0    14966 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/FsCell.fs
--rw-r--r--   0        0        0    28519 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/FsCellsCollection.fs
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.182253 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/__init__.py
--rw-r--r--   0        0        0     9674 2024-04-05 14:00:26.375246 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/cell_builder.py
--rw-r--r--   0        0        0     7331 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/CellBuilder.fs
--rw-r--r--   0        0        0     6738 2024-04-05 14:00:26.441326 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/column_builder.py
--rw-r--r--   0        0        0     7704 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/ColumnBuilder.fs
--rw-r--r--   0        0        0     2108 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/DSL.fs
--rw-r--r--   0        0        0     1636 2024-04-05 14:00:26.491177 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/dsl.py
--rw-r--r--   0        0        0      577 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Expression.fs
--rw-r--r--   0        0        0     1926 2024-04-05 14:00:26.182253 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/expression.py
--rw-r--r--   0        0        0     3861 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Operators.fs
--rw-r--r--   0        0        0      344 2024-04-05 14:00:26.295157 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/operators.py
--rw-r--r--   0        0        0     6530 2024-04-05 14:00:26.407951 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/row_builder.py
--rw-r--r--   0        0        0     7348 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/RowBuilder.fs
--rw-r--r--   0        0        0     4318 2024-04-05 14:00:26.474647 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/sheet_builder.py
--rw-r--r--   0        0        0     4952 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/SheetBuilder.fs
--rw-r--r--   0        0        0     4428 2024-04-05 14:00:26.454915 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/table_builder.py
--rw-r--r--   0        0        0     4244 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/TableBuilder.fs
--rw-r--r--   0        0        0    11104 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Transform.fs
--rw-r--r--   0        0        0    20668 2024-04-05 14:00:26.343454 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/transform.py
--rw-r--r--   0        0        0     3943 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Types.fs
--rw-r--r--   0        0        0     9760 2024-04-05 14:00:26.247028 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/types.py
--rw-r--r--   0        0        0     3898 2024-04-05 14:00:26.486662 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/workbook_builder.py
--rw-r--r--   0        0        0     4084 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/WorkbookBuilder.fs
--rw-r--r--   0        0        0     9464 2024-04-05 14:00:25.588713 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_address.py
--rw-r--r--   0        0        0     7319 2024-04-05 14:00:25.861254 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_column.py
--rw-r--r--   0        0        0     7603 2024-04-05 14:00:25.853123 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_row.py
--rw-r--r--   0        0        0     6429 2024-04-05 14:00:26.141323 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_workbook.py
--rw-r--r--   0        0        0    23625 2024-04-05 14:00:26.174646 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_worksheet.py
--rw-r--r--   0        0        0     7182 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsAddress.fs
--rw-r--r--   0        0        0     8213 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsColumn.fs
--rw-r--r--   0        0        0     8040 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsRow.fs
--rw-r--r--   0        0        0     2378 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsSpreadsheet.fsproj
--rw-r--r--   0        0        0     6657 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsWorkbook.fs
--rw-r--r--   0        0        0    24875 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsWorksheet.fs
--rw-r--r--   0        0        0      184 2024-02-13 12:15:00.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
--rw-r--r--   0        0        0      993 2024-02-13 12:15:00.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs
--rw-r--r--   0        0        0      184 2024-02-13 12:15:04.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
--rw-r--r--   0        0        0      995 2024-02-13 12:16:56.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs
--rw-r--r--   0        0        0        0 2024-04-05 14:00:25.764591 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-05 14:00:25.808014 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range.py
--rw-r--r--   0        0        0     9231 2024-04-05 14:00:25.780677 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_address.py
--rw-r--r--   0        0        0     4662 2024-04-05 14:00:25.774657 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_base.py
--rw-r--r--   0        0        0     4488 2024-04-05 14:00:25.797495 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_column.py
--rw-r--r--   0        0        0     2488 2024-04-05 14:00:25.764591 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_row.py
--rw-r--r--   0        0        0      943 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRange.fs
--rw-r--r--   0        0        0     7801 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeAddress.fs
--rw-r--r--   0        0        0     3618 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeBase.fs
--rw-r--r--   0        0        0     2407 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeColumn.fs
--rw-r--r--   0        0        0      761 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeRow.fs
--rw-r--r--   0        0        0    18095 2024-04-05 14:00:26.241003 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/sheet_builder.py
--rw-r--r--   0        0        0    11695 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/SheetBuilder.fs
--rw-r--r--   0        0        0        0 2024-04-05 14:00:25.853123 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/__init__.py
--rw-r--r--   0        0        0    21031 2024-04-05 14:00:26.024663 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table.py
--rw-r--r--   0        0        0     6013 2024-04-05 14:00:25.874374 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_field.py
--rw-r--r--   0        0        0      700 2024-04-05 14:00:25.853123 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_row.py
--rw-r--r--   0        0        0    22246 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/FsTable.fs
--rw-r--r--   0        0        0     6134 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableField.fs
--rw-r--r--   0        0        0      142 2024-02-12 11:12:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableRow.fs
--rw-r--r--   0        0        0    24722 2024-04-05 14:00:22.090937 arctrl-2.0.0a2/arctrl/fable_modules/project_cracked.json
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.507889 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/__init__.py
--rw-r--r--   0        0        0    48945 2023-12-15 17:16:54.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Decode.fs
--rw-r--r--   0        0        0    80300 2024-04-05 14:00:26.957940 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/decode.py
--rw-r--r--   0        0        0     6632 2023-12-15 16:52:30.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Encode.fs
--rw-r--r--   0        0        0     6007 2024-04-05 14:00:26.772652 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/encode.py
--rw-r--r--   0        0        0      200 2024-01-04 16:40:54.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
--rw-r--r--   0        0        0     1150 2024-01-25 09:07:50.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/Thoth.Json.Core.AssemblyInfo.fs
--rw-r--r--   0        0        0     1058 2024-01-25 09:06:30.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Thoth.Json.Core.fsproj
--rw-r--r--   0        0        0     2733 2023-12-07 15:53:10.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Types.fs
--rw-r--r--   0        0        0     5461 2024-04-05 14:00:26.507889 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/types.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.758470 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/__init__.py
--rw-r--r--   0        0        0     2847 2024-01-04 20:26:24.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Decode.fs
--rw-r--r--   0        0        0     3765 2024-04-05 14:00:26.774686 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/decode.py
--rw-r--r--   0        0        0     1685 2024-04-03 14:51:06.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Encode.fs
--rw-r--r--   0        0        0     1710 2024-04-05 14:00:26.774686 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/encode.py
--rw-r--r--   0        0        0      200 2024-01-04 16:40:54.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
--rw-r--r--   0        0        0      879 2024-03-13 09:22:54.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs
--rw-r--r--   0        0        0      200 2024-01-25 09:08:08.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
--rw-r--r--   0        0        0      922 2024-04-03 14:54:28.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs
--rw-r--r--   0        0        0      455 2024-04-03 14:50:42.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Python.fs
--rw-r--r--   0        0        0        2 2024-04-05 14:00:26.758470 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/python.py
--rw-r--r--   0        0        0      841 2024-04-03 14:46:22.000000 arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Thoth.Json.Python.fsproj
--rw-r--r--   0        0        0        0 2024-04-05 14:00:26.791899 arctrl-2.0.0a2/arctrl/FileSystem/__init__.py
--rw-r--r--   0        0        0      703 2024-04-05 14:00:26.791899 arctrl-2.0.0a2/arctrl/FileSystem/commit.py
--rw-r--r--   0        0        0     1530 2024-04-05 14:00:26.791899 arctrl-2.0.0a2/arctrl/FileSystem/default_gitignore.py
--rw-r--r--   0        0        0     2298 2024-04-05 14:00:26.857690 arctrl-2.0.0a2/arctrl/FileSystem/file_system.py
--rw-r--r--   0        0        0    15233 2024-04-05 14:00:26.886751 arctrl-2.0.0a2/arctrl/FileSystem/file_system_tree.py
--rw-r--r--   0        0        0     1426 2024-04-05 14:00:26.791899 arctrl-2.0.0a2/arctrl/FileSystem/path.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:29.541319 arctrl-2.0.0a2/arctrl/Json/__init__.py
--rw-r--r--   0        0        0     1739 2024-04-05 14:00:30.379213 arctrl-2.0.0a2/arctrl/Json/arc.py
--rw-r--r--   0        0        0    23698 2024-04-05 14:00:30.282682 arctrl-2.0.0a2/arctrl/Json/assay.py
--rw-r--r--   0        0        0     6932 2024-04-05 14:00:29.610169 arctrl-2.0.0a2/arctrl/Json/comment.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:29.401440 arctrl-2.0.0a2/arctrl/Json/context/rocrate/__init__.py
--rw-r--r--   0        0        0     2076 2024-04-05 14:00:29.407956 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_assay_context.py
--rw-r--r--   0        0        0     1266 2024-04-05 14:00:29.407956 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_comment_context.py
--rw-r--r--   0        0        0     1578 2024-04-05 14:00:29.407956 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_component_context.py
--rw-r--r--   0        0        0     1581 2024-04-05 14:00:29.417472 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_data_context.py
--rw-r--r--   0        0        0     1750 2024-04-05 14:00:29.424492 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_factor_context.py
--rw-r--r--   0        0        0     1428 2024-04-05 14:00:29.433511 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_factor_value_context.py
--rw-r--r--   0        0        0     2875 2024-04-05 14:00:29.433511 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_investigation_context.py
--rw-r--r--   0        0        0     1602 2024-04-05 14:00:29.449542 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_attribute_context.py
--rw-r--r--   0        0        0     1446 2024-04-05 14:00:29.449542 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_attribute_value_context.py
--rw-r--r--   0        0        0     1789 2024-04-05 14:00:29.459121 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_context.py
--rw-r--r--   0        0        0     1349 2024-04-05 14:00:29.465648 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_ontology_annotation_context.py
--rw-r--r--   0        0        0     1835 2024-04-05 14:00:29.481681 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_ontology_source_reference_context.py
--rw-r--r--   0        0        0     1260 2024-04-05 14:00:29.481681 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_organization_context.py
--rw-r--r--   0        0        0     2615 2024-04-05 14:00:29.491196 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_person_context.py
--rw-r--r--   0        0        0     1761 2024-04-05 14:00:29.497713 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_process_context.py
--rw-r--r--   0        0        0     1440 2024-04-05 14:00:29.497713 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_process_parameter_value_context.py
--rw-r--r--   0        0        0     1736 2024-04-05 14:00:29.507728 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_protocol_context.py
--rw-r--r--   0        0        0     1574 2024-04-05 14:00:29.507728 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_protocol_parameter_context.py
--rw-r--r--   0        0        0     1427 2024-04-05 14:00:29.513742 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_publication_context.py
--rw-r--r--   0        0        0     1280 2024-04-05 14:00:29.513742 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_sample_context.py
--rw-r--r--   0        0        0     1633 2024-04-05 14:00:29.524258 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_source_context.py
--rw-r--r--   0        0        0     2575 2024-04-05 14:00:29.529804 arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_study_context.py
--rw-r--r--   0        0        0      629 2024-04-05 14:00:29.401440 arctrl-2.0.0a2/arctrl/Json/context/rocrate/property_value_context.py
--rw-r--r--   0        0        0     1273 2024-04-05 14:00:29.529804 arctrl-2.0.0a2/arctrl/Json/context/rocrate/rocrate_context.py
--rw-r--r--   0        0        0      690 2024-04-05 14:00:29.529804 arctrl-2.0.0a2/arctrl/Json/converter_options.py
--rw-r--r--   0        0        0     7418 2024-04-05 14:00:29.578088 arctrl-2.0.0a2/arctrl/Json/decode.py
--rw-r--r--   0        0        0     2314 2024-04-05 14:00:29.578088 arctrl-2.0.0a2/arctrl/Json/encode.py
--rw-r--r--   0        0        0    31419 2024-04-05 14:00:30.460030 arctrl-2.0.0a2/arctrl/Json/investigation.py
--rw-r--r--   0        0        0    14145 2024-04-05 14:00:29.659341 arctrl-2.0.0a2/arctrl/Json/ontology_annotation.py
--rw-r--r--   0        0        0     9759 2024-04-05 14:00:29.659341 arctrl-2.0.0a2/arctrl/Json/ontology_source_reference.py
--rw-r--r--   0        0        0    22692 2024-04-05 14:00:29.774485 arctrl-2.0.0a2/arctrl/Json/person.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:29.724298 arctrl-2.0.0a2/arctrl/Json/Process/__init__.py
--rw-r--r--   0        0        0     1380 2024-04-05 14:00:30.024440 arctrl-2.0.0a2/arctrl/Json/Process/assay_materials.py
--rw-r--r--   0        0        0     4595 2024-04-05 14:00:29.817728 arctrl-2.0.0a2/arctrl/Json/Process/component.py
--rw-r--r--   0        0        0     7236 2024-04-05 14:00:29.924654 arctrl-2.0.0a2/arctrl/Json/Process/data.py
--rw-r--r--   0        0        0     3823 2024-04-05 14:00:29.898027 arctrl-2.0.0a2/arctrl/Json/Process/data_file.py
--rw-r--r--   0        0        0     3566 2024-04-05 14:00:29.769973 arctrl-2.0.0a2/arctrl/Json/Process/factor.py
--rw-r--r--   0        0        0     4237 2024-04-05 14:00:29.774485 arctrl-2.0.0a2/arctrl/Json/Process/factor_value.py
--rw-r--r--   0        0        0     9324 2024-04-05 14:00:29.898027 arctrl-2.0.0a2/arctrl/Json/Process/material.py
--rw-r--r--   0        0        0     2873 2024-04-05 14:00:29.801660 arctrl-2.0.0a2/arctrl/Json/Process/material_attribute.py
--rw-r--r--   0        0        0     5742 2024-04-05 14:00:29.865933 arctrl-2.0.0a2/arctrl/Json/Process/material_attribute_value.py
--rw-r--r--   0        0        0     3024 2024-04-05 14:00:29.791140 arctrl-2.0.0a2/arctrl/Json/Process/material_type.py
--rw-r--r--   0        0        0    14248 2024-04-05 14:00:30.042491 arctrl-2.0.0a2/arctrl/Json/Process/process.py
--rw-r--r--   0        0        0     4307 2024-04-05 14:00:29.978362 arctrl-2.0.0a2/arctrl/Json/Process/process_input.py
--rw-r--r--   0        0        0     4683 2024-04-05 14:00:29.991382 arctrl-2.0.0a2/arctrl/Json/Process/process_output.py
--rw-r--r--   0        0        0     5520 2024-04-05 14:00:29.962325 arctrl-2.0.0a2/arctrl/Json/Process/process_parameter_value.py
--rw-r--r--   0        0        0     3000 2024-04-05 14:00:30.026466 arctrl-2.0.0a2/arctrl/Json/Process/process_sequence.py
--rw-r--r--   0        0        0     5993 2024-04-05 14:00:29.774485 arctrl-2.0.0a2/arctrl/Json/Process/property_value.py
--rw-r--r--   0        0        0    14643 2024-04-05 14:00:29.874453 arctrl-2.0.0a2/arctrl/Json/Process/protocol.py
--rw-r--r--   0        0        0     2858 2024-04-05 14:00:29.786002 arctrl-2.0.0a2/arctrl/Json/Process/protocol_parameter.py
--rw-r--r--   0        0        0    11205 2024-04-05 14:00:29.978362 arctrl-2.0.0a2/arctrl/Json/Process/sample.py
--rw-r--r--   0        0        0     6840 2024-04-05 14:00:29.941218 arctrl-2.0.0a2/arctrl/Json/Process/source.py
--rw-r--r--   0        0        0     1681 2024-04-05 14:00:30.026466 arctrl-2.0.0a2/arctrl/Json/Process/study_materials.py
--rw-r--r--   0        0        0     2595 2024-04-05 14:00:29.724298 arctrl-2.0.0a2/arctrl/Json/Process/value.py
--rw-r--r--   0        0        0    11674 2024-04-05 14:00:29.753842 arctrl-2.0.0a2/arctrl/Json/publication.py
--rw-r--r--   0        0        0     2072 2024-04-05 14:00:29.594124 arctrl-2.0.0a2/arctrl/Json/string_table.py
--rw-r--r--   0        0        0    36074 2024-04-05 14:00:30.411319 arctrl-2.0.0a2/arctrl/Json/study.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:30.042491 arctrl-2.0.0a2/arctrl/Json/Table/__init__.py
--rw-r--r--   0        0        0    20281 2024-04-05 14:00:30.218411 arctrl-2.0.0a2/arctrl/Json/Table/arc_table.py
--rw-r--r--   0        0        0     2544 2024-04-05 14:00:30.074603 arctrl-2.0.0a2/arctrl/Json/Table/cell_table.py
--rw-r--r--   0        0        0     6812 2024-04-05 14:00:30.074603 arctrl-2.0.0a2/arctrl/Json/Table/composite_cell.py
--rw-r--r--   0        0        0     5124 2024-04-05 14:00:30.106142 arctrl-2.0.0a2/arctrl/Json/Table/composite_header.py
--rw-r--r--   0        0        0     3165 2024-04-05 14:00:30.159750 arctrl-2.0.0a2/arctrl/Json/Table/compression.py
--rw-r--r--   0        0        0     1942 2024-04-05 14:00:30.074603 arctrl-2.0.0a2/arctrl/Json/Table/iotype.py
--rw-r--r--   0        0        0     2455 2024-04-05 14:00:30.042491 arctrl-2.0.0a2/arctrl/Json/Table/oatable.py
--rw-r--r--   0        0        0    12885 2024-04-05 14:00:30.218411 arctrl-2.0.0a2/arctrl/Json/Table/templates.py
--rw-r--r--   0        0        0    11277 2024-04-05 14:00:30.651330 arctrl-2.0.0a2/arctrl/json.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:28.583027 arctrl-2.0.0a2/arctrl/Spreadsheet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:29.176584 arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/__init__.py
--rw-r--r--   0        0        0     7627 2024-04-05 14:00:29.224726 arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/arc_table.py
--rw-r--r--   0        0        0     3295 2024-04-05 14:00:29.176584 arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_cell.py
--rw-r--r--   0        0        0     6938 2024-04-05 14:00:29.208675 arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_column.py
--rw-r--r--   0        0        0    21680 2024-04-05 14:00:29.176584 arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_header.py
--rw-r--r--   0        0        0     8460 2024-04-05 14:00:29.274661 arctrl-2.0.0a2/arctrl/Spreadsheet/arc_assay.py
--rw-r--r--   0        0        0    23446 2024-04-05 14:00:29.407956 arctrl-2.0.0a2/arctrl/Spreadsheet/arc_investigation.py
--rw-r--r--   0        0        0     4634 2024-04-05 14:00:29.291303 arctrl-2.0.0a2/arctrl/Spreadsheet/arc_study.py
--rw-r--r--   0        0        0        2 2024-04-05 14:00:28.583027 arctrl-2.0.0a2/arctrl/Spreadsheet/assembly_info.py
--rw-r--r--   0        0        0     5271 2024-04-05 14:00:28.615092 arctrl-2.0.0a2/arctrl/Spreadsheet/collection_aux.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:28.775814 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/__init__.py
--rw-r--r--   0        0        0     8196 2024-04-05 14:00:29.091357 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/assays.py
--rw-r--r--   0        0        0     2894 2024-04-05 14:00:28.775814 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/comment.py
--rw-r--r--   0        0        0     8094 2024-04-05 14:00:28.957911 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/contacts.py
--rw-r--r--   0        0        0     8867 2024-04-05 14:00:28.841064 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/conversions.py
--rw-r--r--   0        0        0     2013 2024-04-05 14:00:28.941372 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/design_descriptors.py
--rw-r--r--   0        0        0     5842 2024-04-05 14:00:29.007552 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/factors.py
--rw-r--r--   0        0        0     5071 2024-04-05 14:00:28.957911 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/ontology_annotation.py
--rw-r--r--   0        0        0     5167 2024-04-05 14:00:29.144493 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/ontology_source_reference.py
--rw-r--r--   0        0        0    11529 2024-04-05 14:00:29.048187 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/protocols.py
--rw-r--r--   0        0        0     7060 2024-04-05 14:00:29.048187 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/publication.py
--rw-r--r--   0        0        0    22803 2024-04-05 14:00:29.000031 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/sparse_table.py
--rw-r--r--   0        0        0    19198 2024-04-05 14:00:29.158541 arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/study.py
--rw-r--r--   0        0        0    21998 2024-04-05 14:00:29.465648 arctrl-2.0.0a2/arctrl/Spreadsheet/template.py
--rw-r--r--   0        0        0      827 2024-04-05 14:00:30.507778 arctrl-2.0.0a2/arctrl/template_web.py
--rw-r--r--   0        0        0        0 2024-04-05 14:00:30.475574 arctrl-2.0.0a2/arctrl/WebRequest/__init__.py
--rw-r--r--   0        0        0      239 2024-04-05 14:00:30.507778 arctrl-2.0.0a2/arctrl/WebRequest/web_request.py
--rw-r--r--   0        0        0        2 2024-04-05 14:00:30.475574 arctrl-2.0.0a2/arctrl/WebRequest/web_request_node.py
--rw-r--r--   0        0        0     5426 2024-04-05 14:00:30.507778 arctrl-2.0.0a2/arctrl/WebRequest/web_request_py.py
--rw-r--r--   0        0        0     3608 2024-04-05 14:00:30.657847 arctrl-2.0.0a2/arctrl/xlsx.py
--rw-r--r--   0        0        0      707 2024-04-05 14:00:32.526473 arctrl-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     3597 2024-04-05 14:00:32.526473 arctrl-2.0.0a2/README.md
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 arctrl-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:16.813675 arctrl-2.0.0a3/arctrl/__init__.py
+-rw-r--r--   0        0        0    28760 2024-04-22 22:49:17.033671 arctrl-2.0.0a3/arctrl/arc.py
+-rw-r--r--   0        0        0      665 2024-04-22 22:49:21.137476 arctrl-2.0.0a3/arctrl/arctrl.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:16.703742 arctrl-2.0.0a3/arctrl/Contract/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-22 22:49:16.782355 arctrl-2.0.0a3/arctrl/Contract/arc.py
+-rw-r--r--   0        0        0     4937 2024-04-22 22:49:16.734996 arctrl-2.0.0a3/arctrl/Contract/arc_assay.py
+-rw-r--r--   0        0        0     4463 2024-04-22 22:49:16.766695 arctrl-2.0.0a3/arctrl/Contract/arc_investigation.py
+-rw-r--r--   0        0        0     5278 2024-04-22 22:49:16.751050 arctrl-2.0.0a3/arctrl/Contract/arc_study.py
+-rw-r--r--   0        0        0     4312 2024-04-22 22:49:16.688109 arctrl-2.0.0a3/arctrl/Contract/contract.py
+-rw-r--r--   0        0        0     4624 2024-04-22 22:49:16.782355 arctrl-2.0.0a3/arctrl/Contract/git.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.682089 arctrl-2.0.0a3/arctrl/Core/__init__.py
+-rw-r--r--   0        0        0   125598 2024-04-22 22:49:14.709446 arctrl-2.0.0a3/arctrl/Core/arc_types.py
+-rw-r--r--   0        0        0     4349 2024-04-22 22:49:12.728931 arctrl-2.0.0a3/arctrl/Core/comment.py
+-rw-r--r--   0        0        0     3731 2024-04-22 22:49:12.728931 arctrl-2.0.0a3/arctrl/Core/comment_list.py
+-rw-r--r--   0        0        0    59641 2024-04-22 22:49:14.819413 arctrl-2.0.0a3/arctrl/Core/conversion.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.493503 arctrl-2.0.0a3/arctrl/Core/Helper/__init__.py
+-rw-r--r--   0        0        0    10402 2024-04-22 22:49:12.682089 arctrl-2.0.0a3/arctrl/Core/Helper/collections_.py
+-rw-r--r--   0        0        0     1959 2024-04-22 22:49:12.666428 arctrl-2.0.0a3/arctrl/Core/Helper/hash_codes.py
+-rw-r--r--   0        0        0     4311 2024-04-22 22:49:12.635162 arctrl-2.0.0a3/arctrl/Core/Helper/identifier.py
+-rw-r--r--   0        0        0      234 2024-04-22 22:49:12.666428 arctrl-2.0.0a3/arctrl/Core/Helper/printer.py
+-rw-r--r--   0        0        0    18730 2024-04-22 22:49:12.650805 arctrl-2.0.0a3/arctrl/Core/Helper/regex.py
+-rw-r--r--   0        0        0     3316 2024-04-22 22:49:12.697710 arctrl-2.0.0a3/arctrl/Core/Helper/sem_ver.py
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:12.493503 arctrl-2.0.0a3/arctrl/Core/Helper/url.py
+-rw-r--r--   0        0        0     1061 2024-04-22 22:49:14.372863 arctrl-2.0.0a3/arctrl/Core/identifier_setters.py
+-rw-r--r--   0        0        0    10862 2024-04-22 22:49:12.823493 arctrl-2.0.0a3/arctrl/Core/ontology_annotation.py
+-rw-r--r--   0        0        0     4731 2024-04-22 22:49:12.886714 arctrl-2.0.0a3/arctrl/Core/ontology_source_reference.py
+-rw-r--r--   0        0        0    11558 2024-04-22 22:49:12.871125 arctrl-2.0.0a3/arctrl/Core/person.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.902365 arctrl-2.0.0a3/arctrl/Core/Process/__init__.py
+-rw-r--r--   0        0        0    14288 2024-04-22 22:49:13.373911 arctrl-2.0.0a3/arctrl/Core/Process/column_index.py
+-rw-r--r--   0        0        0     8025 2024-04-22 22:49:13.133555 arctrl-2.0.0a3/arctrl/Core/Process/component.py
+-rw-r--r--   0        0        0     2393 2024-04-22 22:49:13.059545 arctrl-2.0.0a3/arctrl/Core/Process/data.py
+-rw-r--r--   0        0        0     1843 2024-04-22 22:49:13.043872 arctrl-2.0.0a3/arctrl/Core/Process/data_file.py
+-rw-r--r--   0        0        0     5936 2024-04-22 22:49:12.949709 arctrl-2.0.0a3/arctrl/Core/Process/factor.py
+-rw-r--r--   0        0        0     6548 2024-04-22 22:49:12.965305 arctrl-2.0.0a3/arctrl/Core/Process/factor_value.py
+-rw-r--r--   0        0        0      643 2024-04-22 22:49:12.902365 arctrl-2.0.0a3/arctrl/Core/Process/iproperty_value.py
+-rw-r--r--   0        0        0     3703 2024-04-22 22:49:13.012218 arctrl-2.0.0a3/arctrl/Core/Process/material.py
+-rw-r--r--   0        0        0     4320 2024-04-22 22:49:12.965305 arctrl-2.0.0a3/arctrl/Core/Process/material_attribute.py
+-rw-r--r--   0        0        0     8009 2024-04-22 22:49:13.012218 arctrl-2.0.0a3/arctrl/Core/Process/material_attribute_value.py
+-rw-r--r--   0        0        0     1270 2024-04-22 22:49:12.980938 arctrl-2.0.0a3/arctrl/Core/Process/material_type.py
+-rw-r--r--   0        0        0    21546 2024-04-22 22:49:13.358267 arctrl-2.0.0a3/arctrl/Core/Process/process.py
+-rw-r--r--   0        0        0     9394 2024-04-22 22:49:13.216712 arctrl-2.0.0a3/arctrl/Core/Process/process_input.py
+-rw-r--r--   0        0        0     8212 2024-04-22 22:49:13.201028 arctrl-2.0.0a3/arctrl/Core/Process/process_output.py
+-rw-r--r--   0        0        0     7173 2024-04-22 22:49:13.233837 arctrl-2.0.0a3/arctrl/Core/Process/process_parameter_value.py
+-rw-r--r--   0        0        0    19068 2024-04-22 22:49:13.358267 arctrl-2.0.0a3/arctrl/Core/Process/process_sequence.py
+-rw-r--r--   0        0        0    10509 2024-04-22 22:49:13.216712 arctrl-2.0.0a3/arctrl/Core/Process/protocol.py
+-rw-r--r--   0        0        0     3889 2024-04-22 22:49:13.133555 arctrl-2.0.0a3/arctrl/Core/Process/protocol_parameter.py
+-rw-r--r--   0        0        0     4117 2024-04-22 22:49:13.043872 arctrl-2.0.0a3/arctrl/Core/Process/sample.py
+-rw-r--r--   0        0        0     2686 2024-04-22 22:49:13.027835 arctrl-2.0.0a3/arctrl/Core/Process/source.py
+-rw-r--r--   0        0        0     6388 2024-04-22 22:49:12.917997 arctrl-2.0.0a3/arctrl/Core/Process/value.py
+-rw-r--r--   0        0        0     6958 2024-04-22 22:49:12.886714 arctrl-2.0.0a3/arctrl/Core/publication.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:13.452531 arctrl-2.0.0a3/arctrl/Core/Table/__init__.py
+-rw-r--r--   0        0        0    48412 2024-04-22 22:49:13.923447 arctrl-2.0.0a3/arctrl/Core/Table/arc_table.py
+-rw-r--r--   0        0        0    24986 2024-04-22 22:49:13.640875 arctrl-2.0.0a3/arctrl/Core/Table/arc_table_aux.py
+-rw-r--r--   0        0        0    25506 2024-04-22 22:49:13.923447 arctrl-2.0.0a3/arctrl/Core/Table/arc_tables.py
+-rw-r--r--   0        0        0     6677 2024-04-22 22:49:13.452531 arctrl-2.0.0a3/arctrl/Core/Table/composite_cell.py
+-rw-r--r--   0        0        0     3471 2024-04-22 22:49:13.468139 arctrl-2.0.0a3/arctrl/Core/Table/composite_column.py
+-rw-r--r--   0        0        0    30828 2024-04-22 22:49:13.499409 arctrl-2.0.0a3/arctrl/Core/Table/composite_header.py
+-rw-r--r--   0        0        0     8330 2024-04-22 22:49:14.206697 arctrl-2.0.0a3/arctrl/Core/template.py
+-rw-r--r--   0        0        0     6294 2024-04-22 22:49:14.222229 arctrl-2.0.0a3/arctrl/Core/templates.py
+-rw-r--r--   0        0        0      180 2024-04-22 22:49:12.682089 arctrl-2.0.0a3/arctrl/Core/uri.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.493503 arctrl-2.0.0a3/arctrl/CWL/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:12.493503 arctrl-2.0.0a3/arctrl/CWL/library.py
+-rw-r--r--   0        0        0        4 2024-04-22 22:49:07.232805 arctrl-2.0.0a3/arctrl/fable_modules/.gitignore
+-rw-r--r--   0        0        0        0 2024-03-20 08:48:34.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/__init__.py
+-rw-r--r--   0        0        0    45250 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/array_.py
+-rw-r--r--   0        0        0    10175 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/async_.py
+-rw-r--r--   0        0        0    10722 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/async_builder.py
+-rw-r--r--   0        0        0     4999 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/big_int.py
+-rw-r--r--   0        0        0     3491 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/bit_converter.py
+-rw-r--r--   0        0        0      607 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/boolean.py
+-rw-r--r--   0        0        0     6477 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/char.py
+-rw-r--r--   0        0        0     5685 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/choice.py
+-rw-r--r--   0        0        0    24769 2024-03-01 08:30:20.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/date.py
+-rw-r--r--   0        0        0     1945 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/date_offset.py
+-rw-r--r--   0        0        0     3421 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/decimal_.py
+-rw-r--r--   0        0        0     1578 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/diagnostics.py
+-rw-r--r--   0        0        0     1607 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/double.py
+-rw-r--r--   0        0        0     1089 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/encoding.py
+-rw-r--r--   0        0        0     5357 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/event.py
+-rw-r--r--   0        0        0        0 2024-03-20 08:48:34.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/__init__.py
+-rw-r--r--   0        0        0     5685 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/choice.py
+-rw-r--r--   0        0        0     1590 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_collections.py
+-rw-r--r--   0        0        0     3731 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_core.py
+-rw-r--r--   0        0        0     1652 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/global_.py
+-rw-r--r--   0        0        0    63297 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/map.py
+-rw-r--r--   0        0        0    13120 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/mutable_map.py
+-rw-r--r--   0        0        0     8561 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/mutable_set.py
+-rw-r--r--   0        0        0     3975 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/range.py
+-rw-r--r--   0        0        0     4780 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/result.py
+-rw-r--r--   0        0        0    64235 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/seq.py
+-rw-r--r--   0        0        0     7439 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/seq2.py
+-rw-r--r--   0        0        0    89044 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/set.py
+-rw-r--r--   0        0        0    13519 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/system_collections_generic.py
+-rw-r--r--   0        0        0     7292 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/system_text.py
+-rw-r--r--   0        0        0     2779 2024-02-29 11:27:16.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/file.py
+-rw-r--r--   0        0        0     1590 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fsharp_collections.py
+-rw-r--r--   0        0        0     3731 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fsharp_core.py
+-rw-r--r--   0        0        0     1652 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/global_.py
+-rw-r--r--   0        0        0      727 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/guid.py
+-rw-r--r--   0        0        0     1962 2024-02-29 11:27:16.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/int32.py
+-rw-r--r--   0        0        0    55445 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/list.py
+-rw-r--r--   0        0        0     5014 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/long.py
+-rw-r--r--   0        0        0     5267 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mailbox_processor.py
+-rw-r--r--   0        0        0    63297 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/map.py
+-rw-r--r--   0        0        0     3489 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/map_util.py
+-rw-r--r--   0        0        0    13120 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mutable_map.py
+-rw-r--r--   0        0        0     8561 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mutable_set.py
+-rw-r--r--   0        0        0     1104 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/native.py
+-rw-r--r--   0        0        0      997 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/numeric.py
+-rw-r--r--   0        0        0     6437 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/observable.py
+-rw-r--r--   0        0        0     2913 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/option.py
+-rw-r--r--   0        0        0     1265 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/path.py
+-rw-r--r--   0        0        0     3975 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/range.py
+-rw-r--r--   0        0        0    12890 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/reflection.py
+-rw-r--r--   0        0        0     3424 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/reg_exp.py
+-rw-r--r--   0        0        0      762 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/resize_array.py
+-rw-r--r--   0        0        0     4780 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/result.py
+-rw-r--r--   0        0        0    64235 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/seq.py
+-rw-r--r--   0        0        0     7439 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/seq2.py
+-rw-r--r--   0        0        0    89044 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/set.py
+-rw-r--r--   0        0        0     1160 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/singleton_local_time_zone.py
+-rw-r--r--   0        0        0    16949 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/string_.py
+-rw-r--r--   0        0        0    13519 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/system_collections_generic.py
+-rw-r--r--   0        0        0     7292 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/system_text.py
+-rw-r--r--   0        0        0     2533 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/task.py
+-rw-r--r--   0        0        0     3636 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/task_builder.py
+-rw-r--r--   0        0        0       90 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/thread.py
+-rw-r--r--   0        0        0     7435 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/time_span.py
+-rw-r--r--   0        0        0      563 2024-03-20 08:48:38.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/timer.py
+-rw-r--r--   0        0        0     8974 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/types.py
+-rw-r--r--   0        0        0     3036 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/uri.py
+-rw-r--r--   0        0        0    77185 2024-02-20 20:29:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_library/util.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/cognite-sdk/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/cognite-sdk/cognite_sdk.py
+-rw-r--r--   0        0        0      538 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/cognite-sdk/CogniteSdk.fs
+-rw-r--r--   0        0        0     1799 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/Fable.Python.fsproj
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/flask/__init__.py
+-rw-r--r--   0        0        0      887 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/flask/Flask.fs
+-rw-r--r--   0        0        0      628 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/flask/flask.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/__init__.py
+-rw-r--r--   0        0        0      772 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/ipy_widgets.py
+-rw-r--r--   0        0        0      400 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/IPython.fs
+-rw-r--r--   0        0        0      259 2024-04-22 22:49:10.480836 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/ipython.py
+-rw-r--r--   0        0        0     1052 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/IPyWidgets.fs
+-rw-r--r--   0        0        0      362 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:10.166978 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/__init__.py
+-rw-r--r--   0        0        0     3183 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Ast.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.166978 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/ast.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:09.950893 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/__init__.py
+-rw-r--r--   0        0        0      200 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/Events.fs
+-rw-r--r--   0        0        0      355 2024-04-22 22:49:09.931026 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/events.py
+-rw-r--r--   0        0        0      674 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/Futures.fs
+-rw-r--r--   0        0        0     1062 2024-04-22 22:49:09.931026 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/futures.py
+-rw-r--r--   0        0        0     1164 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/Tasks.fs
+-rw-r--r--   0        0        0      820 2024-04-22 22:49:10.009799 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/tasks.py
+-rw-r--r--   0        0        0     1188 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Base64.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.166978 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/base64_.py
+-rw-r--r--   0        0        0     5639 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Builtins.fs
+-rw-r--r--   0        0        0      831 2024-04-22 22:49:10.433943 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/builtins_.py
+-rw-r--r--   0        0        0      302 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Html.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.276807 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/html.py
+-rw-r--r--   0        0        0      235 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Json.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.276807 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/json.py
+-rw-r--r--   0        0        0     1335 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Math.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.292431 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/math_.py
+-rw-r--r--   0        0        0      736 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Os.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.292431 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/os_.py
+-rw-r--r--   0        0        0     4896 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Queue.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.402283 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/queue_.py
+-rw-r--r--   0        0        0      214 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/String.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.402283 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/string_.py
+-rw-r--r--   0        0        0      716 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Sys.fs
+-rw-r--r--   0        0        0      503 2024-04-22 22:49:10.402283 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/sys_.py
+-rw-r--r--   0        0        0      572 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Time.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.402283 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/time_.py
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:10.465211 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/tk_inter.py
+-rw-r--r--   0        0        0     1669 2023-10-19 07:05:32.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/TkInter.fs
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:10.606298 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/__init__.py
+-rw-r--r--   0        0        0     1158 2022-08-19 12:26:48.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Fable.SimpleHttp.fsproj
+-rw-r--r--   0        0        0    14549 2022-08-04 11:00:56.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Http.fs
+-rw-r--r--   0        0        0    16867 2024-04-22 22:49:11.085115 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/http.py
+-rw-r--r--   0        0        0     1023 2022-06-12 21:10:06.000000 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Types.fs
+-rw-r--r--   0        0        0     4631 2024-04-22 22:49:10.606298 arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/types.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:11.085115 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:11.203982 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/__init__.py
+-rw-r--r--   0        0        0    16722 2024-04-22 22:49:11.203982 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cell.py
+-rw-r--r--   0        0        0    21064 2024-04-22 22:49:11.298193 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cells_collection.py
+-rw-r--r--   0        0        0    14966 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/FsCell.fs
+-rw-r--r--   0        0        0    28519 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/FsCellsCollection.fs
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:11.644259 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/__init__.py
+-rw-r--r--   0        0        0     9674 2024-04-22 22:49:11.951038 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/cell_builder.py
+-rw-r--r--   0        0        0     7331 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/CellBuilder.fs
+-rw-r--r--   0        0        0     6738 2024-04-22 22:49:12.021580 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/column_builder.py
+-rw-r--r--   0        0        0     7704 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/ColumnBuilder.fs
+-rw-r--r--   0        0        0     2108 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/DSL.fs
+-rw-r--r--   0        0        0     1636 2024-04-22 22:49:12.100267 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/dsl.py
+-rw-r--r--   0        0        0      577 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Expression.fs
+-rw-r--r--   0        0        0     1926 2024-04-22 22:49:11.644259 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/expression.py
+-rw-r--r--   0        0        0     3861 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Operators.fs
+-rw-r--r--   0        0        0      344 2024-04-22 22:49:11.770096 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/operators.py
+-rw-r--r--   0        0        0     6530 2024-04-22 22:49:11.974800 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/row_builder.py
+-rw-r--r--   0        0        0     7348 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/RowBuilder.fs
+-rw-r--r--   0        0        0     4318 2024-04-22 22:49:12.068989 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/sheet_builder.py
+-rw-r--r--   0        0        0     4952 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/SheetBuilder.fs
+-rw-r--r--   0        0        0     4428 2024-04-22 22:49:12.030103 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/table_builder.py
+-rw-r--r--   0        0        0     4244 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/TableBuilder.fs
+-rw-r--r--   0        0        0    11104 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Transform.fs
+-rw-r--r--   0        0        0    20668 2024-04-22 22:49:11.912030 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/transform.py
+-rw-r--r--   0        0        0     3943 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Types.fs
+-rw-r--r--   0        0        0     9760 2024-04-22 22:49:11.722498 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/types.py
+-rw-r--r--   0        0        0     3898 2024-04-22 22:49:12.084622 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/workbook_builder.py
+-rw-r--r--   0        0        0     4084 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/WorkbookBuilder.fs
+-rw-r--r--   0        0        0     9464 2024-04-22 22:49:11.085115 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_address.py
+-rw-r--r--   0        0        0     7319 2024-04-22 22:49:11.361187 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_column.py
+-rw-r--r--   0        0        0     7603 2024-04-22 22:49:11.345578 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_row.py
+-rw-r--r--   0        0        0     6429 2024-04-22 22:49:11.596851 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_workbook.py
+-rw-r--r--   0        0        0    23625 2024-04-22 22:49:11.644259 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_worksheet.py
+-rw-r--r--   0        0        0     7182 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsAddress.fs
+-rw-r--r--   0        0        0     8213 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsColumn.fs
+-rw-r--r--   0        0        0     8040 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsRow.fs
+-rw-r--r--   0        0        0     2378 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsSpreadsheet.fsproj
+-rw-r--r--   0        0        0     6657 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsWorkbook.fs
+-rw-r--r--   0        0        0    24875 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsWorksheet.fs
+-rw-r--r--   0        0        0      184 2024-02-13 12:15:00.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
+-rw-r--r--   0        0        0      993 2024-02-13 12:15:00.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs
+-rw-r--r--   0        0        0      184 2024-02-13 12:15:04.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
+-rw-r--r--   0        0        0      995 2024-02-13 12:16:56.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:11.266945 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-22 22:49:11.298193 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range.py
+-rw-r--r--   0        0        0     9231 2024-04-22 22:49:11.266945 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_address.py
+-rw-r--r--   0        0        0     4662 2024-04-22 22:49:11.266945 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_base.py
+-rw-r--r--   0        0        0     4488 2024-04-22 22:49:11.298193 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_column.py
+-rw-r--r--   0        0        0     2488 2024-04-22 22:49:11.266945 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_row.py
+-rw-r--r--   0        0        0      943 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRange.fs
+-rw-r--r--   0        0        0     7801 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeAddress.fs
+-rw-r--r--   0        0        0     3618 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeBase.fs
+-rw-r--r--   0        0        0     2407 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeColumn.fs
+-rw-r--r--   0        0        0      761 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeRow.fs
+-rw-r--r--   0        0        0    18095 2024-04-22 22:49:11.706878 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/sheet_builder.py
+-rw-r--r--   0        0        0    11695 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/SheetBuilder.fs
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:11.376811 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/__init__.py
+-rw-r--r--   0        0        0    21031 2024-04-22 22:49:11.534235 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table.py
+-rw-r--r--   0        0        0     6013 2024-04-22 22:49:11.392438 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_field.py
+-rw-r--r--   0        0        0      700 2024-04-22 22:49:11.376811 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_row.py
+-rw-r--r--   0        0        0    22246 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/FsTable.fs
+-rw-r--r--   0        0        0     6134 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableField.fs
+-rw-r--r--   0        0        0      142 2024-02-12 11:12:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableRow.fs
+-rw-r--r--   0        0        0    24722 2024-04-22 22:49:07.625794 arctrl-2.0.0a3/arctrl/fable_modules/project_cracked.json
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.130506 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/__init__.py
+-rw-r--r--   0        0        0    48945 2023-12-15 17:16:54.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Decode.fs
+-rw-r--r--   0        0        0    80300 2024-04-22 22:49:12.619128 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/decode.py
+-rw-r--r--   0        0        0     6632 2023-12-15 16:52:30.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Encode.fs
+-rw-r--r--   0        0        0     6007 2024-04-22 22:49:12.383332 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/encode.py
+-rw-r--r--   0        0        0      200 2024-01-04 16:40:54.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
+-rw-r--r--   0        0        0     1150 2024-01-25 09:07:50.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/Thoth.Json.Core.AssemblyInfo.fs
+-rw-r--r--   0        0        0     1058 2024-01-25 09:06:30.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Thoth.Json.Core.fsproj
+-rw-r--r--   0        0        0     2733 2023-12-07 15:53:10.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Types.fs
+-rw-r--r--   0        0        0     5461 2024-04-22 22:49:12.115974 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/types.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.352057 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/__init__.py
+-rw-r--r--   0        0        0     2847 2024-01-04 20:26:24.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Decode.fs
+-rw-r--r--   0        0        0     3765 2024-04-22 22:49:12.433490 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/decode.py
+-rw-r--r--   0        0        0     1685 2024-04-03 14:51:06.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Encode.fs
+-rw-r--r--   0        0        0     1710 2024-04-22 22:49:12.433490 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/encode.py
+-rw-r--r--   0        0        0      200 2024-01-04 16:40:54.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
+-rw-r--r--   0        0        0      879 2024-03-13 09:22:54.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs
+-rw-r--r--   0        0        0      200 2024-01-25 09:08:08.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/.NETStandard,Version=v2.0.AssemblyAttributes.fs
+-rw-r--r--   0        0        0      922 2024-04-03 14:54:28.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs
+-rw-r--r--   0        0        0      455 2024-04-03 14:50:42.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Python.fs
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:12.352057 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/python.py
+-rw-r--r--   0        0        0      841 2024-04-03 14:46:22.000000 arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Thoth.Json.Python.fsproj
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:12.433490 arctrl-2.0.0a3/arctrl/FileSystem/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-22 22:49:12.433490 arctrl-2.0.0a3/arctrl/FileSystem/commit.py
+-rw-r--r--   0        0        0     1530 2024-04-22 22:49:12.433490 arctrl-2.0.0a3/arctrl/FileSystem/default_gitignore.py
+-rw-r--r--   0        0        0     2298 2024-04-22 22:49:12.493503 arctrl-2.0.0a3/arctrl/FileSystem/file_system.py
+-rw-r--r--   0        0        0    15233 2024-04-22 22:49:12.556629 arctrl-2.0.0a3/arctrl/FileSystem/file_system_tree.py
+-rw-r--r--   0        0        0     1426 2024-04-22 22:49:12.446611 arctrl-2.0.0a3/arctrl/FileSystem/path.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:15.777509 arctrl-2.0.0a3/arctrl/Json/__init__.py
+-rw-r--r--   0        0        0     1739 2024-04-22 22:49:16.656837 arctrl-2.0.0a3/arctrl/Json/arc.py
+-rw-r--r--   0        0        0    23698 2024-04-22 22:49:16.562673 arctrl-2.0.0a3/arctrl/Json/assay.py
+-rw-r--r--   0        0        0     6932 2024-04-22 22:49:15.919316 arctrl-2.0.0a3/arctrl/Json/comment.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:15.494597 arctrl-2.0.0a3/arctrl/Json/context/rocrate/__init__.py
+-rw-r--r--   0        0        0     2076 2024-04-22 22:49:15.510231 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_assay_context.py
+-rw-r--r--   0        0        0     1266 2024-04-22 22:49:15.510231 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_comment_context.py
+-rw-r--r--   0        0        0     1578 2024-04-22 22:49:15.525850 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_component_context.py
+-rw-r--r--   0        0        0     1581 2024-04-22 22:49:15.540969 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_data_context.py
+-rw-r--r--   0        0        0     1750 2024-04-22 22:49:15.542105 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_factor_context.py
+-rw-r--r--   0        0        0     1428 2024-04-22 22:49:15.557851 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_factor_value_context.py
+-rw-r--r--   0        0        0     2875 2024-04-22 22:49:15.573465 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_investigation_context.py
+-rw-r--r--   0        0        0     1602 2024-04-22 22:49:15.573465 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_attribute_context.py
+-rw-r--r--   0        0        0     1446 2024-04-22 22:49:15.589117 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_attribute_value_context.py
+-rw-r--r--   0        0        0     1789 2024-04-22 22:49:15.620363 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_context.py
+-rw-r--r--   0        0        0     1349 2024-04-22 22:49:15.620363 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_ontology_annotation_context.py
+-rw-r--r--   0        0        0     1835 2024-04-22 22:49:15.641104 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_ontology_source_reference_context.py
+-rw-r--r--   0        0        0     1260 2024-04-22 22:49:15.651731 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_organization_context.py
+-rw-r--r--   0        0        0     2615 2024-04-22 22:49:15.667480 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_person_context.py
+-rw-r--r--   0        0        0     1761 2024-04-22 22:49:15.683118 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_process_context.py
+-rw-r--r--   0        0        0     1440 2024-04-22 22:49:15.683118 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_process_parameter_value_context.py
+-rw-r--r--   0        0        0     1736 2024-04-22 22:49:15.698653 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_protocol_context.py
+-rw-r--r--   0        0        0     1574 2024-04-22 22:49:15.698653 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_protocol_parameter_context.py
+-rw-r--r--   0        0        0     1427 2024-04-22 22:49:15.741592 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_publication_context.py
+-rw-r--r--   0        0        0     1280 2024-04-22 22:49:15.746215 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_sample_context.py
+-rw-r--r--   0        0        0     1633 2024-04-22 22:49:15.746215 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_source_context.py
+-rw-r--r--   0        0        0     2575 2024-04-22 22:49:15.761961 arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_study_context.py
+-rw-r--r--   0        0        0      629 2024-04-22 22:49:15.494597 arctrl-2.0.0a3/arctrl/Json/context/rocrate/property_value_context.py
+-rw-r--r--   0        0        0     1273 2024-04-22 22:49:15.777509 arctrl-2.0.0a3/arctrl/Json/context/rocrate/rocrate_context.py
+-rw-r--r--   0        0        0      690 2024-04-22 22:49:15.777509 arctrl-2.0.0a3/arctrl/Json/converter_options.py
+-rw-r--r--   0        0        0     7418 2024-04-22 22:49:15.824969 arctrl-2.0.0a3/arctrl/Json/decode.py
+-rw-r--r--   0        0        0     2314 2024-04-22 22:49:15.824969 arctrl-2.0.0a3/arctrl/Json/encode.py
+-rw-r--r--   0        0        0    31419 2024-04-22 22:49:16.782355 arctrl-2.0.0a3/arctrl/Json/investigation.py
+-rw-r--r--   0        0        0    14155 2024-04-22 22:49:15.982384 arctrl-2.0.0a3/arctrl/Json/ontology_annotation.py
+-rw-r--r--   0        0        0     9749 2024-04-22 22:49:15.982384 arctrl-2.0.0a3/arctrl/Json/ontology_source_reference.py
+-rw-r--r--   0        0        0    22692 2024-04-22 22:49:16.076557 arctrl-2.0.0a3/arctrl/Json/person.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:16.060932 arctrl-2.0.0a3/arctrl/Json/Process/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-22 22:49:16.311863 arctrl-2.0.0a3/arctrl/Json/Process/assay_materials.py
+-rw-r--r--   0        0        0     4595 2024-04-22 22:49:16.142576 arctrl-2.0.0a3/arctrl/Json/Process/component.py
+-rw-r--r--   0        0        0     7236 2024-04-22 22:49:16.233239 arctrl-2.0.0a3/arctrl/Json/Process/data.py
+-rw-r--r--   0        0        0     3823 2024-04-22 22:49:16.202002 arctrl-2.0.0a3/arctrl/Json/Process/data_file.py
+-rw-r--r--   0        0        0     3566 2024-04-22 22:49:16.092181 arctrl-2.0.0a3/arctrl/Json/Process/factor.py
+-rw-r--r--   0        0        0     4237 2024-04-22 22:49:16.107819 arctrl-2.0.0a3/arctrl/Json/Process/factor_value.py
+-rw-r--r--   0        0        0     9324 2024-04-22 22:49:16.202002 arctrl-2.0.0a3/arctrl/Json/Process/material.py
+-rw-r--r--   0        0        0     2873 2024-04-22 22:49:16.123438 arctrl-2.0.0a3/arctrl/Json/Process/material_attribute.py
+-rw-r--r--   0        0        0     5742 2024-04-22 22:49:16.186401 arctrl-2.0.0a3/arctrl/Json/Process/material_attribute_value.py
+-rw-r--r--   0        0        0     3024 2024-04-22 22:49:16.123438 arctrl-2.0.0a3/arctrl/Json/Process/material_type.py
+-rw-r--r--   0        0        0    14248 2024-04-22 22:49:16.342990 arctrl-2.0.0a3/arctrl/Json/Process/process.py
+-rw-r--r--   0        0        0     4307 2024-04-22 22:49:16.280582 arctrl-2.0.0a3/arctrl/Json/Process/process_input.py
+-rw-r--r--   0        0        0     4683 2024-04-22 22:49:16.280582 arctrl-2.0.0a3/arctrl/Json/Process/process_output.py
+-rw-r--r--   0        0        0     5520 2024-04-22 22:49:16.264958 arctrl-2.0.0a3/arctrl/Json/Process/process_parameter_value.py
+-rw-r--r--   0        0        0     3000 2024-04-22 22:49:16.311863 arctrl-2.0.0a3/arctrl/Json/Process/process_sequence.py
+-rw-r--r--   0        0        0     7415 2024-04-22 22:49:16.092181 arctrl-2.0.0a3/arctrl/Json/Process/property_value.py
+-rw-r--r--   0        0        0    14643 2024-04-22 22:49:16.217629 arctrl-2.0.0a3/arctrl/Json/Process/protocol.py
+-rw-r--r--   0        0        0     2858 2024-04-22 22:49:16.107819 arctrl-2.0.0a3/arctrl/Json/Process/protocol_parameter.py
+-rw-r--r--   0        0        0    11205 2024-04-22 22:49:16.280582 arctrl-2.0.0a3/arctrl/Json/Process/sample.py
+-rw-r--r--   0        0        0     6840 2024-04-22 22:49:16.242757 arctrl-2.0.0a3/arctrl/Json/Process/source.py
+-rw-r--r--   0        0        0     1681 2024-04-22 22:49:16.342990 arctrl-2.0.0a3/arctrl/Json/Process/study_materials.py
+-rw-r--r--   0        0        0     2595 2024-04-22 22:49:16.060932 arctrl-2.0.0a3/arctrl/Json/Process/value.py
+-rw-r--r--   0        0        0    11674 2024-04-22 22:49:16.076557 arctrl-2.0.0a3/arctrl/Json/publication.py
+-rw-r--r--   0        0        0     2072 2024-04-22 22:49:15.841640 arctrl-2.0.0a3/arctrl/Json/string_table.py
+-rw-r--r--   0        0        0    36074 2024-04-22 22:49:16.688109 arctrl-2.0.0a3/arctrl/Json/study.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:16.374266 arctrl-2.0.0a3/arctrl/Json/Table/__init__.py
+-rw-r--r--   0        0        0    20281 2024-04-22 22:49:16.484072 arctrl-2.0.0a3/arctrl/Json/Table/arc_table.py
+-rw-r--r--   0        0        0     2544 2024-04-22 22:49:16.374266 arctrl-2.0.0a3/arctrl/Json/Table/cell_table.py
+-rw-r--r--   0        0        0     6812 2024-04-22 22:49:16.374266 arctrl-2.0.0a3/arctrl/Json/Table/composite_cell.py
+-rw-r--r--   0        0        0     5124 2024-04-22 22:49:16.405509 arctrl-2.0.0a3/arctrl/Json/Table/composite_header.py
+-rw-r--r--   0        0        0     3165 2024-04-22 22:49:16.443278 arctrl-2.0.0a3/arctrl/Json/Table/compression.py
+-rw-r--r--   0        0        0     1942 2024-04-22 22:49:16.389889 arctrl-2.0.0a3/arctrl/Json/Table/iotype.py
+-rw-r--r--   0        0        0     2455 2024-04-22 22:49:16.358635 arctrl-2.0.0a3/arctrl/Json/Table/oatable.py
+-rw-r--r--   0        0        0    12885 2024-04-22 22:49:16.499705 arctrl-2.0.0a3/arctrl/Json/Table/templates.py
+-rw-r--r--   0        0        0    11277 2024-04-22 22:49:16.986704 arctrl-2.0.0a3/arctrl/json.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:14.379893 arctrl-2.0.0a3/arctrl/Spreadsheet/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:15.274587 arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/__init__.py
+-rw-r--r--   0        0        0     7627 2024-04-22 22:49:15.340026 arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/arc_table.py
+-rw-r--r--   0        0        0     3295 2024-04-22 22:49:15.274587 arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_cell.py
+-rw-r--r--   0        0        0     6938 2024-04-22 22:49:15.353152 arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_column.py
+-rw-r--r--   0        0        0    21680 2024-04-22 22:49:15.290213 arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_header.py
+-rw-r--r--   0        0        0     8460 2024-04-22 22:49:15.368807 arctrl-2.0.0a3/arctrl/Spreadsheet/arc_assay.py
+-rw-r--r--   0        0        0    23446 2024-04-22 22:49:15.494597 arctrl-2.0.0a3/arctrl/Spreadsheet/arc_investigation.py
+-rw-r--r--   0        0        0     4634 2024-04-22 22:49:15.384516 arctrl-2.0.0a3/arctrl/Spreadsheet/arc_study.py
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:14.379893 arctrl-2.0.0a3/arctrl/Spreadsheet/assembly_info.py
+-rw-r--r--   0        0        0     5271 2024-04-22 22:49:14.437355 arctrl-2.0.0a3/arctrl/Spreadsheet/collection_aux.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:14.489767 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/__init__.py
+-rw-r--r--   0        0        0     8196 2024-04-22 22:49:14.960882 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/assays.py
+-rw-r--r--   0        0        0     2894 2024-04-22 22:49:14.489767 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/comment.py
+-rw-r--r--   0        0        0     8094 2024-04-22 22:49:14.725093 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/contacts.py
+-rw-r--r--   0        0        0     8867 2024-04-22 22:49:14.521022 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/conversions.py
+-rw-r--r--   0        0        0     2013 2024-04-22 22:49:14.693809 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/design_descriptors.py
+-rw-r--r--   0        0        0     5842 2024-04-22 22:49:14.772470 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/factors.py
+-rw-r--r--   0        0        0     5071 2024-04-22 22:49:14.725093 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/ontology_annotation.py
+-rw-r--r--   0        0        0     5167 2024-04-22 22:49:15.196199 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/ontology_source_reference.py
+-rw-r--r--   0        0        0    11529 2024-04-22 22:49:14.882228 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/protocols.py
+-rw-r--r--   0        0        0     7060 2024-04-22 22:49:14.897875 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/publication.py
+-rw-r--r--   0        0        0    22803 2024-04-22 22:49:14.741172 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/sparse_table.py
+-rw-r--r--   0        0        0    19198 2024-04-22 22:49:15.258969 arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/study.py
+-rw-r--r--   0        0        0    21998 2024-04-22 22:49:15.651731 arctrl-2.0.0a3/arctrl/Spreadsheet/template.py
+-rw-r--r--   0        0        0      827 2024-04-22 22:49:16.813675 arctrl-2.0.0a3/arctrl/template_web.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:49:16.782355 arctrl-2.0.0a3/arctrl/WebRequest/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-22 22:49:16.813675 arctrl-2.0.0a3/arctrl/WebRequest/web_request.py
+-rw-r--r--   0        0        0        2 2024-04-22 22:49:16.782355 arctrl-2.0.0a3/arctrl/WebRequest/web_request_node.py
+-rw-r--r--   0        0        0     5426 2024-04-22 22:49:16.813675 arctrl-2.0.0a3/arctrl/WebRequest/web_request_py.py
+-rw-r--r--   0        0        0     3608 2024-04-22 22:49:16.986704 arctrl-2.0.0a3/arctrl/xlsx.py
+-rw-r--r--   0        0        0      707 2024-04-22 22:49:21.153114 arctrl-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3597 2024-04-22 22:49:21.169509 arctrl-2.0.0a3/README.md
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 arctrl-2.0.0a3/PKG-INFO
```

### Comparing `arctrl-2.0.0a2/arctrl/arc.py` & `arctrl-2.0.0a3/arctrl/arc.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/arctrl.py` & `arctrl-2.0.0a3/arctrl/arctrl.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Contract/arc.py` & `arctrl-2.0.0a3/arctrl/Contract/arc.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Contract/arc_assay.py` & `arctrl-2.0.0a3/arctrl/Contract/arc_assay.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Contract/arc_investigation.py` & `arctrl-2.0.0a3/arctrl/Contract/arc_investigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from ..Core.arc_types import ArcInvestigation
 from ..FileSystem.path import combine_many
 from ..Spreadsheet.arc_investigation import (to_light_fs_workbook, to_fs_workbook, from_fs_workbook)
 from .contract import (Contract, DTOType, DTO)
 
 def _007CInvestigationPath_007C__007C(input: Array[str]) -> str | None:
     (pattern_matching_result,) = (None,)
-    def _arrow1785(x: str, y: str, input: Any=input) -> bool:
+    def _arrow1717(x: str, y: str, input: Any=input) -> bool:
         return x == y
 
-    if (len(input) == 1) if (not equals_with(_arrow1785, input, None)) else False:
+    if (len(input) == 1) if (not equals_with(_arrow1717, input, None)) else False:
         if input[0] == "isa.investigation.xlsx":
             pattern_matching_result = 0
 
         else: 
             pattern_matching_result = 1
 
 
@@ -31,32 +31,32 @@
 
     elif pattern_matching_result == 1:
         return None
 
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_ToCreateContract_6FCE9E49(this: ArcInvestigation, is_light: bool | None=None) -> Contract:
-    def _arrow1786(investigation: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
+    def _arrow1720(investigation: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
         return to_light_fs_workbook(investigation)
 
-    def _arrow1787(investigation_1: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
+    def _arrow1722(investigation_1: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
         return to_fs_workbook(investigation_1)
 
-    converter: Callable[[ArcInvestigation], FsWorkbook] = _arrow1786 if default_arg(is_light, True) else _arrow1787
+    converter: Callable[[ArcInvestigation], FsWorkbook] = _arrow1720 if default_arg(is_light, True) else _arrow1722
     return Contract.create_create("isa.investigation.xlsx", DTOType(2), DTO(0, converter(this)))
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_ToUpdateContract_6FCE9E49(this: ArcInvestigation, is_light: bool | None=None) -> Contract:
-    def _arrow1788(investigation: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
+    def _arrow1727(investigation: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
         return to_light_fs_workbook(investigation)
 
-    def _arrow1789(investigation_1: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
+    def _arrow1728(investigation_1: ArcInvestigation, this: Any=this, is_light: Any=is_light) -> FsWorkbook:
         return to_fs_workbook(investigation_1)
 
-    converter: Callable[[ArcInvestigation], FsWorkbook] = _arrow1788 if default_arg(is_light, True) else _arrow1789
+    converter: Callable[[ArcInvestigation], FsWorkbook] = _arrow1727 if default_arg(is_light, True) else _arrow1728
     return Contract.create_update("isa.investigation.xlsx", DTOType(2), DTO(0, converter(this)))
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_toCreateContract_Static_23B73268(inv: ArcInvestigation, is_light: bool | None=None) -> Contract:
     return ARCtrl_ArcInvestigation__ArcInvestigation_ToCreateContract_6FCE9E49(inv, is_light)
```

### Comparing `arctrl-2.0.0a2/arctrl/Contract/arc_study.py` & `arctrl-2.0.0a3/arctrl/Contract/arc_study.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from ..FileSystem.file_system_tree import FileSystemTree
 from ..FileSystem.path import (combine_many, get_study_folder_path)
 from ..Spreadsheet.arc_study import (ARCtrl_ArcStudy__ArcStudy_toFsWorkbook_Static_353D0DB7, ARCtrl_ArcStudy__ArcStudy_fromFsWorkbook_Static_32154C9D)
 from .contract import (Contract, DTOType, DTO)
 
 def _007CStudyPath_007C__007C(input: Array[str]) -> str | None:
     (pattern_matching_result,) = (None,)
-    def _arrow1732(x: str, y: str, input: Any=input) -> bool:
+    def _arrow1684(x: str, y: str, input: Any=input) -> bool:
         return x == y
 
-    if (len(input) == 3) if (not equals_with(_arrow1732, input, None)) else False:
+    if (len(input) == 3) if (not equals_with(_arrow1684, input, None)) else False:
         if input[0] == "studies":
             if input[2] == "isa.study.xlsx":
                 pattern_matching_result = 0
 
             else: 
                 pattern_matching_result = 1
 
@@ -43,28 +43,28 @@
 
 
 
 def ARCtrl_ArcStudy__ArcStudy_ToCreateContract_6FCE9E49(this: ArcStudy, WithFolder: bool | None=None) -> Array[Contract]:
     with_folder: bool = default_arg(WithFolder, False)
     path: str = Study_fileNameFromIdentifier(this.Identifier)
     c: Contract = Contract.create_create(path, DTOType(1), DTO(0, ARCtrl_ArcStudy__ArcStudy_toFsWorkbook_Static_353D0DB7(this)))
-    def _arrow1744(__unit: None=None, this: Any=this, WithFolder: Any=WithFolder) -> IEnumerable_1[Contract]:
-        def _arrow1742(__unit: None=None) -> IEnumerable_1[Contract]:
+    def _arrow1688(__unit: None=None, this: Any=this, WithFolder: Any=WithFolder) -> IEnumerable_1[Contract]:
+        def _arrow1686(__unit: None=None) -> IEnumerable_1[Contract]:
             folder_fs: FileSystemTree = FileSystemTree.create_studies_folder([FileSystemTree.create_study_folder(this.Identifier)])
-            def _arrow1741(p: str) -> IEnumerable_1[Contract]:
+            def _arrow1685(p: str) -> IEnumerable_1[Contract]:
                 return singleton(Contract.create_create(p, DTOType(6))) if (p != path) else empty()
 
-            return collect(_arrow1741, folder_fs.ToFilePaths(False))
+            return collect(_arrow1685, folder_fs.ToFilePaths(False))
 
-        def _arrow1743(__unit: None=None) -> IEnumerable_1[Contract]:
+        def _arrow1687(__unit: None=None) -> IEnumerable_1[Contract]:
             return singleton(c)
 
-        return append(_arrow1742() if with_folder else empty(), delay(_arrow1743))
+        return append(_arrow1686() if with_folder else empty(), delay(_arrow1687))
 
-    return to_array(delay(_arrow1744))
+    return to_array(delay(_arrow1688))
 
 
 def ARCtrl_ArcStudy__ArcStudy_ToUpdateContract(this: ArcStudy) -> Contract:
     path: str = Study_fileNameFromIdentifier(this.Identifier)
     return Contract.create_update(path, DTOType(1), DTO(0, ARCtrl_ArcStudy__ArcStudy_toFsWorkbook_Static_353D0DB7(this)))
```

### Comparing `arctrl-2.0.0a2/arctrl/Contract/contract.py` & `arctrl-2.0.0a3/arctrl/Contract/contract.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Contract/git.py` & `arctrl-2.0.0a3/arctrl/Contract/git.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/arc_types.py` & `arctrl-2.0.0a3/arctrl/Core/arc_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1679,15 +1679,15 @@
 
 ArcStudy_reflection = _expr644
 
 def ArcStudy__ctor_Z187CCF3B(identifier: str, title: str | None=None, description: str | None=None, submission_date: str | None=None, public_release_date: str | None=None, publications: Array[Publication] | None=None, contacts: Array[Person] | None=None, study_design_descriptors: Array[OntologyAnnotation] | None=None, tables: Array[ArcTable] | None=None, registered_assay_identifiers: Array[str] | None=None, comments: Array[Comment] | None=None) -> ArcStudy:
     return ArcStudy(identifier, title, description, submission_date, public_release_date, publications, contacts, study_design_descriptors, tables, registered_assay_identifiers, comments)
 
 
-def _expr736() -> TypeInfo:
+def _expr723() -> TypeInfo:
     return class_type("ARCtrl.ArcInvestigation", None, ArcInvestigation)
 
 
 class ArcInvestigation:
     def __init__(self, identifier: str, title: str | None=None, description: str | None=None, submission_date: str | None=None, public_release_date: str | None=None, ontology_source_references: Array[OntologySourceReference] | None=None, publications: Array[Publication] | None=None, contacts: Array[Person] | None=None, assays: Array[ArcAssay] | None=None, studies: Array[ArcStudy] | None=None, registered_study_identifiers: Array[str] | None=None, comments: Array[Comment] | None=None, remarks: Array[Remark] | None=None) -> None:
         this: FSharpRef[ArcInvestigation] = FSharpRef(None)
         this.contents = self
@@ -2078,88 +2078,88 @@
             new_investigation.SetAssay(assay_identifier, assay)
             return new_investigation
 
         return _arrow653
 
     def GetAssayIndex(self, assay_identifier: str) -> int:
         this: ArcInvestigation = self
-        def _arrow655(a: ArcAssay) -> bool:
+        def _arrow654(a: ArcAssay) -> bool:
             return a.Identifier == assay_identifier
 
-        index: int = find_index(_arrow655, this.Assays) or 0
+        index: int = find_index(_arrow654, this.Assays) or 0
         if index == -1:
             raise Exception(("Unable to find assay with specified identifier \'" + assay_identifier) + "\'!")
 
         return index
 
     @staticmethod
     def get_assay_index(assay_identifier: str) -> Callable[[ArcInvestigation], int]:
-        def _arrow656(inv: ArcInvestigation) -> int:
+        def _arrow655(inv: ArcInvestigation) -> int:
             return inv.GetAssayIndex(assay_identifier)
 
-        return _arrow656
+        return _arrow655
 
     def GetAssayAt(self, index: int) -> ArcAssay:
         this: ArcInvestigation = self
         return this.Assays[index]
 
     @staticmethod
     def get_assay_at(index: int) -> Callable[[ArcInvestigation], ArcAssay]:
-        def _arrow657(inv: ArcInvestigation) -> ArcAssay:
+        def _arrow656(inv: ArcInvestigation) -> ArcAssay:
             new_investigation: ArcInvestigation = inv.Copy()
             return new_investigation.GetAssayAt(index)
 
-        return _arrow657
+        return _arrow656
 
     def GetAssay(self, assay_identifier: str) -> ArcAssay:
         this: ArcInvestigation = self
         match_value: ArcAssay | None = this.TryGetAssay(assay_identifier)
         if match_value is None:
             raise Exception(ArcTypesAux_ErrorMsgs_unableToFindAssayIdentifier(assay_identifier, this.Identifier))
 
         else: 
             return match_value
 
 
     @staticmethod
     def get_assay(assay_identifier: str) -> Callable[[ArcInvestigation], ArcAssay]:
-        def _arrow660(inv: ArcInvestigation) -> ArcAssay:
+        def _arrow657(inv: ArcInvestigation) -> ArcAssay:
             new_investigation: ArcInvestigation = inv.Copy()
             return new_investigation.GetAssay(assay_identifier)
 
-        return _arrow660
+        return _arrow657
 
     def TryGetAssay(self, assay_identifier: str) -> ArcAssay | None:
         this: ArcInvestigation = self
-        def _arrow661(a: ArcAssay) -> bool:
+        def _arrow658(a: ArcAssay) -> bool:
             return a.Identifier == assay_identifier
 
-        return try_find(_arrow661, this.Assays)
+        return try_find(_arrow658, this.Assays)
 
     @staticmethod
     def try_get_assay(assay_identifier: str) -> Callable[[ArcInvestigation], ArcAssay | None]:
-        def _arrow665(inv: ArcInvestigation) -> ArcAssay | None:
+        def _arrow659(inv: ArcInvestigation) -> ArcAssay | None:
             new_investigation: ArcInvestigation = inv.Copy()
             return new_investigation.TryGetAssay(assay_identifier)
 
-        return _arrow665
+        return _arrow659
 
     def ContainsAssay(self, assay_identifier: str) -> bool:
         this: ArcInvestigation = self
         def predicate(a: ArcAssay) -> bool:
             return a.Identifier == assay_identifier
 
         return exists(predicate, this.Assays)
 
     @staticmethod
     def contains_assay(assay_identifier: str) -> Callable[[ArcInvestigation], bool]:
-        def _arrow666(inv: ArcInvestigation) -> bool:
+        def _arrow660(inv: ArcInvestigation) -> bool:
             return inv.ContainsAssay(assay_identifier)
 
-        return _arrow666
+        return _arrow660
 
     @property
     def RegisteredStudyIdentifierCount(self, __unit: None=None) -> int:
         this: ArcInvestigation = self
         return len(this.RegisteredStudyIdentifiers)
 
     @property
@@ -2196,26 +2196,26 @@
 
         return to_array(map(mapping, this.Studies))
 
     @property
     def UnregisteredStudies(self, __unit: None=None) -> Array[ArcStudy]:
         this: ArcInvestigation = self
         def f(s: ArcStudy) -> bool:
-            def _arrow670(__unit: None=None, s: Any=s) -> bool:
+            def _arrow663(__unit: None=None, s: Any=s) -> bool:
                 source: Array[str] = this.RegisteredStudyIdentifiers
-                def _arrow669(__unit: None=None) -> Callable[[str], bool]:
+                def _arrow662(__unit: None=None) -> Callable[[str], bool]:
                     x: str = s.Identifier
-                    def _arrow668(y: str) -> bool:
+                    def _arrow661(y: str) -> bool:
                         return x == y
 
-                    return _arrow668
+                    return _arrow661
 
-                return exists(_arrow669(), source)
+                return exists(_arrow662(), source)
 
-            return not _arrow670()
+            return not _arrow663()
 
         return ResizeArray_filter(f, this.Studies)
 
     def AddStudy(self, study: ArcStudy) -> None:
         this: ArcInvestigation = self
         study_1: ArcStudy = study
         def predicate(x: ArcStudy) -> bool:
@@ -2229,34 +2229,34 @@
             raise Exception(((("Cannot create study with name " + study_1.Identifier) + ", as study names must be unique and study at index ") + str(match_value)) + " has the same name.")
 
         study.Investigation = this
         (this.Studies.append(study))
 
     @staticmethod
     def add_study(study: ArcStudy) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow673(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow664(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.AddStudy(study)
             return copy
 
-        return _arrow673
+        return _arrow664
 
     def InitStudy(self, study_identifier: str) -> ArcStudy:
         this: ArcInvestigation = self
         study: ArcStudy = ArcStudy.init(study_identifier)
         this.AddStudy(study)
         return study
 
     @staticmethod
     def init_study(study_identifier: str) -> Callable[[ArcInvestigation], tuple[ArcInvestigation, ArcStudy]]:
-        def _arrow674(inv: ArcInvestigation) -> tuple[ArcInvestigation, ArcStudy]:
+        def _arrow665(inv: ArcInvestigation) -> tuple[ArcInvestigation, ArcStudy]:
             copy: ArcInvestigation = inv.Copy()
             return (copy, copy.InitStudy(study_identifier))
 
-        return _arrow674
+        return _arrow665
 
     def RegisterStudy(self, study_identifier: str) -> None:
         this: ArcInvestigation = self
         study_ident: str = study_identifier
         def predicate(x: str) -> bool:
             return x == study_ident
 
@@ -2264,113 +2264,113 @@
         if match_value is not None:
             pass
 
         else: 
             raise Exception(("The given study with identifier \'" + study_ident) + "\' must be added to Investigation before it can be registered.")
 
         study_ident_1: str = study_identifier
-        class ObjectExpr676:
+        class ObjectExpr667:
             @property
             def Equals(self) -> Callable[[str, str], bool]:
-                def _arrow675(x_1: str, y: str) -> bool:
+                def _arrow666(x_1: str, y: str) -> bool:
                     return x_1 == y
 
-                return _arrow675
+                return _arrow666
 
             @property
             def GetHashCode(self) -> Callable[[str], int]:
                 return string_hash
 
-        if contains(study_ident_1, this.RegisteredStudyIdentifiers, ObjectExpr676()):
+        if contains(study_ident_1, this.RegisteredStudyIdentifiers, ObjectExpr667()):
             raise Exception(("Study with identifier \'" + study_ident_1) + "\' is already registered!")
 
         (this.RegisteredStudyIdentifiers.append(study_identifier))
 
     @staticmethod
     def register_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow677(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow668(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.RegisterStudy(study_identifier)
             return copy
 
-        return _arrow677
+        return _arrow668
 
     def AddRegisteredStudy(self, study: ArcStudy) -> None:
         this: ArcInvestigation = self
         this.AddStudy(study)
         this.RegisterStudy(study.Identifier)
 
     @staticmethod
     def add_registered_study(study: ArcStudy) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow678(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow669(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             study_1: ArcStudy = study.Copy()
             copy.AddRegisteredStudy(study_1)
             return copy
 
-        return _arrow678
+        return _arrow669
 
     def DeleteStudyAt(self, index: int) -> None:
         this: ArcInvestigation = self
         this.Studies.pop(index)
 
     @staticmethod
     def delete_study_at(index: int) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow679(i: ArcInvestigation) -> ArcInvestigation:
+        def _arrow670(i: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = i.Copy()
             copy.DeleteStudyAt(index)
             return copy
 
-        return _arrow679
+        return _arrow670
 
     def DeleteStudy(self, study_identifier: str) -> None:
         this: ArcInvestigation = self
-        def _arrow680(s: ArcStudy) -> bool:
+        def _arrow671(s: ArcStudy) -> bool:
             return s.Identifier == study_identifier
 
-        index: int = find_index(_arrow680, this.Studies) or 0
+        index: int = find_index(_arrow671, this.Studies) or 0
         this.DeleteStudyAt(index)
 
     @staticmethod
     def delete_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow681(i: ArcInvestigation) -> ArcInvestigation:
+        def _arrow672(i: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = i.Copy()
             copy.DeleteStudy(study_identifier)
             return copy
 
-        return _arrow681
+        return _arrow672
 
     def RemoveStudyAt(self, index: int) -> None:
         this: ArcInvestigation = self
         ident: str = this.GetStudyAt(index).Identifier
         this.Studies.pop(index)
         this.DeregisterStudy(ident)
 
     @staticmethod
     def remove_study_at(index: int) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow682(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow673(inv: ArcInvestigation) -> ArcInvestigation:
             new_inv: ArcInvestigation = inv.Copy()
             new_inv.RemoveStudyAt(index)
             return new_inv
 
-        return _arrow682
+        return _arrow673
 
     def RemoveStudy(self, study_identifier: str) -> None:
         this: ArcInvestigation = self
         index: int = this.GetStudyIndex(study_identifier) or 0
         this.RemoveStudyAt(index)
 
     @staticmethod
     def remove_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow683(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow674(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.RemoveStudy(study_identifier)
             return copy
 
-        return _arrow683
+        return _arrow674
 
     def SetStudyAt(self, index: int, study: ArcStudy) -> None:
         this: ArcInvestigation = self
         study_1: ArcStudy = study
         def predicate(x: ArcStudy) -> bool:
             return x.Identifier == study_1.Identifier
 
@@ -2382,111 +2382,111 @@
             raise Exception(((("Cannot create study with name " + study_1.Identifier) + ", as study names must be unique and study at index ") + str(match_value)) + " has the same name.")
 
         study.Investigation = this
         this.Studies[index] = study
 
     @staticmethod
     def set_study_at(index: int, study: ArcStudy) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow684(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow675(inv: ArcInvestigation) -> ArcInvestigation:
             new_inv: ArcInvestigation = inv.Copy()
             new_inv.SetStudyAt(index, study)
             return new_inv
 
-        return _arrow684
+        return _arrow675
 
     def SetStudy(self, study_identifier: str, study: ArcStudy) -> None:
         this: ArcInvestigation = self
         index: int = this.GetStudyIndex(study_identifier) or 0
         this.SetStudyAt(index, study)
 
     @staticmethod
     def set_study(study_identifier: str, study: ArcStudy) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow685(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow676(inv: ArcInvestigation) -> ArcInvestigation:
             new_inv: ArcInvestigation = inv.Copy()
             new_inv.SetStudy(study_identifier, study)
             return new_inv
 
-        return _arrow685
+        return _arrow676
 
     def GetStudyIndex(self, study_identifier: str) -> int:
         this: ArcInvestigation = self
-        def _arrow686(s: ArcStudy) -> bool:
+        def _arrow677(s: ArcStudy) -> bool:
             return s.Identifier == study_identifier
 
-        index: int = find_index(_arrow686, this.Studies) or 0
+        index: int = find_index(_arrow677, this.Studies) or 0
         if index == -1:
             raise Exception(("Unable to find study with specified identifier \'" + study_identifier) + "\'!")
 
         return index
 
     @staticmethod
     def get_study_index(study_identifier: str) -> Callable[[ArcInvestigation], int]:
-        def _arrow687(inv: ArcInvestigation) -> int:
+        def _arrow678(inv: ArcInvestigation) -> int:
             return inv.GetStudyIndex(study_identifier)
 
-        return _arrow687
+        return _arrow678
 
     def GetStudyAt(self, index: int) -> ArcStudy:
         this: ArcInvestigation = self
         return this.Studies[index]
 
     @staticmethod
     def get_study_at(index: int) -> Callable[[ArcInvestigation], ArcStudy]:
-        def _arrow688(inv: ArcInvestigation) -> ArcStudy:
+        def _arrow679(inv: ArcInvestigation) -> ArcStudy:
             new_inv: ArcInvestigation = inv.Copy()
             return new_inv.GetStudyAt(index)
 
-        return _arrow688
+        return _arrow679
 
     def GetStudy(self, study_identifier: str) -> ArcStudy:
         this: ArcInvestigation = self
         match_value: ArcStudy | None = this.TryGetStudy(study_identifier)
         if match_value is None:
             raise Exception(ArcTypesAux_ErrorMsgs_unableToFindStudyIdentifier(study_identifier, this.Identifier))
 
         else: 
             return match_value
 
 
     @staticmethod
     def get_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcStudy]:
-        def _arrow689(inv: ArcInvestigation) -> ArcStudy:
+        def _arrow680(inv: ArcInvestigation) -> ArcStudy:
             new_inv: ArcInvestigation = inv.Copy()
             return new_inv.GetStudy(study_identifier)
 
-        return _arrow689
+        return _arrow680
 
     def TryGetStudy(self, study_identifier: str) -> ArcStudy | None:
         this: ArcInvestigation = self
         def predicate(s: ArcStudy) -> bool:
             return s.Identifier == study_identifier
 
         return try_find(predicate, this.Studies)
 
     @staticmethod
     def try_get_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcStudy | None]:
-        def _arrow690(inv: ArcInvestigation) -> ArcStudy | None:
+        def _arrow681(inv: ArcInvestigation) -> ArcStudy | None:
             new_inv: ArcInvestigation = inv.Copy()
             return new_inv.TryGetStudy(study_identifier)
 
-        return _arrow690
+        return _arrow681
 
     def ContainsStudy(self, study_identifier: str) -> bool:
         this: ArcInvestigation = self
         def predicate(s: ArcStudy) -> bool:
             return s.Identifier == study_identifier
 
         return exists(predicate, this.Studies)
 
     @staticmethod
     def contains_study(study_identifier: str) -> Callable[[ArcInvestigation], bool]:
-        def _arrow691(inv: ArcInvestigation) -> bool:
+        def _arrow682(inv: ArcInvestigation) -> bool:
             return inv.ContainsStudy(study_identifier)
 
-        return _arrow691
+        return _arrow682
 
     def RegisterAssayAt(self, study_index: int, assay_identifier: str) -> None:
         this: ArcInvestigation = self
         study: ArcStudy = this.GetStudyAt(study_index)
         def predicate(x: str) -> bool:
             return x == assay_identifier
 
@@ -2511,87 +2511,87 @@
         else: 
             raise Exception(((("Cannot create assay with name " + assay_ident_1) + ", as assay names must be unique and assay at index ") + str(match_value_1)) + " has the same name.")
 
         study.RegisterAssay(assay_identifier)
 
     @staticmethod
     def register_assay_at(study_index: int, assay_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow692(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow683(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.RegisterAssayAt(study_index, assay_identifier)
             return copy
 
-        return _arrow692
+        return _arrow683
 
     def RegisterAssay(self, study_identifier: str, assay_identifier: str) -> None:
         this: ArcInvestigation = self
         index: int = this.GetStudyIndex(study_identifier) or 0
         this.RegisterAssayAt(index, assay_identifier)
 
     @staticmethod
     def register_assay(study_identifier: str, assay_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow693(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow684(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.RegisterAssay(study_identifier, assay_identifier)
             return copy
 
-        return _arrow693
+        return _arrow684
 
     def DeregisterAssayAt(self, study_index: int, assay_identifier: str) -> None:
         this: ArcInvestigation = self
         study: ArcStudy = this.GetStudyAt(study_index)
         study.DeregisterAssay(assay_identifier)
 
     @staticmethod
     def deregister_assay_at(study_index: int, assay_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow694(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow685(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.DeregisterAssayAt(study_index, assay_identifier)
             return copy
 
-        return _arrow694
+        return _arrow685
 
     def DeregisterAssay(self, study_identifier: str, assay_identifier: str) -> None:
         this: ArcInvestigation = self
         index: int = this.GetStudyIndex(study_identifier) or 0
         this.DeregisterAssayAt(index, assay_identifier)
 
     @staticmethod
     def deregister_assay(study_identifier: str, assay_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow695(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow686(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.DeregisterAssay(study_identifier, assay_identifier)
             return copy
 
-        return _arrow695
+        return _arrow686
 
     def DeregisterStudy(self, study_identifier: str) -> None:
         this: ArcInvestigation = self
-        class ObjectExpr697:
+        class ObjectExpr688:
             @property
             def Equals(self) -> Callable[[str, str], bool]:
-                def _arrow696(x: str, y: str) -> bool:
+                def _arrow687(x: str, y: str) -> bool:
                     return x == y
 
-                return _arrow696
+                return _arrow687
 
             @property
             def GetHashCode(self) -> Callable[[str], int]:
                 return string_hash
 
-        ignore(remove_in_place(study_identifier, this.RegisteredStudyIdentifiers, ObjectExpr697()))
+        ignore(remove_in_place(study_identifier, this.RegisteredStudyIdentifiers, ObjectExpr688()))
 
     @staticmethod
     def deregister_study(study_identifier: str) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow698(i: ArcInvestigation) -> ArcInvestigation:
+        def _arrow689(i: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = i.Copy()
             copy.DeregisterStudy(study_identifier)
             return copy
 
-        return _arrow698
+        return _arrow689
 
     def GetAllPersons(self, __unit: None=None) -> Array[Person]:
         this: ArcInvestigation = self
         persons: Array[Person] = []
         enumerator: Any = get_enumerator(this.Assays)
         try: 
             while enumerator.System_Collections_IEnumerator_MoveNext():
@@ -2607,110 +2607,110 @@
                 s: ArcStudy = enumerator_1.System_Collections_Generic_IEnumerator_1_get_Current()
                 add_range_in_place(s.Contacts, persons)
 
         finally: 
             dispose(enumerator_1)
 
         add_range_in_place(this.Contacts, persons)
-        class ObjectExpr699:
+        class ObjectExpr690:
             @property
             def Equals(self) -> Callable[[Person, Person], bool]:
                 return equals
 
             @property
             def GetHashCode(self) -> Callable[[Person], int]:
                 return safe_hash
 
-        return Array_distinct(list(persons), ObjectExpr699())
+        return Array_distinct(list(persons), ObjectExpr690())
 
     def GetAllPublications(self, __unit: None=None) -> Array[Publication]:
         this: ArcInvestigation = self
         pubs: Array[Publication] = []
         enumerator: Any = get_enumerator(this.Studies)
         try: 
             while enumerator.System_Collections_IEnumerator_MoveNext():
                 s: ArcStudy = enumerator.System_Collections_Generic_IEnumerator_1_get_Current()
                 add_range_in_place(s.Publications, pubs)
 
         finally: 
             dispose(enumerator)
 
         add_range_in_place(this.Publications, pubs)
-        class ObjectExpr700:
+        class ObjectExpr691:
             @property
             def Equals(self) -> Callable[[Publication, Publication], bool]:
                 return equals
 
             @property
             def GetHashCode(self) -> Callable[[Publication], int]:
                 return safe_hash
 
-        return Array_distinct(list(pubs), ObjectExpr700())
+        return Array_distinct(list(pubs), ObjectExpr691())
 
     def DeregisterMissingAssays(self, __unit: None=None) -> None:
         this: ArcInvestigation = self
         inv: ArcInvestigation = this
         existing_assays: Array[str] = inv.AssayIdentifiers
         enumerator: Any = get_enumerator(inv.Studies)
         try: 
             while enumerator.System_Collections_IEnumerator_MoveNext():
                 study: ArcStudy = enumerator.System_Collections_Generic_IEnumerator_1_get_Current()
                 enumerator_1: Any = get_enumerator(list(study.RegisteredAssayIdentifiers))
                 try: 
                     while enumerator_1.System_Collections_IEnumerator_MoveNext():
                         registered_assay: str = enumerator_1.System_Collections_Generic_IEnumerator_1_get_Current()
-                        class ObjectExpr702:
+                        class ObjectExpr693:
                             @property
                             def Equals(self) -> Callable[[str, str], bool]:
-                                def _arrow701(x: str, y: str) -> bool:
+                                def _arrow692(x: str, y: str) -> bool:
                                     return x == y
 
-                                return _arrow701
+                                return _arrow692
 
                             @property
                             def GetHashCode(self) -> Callable[[str], int]:
                                 return string_hash
 
-                        if not contains(registered_assay, existing_assays, ObjectExpr702()):
+                        if not contains(registered_assay, existing_assays, ObjectExpr693()):
                             value_1: None = study.DeregisterAssay(registered_assay)
                             ignore(None)
 
 
                 finally: 
                     dispose(enumerator_1)
 
 
         finally: 
             dispose(enumerator)
 
 
     @staticmethod
     def deregister_missing_assays(__unit: None=None) -> Callable[[ArcInvestigation], ArcInvestigation]:
-        def _arrow703(inv: ArcInvestigation) -> ArcInvestigation:
+        def _arrow694(inv: ArcInvestigation) -> ArcInvestigation:
             copy: ArcInvestigation = inv.Copy()
             copy.DeregisterMissingAssays()
             return copy
 
-        return _arrow703
+        return _arrow694
 
     def UpdateIOTypeByEntityID(self, __unit: None=None) -> None:
         this: ArcInvestigation = self
-        def _arrow707(__unit: None=None) -> IEnumerable_1[ArcTable]:
-            def _arrow704(study: ArcStudy) -> IEnumerable_1[ArcTable]:
+        def _arrow698(__unit: None=None) -> IEnumerable_1[ArcTable]:
+            def _arrow695(study: ArcStudy) -> IEnumerable_1[ArcTable]:
                 return study.Tables
 
-            def _arrow706(__unit: None=None) -> IEnumerable_1[ArcTable]:
-                def _arrow705(assay: ArcAssay) -> IEnumerable_1[ArcTable]:
+            def _arrow697(__unit: None=None) -> IEnumerable_1[ArcTable]:
+                def _arrow696(assay: ArcAssay) -> IEnumerable_1[ArcTable]:
                     return assay.Tables
 
-                return collect(_arrow705, this.Assays)
+                return collect(_arrow696, this.Assays)
 
-            return append_3(collect(_arrow704, this.Studies), delay(_arrow706))
+            return append_3(collect(_arrow695, this.Studies), delay(_arrow697))
 
-        io_map: Any = ArcTablesAux_getIOMap(list(to_list(delay(_arrow707))))
+        io_map: Any = ArcTablesAux_getIOMap(list(to_list(delay(_arrow698))))
         enumerator: Any = get_enumerator(this.Studies)
         try: 
             while enumerator.System_Collections_IEnumerator_MoveNext():
                 study_1: ArcStudy = enumerator.System_Collections_Generic_IEnumerator_1_get_Current()
                 ArcTablesAux_applyIOMap(io_map, study_1.Tables)
 
         finally: 
@@ -2774,167 +2774,167 @@
         return ArcInvestigation(this.Identifier, this.Title, this.Description, this.SubmissionDate, this.PublicReleaseDate, next_ontology_source_references, next_publications, next_contacts, next_assays, next_studies, next_study_identifiers, next_comments, next_remarks)
 
     def StructurallyEquals(self, other: ArcInvestigation) -> bool:
         this: ArcInvestigation = self
         def predicate(x: bool) -> bool:
             return x == True
 
-        def _arrow710(__unit: None=None) -> bool:
+        def _arrow701(__unit: None=None) -> bool:
             a: IEnumerable_1[Publication] = this.Publications
             b: IEnumerable_1[Publication] = other.Publications
             def folder(acc: bool, e: bool) -> bool:
                 if acc:
                     return e
 
                 else: 
                     return False
 
 
-            def _arrow709(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow708(i_1: int) -> bool:
+            def _arrow700(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow699(i_1: int) -> bool:
                     return equals(item(i_1, a), item(i_1, b))
 
-                return map(_arrow708, range_big_int(0, 1, length(a) - 1))
+                return map(_arrow699, range_big_int(0, 1, length(a) - 1))
 
-            return fold(folder, True, to_list(delay(_arrow709))) if (length(a) == length(b)) else False
+            return fold(folder, True, to_list(delay(_arrow700))) if (length(a) == length(b)) else False
 
-        def _arrow713(__unit: None=None) -> bool:
+        def _arrow704(__unit: None=None) -> bool:
             a_1: IEnumerable_1[Person] = this.Contacts
             b_1: IEnumerable_1[Person] = other.Contacts
             def folder_1(acc_1: bool, e_1: bool) -> bool:
                 if acc_1:
                     return e_1
 
                 else: 
                     return False
 
 
-            def _arrow712(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow711(i_2: int) -> bool:
+            def _arrow703(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow702(i_2: int) -> bool:
                     return equals(item(i_2, a_1), item(i_2, b_1))
 
-                return map(_arrow711, range_big_int(0, 1, length(a_1) - 1))
+                return map(_arrow702, range_big_int(0, 1, length(a_1) - 1))
 
-            return fold(folder_1, True, to_list(delay(_arrow712))) if (length(a_1) == length(b_1)) else False
+            return fold(folder_1, True, to_list(delay(_arrow703))) if (length(a_1) == length(b_1)) else False
 
-        def _arrow716(__unit: None=None) -> bool:
+        def _arrow707(__unit: None=None) -> bool:
             a_2: IEnumerable_1[OntologySourceReference] = this.OntologySourceReferences
             b_2: IEnumerable_1[OntologySourceReference] = other.OntologySourceReferences
             def folder_2(acc_2: bool, e_2: bool) -> bool:
                 if acc_2:
                     return e_2
 
                 else: 
                     return False
 
 
-            def _arrow715(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow714(i_3: int) -> bool:
+            def _arrow706(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow705(i_3: int) -> bool:
                     return equals(item(i_3, a_2), item(i_3, b_2))
 
-                return map(_arrow714, range_big_int(0, 1, length(a_2) - 1))
+                return map(_arrow705, range_big_int(0, 1, length(a_2) - 1))
 
-            return fold(folder_2, True, to_list(delay(_arrow715))) if (length(a_2) == length(b_2)) else False
+            return fold(folder_2, True, to_list(delay(_arrow706))) if (length(a_2) == length(b_2)) else False
 
-        def _arrow719(__unit: None=None) -> bool:
+        def _arrow710(__unit: None=None) -> bool:
             a_3: IEnumerable_1[ArcAssay] = this.Assays
             b_3: IEnumerable_1[ArcAssay] = other.Assays
             def folder_3(acc_3: bool, e_3: bool) -> bool:
                 if acc_3:
                     return e_3
 
                 else: 
                     return False
 
 
-            def _arrow718(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow717(i_4: int) -> bool:
+            def _arrow709(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow708(i_4: int) -> bool:
                     return equals(item(i_4, a_3), item(i_4, b_3))
 
-                return map(_arrow717, range_big_int(0, 1, length(a_3) - 1))
+                return map(_arrow708, range_big_int(0, 1, length(a_3) - 1))
 
-            return fold(folder_3, True, to_list(delay(_arrow718))) if (length(a_3) == length(b_3)) else False
+            return fold(folder_3, True, to_list(delay(_arrow709))) if (length(a_3) == length(b_3)) else False
 
-        def _arrow722(__unit: None=None) -> bool:
+        def _arrow713(__unit: None=None) -> bool:
             a_4: IEnumerable_1[ArcStudy] = this.Studies
             b_4: IEnumerable_1[ArcStudy] = other.Studies
             def folder_4(acc_4: bool, e_4: bool) -> bool:
                 if acc_4:
                     return e_4
 
                 else: 
                     return False
 
 
-            def _arrow721(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow720(i_5: int) -> bool:
+            def _arrow712(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow711(i_5: int) -> bool:
                     return equals(item(i_5, a_4), item(i_5, b_4))
 
-                return map(_arrow720, range_big_int(0, 1, length(a_4) - 1))
+                return map(_arrow711, range_big_int(0, 1, length(a_4) - 1))
 
-            return fold(folder_4, True, to_list(delay(_arrow721))) if (length(a_4) == length(b_4)) else False
+            return fold(folder_4, True, to_list(delay(_arrow712))) if (length(a_4) == length(b_4)) else False
 
-        def _arrow725(__unit: None=None) -> bool:
+        def _arrow716(__unit: None=None) -> bool:
             a_5: IEnumerable_1[str] = this.RegisteredStudyIdentifiers
             b_5: IEnumerable_1[str] = other.RegisteredStudyIdentifiers
             def folder_5(acc_5: bool, e_5: bool) -> bool:
                 if acc_5:
                     return e_5
 
                 else: 
                     return False
 
 
-            def _arrow724(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow723(i_6: int) -> bool:
+            def _arrow715(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow714(i_6: int) -> bool:
                     return item(i_6, a_5) == item(i_6, b_5)
 
-                return map(_arrow723, range_big_int(0, 1, length(a_5) - 1))
+                return map(_arrow714, range_big_int(0, 1, length(a_5) - 1))
 
-            return fold(folder_5, True, to_list(delay(_arrow724))) if (length(a_5) == length(b_5)) else False
+            return fold(folder_5, True, to_list(delay(_arrow715))) if (length(a_5) == length(b_5)) else False
 
-        def _arrow728(__unit: None=None) -> bool:
+        def _arrow719(__unit: None=None) -> bool:
             a_6: IEnumerable_1[Comment] = this.Comments
             b_6: IEnumerable_1[Comment] = other.Comments
             def folder_6(acc_6: bool, e_6: bool) -> bool:
                 if acc_6:
                     return e_6
 
                 else: 
                     return False
 
 
-            def _arrow727(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow726(i_7: int) -> bool:
+            def _arrow718(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow717(i_7: int) -> bool:
                     return equals(item(i_7, a_6), item(i_7, b_6))
 
-                return map(_arrow726, range_big_int(0, 1, length(a_6) - 1))
+                return map(_arrow717, range_big_int(0, 1, length(a_6) - 1))
 
-            return fold(folder_6, True, to_list(delay(_arrow727))) if (length(a_6) == length(b_6)) else False
+            return fold(folder_6, True, to_list(delay(_arrow718))) if (length(a_6) == length(b_6)) else False
 
-        def _arrow731(__unit: None=None) -> bool:
+        def _arrow722(__unit: None=None) -> bool:
             a_7: IEnumerable_1[Remark] = this.Remarks
             b_7: IEnumerable_1[Remark] = other.Remarks
             def folder_7(acc_7: bool, e_7: bool) -> bool:
                 if acc_7:
                     return e_7
 
                 else: 
                     return False
 
 
-            def _arrow730(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow729(i_8: int) -> bool:
+            def _arrow721(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow720(i_8: int) -> bool:
                     return equals(item(i_8, a_7), item(i_8, b_7))
 
-                return map(_arrow729, range_big_int(0, 1, length(a_7) - 1))
+                return map(_arrow720, range_big_int(0, 1, length(a_7) - 1))
 
-            return fold(folder_7, True, to_list(delay(_arrow730))) if (length(a_7) == length(b_7)) else False
+            return fold(folder_7, True, to_list(delay(_arrow721))) if (length(a_7) == length(b_7)) else False
 
-        return for_all(predicate, to_enumerable([this.Identifier == other.Identifier, equals(this.Title, other.Title), equals(this.Description, other.Description), equals(this.SubmissionDate, other.SubmissionDate), equals(this.PublicReleaseDate, other.PublicReleaseDate), _arrow710(), _arrow713(), _arrow716(), _arrow719(), _arrow722(), _arrow725(), _arrow728(), _arrow731()]))
+        return for_all(predicate, to_enumerable([this.Identifier == other.Identifier, equals(this.Title, other.Title), equals(this.Description, other.Description), equals(this.SubmissionDate, other.SubmissionDate), equals(this.PublicReleaseDate, other.PublicReleaseDate), _arrow701(), _arrow704(), _arrow707(), _arrow710(), _arrow713(), _arrow716(), _arrow719(), _arrow722()]))
 
     def ReferenceEquals(self, other: ArcInvestigation) -> bool:
         this: ArcInvestigation = self
         return this is other
 
     def __str__(self, __unit: None=None) -> str:
         this: ArcInvestigation = self
@@ -2947,30 +2947,30 @@
         arg_6: Array[Publication] = this.Publications
         arg_7: Array[Person] = this.Contacts
         arg_8: Array[ArcAssay] = this.Assays
         arg_9: Array[ArcStudy] = this.Studies
         arg_10: Array[str] = this.RegisteredStudyIdentifiers
         arg_11: Array[Comment] = this.Comments
         arg_12: Array[Remark] = this.Remarks
-        return to_text(printf("ArcStudy {\r\n    Identifier = %A,\r\n    Title = %A,\r\n    Description = %A,\r\n    SubmissionDate = %A,\r\n    PublicReleaseDate = %A,\r\n    OntologySourceReferences = %A,\r\n    Publications = %A,\r\n    Contacts = %A,\r\n    Assays = %A,\r\n    Studies = %A,\r\n    RegisteredStudyIdentifiers = %A,\r\n    Comments = %A,\r\n    Remarks = %A,\r\n}"))(arg)(arg_1)(arg_2)(arg_3)(arg_4)(arg_5)(arg_6)(arg_7)(arg_8)(arg_9)(arg_10)(arg_11)(arg_12)
+        return to_text(printf("ArcInvestigation {\r\n    Identifier = %A,\r\n    Title = %A,\r\n    Description = %A,\r\n    SubmissionDate = %A,\r\n    PublicReleaseDate = %A,\r\n    OntologySourceReferences = %A,\r\n    Publications = %A,\r\n    Contacts = %A,\r\n    Assays = %A,\r\n    Studies = %A,\r\n    RegisteredStudyIdentifiers = %A,\r\n    Comments = %A,\r\n    Remarks = %A,\r\n}"))(arg)(arg_1)(arg_2)(arg_3)(arg_4)(arg_5)(arg_6)(arg_7)(arg_8)(arg_9)(arg_10)(arg_11)(arg_12)
 
     def __eq__(self, other: Any=None) -> bool:
         this: ArcInvestigation = self
         return this.StructurallyEquals(other) if isinstance(other, ArcInvestigation) else False
 
     def __hash__(self, __unit: None=None) -> Any:
         this: ArcInvestigation = self
         return box_hash_array([this.Identifier, box_hash_option(this.Title), box_hash_option(this.Description), box_hash_option(this.SubmissionDate), box_hash_option(this.PublicReleaseDate), box_hash_seq(this.Publications), box_hash_seq(this.Contacts), box_hash_seq(this.OntologySourceReferences), box_hash_seq(this.Assays), box_hash_seq(this.Studies), box_hash_seq(this.RegisteredStudyIdentifiers), box_hash_seq(this.Comments), box_hash_seq(this.Remarks)])
 
     def GetLightHashCode(self, __unit: None=None) -> Any:
         this: ArcInvestigation = self
         return box_hash_array([this.Identifier, box_hash_option(this.Title), box_hash_option(this.Description), box_hash_option(this.SubmissionDate), box_hash_option(this.PublicReleaseDate), box_hash_seq(this.Publications), box_hash_seq(this.Contacts), box_hash_seq(this.OntologySourceReferences), box_hash_seq(this.Comments), box_hash_seq(this.Remarks)])
 
 
-ArcInvestigation_reflection = _expr736
+ArcInvestigation_reflection = _expr723
 
 def ArcInvestigation__ctor_Z2ED5C612(identifier: str, title: str | None=None, description: str | None=None, submission_date: str | None=None, public_release_date: str | None=None, ontology_source_references: Array[OntologySourceReference] | None=None, publications: Array[Publication] | None=None, contacts: Array[Person] | None=None, assays: Array[ArcAssay] | None=None, studies: Array[ArcStudy] | None=None, registered_study_identifiers: Array[str] | None=None, comments: Array[Comment] | None=None, remarks: Array[Remark] | None=None) -> ArcInvestigation:
     return ArcInvestigation(identifier, title, description, submission_date, public_release_date, ontology_source_references, publications, contacts, assays, studies, registered_study_identifiers, comments, remarks)
 
 
 def ArcTypesAux_ErrorMsgs_unableToFindAssayIdentifier(assay_identifier: Any, investigation_identifier: Any) -> str:
     return ((("Error. Unable to find assay with identifier \'" + str(assay_identifier)) + "\' in investigation ") + str(investigation_identifier)) + "."
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/comment.py` & `arctrl-2.0.0a3/arctrl/Core/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 Comment_reflection = _expr273
 
 def Comment__ctor_40457300(name: str | None=None, value: str | None=None) -> Comment:
     return Comment(name, value)
 
 
-def _expr275() -> TypeInfo:
+def _expr274() -> TypeInfo:
     return record_type("ARCtrl.Remark", [], Remark, lambda: [("Line", int32_type), ("Value", string_type)])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class Remark(Record):
     Line: int
     Value: str
@@ -110,11 +110,11 @@
         return (remark.Line, remark.Value)
 
     def Copy(self, __unit: None=None) -> Remark:
         this: Remark = self
         return Remark.make(this.Line, this.Value)
 
 
-Remark_reflection = _expr275
+Remark_reflection = _expr274
 
 __all__ = ["Comment_reflection", "Remark_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/comment_list.py` & `arctrl-2.0.0a3/arctrl/Core/comment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,20 +69,20 @@
         if match_value is not None:
             return (match_value, c.Value)
 
         else: 
             return None
 
 
-    class ObjectExpr274:
+    class ObjectExpr275:
         @property
         def Compare(self) -> Callable[[str, str], int]:
             return compare_primitives
 
-    return of_seq(ResizeArray_choose(f, comments), ObjectExpr274())
+    return of_seq(ResizeArray_choose(f, comments), ObjectExpr275())
 
 
 def set_1(comment: Comment, comments: Array[Comment]) -> Array[Comment]:
     if contains_key(value(comment.Name), comments):
         def f(c: Comment, comment: Any=comment, comments: Any=comments) -> Comment:
             if equals(c.Name, comment.Name):
                 return comment
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/conversion.py` & `arctrl-2.0.0a3/arctrl/Core/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 from .Table.composite_cell import CompositeCell
 from .Table.composite_header import (CompositeHeader, IOType)
 
 Person_orcidKey: str = "ORCID"
 
 Person_AssayIdentifierPrefix: str = "performer (ARC:00000168)"
 
-def _arrow755(__unit: None=None) -> Callable[[str], str]:
+def _arrow752(__unit: None=None) -> Callable[[str], str]:
     clo_1: Callable[[str], str] = to_text(printf("%s %s"))(Person_AssayIdentifierPrefix)
     return clo_1
 
 
-Person_createAssayIdentifierKey: Callable[[str], str] = _arrow755()
+Person_createAssayIdentifierKey: Callable[[str], str] = _arrow752()
 
 def Person_setSourceAssayComment(person: Person, assay_identifier: str) -> Person:
     person_1: Person = person.Copy()
     comment: Comment = Comment(Person_createAssayIdentifierKey(assay_identifier), assay_identifier)
     (person_1.Comments.append(comment))
     return person_1
 
@@ -383,171 +383,171 @@
 
 
 def ProcessParsing_tryComponentGetter(general_i: int, value_i: int, value_header: CompositeHeader) -> Callable[[Any, int], Component] | None:
     if value_header.tag == 0:
         new_oa: OntologyAnnotation = value_header.fields[0].Copy()
         ARCtrl_OntologyAnnotation__OntologyAnnotation_SetColumnIndex_Z524259A4(new_oa, value_i)
         def Value(matrix: Any, general_i: Any=general_i, value_i: Any=value_i, value_header: Any=value_header) -> Callable[[int], Component]:
-            def _arrow756(i: int, matrix: Any=matrix) -> Component:
+            def _arrow753(i: int, matrix: Any=matrix) -> Component:
                 return JsonTypes_composeComponent(CompositeHeader(0, new_oa), get_item_from_dict(matrix, (general_i, i)))
 
-            return _arrow756
+            return _arrow753
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryParameterGetter(general_i: int, value_i: int, value_header: CompositeHeader) -> Callable[[Any, int], ProcessParameterValue] | None:
     if value_header.tag == 3:
         cat: CompositeHeader = CompositeHeader(3, ARCtrl_OntologyAnnotation__OntologyAnnotation_setColumnIndex_Static(value_i, value_header.fields[0]))
         def Value(matrix: Any, general_i: Any=general_i, value_i: Any=value_i, value_header: Any=value_header) -> Callable[[int], ProcessParameterValue]:
-            def _arrow757(i_1: int, matrix: Any=matrix) -> ProcessParameterValue:
+            def _arrow754(i_1: int, matrix: Any=matrix) -> ProcessParameterValue:
                 return JsonTypes_composeParameterValue(cat, get_item_from_dict(matrix, (general_i, i_1)))
 
-            return _arrow757
+            return _arrow754
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryFactorGetter(general_i: int, value_i: int, value_header: CompositeHeader) -> Callable[[Any, int], FactorValue] | None:
     if value_header.tag == 2:
         cat: CompositeHeader = CompositeHeader(2, ARCtrl_OntologyAnnotation__OntologyAnnotation_setColumnIndex_Static(value_i, value_header.fields[0]))
         def Value(matrix: Any, general_i: Any=general_i, value_i: Any=value_i, value_header: Any=value_header) -> Callable[[int], FactorValue]:
-            def _arrow758(i_1: int, matrix: Any=matrix) -> FactorValue:
+            def _arrow755(i_1: int, matrix: Any=matrix) -> FactorValue:
                 return JsonTypes_composeFactorValue(cat, get_item_from_dict(matrix, (general_i, i_1)))
 
-            return _arrow758
+            return _arrow755
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryCharacteristicGetter(general_i: int, value_i: int, value_header: CompositeHeader) -> Callable[[Any, int], MaterialAttributeValue] | None:
     if value_header.tag == 1:
         cat: CompositeHeader = CompositeHeader(1, ARCtrl_OntologyAnnotation__OntologyAnnotation_setColumnIndex_Static(value_i, value_header.fields[0]))
         def Value(matrix: Any, general_i: Any=general_i, value_i: Any=value_i, value_header: Any=value_header) -> Callable[[int], MaterialAttributeValue]:
-            def _arrow759(i_1: int, matrix: Any=matrix) -> MaterialAttributeValue:
+            def _arrow756(i_1: int, matrix: Any=matrix) -> MaterialAttributeValue:
                 return JsonTypes_composeCharacteristicValue(cat, get_item_from_dict(matrix, (general_i, i_1)))
 
-            return _arrow759
+            return _arrow756
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetProtocolTypeGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], OntologyAnnotation] | None:
     if header.tag == 4:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], OntologyAnnotation]:
-            def _arrow760(i: int, matrix: Any=matrix) -> OntologyAnnotation:
+            def _arrow757(i: int, matrix: Any=matrix) -> OntologyAnnotation:
                 return get_item_from_dict(matrix, (general_i, i)).AsTerm
 
-            return _arrow760
+            return _arrow757
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetProtocolREFGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], str] | None:
     if header.tag == 8:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], str]:
-            def _arrow761(i: int, matrix: Any=matrix) -> str:
+            def _arrow758(i: int, matrix: Any=matrix) -> str:
                 return get_item_from_dict(matrix, (general_i, i)).AsFreeText
 
-            return _arrow761
+            return _arrow758
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetProtocolDescriptionGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], str] | None:
     if header.tag == 5:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], str]:
-            def _arrow762(i: int, matrix: Any=matrix) -> str:
+            def _arrow759(i: int, matrix: Any=matrix) -> str:
                 return get_item_from_dict(matrix, (general_i, i)).AsFreeText
 
-            return _arrow762
+            return _arrow759
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetProtocolURIGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], str] | None:
     if header.tag == 6:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], str]:
-            def _arrow763(i: int, matrix: Any=matrix) -> str:
+            def _arrow760(i: int, matrix: Any=matrix) -> str:
                 return get_item_from_dict(matrix, (general_i, i)).AsFreeText
 
-            return _arrow763
+            return _arrow760
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetProtocolVersionGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], str] | None:
     if header.tag == 7:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], str]:
-            def _arrow764(i: int, matrix: Any=matrix) -> str:
+            def _arrow761(i: int, matrix: Any=matrix) -> str:
                 return get_item_from_dict(matrix, (general_i, i)).AsFreeText
 
-            return _arrow764
+            return _arrow761
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetInputGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], ProcessInput] | None:
     if header.tag == 11:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], ProcessInput]:
-            def _arrow765(i: int, matrix: Any=matrix) -> ProcessInput:
+            def _arrow762(i: int, matrix: Any=matrix) -> ProcessInput:
                 return JsonTypes_composeProcessInput(header, get_item_from_dict(matrix, (general_i, i)))
 
-            return _arrow765
+            return _arrow762
 
         return Value
 
     else: 
         return None
 
 
 
 def ProcessParsing_tryGetOutputGetter(general_i: int, header: CompositeHeader) -> Callable[[Any, int], ProcessOutput] | None:
     if header.tag == 12:
         def Value(matrix: Any, general_i: Any=general_i, header: Any=header) -> Callable[[int], ProcessOutput]:
-            def _arrow766(i: int, matrix: Any=matrix) -> ProcessOutput:
+            def _arrow763(i: int, matrix: Any=matrix) -> ProcessOutput:
                 return JsonTypes_composeProcessOutput(header, get_item_from_dict(matrix, (general_i, i)))
 
-            return _arrow766
+            return _arrow763
 
         return Value
 
     else: 
         return None
 
 
@@ -600,74 +600,74 @@
     protocol_version_getter: Callable[[Any, int], str] | None = try_pick(chooser_8, headers_1)
     input_getter_1: Callable[[Any, int], FSharpList[ProcessInput]]
     def chooser_9(tupled_arg_9: tuple[int, CompositeHeader], process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[Any, int], ProcessInput] | None:
         return ProcessParsing_tryGetInputGetter(tupled_arg_9[0], tupled_arg_9[1])
 
     match_value: Callable[[Any, int], ProcessInput] | None = try_pick(chooser_9, headers_1)
     if match_value is None:
-        def _arrow768(matrix_1: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessInput]]:
-            def _arrow767(i_1: int) -> FSharpList[ProcessInput]:
+        def _arrow765(matrix_1: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessInput]]:
+            def _arrow764(i_1: int) -> FSharpList[ProcessInput]:
                 def mapping_1(f_1: Callable[[Any, int], MaterialAttributeValue]) -> MaterialAttributeValue:
                     return f_1(matrix_1)(i_1)
 
                 return singleton(ProcessInput(0, Source_create_Z5CA08497(None, ((("" + process_name_root) + "_Input_") + str(i_1)) + "", to_list(map_1(mapping_1, char_getters)))))
 
-            return _arrow767
+            return _arrow764
 
-        input_getter_1 = _arrow768
+        input_getter_1 = _arrow765
 
     else: 
         input_getter: Callable[[Any, int], ProcessInput] = match_value
-        def _arrow770(matrix: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessInput]]:
-            def _arrow769(i: int) -> FSharpList[ProcessInput]:
+        def _arrow767(matrix: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessInput]]:
+            def _arrow766(i: int) -> FSharpList[ProcessInput]:
                 def mapping(f: Callable[[Any, int], MaterialAttributeValue]) -> MaterialAttributeValue:
                     return f(matrix)(i)
 
                 chars: FSharpList[MaterialAttributeValue] = to_list(map_1(mapping, char_getters))
                 input: ProcessInput = input_getter(matrix)(i)
                 return of_array([input, ProcessInput_createSample_Z598187B7(ProcessInput__get_Name(input), chars)]) if ((not is_empty(chars)) if (not (True if ProcessInput__isSample(input) else ProcessInput__isSource(input))) else False) else singleton(ProcessInput_setCharacteristicValues(chars, input))
 
-            return _arrow769
+            return _arrow766
 
-        input_getter_1 = _arrow770
+        input_getter_1 = _arrow767
 
     output_getter_1: Callable[[Any, int], FSharpList[ProcessOutput]]
     def chooser_10(tupled_arg_10: tuple[int, CompositeHeader], process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[Any, int], ProcessOutput] | None:
         return ProcessParsing_tryGetOutputGetter(tupled_arg_10[0], tupled_arg_10[1])
 
     match_value_1: Callable[[Any, int], ProcessOutput] | None = try_pick(chooser_10, headers_1)
     if match_value_1 is None:
-        def _arrow772(matrix_3: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessOutput]]:
-            def _arrow771(i_3: int) -> FSharpList[ProcessOutput]:
+        def _arrow769(matrix_3: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessOutput]]:
+            def _arrow768(i_3: int) -> FSharpList[ProcessOutput]:
                 def mapping_3(f_3: Callable[[Any, int], FactorValue]) -> FactorValue:
                     return f_3(matrix_3)(i_3)
 
                 return singleton(ProcessOutput(0, Sample_create_62424AD2(None, ((("" + process_name_root) + "_Output_") + str(i_3)) + "", None, to_list(map_1(mapping_3, factor_value_getters)))))
 
-            return _arrow771
+            return _arrow768
 
-        output_getter_1 = _arrow772
+        output_getter_1 = _arrow769
 
     else: 
         output_getter: Callable[[Any, int], ProcessOutput] = match_value_1
-        def _arrow774(matrix_2: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessOutput]]:
-            def _arrow773(i_2: int) -> FSharpList[ProcessOutput]:
+        def _arrow771(matrix_2: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], FSharpList[ProcessOutput]]:
+            def _arrow770(i_2: int) -> FSharpList[ProcessOutput]:
                 def mapping_2(f_2: Callable[[Any, int], FactorValue]) -> FactorValue:
                     return f_2(matrix_2)(i_2)
 
                 factors: FSharpList[FactorValue] = to_list(map_1(mapping_2, factor_value_getters))
                 output: ProcessOutput = output_getter(matrix_2)(i_2)
                 return of_array([output, ProcessOutput_createSample_Z598187B7(ProcessOutput__get_Name(output), None, factors)]) if ((not is_empty(factors)) if (not ProcessOutput__isSample(output)) else False) else singleton(ProcessOutput_setFactorValues(factors, output))
 
-            return _arrow773
+            return _arrow770
 
-        output_getter_1 = _arrow774
+        output_getter_1 = _arrow771
 
-    def _arrow776(matrix_4: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], Process]:
-        def _arrow775(i_4: int) -> Process:
+    def _arrow774(matrix_4: Any, process_name_root: Any=process_name_root, headers: Any=headers) -> Callable[[int], Process]:
+        def _arrow773(i_4: int) -> Process:
             def mapping_4(p: str) -> str:
                 return Process_composeName(p, i_4)
 
             pn: str | None = map(mapping_4, Option_fromValueWithDefault("", process_name_root))
             def mapping_5(f_4: Callable[[Any, int], ProcessParameterValue]) -> ProcessParameterValue:
                 return f_4(matrix_4)(i_4)
 
@@ -739,17 +739,17 @@
 
             pattern_input: tuple[FSharpList[ProcessInput], FSharpList[ProcessOutput]]
             inputs: FSharpList[ProcessInput] = input_getter_1(matrix_4)(i_4)
             outputs: FSharpList[ProcessOutput] = output_getter_1(matrix_4)(i_4)
             pattern_input = ((of_array([item(0, inputs), item(0, inputs)]), outputs)) if ((length(outputs) == 2) if (length(inputs) == 1) else False) else (((inputs, of_array([item(0, outputs), item(0, outputs)]))) if ((length(outputs) == 1) if (length(inputs) == 2) else False) else ((inputs, outputs)))
             return Process_make(None, pn, protocol, paramvalues, None, None, None, None, pattern_input[0], pattern_input[1], None)
 
-        return _arrow775
+        return _arrow773
 
-    return _arrow776
+    return _arrow774
 
 
 def ProcessParsing_groupProcesses(ps: FSharpList[Process]) -> FSharpList[tuple[str, FSharpList[Process]]]:
     def projection(x: Process, ps: Any=ps) -> str:
         if (Process_decomposeName_Z721C83C5(value_9(x.Name))[1] is not None) if (x.Name is not None) else False:
             return Process_decomposeName_Z721C83C5(value_9(x.Name))[0]
 
@@ -766,27 +766,27 @@
         elif (value_9(x.ExecutesProtocol).ID is not None) if (x.ExecutesProtocol is not None) else False:
             return value_9(value_9(x.ExecutesProtocol).ID)
 
         else: 
             return create_missing_identifier()
 
 
-    class ObjectExpr778:
+    class ObjectExpr776:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow777(x_1: str, y: str) -> bool:
+            def _arrow775(x_1: str, y: str) -> bool:
                 return x_1 == y
 
-            return _arrow777
+            return _arrow775
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return List_groupBy(projection, ps, ObjectExpr778())
+    return List_groupBy(projection, ps, ObjectExpr776())
 
 
 def ProcessParsing_mergeIdenticalProcesses(processes: FSharpList[Process]) -> FSharpList[Process]:
     def projection(x: Process, processes: Any=processes) -> tuple[str, Any, Any | None]:
         if (Process_decomposeName_Z721C83C5(value_9(x.Name))[1] is not None) if (x.Name is not None) else False:
             def mapping(a: FSharpList[ProcessParameterValue], x: Any=x) -> Any:
                 return box_hash_seq(a)
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Helper/collections_.py` & `arctrl-2.0.0a3/arctrl/Core/Helper/collections_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Helper/hash_codes.py` & `arctrl-2.0.0a3/arctrl/Core/Helper/hash_codes.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Helper/identifier.py` & `arctrl-2.0.0a3/arctrl/Core/Helper/identifier.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Helper/regex.py` & `arctrl-2.0.0a3/arctrl/Core/Helper/regex.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Helper/sem_ver.py` & `arctrl-2.0.0a3/arctrl/Core/Helper/sem_ver.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/identifier_setters.py` & `arctrl-2.0.0a3/arctrl/Core/identifier_setters.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/ontology_annotation.py` & `arctrl-2.0.0a3/arctrl/Core/ontology_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,18 +84,19 @@
         return default_arg(this.Name, "")
 
     @staticmethod
     def create_uri_annotation(term_source_ref: str, local_tan: str) -> str:
         return ((((("" + "http://purl.obolibrary.org/obo/") + "") + term_source_ref) + "_") + local_tan) + ""
 
     @staticmethod
-    def from_term_annotation(tan: str) -> OntologyAnnotation:
+    def from_term_annotation(tan: str, name: str | None=None) -> OntologyAnnotation:
+        name_1: str = default_arg(name, "")
         r: dict[str, Any] = value_4(try_parse_term_annotation(tan))
         accession: str = (r["IDSpace"] + ":") + r["LocalID"]
-        return OntologyAnnotation.create("", r["IDSpace"], accession)
+        return OntologyAnnotation.create(name_1, r["IDSpace"], accession)
 
     @property
     def TermAccessionShort(self, __unit: None=None) -> str:
         this: OntologyAnnotation = self
         match_value: dict[str, Any] | None = this.TANInfo
         if match_value is not None:
             id: dict[str, Any] = match_value
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/ontology_source_reference.py` & `arctrl-2.0.0a3/arctrl/Core/ontology_source_reference.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/person.py` & `arctrl-2.0.0a3/arctrl/Core/person.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/column_index.py` & `arctrl-2.0.0a3/arctrl/Core/Process/column_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from .material_attribute_value import MaterialAttributeValue
 from .process_parameter_value import ProcessParameterValue
 from .protocol_parameter import ProtocolParameter
 
 def try_int(str_1: str) -> int | None:
     match_value: tuple[bool, int]
     out_arg: int = 0
-    def _arrow373(__unit: None=None, str_1: Any=str_1) -> int:
+    def _arrow374(__unit: None=None, str_1: Any=str_1) -> int:
         return out_arg
 
     def _arrow375(v: int, str_1: Any=str_1) -> None:
         nonlocal out_arg
         out_arg = v or 0
 
-    match_value = (try_parse(str_1, 511, False, 32, FSharpRef(_arrow373, _arrow375)), out_arg)
+    match_value = (try_parse(str_1, 511, False, 32, FSharpRef(_arrow374, _arrow375)), out_arg)
     if match_value[0]:
         return match_value[1]
 
     else: 
         return None
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/component.py` & `arctrl-2.0.0a3/arctrl/Core/Process/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ...fable_modules.fable_library.types import (Record, Array)
 from ..comment import Comment
 from ..Helper.collections_ import Option_fromValueWithDefault
 from ..Helper.regex import ActivePatterns__007CRegex_007C__007C
 from ..ontology_annotation import (OntologyAnnotation, OntologyAnnotation_reflection)
 from .value import (Value, Value_reflection)
 
-def _expr327() -> TypeInfo:
+def _expr328() -> TypeInfo:
     return record_type("ARCtrl.Process.Component", [], Component, lambda: [("ComponentValue", option_type(Value_reflection())), ("ComponentUnit", option_type(OntologyAnnotation_reflection())), ("ComponentType", option_type(OntologyAnnotation_reflection()))])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class Component(Record):
     ComponentValue: Value | None
     ComponentUnit: OntologyAnnotation | None
@@ -34,15 +34,15 @@
         return this.ComponentValue
 
     def GetUnit(self, __unit: None=None) -> OntologyAnnotation | None:
         this: Component = self
         return this.ComponentUnit
 
 
-Component_reflection = _expr327
+Component_reflection = _expr328
 
 def Component__get_ComponentName(this: Component) -> str | None:
     def mapping(v: Value, this: Any=this) -> str:
         return Component_composeName(v, this.ComponentUnit)
 
     return map(mapping, this.ComponentValue)
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/data.py` & `arctrl-2.0.0a3/arctrl/Core/Process/data.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/data_file.py` & `arctrl-2.0.0a3/arctrl/Core/Process/data_file.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/factor.py` & `arctrl-2.0.0a3/arctrl/Core/Process/factor.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/factor_value.py` & `arctrl-2.0.0a3/arctrl/Core/Process/factor_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/iproperty_value.py` & `arctrl-2.0.0a3/arctrl/Core/Process/iproperty_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/material.py` & `arctrl-2.0.0a3/arctrl/Core/Process/material.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/material_attribute.py` & `arctrl-2.0.0a3/arctrl/Core/Process/material_attribute.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/material_attribute_value.py` & `arctrl-2.0.0a3/arctrl/Core/Process/material_attribute_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/material_type.py` & `arctrl-2.0.0a3/arctrl/Core/Process/material_type.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/process.py` & `arctrl-2.0.0a3/arctrl/Core/Process/process.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/process_input.py` & `arctrl-2.0.0a3/arctrl/Core/Process/process_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .factor_value import FactorValue
 from .material import (Material_reflection, Material, Material_setCharacteristicValues, Material_getUnits_ZBCDEB61, Material_create_Z66909A6D)
 from .material_attribute import MaterialAttribute
 from .material_attribute_value import MaterialAttributeValue
 from .sample import (Sample_reflection, Sample, Sample_setCharacteristicValues, Sample_getUnits_53716792, Sample_create_62424AD2)
 from .source import (Source_reflection, Source_get_empty, Source, Source_setCharacteristicValues, Source_getUnits_53E41069, Source_create_Z5CA08497)
 
-def _expr333() -> TypeInfo:
+def _expr330() -> TypeInfo:
     return union_type("ARCtrl.Process.ProcessInput", [], ProcessInput, lambda: [[("Item", Source_reflection())], [("Item", Sample_reflection())], [("Item", Data_reflection())], [("Item", Material_reflection())]])
 
 
 class ProcessInput(Union):
     def __init__(self, tag: int, *fields: Any) -> None:
         super().__init__()
         self.tag: int = tag or 0
@@ -49,15 +49,15 @@
 
         else: 
             arg: str = this.fields[0].PrintCompact()
             return to_text(printf("Sample {%s}"))(arg)
 
 
 
-ProcessInput_reflection = _expr333
+ProcessInput_reflection = _expr330
 
 def ProcessInput__get_TryName(this: ProcessInput) -> str | None:
     if this.tag == 0:
         return this.fields[0].Name
 
     elif this.tag == 3:
         return this.fields[0].Name
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/process_output.py` & `arctrl-2.0.0a3/arctrl/Core/Process/process_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .factor_value import FactorValue
 from .material import (Material_reflection, Material, Material_getUnits_ZBCDEB61, Material_create_Z66909A6D)
 from .material_attribute import MaterialAttribute
 from .material_attribute_value import MaterialAttributeValue
 from .sample import (Sample_reflection, Sample_get_empty, Sample, Sample_setFactorValues, Sample_getUnits_53716792, Sample_create_62424AD2)
 from .source import Source
 
-def _expr334() -> TypeInfo:
+def _expr329() -> TypeInfo:
     return union_type("ARCtrl.Process.ProcessOutput", [], ProcessOutput, lambda: [[("Item", Sample_reflection())], [("Item", Data_reflection())], [("Item", Material_reflection())]])
 
 
 class ProcessOutput(Union):
     def __init__(self, tag: int, *fields: Any) -> None:
         super().__init__()
         self.tag: int = tag or 0
@@ -45,15 +45,15 @@
 
         else: 
             arg: str = this.fields[0].PrintCompact()
             return to_text(printf("Sample {%s}"))(arg)
 
 
 
-ProcessOutput_reflection = _expr334
+ProcessOutput_reflection = _expr329
 
 def ProcessOutput__get_TryName(this: ProcessOutput) -> str | None:
     if this.tag == 2:
         return this.fields[0].Name
 
     elif this.tag == 1:
         return this.fields[0].Name
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/process_parameter_value.py` & `arctrl-2.0.0a3/arctrl/Core/Process/process_parameter_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/process_sequence.py` & `arctrl-2.0.0a3/arctrl/Core/Process/process_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,21 +415,21 @@
     return List_distinct(collect(mapping, process_sequence), ObjectExpr372())
 
 
 def get_materials(process_sequence: FSharpList[Process]) -> FSharpList[Material]:
     def mapping(p: Process, process_sequence: Any=process_sequence) -> FSharpList[Material]:
         return Process_getMaterials_763471FF(p)
 
-    class ObjectExpr374:
+    class ObjectExpr373:
         @property
         def Equals(self) -> Callable[[Material, Material], bool]:
             return equals
 
         @property
         def GetHashCode(self) -> Callable[[Material], int]:
             return safe_hash
 
-    return List_distinct(collect(mapping, process_sequence), ObjectExpr374())
+    return List_distinct(collect(mapping, process_sequence), ObjectExpr373())
 
 
 __all__ = ["get_protocol_names", "get_protocols", "filter_by_protocol_by", "filter_by_protocol_name", "get_inputs_with_parameter_by", "get_outputs_with_parameter_by", "get_parameters", "get_characteristics", "get_inputs_with_characteristic_by", "get_outputs_with_characteristic_by", "get_outputs_with_factor_by", "get_factors", "get_root_inputs", "get_final_outputs", "get_root_input_of", "get_final_outputs_of", "get_units", "get_data", "get_sources", "get_samples", "get_materials"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/protocol.py` & `arctrl-2.0.0a3/arctrl/Core/Process/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...fable_modules.fable_library.types import Record
 from ...fable_modules.fable_library.util import equals
 from ..comment import (Comment, Comment_reflection)
 from ..ontology_annotation import (OntologyAnnotation, OntologyAnnotation_reflection)
 from .component import (Component, Component_reflection)
 from .protocol_parameter import (ProtocolParameter, ProtocolParameter_reflection)
 
-def _expr329() -> TypeInfo:
+def _expr331() -> TypeInfo:
     return record_type("ARCtrl.Process.Protocol", [], Protocol, lambda: [("ID", option_type(string_type)), ("Name", option_type(string_type)), ("ProtocolType", option_type(OntologyAnnotation_reflection())), ("Description", option_type(string_type)), ("Uri", option_type(string_type)), ("Version", option_type(string_type)), ("Parameters", option_type(list_type(ProtocolParameter_reflection()))), ("Components", option_type(list_type(Component_reflection()))), ("Comments", option_type(list_type(Comment_reflection())))])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class Protocol(Record):
     ID: str | None
     Name: str | None
@@ -24,51 +24,51 @@
     Description: str | None
     Uri: str | None
     Version: str | None
     Parameters: FSharpList[ProtocolParameter] | None
     Components: FSharpList[Component] | None
     Comments: FSharpList[Comment] | None
 
-Protocol_reflection = _expr329
+Protocol_reflection = _expr331
 
 def Protocol_make(id: str | None=None, name: str | None=None, protocol_type: OntologyAnnotation | None=None, description: str | None=None, uri: str | None=None, version: str | None=None, parameters: FSharpList[ProtocolParameter] | None=None, components: FSharpList[Component] | None=None, comments: FSharpList[Comment] | None=None) -> Protocol:
     return Protocol(id, name, protocol_type, description, uri, version, parameters, components, comments)
 
 
 def Protocol_create_Z414665E7(Id: str | None=None, Name: str | None=None, ProtocolType: OntologyAnnotation | None=None, Description: str | None=None, Uri: str | None=None, Version: str | None=None, Parameters: FSharpList[ProtocolParameter] | None=None, Components: FSharpList[Component] | None=None, Comments: FSharpList[Comment] | None=None) -> Protocol:
     return Protocol_make(Id, Name, ProtocolType, Description, Uri, Version, Parameters, Components, Comments)
 
 
 def Protocol_get_empty(__unit: None=None) -> Protocol:
     return Protocol_create_Z414665E7()
 
 
 def Protocol_tryGetByName(name: str, protocols: FSharpList[Protocol]) -> Protocol | None:
-    def _arrow330(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
+    def _arrow332(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
         return equals(p.Name, name)
 
-    return try_find(_arrow330, protocols)
+    return try_find(_arrow332, protocols)
 
 
 def Protocol_existsByName(name: str, protocols: FSharpList[Protocol]) -> bool:
-    def _arrow331(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
+    def _arrow333(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
         return equals(p.Name, name)
 
-    return exists(_arrow331, protocols)
+    return exists(_arrow333, protocols)
 
 
 def Protocol_add(protocols: FSharpList[Protocol], protocol: Protocol) -> FSharpList[Protocol]:
     return append(protocols, singleton(protocol))
 
 
 def Protocol_removeByName(name: str, protocols: FSharpList[Protocol]) -> FSharpList[Protocol]:
-    def _arrow332(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
+    def _arrow334(p: Protocol, name: Any=name, protocols: Any=protocols) -> bool:
         return not equals(p.Name, name)
 
-    return filter(_arrow332, protocols)
+    return filter(_arrow334, protocols)
 
 
 def Protocol_getComments_3BF20962(protocol: Protocol) -> FSharpList[Comment] | None:
     return protocol.Comments
 
 
 def Protocol_mapComments(f: Callable[[FSharpList[Comment]], FSharpList[Comment]], protocol: Protocol) -> Protocol:
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/protocol_parameter.py` & `arctrl-2.0.0a3/arctrl/Core/Process/protocol_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...fable_modules.fable_library.option import (default_arg, map, bind)
 from ...fable_modules.fable_library.reflection import (TypeInfo, string_type, option_type, record_type)
 from ...fable_modules.fable_library.types import (Array, to_string, Record)
 from ..comment import Comment
 from ..Helper.collections_ import Option_fromValueWithDefault
 from ..ontology_annotation import (OntologyAnnotation, OntologyAnnotation_reflection)
 
-def _expr328() -> TypeInfo:
+def _expr327() -> TypeInfo:
     return record_type("ARCtrl.Process.ProtocolParameter", [], ProtocolParameter, lambda: [("ID", option_type(string_type)), ("ParameterName", option_type(OntologyAnnotation_reflection()))])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class ProtocolParameter(Record):
     ID: str | None
     ParameterName: OntologyAnnotation | None
@@ -88,11 +88,11 @@
         return to_string(this)
 
     def PrintCompact(self, __unit: None=None) -> str:
         this: ProtocolParameter = self
         return "OA " + this.NameText
 
 
-ProtocolParameter_reflection = _expr328
+ProtocolParameter_reflection = _expr327
 
 __all__ = ["ProtocolParameter_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/sample.py` & `arctrl-2.0.0a3/arctrl/Core/Process/sample.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/source.py` & `arctrl-2.0.0a3/arctrl/Core/Process/source.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Process/value.py` & `arctrl-2.0.0a3/arctrl/Core/Process/value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/publication.py` & `arctrl-2.0.0a3/arctrl/Core/publication.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/arc_table.py` & `arctrl-2.0.0a3/arctrl/Core/Table/arc_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,20 +253,20 @@
         Unchecked_addColumn(header, cells_1, index_1, force_replace_1, False, this.Headers, this.Values)
         if not equals(skip_fill_missing, True):
             Unchecked_fillMissingCells(this.Headers, this.Values)
 
 
     @staticmethod
     def add_column(header: CompositeHeader, cells: Array[CompositeCell] | None=None, index: int | None=None, force_replace: bool | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow430(table: ArcTable) -> ArcTable:
+        def _arrow423(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddColumn(header, cells, index, force_replace)
             return new_table
 
-        return _arrow430
+        return _arrow423
 
     def UpdateColumn(self, column_index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None, skip_fill_missing: bool | None=None) -> None:
         this: ArcTable = self
         SanityChecks_validateColumnIndex(column_index, this.ColumnCount, False)
         column: CompositeColumn = CompositeColumn.create(header, cells)
         SanityChecks_validateColumn(column)
         header_1: CompositeHeader = column.Header
@@ -283,46 +283,46 @@
         iterate_indexed(action, column.Cells)
         if not equals(skip_fill_missing, True):
             Unchecked_fillMissingCells(this.Headers, this.Values)
 
 
     @staticmethod
     def update_column(column_index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow433(table: ArcTable) -> ArcTable:
+        def _arrow424(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.UpdateColumn(column_index, header, cells)
             return new_table
 
-        return _arrow433
+        return _arrow424
 
     def InsertColumn(self, index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTable = self
         this.AddColumn(header, cells, index, False)
 
     @staticmethod
     def insert_column(index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow434(table: ArcTable) -> ArcTable:
+        def _arrow425(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.InsertColumn(index, header, cells)
             return new_table
 
-        return _arrow434
+        return _arrow425
 
     def AppendColumn(self, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTable = self
         this.AddColumn(header, cells, this.ColumnCount, False)
 
     @staticmethod
     def append_column(header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow435(table: ArcTable) -> ArcTable:
+        def _arrow426(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AppendColumn(header, cells)
             return new_table
 
-        return _arrow435
+        return _arrow426
 
     def AddColumns(self, columns: Array[CompositeColumn], index: int | None=None, force_replace: bool | None=None, skip_fill_missing: bool | None=None) -> None:
         this: ArcTable = self
         index_1: int = default_arg(index, this.ColumnCount) or 0
         force_replace_1: bool = default_arg(force_replace, False)
         SanityChecks_validateColumnIndex(index_1, this.ColumnCount, True)
         def mapping(x: CompositeColumn) -> CompositeHeader:
@@ -353,204 +353,204 @@
         iterate_1(action_2, columns)
         if not equals(skip_fill_missing, True):
             Unchecked_fillMissingCells(this.Headers, this.Values)
 
 
     @staticmethod
     def add_columns(columns: Array[CompositeColumn], index: int | None=None, skip_fill_missing: bool | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow436(table: ArcTable) -> ArcTable:
+        def _arrow427(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddColumns(columns, index, None, skip_fill_missing)
             return new_table
 
-        return _arrow436
+        return _arrow427
 
     def RemoveColumn(self, index: int) -> None:
         this: ArcTable = self
         SanityChecks_validateColumnIndex(index, this.ColumnCount, False)
         column_count: int = this.ColumnCount or 0
         Unchecked_removeHeader(index, this.Headers)
         Unchecked_removeColumnCells_withIndexChange(index, column_count, this.RowCount, this.Values)
 
     @staticmethod
     def remove_column(index: int) -> Callable[[ArcTable], ArcTable]:
-        def _arrow437(table: ArcTable) -> ArcTable:
+        def _arrow428(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.RemoveColumn(index)
             return new_table
 
-        return _arrow437
+        return _arrow428
 
     def RemoveColumns(self, index_arr: Array[int]) -> None:
         this: ArcTable = self
-        def _arrow439(index: int) -> None:
+        def _arrow429(index: int) -> None:
             SanityChecks_validateColumnIndex(index, this.ColumnCount, False)
 
-        iterate_1(_arrow439, index_arr)
-        def _arrow440(index_1: int) -> None:
+        iterate_1(_arrow429, index_arr)
+        def _arrow430(index_1: int) -> None:
             this.RemoveColumn(index_1)
 
-        class ObjectExpr441:
+        class ObjectExpr431:
             @property
             def Compare(self) -> Callable[[int, int], int]:
                 return compare_primitives
 
-        iterate_1(_arrow440, sort_descending(index_arr, ObjectExpr441()))
+        iterate_1(_arrow430, sort_descending(index_arr, ObjectExpr431()))
 
     @staticmethod
     def remove_columns(index_arr: Array[int]) -> Callable[[ArcTable], ArcTable]:
-        def _arrow442(table: ArcTable) -> ArcTable:
+        def _arrow432(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.RemoveColumns(index_arr)
             return new_table
 
-        return _arrow442
+        return _arrow432
 
     def GetColumn(self, column_index: int) -> CompositeColumn:
         this: ArcTable = self
         SanityChecks_validateColumnIndex(column_index, this.ColumnCount, False)
         h: CompositeHeader = this.Headers[column_index]
-        def _arrow445(__unit: None=None) -> IEnumerable_1[CompositeCell]:
-            def _arrow443(i: int) -> IEnumerable_1[CompositeCell]:
+        def _arrow434(__unit: None=None) -> IEnumerable_1[CompositeCell]:
+            def _arrow433(i: int) -> IEnumerable_1[CompositeCell]:
                 match_value: CompositeCell | None = this.TryGetCellAt(column_index, i)
                 if match_value is not None:
                     return singleton(match_value)
 
                 else: 
                     to_fail(printf("Unable to find cell for index: (%i, %i)"))(column_index)(i)
                     return empty()
 
 
-            return collect(_arrow443, range_big_int(0, 1, this.RowCount - 1))
+            return collect(_arrow433, range_big_int(0, 1, this.RowCount - 1))
 
-        cells: Array[CompositeCell] = to_array(delay(_arrow445))
+        cells: Array[CompositeCell] = to_array(delay(_arrow434))
         return CompositeColumn.create(h, cells)
 
     @staticmethod
     def get_column(index: int) -> Callable[[ArcTable], CompositeColumn]:
-        def _arrow446(table: ArcTable) -> CompositeColumn:
+        def _arrow435(table: ArcTable) -> CompositeColumn:
             return table.GetColumn(index)
 
-        return _arrow446
+        return _arrow435
 
     def TryGetColumnByHeader(self, header: CompositeHeader) -> CompositeColumn | None:
         this: ArcTable = self
         def mapping(i: int) -> CompositeColumn:
             return this.GetColumn(i)
 
         def predicate(x: CompositeHeader) -> bool:
             return equals(x, header)
 
         return map_2(mapping, try_find_index(predicate, this.Headers))
 
     @staticmethod
     def try_get_column_by_header(header: CompositeHeader) -> Callable[[ArcTable], CompositeColumn | None]:
-        def _arrow448(table: ArcTable) -> CompositeColumn | None:
+        def _arrow436(table: ArcTable) -> CompositeColumn | None:
             return table.TryGetColumnByHeader(header)
 
-        return _arrow448
+        return _arrow436
 
     def GetColumnByHeader(self, header: CompositeHeader) -> CompositeColumn:
         this: ArcTable = self
         match_value: CompositeColumn | None = this.TryGetColumnByHeader(header)
         if match_value is None:
             arg: str = this.Name
             return to_fail(printf("Unable to find column with header in table %s: %O"))(arg)(header)
 
         else: 
             return match_value
 
 
     @staticmethod
     def get_column_by_header(header: CompositeHeader) -> Callable[[ArcTable], CompositeColumn]:
-        def _arrow449(table: ArcTable) -> CompositeColumn:
+        def _arrow437(table: ArcTable) -> CompositeColumn:
             return table.GetColumnByHeader(header)
 
-        return _arrow449
+        return _arrow437
 
     def TryGetInputColumn(self, __unit: None=None) -> CompositeColumn | None:
         this: ArcTable = self
         def mapping(i: int) -> CompositeColumn:
             return this.GetColumn(i)
 
         def predicate(x: CompositeHeader) -> bool:
             return x.is_input
 
         return map_2(mapping, try_find_index(predicate, this.Headers))
 
     @staticmethod
     def try_get_input_column(__unit: None=None) -> Callable[[ArcTable], CompositeColumn | None]:
-        def _arrow450(table: ArcTable) -> CompositeColumn | None:
+        def _arrow438(table: ArcTable) -> CompositeColumn | None:
             return table.TryGetInputColumn()
 
-        return _arrow450
+        return _arrow438
 
     def GetInputColumn(self, __unit: None=None) -> CompositeColumn:
         this: ArcTable = self
         match_value: CompositeColumn | None = this.TryGetInputColumn()
         if match_value is None:
             arg: str = this.Name
             return to_fail(printf("Unable to find input column in table %s"))(arg)
 
         else: 
             return match_value
 
 
     @staticmethod
     def get_input_column(__unit: None=None) -> Callable[[ArcTable], CompositeColumn]:
-        def _arrow452(table: ArcTable) -> CompositeColumn:
+        def _arrow439(table: ArcTable) -> CompositeColumn:
             return table.GetInputColumn()
 
-        return _arrow452
+        return _arrow439
 
     def TryGetOutputColumn(self, __unit: None=None) -> CompositeColumn | None:
         this: ArcTable = self
         def mapping(i: int) -> CompositeColumn:
             return this.GetColumn(i)
 
         def predicate(x: CompositeHeader) -> bool:
             return x.is_output
 
         return map_2(mapping, try_find_index(predicate, this.Headers))
 
     @staticmethod
     def try_get_output_column(__unit: None=None) -> Callable[[ArcTable], CompositeColumn | None]:
-        def _arrow454(table: ArcTable) -> CompositeColumn | None:
+        def _arrow440(table: ArcTable) -> CompositeColumn | None:
             return table.TryGetOutputColumn()
 
-        return _arrow454
+        return _arrow440
 
     def GetOutputColumn(self, __unit: None=None) -> CompositeColumn:
         this: ArcTable = self
         match_value: CompositeColumn | None = this.TryGetOutputColumn()
         if match_value is None:
             arg: str = this.Name
             return to_fail(printf("Unable to find output column in table %s"))(arg)
 
         else: 
             return match_value
 
 
     @staticmethod
     def get_output_column(__unit: None=None) -> Callable[[ArcTable], CompositeColumn]:
-        def _arrow456(table: ArcTable) -> CompositeColumn:
+        def _arrow441(table: ArcTable) -> CompositeColumn:
             return table.GetOutputColumn()
 
-        return _arrow456
+        return _arrow441
 
     def AddRow(self, cells: Array[CompositeCell] | None=None, index: int | None=None) -> None:
         this: ArcTable = self
         index_1: int = default_arg(index, this.RowCount) or 0
-        def _arrow458(__unit: None=None) -> IEnumerable_1[CompositeCell]:
-            def _arrow457(column_index: int) -> IEnumerable_1[CompositeCell]:
+        def _arrow443(__unit: None=None) -> IEnumerable_1[CompositeCell]:
+            def _arrow442(column_index: int) -> IEnumerable_1[CompositeCell]:
                 return singleton(Unchecked_getEmptyCellForHeader(this.Headers[column_index], Unchecked_tryGetCellAt(column_index, 0, this.Values)))
 
-            return collect(_arrow457, range_big_int(0, 1, this.ColumnCount - 1))
+            return collect(_arrow442, range_big_int(0, 1, this.ColumnCount - 1))
 
-        cells_1: Array[CompositeCell] = to_array(delay(_arrow458)) if (cells is None) else value_3(cells)
+        cells_1: Array[CompositeCell] = to_array(delay(_arrow443)) if (cells is None) else value_3(cells)
         SanityChecks_validateRowIndex(index_1, this.RowCount, True)
         column_count: int = this.ColumnCount or 0
         new_cells_count: int = length(cells_1) or 0
         if column_count == 0:
             raise Exception("Table contains no columns! Cannot add row to empty table!")
 
         elif new_cells_count != column_count:
@@ -559,20 +559,20 @@
         for column_index_1 in range(0, (this.ColumnCount - 1) + 1, 1):
             h_1: CompositeHeader = this.Headers[column_index_1]
             SanityChecks_validateColumn(CompositeColumn.create(h_1, [cells_1[column_index_1]]))
         Unchecked_addRow(index_1, cells_1, this.Headers, this.Values)
 
     @staticmethod
     def add_row(cells: Array[CompositeCell] | None=None, index: int | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow459(table: ArcTable) -> ArcTable:
+        def _arrow444(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddRow(cells, index)
             return new_table
 
-        return _arrow459
+        return _arrow444
 
     def UpdateRow(self, row_index: int, cells: Array[CompositeCell]) -> None:
         this: ArcTable = self
         SanityChecks_validateRowIndex(row_index, this.RowCount, False)
         column_count: int = this.RowCount or 0
         new_cells_count: int = length(cells) or 0
         if column_count == 0:
@@ -589,46 +589,46 @@
         def action_1(column_index: int, cell_1: CompositeCell) -> None:
             Unchecked_setCellAt(column_index, row_index, cell_1, this.Values)
 
         iterate_indexed(action_1, cells)
 
     @staticmethod
     def update_row(row_index: int, cells: Array[CompositeCell]) -> Callable[[ArcTable], ArcTable]:
-        def _arrow461(table: ArcTable) -> ArcTable:
+        def _arrow445(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.UpdateRow(row_index, cells)
             return new_table
 
-        return _arrow461
+        return _arrow445
 
     def AppendRow(self, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTable = self
         this.AddRow(cells, this.RowCount)
 
     @staticmethod
     def append_row(cells: Array[CompositeCell] | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow462(table: ArcTable) -> ArcTable:
+        def _arrow446(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AppendRow(cells)
             return new_table
 
-        return _arrow462
+        return _arrow446
 
     def InsertRow(self, index: int, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTable = self
         this.AddRow(cells, index)
 
     @staticmethod
     def insert_row(index: int, cells: Array[CompositeCell] | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow467(table: ArcTable) -> ArcTable:
+        def _arrow450(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddRow(cells, index)
             return new_table
 
-        return _arrow467
+        return _arrow450
 
     def AddRows(self, rows: Array[Array[CompositeCell]], index: int | None=None) -> None:
         this: ArcTable = self
         index_1: int = default_arg(index, this.RowCount) or 0
         SanityChecks_validateRowIndex(index_1, this.RowCount, True)
         def action(row: Array[CompositeCell]) -> None:
             column_count: int = this.ColumnCount or 0
@@ -646,103 +646,103 @@
             for column_index in range(0, (this.ColumnCount - 1) + 1, 1):
                 h: CompositeHeader = this.Headers[column_index]
                 SanityChecks_validateColumn(CompositeColumn.create(h, [row_1[column_index]]))
         Unchecked_addRows(index_1, rows, this.Headers, this.Values)
 
     @staticmethod
     def add_rows(rows: Array[Array[CompositeCell]], index: int | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow469(table: ArcTable) -> ArcTable:
+        def _arrow455(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddRows(rows, index)
             return new_table
 
-        return _arrow469
+        return _arrow455
 
     def AddRowsEmpty(self, row_count: int, index: int | None=None) -> None:
         this: ArcTable = self
-        def _arrow471(__unit: None=None) -> IEnumerable_1[CompositeCell]:
-            def _arrow470(column_index: int) -> IEnumerable_1[CompositeCell]:
+        def _arrow459(__unit: None=None) -> IEnumerable_1[CompositeCell]:
+            def _arrow458(column_index: int) -> IEnumerable_1[CompositeCell]:
                 return singleton(Unchecked_getEmptyCellForHeader(this.Headers[column_index], Unchecked_tryGetCellAt(column_index, 0, this.Values)))
 
-            return collect(_arrow470, range_big_int(0, 1, this.ColumnCount - 1))
+            return collect(_arrow458, range_big_int(0, 1, this.ColumnCount - 1))
 
-        row: Array[CompositeCell] = to_array(delay(_arrow471))
-        def _arrow472(_arg: int) -> Array[CompositeCell]:
+        row: Array[CompositeCell] = to_array(delay(_arrow459))
+        def _arrow460(_arg: int) -> Array[CompositeCell]:
             return row
 
-        rows: Array[Array[CompositeCell]] = initialize(row_count, _arrow472, None)
+        rows: Array[Array[CompositeCell]] = initialize(row_count, _arrow460, None)
         this.AddRows(rows, index)
 
     @staticmethod
     def add_rows_empty(row_count: int, index: int | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow473(table: ArcTable) -> ArcTable:
+        def _arrow461(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.AddRowsEmpty(row_count, index)
             return new_table
 
-        return _arrow473
+        return _arrow461
 
     def RemoveRow(self, index: int) -> None:
         this: ArcTable = self
         SanityChecks_validateRowIndex(index, this.RowCount, False)
         Unchecked_removeRowCells_withIndexChange(index, this.ColumnCount, this.RowCount, this.Values)
 
     @staticmethod
     def remove_row(index: int) -> Callable[[ArcTable], ArcTable]:
-        def _arrow474(table: ArcTable) -> ArcTable:
+        def _arrow462(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.RemoveRow(index)
             return new_table
 
-        return _arrow474
+        return _arrow462
 
     def RemoveRows(self, index_arr: Array[int]) -> None:
         this: ArcTable = self
-        def _arrow475(index: int) -> None:
+        def _arrow463(index: int) -> None:
             SanityChecks_validateRowIndex(index, this.RowCount, False)
 
-        iterate_1(_arrow475, index_arr)
-        def _arrow476(index_1: int) -> None:
+        iterate_1(_arrow463, index_arr)
+        def _arrow464(index_1: int) -> None:
             this.RemoveRow(index_1)
 
-        class ObjectExpr477:
+        class ObjectExpr465:
             @property
             def Compare(self) -> Callable[[int, int], int]:
                 return compare_primitives
 
-        iterate_1(_arrow476, sort_descending(index_arr, ObjectExpr477()))
+        iterate_1(_arrow464, sort_descending(index_arr, ObjectExpr465()))
 
     @staticmethod
     def remove_rows(index_arr: Array[int]) -> Callable[[ArcTable], ArcTable]:
-        def _arrow478(table: ArcTable) -> ArcTable:
+        def _arrow466(table: ArcTable) -> ArcTable:
             new_table: ArcTable = table.Copy()
             new_table.RemoveColumns(index_arr)
             return new_table
 
-        return _arrow478
+        return _arrow466
 
     def GetRow(self, row_index: int, SkipValidation: bool | None=None) -> Array[CompositeCell]:
         this: ArcTable = self
         if not equals(SkipValidation, True):
             SanityChecks_validateRowIndex(row_index, this.RowCount, False)
 
-        def _arrow480(__unit: None=None) -> IEnumerable_1[CompositeCell]:
-            def _arrow479(column_index: int) -> CompositeCell:
+        def _arrow468(__unit: None=None) -> IEnumerable_1[CompositeCell]:
+            def _arrow467(column_index: int) -> CompositeCell:
                 return value_3(this.TryGetCellAt(column_index, row_index))
 
-            return map(_arrow479, range_big_int(0, 1, this.ColumnCount - 1))
+            return map(_arrow467, range_big_int(0, 1, this.ColumnCount - 1))
 
-        return to_array(delay(_arrow480))
+        return to_array(delay(_arrow468))
 
     @staticmethod
     def get_row(index: int) -> Callable[[ArcTable], Array[CompositeCell]]:
-        def _arrow481(table: ArcTable) -> Array[CompositeCell]:
+        def _arrow469(table: ArcTable) -> Array[CompositeCell]:
             return table.GetRow(index)
 
-        return _arrow481
+        return _arrow469
 
     def Join(self, table: ArcTable, index: int | None=None, join_options: str | None=None, force_replace: bool | None=None, skip_fill_missing: bool | None=None) -> None:
         this: ArcTable = self
         join_options_1: str = default_arg(join_options, "headers")
         force_replace_1: bool = default_arg(force_replace, False)
         skip_fill_missing_1: bool = default_arg(skip_fill_missing, False)
         index_1: int = default_arg(index, this.ColumnCount) or 0
@@ -795,20 +795,20 @@
         iterate_1(action_2, columns)
         if not skip_fill_missing_1:
             Unchecked_fillMissingCells(this.Headers, this.Values)
 
 
     @staticmethod
     def join(table: ArcTable, index: int | None=None, join_options: str | None=None, force_replace: bool | None=None) -> Callable[[ArcTable], ArcTable]:
-        def _arrow482(this: ArcTable) -> ArcTable:
+        def _arrow470(this: ArcTable) -> ArcTable:
             copy: ArcTable = this.Copy()
             copy.Join(table, index, join_options, force_replace)
             return copy
 
-        return _arrow482
+        return _arrow470
 
     def AddProtocolTypeColumn(self, types: Array[OntologyAnnotation] | None=None, index: int | None=None) -> None:
         this: ArcTable = self
         def mapping_1(array: Array[OntologyAnnotation]) -> Array[CompositeCell]:
             def mapping(Item: OntologyAnnotation, array: Any=array) -> CompositeCell:
                 return CompositeCell(0, Item)
 
@@ -893,15 +893,15 @@
         def predicate(h: CompositeHeader) -> bool:
             return h.is_component
 
         return map_1(mapping, to_array(filter(predicate, this.Headers)), None)
 
     @staticmethod
     def SplitByColumnValues(column_index: int) -> Callable[[ArcTable], Array[ArcTable]]:
-        def _arrow484(table: ArcTable) -> Array[ArcTable]:
+        def _arrow478(table: ArcTable) -> Array[ArcTable]:
             def mapping_3(i: int, index_group: Array[int]) -> ArcTable:
                 headers: Array[CompositeHeader] = list(table.Headers)
                 def mapping_2(i_1: int, i: Any=i, index_group: Any=index_group) -> Array[CompositeCell]:
                     return table.GetRow(i_1, True)
 
                 rows: Array[Array[CompositeCell]] = map_1(mapping_2, index_group, None)
                 return ArcTable.create_from_rows(table.Name, headers, rows)
@@ -911,50 +911,50 @@
                     return tuple_1[0]
 
                 return map_1(mapping, tupled_arg[1], Int32Array)
 
             def projection(tuple: tuple[int, CompositeCell]) -> CompositeCell:
                 return tuple[1]
 
-            class ObjectExpr483:
+            class ObjectExpr477:
                 @property
                 def Equals(self) -> Callable[[CompositeCell, CompositeCell], bool]:
                     return equals
 
                 @property
                 def GetHashCode(self) -> Callable[[CompositeCell], int]:
                     return safe_hash
 
-            return map_indexed(mapping_3, map_1(mapping_1, Array_groupBy(projection, indexed(table.GetColumn(column_index).Cells), ObjectExpr483()), None), None)
+            return map_indexed(mapping_3, map_1(mapping_1, Array_groupBy(projection, indexed(table.GetColumn(column_index).Cells), ObjectExpr477()), None), None)
 
-        return _arrow484
+        return _arrow478
 
     @staticmethod
     def SplitByColumnValuesByHeader(header: CompositeHeader) -> Callable[[ArcTable], Array[ArcTable]]:
-        def _arrow485(table: ArcTable) -> Array[ArcTable]:
+        def _arrow479(table: ArcTable) -> Array[ArcTable]:
             def predicate(x: CompositeHeader) -> bool:
                 return equals(x, header)
 
             index: int | None = try_find_index(predicate, table.Headers)
             if index is None:
                 return [table.Copy()]
 
             else: 
                 i: int = index or 0
                 return ArcTable.SplitByColumnValues(i)(table)
 
 
-        return _arrow485
+        return _arrow479
 
     @staticmethod
     def SplitByProtocolREF() -> Callable[[ArcTable], Array[ArcTable]]:
-        def _arrow486(table: ArcTable) -> Array[ArcTable]:
+        def _arrow480(table: ArcTable) -> Array[ArcTable]:
             return ArcTable.SplitByColumnValuesByHeader(CompositeHeader(8))(table)
 
-        return _arrow486
+        return _arrow480
 
     @staticmethod
     def update_reference_by_annotation_table(ref_table: ArcTable, annotation_table: ArcTable) -> ArcTable:
         ref_table_1: ArcTable = ref_table.Copy()
         annotation_table_1: ArcTable = annotation_table.Copy()
         def chooser(tupled_arg: tuple[int, CompositeHeader]) -> int | None:
             if tupled_arg[1].is_protocol_column:
@@ -972,83 +972,83 @@
             c: CompositeColumn = arr[idx]
             ref_table_1.AddColumn(c.Header, c.Cells, None, True)
         return ref_table_1
 
     @staticmethod
     def append(table1: ArcTable, table2: ArcTable) -> ArcTable:
         def get_list(t: ArcTable) -> FSharpList[FSharpList[tuple[CompositeHeader, CompositeCell]]]:
-            def _arrow490(__unit: None=None, t: Any=t) -> IEnumerable_1[FSharpList[tuple[CompositeHeader, CompositeCell]]]:
-                def _arrow489(row: int) -> FSharpList[tuple[CompositeHeader, CompositeCell]]:
-                    def _arrow488(__unit: None=None) -> IEnumerable_1[tuple[CompositeHeader, CompositeCell]]:
-                        def _arrow487(col: int) -> tuple[CompositeHeader, CompositeCell]:
+            def _arrow485(__unit: None=None, t: Any=t) -> IEnumerable_1[FSharpList[tuple[CompositeHeader, CompositeCell]]]:
+                def _arrow484(row: int) -> FSharpList[tuple[CompositeHeader, CompositeCell]]:
+                    def _arrow483(__unit: None=None) -> IEnumerable_1[tuple[CompositeHeader, CompositeCell]]:
+                        def _arrow482(col: int) -> tuple[CompositeHeader, CompositeCell]:
                             return (t.Headers[col], get_item_from_dict(t.Values, (col, row)))
 
-                        return map(_arrow487, range_big_int(0, 1, t.ColumnCount - 1))
+                        return map(_arrow482, range_big_int(0, 1, t.ColumnCount - 1))
 
-                    return to_list(delay(_arrow488))
+                    return to_list(delay(_arrow483))
 
-                return map(_arrow489, range_big_int(0, 1, t.RowCount - 1))
+                return map(_arrow484, range_big_int(0, 1, t.RowCount - 1))
 
-            return to_list(delay(_arrow490))
+            return to_list(delay(_arrow485))
 
         pattern_input: tuple[Array[CompositeHeader], Any] = Unchecked_alignByHeaders(False, append(get_list(table1), get_list(table2)))
         return ArcTable.create(table1.Name, pattern_input[0], pattern_input[1])
 
     def __str__(self, __unit: None=None) -> str:
         this: ArcTable = self
-        def _arrow495(__unit: None=None) -> IEnumerable_1[str]:
-            def _arrow494(__unit: None=None) -> IEnumerable_1[str]:
-                def _arrow493(__unit: None=None) -> IEnumerable_1[str]:
-                    def _arrow492(__unit: None=None) -> IEnumerable_1[str]:
-                        def _arrow491(row_i: int) -> str:
+        def _arrow494(__unit: None=None) -> IEnumerable_1[str]:
+            def _arrow493(__unit: None=None) -> IEnumerable_1[str]:
+                def _arrow492(__unit: None=None) -> IEnumerable_1[str]:
+                    def _arrow491(__unit: None=None) -> IEnumerable_1[str]:
+                        def _arrow490(row_i: int) -> str:
                             return join("\t|\t", map(to_string, this.GetRow(row_i)))
 
-                        return map(_arrow491, range_big_int(0, 1, this.RowCount - 1))
+                        return map(_arrow490, range_big_int(0, 1, this.RowCount - 1))
 
-                    return append_1(singleton(join("\t|\t", map(to_string, this.Headers))), delay(_arrow492))
+                    return append_1(singleton(join("\t|\t", map(to_string, this.Headers))), delay(_arrow491))
 
-                return append_1(singleton("-------------"), delay(_arrow493))
+                return append_1(singleton("-------------"), delay(_arrow492))
 
-            return append_1(singleton(("Table: " + this.Name) + ""), delay(_arrow494))
+            return append_1(singleton(("Table: " + this.Name) + ""), delay(_arrow493))
 
-        return join("\n", to_list(delay(_arrow495)))
+        return join("\n", to_list(delay(_arrow494)))
 
     def StructurallyEquals(self, other: ArcTable) -> bool:
         this: ArcTable = self
         def sort(arg: Any) -> Array[Any]:
             def projection(_arg: Any, arg: Any=arg) -> tuple[int, int]:
                 return _arg[0]
 
-            class ObjectExpr496:
+            class ObjectExpr495:
                 @property
                 def Compare(self) -> Callable[[tuple[int, int], tuple[int, int]], int]:
                     return compare_arrays
 
-            return sort_by(projection, list(arg), ObjectExpr496())
+            return sort_by(projection, list(arg), ObjectExpr495())
 
-        def _arrow499(__unit: None=None) -> bool:
+        def _arrow498(__unit: None=None) -> bool:
             a: IEnumerable_1[CompositeHeader] = this.Headers
             b: IEnumerable_1[CompositeHeader] = other.Headers
             def folder(acc: bool, e: bool) -> bool:
                 if acc:
                     return e
 
                 else: 
                     return False
 
 
-            def _arrow498(__unit: None=None) -> IEnumerable_1[bool]:
-                def _arrow497(i: int) -> bool:
+            def _arrow497(__unit: None=None) -> IEnumerable_1[bool]:
+                def _arrow496(i: int) -> bool:
                     return equals(item(i, a), item(i, b))
 
-                return map(_arrow497, range_big_int(0, 1, length(a) - 1))
+                return map(_arrow496, range_big_int(0, 1, length(a) - 1))
 
-            return fold(folder, True, to_list(delay(_arrow498))) if (length(a) == length(b)) else False
+            return fold(folder, True, to_list(delay(_arrow497))) if (length(a) == length(b)) else False
 
-        if _arrow499() if (this.Name == other.Name) else False:
+        if _arrow498() if (this.Name == other.Name) else False:
             a_1: IEnumerable_1[Any] = sort(this.Values)
             b_1: IEnumerable_1[Any] = sort(other.Values)
             def folder_1(acc_1: bool, e_1: bool) -> bool:
                 if acc_1:
                     return e_1
 
                 else:
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/arc_table_aux.py` & `arctrl-2.0.0a3/arctrl/Core/Table/arc_table_aux.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/arc_tables.py` & `arctrl-2.0.0a3/arctrl/Core/Table/arc_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,91 +146,91 @@
 
 
 
 def ArcTablesAux_SanityChecks_validateSheetIndex(index: int, allow_append: bool, sheets: Array[ArcTable]) -> None:
     if index < 0:
         raise Exception("Cannot insert ArcTable at index < 0.")
 
-    def _arrow423(__unit: None=None, index: Any=index, allow_append: Any=allow_append, sheets: Any=sheets) -> bool:
+    def _arrow447(__unit: None=None, index: Any=index, allow_append: Any=allow_append, sheets: Any=sheets) -> bool:
         x: int = index or 0
         y: int = len(sheets) or 0
         return (compare(x, y) > 0) if allow_append else (compare(x, y) >= 0)
 
-    if _arrow423():
+    if _arrow447():
         raise Exception(("Specified index is out of range! Assay contains only " + str(len(sheets))) + " tables.")
 
 
 
 def ArcTablesAux_SanityChecks_validateNamesUnique(names: IEnumerable_1[str]) -> None:
-    class ObjectExpr425:
+    class ObjectExpr449:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow424(x: str, y: str) -> bool:
+            def _arrow448(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow424
+            return _arrow448
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    if not (length(names) == length(distinct(names, ObjectExpr425()))):
+    if not (length(names) == length(distinct(names, ObjectExpr449()))):
         raise Exception("Cannot add multiple tables with the same name! Table names inside one assay must be unqiue")
 
 
 
 def ArcTablesAux_SanityChecks_validateNewNameUnique(new_name: str, existing_names: IEnumerable_1[str]) -> None:
-    def _arrow426(x: str, new_name: Any=new_name, existing_names: Any=existing_names) -> bool:
+    def _arrow451(x: str, new_name: Any=new_name, existing_names: Any=existing_names) -> bool:
         return x == new_name
 
-    match_value: int | None = try_find_index(_arrow426, existing_names)
+    match_value: int | None = try_find_index(_arrow451, existing_names)
     if match_value is None:
         pass
 
     else: 
         raise Exception(((("Cannot create table with name " + new_name) + ", as table names must be unique and table at index ") + str(match_value)) + " has the same name.")
 
 
 
 def ArcTablesAux_SanityChecks_validateNewNameAtUnique(index: int, new_name: str, existing_names: IEnumerable_1[str]) -> None:
-    def _arrow427(x: str, index: Any=index, new_name: Any=new_name, existing_names: Any=existing_names) -> bool:
+    def _arrow452(x: str, index: Any=index, new_name: Any=new_name, existing_names: Any=existing_names) -> bool:
         return x == new_name
 
-    match_value: int | None = try_find_index(_arrow427, existing_names)
+    match_value: int | None = try_find_index(_arrow452, existing_names)
     if match_value is None:
         pass
 
     elif index == match_value:
         i_1: int = match_value or 0
 
     else: 
         i_2: int = match_value or 0
         raise Exception(((("Cannot create table with name " + new_name) + ", as table names must be unique and table at index ") + str(i_2)) + " has the same name.")
 
 
 
 def ArcTablesAux_SanityChecks_validateNewNamesUnique(new_names: IEnumerable_1[str], existing_names: IEnumerable_1[str]) -> None:
     ArcTablesAux_SanityChecks_validateNamesUnique(new_names)
-    class ObjectExpr428:
+    class ObjectExpr453:
         @property
         def Compare(self) -> Callable[[str, str], int]:
             return compare_primitives
 
-    class ObjectExpr429:
+    class ObjectExpr454:
         @property
         def Compare(self) -> Callable[[str, str], int]:
             return compare_primitives
 
-    same: Any = intersect(of_seq(new_names, ObjectExpr428()), of_seq(existing_names, ObjectExpr429()))
+    same: Any = intersect(of_seq(new_names, ObjectExpr453()), of_seq(existing_names, ObjectExpr454()))
     if not FSharpSet__get_IsEmpty(same):
         raise Exception(("Cannot create tables with the names " + str(same)) + ", as table names must be unique.")
 
 
 
-def _expr468() -> TypeInfo:
+def _expr499() -> TypeInfo:
     return class_type("ARCtrl.ArcTables", None, ArcTables)
 
 
 class ArcTables:
     def __init__(self, init_tables: Array[ArcTable]) -> None:
         self.tables: Array[ArcTable] = init_tables
 
@@ -247,21 +247,21 @@
     def get_item(self, index: int) -> ArcTable:
         this: ArcTables = self
         return this.Tables[index]
 
     @property
     def TableNames(self, __unit: None=None) -> FSharpList[str]:
         this: ArcTables = self
-        def _arrow432(__unit: None=None) -> IEnumerable_1[str]:
-            def _arrow431(s: ArcTable) -> str:
+        def _arrow457(__unit: None=None) -> IEnumerable_1[str]:
+            def _arrow456(s: ArcTable) -> str:
                 return s.Name
 
-            return map_1(_arrow431, this.Tables)
+            return map_1(_arrow456, this.Tables)
 
-        return to_list(delay(_arrow432))
+        return to_list(delay(_arrow457))
 
     @property
     def TableCount(self, __unit: None=None) -> int:
         this: ArcTables = self
         return len(this.Tables)
 
     def AddTable(self, table: ArcTable, index: int | None=None) -> None:
@@ -372,42 +372,42 @@
     def RenameTable(self, name: str, new_name: str) -> None:
         this: ArcTables = self
         tupled_arg: tuple[int, str] = (ArcTablesAux_findIndexByTableName(name, this.Tables), new_name)
         this.RenameTableAt(tupled_arg[0], tupled_arg[1])
 
     def AddColumnAt(self, table_index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None, column_index: int | None=None, force_replace: bool | None=None) -> None:
         this: ArcTables = self
-        def _arrow438(table: ArcTable) -> None:
+        def _arrow471(table: ArcTable) -> None:
             table.AddColumn(header, cells, column_index, force_replace)
 
-        this.MapTableAt(table_index, _arrow438)
+        this.MapTableAt(table_index, _arrow471)
 
     def AddColumn(self, table_name: str, header: CompositeHeader, cells: Array[CompositeCell] | None=None, column_index: int | None=None, force_replace: bool | None=None) -> None:
         this: ArcTables = self
         i: int = ArcTablesAux_findIndexByTableName(table_name, this.Tables) or 0
         this.AddColumnAt(i, header, cells, column_index, force_replace)
 
     def RemoveColumnAt(self, table_index: int, column_index: int) -> None:
         this: ArcTables = self
-        def _arrow444(table: ArcTable) -> None:
+        def _arrow472(table: ArcTable) -> None:
             table.RemoveColumn(column_index)
 
-        this.MapTableAt(table_index, _arrow444)
+        this.MapTableAt(table_index, _arrow472)
 
     def RemoveColumn(self, table_name: str, column_index: int) -> None:
         this: ArcTables = self
         tupled_arg: tuple[int, int] = (ArcTablesAux_findIndexByTableName(table_name, this.Tables), column_index)
         this.RemoveColumnAt(tupled_arg[0], tupled_arg[1])
 
     def UpdateColumnAt(self, table_index: int, column_index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTables = self
-        def _arrow447(table: ArcTable) -> None:
+        def _arrow473(table: ArcTable) -> None:
             table.UpdateColumn(column_index, header, cells)
 
-        this.MapTableAt(table_index, _arrow447)
+        this.MapTableAt(table_index, _arrow473)
 
     def UpdateColumn(self, table_name: str, column_index: int, header: CompositeHeader, cells: Array[CompositeCell] | None=None) -> None:
         this: ArcTables = self
         table_index: int = ArcTablesAux_findIndexByTableName(table_name, this.Tables) or 0
         this.UpdateColumnAt(table_index, column_index, header, cells)
 
     def GetColumnAt(self, table_index: int, column_index: int) -> CompositeColumn:
@@ -418,42 +418,42 @@
     def GetColumn(self, table_name: str, column_index: int) -> CompositeColumn:
         this: ArcTables = self
         tupled_arg: tuple[int, int] = (ArcTablesAux_findIndexByTableName(table_name, this.Tables), column_index)
         return this.GetColumnAt(tupled_arg[0], tupled_arg[1])
 
     def AddRowAt(self, table_index: int, cells: Array[CompositeCell] | None=None, row_index: int | None=None) -> None:
         this: ArcTables = self
-        def _arrow451(table: ArcTable) -> None:
+        def _arrow474(table: ArcTable) -> None:
             table.AddRow(cells, row_index)
 
-        this.MapTableAt(table_index, _arrow451)
+        this.MapTableAt(table_index, _arrow474)
 
     def AddRow(self, table_name: str, cells: Array[CompositeCell] | None=None, row_index: int | None=None) -> None:
         this: ArcTables = self
         i: int = ArcTablesAux_findIndexByTableName(table_name, this.Tables) or 0
         this.AddRowAt(i, cells, row_index)
 
     def RemoveRowAt(self, table_index: int, row_index: int) -> None:
         this: ArcTables = self
-        def _arrow453(table: ArcTable) -> None:
+        def _arrow475(table: ArcTable) -> None:
             table.RemoveRow(row_index)
 
-        this.MapTableAt(table_index, _arrow453)
+        this.MapTableAt(table_index, _arrow475)
 
     def RemoveRow(self, table_name: str, row_index: int) -> None:
         this: ArcTables = self
         tupled_arg: tuple[int, int] = (ArcTablesAux_findIndexByTableName(table_name, this.Tables), row_index)
         this.RemoveRowAt(tupled_arg[0], tupled_arg[1])
 
     def UpdateRowAt(self, table_index: int, row_index: int, cells: Array[CompositeCell]) -> None:
         this: ArcTables = self
-        def _arrow455(table: ArcTable) -> None:
+        def _arrow476(table: ArcTable) -> None:
             table.UpdateRow(row_index, cells)
 
-        this.MapTableAt(table_index, _arrow455)
+        this.MapTableAt(table_index, _arrow476)
 
     def UpdateRow(self, table_name: str, row_index: int, cells: Array[CompositeCell]) -> None:
         this: ArcTables = self
         tupled_arg: tuple[int, int, Array[CompositeCell]] = (ArcTablesAux_findIndexByTableName(table_name, this.Tables), row_index, cells)
         this.UpdateRowAt(tupled_arg[0], tupled_arg[1], tupled_arg[2])
 
     def GetRowAt(self, table_index: int, row_index: int) -> Array[CompositeCell]:
@@ -482,21 +482,21 @@
         used_tables: Any = set([])
         def chooser(t: ArcTable) -> tuple[str, ArcTable] | None:
             def mapping(c: CompositeColumn, t: Any=t) -> tuple[str, ArcTable]:
                 return (c.Cells[0].AsFreeText, t)
 
             return map_2(mapping, t.TryGetProtocolNameColumn())
 
-        class ObjectExpr460:
+        class ObjectExpr481:
             @property
             def Compare(self) -> Callable[[str, str], int]:
                 return compare_primitives
 
-        reference_table_map: Any = of_seq_1(choose(chooser, reference_tables.Tables), ObjectExpr460())
-        def _arrow466(__unit: None=None) -> IEnumerable_1[ArcTable]:
+        reference_table_map: Any = of_seq_1(choose(chooser, reference_tables.Tables), ObjectExpr481())
+        def _arrow489(__unit: None=None) -> IEnumerable_1[ArcTable]:
             def mapping_4(t_3: ArcTable) -> ArcTable:
                 Unchecked_fillMissingCells(t_3.Headers, t_3.Values)
                 return t_3
 
             def mapping_3(tupled_arg: tuple[str, Array[ArcTable]]) -> ArcTable:
                 def reduction(table: ArcTable, table_1: ArcTable, tupled_arg: Any=tupled_arg) -> ArcTable:
                     return ArcTable.append(table, table_1)
@@ -529,56 +529,56 @@
                 else: 
                     rt: ArcTable = match_value
                     ignore(add_to_set(k, used_tables))
                     updated_table: ArcTable = ArcTable.update_reference_by_annotation_table(rt, t_1)
                     return ArcTable.create(t_1.Name, updated_table.Headers, updated_table.Values)
 
 
-            def _arrow463(__unit: None=None) -> Array[ArcTable]:
+            def _arrow486(__unit: None=None) -> Array[ArcTable]:
                 array: Array[ArcTable] = to_array(sheet_tables.Tables)
                 return collect(ArcTable.SplitByProtocolREF(), array, None)
 
-            class ObjectExpr465:
+            class ObjectExpr488:
                 @property
                 def Equals(self) -> Callable[[str, str], bool]:
-                    def _arrow464(x_2: str, y_1: str) -> bool:
+                    def _arrow487(x_2: str, y_1: str) -> bool:
                         return x_2 == y_1
 
-                    return _arrow464
+                    return _arrow487
 
                 @property
                 def GetHashCode(self) -> Callable[[str], int]:
                     return string_hash
 
-            s: Array[ArcTable] = map_3(mapping_4, map_3(mapping_3, Array_groupBy(projection, map_3(mapping_2, _arrow463(), None), ObjectExpr465()), None), None)
+            s: Array[ArcTable] = map_3(mapping_4, map_3(mapping_3, Array_groupBy(projection, map_3(mapping_2, _arrow486(), None), ObjectExpr488()), None), None)
             def chooser_1(kv: Any) -> ArcTable | None:
                 if kv[0] in used_tables:
                     return None
 
                 else: 
                     return kv[1]
 
 
             return append(choose(chooser_1, reference_table_map), s) if keep_unused_ref_tables_1 else s
 
-        return ArcTables(list(_arrow466()))
+        return ArcTables(list(_arrow489()))
 
     def GetEnumerator(self, __unit: None=None) -> IEnumerator[ArcTable]:
         this: ArcTables = self
         return get_enumerator(this.Tables)
 
     def __iter__(self) -> IEnumerator[ArcTable]:
         return to_iterator(self.GetEnumerator())
 
     def System_Collections_IEnumerable_GetEnumerator(self, __unit: None=None) -> IEnumerator[Any]:
         this: ArcTables = self
         return get_enumerator(this.Tables)
 
 
-ArcTables_reflection = _expr468
+ArcTables_reflection = _expr499
 
 def ArcTables__ctor_Z420F2E1A(init_tables: Array[ArcTable]) -> ArcTables:
     return ArcTables(init_tables)
 
 
 __all__ = ["ArcTablesAux_tryFindIndexByTableName", "ArcTablesAux_findIndexByTableName", "ArcTablesAux_getIOMap", "ArcTablesAux_applyIOMap", "ArcTablesAux_SanityChecks_validateSheetIndex", "ArcTablesAux_SanityChecks_validateNamesUnique", "ArcTablesAux_SanityChecks_validateNewNameUnique", "ArcTablesAux_SanityChecks_validateNewNameAtUnique", "ArcTablesAux_SanityChecks_validateNewNamesUnique", "ArcTables_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/composite_cell.py` & `arctrl-2.0.0a3/arctrl/Core/Table/composite_cell.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/composite_column.py` & `arctrl-2.0.0a3/arctrl/Core/Table/composite_column.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/Table/composite_header.py` & `arctrl-2.0.0a3/arctrl/Core/Table/composite_header.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/template.py` & `arctrl-2.0.0a3/arctrl/Core/template.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Core/templates.py` & `arctrl-2.0.0a3/arctrl/Core/templates.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/array_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/array_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/async_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/async_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/async_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/async_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/big_int.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/big_int.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/bit_converter.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/bit_converter.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/boolean.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/boolean.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/char.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/char.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/choice.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/choice.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/date.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/date.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/date_offset.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/date_offset.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/decimal_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/decimal_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/diagnostics.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/diagnostics.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/double.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/double.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/encoding.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/encoding.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/event.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/event.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/choice.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/choice.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_collections.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_collections.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_core.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/fsharp_core.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/global_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/global_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/map.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/map.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/mutable_map.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/mutable_map.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/mutable_set.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/mutable_set.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/range.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/range.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/result.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/result.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/seq.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/seq.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/seq2.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/seq2.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/set.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/set.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/system_collections_generic.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/system_collections_generic.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fable-library-ts/system_text.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fable-library-ts/system_text.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/file.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/file.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fsharp_collections.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fsharp_collections.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/fsharp_core.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/fsharp_core.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/global_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/global_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/guid.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/guid.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/int32.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/int32.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/list.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/list.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/long.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/long.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mailbox_processor.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mailbox_processor.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/map.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/map.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/map_util.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/map_util.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mutable_map.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mutable_map.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/mutable_set.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/mutable_set.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/native.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/native.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/numeric.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/numeric.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/observable.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/observable.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/option.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/option.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/path.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/path.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/range.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/range.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/reflection.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/reflection.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/reg_exp.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/reg_exp.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/resize_array.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/resize_array.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/result.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/result.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/seq.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/seq.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/seq2.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/seq2.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/set.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/set.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/singleton_local_time_zone.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/singleton_local_time_zone.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/string_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/string_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/system_collections_generic.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/system_collections_generic.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/system_text.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/system_text.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/task.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/task.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/task_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/task_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/time_span.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/time_span.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/timer.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/timer.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/types.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/types.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/uri.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/uri.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_library/util.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_library/util.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/cognite-sdk/cognite_sdk.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/cognite-sdk/cognite_sdk.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/cognite-sdk/CogniteSdk.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/cognite-sdk/CogniteSdk.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/Fable.Python.fsproj` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/Fable.Python.fsproj`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/flask/Flask.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/flask/Flask.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/flask/flask.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/flask/flask.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/ipy_widgets.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/ipy_widgets.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/jupyter/IPyWidgets.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/jupyter/IPyWidgets.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Ast.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Ast.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/Futures.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/Futures.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/futures.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/futures.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/Tasks.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/Tasks.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/asyncio/tasks.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Base64.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Base64.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Builtins.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Builtins.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/builtins_.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/builtins_.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Math.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Math.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Os.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Os.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Queue.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Queue.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Sys.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Sys.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/Time.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/Time.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_python/stdlib/TkInter.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_python/stdlib/TkInter.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Fable.SimpleHttp.fsproj` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Fable.SimpleHttp.fsproj`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Http.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Http.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/http.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/http.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/Types.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/Types.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fable_simple_http/types.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fable_simple_http/types.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cell.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cell.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cells_collection.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/fs_cells_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,42 +422,42 @@
 
 
 def FsCellsCollection__GetFirstAddress(this: FsCellsCollection) -> FsAddress:
     if True if is_empty(this._rowsCollection) else is_empty(this._rowsCollection.keys()):
         return FsAddress__ctor_Z37302880(0, 0)
 
     else: 
-        class ObjectExpr43:
+        class ObjectExpr42:
             @property
             def Compare(self) -> Callable[[int, int], int]:
                 return compare_primitives
 
-        def _arrow47(__unit: None=None, this: Any=this) -> int:
+        def _arrow46(__unit: None=None, this: Any=this) -> int:
             def projection(d: Any) -> int:
-                class ObjectExpr44:
+                class ObjectExpr43:
                     @property
                     def Compare(self) -> Callable[[int, int], int]:
                         return compare_primitives
 
-                return min(d.keys(), ObjectExpr44())
+                return min(d.keys(), ObjectExpr43())
 
-            class ObjectExpr45:
+            class ObjectExpr44:
                 @property
                 def Compare(self) -> Callable[[int, int], int]:
                     return compare_primitives
 
-            d_1: Any = min_by(projection, this._rowsCollection.values(), ObjectExpr45())
-            class ObjectExpr46:
+            d_1: Any = min_by(projection, this._rowsCollection.values(), ObjectExpr44())
+            class ObjectExpr45:
                 @property
                 def Compare(self) -> Callable[[int, int], int]:
                     return compare_primitives
 
-            return min(d_1.keys(), ObjectExpr46())
+            return min(d_1.keys(), ObjectExpr45())
 
-        return FsAddress__ctor_Z37302880(min(this._rowsCollection.keys(), ObjectExpr43()), _arrow47())
+        return FsAddress__ctor_Z37302880(min(this._rowsCollection.keys(), ObjectExpr42()), _arrow46())
 
 
 
 def FsCellsCollection_getFirstAddress_Z2740B3CA(cells: FsCellsCollection) -> FsAddress:
     return FsCellsCollection__GetFirstAddress(cells)
```

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/FsCell.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/FsCell.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Cells/FsCellsCollection.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Cells/FsCellsCollection.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/cell_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/cell_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/CellBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/CellBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/column_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/column_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/ColumnBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/ColumnBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/DSL.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/DSL.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/dsl.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/dsl.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Expression.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Expression.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/expression.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/expression.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Operators.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Operators.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/row_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/row_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/RowBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/RowBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/sheet_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/sheet_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/SheetBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/SheetBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/table_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/table_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/TableBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/TableBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Transform.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Transform.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/transform.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/transform.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/Types.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/Types.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/types.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/types.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/workbook_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/workbook_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/DSL/WorkbookBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/DSL/WorkbookBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_address.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_address.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_column.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..fable_library.util import (IEnumerable_1, compare_primitives, ignore, get_enumerator, IEnumerator, to_iterator)
 from .Cells.fs_cell import FsCell
 from .Cells.fs_cells_collection import (FsCellsCollection__ctor, FsCellsCollection__GetCellsInColumn_Z524259A4, FsCellsCollection, FsCellsCollection__Add_Z21F271A4)
 from .fs_address import (FsAddress__ctor_Z37302880, FsAddress__get_RowNumber, FsAddress__get_ColumnNumber, FsAddress__set_ColumnNumber_Z524259A4)
 from .Ranges.fs_range_address import (FsRangeAddress__ctor_7E77A4A0, FsRangeAddress__get_FirstAddress, FsRangeAddress__get_LastAddress, FsRangeAddress__Copy, FsRangeAddress)
 from .Ranges.fs_range_base import (FsRangeBase__Cells_Z2740B3CA, FsRangeBase__get_RangeAddress, FsRangeBase__Cell_Z3407A44B, FsRangeBase, FsRangeBase_reflection)
 
-def _expr65() -> TypeInfo:
+def _expr64() -> TypeInfo:
     return class_type("FsSpreadsheet.FsColumn", None, FsColumn, FsRangeBase_reflection())
 
 
 class FsColumn(FsRangeBase):
     def __init__(self, range_address: FsRangeAddress, cells: FsCellsCollection) -> None:
         super().__init__(range_address)
         self.cells_004018: FsCellsCollection = cells
@@ -26,44 +26,44 @@
     @staticmethod
     def create_at(index: int, cells: FsCellsCollection) -> FsColumn:
         def get_index_by(f: Callable[[Callable[[FsCell], int], IEnumerable_1[FsCell]], FsCell]) -> int:
             if length(FsCellsCollection__GetCellsInColumn_Z524259A4(cells, index)) == 0:
                 return 1
 
             else: 
-                def _arrow58(c: FsCell, f: Any=f) -> int:
+                def _arrow57(c: FsCell, f: Any=f) -> int:
                     return FsAddress__get_RowNumber(c.Address)
 
-                return FsAddress__get_RowNumber(f(_arrow58)(FsCellsCollection__GetCellsInColumn_Z524259A4(cells, index)).Address)
+                return FsAddress__get_RowNumber(f(_arrow57)(FsCellsCollection__GetCellsInColumn_Z524259A4(cells, index)).Address)
 
 
-        def _arrow61(projection: Callable[[FsCell], int]) -> Callable[[IEnumerable_1[FsCell]], FsCell]:
-            def _arrow60(source_1: IEnumerable_1[FsCell]) -> FsCell:
-                class ObjectExpr59:
+        def _arrow60(projection: Callable[[FsCell], int]) -> Callable[[IEnumerable_1[FsCell]], FsCell]:
+            def _arrow59(source_1: IEnumerable_1[FsCell]) -> FsCell:
+                class ObjectExpr58:
                     @property
                     def Compare(self) -> Callable[[int, int], int]:
                         return compare_primitives
 
-                return min_by(projection, source_1, ObjectExpr59())
+                return min_by(projection, source_1, ObjectExpr58())
 
-            return _arrow60
+            return _arrow59
 
-        min_row_index: int = get_index_by(_arrow61) or 0
-        def _arrow64(projection_1: Callable[[FsCell], int]) -> Callable[[IEnumerable_1[FsCell]], FsCell]:
-            def _arrow63(source_2: IEnumerable_1[FsCell]) -> FsCell:
-                class ObjectExpr62:
+        min_row_index: int = get_index_by(_arrow60) or 0
+        def _arrow63(projection_1: Callable[[FsCell], int]) -> Callable[[IEnumerable_1[FsCell]], FsCell]:
+            def _arrow62(source_2: IEnumerable_1[FsCell]) -> FsCell:
+                class ObjectExpr61:
                     @property
                     def Compare(self) -> Callable[[int, int], int]:
                         return compare_primitives
 
-                return max_by(projection_1, source_2, ObjectExpr62())
+                return max_by(projection_1, source_2, ObjectExpr61())
 
-            return _arrow63
+            return _arrow62
 
-        max_row_index: int = get_index_by(_arrow64) or 0
+        max_row_index: int = get_index_by(_arrow63) or 0
         return FsColumn(FsRangeAddress__ctor_7E77A4A0(FsAddress__ctor_Z37302880(min_row_index, index), FsAddress__ctor_Z37302880(max_row_index, index)), cells)
 
     @property
     def Cells(self, __unit: None=None) -> IEnumerable_1[FsCell]:
         this: FsColumn = self
         return FsRangeBase__Cells_Z2740B3CA(this, this.cells_004018)
 
@@ -158,15 +158,15 @@
         return to_iterator(self.GetEnumerator())
 
     def System_Collections_IEnumerable_GetEnumerator(self, __unit: None=None) -> IEnumerator[Any]:
         this: FsColumn = self
         return get_enumerator(this)
 
 
-FsColumn_reflection = _expr65
+FsColumn_reflection = _expr64
 
 def FsColumn__ctor_7678C70A(range_address: FsRangeAddress, cells: FsCellsCollection) -> FsColumn:
     return FsColumn(range_address, cells)
 
 
 __all__ = ["FsColumn_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_row.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..fable_library.util import (IEnumerable_1, compare_primitives, ignore, get_enumerator, IEnumerator, to_iterator)
 from .Cells.fs_cell import FsCell
 from .Cells.fs_cells_collection import (FsCellsCollection__ctor, FsCellsCollection__GetCellsInRow_Z524259A4, FsCellsCollection, FsCellsCollection__Add_Z21F271A4, FsCellsCollection__Add_2E78CE33)
 from .fs_address import (FsAddress__ctor_Z37302880, FsAddress__get_ColumnNumber, FsAddress__get_RowNumber, FsAddress__set_RowNumber_Z524259A4)
 from .Ranges.fs_range_address import (FsRangeAddress__ctor_7E77A4A0, FsRangeAddress__get_FirstAddress, FsRangeAddress__get_LastAddress, FsRangeAddress__Copy, FsRangeAddress)
 from .Ranges.fs_range_base import (FsRangeBase__Cells_Z2740B3CA, FsRangeBase__get_RangeAddress, FsRangeBase__Cell_Z3407A44B, FsRangeBase, FsRangeBase_reflection)
 
-def _expr57() -> TypeInfo:
+def _expr56() -> TypeInfo:
     return class_type("FsSpreadsheet.FsRow", None, FsRow, FsRangeBase_reflection())
 
 
 class FsRow(FsRangeBase):
     def __init__(self, range_address: FsRangeAddress, cells: FsCellsCollection) -> None:
         super().__init__(range_address)
         self.cells_004021: FsCellsCollection = cells
@@ -169,15 +169,15 @@
         return to_iterator(self.GetEnumerator())
 
     def System_Collections_IEnumerable_GetEnumerator(self, __unit: None=None) -> IEnumerator[Any]:
         this: FsRow = self
         return get_enumerator(this)
 
 
-FsRow_reflection = _expr57
+FsRow_reflection = _expr56
 
 def FsRow__ctor_7678C70A(range_address: FsRangeAddress, cells: FsCellsCollection) -> FsRow:
     return FsRow(range_address, cells)
 
 
 __all__ = ["FsRow_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_workbook.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_workbook.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/fs_worksheet.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/fs_worksheet.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsAddress.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsAddress.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsColumn.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsColumn.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsRow.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsRow.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsSpreadsheet.fsproj` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsSpreadsheet.fsproj`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsWorkbook.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsWorkbook.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/FsWorksheet.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/FsWorksheet.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Debug/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/obj/Release/netstandard2.0/FsSpreadsheet.AssemblyInfo.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_address.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_address.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_base.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_base.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_column.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from ...fable_library.util import IEnumerable_1
 from ..Cells.fs_cell import FsCell
 from ..Cells.fs_cells_collection import FsCellsCollection
 from ..fs_address import (FsAddress__ctor_Z37302880, FsAddress__get_ColumnNumber, FsAddress__set_ColumnNumber_Z524259A4, FsAddress__get_RowNumber)
 from .fs_range_address import (FsRangeAddress, FsRangeAddress__ctor_7E77A4A0, FsRangeAddress__get_FirstAddress, FsRangeAddress__get_LastAddress, FsRangeAddress__Copy)
 from .fs_range_base import (FsRangeBase, FsRangeBase_reflection, FsRangeBase__get_RangeAddress, FsRangeBase__Cell_Z3407A44B, FsRangeBase__Cells_Z2740B3CA)
 
-def _expr42() -> TypeInfo:
+def _expr47() -> TypeInfo:
     return class_type("FsSpreadsheet.FsRangeColumn", None, FsRangeColumn, FsRangeBase_reflection())
 
 
 class FsRangeColumn(FsRangeBase):
     def __init__(self, range_address: FsRangeAddress) -> None:
         super().__init__(range_address)
         pass
 
 
-FsRangeColumn_reflection = _expr42
+FsRangeColumn_reflection = _expr47
 
 def FsRangeColumn__ctor_6A2513BC(range_address: FsRangeAddress) -> FsRangeColumn:
     return FsRangeColumn(range_address)
 
 
 def FsRangeColumn__ctor_Z524259A4(index: int) -> FsRangeColumn:
     return FsRangeColumn__ctor_6A2513BC(FsRangeAddress__ctor_7E77A4A0(FsAddress__ctor_Z37302880(0, index), FsAddress__ctor_Z37302880(0, index)))
```

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_row.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/fs_range_row.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRange.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRange.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeAddress.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeAddress.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeBase.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeBase.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeColumn.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeColumn.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeRow.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Ranges/FsRangeRow.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/sheet_builder.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/sheet_builder.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/SheetBuilder.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/SheetBuilder.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_field.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_field.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_row.py` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/fs_table_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 from ...fable_library.reflection import (TypeInfo, class_type)
 from ..Ranges.fs_range_address import FsRangeAddress
 from ..Ranges.fs_range_row import (FsRangeRow, FsRangeRow_reflection)
 
-def _expr56() -> TypeInfo:
+def _expr65() -> TypeInfo:
     return class_type("FsSpreadsheet.FsTableRow", None, FsTableRow, FsRangeRow_reflection())
 
 
 class FsTableRow(FsRangeRow):
     def __init__(self, range_address: FsRangeAddress) -> None:
         super().__init__(range_address)
         pass
 
 
-FsTableRow_reflection = _expr56
+FsTableRow_reflection = _expr65
 
 def FsTableRow__ctor_6A2513BC(range_address: FsRangeAddress) -> FsTableRow:
     return FsTableRow(range_address)
 
 
 __all__ = ["FsTableRow_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/FsTable.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/FsTable.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableField.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/fs_spreadsheet/Tables/FsTableField.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/project_cracked.json` & `arctrl-2.0.0a3/arctrl/fable_modules/project_cracked.json`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Decode.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Decode.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/decode.py` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/decode.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Encode.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Encode.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/encode.py` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/encode.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/Thoth.Json.Core.AssemblyInfo.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/obj/Debug/netstandard2.0/Thoth.Json.Core.AssemblyInfo.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Thoth.Json.Core.fsproj` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Thoth.Json.Core.fsproj`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/Types.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/Types.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_core/types.py` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_core/types.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Decode.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Decode.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/decode.py` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/decode.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Encode.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Encode.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/encode.py` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/encode.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Debug/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/obj/Release/netstandard2.0/Thoth.Json.Python.AssemblyInfo.fs`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/fable_modules/thoth_json_python/Thoth.Json.Python.fsproj` & `arctrl-2.0.0a3/arctrl/fable_modules/thoth_json_python/Thoth.Json.Python.fsproj`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/FileSystem/commit.py` & `arctrl-2.0.0a3/arctrl/FileSystem/commit.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/FileSystem/default_gitignore.py` & `arctrl-2.0.0a3/arctrl/FileSystem/default_gitignore.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/FileSystem/file_system.py` & `arctrl-2.0.0a3/arctrl/FileSystem/file_system.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/FileSystem/file_system_tree.py` & `arctrl-2.0.0a3/arctrl/FileSystem/file_system_tree.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/FileSystem/path.py` & `arctrl-2.0.0a3/arctrl/FileSystem/path.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/arc.py` & `arctrl-2.0.0a3/arctrl/Json/arc.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/assay.py` & `arctrl-2.0.0a3/arctrl/Json/assay.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/comment.py` & `arctrl-2.0.0a3/arctrl/Json/comment.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_assay_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_assay_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_comment_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_comment_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_component_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_component_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_data_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_data_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_factor_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_factor_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_factor_value_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_factor_value_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_investigation_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_investigation_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_attribute_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_attribute_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_attribute_value_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_attribute_value_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_material_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_material_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_ontology_annotation_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_ontology_annotation_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from ....fable_modules.fable_library.reflection import (TypeInfo, string_type, record_type)
 from ....fable_modules.fable_library.types import Record
 from ....fable_modules.fable_library.util import to_enumerable
 from ....fable_modules.thoth_json_core.types import Json
 
-def _expr923() -> TypeInfo:
+def _expr919() -> TypeInfo:
     return record_type("ARCtrl.Json.ROCrateContext.OntologyAnnotation.IContext", [], IContext, lambda: [("sdo", string_type), ("arc", string_type), ("OntologyAnnotation", string_type), ("annotation_value", string_type), ("term_source", string_type), ("term_accession", string_type), ("comments", string_type)])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class IContext(Record):
     sdo: str
     arc: str
     OntologyAnnotation: str
     annotation_value: str
     term_source: str
     term_accession: str
     comments: str
 
-IContext_reflection = _expr923
+IContext_reflection = _expr919
 
 context_jsonvalue: Json = Json(5, to_enumerable([("sdo", Json(0, "http://schema.org/")), ("OntologyAnnotation", Json(0, "sdo:DefinedTerm")), ("annotationValue", Json(0, "sdo:name")), ("termSource", Json(0, "sdo:inDefinedTermSet")), ("termAccession", Json(0, "sdo:termCode")), ("comments", Json(0, "sdo:disambiguatingDescription"))]))
 
 __all__ = ["IContext_reflection", "context_jsonvalue"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_ontology_source_reference_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_ontology_source_reference_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from ....fable_modules.fable_library.reflection import (TypeInfo, string_type, record_type)
 from ....fable_modules.fable_library.types import Record
 from ....fable_modules.fable_library.util import to_enumerable
 from ....fable_modules.thoth_json_core.types import Json
 
-def _expr933() -> TypeInfo:
+def _expr930() -> TypeInfo:
     return record_type("ARCtrl.Json.ROCrateContext.OntologySourceReference.IContext", [], IContext, lambda: [("sdo", string_type), ("arc", string_type), ("OntologySourceReference", string_type), ("description", string_type), ("name", string_type), ("file", string_type), ("version", string_type), ("comments", string_type)])
 
 
 @dataclass(eq = False, repr = False, slots = True)
 class IContext(Record):
     sdo: str
     arc: str
     OntologySourceReference: str
     description: str
     name: str
     file: str
     version: str
     comments: str
 
-IContext_reflection = _expr933
+IContext_reflection = _expr930
 
 context_jsonvalue: Json = Json(5, to_enumerable([("sdo", Json(0, "http://schema.org/")), ("OntologySourceReference", Json(0, "sdo:DefinedTermSet")), ("description", Json(0, "sdo:description")), ("name", Json(0, "sdo:name")), ("file", Json(0, "sdo:url")), ("version", Json(0, "sdo:version")), ("comments", Json(0, "sdo:disambiguatingDescription"))]))
 
 context_str: str = "\r\n{\r\n  \"@context\": {\r\n    \"sdo\": \"http://schema.org/\",\r\n    \"arc\": \"http://purl.org/nfdi4plants/ontology/\",\r\n\r\n    \"OntologySourceReference\": \"sdo:DefinedTermSet\",\r\n    \r\n    \"description\": \"sdo:description\",\r\n    \"name\": \"sdo:name\",\r\n    \"file\": \"sdo:url\",\r\n    \"version\": \"sdo:version\",\r\n    \"comments\": \"sdo:disambiguatingDescription\"\r\n  }\r\n}\r\n    "
 
 __all__ = ["IContext_reflection", "context_jsonvalue", "context_str"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_organization_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_organization_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_person_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_person_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_process_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_process_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_process_parameter_value_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_process_parameter_value_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_protocol_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_protocol_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_protocol_parameter_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_protocol_parameter_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_publication_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_publication_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_sample_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_sample_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_source_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_source_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/isa_study_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/isa_study_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/property_value_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/property_value_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/context/rocrate/rocrate_context.py` & `arctrl-2.0.0a3/arctrl/Json/context/rocrate/rocrate_context.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/converter_options.py` & `arctrl-2.0.0a3/arctrl/Json/converter_options.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/decode.py` & `arctrl-2.0.0a3/arctrl/Json/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,46 +42,46 @@
 
 Decode_helpers: IDecoderHelpers_1[Any] = Decode_helpers_1
 
 def Decode_isURI(s: str) -> bool:
     return True
 
 
-class ObjectExpr947(Decoder_1[str]):
+class ObjectExpr946(Decoder_1[str]):
     def Decode(self, s: IDecoderHelpers_1[__A_], json: __A_) -> FSharpResult_2[str, tuple[str, ErrorReason_1[__A_]]]:
         match_value: FSharpResult_2[str, tuple[str, ErrorReason_1[__A_]]] = string.Decode(s, json)
         if match_value.tag == 1:
             return FSharpResult_2(1, match_value.fields[0])
 
         elif Decode_isURI(match_value.fields[0]):
             return FSharpResult_2(0, match_value.fields[0])
 
         else: 
             s_3: str = match_value.fields[0]
             return FSharpResult_2(1, (s_3, ErrorReason_1(6, to_text(printf("Expected URI, got %s"))(s_3))))
 
 
 
-Decode_uri: Decoder_1[str] = ObjectExpr947()
+Decode_uri: Decoder_1[str] = ObjectExpr946()
 
 def Decode_hasUnknownFields(helpers: IDecoderHelpers_1[_JSONVALUE], known_fields: Any, json: _JSONVALUE) -> bool:
     def predicate(x: str, helpers: Any=helpers, known_fields: Any=known_fields, json: Any=json) -> bool:
         return not contains(x, known_fields)
 
     return exists(predicate, helpers.get_properties(json))
 
 
 def Decode_objectNoAdditionalProperties(allowed_properties: IEnumerable_1[str], builder: Callable[[IGetters], _VALUE]) -> Decoder_1[_VALUE]:
-    class ObjectExpr948:
+    class ObjectExpr947:
         @property
         def Compare(self) -> Callable[[str, str], int]:
             return compare_primitives
 
-    allowed_properties_1: Any = of_seq(allowed_properties, ObjectExpr948())
-    class ObjectExpr949(Decoder_1[_VALUE_]):
+    allowed_properties_1: Any = of_seq(allowed_properties, ObjectExpr947())
+    class ObjectExpr948(Decoder_1[_VALUE_]):
         def Decode(self, helpers: IDecoderHelpers_1[__A_], value: __A_, allowed_properties: Any=allowed_properties, builder: Any=builder) -> FSharpResult_2[_VALUE_, tuple[str, ErrorReason_1[__A_]]]:
             getters: Getters_2[__A_, Any] = Getters_2__ctor_Z4BE6C149(helpers, value)
             if Decode_hasUnknownFields(helpers, allowed_properties_1, value):
                 return FSharpResult_2(1, ("Unknown fields in object", ErrorReason_1(0, "", value)))
 
             else: 
                 result: _VALUE_ = builder(getters)
@@ -91,24 +91,24 @@
                     return FSharpResult_2(1, ("", ErrorReason_1(7, errors))) if (length(errors) > 1) else FSharpResult_2(1, head(match_value))
 
                 else: 
                     return FSharpResult_2(0, result)
 
 
 
-    return ObjectExpr949()
+    return ObjectExpr948()
 
 
 def Decode_noAdditionalProperties(allowed_properties: IEnumerable_1[str], decoder: Decoder_1[_VALUE]) -> Decoder_1[_VALUE]:
-    class ObjectExpr950:
+    class ObjectExpr949:
         @property
         def Compare(self) -> Callable[[str, str], int]:
             return compare_primitives
 
-    allowed_properties_1: Any = of_seq(allowed_properties, ObjectExpr950())
+    allowed_properties_1: Any = of_seq(allowed_properties, ObjectExpr949())
     class ObjectExpr951(Decoder_1[_VALUE_]):
         def Decode(self, helpers: IDecoderHelpers_1[__A_], value: __A_, allowed_properties: Any=allowed_properties, decoder: Any=decoder) -> FSharpResult_2[_VALUE_, tuple[str, ErrorReason_1[__A_]]]:
             getters: Getters_2[__A_, Any] = Getters_2__ctor_Z4BE6C149(helpers, value)
             return FSharpResult_2(1, ("Unknown fields in object", ErrorReason_1(0, "", value))) if Decode_hasUnknownFields(helpers, allowed_properties_1, value) else decoder.Decode(helpers, value)
 
     return ObjectExpr951()
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/encode.py` & `arctrl-2.0.0a3/arctrl/Json/encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 
 def try_include_list(name: __A, encoder: Callable[[_VALUE], Json], value: FSharpList[_VALUE]) -> tuple[__A, Json]:
     return (name, Json(3) if is_empty_1(value) else list_1_1(map_2(encoder, value)))
 
 
 def try_include_list_opt(name: __A, encoder: Callable[[_VALUE], Json], value: FSharpList[_VALUE] | None=None) -> tuple[__A, Json]:
-    def _arrow946(__unit: None=None, name: Any=name, encoder: Any=encoder, value: Any=value) -> Json:
+    def _arrow950(__unit: None=None, name: Any=name, encoder: Any=encoder, value: Any=value) -> Json:
         o: FSharpList[_VALUE] = value
         return Json(3) if is_empty_1(o) else list_1_1(map_2(encoder, o))
 
-    return (name, _arrow946() if (value is not None) else Json(3))
+    return (name, _arrow950() if (value is not None) else Json(3))
 
 
 DefaultSpaces: int = 0
 
 def default_spaces(spaces: int | None=None) -> int:
     return default_arg(spaces, DefaultSpaces)
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/investigation.py` & `arctrl-2.0.0a3/arctrl/Json/investigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,217 +39,217 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1684(value_1: str, inv: Any=inv) -> Json:
+    def _arrow1689(value_1: str, inv: Any=inv) -> Json:
         return Json(0, value_1)
 
-    def _arrow1685(value_3: str, inv: Any=inv) -> Json:
+    def _arrow1690(value_3: str, inv: Any=inv) -> Json:
         return Json(0, value_3)
 
-    def _arrow1686(value_5: str, inv: Any=inv) -> Json:
+    def _arrow1691(value_5: str, inv: Any=inv) -> Json:
         return Json(0, value_5)
 
-    def _arrow1687(value_7: str, inv: Any=inv) -> Json:
+    def _arrow1692(value_7: str, inv: Any=inv) -> Json:
         return Json(0, value_7)
 
-    def _arrow1688(osr: OntologySourceReference, inv: Any=inv) -> Json:
+    def _arrow1693(osr: OntologySourceReference, inv: Any=inv) -> Json:
         return OntologySourceReference_encoder(osr)
 
-    def _arrow1689(oa: Publication, inv: Any=inv) -> Json:
+    def _arrow1694(oa: Publication, inv: Any=inv) -> Json:
         return Publication_encoder(oa)
 
-    def _arrow1690(person: Person, inv: Any=inv) -> Json:
+    def _arrow1695(person: Person, inv: Any=inv) -> Json:
         return Person_encoder(person)
 
-    def _arrow1691(assay: ArcAssay, inv: Any=inv) -> Json:
+    def _arrow1696(assay: ArcAssay, inv: Any=inv) -> Json:
         return Assay_encoder(assay)
 
-    def _arrow1692(study: ArcStudy, inv: Any=inv) -> Json:
+    def _arrow1697(study: ArcStudy, inv: Any=inv) -> Json:
         return Study_encoder(study)
 
-    def _arrow1693(value_9: str, inv: Any=inv) -> Json:
+    def _arrow1698(value_9: str, inv: Any=inv) -> Json:
         return Json(0, value_9)
 
-    def _arrow1694(comment: Comment, inv: Any=inv) -> Json:
+    def _arrow1699(comment: Comment, inv: Any=inv) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("Identifier", Json(0, inv.Identifier)), try_include("Title", _arrow1684, inv.Title), try_include("Description", _arrow1685, inv.Description), try_include("SubmissionDate", _arrow1686, inv.SubmissionDate), try_include("PublicReleaseDate", _arrow1687, inv.PublicReleaseDate), try_include_seq("OntologySourceReferences", _arrow1688, inv.OntologySourceReferences), try_include_seq("Publications", _arrow1689, inv.Publications), try_include_seq("Contacts", _arrow1690, inv.Contacts), try_include_seq("Assays", _arrow1691, inv.Assays), try_include_seq("Studies", _arrow1692, inv.Studies), try_include_seq("RegisteredStudyIdentifiers", _arrow1693, inv.RegisteredStudyIdentifiers), try_include_seq("Comments", _arrow1694, inv.Comments)])))
+    return Json(5, choose(chooser, of_array([("Identifier", Json(0, inv.Identifier)), try_include("Title", _arrow1689, inv.Title), try_include("Description", _arrow1690, inv.Description), try_include("SubmissionDate", _arrow1691, inv.SubmissionDate), try_include("PublicReleaseDate", _arrow1692, inv.PublicReleaseDate), try_include_seq("OntologySourceReferences", _arrow1693, inv.OntologySourceReferences), try_include_seq("Publications", _arrow1694, inv.Publications), try_include_seq("Contacts", _arrow1695, inv.Contacts), try_include_seq("Assays", _arrow1696, inv.Assays), try_include_seq("Studies", _arrow1697, inv.Studies), try_include_seq("RegisteredStudyIdentifiers", _arrow1698, inv.RegisteredStudyIdentifiers), try_include_seq("Comments", _arrow1699, inv.Comments)])))
 
 
-def _arrow1707(get: IGetters) -> ArcInvestigation:
-    def _arrow1695(__unit: None=None) -> str:
+def _arrow1712(get: IGetters) -> ArcInvestigation:
+    def _arrow1700(__unit: None=None) -> str:
         object_arg: IRequiredGetter = get.Required
         return object_arg.Field("Identifier", string)
 
-    def _arrow1696(__unit: None=None) -> str | None:
+    def _arrow1701(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("Title", string)
 
-    def _arrow1697(__unit: None=None) -> str | None:
+    def _arrow1702(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("Description", string)
 
-    def _arrow1698(__unit: None=None) -> str | None:
+    def _arrow1703(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("SubmissionDate", string)
 
-    def _arrow1699(__unit: None=None) -> str | None:
+    def _arrow1704(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("PublicReleaseDate", string)
 
-    def _arrow1700(__unit: None=None) -> Array[OntologySourceReference] | None:
+    def _arrow1705(__unit: None=None) -> Array[OntologySourceReference] | None:
         arg_11: Decoder_1[Array[OntologySourceReference]] = Decode_resizeArray(OntologySourceReference_decoder)
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("OntologySourceReferences", arg_11)
 
-    def _arrow1701(__unit: None=None) -> Array[Publication] | None:
+    def _arrow1706(__unit: None=None) -> Array[Publication] | None:
         arg_13: Decoder_1[Array[Publication]] = Decode_resizeArray(Publication_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("Publications", arg_13)
 
-    def _arrow1702(__unit: None=None) -> Array[Person] | None:
+    def _arrow1707(__unit: None=None) -> Array[Person] | None:
         arg_15: Decoder_1[Array[Person]] = Decode_resizeArray(Person_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("Contacts", arg_15)
 
-    def _arrow1703(__unit: None=None) -> Array[ArcAssay] | None:
+    def _arrow1708(__unit: None=None) -> Array[ArcAssay] | None:
         arg_17: Decoder_1[Array[ArcAssay]] = Decode_resizeArray(Assay_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("Assays", arg_17)
 
-    def _arrow1704(__unit: None=None) -> Array[ArcStudy] | None:
+    def _arrow1709(__unit: None=None) -> Array[ArcStudy] | None:
         arg_19: Decoder_1[Array[ArcStudy]] = Decode_resizeArray(Study_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("Studies", arg_19)
 
-    def _arrow1705(__unit: None=None) -> Array[str] | None:
+    def _arrow1710(__unit: None=None) -> Array[str] | None:
         arg_21: Decoder_1[Array[str]] = Decode_resizeArray(string)
         object_arg_10: IOptionalGetter = get.Optional
         return object_arg_10.Field("RegisteredStudyIdentifiers", arg_21)
 
-    def _arrow1706(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1711(__unit: None=None) -> Array[Comment] | None:
         arg_23: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_11: IOptionalGetter = get.Optional
         return object_arg_11.Field("Comments", arg_23)
 
-    return ArcInvestigation(_arrow1695(), _arrow1696(), _arrow1697(), _arrow1698(), _arrow1699(), _arrow1700(), _arrow1701(), _arrow1702(), _arrow1703(), _arrow1704(), _arrow1705(), _arrow1706())
+    return ArcInvestigation(_arrow1700(), _arrow1701(), _arrow1702(), _arrow1703(), _arrow1704(), _arrow1705(), _arrow1706(), _arrow1707(), _arrow1708(), _arrow1709(), _arrow1710(), _arrow1711())
 
 
-Investigation_decoder: Decoder_1[ArcInvestigation] = object(_arrow1707)
+Investigation_decoder: Decoder_1[ArcInvestigation] = object(_arrow1712)
 
 def Investigation_encoderCompressed(string_table: Any, oa_table: Any, cell_table: Any, inv: ArcInvestigation) -> Json:
     def chooser(tupled_arg: tuple[str, Json], string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1708(value_1: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1713(value_1: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Json(0, value_1)
 
-    def _arrow1709(value_3: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1714(value_3: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Json(0, value_3)
 
-    def _arrow1710(value_5: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1715(value_5: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Json(0, value_5)
 
-    def _arrow1711(value_7: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1716(value_7: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Json(0, value_7)
 
-    def _arrow1712(osr: OntologySourceReference, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1718(osr: OntologySourceReference, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return OntologySourceReference_encoder(osr)
 
-    def _arrow1713(oa: Publication, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1719(oa: Publication, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Publication_encoder(oa)
 
-    def _arrow1714(person: Person, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1721(person: Person, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Person_encoder(person)
 
-    def _arrow1715(assay: ArcAssay, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1723(assay: ArcAssay, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Assay_encoderCompressed(string_table, oa_table, cell_table, assay)
 
-    def _arrow1716(study: ArcStudy, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1724(study: ArcStudy, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Study_encoderCompressed(string_table, oa_table, cell_table, study)
 
-    def _arrow1717(value_9: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1725(value_9: str, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Json(0, value_9)
 
-    def _arrow1718(comment: Comment, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
+    def _arrow1726(comment: Comment, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, inv: Any=inv) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("Identifier", Json(0, inv.Identifier)), try_include("Title", _arrow1708, inv.Title), try_include("Description", _arrow1709, inv.Description), try_include("SubmissionDate", _arrow1710, inv.SubmissionDate), try_include("PublicReleaseDate", _arrow1711, inv.PublicReleaseDate), try_include_seq("OntologySourceReferences", _arrow1712, inv.OntologySourceReferences), try_include_seq("Publications", _arrow1713, inv.Publications), try_include_seq("Contacts", _arrow1714, inv.Contacts), try_include_seq("Assays", _arrow1715, inv.Assays), try_include_seq("Studies", _arrow1716, inv.Studies), try_include_seq("RegisteredStudyIdentifiers", _arrow1717, inv.RegisteredStudyIdentifiers), try_include_seq("Comments", _arrow1718, inv.Comments)])))
+    return Json(5, choose(chooser, of_array([("Identifier", Json(0, inv.Identifier)), try_include("Title", _arrow1713, inv.Title), try_include("Description", _arrow1714, inv.Description), try_include("SubmissionDate", _arrow1715, inv.SubmissionDate), try_include("PublicReleaseDate", _arrow1716, inv.PublicReleaseDate), try_include_seq("OntologySourceReferences", _arrow1718, inv.OntologySourceReferences), try_include_seq("Publications", _arrow1719, inv.Publications), try_include_seq("Contacts", _arrow1721, inv.Contacts), try_include_seq("Assays", _arrow1723, inv.Assays), try_include_seq("Studies", _arrow1724, inv.Studies), try_include_seq("RegisteredStudyIdentifiers", _arrow1725, inv.RegisteredStudyIdentifiers), try_include_seq("Comments", _arrow1726, inv.Comments)])))
 
 
 def Investigation_decoderCompressed(string_table: Array[str], oa_table: Array[OntologyAnnotation], cell_table: Array[CompositeCell]) -> Decoder_1[ArcInvestigation]:
-    def _arrow1731(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> ArcInvestigation:
-        def _arrow1719(__unit: None=None) -> str:
+    def _arrow1741(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> ArcInvestigation:
+        def _arrow1729(__unit: None=None) -> str:
             object_arg: IRequiredGetter = get.Required
             return object_arg.Field("Identifier", string)
 
-        def _arrow1720(__unit: None=None) -> str | None:
+        def _arrow1730(__unit: None=None) -> str | None:
             object_arg_1: IOptionalGetter = get.Optional
             return object_arg_1.Field("Title", string)
 
-        def _arrow1721(__unit: None=None) -> str | None:
+        def _arrow1731(__unit: None=None) -> str | None:
             object_arg_2: IOptionalGetter = get.Optional
             return object_arg_2.Field("Description", string)
 
-        def _arrow1722(__unit: None=None) -> str | None:
+        def _arrow1732(__unit: None=None) -> str | None:
             object_arg_3: IOptionalGetter = get.Optional
             return object_arg_3.Field("SubmissionDate", string)
 
-        def _arrow1723(__unit: None=None) -> str | None:
+        def _arrow1733(__unit: None=None) -> str | None:
             object_arg_4: IOptionalGetter = get.Optional
             return object_arg_4.Field("PublicReleaseDate", string)
 
-        def _arrow1724(__unit: None=None) -> Array[OntologySourceReference] | None:
+        def _arrow1734(__unit: None=None) -> Array[OntologySourceReference] | None:
             arg_11: Decoder_1[Array[OntologySourceReference]] = Decode_resizeArray(OntologySourceReference_decoder)
             object_arg_5: IOptionalGetter = get.Optional
             return object_arg_5.Field("OntologySourceReferences", arg_11)
 
-        def _arrow1725(__unit: None=None) -> Array[Publication] | None:
+        def _arrow1735(__unit: None=None) -> Array[Publication] | None:
             arg_13: Decoder_1[Array[Publication]] = Decode_resizeArray(Publication_decoder)
             object_arg_6: IOptionalGetter = get.Optional
             return object_arg_6.Field("Publications", arg_13)
 
-        def _arrow1726(__unit: None=None) -> Array[Person] | None:
+        def _arrow1736(__unit: None=None) -> Array[Person] | None:
             arg_15: Decoder_1[Array[Person]] = Decode_resizeArray(Person_decoder)
             object_arg_7: IOptionalGetter = get.Optional
             return object_arg_7.Field("Contacts", arg_15)
 
-        def _arrow1727(__unit: None=None) -> Array[ArcAssay] | None:
+        def _arrow1737(__unit: None=None) -> Array[ArcAssay] | None:
             arg_17: Decoder_1[Array[ArcAssay]] = Decode_resizeArray(Assay_decoderCompressed(string_table, oa_table, cell_table))
             object_arg_8: IOptionalGetter = get.Optional
             return object_arg_8.Field("Assays", arg_17)
 
-        def _arrow1728(__unit: None=None) -> Array[ArcStudy] | None:
+        def _arrow1738(__unit: None=None) -> Array[ArcStudy] | None:
             arg_19: Decoder_1[Array[ArcStudy]] = Decode_resizeArray(Study_decoderCompressed(string_table, oa_table, cell_table))
             object_arg_9: IOptionalGetter = get.Optional
             return object_arg_9.Field("Studies", arg_19)
 
-        def _arrow1729(__unit: None=None) -> Array[str] | None:
+        def _arrow1739(__unit: None=None) -> Array[str] | None:
             arg_21: Decoder_1[Array[str]] = Decode_resizeArray(string)
             object_arg_10: IOptionalGetter = get.Optional
             return object_arg_10.Field("RegisteredStudyIdentifiers", arg_21)
 
-        def _arrow1730(__unit: None=None) -> Array[Comment] | None:
+        def _arrow1740(__unit: None=None) -> Array[Comment] | None:
             arg_23: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
             object_arg_11: IOptionalGetter = get.Optional
             return object_arg_11.Field("Comments", arg_23)
 
-        return ArcInvestigation(_arrow1719(), _arrow1720(), _arrow1721(), _arrow1722(), _arrow1723(), _arrow1724(), _arrow1725(), _arrow1726(), _arrow1727(), _arrow1728(), _arrow1729(), _arrow1730())
+        return ArcInvestigation(_arrow1729(), _arrow1730(), _arrow1731(), _arrow1732(), _arrow1733(), _arrow1734(), _arrow1735(), _arrow1736(), _arrow1737(), _arrow1738(), _arrow1739(), _arrow1740())
 
-    return object(_arrow1731)
+    return object(_arrow1741)
 
 
 def Investigation_ROCrate_genID(i: ArcInvestigation) -> str:
     return "./"
 
 
 def Investigation_ROCrate_encoder(oa: ArcInvestigation) -> Json:
@@ -258,268 +258,268 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1733(value_5: str, oa: Any=oa) -> Json:
+    def _arrow1742(value_5: str, oa: Any=oa) -> Json:
         return Json(0, value_5)
 
-    def _arrow1734(value_7: str, oa: Any=oa) -> Json:
+    def _arrow1743(value_7: str, oa: Any=oa) -> Json:
         return Json(0, value_7)
 
-    def _arrow1735(value_9: str, oa: Any=oa) -> Json:
+    def _arrow1744(value_9: str, oa: Any=oa) -> Json:
         return Json(0, value_9)
 
-    def _arrow1736(value_11: str, oa: Any=oa) -> Json:
+    def _arrow1745(value_11: str, oa: Any=oa) -> Json:
         return Json(0, value_11)
 
-    def _arrow1737(osr: OntologySourceReference, oa: Any=oa) -> Json:
+    def _arrow1746(osr: OntologySourceReference, oa: Any=oa) -> Json:
         return OntologySourceReference_ROCrate_encoder(osr)
 
-    def _arrow1738(oa_1: Publication, oa: Any=oa) -> Json:
+    def _arrow1747(oa_1: Publication, oa: Any=oa) -> Json:
         return Publication_ROCrate_encoder(oa_1)
 
-    def _arrow1739(oa_2: Person, oa: Any=oa) -> Json:
+    def _arrow1748(oa_2: Person, oa: Any=oa) -> Json:
         return Person_ROCrate_encoder(oa_2)
 
-    def _arrow1740(s: ArcStudy, oa: Any=oa) -> Json:
+    def _arrow1749(s: ArcStudy, oa: Any=oa) -> Json:
         return Study_ROCrate_encoder(None, s)
 
-    def _arrow1745(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow1750(comment: Comment, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Investigation_ROCrate_genID(oa))), ("@type", Json(0, "Investigation")), ("additionalType", Json(0, "Investigation")), ("identifier", Json(0, oa.Identifier)), ("filename", Json(0, ArcInvestigation.FileName())), try_include("title", _arrow1733, oa.Title), try_include("description", _arrow1734, oa.Description), try_include("submissionDate", _arrow1735, oa.SubmissionDate), try_include("publicReleaseDate", _arrow1736, oa.PublicReleaseDate), try_include_seq("ontologySourceReferences", _arrow1737, oa.OntologySourceReferences), try_include_seq("publications", _arrow1738, oa.Publications), try_include_seq("people", _arrow1739, oa.Contacts), try_include_seq("studies", _arrow1740, oa.Studies), try_include_seq("comments", _arrow1745, oa.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Investigation_ROCrate_genID(oa))), ("@type", Json(0, "Investigation")), ("additionalType", Json(0, "Investigation")), ("identifier", Json(0, oa.Identifier)), ("filename", Json(0, ArcInvestigation.FileName())), try_include("title", _arrow1742, oa.Title), try_include("description", _arrow1743, oa.Description), try_include("submissionDate", _arrow1744, oa.SubmissionDate), try_include("publicReleaseDate", _arrow1745, oa.PublicReleaseDate), try_include_seq("ontologySourceReferences", _arrow1746, oa.OntologySourceReferences), try_include_seq("publications", _arrow1747, oa.Publications), try_include_seq("people", _arrow1748, oa.Contacts), try_include_seq("studies", _arrow1749, oa.Studies), try_include_seq("comments", _arrow1750, oa.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow1757(get: IGetters) -> ArcInvestigation:
+def _arrow1762(get: IGetters) -> ArcInvestigation:
     identifier: str
     match_value: str | None
     object_arg: IOptionalGetter = get.Optional
     match_value = object_arg.Field("identifier", string)
     identifier = create_missing_identifier() if (match_value is None) else match_value
-    def _arrow1746(__unit: None=None) -> FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]] | None:
+    def _arrow1751(__unit: None=None) -> FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]] | None:
         arg_3: Decoder_1[FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]]] = list_1_1(Study_ROCrate_decoder)
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("studies", arg_3)
 
-    pattern_input: tuple[FSharpList[ArcStudy], FSharpList[FSharpList[ArcAssay]]] = unzip(default_arg(_arrow1746(), empty()))
+    pattern_input: tuple[FSharpList[ArcStudy], FSharpList[FSharpList[ArcAssay]]] = unzip(default_arg(_arrow1751(), empty()))
     studies_raw: FSharpList[ArcStudy] = pattern_input[0]
     def projection(a: ArcAssay) -> str:
         return a.Identifier
 
-    class ObjectExpr1748:
+    class ObjectExpr1753:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow1747(x: str, y: str) -> bool:
+            def _arrow1752(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow1747
+            return _arrow1752
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    assays: Array[ArcAssay] = list(distinct_by(projection, concat(pattern_input[1]), ObjectExpr1748()))
+    assays: Array[ArcAssay] = list(distinct_by(projection, concat(pattern_input[1]), ObjectExpr1753()))
     studies: Array[ArcStudy] = list(studies_raw)
     def mapping(a_1: ArcStudy) -> str:
         return a_1.Identifier
 
     study_identifiers: Array[str] = list(map(mapping, studies_raw))
-    def _arrow1749(__unit: None=None) -> str | None:
+    def _arrow1754(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("title", string)
 
-    def _arrow1750(__unit: None=None) -> str | None:
+    def _arrow1755(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("description", string)
 
-    def _arrow1751(__unit: None=None) -> str | None:
+    def _arrow1756(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("submissionDate", string)
 
-    def _arrow1752(__unit: None=None) -> str | None:
+    def _arrow1757(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("publicReleaseDate", string)
 
-    def _arrow1753(__unit: None=None) -> Array[OntologySourceReference] | None:
+    def _arrow1758(__unit: None=None) -> Array[OntologySourceReference] | None:
         arg_13: Decoder_1[Array[OntologySourceReference]] = Decode_resizeArray(OntologySourceReference_ROCrate_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("ontologySourceReferences", arg_13)
 
-    def _arrow1754(__unit: None=None) -> Array[Publication] | None:
+    def _arrow1759(__unit: None=None) -> Array[Publication] | None:
         arg_15: Decoder_1[Array[Publication]] = Decode_resizeArray(Publication_ROCrate_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("publications", arg_15)
 
-    def _arrow1755(__unit: None=None) -> Array[Person] | None:
+    def _arrow1760(__unit: None=None) -> Array[Person] | None:
         arg_17: Decoder_1[Array[Person]] = Decode_resizeArray(Person_ROCrate_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("people", arg_17)
 
-    def _arrow1756(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1761(__unit: None=None) -> Array[Comment] | None:
         arg_19: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ROCrate_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("comments", arg_19)
 
-    return ArcInvestigation(identifier, _arrow1749(), _arrow1750(), _arrow1751(), _arrow1752(), _arrow1753(), _arrow1754(), _arrow1755(), assays, studies, study_identifiers, _arrow1756())
+    return ArcInvestigation(identifier, _arrow1754(), _arrow1755(), _arrow1756(), _arrow1757(), _arrow1758(), _arrow1759(), _arrow1760(), assays, studies, study_identifiers, _arrow1761())
 
 
-Investigation_ROCrate_decoder: Decoder_1[ArcInvestigation] = object(_arrow1757)
+Investigation_ROCrate_decoder: Decoder_1[ArcInvestigation] = object(_arrow1762)
 
 def Investigation_ROCrate_encodeRoCrate(oa: ArcInvestigation) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1759(value: str, oa: Any=oa) -> Json:
+    def _arrow1764(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1760(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1765(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1761(oa_1: ArcInvestigation, oa: Any=oa) -> Json:
+    def _arrow1766(oa_1: ArcInvestigation, oa: Any=oa) -> Json:
         return Investigation_ROCrate_encoder(oa_1)
 
-    return Json(5, choose(chooser, of_array([try_include("@type", _arrow1759, "CreativeWork"), try_include("@id", _arrow1760, "ro-crate-metadata.json"), try_include("about", _arrow1761, oa), ("conformsTo", conforms_to_jsonvalue), ("@context", context_jsonvalue_1)])))
+    return Json(5, choose(chooser, of_array([try_include("@type", _arrow1764, "CreativeWork"), try_include("@id", _arrow1765, "ro-crate-metadata.json"), try_include("about", _arrow1766, oa), ("conformsTo", conforms_to_jsonvalue), ("@context", context_jsonvalue_1)])))
 
 
 Investigation_ISAJson_allowedFields: FSharpList[str] = of_array(["@id", "filename", "identifier", "title", "description", "submissionDate", "publicReleaseDate", "ontologySourceReferences", "publications", "people", "studies", "comments", "@type", "@context"])
 
 def Investigation_ISAJson_encoder(inv: ArcInvestigation) -> Json:
     def chooser(tupled_arg: tuple[str, Json], inv: Any=inv) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1762(value_2: str, inv: Any=inv) -> Json:
+    def _arrow1767(value_2: str, inv: Any=inv) -> Json:
         return Json(0, value_2)
 
-    def _arrow1763(value_4: str, inv: Any=inv) -> Json:
+    def _arrow1768(value_4: str, inv: Any=inv) -> Json:
         return Json(0, value_4)
 
-    def _arrow1764(value_6: str, inv: Any=inv) -> Json:
+    def _arrow1769(value_6: str, inv: Any=inv) -> Json:
         return Json(0, value_6)
 
-    def _arrow1765(value_8: str, inv: Any=inv) -> Json:
+    def _arrow1770(value_8: str, inv: Any=inv) -> Json:
         return Json(0, value_8)
 
-    def _arrow1766(oa: Publication, inv: Any=inv) -> Json:
+    def _arrow1771(oa: Publication, inv: Any=inv) -> Json:
         return Publication_ISAJson_encoder(oa)
 
-    def _arrow1767(person: Person, inv: Any=inv) -> Json:
+    def _arrow1772(person: Person, inv: Any=inv) -> Json:
         return Person_ISAJson_encoder(person)
 
-    def _arrow1768(s: ArcStudy, inv: Any=inv) -> Json:
+    def _arrow1773(s: ArcStudy, inv: Any=inv) -> Json:
         return Study_ISAJson_encoder(None, s)
 
-    return Json(5, choose(chooser, of_array([("filename", Json(0, ArcInvestigation.FileName())), ("identifier", Json(0, inv.Identifier)), try_include("title", _arrow1762, inv.Title), try_include("description", _arrow1763, inv.Description), try_include("submissionDate", _arrow1764, inv.SubmissionDate), try_include("publicReleaseDate", _arrow1765, inv.PublicReleaseDate), try_include_seq("ontologySourceReferences", OntologySourceReference_ISAJson_encoder, inv.OntologySourceReferences), try_include_seq("publications", _arrow1766, inv.Publications), try_include_seq("people", _arrow1767, inv.Contacts), try_include_seq("studies", _arrow1768, inv.Studies), try_include_seq("comments", Comment_ISAJson_encoder, inv.Comments)])))
+    return Json(5, choose(chooser, of_array([("filename", Json(0, ArcInvestigation.FileName())), ("identifier", Json(0, inv.Identifier)), try_include("title", _arrow1767, inv.Title), try_include("description", _arrow1768, inv.Description), try_include("submissionDate", _arrow1769, inv.SubmissionDate), try_include("publicReleaseDate", _arrow1770, inv.PublicReleaseDate), try_include_seq("ontologySourceReferences", OntologySourceReference_ISAJson_encoder, inv.OntologySourceReferences), try_include_seq("publications", _arrow1771, inv.Publications), try_include_seq("people", _arrow1772, inv.Contacts), try_include_seq("studies", _arrow1773, inv.Studies), try_include_seq("comments", Comment_ISAJson_encoder, inv.Comments)])))
 
 
-def _arrow1780(get: IGetters) -> ArcInvestigation:
+def _arrow1785(get: IGetters) -> ArcInvestigation:
     identifer: str
     match_value: str | None
     object_arg: IOptionalGetter = get.Optional
     match_value = object_arg.Field("identifier", string)
     identifer = create_missing_identifier() if (match_value is None) else match_value
-    def _arrow1769(__unit: None=None) -> FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]] | None:
+    def _arrow1774(__unit: None=None) -> FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]] | None:
         arg_3: Decoder_1[FSharpList[tuple[ArcStudy, FSharpList[ArcAssay]]]] = list_1_1(Study_ISAJson_decoder)
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("studies", arg_3)
 
-    pattern_input: tuple[FSharpList[ArcStudy], FSharpList[FSharpList[ArcAssay]]] = unzip(default_arg(_arrow1769(), empty()))
+    pattern_input: tuple[FSharpList[ArcStudy], FSharpList[FSharpList[ArcAssay]]] = unzip(default_arg(_arrow1774(), empty()))
     studies_raw: FSharpList[ArcStudy] = pattern_input[0]
     def projection(a: ArcAssay) -> str:
         return a.Identifier
 
-    class ObjectExpr1771:
+    class ObjectExpr1776:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow1770(x: str, y: str) -> bool:
+            def _arrow1775(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow1770
+            return _arrow1775
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    assays: Array[ArcAssay] = list(distinct_by(projection, concat(pattern_input[1]), ObjectExpr1771()))
+    assays: Array[ArcAssay] = list(distinct_by(projection, concat(pattern_input[1]), ObjectExpr1776()))
     studies: Array[ArcStudy] = list(studies_raw)
     def mapping(a_1: ArcStudy) -> str:
         return a_1.Identifier
 
     study_identifiers: Array[str] = list(map(mapping, studies_raw))
-    def _arrow1772(__unit: None=None) -> str | None:
+    def _arrow1777(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("title", string)
 
-    def _arrow1773(__unit: None=None) -> str | None:
+    def _arrow1778(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("description", string)
 
-    def _arrow1774(__unit: None=None) -> str | None:
+    def _arrow1779(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("submissionDate", string)
 
-    def _arrow1775(__unit: None=None) -> str | None:
+    def _arrow1780(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("publicReleaseDate", string)
 
-    def _arrow1776(__unit: None=None) -> Array[OntologySourceReference] | None:
+    def _arrow1781(__unit: None=None) -> Array[OntologySourceReference] | None:
         arg_13: Decoder_1[Array[OntologySourceReference]] = Decode_resizeArray(OntologySourceReference_ISAJson_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("ontologySourceReferences", arg_13)
 
-    def _arrow1777(__unit: None=None) -> Array[Publication] | None:
+    def _arrow1782(__unit: None=None) -> Array[Publication] | None:
         arg_15: Decoder_1[Array[Publication]] = Decode_resizeArray(Publication_ISAJson_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("publications", arg_15)
 
-    def _arrow1778(__unit: None=None) -> Array[Person] | None:
+    def _arrow1783(__unit: None=None) -> Array[Person] | None:
         arg_17: Decoder_1[Array[Person]] = Decode_resizeArray(Person_ISAJson_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("people", arg_17)
 
-    def _arrow1779(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1784(__unit: None=None) -> Array[Comment] | None:
         arg_19: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ISAJson_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("comments", arg_19)
 
-    return ArcInvestigation(identifer, _arrow1772(), _arrow1773(), _arrow1774(), _arrow1775(), _arrow1776(), _arrow1777(), _arrow1778(), assays, studies, study_identifiers, _arrow1779())
+    return ArcInvestigation(identifer, _arrow1777(), _arrow1778(), _arrow1779(), _arrow1780(), _arrow1781(), _arrow1782(), _arrow1783(), assays, studies, study_identifiers, _arrow1784())
 
 
-Investigation_ISAJson_decoder: Decoder_1[ArcInvestigation] = Decode_objectNoAdditionalProperties(Investigation_ISAJson_allowedFields, _arrow1780)
+Investigation_ISAJson_decoder: Decoder_1[ArcInvestigation] = Decode_objectNoAdditionalProperties(Investigation_ISAJson_allowedFields, _arrow1785)
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_fromJsonString_Static_Z721C83C5(s: str) -> ArcInvestigation:
     match_value: FSharpResult_2[ArcInvestigation, str] = Decode_fromString(Investigation_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcInvestigation], str]:
-    def _arrow1781(obj: ArcInvestigation, spaces: Any=spaces) -> str:
+    def _arrow1786(obj: ArcInvestigation, spaces: Any=spaces) -> str:
         value: Json = Investigation_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1781
+    return _arrow1786
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_fromCompressedJsonString_Static_Z721C83C5(s: str) -> ArcInvestigation:
     try: 
         match_value: FSharpResult_2[ArcInvestigation, str] = Decode_fromString(decode(Investigation_decoderCompressed), s)
         if match_value.tag == 1:
             raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
@@ -531,44 +531,44 @@
     except Exception as e_1:
         arg_1: str = str(e_1)
         return to_fail(printf("Error. Unable to parse json string to ArcStudy: %s"))(arg_1)
 
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_toCompressedJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcInvestigation], str]:
-    def _arrow1782(obj: ArcInvestigation, spaces: Any=spaces) -> str:
+    def _arrow1787(obj: ArcInvestigation, spaces: Any=spaces) -> str:
         return to_string(default_arg(spaces, 0), encode(Investigation_encoderCompressed, obj))
 
-    return _arrow1782
+    return _arrow1787
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_fromROCrateJsonString_Static_Z721C83C5(s: str) -> ArcInvestigation:
     match_value: FSharpResult_2[ArcInvestigation, str] = Decode_fromString(Investigation_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcInvestigation], str]:
-    def _arrow1783(obj: ArcInvestigation, spaces: Any=spaces) -> str:
+    def _arrow1788(obj: ArcInvestigation, spaces: Any=spaces) -> str:
         value: Json = Investigation_ROCrate_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1783
+    return _arrow1788
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcInvestigation], str]:
-    def _arrow1784(obj: ArcInvestigation, spaces: Any=spaces) -> str:
+    def _arrow1789(obj: ArcInvestigation, spaces: Any=spaces) -> str:
         value: Json = Investigation_ISAJson_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1784
+    return _arrow1789
 
 
 def ARCtrl_ArcInvestigation__ArcInvestigation_fromISAJsonString_Static_Z721C83C5(s: str) -> ArcInvestigation:
     match_value: FSharpResult_2[ArcInvestigation, str] = Decode_fromString(Investigation_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/ontology_annotation.py` & `arctrl-2.0.0a3/arctrl/Json/ontology_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,83 +159,83 @@
 
     def _arrow991(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
     def _arrow992(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow993(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow994(comment: Comment, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoderDisambiguatingDescription(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologyAnnotation_ROCrate_genID(oa))), ("@type", Json(0, "OntologyAnnotation")), try_include("annotationValue", _arrow990, oa.Name), try_include("termSource", _arrow991, oa.TermSourceREF), try_include("termAccession", _arrow992, oa.TermAccessionNumber), try_include_seq("comments", _arrow993, oa.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologyAnnotation_ROCrate_genID(oa))), ("@type", Json(0, "OntologyAnnotation")), try_include("annotationValue", _arrow990, oa.Name), try_include("termSource", _arrow991, oa.TermSourceREF), try_include("termAccession", _arrow992, oa.TermAccessionNumber), try_include_seq("comments", _arrow994, oa.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow998(get: IGetters) -> OntologyAnnotation:
-    def _arrow994(__unit: None=None) -> str | None:
+def _arrow1004(get: IGetters) -> OntologyAnnotation:
+    def _arrow1000(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("annotationValue", AnnotationValue_decoder)
 
-    def _arrow995(__unit: None=None) -> str | None:
+    def _arrow1001(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("termSource", string)
 
-    def _arrow996(__unit: None=None) -> str | None:
+    def _arrow1002(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("termAccession", string)
 
-    def _arrow997(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1003(__unit: None=None) -> Array[Comment] | None:
         arg_7: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ROCrate_decoderDisambiguatingDescription)
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("comments", arg_7)
 
-    return OntologyAnnotation.create(_arrow994(), _arrow995(), _arrow996(), _arrow997())
+    return OntologyAnnotation.create(_arrow1000(), _arrow1001(), _arrow1002(), _arrow1003())
 
 
-OntologyAnnotation_ROCrate_decoderDefinedTerm: Decoder_1[OntologyAnnotation] = object(_arrow998)
+OntologyAnnotation_ROCrate_decoderDefinedTerm: Decoder_1[OntologyAnnotation] = object(_arrow1004)
 
 def OntologyAnnotation_ROCrate_encoderPropertyValue(oa: OntologyAnnotation) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1004(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1009(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1005(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1011(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1007(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow1013(comment: Comment, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoderDisambiguatingDescription(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologyAnnotation_ROCrate_genID(oa))), ("@type", Json(0, "PropertyValue")), try_include("category", _arrow1004, oa.Name), try_include("categoryCode", _arrow1005, oa.TermAccessionNumber), try_include_seq("comments", _arrow1007, oa.Comments), ("@context", context_jsonvalue_1)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologyAnnotation_ROCrate_genID(oa))), ("@type", Json(0, "PropertyValue")), try_include("category", _arrow1009, oa.Name), try_include("categoryCode", _arrow1011, oa.TermAccessionNumber), try_include_seq("comments", _arrow1013, oa.Comments), ("@context", context_jsonvalue_1)])))
 
 
-def _arrow1015(get: IGetters) -> OntologyAnnotation:
-    def _arrow1009(__unit: None=None) -> str | None:
+def _arrow1020(get: IGetters) -> OntologyAnnotation:
+    def _arrow1014(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("category", string)
 
-    def _arrow1011(__unit: None=None) -> str | None:
+    def _arrow1015(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("categoryCode", string)
 
-    def _arrow1014(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1018(__unit: None=None) -> Array[Comment] | None:
         arg_5: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ROCrate_decoderDisambiguatingDescription)
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("comments", arg_5)
 
-    return OntologyAnnotation.create(_arrow1009(), None, _arrow1011(), _arrow1014())
+    return OntologyAnnotation.create(_arrow1014(), None, _arrow1015(), _arrow1018())
 
 
-OntologyAnnotation_ROCrate_decoderPropertyValue: Decoder_1[OntologyAnnotation] = object(_arrow1015)
+OntologyAnnotation_ROCrate_decoderPropertyValue: Decoder_1[OntologyAnnotation] = object(_arrow1020)
 
 OntologyAnnotation_ISAJson_encoder: Callable[[OntologyAnnotation], Json] = OntologyAnnotation_encoder
 
 OntologyAnnotation_ISAJson_decoder: Decoder_1[OntologyAnnotation] = OntologyAnnotation_decoder
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_fromJsonString_Static_Z721C83C5(s: str) -> OntologyAnnotation:
     match_value: FSharpResult_2[OntologyAnnotation, str] = Decode_fromString(OntologyAnnotation_decoder, s)
@@ -244,45 +244,45 @@
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[OntologyAnnotation], str]:
-    def _arrow1021(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
+    def _arrow1024(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
         value: Json = OntologyAnnotation_encoder(obj)
         return to_string_1(default_spaces(spaces), value)
 
-    return _arrow1021
+    return _arrow1024
 
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_fromROCrateJsonString_Static_Z721C83C5(s: str) -> OntologyAnnotation:
     match_value: FSharpResult_2[OntologyAnnotation, str] = Decode_fromString(OntologyAnnotation_ROCrate_decoderDefinedTerm, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[OntologyAnnotation], str]:
-    def _arrow1024(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
+    def _arrow1028(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
         value: Json = OntologyAnnotation_ROCrate_encoderDefinedTerm(obj)
         return to_string_1(default_spaces(spaces), value)
 
-    return _arrow1024
+    return _arrow1028
 
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[OntologyAnnotation], str]:
-    def _arrow1026(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
+    def _arrow1031(obj: OntologyAnnotation, spaces: Any=spaces) -> str:
         value: Json = OntologyAnnotation_ISAJson_encoder(obj)
         return to_string_1(default_spaces(spaces), value)
 
-    return _arrow1026
+    return _arrow1031
 
 
 def ARCtrl_OntologyAnnotation__OntologyAnnotation_fromISAJsonString_Static_Z721C83C5(s: str) -> OntologyAnnotation:
     match_value: FSharpResult_2[OntologyAnnotation, str] = Decode_fromString(OntologyAnnotation_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/ontology_source_reference.py` & `arctrl-2.0.0a3/arctrl/Json/ontology_source_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,58 +23,58 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1000(value: str, osr: Any=osr) -> Json:
+    def _arrow995(value: str, osr: Any=osr) -> Json:
         return Json(0, value)
 
-    def _arrow1001(value_2: str, osr: Any=osr) -> Json:
+    def _arrow996(value_2: str, osr: Any=osr) -> Json:
         return Json(0, value_2)
 
-    def _arrow1002(value_4: str, osr: Any=osr) -> Json:
+    def _arrow997(value_4: str, osr: Any=osr) -> Json:
         return Json(0, value_4)
 
-    def _arrow1003(value_6: str, osr: Any=osr) -> Json:
+    def _arrow998(value_6: str, osr: Any=osr) -> Json:
         return Json(0, value_6)
 
-    def _arrow1006(comment: Comment, osr: Any=osr) -> Json:
+    def _arrow999(comment: Comment, osr: Any=osr) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([try_include("description", _arrow1000, osr.Description), try_include("file", _arrow1001, osr.File), try_include("name", _arrow1002, osr.Name), try_include("version", _arrow1003, osr.Version), try_include_seq("comments", _arrow1006, osr.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("description", _arrow995, osr.Description), try_include("file", _arrow996, osr.File), try_include("name", _arrow997, osr.Name), try_include("version", _arrow998, osr.Version), try_include_seq("comments", _arrow999, osr.Comments)])))
 
 
-def _arrow1017(get: IGetters) -> OntologySourceReference:
-    def _arrow1008(__unit: None=None) -> str | None:
+def _arrow1012(get: IGetters) -> OntologySourceReference:
+    def _arrow1005(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("description", Decode_uri)
 
-    def _arrow1010(__unit: None=None) -> str | None:
+    def _arrow1006(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("file", string)
 
-    def _arrow1012(__unit: None=None) -> str | None:
+    def _arrow1007(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("name", string)
 
-    def _arrow1013(__unit: None=None) -> str | None:
+    def _arrow1008(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("version", string)
 
-    def _arrow1016(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1010(__unit: None=None) -> Array[Comment] | None:
         arg_9: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("comments", arg_9)
 
-    return OntologySourceReference(_arrow1008(), _arrow1010(), _arrow1012(), _arrow1013(), _arrow1016())
+    return OntologySourceReference(_arrow1005(), _arrow1006(), _arrow1007(), _arrow1008(), _arrow1010())
 
 
-OntologySourceReference_decoder: Decoder_1[OntologySourceReference] = object(_arrow1017)
+OntologySourceReference_decoder: Decoder_1[OntologySourceReference] = object(_arrow1012)
 
 def OntologySourceReference_ROCrate_genID(o: OntologySourceReference) -> str:
     match_value: str | None = o.File
     if match_value is None:
         match_value_1: str | None = o.Name
         if match_value_1 is None:
             return "#DummyOntologySourceRef"
@@ -94,58 +94,58 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1018(value_2: str, osr: Any=osr) -> Json:
+    def _arrow1016(value_2: str, osr: Any=osr) -> Json:
         return Json(0, value_2)
 
-    def _arrow1019(value_4: str, osr: Any=osr) -> Json:
+    def _arrow1017(value_4: str, osr: Any=osr) -> Json:
         return Json(0, value_4)
 
-    def _arrow1020(value_6: str, osr: Any=osr) -> Json:
+    def _arrow1019(value_6: str, osr: Any=osr) -> Json:
         return Json(0, value_6)
 
-    def _arrow1022(value_8: str, osr: Any=osr) -> Json:
+    def _arrow1021(value_8: str, osr: Any=osr) -> Json:
         return Json(0, value_8)
 
-    def _arrow1023(comment: Comment, osr: Any=osr) -> Json:
+    def _arrow1022(comment: Comment, osr: Any=osr) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologySourceReference_ROCrate_genID(osr))), ("@type", Json(0, "OntologySourceReference")), try_include("description", _arrow1018, osr.Description), try_include("file", _arrow1019, osr.File), try_include("name", _arrow1020, osr.Name), try_include("version", _arrow1022, osr.Version), try_include_seq("comments", _arrow1023, osr.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, OntologySourceReference_ROCrate_genID(osr))), ("@type", Json(0, "OntologySourceReference")), try_include("description", _arrow1016, osr.Description), try_include("file", _arrow1017, osr.File), try_include("name", _arrow1019, osr.Name), try_include("version", _arrow1021, osr.Version), try_include_seq("comments", _arrow1022, osr.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow1031(get: IGetters) -> OntologySourceReference:
-    def _arrow1025(__unit: None=None) -> str | None:
+def _arrow1030(get: IGetters) -> OntologySourceReference:
+    def _arrow1023(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("description", Decode_uri)
 
-    def _arrow1027(__unit: None=None) -> str | None:
+    def _arrow1025(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("file", string)
 
-    def _arrow1028(__unit: None=None) -> str | None:
+    def _arrow1026(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("name", string)
 
-    def _arrow1029(__unit: None=None) -> str | None:
+    def _arrow1027(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("version", string)
 
-    def _arrow1030(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1029(__unit: None=None) -> Array[Comment] | None:
         arg_9: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("comments", arg_9)
 
-    return OntologySourceReference(_arrow1025(), _arrow1027(), _arrow1028(), _arrow1029(), _arrow1030())
+    return OntologySourceReference(_arrow1023(), _arrow1025(), _arrow1026(), _arrow1027(), _arrow1029())
 
 
-OntologySourceReference_ROCrate_decoder: Decoder_1[OntologySourceReference] = object(_arrow1031)
+OntologySourceReference_ROCrate_decoder: Decoder_1[OntologySourceReference] = object(_arrow1030)
 
 OntologySourceReference_ISAJson_encoder: Callable[[OntologySourceReference], Json] = OntologySourceReference_encoder
 
 OntologySourceReference_ISAJson_decoder: Decoder_1[OntologySourceReference] = OntologySourceReference_decoder
 
 def ARCtrl_OntologySourceReference__OntologySourceReference_fromJsonString_Static_Z721C83C5(s: str) -> OntologySourceReference:
     match_value: FSharpResult_2[OntologySourceReference, str] = Decode_fromString(OntologySourceReference_decoder, s)
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/person.py` & `arctrl-2.0.0a3/arctrl/Json/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,101 +30,101 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1078(value: str, person: Any=person) -> Json:
+    def _arrow1042(value: str, person: Any=person) -> Json:
         return Json(0, value)
 
-    def _arrow1079(value_2: str, person: Any=person) -> Json:
+    def _arrow1043(value_2: str, person: Any=person) -> Json:
         return Json(0, value_2)
 
-    def _arrow1080(value_4: str, person: Any=person) -> Json:
+    def _arrow1044(value_4: str, person: Any=person) -> Json:
         return Json(0, value_4)
 
-    def _arrow1081(value_6: str, person: Any=person) -> Json:
+    def _arrow1045(value_6: str, person: Any=person) -> Json:
         return Json(0, value_6)
 
-    def _arrow1082(value_8: str, person: Any=person) -> Json:
+    def _arrow1046(value_8: str, person: Any=person) -> Json:
         return Json(0, value_8)
 
-    def _arrow1083(value_10: str, person: Any=person) -> Json:
+    def _arrow1047(value_10: str, person: Any=person) -> Json:
         return Json(0, value_10)
 
-    def _arrow1084(value_12: str, person: Any=person) -> Json:
+    def _arrow1048(value_12: str, person: Any=person) -> Json:
         return Json(0, value_12)
 
-    def _arrow1085(value_14: str, person: Any=person) -> Json:
+    def _arrow1049(value_14: str, person: Any=person) -> Json:
         return Json(0, value_14)
 
-    def _arrow1086(value_16: str, person: Any=person) -> Json:
+    def _arrow1050(value_16: str, person: Any=person) -> Json:
         return Json(0, value_16)
 
-    def _arrow1087(oa: OntologyAnnotation, person: Any=person) -> Json:
+    def _arrow1051(oa: OntologyAnnotation, person: Any=person) -> Json:
         return OntologyAnnotation_encoder(oa)
 
-    def _arrow1088(comment: Comment, person: Any=person) -> Json:
+    def _arrow1052(comment: Comment, person: Any=person) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([try_include("firstName", _arrow1078, person.FirstName), try_include("lastName", _arrow1079, person.LastName), try_include("midInitials", _arrow1080, person.MidInitials), try_include("orcid", _arrow1081, person.ORCID), try_include("email", _arrow1082, person.EMail), try_include("phone", _arrow1083, person.Phone), try_include("fax", _arrow1084, person.Fax), try_include("address", _arrow1085, person.Address), try_include("affiliation", _arrow1086, person.Affiliation), try_include_seq("roles", _arrow1087, person.Roles), try_include_seq("comments", _arrow1088, person.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("firstName", _arrow1042, person.FirstName), try_include("lastName", _arrow1043, person.LastName), try_include("midInitials", _arrow1044, person.MidInitials), try_include("orcid", _arrow1045, person.ORCID), try_include("email", _arrow1046, person.EMail), try_include("phone", _arrow1047, person.Phone), try_include("fax", _arrow1048, person.Fax), try_include("address", _arrow1049, person.Address), try_include("affiliation", _arrow1050, person.Affiliation), try_include_seq("roles", _arrow1051, person.Roles), try_include_seq("comments", _arrow1052, person.Comments)])))
 
 
-def _arrow1100(get: IGetters) -> Person:
-    def _arrow1089(__unit: None=None) -> str | None:
+def _arrow1064(get: IGetters) -> Person:
+    def _arrow1053(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("orcid", string)
 
-    def _arrow1090(__unit: None=None) -> str | None:
+    def _arrow1054(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("lastName", string)
 
-    def _arrow1091(__unit: None=None) -> str | None:
+    def _arrow1055(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("firstName", string)
 
-    def _arrow1092(__unit: None=None) -> str | None:
+    def _arrow1056(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("midInitials", string)
 
-    def _arrow1093(__unit: None=None) -> str | None:
+    def _arrow1057(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("email", string)
 
-    def _arrow1094(__unit: None=None) -> str | None:
+    def _arrow1058(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("phone", string)
 
-    def _arrow1095(__unit: None=None) -> str | None:
+    def _arrow1059(__unit: None=None) -> str | None:
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("fax", string)
 
-    def _arrow1096(__unit: None=None) -> str | None:
+    def _arrow1060(__unit: None=None) -> str | None:
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("address", string)
 
-    def _arrow1097(__unit: None=None) -> str | None:
+    def _arrow1061(__unit: None=None) -> str | None:
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("affiliation", string)
 
-    def _arrow1098(__unit: None=None) -> Array[OntologyAnnotation] | None:
+    def _arrow1062(__unit: None=None) -> Array[OntologyAnnotation] | None:
         arg_19: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("roles", arg_19)
 
-    def _arrow1099(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1063(__unit: None=None) -> Array[Comment] | None:
         arg_21: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_10: IOptionalGetter = get.Optional
         return object_arg_10.Field("comments", arg_21)
 
-    return Person(_arrow1089(), _arrow1090(), _arrow1091(), _arrow1092(), _arrow1093(), _arrow1094(), _arrow1095(), _arrow1096(), _arrow1097(), _arrow1098(), _arrow1099())
+    return Person(_arrow1053(), _arrow1054(), _arrow1055(), _arrow1056(), _arrow1057(), _arrow1058(), _arrow1059(), _arrow1060(), _arrow1061(), _arrow1062(), _arrow1063())
 
 
-Person_decoder: Decoder_1[Person] = object(_arrow1100)
+Person_decoder: Decoder_1[Person] = object(_arrow1064)
 
 def Person_ROCrate_genID(p: Person) -> str:
     def chooser(c: Comment, p: Any=p) -> str | None:
         matchValue: str | None = c.Name
         matchValue_1: str | None = c.Value
         (pattern_matching_result, n, v) = (None, None, None)
         if matchValue is not None:
@@ -219,291 +219,291 @@
 
 
 
 def Person_ROCrate_Affiliation_encoder(affiliation: str) -> Json:
     return Json(5, to_enumerable([("@type", Json(0, "Organization")), ("@id", Json(0, replace(("#Organization_" + affiliation) + "", " ", "_"))), ("name", Json(0, affiliation)), ("@context", context_jsonvalue)]))
 
 
-def _arrow1101(get: IGetters) -> str:
+def _arrow1065(get: IGetters) -> str:
     object_arg: IRequiredGetter = get.Required
     return object_arg.Field("name", string)
 
 
-Person_ROCrate_Affiliation_decoder: Decoder_1[str] = object(_arrow1101)
+Person_ROCrate_Affiliation_decoder: Decoder_1[str] = object(_arrow1065)
 
 def Person_ROCrate_encoder(oa: Person) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1102(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1066(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1103(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1067(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1104(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1068(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1105(value_8: str, oa: Any=oa) -> Json:
+    def _arrow1069(value_8: str, oa: Any=oa) -> Json:
         return Json(0, value_8)
 
-    def _arrow1106(value_10: str, oa: Any=oa) -> Json:
+    def _arrow1070(value_10: str, oa: Any=oa) -> Json:
         return Json(0, value_10)
 
-    def _arrow1107(value_12: str, oa: Any=oa) -> Json:
+    def _arrow1071(value_12: str, oa: Any=oa) -> Json:
         return Json(0, value_12)
 
-    def _arrow1108(value_14: str, oa: Any=oa) -> Json:
+    def _arrow1072(value_14: str, oa: Any=oa) -> Json:
         return Json(0, value_14)
 
-    def _arrow1109(value_16: str, oa: Any=oa) -> Json:
+    def _arrow1073(value_16: str, oa: Any=oa) -> Json:
         return Json(0, value_16)
 
-    def _arrow1110(affiliation: str, oa: Any=oa) -> Json:
+    def _arrow1074(affiliation: str, oa: Any=oa) -> Json:
         return Person_ROCrate_Affiliation_encoder(affiliation)
 
-    def _arrow1111(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
+    def _arrow1075(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
         return OntologyAnnotation_ROCrate_encoderDefinedTerm(oa_1)
 
-    def _arrow1112(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow1076(comment: Comment, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoderDisambiguatingDescription(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Person_ROCrate_genID(oa))), ("@type", Json(0, "Person")), try_include("orcid", _arrow1102, oa.ORCID), try_include("firstName", _arrow1103, oa.FirstName), try_include("lastName", _arrow1104, oa.LastName), try_include("midInitials", _arrow1105, oa.MidInitials), try_include("email", _arrow1106, oa.EMail), try_include("phone", _arrow1107, oa.Phone), try_include("fax", _arrow1108, oa.Fax), try_include("address", _arrow1109, oa.Address), try_include("affiliation", _arrow1110, oa.Affiliation), try_include_seq("roles", _arrow1111, oa.Roles), try_include_seq("comments", _arrow1112, oa.Comments), ("@context", context_jsonvalue_1)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Person_ROCrate_genID(oa))), ("@type", Json(0, "Person")), try_include("orcid", _arrow1066, oa.ORCID), try_include("firstName", _arrow1067, oa.FirstName), try_include("lastName", _arrow1068, oa.LastName), try_include("midInitials", _arrow1069, oa.MidInitials), try_include("email", _arrow1070, oa.EMail), try_include("phone", _arrow1071, oa.Phone), try_include("fax", _arrow1072, oa.Fax), try_include("address", _arrow1073, oa.Address), try_include("affiliation", _arrow1074, oa.Affiliation), try_include_seq("roles", _arrow1075, oa.Roles), try_include_seq("comments", _arrow1076, oa.Comments), ("@context", context_jsonvalue_1)])))
 
 
-def _arrow1124(get: IGetters) -> Person:
-    def _arrow1113(__unit: None=None) -> str | None:
+def _arrow1095(get: IGetters) -> Person:
+    def _arrow1077(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("orcid", string)
 
-    def _arrow1114(__unit: None=None) -> str | None:
+    def _arrow1078(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("lastName", string)
 
-    def _arrow1115(__unit: None=None) -> str | None:
+    def _arrow1079(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("firstName", string)
 
-    def _arrow1116(__unit: None=None) -> str | None:
+    def _arrow1080(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("midInitials", string)
 
-    def _arrow1117(__unit: None=None) -> str | None:
+    def _arrow1081(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("email", string)
 
-    def _arrow1118(__unit: None=None) -> str | None:
+    def _arrow1082(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("phone", string)
 
-    def _arrow1119(__unit: None=None) -> str | None:
+    def _arrow1084(__unit: None=None) -> str | None:
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("fax", string)
 
-    def _arrow1120(__unit: None=None) -> str | None:
+    def _arrow1085(__unit: None=None) -> str | None:
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("address", string)
 
-    def _arrow1121(__unit: None=None) -> str | None:
+    def _arrow1087(__unit: None=None) -> str | None:
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("affiliation", Person_ROCrate_Affiliation_decoder)
 
-    def _arrow1122(__unit: None=None) -> Array[OntologyAnnotation] | None:
+    def _arrow1091(__unit: None=None) -> Array[OntologyAnnotation] | None:
         arg_19: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_ROCrate_decoderDefinedTerm)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("roles", arg_19)
 
-    def _arrow1123(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1093(__unit: None=None) -> Array[Comment] | None:
         arg_21: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ROCrate_decoderDisambiguatingDescription)
         object_arg_10: IOptionalGetter = get.Optional
         return object_arg_10.Field("comments", arg_21)
 
-    return Person(_arrow1113(), _arrow1114(), _arrow1115(), _arrow1116(), _arrow1117(), _arrow1118(), _arrow1119(), _arrow1120(), _arrow1121(), _arrow1122(), _arrow1123())
+    return Person(_arrow1077(), _arrow1078(), _arrow1079(), _arrow1080(), _arrow1081(), _arrow1082(), _arrow1084(), _arrow1085(), _arrow1087(), _arrow1091(), _arrow1093())
 
 
-Person_ROCrate_decoder: Decoder_1[Person] = object(_arrow1124)
+Person_ROCrate_decoder: Decoder_1[Person] = object(_arrow1095)
 
 def Person_ROCrate_encodeAuthorListString(author_list: str) -> Json:
     def encode_single(name: str, author_list: Any=author_list) -> Json:
         def chooser(tupled_arg: tuple[str, Json], name: Any=name) -> tuple[str, Json] | None:
             v: Json = tupled_arg[1]
             if equals(v, Json(3)):
                 return None
 
             else: 
                 return (tupled_arg[0], v)
 
 
-        def _arrow1125(value_1: str, name: Any=name) -> Json:
+        def _arrow1096(value_1: str, name: Any=name) -> Json:
             return Json(0, value_1)
 
-        return Json(5, choose(chooser, of_array([("@type", Json(0, "Person")), try_include("name", _arrow1125, name), ("@context", context_minimal_json_value)])))
+        return Json(5, choose(chooser, of_array([("@type", Json(0, "Person")), try_include("name", _arrow1096, name), ("@context", context_minimal_json_value)])))
 
     def mapping(s: str, author_list: Any=author_list) -> str:
         return s.strip()
 
     return Json(6, map(encode_single, map(mapping, split(author_list, ["\t" if (author_list.find("\t") >= 0) else (";" if (author_list.find(";") >= 0) else ",")], None, 0), None), None))
 
 
 def ctor(v: Array[str]) -> str:
     return join(", ", v)
 
 
-def _arrow1127(get: IGetters) -> str:
-    def _arrow1126(__unit: None=None) -> str | None:
+def _arrow1102(get: IGetters) -> str:
+    def _arrow1101(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("name", string)
 
-    return default_arg(_arrow1126(), "")
+    return default_arg(_arrow1101(), "")
 
 
-Person_ROCrate_decodeAuthorListString: Decoder_1[str] = map_1(ctor, array_2(object(_arrow1127)))
+Person_ROCrate_decodeAuthorListString: Decoder_1[str] = map_1(ctor, array_2(object(_arrow1102)))
 
 Person_ISAJson_allowedFields: FSharpList[str] = of_array(["@id", "firstName", "lastName", "midInitials", "email", "phone", "fax", "address", "affiliation", "roles", "comments", "@type", "@context"])
 
 def Person_ISAJson_encoder(person: Person) -> Json:
     person_1: Person = Person_setCommentFromORCID(person)
     def chooser(tupled_arg: tuple[str, Json], person: Any=person) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1129(value: str, person: Any=person) -> Json:
+    def _arrow1107(value: str, person: Any=person) -> Json:
         return Json(0, value)
 
-    def _arrow1130(value_2: str, person: Any=person) -> Json:
+    def _arrow1108(value_2: str, person: Any=person) -> Json:
         return Json(0, value_2)
 
-    def _arrow1131(value_4: str, person: Any=person) -> Json:
+    def _arrow1109(value_4: str, person: Any=person) -> Json:
         return Json(0, value_4)
 
-    def _arrow1132(value_6: str, person: Any=person) -> Json:
+    def _arrow1110(value_6: str, person: Any=person) -> Json:
         return Json(0, value_6)
 
-    def _arrow1133(value_8: str, person: Any=person) -> Json:
+    def _arrow1111(value_8: str, person: Any=person) -> Json:
         return Json(0, value_8)
 
-    def _arrow1134(value_10: str, person: Any=person) -> Json:
+    def _arrow1113(value_10: str, person: Any=person) -> Json:
         return Json(0, value_10)
 
-    def _arrow1135(value_12: str, person: Any=person) -> Json:
+    def _arrow1115(value_12: str, person: Any=person) -> Json:
         return Json(0, value_12)
 
-    def _arrow1136(value_14: str, person: Any=person) -> Json:
+    def _arrow1117(value_14: str, person: Any=person) -> Json:
         return Json(0, value_14)
 
-    def _arrow1137(oa: OntologyAnnotation, person: Any=person) -> Json:
+    def _arrow1119(oa: OntologyAnnotation, person: Any=person) -> Json:
         return OntologyAnnotation_encoder(oa)
 
-    def _arrow1138(comment: Comment, person: Any=person) -> Json:
+    def _arrow1121(comment: Comment, person: Any=person) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([try_include("firstName", _arrow1129, person_1.FirstName), try_include("lastName", _arrow1130, person_1.LastName), try_include("midInitials", _arrow1131, person_1.MidInitials), try_include("email", _arrow1132, person_1.EMail), try_include("phone", _arrow1133, person_1.Phone), try_include("fax", _arrow1134, person_1.Fax), try_include("address", _arrow1135, person_1.Address), try_include("affiliation", _arrow1136, person_1.Affiliation), try_include_seq("roles", _arrow1137, person_1.Roles), try_include_seq("comments", _arrow1138, person_1.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("firstName", _arrow1107, person_1.FirstName), try_include("lastName", _arrow1108, person_1.LastName), try_include("midInitials", _arrow1109, person_1.MidInitials), try_include("email", _arrow1110, person_1.EMail), try_include("phone", _arrow1111, person_1.Phone), try_include("fax", _arrow1113, person_1.Fax), try_include("address", _arrow1115, person_1.Address), try_include("affiliation", _arrow1117, person_1.Affiliation), try_include_seq("roles", _arrow1119, person_1.Roles), try_include_seq("comments", _arrow1121, person_1.Comments)])))
 
 
-def _arrow1149(get: IGetters) -> Person:
-    def _arrow1139(__unit: None=None) -> str | None:
+def _arrow1141(get: IGetters) -> Person:
+    def _arrow1124(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("lastName", string)
 
-    def _arrow1140(__unit: None=None) -> str | None:
+    def _arrow1126(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("firstName", string)
 
-    def _arrow1141(__unit: None=None) -> str | None:
+    def _arrow1129(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("midInitials", string)
 
-    def _arrow1142(__unit: None=None) -> str | None:
+    def _arrow1130(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("email", string)
 
-    def _arrow1143(__unit: None=None) -> str | None:
+    def _arrow1132(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("phone", string)
 
-    def _arrow1144(__unit: None=None) -> str | None:
+    def _arrow1133(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("fax", string)
 
-    def _arrow1145(__unit: None=None) -> str | None:
+    def _arrow1134(__unit: None=None) -> str | None:
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("address", string)
 
-    def _arrow1146(__unit: None=None) -> str | None:
+    def _arrow1137(__unit: None=None) -> str | None:
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("affiliation", string)
 
-    def _arrow1147(__unit: None=None) -> Array[OntologyAnnotation] | None:
+    def _arrow1138(__unit: None=None) -> Array[OntologyAnnotation] | None:
         arg_17: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("roles", arg_17)
 
-    def _arrow1148(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1140(__unit: None=None) -> Array[Comment] | None:
         arg_19: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("comments", arg_19)
 
-    return Person_setOrcidFromComments(Person(None, _arrow1139(), _arrow1140(), _arrow1141(), _arrow1142(), _arrow1143(), _arrow1144(), _arrow1145(), _arrow1146(), _arrow1147(), _arrow1148()))
+    return Person_setOrcidFromComments(Person(None, _arrow1124(), _arrow1126(), _arrow1129(), _arrow1130(), _arrow1132(), _arrow1133(), _arrow1134(), _arrow1137(), _arrow1138(), _arrow1140()))
 
 
-Person_ISAJson_decoder: Decoder_1[Person] = Decode_objectNoAdditionalProperties(Person_ISAJson_allowedFields, _arrow1149)
+Person_ISAJson_decoder: Decoder_1[Person] = Decode_objectNoAdditionalProperties(Person_ISAJson_allowedFields, _arrow1141)
 
 def ARCtrl_Person__Person_fromJsonString_Static_Z721C83C5(s: str) -> Person:
     match_value: FSharpResult_2[Person, str] = Decode_fromString(Person_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Person__Person_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Person], str]:
-    def _arrow1150(obj: Person, spaces: Any=spaces) -> str:
+    def _arrow1147(obj: Person, spaces: Any=spaces) -> str:
         value: Json = Person_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1150
+    return _arrow1147
 
 
 def ARCtrl_Person__Person_fromROCrateJsonString_Static_Z721C83C5(s: str) -> Person:
     match_value: FSharpResult_2[Person, str] = Decode_fromString(Person_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Person__Person_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Person], str]:
-    def _arrow1151(obj: Person, spaces: Any=spaces) -> str:
+    def _arrow1148(obj: Person, spaces: Any=spaces) -> str:
         value: Json = Person_ROCrate_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1151
+    return _arrow1148
 
 
 def ARCtrl_Person__Person_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Person], str]:
-    def _arrow1152(obj: Person, spaces: Any=spaces) -> str:
+    def _arrow1150(obj: Person, spaces: Any=spaces) -> str:
         value: Json = Person_ISAJson_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1152
+    return _arrow1150
 
 
 def ARCtrl_Person__Person_fromISAJsonString_Static_Z721C83C5(s: str) -> Person:
     match_value: FSharpResult_2[Person, str] = Decode_fromString(Person_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/assay_materials.py` & `arctrl-2.0.0a3/arctrl/Json/Process/assay_materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1361(oa: Sample, ps: Any=ps) -> Json:
+    def _arrow1364(oa: Sample, ps: Any=ps) -> Json:
         return Sample_ISAJson_encoder(oa)
 
-    def _arrow1362(oa_1: Material, ps: Any=ps) -> Json:
+    def _arrow1365(oa_1: Material, ps: Any=ps) -> Json:
         return Material_ISAJson_encoder(oa_1)
 
-    return Json(5, choose(chooser, of_array([try_include_list("samples", _arrow1361, samples), try_include_list("otherMaterials", _arrow1362, materials)])))
+    return Json(5, choose(chooser, of_array([try_include_list("samples", _arrow1364, samples), try_include_list("otherMaterials", _arrow1365, materials)])))
 
 
 __all__ = ["encoder"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/component.py` & `arctrl-2.0.0a3/arctrl/Json/Process/component.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/data.py` & `arctrl-2.0.0a3/arctrl/Json/Process/data.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/data_file.py` & `arctrl-2.0.0a3/arctrl/Json/Process/data_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return Json(0, "Image File")
 
     else: 
         return Json(0, "Raw Data File")
 
 
 
-class ObjectExpr1247(Decoder_1[DataFile]):
+class ObjectExpr1233(Decoder_1[DataFile]):
     def Decode(self, s: IDecoderHelpers_1[__A_], json: __A_) -> FSharpResult_2[DataFile, tuple[str, ErrorReason_1[__A_]]]:
         match_value: FSharpResult_2[str, tuple[str, ErrorReason_1[__A_]]] = string.Decode(s, json)
         if match_value.tag == 1:
             return FSharpResult_2(1, match_value.fields[0])
 
         elif match_value.fields[0] == "Raw Data File":
             return FSharpResult_2(0, DataFile(0))
@@ -41,15 +41,15 @@
 
         else: 
             s_1: str = match_value.fields[0]
             return FSharpResult_2(1, (("Could not parse " + s_1) + ".", ErrorReason_1(0, s_1, json)))
 
 
 
-DataFile_ROCrate_decoder: Decoder_1[DataFile] = ObjectExpr1247()
+DataFile_ROCrate_decoder: Decoder_1[DataFile] = ObjectExpr1233()
 
 DataFile_ISAJson_encoder: Callable[[DataFile], Json] = DataFile_ROCrate_encoder
 
 DataFile_ISAJson_decoder: Decoder_1[DataFile] = DataFile_ROCrate_decoder
 
 def ARCtrl_Process_DataFile__DataFile_fromISAJsonString_Static_Z721C83C5(s: str) -> DataFile:
     match_value: FSharpResult_2[DataFile, str] = Decode_fromString(DataFile_ISAJson_decoder, s)
@@ -58,34 +58,34 @@
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_DataFile__DataFile_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[DataFile], str]:
-    def _arrow1248(f: DataFile, spaces: Any=spaces) -> str:
+    def _arrow1234(f: DataFile, spaces: Any=spaces) -> str:
         value: Json = DataFile_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1248
+    return _arrow1234
 
 
 def ARCtrl_Process_DataFile__DataFile_fromROCrateJsonString_Static_Z721C83C5(s: str) -> DataFile:
     match_value: FSharpResult_2[DataFile, str] = Decode_fromString(DataFile_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_DataFile__DataFile_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[DataFile], str]:
-    def _arrow1251(f: DataFile, spaces: Any=spaces) -> str:
+    def _arrow1235(f: DataFile, spaces: Any=spaces) -> str:
         value: Json = DataFile_ROCrate_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1251
+    return _arrow1235
 
 
 __all__ = ["DataFile_ROCrate_encoder", "DataFile_ROCrate_decoder", "DataFile_ISAJson_encoder", "DataFile_ISAJson_decoder", "ARCtrl_Process_DataFile__DataFile_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_DataFile__DataFile_toISAJsonString_Static_71136F3F", "ARCtrl_Process_DataFile__DataFile_fromROCrateJsonString_Static_Z721C83C5", "ARCtrl_Process_DataFile__DataFile_toROCrateJsonString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/factor.py` & `arctrl-2.0.0a3/arctrl/Json/Process/factor.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/factor_value.py` & `arctrl-2.0.0a3/arctrl/Json/Process/factor_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/material.py` & `arctrl-2.0.0a3/arctrl/Json/Process/material.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,152 +41,152 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1249(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1209(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1250(value_4: MaterialType, oa: Any=oa) -> Json:
+    def _arrow1210(value_4: MaterialType, oa: Any=oa) -> Json:
         return MaterialType_ROCrate_encoder(value_4)
 
-    def _arrow1252(oa_1: Material, oa: Any=oa) -> Json:
+    def _arrow1211(oa_1: Material, oa: Any=oa) -> Json:
         return Material_ROCrate_encoder(oa_1)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Material_ROCrate_genID(oa))), ("@type", list_1_1(singleton(Json(0, "Material")))), try_include("name", _arrow1249, oa.Name), try_include("type", _arrow1250, oa.MaterialType), try_include_list_opt("characteristics", MaterialAttributeValue_ROCrate_encoder, oa.Characteristics), try_include_list_opt("derivesFrom", _arrow1252, oa.DerivesFrom), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Material_ROCrate_genID(oa))), ("@type", list_1_1(singleton(Json(0, "Material")))), try_include("name", _arrow1209, oa.Name), try_include("type", _arrow1210, oa.MaterialType), try_include_list_opt("characteristics", MaterialAttributeValue_ROCrate_encoder, oa.Characteristics), try_include_list_opt("derivesFrom", _arrow1211, oa.DerivesFrom), ("@context", context_jsonvalue)])))
 
 
-def _arrow1259(__unit: None=None) -> Decoder_1[Material]:
+def _arrow1218(__unit: None=None) -> Decoder_1[Material]:
     def decode(__unit: None=None) -> Decoder_1[Material]:
-        def _arrow1258(get: IGetters) -> Material:
-            def _arrow1253(__unit: None=None) -> str | None:
+        def _arrow1217(get: IGetters) -> Material:
+            def _arrow1212(__unit: None=None) -> str | None:
                 object_arg: IOptionalGetter = get.Optional
                 return object_arg.Field("@id", Decode_uri)
 
-            def _arrow1254(__unit: None=None) -> str | None:
+            def _arrow1213(__unit: None=None) -> str | None:
                 object_arg_1: IOptionalGetter = get.Optional
                 return object_arg_1.Field("name", string)
 
-            def _arrow1255(__unit: None=None) -> MaterialType | None:
+            def _arrow1214(__unit: None=None) -> MaterialType | None:
                 object_arg_2: IOptionalGetter = get.Optional
                 return object_arg_2.Field("type", MaterialType_ROCrate_decoder)
 
-            def _arrow1256(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
+            def _arrow1215(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
                 arg_7: Decoder_1[FSharpList[MaterialAttributeValue]] = list_1_2(MaterialAttributeValue_ROCrate_decoder)
                 object_arg_3: IOptionalGetter = get.Optional
                 return object_arg_3.Field("characteristics", arg_7)
 
-            def _arrow1257(__unit: None=None) -> FSharpList[Material] | None:
+            def _arrow1216(__unit: None=None) -> FSharpList[Material] | None:
                 arg_9: Decoder_1[FSharpList[Material]] = list_1_2(decode(None))
                 object_arg_4: IOptionalGetter = get.Optional
                 return object_arg_4.Field("derivesFrom", arg_9)
 
-            return Material(_arrow1253(), _arrow1254(), _arrow1255(), _arrow1256(), _arrow1257())
+            return Material(_arrow1212(), _arrow1213(), _arrow1214(), _arrow1215(), _arrow1216())
 
-        return object(_arrow1258)
+        return object(_arrow1217)
 
     return decode(None)
 
 
-Material_ROCrate_decoder: Decoder_1[Material] = _arrow1259()
+Material_ROCrate_decoder: Decoder_1[Material] = _arrow1218()
 
 def Material_ISAJson_encoder(oa: Material) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1261(value: str, oa: Any=oa) -> Json:
+    def _arrow1220(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1262(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1221(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1263(oa_1: MaterialAttributeValue, oa: Any=oa) -> Json:
+    def _arrow1222(oa_1: MaterialAttributeValue, oa: Any=oa) -> Json:
         return MaterialAttributeValue_ISAJson_encoder(oa_1)
 
-    def _arrow1264(oa_2: Material, oa: Any=oa) -> Json:
+    def _arrow1223(oa_2: Material, oa: Any=oa) -> Json:
         return Material_ISAJson_encoder(oa_2)
 
-    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1261, oa.ID), try_include("name", _arrow1262, oa.Name), try_include("type", MaterialType_ISAJson_encoder, oa.MaterialType), try_include_list_opt("characteristics", _arrow1263, oa.Characteristics), try_include_list_opt("derivesFrom", _arrow1264, oa.DerivesFrom)])))
+    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1220, oa.ID), try_include("name", _arrow1221, oa.Name), try_include("type", MaterialType_ISAJson_encoder, oa.MaterialType), try_include_list_opt("characteristics", _arrow1222, oa.Characteristics), try_include_list_opt("derivesFrom", _arrow1223, oa.DerivesFrom)])))
 
 
 Material_ISAJson_allowedFields: FSharpList[str] = of_array(["@id", "@type", "name", "type", "characteristics", "derivesFrom", "@context"])
 
-def _arrow1271(__unit: None=None) -> Decoder_1[Material]:
+def _arrow1230(__unit: None=None) -> Decoder_1[Material]:
     def decode(__unit: None=None) -> Decoder_1[Material]:
-        def _arrow1270(get: IGetters) -> Material:
-            def _arrow1265(__unit: None=None) -> str | None:
+        def _arrow1229(get: IGetters) -> Material:
+            def _arrow1224(__unit: None=None) -> str | None:
                 object_arg: IOptionalGetter = get.Optional
                 return object_arg.Field("@id", Decode_uri)
 
-            def _arrow1266(__unit: None=None) -> str | None:
+            def _arrow1225(__unit: None=None) -> str | None:
                 object_arg_1: IOptionalGetter = get.Optional
                 return object_arg_1.Field("name", string)
 
-            def _arrow1267(__unit: None=None) -> MaterialType | None:
+            def _arrow1226(__unit: None=None) -> MaterialType | None:
                 object_arg_2: IOptionalGetter = get.Optional
                 return object_arg_2.Field("type", MaterialType_ISAJson_decoder)
 
-            def _arrow1268(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
+            def _arrow1227(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
                 arg_7: Decoder_1[FSharpList[MaterialAttributeValue]] = list_1_2(MaterialAttributeValue_ISAJson_decoder)
                 object_arg_3: IOptionalGetter = get.Optional
                 return object_arg_3.Field("characteristics", arg_7)
 
-            def _arrow1269(__unit: None=None) -> FSharpList[Material] | None:
+            def _arrow1228(__unit: None=None) -> FSharpList[Material] | None:
                 arg_9: Decoder_1[FSharpList[Material]] = list_1_2(decode(None))
                 object_arg_4: IOptionalGetter = get.Optional
                 return object_arg_4.Field("derivesFrom", arg_9)
 
-            return Material(_arrow1265(), _arrow1266(), _arrow1267(), _arrow1268(), _arrow1269())
+            return Material(_arrow1224(), _arrow1225(), _arrow1226(), _arrow1227(), _arrow1228())
 
-        return Decode_objectNoAdditionalProperties(Material_ISAJson_allowedFields, _arrow1270)
+        return Decode_objectNoAdditionalProperties(Material_ISAJson_allowedFields, _arrow1229)
 
     return decode(None)
 
 
-Material_ISAJson_decoder: Decoder_1[Material] = _arrow1271()
+Material_ISAJson_decoder: Decoder_1[Material] = _arrow1230()
 
 def ARCtrl_Process_Material__Material_fromISAJsonString_Static_Z721C83C5(s: str) -> Material:
     match_value: FSharpResult_2[Material, str] = Decode_fromString(Material_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Material__Material_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Material], str]:
-    def _arrow1272(f: Material, spaces: Any=spaces) -> str:
+    def _arrow1231(f: Material, spaces: Any=spaces) -> str:
         value: Json = Material_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1272
+    return _arrow1231
 
 
 def ARCtrl_Process_Material__Material_fromROCrateJsonString_Static_Z721C83C5(s: str) -> Material:
     match_value: FSharpResult_2[Material, str] = Decode_fromString(Material_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Material__Material_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Material], str]:
-    def _arrow1273(f: Material, spaces: Any=spaces) -> str:
+    def _arrow1232(f: Material, spaces: Any=spaces) -> str:
         value: Json = Material_ROCrate_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1273
+    return _arrow1232
 
 
 __all__ = ["Material_ROCrate_genID", "Material_ROCrate_encoder", "Material_ROCrate_decoder", "Material_ISAJson_encoder", "Material_ISAJson_allowedFields", "Material_ISAJson_decoder", "ARCtrl_Process_Material__Material_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_Material__Material_toISAJsonString_Static_71136F3F", "ARCtrl_Process_Material__Material_fromROCrateJsonString_Static_Z721C83C5", "ARCtrl_Process_Material__Material_toROCrateJsonString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/material_attribute.py` & `arctrl-2.0.0a3/arctrl/Json/Process/material_attribute.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/material_attribute_value.py` & `arctrl-2.0.0a3/arctrl/Json/Process/material_attribute_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/material_type.py` & `arctrl-2.0.0a3/arctrl/Json/Process/material_type.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/process.py` & `arctrl-2.0.0a3/arctrl/Json/Process/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,220 +49,220 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1370(value_2: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1366(value_2: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1371(oa_1: Protocol, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1367(oa_1: Protocol, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return Protocol_ROCrate_encoder(study_name, assay_name, oa.Name, oa_1)
 
-    def _arrow1372(author_list: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1368(author_list: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return Person_ROCrate_encodeAuthorListString(author_list)
 
-    def _arrow1373(value_4: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1369(value_4: str, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1374(value_6: ProcessInput, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1370(value_6: ProcessInput, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return ProcessInput_ROCrate_encoder(value_6)
 
-    def _arrow1375(value_7: ProcessOutput, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1371(value_7: ProcessOutput, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return ProcessOutput_ROCrate_encoder(value_7)
 
-    def _arrow1376(comment: Comment, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
+    def _arrow1372(comment: Comment, study_name: Any=study_name, assay_name: Any=assay_name, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Process_ROCrate_genID(oa))), ("@type", list_1_1(singleton(Json(0, "Process")))), try_include("name", _arrow1370, oa.Name), try_include("executesProtocol", _arrow1371, oa.ExecutesProtocol), try_include_list_opt("parameterValues", ProcessParameterValue_ROCrate_encoder, oa.ParameterValues), try_include("performer", _arrow1372, oa.Performer), try_include("date", _arrow1373, oa.Date), try_include_list_opt("inputs", _arrow1374, oa.Inputs), try_include_list_opt("outputs", _arrow1375, oa.Outputs), try_include_list_opt("comments", _arrow1376, oa.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Process_ROCrate_genID(oa))), ("@type", list_1_1(singleton(Json(0, "Process")))), try_include("name", _arrow1366, oa.Name), try_include("executesProtocol", _arrow1367, oa.ExecutesProtocol), try_include_list_opt("parameterValues", ProcessParameterValue_ROCrate_encoder, oa.ParameterValues), try_include("performer", _arrow1368, oa.Performer), try_include("date", _arrow1369, oa.Date), try_include_list_opt("inputs", _arrow1370, oa.Inputs), try_include_list_opt("outputs", _arrow1371, oa.Outputs), try_include_list_opt("comments", _arrow1372, oa.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow1386(get: IGetters) -> Process:
-    def _arrow1377(__unit: None=None) -> str | None:
+def _arrow1382(get: IGetters) -> Process:
+    def _arrow1373(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("@id", Decode_uri)
 
-    def _arrow1378(__unit: None=None) -> str | None:
+    def _arrow1374(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("name", string)
 
-    def _arrow1379(__unit: None=None) -> Protocol | None:
+    def _arrow1375(__unit: None=None) -> Protocol | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("executesProtocol", Protocol_ROCrate_decoder)
 
-    def _arrow1380(__unit: None=None) -> FSharpList[ProcessParameterValue] | None:
+    def _arrow1376(__unit: None=None) -> FSharpList[ProcessParameterValue] | None:
         arg_7: Decoder_1[FSharpList[ProcessParameterValue]] = list_1_2(ProcessParameterValue_ROCrate_decoder)
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("parameterValues", arg_7)
 
-    def _arrow1381(__unit: None=None) -> str | None:
+    def _arrow1377(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("performer", Person_ROCrate_decodeAuthorListString)
 
-    def _arrow1382(__unit: None=None) -> str | None:
+    def _arrow1378(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("date", string)
 
-    def _arrow1383(__unit: None=None) -> FSharpList[ProcessInput] | None:
+    def _arrow1379(__unit: None=None) -> FSharpList[ProcessInput] | None:
         arg_13: Decoder_1[FSharpList[ProcessInput]] = list_1_2(ProcessInput_ROCrate_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("inputs", arg_13)
 
-    def _arrow1384(__unit: None=None) -> FSharpList[ProcessOutput] | None:
+    def _arrow1380(__unit: None=None) -> FSharpList[ProcessOutput] | None:
         arg_15: Decoder_1[FSharpList[ProcessOutput]] = list_1_2(ProcessOutput_ROCrate_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("outputs", arg_15)
 
-    def _arrow1385(__unit: None=None) -> FSharpList[Comment] | None:
+    def _arrow1381(__unit: None=None) -> FSharpList[Comment] | None:
         arg_17: Decoder_1[FSharpList[Comment]] = list_1_2(Comment_ROCrate_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("comments", arg_17)
 
-    return Process(_arrow1377(), _arrow1378(), _arrow1379(), _arrow1380(), _arrow1381(), _arrow1382(), None, None, _arrow1383(), _arrow1384(), _arrow1385())
+    return Process(_arrow1373(), _arrow1374(), _arrow1375(), _arrow1376(), _arrow1377(), _arrow1378(), None, None, _arrow1379(), _arrow1380(), _arrow1381())
 
 
-Process_ROCrate_decoder: Decoder_1[Process] = object(_arrow1386)
+Process_ROCrate_decoder: Decoder_1[Process] = object(_arrow1382)
 
 def Process_ISAJson_encoder(oa: Process) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1388(value: str, oa: Any=oa) -> Json:
+    def _arrow1384(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1389(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1385(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1390(oa_1: Protocol, oa: Any=oa) -> Json:
+    def _arrow1386(oa_1: Protocol, oa: Any=oa) -> Json:
         return Protocol_ISAJson_encoder(oa_1)
 
-    def _arrow1391(oa_2: ProcessParameterValue, oa: Any=oa) -> Json:
+    def _arrow1387(oa_2: ProcessParameterValue, oa: Any=oa) -> Json:
         return ProcessParameterValue_ISAJson_encoder(oa_2)
 
-    def _arrow1392(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1388(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1393(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1389(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1394(oa_3: Process, oa: Any=oa) -> Json:
+    def _arrow1390(oa_3: Process, oa: Any=oa) -> Json:
         return Process_ISAJson_encoder(oa_3)
 
-    def _arrow1395(oa_4: Process, oa: Any=oa) -> Json:
+    def _arrow1391(oa_4: Process, oa: Any=oa) -> Json:
         return Process_ISAJson_encoder(oa_4)
 
-    def _arrow1396(value_8: ProcessInput, oa: Any=oa) -> Json:
+    def _arrow1392(value_8: ProcessInput, oa: Any=oa) -> Json:
         return ProcessInput_ISAJson_encoder(value_8)
 
-    def _arrow1397(value_9: ProcessOutput, oa: Any=oa) -> Json:
+    def _arrow1393(value_9: ProcessOutput, oa: Any=oa) -> Json:
         return ProcessOutput_ISAJson_encoder(value_9)
 
-    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1388, oa.ID), try_include("name", _arrow1389, oa.Name), try_include("executesProtocol", _arrow1390, oa.ExecutesProtocol), try_include_list_opt("parameterValues", _arrow1391, oa.ParameterValues), try_include("performer", _arrow1392, oa.Performer), try_include("date", _arrow1393, oa.Date), try_include("previousProcess", _arrow1394, oa.PreviousProcess), try_include("nextProcess", _arrow1395, oa.NextProcess), try_include_list_opt("inputs", _arrow1396, oa.Inputs), try_include_list_opt("outputs", _arrow1397, oa.Outputs), try_include_list_opt("comments", Comment_ISAJson_encoder, oa.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1384, oa.ID), try_include("name", _arrow1385, oa.Name), try_include("executesProtocol", _arrow1386, oa.ExecutesProtocol), try_include_list_opt("parameterValues", _arrow1387, oa.ParameterValues), try_include("performer", _arrow1388, oa.Performer), try_include("date", _arrow1389, oa.Date), try_include("previousProcess", _arrow1390, oa.PreviousProcess), try_include("nextProcess", _arrow1391, oa.NextProcess), try_include_list_opt("inputs", _arrow1392, oa.Inputs), try_include_list_opt("outputs", _arrow1393, oa.Outputs), try_include_list_opt("comments", Comment_ISAJson_encoder, oa.Comments)])))
 
 
-def _arrow1410(__unit: None=None) -> Decoder_1[Process]:
+def _arrow1406(__unit: None=None) -> Decoder_1[Process]:
     def decode(__unit: None=None) -> Decoder_1[Process]:
-        def _arrow1409(get: IGetters) -> Process:
-            def _arrow1398(__unit: None=None) -> str | None:
+        def _arrow1405(get: IGetters) -> Process:
+            def _arrow1394(__unit: None=None) -> str | None:
                 object_arg: IOptionalGetter = get.Optional
                 return object_arg.Field("@id", Decode_uri)
 
-            def _arrow1399(__unit: None=None) -> str | None:
+            def _arrow1395(__unit: None=None) -> str | None:
                 object_arg_1: IOptionalGetter = get.Optional
                 return object_arg_1.Field("name", string)
 
-            def _arrow1400(__unit: None=None) -> Protocol | None:
+            def _arrow1396(__unit: None=None) -> Protocol | None:
                 object_arg_2: IOptionalGetter = get.Optional
                 return object_arg_2.Field("executesProtocol", Protocol_ISAJson_decoder)
 
-            def _arrow1401(__unit: None=None) -> FSharpList[ProcessParameterValue] | None:
+            def _arrow1397(__unit: None=None) -> FSharpList[ProcessParameterValue] | None:
                 arg_7: Decoder_1[FSharpList[ProcessParameterValue]] = list_1_2(ProcessParameterValue_ISAJson_decoder)
                 object_arg_3: IOptionalGetter = get.Optional
                 return object_arg_3.Field("parameterValues", arg_7)
 
-            def _arrow1402(__unit: None=None) -> str | None:
+            def _arrow1398(__unit: None=None) -> str | None:
                 object_arg_4: IOptionalGetter = get.Optional
                 return object_arg_4.Field("performer", string)
 
-            def _arrow1403(__unit: None=None) -> str | None:
+            def _arrow1399(__unit: None=None) -> str | None:
                 object_arg_5: IOptionalGetter = get.Optional
                 return object_arg_5.Field("date", string)
 
-            def _arrow1404(__unit: None=None) -> Process | None:
+            def _arrow1400(__unit: None=None) -> Process | None:
                 arg_13: Decoder_1[Process] = decode(None)
                 object_arg_6: IOptionalGetter = get.Optional
                 return object_arg_6.Field("previousProcess", arg_13)
 
-            def _arrow1405(__unit: None=None) -> Process | None:
+            def _arrow1401(__unit: None=None) -> Process | None:
                 arg_15: Decoder_1[Process] = decode(None)
                 object_arg_7: IOptionalGetter = get.Optional
                 return object_arg_7.Field("nextProcess", arg_15)
 
-            def _arrow1406(__unit: None=None) -> FSharpList[ProcessInput] | None:
+            def _arrow1402(__unit: None=None) -> FSharpList[ProcessInput] | None:
                 arg_17: Decoder_1[FSharpList[ProcessInput]] = list_1_2(ProcessInput_ISAJson_decoder)
                 object_arg_8: IOptionalGetter = get.Optional
                 return object_arg_8.Field("inputs", arg_17)
 
-            def _arrow1407(__unit: None=None) -> FSharpList[ProcessOutput] | None:
+            def _arrow1403(__unit: None=None) -> FSharpList[ProcessOutput] | None:
                 arg_19: Decoder_1[FSharpList[ProcessOutput]] = list_1_2(ProcessOutput_ISAJson_decoder)
                 object_arg_9: IOptionalGetter = get.Optional
                 return object_arg_9.Field("outputs", arg_19)
 
-            def _arrow1408(__unit: None=None) -> FSharpList[Comment] | None:
+            def _arrow1404(__unit: None=None) -> FSharpList[Comment] | None:
                 arg_21: Decoder_1[FSharpList[Comment]] = list_1_2(Comment_ISAJson_decoder)
                 object_arg_10: IOptionalGetter = get.Optional
                 return object_arg_10.Field("comments", arg_21)
 
-            return Process(_arrow1398(), _arrow1399(), _arrow1400(), _arrow1401(), _arrow1402(), _arrow1403(), _arrow1404(), _arrow1405(), _arrow1406(), _arrow1407(), _arrow1408())
+            return Process(_arrow1394(), _arrow1395(), _arrow1396(), _arrow1397(), _arrow1398(), _arrow1399(), _arrow1400(), _arrow1401(), _arrow1402(), _arrow1403(), _arrow1404())
 
-        return object(_arrow1409)
+        return object(_arrow1405)
 
     return decode(None)
 
 
-Process_ISAJson_decoder: Decoder_1[Process] = _arrow1410()
+Process_ISAJson_decoder: Decoder_1[Process] = _arrow1406()
 
 def ARCtrl_Process_Process__Process_fromISAJsonString_Static_Z721C83C5(s: str) -> Process:
     match_value: FSharpResult_2[Process, str] = Decode_fromString(Process_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Process__Process_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Process], str]:
-    def _arrow1411(f: Process, spaces: Any=spaces) -> str:
+    def _arrow1407(f: Process, spaces: Any=spaces) -> str:
         value: Json = Process_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1411
+    return _arrow1407
 
 
 def ARCtrl_Process_Process__Process_fromROCrateString_Static_Z721C83C5(s: str) -> Process:
     match_value: FSharpResult_2[Process, str] = Decode_fromString(Process_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Process__Process_toROCrateString_Static_39E0BC3F(study_name: str | None=None, assay_name: str | None=None, spaces: int | None=None) -> Callable[[Process], str]:
-    def _arrow1412(f: Process, study_name: Any=study_name, assay_name: Any=assay_name, spaces: Any=spaces) -> str:
+    def _arrow1408(f: Process, study_name: Any=study_name, assay_name: Any=assay_name, spaces: Any=spaces) -> str:
         value: Json = Process_ROCrate_encoder(study_name, assay_name, f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1412
+    return _arrow1408
 
 
 __all__ = ["Process_ROCrate_genID", "Process_ROCrate_encoder", "Process_ROCrate_decoder", "Process_ISAJson_encoder", "Process_ISAJson_decoder", "ARCtrl_Process_Process__Process_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_Process__Process_toISAJsonString_Static_71136F3F", "ARCtrl_Process_Process__Process_fromROCrateString_Static_Z721C83C5", "ARCtrl_Process_Process__Process_toROCrateString_Static_39E0BC3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/process_input.py` & `arctrl-2.0.0a3/arctrl/Json/Process/process_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,31 +30,31 @@
         return Material_ROCrate_encoder(value.fields[0])
 
     else: 
         return Source_ROCrate_encoder(value.fields[0])
 
 
 
-def _arrow1322(Item: Source) -> ProcessInput:
+def _arrow1318(Item: Source) -> ProcessInput:
     return ProcessInput(0, Item)
 
 
-def _arrow1325(Item_1: Sample) -> ProcessInput:
+def _arrow1319(Item_1: Sample) -> ProcessInput:
     return ProcessInput(1, Item_1)
 
 
-def _arrow1328(Item_2: Data) -> ProcessInput:
+def _arrow1320(Item_2: Data) -> ProcessInput:
     return ProcessInput(2, Item_2)
 
 
-def _arrow1329(Item_3: Material) -> ProcessInput:
+def _arrow1321(Item_3: Material) -> ProcessInput:
     return ProcessInput(3, Item_3)
 
 
-ProcessInput_ROCrate_decoder: Decoder_1[ProcessInput] = one_of(of_array([map(_arrow1322, Source_ROCrate_decoder), map(_arrow1325, Sample_ROCrate_decoder), map(_arrow1328, Data_ROCrate_decoder), map(_arrow1329, Material_ROCrate_decoder)]))
+ProcessInput_ROCrate_decoder: Decoder_1[ProcessInput] = one_of(of_array([map(_arrow1318, Source_ROCrate_decoder), map(_arrow1319, Sample_ROCrate_decoder), map(_arrow1320, Data_ROCrate_decoder), map(_arrow1321, Material_ROCrate_decoder)]))
 
 def ProcessInput_ISAJson_encoder(value: ProcessInput) -> Json:
     if value.tag == 1:
         return Sample_ISAJson_encoder(value.fields[0])
 
     elif value.tag == 2:
         return Data_ISAJson_encoder(value.fields[0])
@@ -63,45 +63,45 @@
         return Material_ISAJson_encoder(value.fields[0])
 
     else: 
         return Source_ISAJson_encoder(value.fields[0])
 
 
 
-def _arrow1341(Item: Source) -> ProcessInput:
+def _arrow1323(Item: Source) -> ProcessInput:
     return ProcessInput(0, Item)
 
 
-def _arrow1344(Item_1: Sample) -> ProcessInput:
+def _arrow1324(Item_1: Sample) -> ProcessInput:
     return ProcessInput(1, Item_1)
 
 
-def _arrow1345(Item_2: Data) -> ProcessInput:
+def _arrow1325(Item_2: Data) -> ProcessInput:
     return ProcessInput(2, Item_2)
 
 
-def _arrow1347(Item_3: Material) -> ProcessInput:
+def _arrow1326(Item_3: Material) -> ProcessInput:
     return ProcessInput(3, Item_3)
 
 
-ProcessInput_ISAJson_decoder: Decoder_1[ProcessInput] = one_of(of_array([map(_arrow1341, Source_ISAJson_decoder), map(_arrow1344, Sample_ISAJson_decoder), map(_arrow1345, Data_ISAJson_decoder), map(_arrow1347, Material_ISAJson_decoder)]))
+ProcessInput_ISAJson_decoder: Decoder_1[ProcessInput] = one_of(of_array([map(_arrow1323, Source_ISAJson_decoder), map(_arrow1324, Sample_ISAJson_decoder), map(_arrow1325, Data_ISAJson_decoder), map(_arrow1326, Material_ISAJson_decoder)]))
 
 def ARCtrl_Process_ProcessInput__ProcessInput_fromISAJsonString_Static_Z721C83C5(s: str) -> ProcessInput:
     match_value: FSharpResult_2[ProcessInput, str] = Decode_fromString(ProcessInput_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_ProcessInput__ProcessInput_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ProcessInput], str]:
-    def _arrow1349(f: ProcessInput, spaces: Any=spaces) -> str:
+    def _arrow1329(f: ProcessInput, spaces: Any=spaces) -> str:
         value: Json = ProcessInput_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1349
+    return _arrow1329
 
 
 __all__ = ["ProcessInput_ROCrate_encoder", "ProcessInput_ROCrate_decoder", "ProcessInput_ISAJson_encoder", "ProcessInput_ISAJson_decoder", "ARCtrl_Process_ProcessInput__ProcessInput_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_ProcessInput__ProcessInput_toISAJsonString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/process_output.py` & `arctrl-2.0.0a3/arctrl/Json/Process/process_output.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/process_parameter_value.py` & `arctrl-2.0.0a3/arctrl/Json/Process/process_parameter_value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/process_sequence.py` & `arctrl-2.0.0a3/arctrl/Json/Process/process_sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,57 +10,57 @@
 from ...fable_modules.thoth_json_core.types import Json
 from ...fable_modules.thoth_json_python.decode import Decode_fromString
 from ...fable_modules.thoth_json_python.encode import to_string
 from ...Core.Process.process import Process
 from ..encode import default_spaces
 from .process import (Process_ISAJson_decoder, Process_ISAJson_encoder, Process_ROCrate_decoder, Process_ROCrate_encoder)
 
-def _expr1363() -> TypeInfo:
+def _expr1360() -> TypeInfo:
     return class_type("ARCtrl.Json.ProcessSequence", None, ProcessSequence)
 
 
 class ProcessSequence:
     ...
 
-ProcessSequence_reflection = _expr1363
+ProcessSequence_reflection = _expr1360
 
 def ProcessSequence_fromISAJsonString_Z721C83C5(s: str) -> FSharpList[Process]:
     match_value: FSharpResult_2[FSharpList[Process], str] = Decode_fromString(list_1_1(Process_ISAJson_decoder), s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ProcessSequence_toISAJsonString_71136F3F(spaces: int | None=None) -> Callable[[FSharpList[Process]], str]:
-    def _arrow1364(f: FSharpList[Process], spaces: Any=spaces) -> str:
+    def _arrow1361(f: FSharpList[Process], spaces: Any=spaces) -> str:
         value: Json = list_1_2(map(Process_ISAJson_encoder, f))
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1364
+    return _arrow1361
 
 
 def ProcessSequence_fromROCrateJsonString_Z721C83C5(s: str) -> FSharpList[Process]:
     match_value: FSharpResult_2[FSharpList[Process], str] = Decode_fromString(list_1_1(Process_ROCrate_decoder), s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ProcessSequence_toROCrateJsonString_39E0BC3F(study_name: str | None=None, assay_name: str | None=None, spaces: int | None=None) -> Callable[[FSharpList[Process]], str]:
-    def _arrow1365(f: FSharpList[Process], study_name: Any=study_name, assay_name: Any=assay_name, spaces: Any=spaces) -> str:
+    def _arrow1362(f: FSharpList[Process], study_name: Any=study_name, assay_name: Any=assay_name, spaces: Any=spaces) -> str:
         def mapping(oa: Process) -> Json:
             return Process_ROCrate_encoder(study_name, assay_name, oa)
 
         value: Json = list_1_2(map(mapping, f))
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1365
+    return _arrow1362
 
 
 __all__ = ["ProcessSequence_reflection", "ProcessSequence_fromISAJsonString_Z721C83C5", "ProcessSequence_toISAJsonString_71136F3F", "ProcessSequence_fromROCrateJsonString_Z721C83C5", "ProcessSequence_toROCrateJsonString_39E0BC3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/property_value.py` & `arctrl-2.0.0a3/arctrl/Json/Process/property_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ...fable_modules.thoth_json_core.decode import (object, IOptionalGetter, string, IGetters)
 from ...fable_modules.thoth_json_core.types import (Json, Decoder_1)
 from ...Core.ontology_annotation import OntologyAnnotation
 from ...Core.Process.iproperty_value import IPropertyValue_1
 from ...Core.Process.value import Value
 from ..context.rocrate.property_value_context import context_jsonvalue
 from ..encode import try_include
+from ..ontology_annotation import AnnotationValue_decoder
 
 _T = TypeVar("_T")
 
 def gen_id(p: IPropertyValue_1[Any]) -> str:
     match_value: OntologyAnnotation | None = p.GetCategory()
     if match_value is None:
         def _arrow1160(__unit: None=None, p: Any=p) -> str:
@@ -111,33 +112,83 @@
         def _arrow1170(__unit: None=None) -> OntologyAnnotation | None:
             name: str | None
             object_arg: IOptionalGetter = get.Optional
             name = object_arg.Field("category", string)
             code: str | None
             object_arg_1: IOptionalGetter = get.Optional
             code = object_arg_1.Field("categoryCode", string)
-            return None if ((code is None) if (name is None) else False) else OntologyAnnotation.create(name, None, code)
+            (pattern_matching_result, code_1) = (None, None)
+            if name is None:
+                if code is not None:
+                    pattern_matching_result = 2
+                    code_1 = code
+
+                else: 
+                    pattern_matching_result = 0
+
+
+            elif code is not None:
+                pattern_matching_result = 2
+                code_1 = code
+
+            else: 
+                pattern_matching_result = 1
+
+            if pattern_matching_result == 0:
+                return None
+
+            elif pattern_matching_result == 1:
+                return OntologyAnnotation.create(name)
+
+            elif pattern_matching_result == 2:
+                return OntologyAnnotation.from_term_annotation(code_1, name)
+
 
         def _arrow1171(__unit: None=None) -> Value | None:
             value: str | None
             object_arg_2: IOptionalGetter = get.Optional
-            value = object_arg_2.Field("value", string)
-            code_1: str | None
+            value = object_arg_2.Field("value", AnnotationValue_decoder)
+            code_2: str | None
             object_arg_3: IOptionalGetter = get.Optional
-            code_1 = object_arg_3.Field("valueCode", string)
-            return None if ((code_1 is None) if (value is None) else False) else Value.from_options(value, None, code_1)
+            code_2 = object_arg_3.Field("valueCode", string)
+            return None if ((code_2 is None) if (value is None) else False) else Value.from_options(value, None, code_2)
 
         def _arrow1172(__unit: None=None) -> OntologyAnnotation | None:
             name_1: str | None
             object_arg_4: IOptionalGetter = get.Optional
             name_1 = object_arg_4.Field("unit", string)
-            code_2: str | None
+            code_3: str | None
             object_arg_5: IOptionalGetter = get.Optional
-            code_2 = object_arg_5.Field("unitCode", string)
-            return None if ((code_2 is None) if (name_1 is None) else False) else OntologyAnnotation.create(name_1, None, code_2)
+            code_3 = object_arg_5.Field("unitCode", string)
+            (pattern_matching_result_1, code_4) = (None, None)
+            if name_1 is None:
+                if code_3 is not None:
+                    pattern_matching_result_1 = 2
+                    code_4 = code_3
+
+                else: 
+                    pattern_matching_result_1 = 0
+
+
+            elif code_3 is not None:
+                pattern_matching_result_1 = 2
+                code_4 = code_3
+
+            else: 
+                pattern_matching_result_1 = 1
+
+            if pattern_matching_result_1 == 0:
+                return None
+
+            elif pattern_matching_result_1 == 1:
+                return OntologyAnnotation.create(name_1)
+
+            elif pattern_matching_result_1 == 2:
+                return OntologyAnnotation.from_term_annotation(code_4, name_1)
+
 
         return create(_arrow1170(), _arrow1171(), _arrow1172())
 
     return object(_arrow1173)
 
 
 __all__ = ["gen_id", "encoder", "decoder"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/protocol.py` & `arctrl-2.0.0a3/arctrl/Json/Process/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,202 +92,202 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1209(value_2: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1236(value_2: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1210(oa_1: OntologyAnnotation, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1237(oa_1: OntologyAnnotation, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return OntologyAnnotation_ROCrate_encoderDefinedTerm(oa_1)
 
-    def _arrow1211(value_4: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1238(value_4: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1212(value_6: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1239(value_6: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1213(value_8: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1240(value_8: str, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return Json(0, value_8)
 
-    def _arrow1214(comment: Comment, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
+    def _arrow1241(comment: Comment, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Protocol_ROCrate_genID(study_name, assay_name, process_name, oa))), ("@type", list_1_1(singleton(Json(0, "Protocol")))), try_include("name", _arrow1209, oa.Name), try_include("protocolType", _arrow1210, oa.ProtocolType), try_include("description", _arrow1211, oa.Description), try_include("uri", _arrow1212, oa.Uri), try_include("version", _arrow1213, oa.Version), try_include_list_opt("components", Component_ROCrate_encoder, oa.Components), try_include_list_opt("comments", _arrow1214, oa.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Protocol_ROCrate_genID(study_name, assay_name, process_name, oa))), ("@type", list_1_1(singleton(Json(0, "Protocol")))), try_include("name", _arrow1236, oa.Name), try_include("protocolType", _arrow1237, oa.ProtocolType), try_include("description", _arrow1238, oa.Description), try_include("uri", _arrow1239, oa.Uri), try_include("version", _arrow1240, oa.Version), try_include_list_opt("components", Component_ROCrate_encoder, oa.Components), try_include_list_opt("comments", _arrow1241, oa.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow1226(get: IGetters) -> Protocol:
-    def _arrow1218(__unit: None=None) -> FSharpList[Component]:
+def _arrow1253(get: IGetters) -> Protocol:
+    def _arrow1245(__unit: None=None) -> FSharpList[Component]:
         list_4: FSharpList[Component]
-        def _arrow1215(__unit: None=None) -> FSharpList[Component] | None:
+        def _arrow1242(__unit: None=None) -> FSharpList[Component] | None:
             arg_1: Decoder_1[FSharpList[Component]] = list_1_2(Component_ROCrate_decoder)
             object_arg: IOptionalGetter = get.Optional
             return object_arg.Field("components", arg_1)
 
-        list_2: FSharpList[Component] = default_arg(_arrow1215(), empty())
-        def _arrow1216(__unit: None=None) -> FSharpList[Component] | None:
+        list_2: FSharpList[Component] = default_arg(_arrow1242(), empty())
+        def _arrow1243(__unit: None=None) -> FSharpList[Component] | None:
             arg_3: Decoder_1[FSharpList[Component]] = list_1_2(Component_ROCrate_decoder)
             object_arg_1: IOptionalGetter = get.Optional
             return object_arg_1.Field("reagents", arg_3)
 
-        list_4 = append(default_arg(_arrow1216(), empty()), list_2)
-        def _arrow1217(__unit: None=None) -> FSharpList[Component] | None:
+        list_4 = append(default_arg(_arrow1243(), empty()), list_2)
+        def _arrow1244(__unit: None=None) -> FSharpList[Component] | None:
             arg_5: Decoder_1[FSharpList[Component]] = list_1_2(Component_ROCrate_decoder)
             object_arg_2: IOptionalGetter = get.Optional
             return object_arg_2.Field("computationalTools", arg_5)
 
-        return append(default_arg(_arrow1217(), empty()), list_4)
+        return append(default_arg(_arrow1244(), empty()), list_4)
 
-    components: FSharpList[Component] | None = Option_fromValueWithDefault(empty(), _arrow1218())
-    def _arrow1219(__unit: None=None) -> str | None:
+    components: FSharpList[Component] | None = Option_fromValueWithDefault(empty(), _arrow1245())
+    def _arrow1246(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("@id", Decode_uri)
 
-    def _arrow1220(__unit: None=None) -> str | None:
+    def _arrow1247(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("name", string)
 
-    def _arrow1221(__unit: None=None) -> OntologyAnnotation | None:
+    def _arrow1248(__unit: None=None) -> OntologyAnnotation | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("protocolType", OntologyAnnotation_ROCrate_decoderDefinedTerm)
 
-    def _arrow1222(__unit: None=None) -> str | None:
+    def _arrow1249(__unit: None=None) -> str | None:
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("description", string)
 
-    def _arrow1223(__unit: None=None) -> str | None:
+    def _arrow1250(__unit: None=None) -> str | None:
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("uri", Decode_uri)
 
-    def _arrow1224(__unit: None=None) -> str | None:
+    def _arrow1251(__unit: None=None) -> str | None:
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("version", string)
 
-    def _arrow1225(__unit: None=None) -> FSharpList[Comment] | None:
+    def _arrow1252(__unit: None=None) -> FSharpList[Comment] | None:
         arg_19: Decoder_1[FSharpList[Comment]] = list_1_2(Comment_ROCrate_decoder)
         object_arg_9: IOptionalGetter = get.Optional
         return object_arg_9.Field("comments", arg_19)
 
-    return Protocol(_arrow1219(), _arrow1220(), _arrow1221(), _arrow1222(), _arrow1223(), _arrow1224(), None, components, _arrow1225())
+    return Protocol(_arrow1246(), _arrow1247(), _arrow1248(), _arrow1249(), _arrow1250(), _arrow1251(), None, components, _arrow1252())
 
 
-Protocol_ROCrate_decoder: Decoder_1[Protocol] = object(_arrow1226)
+Protocol_ROCrate_decoder: Decoder_1[Protocol] = object(_arrow1253)
 
 def Protocol_ISAJson_encoder(oa: Protocol) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1228(value: str, oa: Any=oa) -> Json:
+    def _arrow1255(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1229(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1256(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1230(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1257(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1231(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1258(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1232(value_8: str, oa: Any=oa) -> Json:
+    def _arrow1259(value_8: str, oa: Any=oa) -> Json:
         return Json(0, value_8)
 
-    def _arrow1233(value_10: ProtocolParameter, oa: Any=oa) -> Json:
+    def _arrow1260(value_10: ProtocolParameter, oa: Any=oa) -> Json:
         return ProtocolParameter_ISAJson_encoder(value_10)
 
-    def _arrow1234(c: Component, oa: Any=oa) -> Json:
+    def _arrow1261(c: Component, oa: Any=oa) -> Json:
         return Component_ISAJson_encoder(c)
 
-    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1228, oa.ID), try_include("name", _arrow1229, oa.Name), try_include("protocolType", OntologyAnnotation_ISAJson_encoder, oa.ProtocolType), try_include("description", _arrow1230, oa.Description), try_include("uri", _arrow1231, oa.Uri), try_include("version", _arrow1232, oa.Version), try_include_list_opt("parameters", _arrow1233, oa.Parameters), try_include_list_opt("components", _arrow1234, oa.Components), try_include_list_opt("comments", Comment_ISAJson_encoder, oa.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1255, oa.ID), try_include("name", _arrow1256, oa.Name), try_include("protocolType", OntologyAnnotation_ISAJson_encoder, oa.ProtocolType), try_include("description", _arrow1257, oa.Description), try_include("uri", _arrow1258, oa.Uri), try_include("version", _arrow1259, oa.Version), try_include_list_opt("parameters", _arrow1260, oa.Parameters), try_include_list_opt("components", _arrow1261, oa.Components), try_include_list_opt("comments", Comment_ISAJson_encoder, oa.Comments)])))
 
 
-def _arrow1244(get: IGetters) -> Protocol:
-    def _arrow1235(__unit: None=None) -> str | None:
+def _arrow1271(get: IGetters) -> Protocol:
+    def _arrow1262(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("@id", Decode_uri)
 
-    def _arrow1236(__unit: None=None) -> str | None:
+    def _arrow1263(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("name", string)
 
-    def _arrow1237(__unit: None=None) -> OntologyAnnotation | None:
+    def _arrow1264(__unit: None=None) -> OntologyAnnotation | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("protocolType", OntologyAnnotation_ISAJson_decoder)
 
-    def _arrow1238(__unit: None=None) -> str | None:
+    def _arrow1265(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("description", string)
 
-    def _arrow1239(__unit: None=None) -> str | None:
+    def _arrow1266(__unit: None=None) -> str | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("uri", Decode_uri)
 
-    def _arrow1240(__unit: None=None) -> str | None:
+    def _arrow1267(__unit: None=None) -> str | None:
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("version", string)
 
-    def _arrow1241(__unit: None=None) -> FSharpList[ProtocolParameter] | None:
+    def _arrow1268(__unit: None=None) -> FSharpList[ProtocolParameter] | None:
         arg_13: Decoder_1[FSharpList[ProtocolParameter]] = list_1_2(ProtocolParameter_ISAJson_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("parameters", arg_13)
 
-    def _arrow1242(__unit: None=None) -> FSharpList[Component] | None:
+    def _arrow1269(__unit: None=None) -> FSharpList[Component] | None:
         arg_15: Decoder_1[FSharpList[Component]] = list_1_2(Component_ISAJson_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("components", arg_15)
 
-    def _arrow1243(__unit: None=None) -> FSharpList[Comment] | None:
+    def _arrow1270(__unit: None=None) -> FSharpList[Comment] | None:
         arg_17: Decoder_1[FSharpList[Comment]] = list_1_2(Comment_ISAJson_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("comments", arg_17)
 
-    return Protocol(_arrow1235(), _arrow1236(), _arrow1237(), _arrow1238(), _arrow1239(), _arrow1240(), _arrow1241(), _arrow1242(), _arrow1243())
+    return Protocol(_arrow1262(), _arrow1263(), _arrow1264(), _arrow1265(), _arrow1266(), _arrow1267(), _arrow1268(), _arrow1269(), _arrow1270())
 
 
-Protocol_ISAJson_decoder: Decoder_1[Protocol] = object(_arrow1244)
+Protocol_ISAJson_decoder: Decoder_1[Protocol] = object(_arrow1271)
 
 def ARCtrl_Process_Protocol__Protocol_fromISAJsonString_Static_Z721C83C5(s: str) -> Protocol:
     match_value: FSharpResult_2[Protocol, str] = Decode_fromString(Protocol_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Protocol__Protocol_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Protocol], str]:
-    def _arrow1245(f: Protocol, spaces: Any=spaces) -> str:
+    def _arrow1272(f: Protocol, spaces: Any=spaces) -> str:
         value: Json = Protocol_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1245
+    return _arrow1272
 
 
 def ARCtrl_Process_Protocol__Protocol_fromROCrateString_Static_Z721C83C5(s: str) -> Protocol:
     match_value: FSharpResult_2[Protocol, str] = Decode_fromString(Protocol_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Protocol__Protocol_toROCrateString_Static(study_name: str | None=None, assay_name: str | None=None, process_name: str | None=None, spaces: int | None=None) -> Callable[[Protocol], str]:
-    def _arrow1246(f: Protocol, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, spaces: Any=spaces) -> str:
+    def _arrow1273(f: Protocol, study_name: Any=study_name, assay_name: Any=assay_name, process_name: Any=process_name, spaces: Any=spaces) -> str:
         value: Json = Protocol_ROCrate_encoder(study_name, assay_name, process_name, f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1246
+    return _arrow1273
 
 
 __all__ = ["Protocol_ROCrate_genID", "Protocol_ROCrate_encoder", "Protocol_ROCrate_decoder", "Protocol_ISAJson_encoder", "Protocol_ISAJson_decoder", "ARCtrl_Process_Protocol__Protocol_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_Protocol__Protocol_toISAJsonString_Static_71136F3F", "ARCtrl_Process_Protocol__Protocol_fromROCrateString_Static_Z721C83C5", "ARCtrl_Process_Protocol__Protocol_toROCrateString_Static"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/protocol_parameter.py` & `arctrl-2.0.0a3/arctrl/Json/Process/protocol_parameter.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/sample.py` & `arctrl-2.0.0a3/arctrl/Json/Process/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,42 +50,42 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1317(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1327(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1318(x: Json, oa: Any=oa) -> Json:
+    def _arrow1328(x: Json, oa: Any=oa) -> Json:
         return x
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Sample_ROCrate_genID(oa))), ("@type", list_1_2(singleton(Json(0, "Sample")))), try_include("name", _arrow1317, oa.Name), try_include_list("additionalProperties", _arrow1318, additional_properties), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Sample_ROCrate_genID(oa))), ("@type", list_1_2(singleton(Json(0, "Sample")))), try_include("name", _arrow1327, oa.Name), try_include_list("additionalProperties", _arrow1328, additional_properties), ("@context", context_jsonvalue)])))
 
 
-class ObjectExpr1320(Decoder_1[tuple[MaterialAttributeValue | None, FactorValue | None]]):
+class ObjectExpr1331(Decoder_1[tuple[MaterialAttributeValue | None, FactorValue | None]]):
     def Decode(self, s: IDecoderHelpers_1[__A_], json: __A_) -> FSharpResult_2[tuple[MaterialAttributeValue | None, FactorValue | None], tuple[str, ErrorReason_1[__A_]]]:
-        def _arrow1319(__unit: None=None) -> str:
+        def _arrow1330(__unit: None=None) -> str:
             match_value: FSharpResult_2[str, tuple[str, ErrorReason_1[__A_]]] = string.Decode(s, s.get_property("additionalType", json))
             return match_value.fields[0] if (match_value.tag == 0) else ""
 
-        if (_arrow1319() if s.has_property("additionalType", json) else "") == "FactorValue":
+        if (_arrow1330() if s.has_property("additionalType", json) else "") == "FactorValue":
             match_value_1: FSharpResult_2[FactorValue, tuple[str, ErrorReason_1[__A_]]] = FactorValue_ROCrate_decoder.Decode(s, json)
             return FSharpResult_2(1, match_value_1.fields[0]) if (match_value_1.tag == 1) else FSharpResult_2(0, (None, match_value_1.fields[0]))
 
         else: 
             match_value_2: FSharpResult_2[MaterialAttributeValue, tuple[str, ErrorReason_1[__A_]]] = MaterialAttributeValue_ROCrate_decoder.Decode(s, json)
             return FSharpResult_2(1, match_value_2.fields[0]) if (match_value_2.tag == 1) else FSharpResult_2(0, (match_value_2.fields[0], None))
 
 
 
-Sample_ROCrate_additionalPropertyDecoder: Decoder_1[tuple[MaterialAttributeValue | None, FactorValue | None]] = ObjectExpr1320()
+Sample_ROCrate_additionalPropertyDecoder: Decoder_1[tuple[MaterialAttributeValue | None, FactorValue | None]] = ObjectExpr1331()
 
-def _arrow1327(get: IGetters) -> Sample:
+def _arrow1335(get: IGetters) -> Sample:
     additional_properties: FSharpList[tuple[MaterialAttributeValue | None, FactorValue | None]] | None
     arg_1: Decoder_1[FSharpList[tuple[MaterialAttributeValue | None, FactorValue | None]]] = list_1_3(Sample_ROCrate_additionalPropertyDecoder)
     object_arg: IOptionalGetter = get.Optional
     additional_properties = object_arg.Field("additionalProperties", arg_1)
     pattern_input: tuple[FSharpList[MaterialAttributeValue] | None, FSharpList[FactorValue] | None]
     if additional_properties is not None:
         additional_properties_1: FSharpList[tuple[MaterialAttributeValue | None, FactorValue | None]] = additional_properties
@@ -96,122 +96,122 @@
             return tuple_1[1]
 
         pattern_input = (Option_fromValueWithDefault(empty(), choose(chooser, additional_properties_1)), Option_fromValueWithDefault(empty(), choose(chooser_1, additional_properties_1)))
 
     else: 
         pattern_input = (None, None)
 
-    def _arrow1323(__unit: None=None) -> str | None:
+    def _arrow1332(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("@id", Decode_uri)
 
-    def _arrow1324(__unit: None=None) -> str | None:
+    def _arrow1333(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("name", string)
 
-    def _arrow1326(__unit: None=None) -> FSharpList[Source] | None:
+    def _arrow1334(__unit: None=None) -> FSharpList[Source] | None:
         arg_7: Decoder_1[FSharpList[Source]] = list_1_3(Source_ROCrate_decoder)
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("derivesFrom", arg_7)
 
-    return Sample(_arrow1323(), _arrow1324(), pattern_input[0], pattern_input[1], _arrow1326())
+    return Sample(_arrow1332(), _arrow1333(), pattern_input[0], pattern_input[1], _arrow1334())
 
 
-Sample_ROCrate_decoder: Decoder_1[Sample] = object(_arrow1327)
+Sample_ROCrate_decoder: Decoder_1[Sample] = object(_arrow1335)
 
 def Sample_ISAJson_encoder(oa: Sample) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1331(value: str, oa: Any=oa) -> Json:
+    def _arrow1337(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1332(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1338(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1333(oa_1: MaterialAttributeValue, oa: Any=oa) -> Json:
+    def _arrow1339(oa_1: MaterialAttributeValue, oa: Any=oa) -> Json:
         return MaterialAttributeValue_ISAJson_encoder(oa_1)
 
-    def _arrow1334(fv: FactorValue, oa: Any=oa) -> Json:
+    def _arrow1340(fv: FactorValue, oa: Any=oa) -> Json:
         return FactorValue_ISAJson_encoder(fv)
 
-    def _arrow1335(oa_2: Source, oa: Any=oa) -> Json:
+    def _arrow1341(oa_2: Source, oa: Any=oa) -> Json:
         return Source_ISAJson_encoder(oa_2)
 
-    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1331, oa.ID), try_include("name", _arrow1332, oa.Name), try_include_list_opt("characteristics", _arrow1333, oa.Characteristics), try_include_list_opt("factorValues", _arrow1334, oa.FactorValues), try_include_list_opt("derivesFrom", _arrow1335, oa.DerivesFrom)])))
+    return Json(5, choose(chooser, of_array([try_include("@id", _arrow1337, oa.ID), try_include("name", _arrow1338, oa.Name), try_include_list_opt("characteristics", _arrow1339, oa.Characteristics), try_include_list_opt("factorValues", _arrow1340, oa.FactorValues), try_include_list_opt("derivesFrom", _arrow1341, oa.DerivesFrom)])))
 
 
 Sample_ISAJson_allowedFields: FSharpList[str] = of_array(["@id", "name", "characteristics", "factorValues", "derivesFrom", "@type", "@context"])
 
-def _arrow1343(get: IGetters) -> Sample:
-    def _arrow1336(__unit: None=None) -> str | None:
+def _arrow1347(get: IGetters) -> Sample:
+    def _arrow1342(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("@id", Decode_uri)
 
-    def _arrow1337(__unit: None=None) -> str | None:
+    def _arrow1343(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("name", string)
 
-    def _arrow1339(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
+    def _arrow1344(__unit: None=None) -> FSharpList[MaterialAttributeValue] | None:
         arg_5: Decoder_1[FSharpList[MaterialAttributeValue]] = list_1_3(MaterialAttributeValue_ISAJson_decoder)
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("characteristics", arg_5)
 
-    def _arrow1340(__unit: None=None) -> FSharpList[FactorValue] | None:
+    def _arrow1345(__unit: None=None) -> FSharpList[FactorValue] | None:
         arg_7: Decoder_1[FSharpList[FactorValue]] = list_1_3(FactorValue_ISAJson_decoder)
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("factorValues", arg_7)
 
-    def _arrow1342(__unit: None=None) -> FSharpList[Source] | None:
+    def _arrow1346(__unit: None=None) -> FSharpList[Source] | None:
         arg_9: Decoder_1[FSharpList[Source]] = list_1_3(Source_ISAJson_decoder)
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("derivesFrom", arg_9)
 
-    return Sample(_arrow1336(), _arrow1337(), _arrow1339(), _arrow1340(), _arrow1342())
+    return Sample(_arrow1342(), _arrow1343(), _arrow1344(), _arrow1345(), _arrow1346())
 
 
-Sample_ISAJson_decoder: Decoder_1[Sample] = Decode_objectNoAdditionalProperties(Sample_ISAJson_allowedFields, _arrow1343)
+Sample_ISAJson_decoder: Decoder_1[Sample] = Decode_objectNoAdditionalProperties(Sample_ISAJson_allowedFields, _arrow1347)
 
 def ARCtrl_Process_Sample__Sample_fromISAJsonString_Static_Z721C83C5(s: str) -> Sample:
     match_value: FSharpResult_2[Sample, str] = Decode_fromString(Sample_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Sample__Sample_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Sample], str]:
-    def _arrow1346(f: Sample, spaces: Any=spaces) -> str:
+    def _arrow1348(f: Sample, spaces: Any=spaces) -> str:
         value: Json = Sample_ISAJson_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1346
+    return _arrow1348
 
 
 def ARCtrl_Process_Sample__Sample_fromROCrateString_Static_Z721C83C5(s: str) -> Sample:
     match_value: FSharpResult_2[Sample, str] = Decode_fromString(Sample_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Process_Sample__Sample_toROCrateString_Static_71136F3F(spaces: int | None=None) -> Callable[[Sample], str]:
-    def _arrow1348(f: Sample, spaces: Any=spaces) -> str:
+    def _arrow1349(f: Sample, spaces: Any=spaces) -> str:
         value: Json = Sample_ROCrate_encoder(f)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1348
+    return _arrow1349
 
 
 __all__ = ["Sample_ROCrate_genID", "Sample_ROCrate_encoder", "Sample_ROCrate_additionalPropertyDecoder", "Sample_ROCrate_decoder", "Sample_ISAJson_encoder", "Sample_ISAJson_allowedFields", "Sample_ISAJson_decoder", "ARCtrl_Process_Sample__Sample_fromISAJsonString_Static_Z721C83C5", "ARCtrl_Process_Sample__Sample_toISAJsonString_Static_71136F3F", "ARCtrl_Process_Sample__Sample_fromROCrateString_Static_Z721C83C5", "ARCtrl_Process_Sample__Sample_toROCrateString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/source.py` & `arctrl-2.0.0a3/arctrl/Json/Process/source.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/study_materials.py` & `arctrl-2.0.0a3/arctrl/Json/Process/study_materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1367(oa: Source, ps: Any=ps) -> Json:
+    def _arrow1410(oa: Source, ps: Any=ps) -> Json:
         return Source_ISAJson_encoder(oa)
 
-    def _arrow1368(oa_1: Sample, ps: Any=ps) -> Json:
+    def _arrow1411(oa_1: Sample, ps: Any=ps) -> Json:
         return Sample_ISAJson_encoder(oa_1)
 
-    def _arrow1369(oa_2: Material, ps: Any=ps) -> Json:
+    def _arrow1412(oa_2: Material, ps: Any=ps) -> Json:
         return Material_ISAJson_encoder(oa_2)
 
-    return Json(5, choose(chooser, of_array([try_include_list("sources", _arrow1367, source), try_include_list("samples", _arrow1368, samples), try_include_list("otherMaterials", _arrow1369, materials)])))
+    return Json(5, choose(chooser, of_array([try_include_list("sources", _arrow1410, source), try_include_list("samples", _arrow1411, samples), try_include_list("otherMaterials", _arrow1412, materials)])))
 
 
 __all__ = ["encoder"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Process/value.py` & `arctrl-2.0.0a3/arctrl/Json/Process/value.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/publication.py` & `arctrl-2.0.0a3/arctrl/Json/publication.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,65 +26,65 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1042(value: str, oa: Any=oa) -> Json:
+    def _arrow1086(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1043(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1088(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1044(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1089(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1045(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1090(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1046(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
+    def _arrow1092(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
         return OntologyAnnotation_encoder(oa_1)
 
-    def _arrow1047(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow1094(comment: Comment, oa: Any=oa) -> Json:
         return Comment_encoder(comment)
 
-    return Json(5, choose(chooser, of_array([try_include("pubMedID", _arrow1042, oa.PubMedID), try_include("doi", _arrow1043, oa.DOI), try_include("authorList", _arrow1044, oa.Authors), try_include("title", _arrow1045, oa.Title), try_include("status", _arrow1046, oa.Status), try_include_seq("comments", _arrow1047, oa.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("pubMedID", _arrow1086, oa.PubMedID), try_include("doi", _arrow1088, oa.DOI), try_include("authorList", _arrow1089, oa.Authors), try_include("title", _arrow1090, oa.Title), try_include("status", _arrow1092, oa.Status), try_include_seq("comments", _arrow1094, oa.Comments)])))
 
 
-def _arrow1054(get: IGetters) -> Publication:
-    def _arrow1048(__unit: None=None) -> str | None:
+def _arrow1105(get: IGetters) -> Publication:
+    def _arrow1097(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("pubMedID", Decode_uri)
 
-    def _arrow1049(__unit: None=None) -> str | None:
+    def _arrow1098(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("doi", string)
 
-    def _arrow1050(__unit: None=None) -> str | None:
+    def _arrow1099(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("authorList", string)
 
-    def _arrow1051(__unit: None=None) -> str | None:
+    def _arrow1100(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("title", string)
 
-    def _arrow1052(__unit: None=None) -> OntologyAnnotation | None:
+    def _arrow1103(__unit: None=None) -> OntologyAnnotation | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("status", OntologyAnnotation_decoder)
 
-    def _arrow1053(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1104(__unit: None=None) -> Array[Comment] | None:
         arg_11: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_decoder)
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("comments", arg_11)
 
-    return Publication(_arrow1048(), _arrow1049(), _arrow1050(), _arrow1051(), _arrow1052(), _arrow1053())
+    return Publication(_arrow1097(), _arrow1098(), _arrow1099(), _arrow1100(), _arrow1103(), _arrow1104())
 
 
-Publication_decoder: Decoder_1[Publication] = object(_arrow1054)
+Publication_decoder: Decoder_1[Publication] = object(_arrow1105)
 
 def Publication_ROCrate_genID(p: Publication) -> str:
     match_value: str | None = p.DOI
     if match_value is None:
         match_value_1: str | None = p.PubMedID
         if match_value_1 is None:
             match_value_2: str | None = p.Title
@@ -110,92 +110,92 @@
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1055(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1112(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1056(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1114(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1057(author_list: str, oa: Any=oa) -> Json:
+    def _arrow1116(author_list: str, oa: Any=oa) -> Json:
         return Person_ROCrate_encodeAuthorListString(author_list)
 
-    def _arrow1058(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1118(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1059(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
+    def _arrow1120(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
         return OntologyAnnotation_ROCrate_encoderDefinedTerm(oa_1)
 
-    def _arrow1060(comment: Comment, oa: Any=oa) -> Json:
+    def _arrow1122(comment: Comment, oa: Any=oa) -> Json:
         return Comment_ROCrate_encoderDisambiguatingDescription(comment)
 
-    return Json(5, choose(chooser, of_array([("@id", Json(0, Publication_ROCrate_genID(oa))), ("@type", Json(0, "Publication")), try_include("pubMedID", _arrow1055, oa.PubMedID), try_include("doi", _arrow1056, oa.DOI), try_include("authorList", _arrow1057, oa.Authors), try_include("title", _arrow1058, oa.Title), try_include("status", _arrow1059, oa.Status), try_include_seq("comments", _arrow1060, oa.Comments), ("@context", context_jsonvalue)])))
+    return Json(5, choose(chooser, of_array([("@id", Json(0, Publication_ROCrate_genID(oa))), ("@type", Json(0, "Publication")), try_include("pubMedID", _arrow1112, oa.PubMedID), try_include("doi", _arrow1114, oa.DOI), try_include("authorList", _arrow1116, oa.Authors), try_include("title", _arrow1118, oa.Title), try_include("status", _arrow1120, oa.Status), try_include_seq("comments", _arrow1122, oa.Comments), ("@context", context_jsonvalue)])))
 
 
-def _arrow1067(get: IGetters) -> Publication:
-    def _arrow1061(__unit: None=None) -> str | None:
+def _arrow1136(get: IGetters) -> Publication:
+    def _arrow1123(__unit: None=None) -> str | None:
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("pubMedID", Decode_uri)
 
-    def _arrow1062(__unit: None=None) -> str | None:
+    def _arrow1125(__unit: None=None) -> str | None:
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("doi", string)
 
-    def _arrow1063(__unit: None=None) -> str | None:
+    def _arrow1127(__unit: None=None) -> str | None:
         object_arg_2: IOptionalGetter = get.Optional
         return object_arg_2.Field("authorList", Person_ROCrate_decodeAuthorListString)
 
-    def _arrow1064(__unit: None=None) -> str | None:
+    def _arrow1128(__unit: None=None) -> str | None:
         object_arg_3: IOptionalGetter = get.Optional
         return object_arg_3.Field("title", string)
 
-    def _arrow1065(__unit: None=None) -> OntologyAnnotation | None:
+    def _arrow1131(__unit: None=None) -> OntologyAnnotation | None:
         object_arg_4: IOptionalGetter = get.Optional
         return object_arg_4.Field("status", OntologyAnnotation_ROCrate_decoderDefinedTerm)
 
-    def _arrow1066(__unit: None=None) -> Array[Comment] | None:
+    def _arrow1135(__unit: None=None) -> Array[Comment] | None:
         arg_11: Decoder_1[Array[Comment]] = Decode_resizeArray(Comment_ROCrate_decoderDisambiguatingDescription)
         object_arg_5: IOptionalGetter = get.Optional
         return object_arg_5.Field("comments", arg_11)
 
-    return Publication(_arrow1061(), _arrow1062(), _arrow1063(), _arrow1064(), _arrow1065(), _arrow1066())
+    return Publication(_arrow1123(), _arrow1125(), _arrow1127(), _arrow1128(), _arrow1131(), _arrow1135())
 
 
-Publication_ROCrate_decoder: Decoder_1[Publication] = object(_arrow1067)
+Publication_ROCrate_decoder: Decoder_1[Publication] = object(_arrow1136)
 
 def Publication_ISAJson_encoder(oa: Publication) -> Json:
     def chooser(tupled_arg: tuple[str, Json], oa: Any=oa) -> tuple[str, Json] | None:
         v: Json = tupled_arg[1]
         if equals(v, Json(3)):
             return None
 
         else: 
             return (tupled_arg[0], v)
 
 
-    def _arrow1069(value: str, oa: Any=oa) -> Json:
+    def _arrow1142(value: str, oa: Any=oa) -> Json:
         return Json(0, value)
 
-    def _arrow1070(value_2: str, oa: Any=oa) -> Json:
+    def _arrow1143(value_2: str, oa: Any=oa) -> Json:
         return Json(0, value_2)
 
-    def _arrow1071(value_4: str, oa: Any=oa) -> Json:
+    def _arrow1144(value_4: str, oa: Any=oa) -> Json:
         return Json(0, value_4)
 
-    def _arrow1072(value_6: str, oa: Any=oa) -> Json:
+    def _arrow1145(value_6: str, oa: Any=oa) -> Json:
         return Json(0, value_6)
 
-    def _arrow1073(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
+    def _arrow1146(oa_1: OntologyAnnotation, oa: Any=oa) -> Json:
         return OntologyAnnotation_encoder(oa_1)
 
-    return Json(5, choose(chooser, of_array([try_include("pubMedID", _arrow1069, oa.PubMedID), try_include("doi", _arrow1070, oa.DOI), try_include("authorList", _arrow1071, oa.Authors), try_include("title", _arrow1072, oa.Title), try_include("status", _arrow1073, oa.Status), try_include_seq("comments", Comment_ISAJson_encoder, oa.Comments)])))
+    return Json(5, choose(chooser, of_array([try_include("pubMedID", _arrow1142, oa.PubMedID), try_include("doi", _arrow1143, oa.DOI), try_include("authorList", _arrow1144, oa.Authors), try_include("title", _arrow1145, oa.Title), try_include("status", _arrow1146, oa.Status), try_include_seq("comments", Comment_ISAJson_encoder, oa.Comments)])))
 
 
 Publication_ISAJson_allowedFields: FSharpList[str] = of_array(["pubMedID", "doi", "authorList", "title", "status", "comments"])
 
 Publication_ISAJson_decoder: Decoder_1[Publication] = Decode_noAdditionalProperties(Publication_ISAJson_allowedFields, Publication_decoder)
 
 def ARCtrl_Publication__Publication_fromJsonString_Static_Z721C83C5(s: str) -> Publication:
@@ -205,45 +205,45 @@
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Publication__Publication_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Publication], str]:
-    def _arrow1074(obj: Publication, spaces: Any=spaces) -> str:
+    def _arrow1149(obj: Publication, spaces: Any=spaces) -> str:
         value: Json = Publication_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1074
+    return _arrow1149
 
 
 def ARCtrl_Publication__Publication_fromROCrateJsonString_Static_Z721C83C5(s: str) -> Publication:
     match_value: FSharpResult_2[Publication, str] = Decode_fromString(Publication_ROCrate_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_Publication__Publication_toROCrateJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Publication], str]:
-    def _arrow1075(obj: Publication, spaces: Any=spaces) -> str:
+    def _arrow1151(obj: Publication, spaces: Any=spaces) -> str:
         value: Json = Publication_ROCrate_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1075
+    return _arrow1151
 
 
 def ARCtrl_Publication__Publication_toISAJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Publication], str]:
-    def _arrow1076(obj: Publication, spaces: Any=spaces) -> str:
+    def _arrow1152(obj: Publication, spaces: Any=spaces) -> str:
         value: Json = Publication_ISAJson_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1076
+    return _arrow1152
 
 
 def ARCtrl_Publication__Publication_fromISAJsonString_Static_Z721C83C5(s: str) -> Publication:
     match_value: FSharpResult_2[Publication, str] = Decode_fromString(Publication_ISAJson_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/string_table.py` & `arctrl-2.0.0a3/arctrl/Json/string_table.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/study.py` & `arctrl-2.0.0a3/arctrl/Json/study.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ..fable_modules.thoth_json_core.types import (Json, Decoder_1)
 from ..fable_modules.thoth_json_python.decode import Decode_fromString
 from ..fable_modules.thoth_json_python.encode import to_string
 from ..Core.arc_types import (ArcAssay, ArcStudy)
 from ..Core.comment import Comment
 from ..Core.conversion import (ARCtrl_ArcTables__ArcTables_GetProcesses, ARCtrl_ArcTables__ArcTables_fromProcesses_Static_62A3309D, Person_setSourceAssayComment, Person_getSourceAssayIdentifiersFromComments, Person_removeSourceAssayComments)
 from ..Core.Helper.collections_ import (ResizeArray_map, Option_fromValueWithDefault)
-from ..Core.Helper.identifier import (Study_tryFileNameFromIdentifier, Study_tryIdentifierFromFileName, create_missing_identifier, Assay_fileNameFromIdentifier)
+from ..Core.Helper.identifier import (Study_tryFileNameFromIdentifier, Study_tryIdentifierFromFileName, create_missing_identifier, Study_fileNameFromIdentifier)
 from ..Core.ontology_annotation import OntologyAnnotation
 from ..Core.person import Person
 from ..Core.Process.factor import Factor
 from ..Core.Process.material_attribute import MaterialAttribute
 from ..Core.Process.process import Process
 from ..Core.Process.process_sequence import (get_protocols, get_factors, get_characteristics, get_units)
 from ..Core.Process.protocol import Protocol
@@ -391,15 +391,15 @@
     return (ArcStudy(identifier, _arrow1639(), _arrow1640(), _arrow1641(), _arrow1642(), _arrow1643(), _arrow1644(), _arrow1645(), tables, assay_identifiers, _arrow1646()), default_arg(assays, empty()))
 
 
 Study_ROCrate_decoder: Decoder_1[tuple[ArcStudy, FSharpList[ArcAssay]]] = object(_arrow1647)
 
 def Study_ISAJson_encoder(assays: FSharpList[ArcAssay] | None, s: ArcStudy) -> Json:
     study: ArcStudy = s.Copy(True)
-    file_name: str = Assay_fileNameFromIdentifier(study.Identifier)
+    file_name: str = Study_fileNameFromIdentifier(study.Identifier)
     assays_1: Array[ArcAssay]
     n: Array[ArcAssay] = []
     enumerator: Any = get_enumerator(Study_Helper_getAssayInformation(assays, study))
     try: 
         while enumerator.System_Collections_IEnumerator_MoveNext():
             a: ArcAssay = enumerator.System_Collections_Generic_IEnumerator_1_get_Current()
             assay: ArcAssay = a.Copy()
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/arc_table.py` & `arctrl-2.0.0a3/arctrl/Json/Table/arc_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,135 +68,135 @@
             return append(singleton(("header", list_1(to_list(delay(_arrow1435))))) if (len(table.Headers) != 0) else empty(), delay(_arrow1441))
 
         return append(singleton(("name", Json(0, table.Name))), delay(_arrow1442))
 
     return Json(5, to_list(delay(_arrow1443)))
 
 
-def _arrow1450(get: IGetters) -> ArcTable:
+def _arrow1449(get: IGetters) -> ArcTable:
     def _arrow1444(__unit: None=None) -> FSharpList[CompositeHeader] | None:
         arg_1: Decoder_1[FSharpList[CompositeHeader]] = list_1_1(CompositeHeader_decoder)
         object_arg: IOptionalGetter = get.Optional
         return object_arg.Field("header", arg_1)
 
     decoded_header: Array[CompositeHeader] = list(default_arg(_arrow1444(), empty_1()))
     def _arrow1445(__unit: None=None) -> Any | None:
         arg_3: Decoder_1[Any] = map_0027(tuple2_1(int_1, int_1), CompositeCell_decoder)
         object_arg_1: IOptionalGetter = get.Optional
         return object_arg_1.Field("values", arg_3)
 
-    class ObjectExpr1447:
+    class ObjectExpr1446:
         @property
         def Compare(self) -> Callable[[tuple[int, int], tuple[int, int]], int]:
             return compare_arrays
 
-    class ObjectExpr1448:
+    class ObjectExpr1447:
         @property
         def Equals(self) -> Callable[[tuple[int, int], tuple[int, int]], bool]:
             return equal_arrays
 
         @property
         def GetHashCode(self) -> Callable[[tuple[int, int]], int]:
             return array_hash
 
-    decoded_values: Any = Dictionary(default_arg(_arrow1445(), empty_2(ObjectExpr1447())), ObjectExpr1448())
-    def _arrow1449(__unit: None=None) -> str:
+    decoded_values: Any = Dictionary(default_arg(_arrow1445(), empty_2(ObjectExpr1446())), ObjectExpr1447())
+    def _arrow1448(__unit: None=None) -> str:
         object_arg_2: IRequiredGetter = get.Required
         return object_arg_2.Field("name", string)
 
-    return ArcTable.create(_arrow1449(), decoded_header, decoded_values)
+    return ArcTable.create(_arrow1448(), decoded_header, decoded_values)
 
 
-ArcTable_decoder: Decoder_1[ArcTable] = object(_arrow1450)
+ArcTable_decoder: Decoder_1[ArcTable] = object(_arrow1449)
 
 def ArcTable_encoderCompressedColumn(column_index: int, row_count: int, cell_table: Any, table: ArcTable) -> Json:
     if True if table.Headers[column_index].IsIOType else (row_count < 100):
-        def _arrow1453(__unit: None=None, column_index: Any=column_index, row_count: Any=row_count, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[Json]:
-            def _arrow1452(r: int) -> Json:
+        def _arrow1451(__unit: None=None, column_index: Any=column_index, row_count: Any=row_count, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[Json]:
+            def _arrow1450(r: int) -> Json:
                 return encode_cell(cell_table, get_item_from_dict(table.Values, (column_index, r)))
 
-            return map(_arrow1452, range_big_int(0, 1, row_count - 1))
+            return map(_arrow1450, range_big_int(0, 1, row_count - 1))
 
-        return Json(6, to_array(delay(_arrow1453)))
+        return Json(6, to_array(delay(_arrow1451)))
 
     else: 
         current: CompositeCell = get_item_from_dict(table.Values, (column_index, 0))
         from_: int = 0
-        def _arrow1464(__unit: None=None, column_index: Any=column_index, row_count: Any=row_count, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[Json]:
-            def _arrow1460(i: int) -> IEnumerable_1[Json]:
+        def _arrow1459(__unit: None=None, column_index: Any=column_index, row_count: Any=row_count, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[Json]:
+            def _arrow1455(i: int) -> IEnumerable_1[Json]:
                 next_1: CompositeCell = get_item_from_dict(table.Values, (column_index, i))
-                def _arrow1456(__unit: None=None) -> Json:
+                def _arrow1452(__unit: None=None) -> Json:
                     value: int = from_ or 0
                     return Json(7, int(value+0x100000000 if value < 0 else value))
 
-                def _arrow1458(__unit: None=None) -> Json:
+                def _arrow1453(__unit: None=None) -> Json:
                     value_1: int = (i - 1) or 0
                     return Json(7, int(value_1+0x100000000 if value_1 < 0 else value_1))
 
-                def _arrow1459(__unit: None=None) -> IEnumerable_1[Json]:
+                def _arrow1454(__unit: None=None) -> IEnumerable_1[Json]:
                     nonlocal current, from_
                     current = next_1
                     from_ = i or 0
                     return empty()
 
-                return append(singleton(Json(5, to_enumerable([("f", _arrow1456()), ("t", _arrow1458()), ("v", encode_cell(cell_table, current))]))), delay(_arrow1459)) if (not equals(next_1, current)) else empty()
+                return append(singleton(Json(5, to_enumerable([("f", _arrow1452()), ("t", _arrow1453()), ("v", encode_cell(cell_table, current))]))), delay(_arrow1454)) if (not equals(next_1, current)) else empty()
 
-            def _arrow1463(__unit: None=None) -> IEnumerable_1[Json]:
-                def _arrow1461(__unit: None=None) -> Json:
+            def _arrow1458(__unit: None=None) -> IEnumerable_1[Json]:
+                def _arrow1456(__unit: None=None) -> Json:
                     value_2: int = from_ or 0
                     return Json(7, int(value_2+0x100000000 if value_2 < 0 else value_2))
 
-                def _arrow1462(__unit: None=None) -> Json:
+                def _arrow1457(__unit: None=None) -> Json:
                     value_3: int = (row_count - 1) or 0
                     return Json(7, int(value_3+0x100000000 if value_3 < 0 else value_3))
 
-                return singleton(Json(5, to_enumerable([("f", _arrow1461()), ("t", _arrow1462()), ("v", encode_cell(cell_table, current))])))
+                return singleton(Json(5, to_enumerable([("f", _arrow1456()), ("t", _arrow1457()), ("v", encode_cell(cell_table, current))])))
 
-            return append(collect(_arrow1460, range_big_int(1, 1, row_count - 1)), delay(_arrow1463))
+            return append(collect(_arrow1455, range_big_int(1, 1, row_count - 1)), delay(_arrow1458))
 
-        return Json(6, to_array(delay(_arrow1464)))
+        return Json(6, to_array(delay(_arrow1459)))
 
 
 
 def ArcTable_decoderCompressedColumn(cell_table: Array[CompositeCell], table: ArcTable, column_index: int) -> Decoder_1[None]:
-    class ObjectExpr1479(Decoder_1[None]):
+    class ObjectExpr1461(Decoder_1[None]):
         def Decode(self, helper: IDecoderHelpers_1[__A_], column: __A_, cell_table: Any=cell_table, table: Any=table, column_index: Any=column_index) -> FSharpResult_2[None, tuple[str, ErrorReason_1[__A_]]]:
             match_value: FSharpResult_2[Array[CompositeCell], tuple[str, ErrorReason_1[__A_]]] = array_1(decode_cell(cell_table)).Decode(helper, column)
             if match_value.tag == 1:
-                def _arrow1476(get: IGetters) -> None:
+                def _arrow1460(get: IGetters) -> None:
                     from_: int
                     object_arg: IRequiredGetter = get.Required
                     from_ = object_arg.Field("f", int_1)
                     to_: int
                     object_arg_1: IRequiredGetter = get.Required
                     to_ = object_arg_1.Field("t", int_1)
                     value: CompositeCell
                     arg_5: Decoder_1[CompositeCell] = decode_cell(cell_table)
                     object_arg_2: IRequiredGetter = get.Required
                     value = object_arg_2.Field("v", arg_5)
                     for i in range(from_, to_ + 1, 1):
                         add_to_dict(table.Values, (column_index, i), value)
 
-                range_decoder: Decoder_1[None] = object(_arrow1476)
+                range_decoder: Decoder_1[None] = object(_arrow1460)
                 match_value_1: FSharpResult_2[Array[None], tuple[str, ErrorReason_1[__A_]]] = array_1(range_decoder).Decode(helper, column)
                 return FSharpResult_2(1, match_value_1.fields[0]) if (match_value_1.tag == 1) else FSharpResult_2(0, None)
 
             else: 
                 def action(r: int, cell: CompositeCell) -> None:
                     add_to_dict(table.Values, (column_index, r), cell)
 
                 iterate_indexed(action, match_value.fields[0])
                 return FSharpResult_2(0, None)
 
 
-    return ObjectExpr1479()
+    return ObjectExpr1461()
 
 
 def ArcTable_arrayi(decoderi: Callable[[int], Decoder_1[_VALUE]]) -> Decoder_1[Array[_VALUE]]:
-    class ObjectExpr1485(Decoder_1[Array[_VALUE_]]):
+    class ObjectExpr1463(Decoder_1[Array[_VALUE_]]):
         def Decode(self, helpers: IDecoderHelpers_1[__A_], value: __A_, decoderi: Any=decoderi) -> FSharpResult_2[Array[_VALUE_], tuple[str, ErrorReason_1[__A_]]]:
             if helpers.is_array(value):
                 i: int = -1
                 tokens: Array[__A_] = helpers.as_array(value)
                 def folder(acc: FSharpResult_2[Array[_VALUE_], tuple[str, ErrorReason_1[__A_]]], value_1: __A_) -> FSharpResult_2[Array[_VALUE_], tuple[str, ErrorReason_1[__A_]]]:
                     nonlocal i
                     i = (i + 1) or 0
@@ -204,177 +204,177 @@
                         acc_1: Array[_VALUE_] = acc.fields[0]
                         match_value: FSharpResult_2[_VALUE_, tuple[str, ErrorReason_1[__A_]]] = decoderi(i).Decode(helpers, value_1)
                         if match_value.tag == 0:
                             acc_1[i] = match_value.fields[0]
                             return FSharpResult_2(0, acc_1)
 
                         else: 
-                            def _arrow1482(__unit: None=None, acc: Any=acc, value_1: Any=value_1) -> tuple[str, ErrorReason_1[__A_]]:
+                            def _arrow1462(__unit: None=None, acc: Any=acc, value_1: Any=value_1) -> tuple[str, ErrorReason_1[__A_]]:
                                 tupled_arg: tuple[str, ErrorReason_1[__A_]] = match_value.fields[0]
                                 return Helpers_prependPath((".[" + int32_to_string(i)) + "]", tupled_arg[0], tupled_arg[1])
 
-                            return FSharpResult_2(1, _arrow1482())
+                            return FSharpResult_2(1, _arrow1462())
 
 
                     else: 
                         return acc
 
 
                 return fold(folder, FSharpResult_2(0, fill([0] * len(tokens), 0, len(tokens), None)), tokens)
 
             else: 
                 return FSharpResult_2(1, ("", ErrorReason_1(0, "an array", value)))
 
 
-    return ObjectExpr1485()
+    return ObjectExpr1463()
 
 
 def ArcTable_encoderCompressed(string_table: Any, oa_table: Any, cell_table: Any, table: ArcTable) -> Json:
-    def _arrow1497(__unit: None=None, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[tuple[str, Json]]:
-        def _arrow1496(__unit: None=None) -> IEnumerable_1[tuple[str, Json]]:
-            def _arrow1490(__unit: None=None) -> IEnumerable_1[Json]:
+    def _arrow1469(__unit: None=None, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, table: Any=table) -> IEnumerable_1[tuple[str, Json]]:
+        def _arrow1468(__unit: None=None) -> IEnumerable_1[tuple[str, Json]]:
+            def _arrow1464(__unit: None=None) -> IEnumerable_1[Json]:
                 return map(CompositeHeader_encoder, table.Headers)
 
-            def _arrow1495(__unit: None=None) -> IEnumerable_1[tuple[str, Json]]:
+            def _arrow1467(__unit: None=None) -> IEnumerable_1[tuple[str, Json]]:
                 if len(table.Values) != 0:
                     row_count: int = table.RowCount or 0
-                    def _arrow1493(__unit: None=None) -> IEnumerable_1[Json]:
-                        def _arrow1492(c: int) -> Json:
+                    def _arrow1466(__unit: None=None) -> IEnumerable_1[Json]:
+                        def _arrow1465(c: int) -> Json:
                             return ArcTable_encoderCompressedColumn(c, row_count, cell_table, table)
 
-                        return map(_arrow1492, range_big_int(0, 1, table.ColumnCount - 1))
+                        return map(_arrow1465, range_big_int(0, 1, table.ColumnCount - 1))
 
-                    return singleton(("c", Json(6, to_array(delay(_arrow1493)))))
+                    return singleton(("c", Json(6, to_array(delay(_arrow1466)))))
 
                 else: 
                     return empty()
 
 
-            return append(singleton(("h", list_1(to_list(delay(_arrow1490))))) if (len(table.Headers) != 0) else empty(), delay(_arrow1495))
+            return append(singleton(("h", list_1(to_list(delay(_arrow1464))))) if (len(table.Headers) != 0) else empty(), delay(_arrow1467))
 
-        return append(singleton(("n", encode_string(string_table, table.Name))), delay(_arrow1496))
+        return append(singleton(("n", encode_string(string_table, table.Name))), delay(_arrow1468))
 
-    return Json(5, to_list(delay(_arrow1497)))
+    return Json(5, to_list(delay(_arrow1469)))
 
 
 def ArcTable_decoderCompressed(string_table: Array[str], oa_table: Array[OntologyAnnotation], cell_table: Array[CompositeCell]) -> Decoder_1[ArcTable]:
-    def _arrow1506(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> ArcTable:
-        def _arrow1501(__unit: None=None) -> FSharpList[CompositeHeader] | None:
+    def _arrow1475(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> ArcTable:
+        def _arrow1470(__unit: None=None) -> FSharpList[CompositeHeader] | None:
             arg_1: Decoder_1[FSharpList[CompositeHeader]] = list_1_1(CompositeHeader_decoder)
             object_arg: IOptionalGetter = get.Optional
             return object_arg.Field("h", arg_1)
 
-        decoded_header: Array[CompositeHeader] = list(default_arg(_arrow1501(), empty_1()))
-        def _arrow1502(__unit: None=None) -> str:
+        decoded_header: Array[CompositeHeader] = list(default_arg(_arrow1470(), empty_1()))
+        def _arrow1471(__unit: None=None) -> str:
             arg_3: Decoder_1[str] = decode_string(string_table)
             object_arg_1: IRequiredGetter = get.Required
             return object_arg_1.Field("n", arg_3)
 
-        class ObjectExpr1503:
+        class ObjectExpr1472:
             @property
             def Equals(self) -> Callable[[tuple[int, int], tuple[int, int]], bool]:
                 return equal_arrays
 
             @property
             def GetHashCode(self) -> Callable[[tuple[int, int]], int]:
                 return array_hash
 
-        table: ArcTable = ArcTable.create(_arrow1502(), decoded_header, Dictionary([], ObjectExpr1503()))
-        def _arrow1505(__unit: None=None) -> Array[None] | None:
-            def _arrow1504(column_index: int) -> Decoder_1[None]:
+        table: ArcTable = ArcTable.create(_arrow1471(), decoded_header, Dictionary([], ObjectExpr1472()))
+        def _arrow1474(__unit: None=None) -> Array[None] | None:
+            def _arrow1473(column_index: int) -> Decoder_1[None]:
                 return ArcTable_decoderCompressedColumn(cell_table, table, column_index)
 
-            arg_5: Decoder_1[Array[None]] = ArcTable_arrayi(_arrow1504)
+            arg_5: Decoder_1[Array[None]] = ArcTable_arrayi(_arrow1473)
             object_arg_2: IOptionalGetter = get.Optional
             return object_arg_2.Field("c", arg_5)
 
-        ignore(_arrow1505())
+        ignore(_arrow1474())
         return table
 
-    return object(_arrow1506)
+    return object(_arrow1475)
 
 
 def ARCtrl_ArcTable__ArcTable_fromJsonString_Static_Z721C83C5(s: str) -> ArcTable:
     match_value: FSharpResult_2[ArcTable, str] = Decode_fromString(ArcTable_decoder, s)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_ArcTable__ArcTable_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcTable], str]:
-    def _arrow1508(obj: ArcTable, spaces: Any=spaces) -> str:
+    def _arrow1476(obj: ArcTable, spaces: Any=spaces) -> str:
         value: Json = ArcTable_encoder(obj)
         return to_string(default_spaces(spaces), value)
 
-    return _arrow1508
+    return _arrow1476
 
 
 def ARCtrl_ArcTable__ArcTable_ToJsonString_71136F3F(this: ArcTable, spaces: int | None=None) -> str:
     return ARCtrl_ArcTable__ArcTable_toJsonString_Static_71136F3F(spaces)(this)
 
 
 def ARCtrl_ArcTable__ArcTable_fromCompressedJsonString_Static_Z721C83C5(json_string: str) -> ArcTable:
-    def _arrow1511(get: IGetters, json_string: Any=json_string) -> ArcTable:
+    def _arrow1478(get: IGetters, json_string: Any=json_string) -> ArcTable:
         string_table: Array[str]
         object_arg: IRequiredGetter = get.Required
         string_table = object_arg.Field("stringTable", decoder_2)
         oa_table: Array[OntologyAnnotation]
         arg_3: Decoder_1[Array[OntologyAnnotation]] = decoder_3(string_table)
         object_arg_1: IRequiredGetter = get.Required
         oa_table = object_arg_1.Field("oaTable", arg_3)
-        def _arrow1510(__unit: None=None) -> Array[CompositeCell]:
+        def _arrow1477(__unit: None=None) -> Array[CompositeCell]:
             arg_5: Decoder_1[Array[CompositeCell]] = decoder_4(string_table, oa_table)
             object_arg_2: IRequiredGetter = get.Required
             return object_arg_2.Field("cellTable", arg_5)
 
-        arg_7: Decoder_1[ArcTable] = ArcTable_decoderCompressed(string_table, oa_table, _arrow1510())
+        arg_7: Decoder_1[ArcTable] = ArcTable_decoderCompressed(string_table, oa_table, _arrow1477())
         object_arg_3: IRequiredGetter = get.Required
         return object_arg_3.Field("table", arg_7)
 
-    match_value: FSharpResult_2[ArcTable, str] = Decode_fromString(object(_arrow1511), json_string)
+    match_value: FSharpResult_2[ArcTable, str] = Decode_fromString(object(_arrow1478), json_string)
     if match_value.tag == 1:
         raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
 
     else: 
         return match_value.fields[0]
 
 
 
 def ARCtrl_ArcTable__ArcTable_ToCompressedJsonString_71136F3F(this: ArcTable, spaces: int | None=None) -> str:
     spaces_1: int = default_spaces(spaces) or 0
     string_table: Any = dict([])
-    class ObjectExpr1512:
+    class ObjectExpr1479:
         @property
         def Equals(self) -> Callable[[OntologyAnnotation, OntologyAnnotation], bool]:
             return equals
 
         @property
         def GetHashCode(self) -> Callable[[OntologyAnnotation], int]:
             return safe_hash
 
-    oa_table: Any = Dictionary([], ObjectExpr1512())
-    class ObjectExpr1513:
+    oa_table: Any = Dictionary([], ObjectExpr1479())
+    class ObjectExpr1480:
         @property
         def Equals(self) -> Callable[[CompositeCell, CompositeCell], bool]:
             return equals
 
         @property
         def GetHashCode(self) -> Callable[[CompositeCell], int]:
             return safe_hash
 
-    cell_table: Any = Dictionary([], ObjectExpr1513())
+    cell_table: Any = Dictionary([], ObjectExpr1480())
     arc_table: Json = ArcTable_encoderCompressed(string_table, oa_table, cell_table, this)
     return to_string(spaces_1, Json(5, to_enumerable([("cellTable", encoder(string_table, oa_table, array_from_map(cell_table))), ("oaTable", encoder_1(string_table, array_from_map_1(oa_table))), ("stringTable", encoder_2(array_from_map_2(string_table))), ("table", arc_table)])))
 
 
 def ARCtrl_ArcTable__ArcTable_toCompressedJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[ArcTable], str]:
-    def _arrow1514(obj: ArcTable, spaces: Any=spaces) -> str:
+    def _arrow1481(obj: ArcTable, spaces: Any=spaces) -> str:
         return ARCtrl_ArcTable__ArcTable_ToCompressedJsonString_71136F3F(obj, spaces)
 
-    return _arrow1514
+    return _arrow1481
 
 
 __all__ = ["ArcTable_encoder", "ArcTable_decoder", "ArcTable_encoderCompressedColumn", "ArcTable_decoderCompressedColumn", "ArcTable_arrayi", "ArcTable_encoderCompressed", "ArcTable_decoderCompressed", "ARCtrl_ArcTable__ArcTable_fromJsonString_Static_Z721C83C5", "ARCtrl_ArcTable__ArcTable_toJsonString_Static_71136F3F", "ARCtrl_ArcTable__ArcTable_ToJsonString_71136F3F", "ARCtrl_ArcTable__ArcTable_fromCompressedJsonString_Static_Z721C83C5", "ARCtrl_ArcTable__ArcTable_ToCompressedJsonString_71136F3F", "ARCtrl_ArcTable__ArcTable_toCompressedJsonString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/cell_table.py` & `arctrl-2.0.0a3/arctrl/Json/Table/cell_table.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/composite_cell.py` & `arctrl-2.0.0a3/arctrl/Json/Table/composite_cell.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/composite_header.py` & `arctrl-2.0.0a3/arctrl/Json/Table/composite_header.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/compression.py` & `arctrl-2.0.0a3/arctrl/Json/Table/compression.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/iotype.py` & `arctrl-2.0.0a3/arctrl/Json/Table/iotype.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/oatable.py` & `arctrl-2.0.0a3/arctrl/Json/Table/oatable.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Json/Table/templates.py` & `arctrl-2.0.0a3/arctrl/Json/Table/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,158 +20,158 @@
 from ..decode import (Decode_resizeArray, Decode_datetime)
 from ..encode import (try_include_seq, date_time, default_spaces)
 from ..ontology_annotation import (OntologyAnnotation_encoder, OntologyAnnotation_decoder)
 from ..person import (Person_encoder, Person_decoder)
 from .arc_table import (ArcTable_encoder, ArcTable_decoder, ArcTable_encoderCompressed, ArcTable_decoderCompressed)
 from .compression import (decode, encode)
 
-def _arrow1446(arg: Organisation) -> Json:
+def _arrow1482(arg: Organisation) -> Json:
     return Json(0, to_string(arg))
 
 
-Template_Organisation_encoder: Callable[[Organisation], Json] = _arrow1446
+Template_Organisation_encoder: Callable[[Organisation], Json] = _arrow1482
 
 def cb(text_value: str) -> Decoder_1[Organisation]:
     return succeed(Organisation.of_string(text_value))
 
 
 Template_Organisation_decoder: Decoder_1[Organisation] = and_then(cb, string)
 
 def Template_encoder(template: Template) -> Json:
-    def _arrow1451(__unit: None=None, template: Any=template) -> str:
+    def _arrow1483(__unit: None=None, template: Any=template) -> str:
         copy_of_struct: str = template.Id
         return str(copy_of_struct)
 
-    def _arrow1454(person: Person, template: Any=template) -> Json:
+    def _arrow1484(person: Person, template: Any=template) -> Json:
         return Person_encoder(person)
 
-    def _arrow1455(oa: OntologyAnnotation, template: Any=template) -> Json:
+    def _arrow1485(oa: OntologyAnnotation, template: Any=template) -> Json:
         return OntologyAnnotation_encoder(oa)
 
-    def _arrow1457(oa_1: OntologyAnnotation, template: Any=template) -> Json:
+    def _arrow1486(oa_1: OntologyAnnotation, template: Any=template) -> Json:
         return OntologyAnnotation_encoder(oa_1)
 
-    return Json(5, to_enumerable([("id", Json(0, _arrow1451())), ("table", ArcTable_encoder(template.Table)), ("name", Json(0, template.Name)), ("description", Json(0, template.Description)), ("organisation", Template_Organisation_encoder(template.Organisation)), ("version", Json(0, template.Version)), try_include_seq("authors", _arrow1454, template.Authors), try_include_seq("endpoint_repositories", _arrow1455, template.EndpointRepositories), try_include_seq("tags", _arrow1457, template.Tags), ("last_updated", date_time(template.LastUpdated))]))
+    return Json(5, to_enumerable([("id", Json(0, _arrow1483())), ("table", ArcTable_encoder(template.Table)), ("name", Json(0, template.Name)), ("description", Json(0, template.Description)), ("organisation", Template_Organisation_encoder(template.Organisation)), ("version", Json(0, template.Version)), try_include_seq("authors", _arrow1484, template.Authors), try_include_seq("endpoint_repositories", _arrow1485, template.EndpointRepositories), try_include_seq("tags", _arrow1486, template.Tags), ("last_updated", date_time(template.LastUpdated))]))
 
 
-def _arrow1475(get: IGetters) -> Template:
-    def _arrow1465(__unit: None=None) -> str:
+def _arrow1497(get: IGetters) -> Template:
+    def _arrow1487(__unit: None=None) -> str:
         object_arg: IRequiredGetter = get.Required
         return object_arg.Field("id", guid)
 
-    def _arrow1466(__unit: None=None) -> ArcTable:
+    def _arrow1488(__unit: None=None) -> ArcTable:
         object_arg_1: IRequiredGetter = get.Required
         return object_arg_1.Field("table", ArcTable_decoder)
 
-    def _arrow1467(__unit: None=None) -> str:
+    def _arrow1489(__unit: None=None) -> str:
         object_arg_2: IRequiredGetter = get.Required
         return object_arg_2.Field("name", string)
 
-    def _arrow1468(__unit: None=None) -> str:
+    def _arrow1490(__unit: None=None) -> str:
         object_arg_3: IRequiredGetter = get.Required
         return object_arg_3.Field("description", string)
 
-    def _arrow1469(__unit: None=None) -> Organisation:
+    def _arrow1491(__unit: None=None) -> Organisation:
         object_arg_4: IRequiredGetter = get.Required
         return object_arg_4.Field("organisation", Template_Organisation_decoder)
 
-    def _arrow1470(__unit: None=None) -> str:
+    def _arrow1492(__unit: None=None) -> str:
         object_arg_5: IRequiredGetter = get.Required
         return object_arg_5.Field("version", string)
 
-    def _arrow1471(__unit: None=None) -> Array[Person] | None:
+    def _arrow1493(__unit: None=None) -> Array[Person] | None:
         arg_13: Decoder_1[Array[Person]] = Decode_resizeArray(Person_decoder)
         object_arg_6: IOptionalGetter = get.Optional
         return object_arg_6.Field("authors", arg_13)
 
-    def _arrow1472(__unit: None=None) -> Array[OntologyAnnotation] | None:
+    def _arrow1494(__unit: None=None) -> Array[OntologyAnnotation] | None:
         arg_15: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
         object_arg_7: IOptionalGetter = get.Optional
         return object_arg_7.Field("endpoint_repositories", arg_15)
 
-    def _arrow1473(__unit: None=None) -> Array[OntologyAnnotation] | None:
+    def _arrow1495(__unit: None=None) -> Array[OntologyAnnotation] | None:
         arg_17: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
         object_arg_8: IOptionalGetter = get.Optional
         return object_arg_8.Field("tags", arg_17)
 
-    def _arrow1474(__unit: None=None) -> Any:
+    def _arrow1496(__unit: None=None) -> Any:
         object_arg_9: IRequiredGetter = get.Required
         return object_arg_9.Field("last_updated", Decode_datetime)
 
-    return Template.create(_arrow1465(), _arrow1466(), _arrow1467(), _arrow1468(), _arrow1469(), _arrow1470(), _arrow1471(), _arrow1472(), _arrow1473(), _arrow1474())
+    return Template.create(_arrow1487(), _arrow1488(), _arrow1489(), _arrow1490(), _arrow1491(), _arrow1492(), _arrow1493(), _arrow1494(), _arrow1495(), _arrow1496())
 
 
-Template_decoder: Decoder_1[Template] = object(_arrow1475)
+Template_decoder: Decoder_1[Template] = object(_arrow1497)
 
 def Template_encoderCompressed(string_table: Any, oa_table: Any, cell_table: Any, template: Template) -> Json:
-    def _arrow1477(__unit: None=None, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> str:
+    def _arrow1498(__unit: None=None, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> str:
         copy_of_struct: str = template.Id
         return str(copy_of_struct)
 
-    def _arrow1478(person: Person, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
+    def _arrow1499(person: Person, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
         return Person_encoder(person)
 
-    def _arrow1480(oa: OntologyAnnotation, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
+    def _arrow1500(oa: OntologyAnnotation, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
         return OntologyAnnotation_encoder(oa)
 
-    def _arrow1481(oa_1: OntologyAnnotation, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
+    def _arrow1501(oa_1: OntologyAnnotation, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table, template: Any=template) -> Json:
         return OntologyAnnotation_encoder(oa_1)
 
-    return Json(5, to_enumerable([("id", Json(0, _arrow1477())), ("table", ArcTable_encoderCompressed(string_table, oa_table, cell_table, template.Table)), ("name", Json(0, template.Name)), ("description", Json(0, template.Description)), ("organisation", Template_Organisation_encoder(template.Organisation)), ("version", Json(0, template.Version)), try_include_seq("authors", _arrow1478, template.Authors), try_include_seq("endpoint_repositories", _arrow1480, template.EndpointRepositories), try_include_seq("tags", _arrow1481, template.Tags), ("last_updated", Json(0, to_string_1(template.LastUpdated, "O", {})))]))
+    return Json(5, to_enumerable([("id", Json(0, _arrow1498())), ("table", ArcTable_encoderCompressed(string_table, oa_table, cell_table, template.Table)), ("name", Json(0, template.Name)), ("description", Json(0, template.Description)), ("organisation", Template_Organisation_encoder(template.Organisation)), ("version", Json(0, template.Version)), try_include_seq("authors", _arrow1499, template.Authors), try_include_seq("endpoint_repositories", _arrow1500, template.EndpointRepositories), try_include_seq("tags", _arrow1501, template.Tags), ("last_updated", Json(0, to_string_1(template.LastUpdated, "O", {})))]))
 
 
 def Template_decoderCompressed(string_table: Array[str], oa_table: Array[OntologyAnnotation], cell_table: Array[CompositeCell]) -> Decoder_1[Template]:
-    def _arrow1500(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> Template:
-        def _arrow1483(__unit: None=None) -> str:
+    def _arrow1512(get: IGetters, string_table: Any=string_table, oa_table: Any=oa_table, cell_table: Any=cell_table) -> Template:
+        def _arrow1502(__unit: None=None) -> str:
             object_arg: IRequiredGetter = get.Required
             return object_arg.Field("id", guid)
 
-        def _arrow1484(__unit: None=None) -> ArcTable:
+        def _arrow1503(__unit: None=None) -> ArcTable:
             arg_3: Decoder_1[ArcTable] = ArcTable_decoderCompressed(string_table, oa_table, cell_table)
             object_arg_1: IRequiredGetter = get.Required
             return object_arg_1.Field("table", arg_3)
 
-        def _arrow1486(__unit: None=None) -> str:
+        def _arrow1504(__unit: None=None) -> str:
             object_arg_2: IRequiredGetter = get.Required
             return object_arg_2.Field("name", string)
 
-        def _arrow1487(__unit: None=None) -> str:
+        def _arrow1505(__unit: None=None) -> str:
             object_arg_3: IRequiredGetter = get.Required
             return object_arg_3.Field("description", string)
 
-        def _arrow1488(__unit: None=None) -> Organisation:
+        def _arrow1506(__unit: None=None) -> Organisation:
             object_arg_4: IRequiredGetter = get.Required
             return object_arg_4.Field("organisation", Template_Organisation_decoder)
 
-        def _arrow1489(__unit: None=None) -> str:
+        def _arrow1507(__unit: None=None) -> str:
             object_arg_5: IRequiredGetter = get.Required
             return object_arg_5.Field("version", string)
 
-        def _arrow1491(__unit: None=None) -> Array[Person] | None:
+        def _arrow1508(__unit: None=None) -> Array[Person] | None:
             arg_13: Decoder_1[Array[Person]] = Decode_resizeArray(Person_decoder)
             object_arg_6: IOptionalGetter = get.Optional
             return object_arg_6.Field("authors", arg_13)
 
-        def _arrow1494(__unit: None=None) -> Array[OntologyAnnotation] | None:
+        def _arrow1509(__unit: None=None) -> Array[OntologyAnnotation] | None:
             arg_15: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
             object_arg_7: IOptionalGetter = get.Optional
             return object_arg_7.Field("endpoint_repositories", arg_15)
 
-        def _arrow1498(__unit: None=None) -> Array[OntologyAnnotation] | None:
+        def _arrow1510(__unit: None=None) -> Array[OntologyAnnotation] | None:
             arg_17: Decoder_1[Array[OntologyAnnotation]] = Decode_resizeArray(OntologyAnnotation_decoder)
             object_arg_8: IOptionalGetter = get.Optional
             return object_arg_8.Field("tags", arg_17)
 
-        def _arrow1499(__unit: None=None) -> Any:
+        def _arrow1511(__unit: None=None) -> Any:
             object_arg_9: IRequiredGetter = get.Required
             return object_arg_9.Field("last_updated", datetime_local)
 
-        return Template.create(_arrow1483(), _arrow1484(), _arrow1486(), _arrow1487(), _arrow1488(), _arrow1489(), _arrow1491(), _arrow1494(), _arrow1498(), _arrow1499())
+        return Template.create(_arrow1502(), _arrow1503(), _arrow1504(), _arrow1505(), _arrow1506(), _arrow1507(), _arrow1508(), _arrow1509(), _arrow1510(), _arrow1511())
 
-    return object(_arrow1500)
+    return object(_arrow1512)
 
 
 def Templates_encoder(templates: Array[Template]) -> Json:
     def mapping(template: Template, templates: Any=templates) -> Json:
         return Template_encoder(template)
 
     return Json(6, map(mapping, templates, None))
@@ -210,18 +210,18 @@
 
     except Exception as exn:
         return to_fail(printf("Error. Given json string cannot be parsed to Template: %A"))(exn)
 
 
 
 def ARCtrl_Template__Template_toJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Template], str]:
-    def _arrow1507(template: Template, spaces: Any=spaces) -> str:
+    def _arrow1513(template: Template, spaces: Any=spaces) -> str:
         return to_string_2(default_spaces(spaces), Template_encoder(template))
 
-    return _arrow1507
+    return _arrow1513
 
 
 def ARCtrl_Template__Template_fromCompressedJsonString_Static_Z721C83C5(s: str) -> Template:
     try: 
         match_value: FSharpResult_2[Template, str] = Decode_fromString(decode(Template_decoderCompressed), s)
         if match_value.tag == 1:
             raise Exception(to_text(printf("Error decoding string: %O"))(match_value.fields[0]))
@@ -233,15 +233,15 @@
     except Exception as e_1:
         arg_1: str = str(e_1)
         return to_fail(printf("Error. Unable to parse json string to ArcStudy: %s"))(arg_1)
 
 
 
 def ARCtrl_Template__Template_toCompressedJsonString_Static_71136F3F(spaces: int | None=None) -> Callable[[Template], str]:
-    def _arrow1509(obj: Template, spaces: Any=spaces) -> str:
+    def _arrow1514(obj: Template, spaces: Any=spaces) -> str:
         return to_string_2(default_arg(spaces, 0), encode(Template_encoderCompressed, obj))
 
-    return _arrow1509
+    return _arrow1514
 
 
 __all__ = ["Template_Organisation_encoder", "Template_Organisation_decoder", "Template_encoder", "Template_decoder", "Template_encoderCompressed", "Template_decoderCompressed", "Templates_encoder", "Templates_decoder", "Templates_fromJsonString", "Templates_toJsonString", "ARCtrl_Template__Template_fromJsonString_Static_Z721C83C5", "ARCtrl_Template__Template_toJsonString_Static_71136F3F", "ARCtrl_Template__Template_fromCompressedJsonString_Static_Z721C83C5", "ARCtrl_Template__Template_toCompressedJsonString_Static_71136F3F"]
```

### Comparing `arctrl-2.0.0a2/arctrl/json.py` & `arctrl-2.0.0a3/arctrl/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
 JsonHelper_ARCJson_reflection = _expr1812
 
 def JsonHelper_ARCJson__ctor(__unit: None=None) -> JsonHelper_ARCJson:
     return JsonHelper_ARCJson(__unit)
 
 
-def _expr1813() -> TypeInfo:
+def _expr1814() -> TypeInfo:
     return class_type("ARCtrl.JsonController", None, JsonController)
 
 
 class JsonController:
     @staticmethod
     def OntologyAnnotation() -> JsonHelper_OntologyAnnotationJson:
         return JsonHelper_OntologyAnnotationJson()
@@ -203,11 +203,11 @@
         return JsonHelper_InvestigationJson()
 
     @staticmethod
     def ARC() -> JsonHelper_ARCJson:
         return JsonHelper_ARCJson()
 
 
-JsonController_reflection = _expr1813
+JsonController_reflection = _expr1814
 
 __all__ = ["JsonHelper_OntologyAnnotationJson_reflection", "JsonHelper_AssayJson_reflection", "JsonHelper_StudyJson_reflection", "JsonHelper_InvestigationJson_reflection", "JsonHelper_ARCJson_reflection", "JsonController_reflection"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/arc_table.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/arc_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,18 @@
     def predicate(t: FsTable, sheet: Any=sheet) -> bool:
         return t.Name.find("annotationTable") == 0
 
     return try_find(predicate, sheet.Tables)
 
 
 def compose_columns(columns: IEnumerable_1[FsColumn]) -> Array[CompositeColumn]:
-    def _arrow876(columns_2: FSharpList[FsColumn], columns: Any=columns) -> CompositeColumn:
+    def _arrow844(columns_2: FSharpList[FsColumn], columns: Any=columns) -> CompositeColumn:
         return from_fs_columns(columns_2)
 
-    return to_array(map(_arrow876, group_columns_by_header(to_list(columns))))
+    return to_array(map(_arrow844, group_columns_by_header(to_list(columns))))
 
 
 def try_from_fs_worksheet(sheet: FsWorksheet) -> ArcTable | None:
     try: 
         match_value: FsTable | None = try_annotation_table(sheet)
         if match_value is None:
             return None
@@ -111,26 +111,26 @@
 def to_fs_worksheet(table: ArcTable) -> FsWorksheet:
     string_count: Any = dict([])
     ws: FsWorksheet = FsWorksheet(table.Name)
     if len(table.Columns) == 0:
         return ws
 
     else: 
-        def _arrow877(column_1: CompositeColumn, table: Any=table) -> FSharpList[FSharpList[FsCell]]:
+        def _arrow845(column_1: CompositeColumn, table: Any=table) -> FSharpList[FSharpList[FsCell]]:
             return to_fs_columns(column_1)
 
-        def _arrow878(column: CompositeColumn, table: Any=table) -> enum_type("ARCtrl.Spreadsheet.ArcTable.ColumnOrder", int, [("InputClass", 1.0), ("ProtocolClass", 2.0), ("ParamsClass", 3.0), ("OutputClass", 4.0)]):
+        def _arrow846(column: CompositeColumn, table: Any=table) -> enum_type("ARCtrl.Spreadsheet.ArcTable.ColumnOrder", int, [("InputClass", 1.0), ("ProtocolClass", 2.0), ("ParamsClass", 3.0), ("OutputClass", 4.0)]):
             return classify_column_order(column)
 
-        class ObjectExpr879:
+        class ObjectExpr847:
             @property
             def Compare(self) -> Callable[[enum_type("ARCtrl.Spreadsheet.ArcTable.ColumnOrder", int, [("InputClass", 1.0), ("ProtocolClass", 2.0), ("ParamsClass", 3.0), ("OutputClass", 4.0)]), enum_type("ARCtrl.Spreadsheet.ArcTable.ColumnOrder", int, [("InputClass", 1.0), ("ProtocolClass", 2.0), ("ParamsClass", 3.0), ("OutputClass", 4.0)])], int]:
                 return compare_primitives
 
-        columns: FSharpList[FSharpList[FsCell]] = collect(_arrow877, sort_by(_arrow878, of_array(table.Columns), ObjectExpr879()))
+        columns: FSharpList[FSharpList[FsCell]] = collect(_arrow845, sort_by(_arrow846, of_array(table.Columns), ObjectExpr847()))
         max_row: int = length(head(columns)) or 0
         max_col: int = length(columns) or 0
         fs_table: FsTable = ws.Table("annotationTable", FsRangeAddress__ctor_7E77A4A0(FsAddress__ctor_Z37302880(1, 1), FsAddress__ctor_Z37302880(max_row, max_col)))
         def action_1(col_i: int, col: FSharpList[FsCell], table: Any=table) -> None:
             def action(row_i: int, cell: FsCell, col_i: Any=col_i, col: Any=col) -> None:
                 value: str
                 v: str = cell.ValueAsString()
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_cell.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_cell.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_column.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 
 def from_fs_columns(columns: FSharpList[FsColumn]) -> CompositeColumn:
     def mapping(c: FsColumn, columns: Any=columns) -> FsCell:
         return c.Item(1)
 
     header: CompositeHeader = from_fs_cells(map(mapping, columns))
     l: int = FsAddress__get_RowNumber(FsRangeAddress__get_LastAddress(FsRangeBase__get_RangeAddress(item(0, columns)))) or 0
-    def _arrow845(__unit: None=None, columns: Any=columns) -> IEnumerable_1[CompositeCell]:
-        def _arrow844(i: int) -> CompositeCell:
+    def _arrow849(__unit: None=None, columns: Any=columns) -> IEnumerable_1[CompositeCell]:
+        def _arrow848(i: int) -> CompositeCell:
             def mapping_1(c_1: FsColumn) -> FsCell:
                 return c_1.Item(i)
 
             return from_fs_cells_1(map(mapping_1, columns))
 
-        return map_1(_arrow844, range_big_int(2, 1, l))
+        return map_1(_arrow848, range_big_int(2, 1, l))
 
-    cells_2: Array[CompositeCell] = to_array(delay(_arrow845))
+    cells_2: Array[CompositeCell] = to_array(delay(_arrow849))
     return CompositeColumn.create(header, cells_2)
 
 
 def to_fs_columns(column: CompositeColumn) -> FSharpList[FSharpList[FsCell]]:
     def predicate(c: CompositeCell, column: Any=column) -> bool:
         return c.is_unitized
 
@@ -59,91 +59,91 @@
     is_term: bool = column.Header.IsTermColumn
     header: FSharpList[FsCell] = to_fs_cells(has_unit, column.Header)
     def mapping(cell: CompositeCell, column: Any=column) -> FSharpList[FsCell]:
         return to_fs_cells_1(is_term, has_unit, cell)
 
     cells: Array[FSharpList[FsCell]] = map_2(mapping, column.Cells, None)
     if has_unit:
-        def _arrow851(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow850(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow849(i: int) -> FsCell:
+        def _arrow855(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow854(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow853(i: int) -> FsCell:
                     return item(0, cells[i])
 
-                return map_1(_arrow849, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow853, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(0, header)), delay(_arrow850))
+            return append(singleton(item(0, header)), delay(_arrow854))
 
-        def _arrow854(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow853(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow852(i_1: int) -> FsCell:
+        def _arrow858(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow857(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow856(i_1: int) -> FsCell:
                     return item(1, cells[i_1])
 
-                return map_1(_arrow852, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow856, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(1, header)), delay(_arrow853))
+            return append(singleton(item(1, header)), delay(_arrow857))
 
-        def _arrow857(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow856(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow855(i_2: int) -> FsCell:
+        def _arrow861(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow860(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow859(i_2: int) -> FsCell:
                     return item(2, cells[i_2])
 
-                return map_1(_arrow855, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow859, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(2, header)), delay(_arrow856))
+            return append(singleton(item(2, header)), delay(_arrow860))
 
-        def _arrow860(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow859(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow858(i_3: int) -> FsCell:
+        def _arrow864(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow863(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow862(i_3: int) -> FsCell:
                     return item(3, cells[i_3])
 
-                return map_1(_arrow858, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow862, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(3, header)), delay(_arrow859))
+            return append(singleton(item(3, header)), delay(_arrow863))
 
-        return of_array([to_list(delay(_arrow851)), to_list(delay(_arrow854)), to_list(delay(_arrow857)), to_list(delay(_arrow860))])
+        return of_array([to_list(delay(_arrow855)), to_list(delay(_arrow858)), to_list(delay(_arrow861)), to_list(delay(_arrow864))])
 
     elif is_term:
-        def _arrow866(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow865(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow864(i_4: int) -> FsCell:
+        def _arrow870(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow869(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow868(i_4: int) -> FsCell:
                     return item(0, cells[i_4])
 
-                return map_1(_arrow864, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow868, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(0, header)), delay(_arrow865))
+            return append(singleton(item(0, header)), delay(_arrow869))
 
-        def _arrow869(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow868(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow867(i_5: int) -> FsCell:
+        def _arrow873(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow872(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow871(i_5: int) -> FsCell:
                     return item(1, cells[i_5])
 
-                return map_1(_arrow867, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow871, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(1, header)), delay(_arrow868))
+            return append(singleton(item(1, header)), delay(_arrow872))
 
-        def _arrow872(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow871(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow870(i_6: int) -> FsCell:
+        def _arrow876(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow875(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow874(i_6: int) -> FsCell:
                     return item(2, cells[i_6])
 
-                return map_1(_arrow870, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow874, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(2, header)), delay(_arrow871))
+            return append(singleton(item(2, header)), delay(_arrow875))
 
-        return of_array([to_list(delay(_arrow866)), to_list(delay(_arrow869)), to_list(delay(_arrow872))])
+        return of_array([to_list(delay(_arrow870)), to_list(delay(_arrow873)), to_list(delay(_arrow876))])
 
     else: 
-        def _arrow875(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
-            def _arrow874(__unit: None=None) -> IEnumerable_1[FsCell]:
-                def _arrow873(i_7: int) -> FsCell:
+        def _arrow879(__unit: None=None, column: Any=column) -> IEnumerable_1[FsCell]:
+            def _arrow878(__unit: None=None) -> IEnumerable_1[FsCell]:
+                def _arrow877(i_7: int) -> FsCell:
                     return item(0, cells[i_7])
 
-                return map_1(_arrow873, range_big_int(0, 1, len(column.Cells) - 1))
+                return map_1(_arrow877, range_big_int(0, 1, len(column.Cells) - 1))
 
-            return append(singleton(item(0, header)), delay(_arrow874))
+            return append(singleton(item(0, header)), delay(_arrow878))
 
-        return singleton_1(to_list(delay(_arrow875)))
+        return singleton_1(to_list(delay(_arrow879)))
 
 
 
 __all__ = ["fix_deprecated_ioheader", "from_fs_columns", "to_fs_columns"]
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/AnnotationTable/composite_header.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/AnnotationTable/composite_header.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/arc_assay.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/arc_assay.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/arc_investigation.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/arc_investigation.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/arc_study.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/arc_study.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/collection_aux.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/collection_aux.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/assays.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/assays.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/comment.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/comment.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/contacts.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/contacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,40 +37,40 @@
 roles_term_accession_number_label: str = "Roles Term Accession Number"
 
 roles_term_source_reflabel: str = "Roles Term Source REF"
 
 labels: FSharpList[str] = of_array([last_name_label, first_name_label, mid_initials_label, email_label, phone_label, fax_label, address_label, affiliation_label, roles_label, roles_term_accession_number_label, roles_term_source_reflabel])
 
 def from_string(last_name: str | None, first_name: str | None, mid_initials: str | None, email: str | None, phone: str | None, fax: str | None, address: str | None, affiliation: str | None, role: str, roles_term_accession_number: str, roles_term_source_ref: str, comments: Array[Comment]) -> Person:
-    def _arrow659(__unit: None=None, last_name: Any=last_name, first_name: Any=first_name, mid_initials: Any=mid_initials, email: Any=email, phone: Any=phone, fax: Any=fax, address: Any=address, affiliation: Any=affiliation, role: Any=role, roles_term_accession_number: Any=roles_term_accession_number, roles_term_source_ref: Any=roles_term_source_ref, comments: Any=comments) -> Person:
+    def _arrow724(__unit: None=None, last_name: Any=last_name, first_name: Any=first_name, mid_initials: Any=mid_initials, email: Any=email, phone: Any=phone, fax: Any=fax, address: Any=address, affiliation: Any=affiliation, role: Any=role, roles_term_accession_number: Any=roles_term_accession_number, roles_term_source_ref: Any=roles_term_source_ref, comments: Any=comments) -> Person:
         roles_1: Array[OntologyAnnotation] = OntologyAnnotation_fromAggregatedStrings(";", role, roles_term_source_ref, roles_term_accession_number)
         return Person.make(None, last_name, first_name, mid_initials, email, phone, fax, address, affiliation, roles_1, comments)
 
-    return Person_setOrcidFromComments(_arrow659())
+    return Person_setOrcidFromComments(_arrow724())
 
 
 def from_sparse_table(matrix: SparseTable) -> FSharpList[Person]:
     if (length(matrix.CommentKeys) != 0) if (matrix.ColumnCount == 0) else False:
         comments: Array[Comment] = SparseTable_GetEmptyComments_3ECCA699(matrix)
-        def _arrow664(__unit: None=None, matrix: Any=matrix) -> Person:
+        def _arrow725(__unit: None=None, matrix: Any=matrix) -> Person:
             return_val: Person = Person.create()
             return_val.Comments = comments
             return return_val
 
-        return singleton(_arrow664())
+        return singleton(_arrow725())
 
     else: 
-        def _arrow667(i: int, matrix: Any=matrix) -> Person:
+        def _arrow726(i: int, matrix: Any=matrix) -> Person:
             def mapping(k: str) -> Comment:
                 return Comment_fromString(k, SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (k, i)))
 
             comments_1: Array[Comment] = list(map(mapping, matrix.CommentKeys))
             return from_string(SparseTable__TryGetValue_11FD62A8(matrix, (last_name_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (first_name_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (mid_initials_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (email_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (phone_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (fax_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (address_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (affiliation_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (roles_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (roles_term_accession_number_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (roles_term_source_reflabel, i)), comments_1)
 
-        return initialize(matrix.ColumnCount, _arrow667)
+        return initialize(matrix.ColumnCount, _arrow726)
 
 
 
 def to_sparse_table(persons: FSharpList[Person]) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, labels, None, length(persons) + 1)
     comment_keys: FSharpList[str] = empty()
     def action(i: int, p: Person, persons: Any=persons) -> None:
@@ -96,27 +96,27 @@
 
         ResizeArray_iter(f, p.Comments)
 
     def mapping(person: Person, persons: Any=persons) -> Person:
         return Person_setCommentFromORCID(person)
 
     iterate_indexed(action, map(mapping, persons))
-    class ObjectExpr672:
+    class ObjectExpr728:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow671(x: str, y: str) -> bool:
+            def _arrow727(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow671
+            return _arrow727
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr672())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr728())), matrix.ColumnCount)
 
 
 def from_rows(prefix: str | None, line_number: int, rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, int, FSharpList[Remark], FSharpList[Person]]:
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, labels, line_number, prefix)
     return (tupled_arg[0], tupled_arg[1], tupled_arg[2], from_sparse_table(tupled_arg[3]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/conversions.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/conversions.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/design_descriptors.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/design_descriptors.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/factors.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/factors.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
 def from_sparse_table(matrix: SparseTable) -> FSharpList[Factor]:
     if (length(matrix.CommentKeys) != 0) if (matrix.ColumnCount == 0) else False:
         comments: Array[Comment] = SparseTable_GetEmptyComments_3ECCA699(matrix)
         return singleton(Factor.create(None, None, comments))
 
     else: 
-        def _arrow752(i: int, matrix: Any=matrix) -> Factor:
+        def _arrow772(i: int, matrix: Any=matrix) -> Factor:
             def mapping(k: str) -> Comment:
                 return Comment_fromString(k, SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (k, i)))
 
             comments_1: Array[Comment] = list(map(mapping, matrix.CommentKeys))
             return from_string(SparseTable__TryGetValue_11FD62A8(matrix, (name_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (factor_type_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (type_term_source_reflabel, i)), SparseTable__TryGetValue_11FD62A8(matrix, (type_term_accession_number_label, i)), comments_1)
 
-        return initialize(matrix.ColumnCount, _arrow752)
+        return initialize(matrix.ColumnCount, _arrow772)
 
 
 
 def to_sparse_table(factors: FSharpList[Factor]) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, labels, None, length(factors) + 1)
     comment_keys: FSharpList[str] = empty()
     def action(i: int, f: Factor, factors: Any=factors) -> None:
@@ -69,27 +69,27 @@
                 comment_keys = cons(n, comment_keys)
                 add_to_dict(matrix.Matrix, (n, i_1), pattern_input[1])
 
             ResizeArray_iter(f_2, match_value)
 
 
     iterate_indexed(action, factors)
-    class ObjectExpr754:
+    class ObjectExpr778:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow753(x: str, y: str) -> bool:
+            def _arrow777(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow753
+            return _arrow777
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr754())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr778())), matrix.ColumnCount)
 
 
 def from_rows(prefix: str | None, line_number: int, rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, int, FSharpList[Remark], FSharpList[Factor]]:
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, labels, line_number) if (prefix is None) else SparseTable_FromRows_Z5579EC29(rows, labels, line_number, prefix)
     return (tupled_arg[0], tupled_arg[1], tupled_arg[2], from_sparse_table(tupled_arg[3]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/ontology_annotation.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/ontology_annotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 from ...Core.ontology_annotation import OntologyAnnotation
 from .comment import (Comment_fromString, Comment_toString)
 from .sparse_table import (SparseTable_GetEmptyComments_3ECCA699, SparseTable__TryGetValueDefault_5BAE6133, SparseTable__TryGetValue_11FD62A8, SparseTable, SparseTable_Create_Z2192E64B, SparseTable_FromRows_Z5579EC29, SparseTable_ToRows_759CAFC1)
 
 def from_sparse_table(label: str, label_tsr: str, label_tan: str, matrix: SparseTable) -> FSharpList[OntologyAnnotation]:
     if (length(matrix.CommentKeys) != 0) if (matrix.ColumnCount == 0) else False:
         comments: Array[Comment] = SparseTable_GetEmptyComments_3ECCA699(matrix)
-        def _arrow654(__unit: None=None, label: Any=label, label_tsr: Any=label_tsr, label_tan: Any=label_tan, matrix: Any=matrix) -> OntologyAnnotation:
+        def _arrow729(__unit: None=None, label: Any=label, label_tsr: Any=label_tsr, label_tan: Any=label_tan, matrix: Any=matrix) -> OntologyAnnotation:
             return_val: OntologyAnnotation = OntologyAnnotation.create()
             return_val.Comments = comments
             return return_val
 
-        return singleton(_arrow654())
+        return singleton(_arrow729())
 
     else: 
-        def _arrow658(i: int, label: Any=label, label_tsr: Any=label_tsr, label_tan: Any=label_tan, matrix: Any=matrix) -> OntologyAnnotation:
+        def _arrow730(i: int, label: Any=label, label_tsr: Any=label_tsr, label_tan: Any=label_tan, matrix: Any=matrix) -> OntologyAnnotation:
             def mapping(k: str) -> Comment:
                 return Comment_fromString(k, SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (k, i)))
 
             comments_1: Array[Comment] = list(map(mapping, matrix.CommentKeys))
             return OntologyAnnotation(SparseTable__TryGetValue_11FD62A8(matrix, (label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (label_tsr, i)), SparseTable__TryGetValue_11FD62A8(matrix, (label_tan, i)), comments_1)
 
-        return initialize(matrix.ColumnCount, _arrow658)
+        return initialize(matrix.ColumnCount, _arrow730)
 
 
 
 def to_sparse_table(label: str, label_tsr: str, label_tan: str, designs: FSharpList[OntologyAnnotation]) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, of_array([label, label_tan, label_tsr]), None, length(designs) + 1)
     comment_keys: FSharpList[str] = empty()
     def action(i: int, d: OntologyAnnotation, label: Any=label, label_tsr: Any=label_tsr, label_tan: Any=label_tan, designs: Any=designs) -> None:
@@ -49,27 +49,27 @@
             n: str = pattern_input[0]
             comment_keys = cons(n, comment_keys)
             add_to_dict(matrix.Matrix, (n, i_1), pattern_input[1])
 
         ResizeArray_iter(f, d.Comments)
 
     iterate_indexed(action, designs)
-    class ObjectExpr663:
+    class ObjectExpr734:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow662(x: str, y: str) -> bool:
+            def _arrow732(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow662
+            return _arrow732
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr663())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr734())), matrix.ColumnCount)
 
 
 def from_rows(prefix: str | None, label: str, label_tsr: str, label_tan: str, line_number: int, rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, int, FSharpList[Remark], FSharpList[OntologyAnnotation]]:
     labels: FSharpList[str] = of_array([label, label_tan, label_tsr])
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, labels, line_number) if (prefix is None) else SparseTable_FromRows_Z5579EC29(rows, labels, line_number, prefix)
     return (tupled_arg[0], tupled_arg[1], tupled_arg[2], from_sparse_table(label, label_tsr, label_tan, tupled_arg[3]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/ontology_source_reference.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/ontology_source_reference.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/protocols.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,36 +46,36 @@
 
 labels: FSharpList[str] = of_array([name_label, protocol_type_label, type_term_accession_number_label, type_term_source_reflabel, description_label, uri_label, version_label, parameters_name_label, parameters_term_accession_number_label, parameters_term_source_reflabel, components_name_label, components_type_label, components_type_term_accession_number_label, components_type_term_source_reflabel])
 
 def from_string(name: str | None, protocol_type: str | None, type_term_accession_number: str | None, type_term_source_ref: str | None, description: str | None, uri: str | None, version: str | None, parameters_name: str, parameters_term_accession_number: str, parameters_term_source_ref: str, components_name: str, components_type: str, components_type_term_accession_number: str, components_type_term_source_ref: str, comments: FSharpList[Comment]) -> Protocol:
     protocol_type_1: OntologyAnnotation = OntologyAnnotation.create(protocol_type, type_term_source_ref, type_term_accession_number)
     parameters: FSharpList[ProtocolParameter] = of_seq(ProtocolParameter_fromAggregatedStrings(";", parameters_name, parameters_term_source_ref, parameters_term_accession_number))
     components: FSharpList[Component] = Component_fromAggregatedStrings(";", components_name, components_type, components_type_term_source_ref, components_type_term_accession_number)
-    def _arrow800(s: str, name: Any=name, protocol_type: Any=protocol_type, type_term_accession_number: Any=type_term_accession_number, type_term_source_ref: Any=type_term_source_ref, description: Any=description, uri: Any=uri, version: Any=version, parameters_name: Any=parameters_name, parameters_term_accession_number: Any=parameters_term_accession_number, parameters_term_source_ref: Any=parameters_term_source_ref, components_name: Any=components_name, components_type: Any=components_type, components_type_term_accession_number: Any=components_type_term_accession_number, components_type_term_source_ref: Any=components_type_term_source_ref, comments: Any=comments) -> str:
+    def _arrow798(s: str, name: Any=name, protocol_type: Any=protocol_type, type_term_accession_number: Any=type_term_accession_number, type_term_source_ref: Any=type_term_source_ref, description: Any=description, uri: Any=uri, version: Any=version, parameters_name: Any=parameters_name, parameters_term_accession_number: Any=parameters_term_accession_number, parameters_term_source_ref: Any=parameters_term_source_ref, components_name: Any=components_name, components_type: Any=components_type, components_type_term_accession_number: Any=components_type_term_accession_number, components_type_term_source_ref: Any=components_type_term_source_ref, comments: Any=comments) -> str:
         return URIModule_fromString(s)
 
-    def _arrow802(s_1: str, name: Any=name, protocol_type: Any=protocol_type, type_term_accession_number: Any=type_term_accession_number, type_term_source_ref: Any=type_term_source_ref, description: Any=description, uri: Any=uri, version: Any=version, parameters_name: Any=parameters_name, parameters_term_accession_number: Any=parameters_term_accession_number, parameters_term_source_ref: Any=parameters_term_source_ref, components_name: Any=components_name, components_type: Any=components_type, components_type_term_accession_number: Any=components_type_term_accession_number, components_type_term_source_ref: Any=components_type_term_source_ref, comments: Any=comments) -> str:
+    def _arrow799(s_1: str, name: Any=name, protocol_type: Any=protocol_type, type_term_accession_number: Any=type_term_accession_number, type_term_source_ref: Any=type_term_source_ref, description: Any=description, uri: Any=uri, version: Any=version, parameters_name: Any=parameters_name, parameters_term_accession_number: Any=parameters_term_accession_number, parameters_term_source_ref: Any=parameters_term_source_ref, components_name: Any=components_name, components_type: Any=components_type, components_type_term_accession_number: Any=components_type_term_accession_number, components_type_term_source_ref: Any=components_type_term_source_ref, comments: Any=comments) -> str:
         return URIModule_fromString(s_1)
 
-    return Protocol_make(None, map(_arrow800, name), Option_fromValueWithDefault(OntologyAnnotation(), protocol_type_1), description, map(_arrow802, uri), version, Option_fromValueWithDefault(empty(), parameters), Option_fromValueWithDefault(empty(), components), Option_fromValueWithDefault(empty(), comments))
+    return Protocol_make(None, map(_arrow798, name), Option_fromValueWithDefault(OntologyAnnotation(), protocol_type_1), description, map(_arrow799, uri), version, Option_fromValueWithDefault(empty(), parameters), Option_fromValueWithDefault(empty(), components), Option_fromValueWithDefault(empty(), comments))
 
 
 def from_sparse_table(matrix: SparseTable) -> FSharpList[Protocol]:
     if (length(matrix.CommentKeys) != 0) if (matrix.ColumnCount == 0) else False:
         return singleton(Protocol_create_Z414665E7(None, None, None, None, None, None, None, None, of_seq(SparseTable_GetEmptyComments_3ECCA699(matrix))))
 
     else: 
-        def _arrow805(i: int, matrix: Any=matrix) -> Protocol:
+        def _arrow800(i: int, matrix: Any=matrix) -> Protocol:
             def mapping(k: str) -> Comment:
                 return Comment_fromString(k, SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (k, i)))
 
             comments_1: FSharpList[Comment] = map_1(mapping, matrix.CommentKeys)
             return from_string(SparseTable__TryGetValue_11FD62A8(matrix, (name_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (protocol_type_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (type_term_accession_number_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (type_term_source_reflabel, i)), SparseTable__TryGetValue_11FD62A8(matrix, (description_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (uri_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (version_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (parameters_name_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (parameters_term_accession_number_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (parameters_term_source_reflabel, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (components_name_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (components_type_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (components_type_term_accession_number_label, i)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (components_type_term_source_reflabel, i)), comments_1)
 
-        return initialize(matrix.ColumnCount, _arrow805)
+        return initialize(matrix.ColumnCount, _arrow800)
 
 
 
 def to_sparse_table(protocols: FSharpList[Protocol]) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, labels, None, length(protocols) + 1)
     comment_keys: FSharpList[str] = empty()
     def action_1(i: int, p: Protocol, protocols: Any=protocols) -> None:
@@ -108,27 +108,27 @@
                 comment_keys = cons(n, comment_keys)
                 add_to_dict(matrix.Matrix, (n, i_1), pattern_input[1])
 
             iterate(action, match_value)
 
 
     iterate_indexed(action_1, protocols)
-    class ObjectExpr807:
+    class ObjectExpr802:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow806(x: str, y: str) -> bool:
+            def _arrow801(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow806
+            return _arrow801
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr807())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr802())), matrix.ColumnCount)
 
 
 def from_rows(prefix: str | None, line_number: int, rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, int, FSharpList[Remark], FSharpList[Protocol]]:
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, labels, line_number) if (prefix is None) else SparseTable_FromRows_Z5579EC29(rows, labels, line_number, prefix)
     return (tupled_arg[0], tupled_arg[1], tupled_arg[2], from_sparse_table(tupled_arg[3]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/publication.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/publication.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,41 +29,41 @@
 
 status_term_source_reflabel: str = "Status Term Source REF"
 
 labels: FSharpList[str] = of_array([pub_med_idlabel, doi_label, author_list_label, title_label, status_label, status_term_accession_number_label, status_term_source_reflabel])
 
 def from_string(pub_med_id: str | None, doi: str | None, author: str | None, title: str | None, status: str | None, status_term_source_ref: str | None, status_term_accession_number: str | None, comments: Array[Comment]) -> Publication:
     status_1: OntologyAnnotation = OntologyAnnotation(status, status_term_source_ref, status_term_accession_number)
-    def _arrow798(s: str, pub_med_id: Any=pub_med_id, doi: Any=doi, author: Any=author, title: Any=title, status: Any=status, status_term_source_ref: Any=status_term_source_ref, status_term_accession_number: Any=status_term_accession_number, comments: Any=comments) -> str:
+    def _arrow803(s: str, pub_med_id: Any=pub_med_id, doi: Any=doi, author: Any=author, title: Any=title, status: Any=status, status_term_source_ref: Any=status_term_source_ref, status_term_accession_number: Any=status_term_accession_number, comments: Any=comments) -> str:
         return URIModule_fromString(s)
 
-    pub_med_id_1: str | None = map(_arrow798, pub_med_id)
+    pub_med_id_1: str | None = map(_arrow803, pub_med_id)
     status_2: OntologyAnnotation | None = Option_fromValueWithDefault(OntologyAnnotation(), status_1)
     return Publication.make(pub_med_id_1, doi, author, title, status_2, comments)
 
 
 def from_sparse_table(matrix: SparseTable) -> FSharpList[Publication]:
     if (length(matrix.CommentKeys) != 0) if (matrix.ColumnCount == 0) else False:
         comments: Array[Comment] = SparseTable_GetEmptyComments_3ECCA699(matrix)
-        def _arrow799(__unit: None=None, matrix: Any=matrix) -> Publication:
+        def _arrow804(__unit: None=None, matrix: Any=matrix) -> Publication:
             return_val: Publication = Publication.create()
             return_val.Comments = comments
             return return_val
 
-        return singleton(_arrow799())
+        return singleton(_arrow804())
 
     else: 
-        def _arrow801(i: int, matrix: Any=matrix) -> Publication:
+        def _arrow805(i: int, matrix: Any=matrix) -> Publication:
             def mapping(k: str) -> Comment:
                 return Comment_fromString(k, SparseTable__TryGetValueDefault_5BAE6133(matrix, "", (k, i)))
 
             comments_1: Array[Comment] = list(map_1(mapping, matrix.CommentKeys))
             return from_string(SparseTable__TryGetValue_11FD62A8(matrix, (pub_med_idlabel, i)), SparseTable__TryGetValue_11FD62A8(matrix, (doi_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (author_list_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (title_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (status_label, i)), SparseTable__TryGetValue_11FD62A8(matrix, (status_term_source_reflabel, i)), SparseTable__TryGetValue_11FD62A8(matrix, (status_term_accession_number_label, i)), comments_1)
 
-        return initialize(matrix.ColumnCount, _arrow801)
+        return initialize(matrix.ColumnCount, _arrow805)
 
 
 
 def to_sparse_table(publications: FSharpList[Publication]) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, labels, None, length(publications) + 1)
     comment_keys: FSharpList[str] = empty()
     def action(i: int, p: Publication, publications: Any=publications) -> None:
@@ -84,27 +84,27 @@
             n: str = pattern_input[0]
             comment_keys = cons(n, comment_keys)
             add_to_dict(matrix.Matrix, (n, i_1), pattern_input[1])
 
         ResizeArray_iter(f, p.Comments)
 
     iterate_indexed(action, publications)
-    class ObjectExpr804:
+    class ObjectExpr807:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow803(x: str, y: str) -> bool:
+            def _arrow806(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow803
+            return _arrow806
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr804())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr807())), matrix.ColumnCount)
 
 
 def from_rows(prefix: str | None, line_number: int, rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, int, FSharpList[Remark], FSharpList[Publication]]:
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, labels, line_number) if (prefix is None) else SparseTable_FromRows_Z5579EC29(rows, labels, line_number, prefix)
     return (tupled_arg[0], tupled_arg[1], tupled_arg[2], from_sparse_table(tupled_arg[3]))
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/sparse_table.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/sparse_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,41 +35,41 @@
         return tuple[1]
 
     return map(mapping, i)
 
 
 def SparseRowModule_fromAllValues(v: IEnumerable_1[str | None]) -> IEnumerable_1[tuple[int, str]]:
     def chooser(tupled_arg: tuple[int, str | None], v: Any=v) -> tuple[int, str] | None:
-        def _arrow732(v_1: str, tupled_arg: Any=tupled_arg) -> tuple[int, str]:
+        def _arrow731(v_1: str, tupled_arg: Any=tupled_arg) -> tuple[int, str]:
             return (tupled_arg[0], v_1)
 
-        return map_1(_arrow732, tupled_arg[1])
+        return map_1(_arrow731, tupled_arg[1])
 
     return choose(chooser, indexed(v))
 
 
 def SparseRowModule_getAllValues(i: IEnumerable_1[tuple[int, str]]) -> IEnumerable_1[str | None]:
     class ObjectExpr733:
         @property
         def Compare(self) -> Callable[[int, int], int]:
             return compare_primitives
 
     m: Any = of_seq(i, ObjectExpr733())
     def projection(tuple: tuple[int, str], i: Any=i) -> int:
         return tuple[0]
 
-    class ObjectExpr734:
+    class ObjectExpr735:
         @property
         def Compare(self) -> Callable[[int, int], int]:
             return compare_primitives
 
-    def _arrow735(i_1: int, i: Any=i) -> str | None:
+    def _arrow736(i_1: int, i: Any=i) -> str | None:
         return try_find(i_1, m)
 
-    return initialize(max_by(projection, i, ObjectExpr734())[0] + 1, _arrow735)
+    return initialize(max_by(projection, i, ObjectExpr735())[0] + 1, _arrow736)
 
 
 def SparseRowModule_fromFsRow(r: FsRow) -> IEnumerable_1[tuple[int, str]]:
     def chooser(c: FsCell, r: Any=r) -> tuple[int, str] | None:
         if equals(c.Value, ""):
             return None
```

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/Metadata/study.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/Metadata/study.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/Spreadsheet/template.py` & `arctrl-2.0.0a3/arctrl/Spreadsheet/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,41 +114,41 @@
     comments: FSharpList[Comment] = map(mapping, matrix.CommentKeys)
     return Metadata_Template_TemplateInfo_create(SparseTable__TryGetValueDefault_5BAE6133(matrix, create_missing_identifier(), ("Id", 0)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", ("Name", 0)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", ("Version", 0)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", ("Description", 0)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", ("Organisation", 0)), SparseTable__TryGetValueDefault_5BAE6133(matrix, "", ("Table", 0)), comments)
 
 
 def Metadata_Template_TemplateInfo_ToSparseTable_48C39BE1(template: Template) -> SparseTable:
     matrix: SparseTable = SparseTable_Create_Z2192E64B(None, Metadata_Template_TemplateInfo_get_Labels(), None, 2)
     comment_keys: FSharpList[str] = empty()
-    def _arrow919(__unit: None=None, template: Any=template) -> str:
+    def _arrow920(__unit: None=None, template: Any=template) -> str:
         copy_of_struct: str = template.Id
         return str(copy_of_struct)
 
-    def _arrow920(__unit: None=None, template: Any=template) -> str:
+    def _arrow921(__unit: None=None, template: Any=template) -> str:
         copy_of_struct_1: str = template.Id
         return str(copy_of_struct_1)
 
-    add_to_dict(matrix.Matrix, ("Id", 1), "" if (_arrow919().find("MISSING_IDENTIFIER_") == 0) else _arrow920())
+    add_to_dict(matrix.Matrix, ("Id", 1), "" if (_arrow920().find("MISSING_IDENTIFIER_") == 0) else _arrow921())
     add_to_dict(matrix.Matrix, ("Name", 1), template.Name)
     add_to_dict(matrix.Matrix, ("Version", 1), template.Version)
     add_to_dict(matrix.Matrix, ("Description", 1), template.Description)
     add_to_dict(matrix.Matrix, ("Organisation", 1), to_string(template.Organisation))
     add_to_dict(matrix.Matrix, ("Table", 1), template.Table.Name)
-    class ObjectExpr922:
+    class ObjectExpr923:
         @property
         def Equals(self) -> Callable[[str, str], bool]:
-            def _arrow921(x: str, y: str) -> bool:
+            def _arrow922(x: str, y: str) -> bool:
                 return x == y
 
-            return _arrow921
+            return _arrow922
 
         @property
         def GetHashCode(self) -> Callable[[str], int]:
             return string_hash
 
-    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr922())), matrix.ColumnCount)
+    return SparseTable(matrix.Matrix, matrix.Keys, reverse(List_distinct(comment_keys, ObjectExpr923())), matrix.ColumnCount)
 
 
 def Metadata_Template_TemplateInfo_fromRows_9F97F2A(rows: IEnumerator[IEnumerable_1[tuple[int, str]]]) -> tuple[str | None, Metadata_Template_TemplateInfo]:
     tupled_arg: tuple[str | None, int, FSharpList[Remark], SparseTable] = SparseTable_FromRows_Z5579EC29(rows, Metadata_Template_TemplateInfo_get_Labels(), 0)
     return (tupled_arg[0], Metadata_Template_TemplateInfo_FromSparseTable_3ECCA699(tupled_arg[3]))
 
 
@@ -289,16 +289,16 @@
     en_1: IEnumerator[IEnumerable_1[tuple[int, str]]] = get_enumerator(Metadata_Template_mapDeprecatedKeys(rows))
     ignore(en_1.System_Collections_IEnumerator_MoveNext())
     pattern_input_3: tuple[str | None, Metadata_Template_TemplateInfo] = Metadata_Template_TemplateInfo_fromRows_9F97F2A(en_1)
     return loop(en_1, pattern_input_3[0], pattern_input_3[1], empty(), empty(), empty())
 
 
 def Metadata_Template_toRows(template: Template) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
-    def _arrow931(__unit: None=None, template: Any=template) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
-        def _arrow930(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
+    def _arrow932(__unit: None=None, template: Any=template) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
+        def _arrow931(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
             def _arrow929(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                 def _arrow928(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                     def _arrow927(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                         def _arrow926(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                             def _arrow925(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                                 def _arrow924(__unit: None=None) -> IEnumerable_1[IEnumerable_1[tuple[int, str]]]:
                                     return to_rows_1("Author", of_seq(template.Authors))
@@ -311,17 +311,17 @@
 
                     return append(Metadata_ER_toRows(None, to_list(template.EndpointRepositories)), delay(_arrow927))
 
                 return append(singleton(SparseRowModule_fromValues(to_enumerable(["ERS"]))), delay(_arrow928))
 
             return append(Metadata_Template_TemplateInfo_toRows_48C39BE1(template), delay(_arrow929))
 
-        return append(singleton(SparseRowModule_fromValues(to_enumerable(["TEMPLATE"]))), delay(_arrow930))
+        return append(singleton(SparseRowModule_fromValues(to_enumerable(["TEMPLATE"]))), delay(_arrow931))
 
-    return delay(_arrow931)
+    return delay(_arrow932)
 
 
 def Template_fromParts(template_info: Metadata_Template_TemplateInfo, ers: FSharpList[OntologyAnnotation], tags: FSharpList[OntologyAnnotation], authors: FSharpList[Person], table: ArcTable, last_updated: Any) -> Template:
     id: str = parse(template_info.Id)
     organisation: Organisation = Organisation.of_string(template_info.Organisation)
     authors_1: Array[Person] = list(authors)
     repos: Array[OntologyAnnotation] = list(ers)
@@ -353,15 +353,15 @@
         pattern_input = ((Metadata_Template_TemplateInfo_get_empty(), empty(), empty(), empty())) if (match_value_1 is None) else Template_fromMetadataSheet(match_value_1)
 
     else: 
         pattern_input = Template_fromMetadataSheet(match_value)
 
     template_info: Metadata_Template_TemplateInfo = pattern_input[0]
     sheets: Array[FsWorksheet] = doc.GetWorksheets()
-    def _arrow932(__unit: None=None, doc: Any=doc) -> ArcTable:
+    def _arrow933(__unit: None=None, doc: Any=doc) -> ArcTable:
         def try_table_name_matches(ws: FsWorksheet) -> FsWorksheet | None:
             def predicate(t: FsTable, ws: Any=ws) -> bool:
                 return t.Name == template_info.Table
 
             if exists(predicate, ws.Tables):
                 return ws
 
@@ -401,15 +401,15 @@
                 raise TemplateReadError(("Ws with name `" + ws_2.Name) + "` could not be converted to a table")
 
             else: 
                 return match_value_3
 
 
 
-    return Template_fromParts(template_info, pattern_input[1], pattern_input[2], pattern_input[3], _arrow932(), now())
+    return Template_fromParts(template_info, pattern_input[1], pattern_input[2], pattern_input[3], _arrow933(), now())
 
 
 def Template_toFsWorkbook(template: Template) -> FsWorkbook:
     doc: FsWorkbook = FsWorkbook()
     meta_data_sheet: FsWorksheet = Template_toMetadataSheet(template)
     doc.AddWorksheet(meta_data_sheet)
     sheet: FsWorksheet = to_fs_worksheet(template.Table)
```

### Comparing `arctrl-2.0.0a2/arctrl/template_web.py` & `arctrl-2.0.0a3/arctrl/template_web.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/WebRequest/web_request_py.py` & `arctrl-2.0.0a3/arctrl/WebRequest/web_request_py.py`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/arctrl/xlsx.py` & `arctrl-2.0.0a3/arctrl/xlsx.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from .fable_modules.fable_library.types import Array
 from .fable_modules.fs_spreadsheet.fs_workbook import FsWorkbook
 from .Core.arc_types import (ArcAssay, ArcStudy, ArcInvestigation)
 from .Spreadsheet.arc_assay import (from_fs_workbook, to_fs_workbook)
 from .Spreadsheet.arc_investigation import (from_fs_workbook as from_fs_workbook_1, to_fs_workbook as to_fs_workbook_1, to_light_fs_workbook)
 from .Spreadsheet.arc_study import (ARCtrl_ArcStudy__ArcStudy_fromFsWorkbook_Static_32154C9D, ARCtrl_ArcStudy__ArcStudy_toFsWorkbook_Static_353D0DB7)
 
-def _expr1814() -> TypeInfo:
+def _expr1813() -> TypeInfo:
     return class_type("ARCtrl.XlsxHelper.AssayXlsx", None, XlsxHelper_AssayXlsx)
 
 
 class XlsxHelper_AssayXlsx:
     def __init__(self, __unit: None=None) -> None:
         pass
 
     def from_fs_workbook(self, fswb: FsWorkbook) -> ArcAssay:
         return from_fs_workbook(fswb)
 
     def to_fs_workbook(self, assay: ArcAssay) -> FsWorkbook:
         return to_fs_workbook(assay)
 
 
-XlsxHelper_AssayXlsx_reflection = _expr1814
+XlsxHelper_AssayXlsx_reflection = _expr1813
 
 def XlsxHelper_AssayXlsx__ctor(__unit: None=None) -> XlsxHelper_AssayXlsx:
     return XlsxHelper_AssayXlsx(__unit)
 
 
 def _expr1815() -> TypeInfo:
     return class_type("ARCtrl.XlsxHelper.StudyXlsx", None, XlsxHelper_StudyXlsx)
```

### Comparing `arctrl-2.0.0a2/pyproject.toml` & `arctrl-2.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ARCtrl"
-version = "2.0.0a2"
+version = "2.0.0a3"
 description = "Library for management of Annotated Research Contexts (ARCs) using an in-memory representation and runtimer agnostic contract systems."
 authors = ["Heinrich Lukas Weil <weil@rptu.de>", "Kevin Frey <freymaurer@gmx.de>"]
 maintainers = ["Florian Wetzels"]
 readme = "README.md"
 repository = "https://github.com/nfdi4plants/ARCtrl"
 keywords = ["arc", "annotated research context", "isa", "research data", "multi platform"]
```

### Comparing `arctrl-2.0.0a2/README.md` & `arctrl-2.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `arctrl-2.0.0a2/PKG-INFO` & `arctrl-2.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARCtrl
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Library for management of Annotated Research Contexts (ARCs) using an in-memory representation and runtimer agnostic contract systems.
 Home-page: https://github.com/nfdi4plants/ARCtrl
 Keywords: arc,annotated research context,isa,research data,multi platform
 Author: Heinrich Lukas Weil
 Author-email: weil@rptu.de
 Maintainer: Florian Wetzels
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ARCtrl Version: 2.0.0a2 Summary: Library for
+Metadata-Version: 2.1 Name: ARCtrl Version: 2.0.0a3 Summary: Library for
 management of Annotated Research Contexts (ARCs) using an in-memory
 representation and runtimer agnostic contract systems. Home-page: https://
 github.com/nfdi4plants/ARCtrl Keywords: arc,annotated research
 context,isa,research data,multi platform Author: Heinrich Lukas Weil Author-
 email: weil@rptu.de Maintainer: Florian Wetzels Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

