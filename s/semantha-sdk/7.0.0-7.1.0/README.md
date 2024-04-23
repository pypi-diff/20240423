# Comparing `tmp/semantha_sdk-7.0.0.tar.gz` & `tmp/semantha_sdk-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-7.0.0.tar", max compression
+gzip compressed data, was "semantha_sdk-7.1.0.tar", max compression
```

## Comparing `semantha_sdk-7.0.0.tar` & `semantha_sdk-7.1.0.tar`

### file list

```diff
@@ -1,242 +1,258 @@
--rw-r--r--   0        0        0     5931 2024-04-09 08:27:47.522642 semantha_sdk-7.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    14639 2024-03-18 16:00:01.047358 semantha_sdk-7.0.0/DOCU.md
--rw-r--r--   0        0        0    11545 2024-03-08 20:30:37.820624 semantha_sdk-7.0.0/LICENSE
--rw-r--r--   0        0        0     1634 2024-04-09 08:23:39.338374 semantha_sdk-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     4900 2024-03-08 20:30:37.825616 semantha_sdk-7.0.0/README.md
--rw-r--r--   0        0        0     2652 2024-03-18 16:02:42.701241 semantha_sdk-7.0.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 20:30:38.006648 semantha_sdk-7.0.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     2122 2024-03-20 09:22:23.597528 semantha_sdk-7.0.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0      954 2024-03-20 09:22:23.585002 semantha_sdk-7.0.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      791 2024-03-20 09:22:23.465373 semantha_sdk-7.0.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      773 2024-03-20 09:22:23.479496 semantha_sdk-7.0.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1807 2024-03-20 09:22:23.569425 semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1512 2024-03-20 09:22:23.525618 semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_documenttypes.py
--rw-r--r--   0        0        0     1842 2024-03-20 09:22:23.527619 semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     4894 2024-03-20 09:22:23.515082 semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3272 2024-03-20 09:22:23.530618 semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1325 2024-03-20 09:22:23.483496 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      916 2024-03-20 09:22:23.467380 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1920 2024-03-20 09:22:23.464373 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1755 2024-03-20 09:22:23.559904 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2993 2024-03-20 09:22:23.473411 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      794 2024-03-20 09:22:23.500525 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1677 2024-03-20 09:22:23.502526 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1722 2024-03-20 09:22:23.561904 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1355 2024-03-20 09:22:23.544350 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1614 2024-03-20 09:22:23.571424 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_rules.py
--rw-r--r--   0        0        0     1238 2024-03-20 09:22:23.454854 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1299 2024-03-20 09:22:23.469411 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1189 2024-03-20 09:22:23.428298 semantha_sdk-7.0.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0      980 2024-03-20 09:22:23.441820 semantha_sdk-7.0.0/semantha_sdk/api/celltypes.py
--rw-r--r--   0        0        0     1253 2024-03-20 09:22:23.492012 semantha_sdk-7.0.0/semantha_sdk/api/child_extractorclasses.py
--rw-r--r--   0        0        0     1299 2024-03-20 09:22:23.425292 semantha_sdk-7.0.0/semantha_sdk/api/clone.py
--rw-r--r--   0        0        0     6426 2024-03-20 09:22:23.493518 semantha_sdk-7.0.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1209 2024-03-20 09:22:23.477496 semantha_sdk-7.0.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1359 2024-03-20 09:22:23.594522 semantha_sdk-7.0.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     1144 2024-03-20 09:22:23.556907 semantha_sdk-7.0.0/semantha_sdk/api/docclass_customfields.py
--rw-r--r--   0        0        0     2241 2024-03-20 09:22:23.591008 semantha_sdk-7.0.0/semantha_sdk/api/docclass_documentclasses.py
--rw-r--r--   0        0        0     1749 2024-03-20 09:22:23.504036 semantha_sdk-7.0.0/semantha_sdk/api/docclass_referencedocuments.py
--rw-r--r--   0        0        0     3956 2024-03-20 09:22:23.545351 semantha_sdk-7.0.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     2513 2024-03-20 09:22:23.537832 semantha_sdk-7.0.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1979 2024-03-20 09:22:23.489011 semantha_sdk-7.0.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     6591 2024-03-20 09:22:23.476495 semantha_sdk-7.0.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     1991 2024-03-20 09:22:23.490012 semantha_sdk-7.0.0/semantha_sdk/api/documenttype.py
--rw-r--r--   0        0        0     2049 2024-03-20 09:22:23.509042 semantha_sdk-7.0.0/semantha_sdk/api/documenttypes.py
--rw-r--r--   0        0        0     4751 2024-03-20 09:22:23.437821 semantha_sdk-7.0.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1241 2024-03-20 09:22:23.549355 semantha_sdk-7.0.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      941 2024-03-20 09:22:23.417779 semantha_sdk-7.0.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1678 2024-03-20 09:22:23.497525 semantha_sdk-7.0.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1546 2024-03-20 09:22:23.512043 semantha_sdk-7.0.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1087 2024-03-20 09:22:23.552351 semantha_sdk-7.0.0/semantha_sdk/api/model_attributes.py
--rw-r--r--   0        0        0      998 2024-03-20 09:22:23.435820 semantha_sdk-7.0.0/semantha_sdk/api/model_backups.py
--rw-r--r--   0        0        0     1512 2024-03-20 09:22:23.541834 semantha_sdk-7.0.0/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1907 2024-03-20 09:22:23.419779 semantha_sdk-7.0.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0     2073 2024-03-20 09:22:23.511043 semantha_sdk-7.0.0/semantha_sdk/api/model_dataproperties.py
--rw-r--r--   0        0        0     1561 2024-03-20 09:22:23.565418 semantha_sdk-7.0.0/semantha_sdk/api/model_dataproperty.py
--rw-r--r--   0        0        0      888 2024-03-20 09:22:23.427298 semantha_sdk-7.0.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     5799 2024-03-20 09:22:23.508042 semantha_sdk-7.0.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      769 2024-03-20 09:22:23.529618 semantha_sdk-7.0.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0     1888 2024-03-20 09:22:23.595522 semantha_sdk-7.0.0/semantha_sdk/api/model_extractorclass.py
--rw-r--r--   0        0        0     2480 2024-03-20 09:22:23.574937 semantha_sdk-7.0.0/semantha_sdk/api/model_extractorclasses.py
--rw-r--r--   0        0        0     1019 2024-03-20 09:22:23.430298 semantha_sdk-7.0.0/semantha_sdk/api/model_extractors.py
--rw-r--r--   0        0        0      908 2024-03-20 09:22:23.572424 semantha_sdk-7.0.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0     1037 2024-03-20 09:22:23.471406 semantha_sdk-7.0.0/semantha_sdk/api/model_formatters.py
--rw-r--r--   0        0        0     1942 2024-03-20 09:22:23.554904 semantha_sdk-7.0.0/semantha_sdk/api/model_metadata.py
--rw-r--r--   0        0        0      904 2024-03-20 09:22:23.443326 semantha_sdk-7.0.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1956 2024-03-20 09:22:23.567424 semantha_sdk-7.0.0/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1549 2024-03-20 09:22:23.481495 semantha_sdk-7.0.0/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0     1056 2024-03-20 09:22:23.495526 semantha_sdk-7.0.0/semantha_sdk/api/model_objectproperties.py
--rw-r--r--   0        0        0     1543 2024-03-20 09:22:23.485012 semantha_sdk-7.0.0/semantha_sdk/api/model_onemetadata.py
--rw-r--r--   0        0        0     1450 2024-03-20 09:22:23.589009 semantha_sdk-7.0.0/semantha_sdk/api/model_regex.py
--rw-r--r--   0        0        0     1830 2024-03-20 09:22:23.450341 semantha_sdk-7.0.0/semantha_sdk/api/model_regexes.py
--rw-r--r--   0        0        0     1495 2024-03-20 09:22:23.583489 semantha_sdk-7.0.0/semantha_sdk/api/model_relation.py
--rw-r--r--   0        0        0     1884 2024-03-20 09:22:23.498526 semantha_sdk-7.0.0/semantha_sdk/api/model_relations.py
--rw-r--r--   0        0        0     1435 2024-03-20 09:22:23.518089 semantha_sdk-7.0.0/semantha_sdk/api/model_rule.py
--rw-r--r--   0        0        0     1070 2024-03-20 09:22:23.461860 semantha_sdk-7.0.0/semantha_sdk/api/model_rulefunctions.py
--rw-r--r--   0        0        0     1938 2024-03-20 09:22:23.432330 semantha_sdk-7.0.0/semantha_sdk/api/model_rules.py
--rw-r--r--   0        0        0     1500 2024-03-20 09:22:23.579944 semantha_sdk-7.0.0/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1889 2024-03-20 09:22:23.453846 semantha_sdk-7.0.0/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1480 2024-03-20 09:22:23.540832 semantha_sdk-7.0.0/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1863 2024-03-20 09:22:23.433813 semantha_sdk-7.0.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1277 2024-03-20 09:22:23.558904 semantha_sdk-7.0.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     4972 2024-03-20 09:22:23.575943 semantha_sdk-7.0.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1462 2024-03-20 09:22:23.520089 semantha_sdk-7.0.0/semantha_sdk/api/modelont_attribute.py
--rw-r--r--   0        0        0     1881 2024-03-20 09:22:23.522090 semantha_sdk-7.0.0/semantha_sdk/api/modelont_attributes.py
--rw-r--r--   0        0        0     1963 2024-03-20 09:22:23.524612 semantha_sdk-7.0.0/semantha_sdk/api/modelont_class.py
--rw-r--r--   0        0        0     2460 2024-03-20 09:22:23.487015 semantha_sdk-7.0.0/semantha_sdk/api/modelont_classes.py
--rw-r--r--   0        0        0     1501 2024-03-20 09:22:23.474496 semantha_sdk-7.0.0/semantha_sdk/api/modelont_instance.py
--rw-r--r--   0        0        0     2594 2024-03-20 09:22:23.587009 semantha_sdk-7.0.0/semantha_sdk/api/modelont_instances.py
--rw-r--r--   0        0        0     1269 2024-03-20 09:22:23.592008 semantha_sdk-7.0.0/semantha_sdk/api/modelontclass_instances.py
--rw-r--r--   0        0        0     1848 2024-03-20 09:22:23.516089 semantha_sdk-7.0.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1831 2024-03-20 09:22:23.439821 semantha_sdk-7.0.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      795 2024-03-20 09:22:23.563410 semantha_sdk-7.0.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2545 2024-03-20 09:22:23.506043 semantha_sdk-7.0.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0    16724 2024-03-20 09:22:23.533621 semantha_sdk-7.0.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0    22091 2024-03-20 09:22:23.446341 semantha_sdk-7.0.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      895 2024-03-20 09:22:23.581489 semantha_sdk-7.0.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2430 2024-03-18 16:00:01.061363 semantha_sdk-7.0.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0     1091 2024-03-20 09:22:23.577944 semantha_sdk-7.0.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      788 2024-03-20 09:22:23.547350 semantha_sdk-7.0.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1664 2024-03-20 09:22:23.445335 semantha_sdk-7.0.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5082 2024-03-20 09:22:23.423285 semantha_sdk-7.0.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4589 2024-03-20 09:22:23.458860 semantha_sdk-7.0.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0     1071 2024-03-20 09:22:23.448341 semantha_sdk-7.0.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     2583 2024-03-28 16:09:02.684081 semantha_sdk-7.0.0/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      910 2024-03-20 09:22:23.451341 semantha_sdk-7.0.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1361 2024-03-20 09:22:23.456861 semantha_sdk-7.0.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1070 2024-03-20 09:22:23.460860 semantha_sdk-7.0.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1559 2024-03-20 09:22:23.421779 semantha_sdk-7.0.0/semantha_sdk/api/transactions.py
--rw-r--r--   0        0        0     1338 2024-03-20 09:22:23.551352 semantha_sdk-7.0.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     6740 2024-03-18 16:00:01.028358 semantha_sdk-7.0.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      548 2024-03-27 10:40:51.164272 semantha_sdk-7.0.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      632 2024-03-27 10:40:51.167272 semantha_sdk-7.0.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      507 2024-03-27 10:40:51.171316 semantha_sdk-7.0.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      487 2024-03-27 10:40:51.174875 semantha_sdk-7.0.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      358 2024-03-27 10:40:51.177881 semantha_sdk-7.0.0/semantha_sdk/model/area.py
--rw-r--r--   0        0        0      710 2024-03-27 10:40:51.181389 semantha_sdk-7.0.0/semantha_sdk/model/argument.py
--rw-r--r--   0        0        0      823 2024-03-27 10:40:51.184402 semantha_sdk-7.0.0/semantha_sdk/model/attribute.py
--rw-r--r--   0        0        0      479 2024-03-27 10:40:51.187402 semantha_sdk-7.0.0/semantha_sdk/model/attribute_overview.py
--rw-r--r--   0        0        0      525 2024-03-27 10:40:51.190529 semantha_sdk-7.0.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      350 2024-03-27 10:40:51.193736 semantha_sdk-7.0.0/semantha_sdk/model/cell_type.py
--rw-r--r--   0        0        0      972 2024-03-27 10:40:51.196966 semantha_sdk-7.0.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      751 2024-03-27 10:40:51.200983 semantha_sdk-7.0.0/semantha_sdk/model/classes_overview.py
--rw-r--r--   0        0        0      799 2024-03-27 10:40:51.205516 semantha_sdk-7.0.0/semantha_sdk/model/clazz.py
--rw-r--r--   0        0        0      557 2024-03-27 10:40:51.208514 semantha_sdk-7.0.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      640 2024-03-27 10:40:51.213038 semantha_sdk-7.0.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0      197 2024-03-18 16:03:00.140284 semantha_sdk-7.0.0/semantha_sdk/model/clusteringstructure_enum.py
--rw-r--r--   0        0        0     1180 2024-03-27 10:40:51.216049 semantha_sdk-7.0.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      565 2024-03-27 10:40:51.219047 semantha_sdk-7.0.0/semantha_sdk/model/condition.py
--rw-r--r--   0        0        0      634 2024-03-27 10:40:51.221556 semantha_sdk-7.0.0/semantha_sdk/model/condition_value.py
--rw-r--r--   0        0        0      443 2024-03-27 10:40:51.224578 semantha_sdk-7.0.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      361 2024-03-27 10:40:51.228578 semantha_sdk-7.0.0/semantha_sdk/model/custom_field.py
--rw-r--r--   0        0        0      575 2024-03-27 10:40:51.232098 semantha_sdk-7.0.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      348 2024-03-27 10:40:51.234620 semantha_sdk-7.0.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      471 2024-03-27 10:40:51.237619 semantha_sdk-7.0.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1372 2024-03-27 10:40:51.241135 semantha_sdk-7.0.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1110 2024-03-27 10:40:51.245149 semantha_sdk-7.0.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0     1043 2024-03-27 10:40:51.248146 semantha_sdk-7.0.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      654 2024-03-27 10:40:51.251654 semantha_sdk-7.0.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      647 2024-03-27 10:40:51.253674 semantha_sdk-7.0.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1134 2024-03-27 10:40:51.257675 semantha_sdk-7.0.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      437 2024-03-27 10:40:51.261201 semantha_sdk-7.0.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      432 2024-03-27 10:40:51.266910 semantha_sdk-7.0.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      452 2024-03-27 10:40:51.270919 semantha_sdk-7.0.0/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      632 2024-03-27 10:40:51.274952 semantha_sdk-7.0.0/semantha_sdk/model/document_type.py
--rw-r--r--   0        0        0      797 2024-03-27 10:40:51.277951 semantha_sdk-7.0.0/semantha_sdk/model/document_type_change.py
--rw-r--r--   0        0        0     1155 2024-03-27 10:40:51.281459 semantha_sdk-7.0.0/semantha_sdk/model/document_type_config.py
--rw-r--r--   0        0        0      175 2024-03-18 16:03:00.143266 semantha_sdk-7.0.0/semantha_sdk/model/documentmode_enum.py
--rw-r--r--   0        0        0      401 2024-03-27 10:40:51.284476 semantha_sdk-7.0.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      359 2024-03-27 10:40:51.287477 semantha_sdk-7.0.0/semantha_sdk/model/domain_info.py
--rw-r--r--   0        0        0      374 2024-03-27 10:40:51.292010 semantha_sdk-7.0.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      621 2024-03-27 10:40:51.295019 semantha_sdk-7.0.0/semantha_sdk/model/expression.py
--rw-r--r--   0        0        0      529 2024-03-27 10:40:51.300403 semantha_sdk-7.0.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      725 2024-03-27 10:40:51.303942 semantha_sdk-7.0.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      479 2024-03-27 10:40:51.307942 semantha_sdk-7.0.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      909 2024-03-27 10:40:51.311450 semantha_sdk-7.0.0/semantha_sdk/model/extractor.py
--rw-r--r--   0        0        0      742 2024-03-27 10:40:51.314470 semantha_sdk-7.0.0/semantha_sdk/model/extractor_attribute.py
--rw-r--r--   0        0        0      855 2024-03-27 10:40:51.320976 semantha_sdk-7.0.0/semantha_sdk/model/extractor_class.py
--rw-r--r--   0        0        0      656 2024-03-27 10:40:51.325998 semantha_sdk-7.0.0/semantha_sdk/model/extractor_class_overview.py
--rw-r--r--   0        0        0      874 2024-03-27 10:40:51.329001 semantha_sdk-7.0.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      326 2024-03-27 10:40:51.332535 semantha_sdk-7.0.0/semantha_sdk/model/field.py
--rw-r--r--   0        0        0      455 2024-03-27 10:40:51.336545 semantha_sdk-7.0.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      441 2024-03-27 10:40:51.338542 semantha_sdk-7.0.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      421 2024-03-27 10:40:51.342069 semantha_sdk-7.0.0/semantha_sdk/model/formatter.py
--rw-r--r--   0        0        0      372 2024-03-27 10:40:51.345076 semantha_sdk-7.0.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0     1018 2024-03-27 10:40:51.349599 semantha_sdk-7.0.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      471 2024-03-27 10:40:51.353124 semantha_sdk-7.0.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      513 2024-03-27 10:40:51.356138 semantha_sdk-7.0.0/semantha_sdk/model/instance_overview.py
--rw-r--r--   0        0        0      329 2024-03-27 10:40:51.359156 semantha_sdk-7.0.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      354 2024-03-27 10:40:51.362302 semantha_sdk-7.0.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      442 2024-03-27 10:40:51.365306 semantha_sdk-7.0.0/semantha_sdk/model/link.py
--rw-r--r--   0        0        0      527 2024-03-27 10:40:51.368302 semantha_sdk-7.0.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      417 2024-03-27 10:40:51.370303 semantha_sdk-7.0.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      397 2024-03-27 10:40:51.373824 semantha_sdk-7.0.0/semantha_sdk/model/matcher.py
--rw-r--r--   0        0        0      542 2024-03-27 10:40:51.377335 semantha_sdk-7.0.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      442 2024-03-27 10:40:51.381075 semantha_sdk-7.0.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      338 2024-03-27 10:40:51.384252 semantha_sdk-7.0.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      351 2024-03-27 10:40:51.386250 semantha_sdk-7.0.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      338 2024-03-18 16:02:54.126838 semantha_sdk-7.0.0/semantha_sdk/model/mode_enum.py
--rw-r--r--   0        0        0      673 2024-03-27 10:40:51.389251 semantha_sdk-7.0.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1547 2024-03-27 10:40:51.391764 semantha_sdk-7.0.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      446 2024-03-27 10:40:51.394790 semantha_sdk-7.0.0/semantha_sdk/model/model_metadata.py
--rw-r--r--   0        0        0      311 2024-03-27 10:40:51.397793 semantha_sdk-7.0.0/semantha_sdk/model/name.py
--rw-r--r--   0        0        0      421 2024-03-27 10:40:51.401299 semantha_sdk-7.0.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      417 2024-03-27 10:40:51.403308 semantha_sdk-7.0.0/semantha_sdk/model/overview.py
--rw-r--r--   0        0        0      778 2024-03-27 10:40:51.408311 semantha_sdk-7.0.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      470 2024-03-27 10:40:51.412977 semantha_sdk-7.0.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1031 2024-03-27 10:40:51.416988 semantha_sdk-7.0.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      420 2024-03-27 10:40:51.420987 semantha_sdk-7.0.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      463 2024-03-27 10:40:51.425129 semantha_sdk-7.0.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      519 2024-03-27 10:40:51.429130 semantha_sdk-7.0.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      432 2024-03-27 10:40:51.433663 semantha_sdk-7.0.0/semantha_sdk/model/range.py
--rw-r--r--   0        0        0      196 2024-03-18 16:02:54.127838 semantha_sdk-7.0.0/semantha_sdk/model/range_enum.py
--rw-r--r--   0        0        0      372 2024-03-27 10:40:51.437660 semantha_sdk-7.0.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      817 2024-03-27 10:40:51.442189 semantha_sdk-7.0.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      678 2024-03-27 10:40:51.446263 semantha_sdk-7.0.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      386 2024-03-27 10:40:51.449255 semantha_sdk-7.0.0/semantha_sdk/model/regex.py
--rw-r--r--   0        0        0      626 2024-03-27 10:40:51.452453 semantha_sdk-7.0.0/semantha_sdk/model/relation.py
--rw-r--r--   0        0        0      427 2024-03-27 10:40:51.455454 semantha_sdk-7.0.0/semantha_sdk/model/relation_condition.py
--rw-r--r--   0        0        0      651 2024-03-27 10:40:51.458460 semantha_sdk-7.0.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      442 2024-03-27 10:40:51.461974 semantha_sdk-7.0.0/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      611 2024-03-27 10:40:51.464984 semantha_sdk-7.0.0/semantha_sdk/model/rule.py
--rw-r--r--   0        0        0      493 2024-03-27 10:40:51.467982 semantha_sdk-7.0.0/semantha_sdk/model/rule_function.py
--rw-r--r--   0        0        0      528 2024-03-27 10:40:51.470983 semantha_sdk-7.0.0/semantha_sdk/model/rule_overview.py
--rw-r--r--   0        0        0      839 2024-03-27 10:40:51.474561 semantha_sdk-7.0.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      452 2024-03-27 10:40:51.478561 semantha_sdk-7.0.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      777 2024-03-27 10:40:51.482095 semantha_sdk-7.0.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1930 2024-03-27 10:40:51.485089 semantha_sdk-7.0.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      377 2024-03-27 10:40:51.488088 semantha_sdk-7.0.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      627 2024-03-27 10:40:51.491090 semantha_sdk-7.0.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      847 2024-03-27 10:40:51.494753 semantha_sdk-7.0.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      432 2024-03-27 10:40:51.498312 semantha_sdk-7.0.0/semantha_sdk/model/source_document.py
--rw-r--r--   0        0        0      526 2024-03-27 10:40:51.501310 semantha_sdk-7.0.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      416 2024-03-27 10:40:51.505348 semantha_sdk-7.0.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      386 2024-03-27 10:40:51.508358 semantha_sdk-7.0.0/semantha_sdk/model/summarization.py
--rw-r--r--   0        0        0      183 2024-03-18 16:02:54.129838 semantha_sdk-7.0.0/semantha_sdk/model/summarylength_enum.py
--rw-r--r--   0        0        0      521 2024-03-27 10:40:51.511865 semantha_sdk-7.0.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      371 2024-03-27 10:40:51.514875 semantha_sdk-7.0.0/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      498 2024-03-27 10:40:51.517874 semantha_sdk-7.0.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      396 2024-03-27 10:40:51.519873 semantha_sdk-7.0.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      410 2024-03-27 10:40:51.523416 semantha_sdk-7.0.0/semantha_sdk/model/transaction_summary.py
--rw-r--r--   0        0        0      173 2024-03-18 16:02:54.130839 semantha_sdk-7.0.0/semantha_sdk/model/type_enum.py
--rw-r--r--   0        0        0      398 2024-03-27 10:40:51.527394 semantha_sdk-7.0.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       37 2024-03-08 20:30:39.116486 semantha_sdk-7.0.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0    11509 2024-03-20 07:38:23.440665 semantha_sdk-7.0.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     4540 2024-03-08 20:30:39.129478 semantha_sdk-7.0.0/semantha_sdk/semantha/__init__.py
--rw-r--r--   0        0        0     1741 2024-03-08 20:30:39.135482 semantha_sdk-7.0.0/semantha_sdk/semantha/compare/__init__.py
--rw-r--r--   0        0        0     1199 2024-03-08 20:30:39.142482 semantha_sdk-7.0.0/semantha_sdk/semantha/customization.py
--rw-r--r--   0        0        0     1765 2024-03-08 20:30:39.147483 semantha_sdk-7.0.0/semantha_sdk/semantha/domain/__init__.py
--rw-r--r--   0        0        0      423 2024-03-08 20:30:39.152479 semantha_sdk-7.0.0/semantha_sdk/semantha/domain/settings.py
--rw-r--r--   0        0        0      155 2024-03-08 20:30:39.158484 semantha_sdk-7.0.0/semantha_sdk/semantha/files.py
--rw-r--r--   0        0        0    10217 2024-03-08 20:30:39.163486 semantha_sdk-7.0.0/semantha_sdk/semantha/library/__init__.py
--rw-r--r--   0        0        0     3192 2024-03-08 20:30:39.169488 semantha_sdk-7.0.0/semantha_sdk/semantha/library/document.py
--rw-r--r--   0        0        0     2165 2024-03-08 20:30:39.176037 semantha_sdk-7.0.0/semantha_sdk/semantha/library/documentiter.py
--rw-r--r--   0        0        0     1210 2024-03-08 20:30:39.182027 semantha_sdk-7.0.0/semantha_sdk/semantha/library/documenttags.py
--rw-r--r--   0        0        0     1319 2024-03-08 20:30:39.189036 semantha_sdk-7.0.0/semantha_sdk/semantha/library/metadata.py
--rw-r--r--   0        0        0      799 2024-03-08 20:30:39.195022 semantha_sdk-7.0.0/semantha_sdk/semantha/library/reference.py
--rw-r--r--   0        0        0      652 2024-03-08 20:30:39.201033 semantha_sdk-7.0.0/semantha_sdk/semantha/library/tags.py
--rw-r--r--   0        0        0      393 2024-03-08 20:30:39.208014 semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/__init__.py
--rw-r--r--   0        0        0      311 2024-03-08 20:30:39.214014 semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/dense.py
--rw-r--r--   0        0        0      925 2024-03-08 20:30:39.219016 semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/hybrid.py
--rw-r--r--   0        0        0      533 2024-03-08 20:30:39.224012 semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/sparse.py
--rw-r--r--   0        0        0    25922 1970-01-01 00:00:00.000000 semantha_sdk-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6181 2024-04-23 13:32:48.112786 semantha_sdk-7.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    14639 2024-03-18 16:00:01.047358 semantha_sdk-7.1.0/DOCU.md
+-rw-r--r--   0        0        0    11545 2024-03-08 20:30:37.820624 semantha_sdk-7.1.0/LICENSE
+-rw-r--r--   0        0        0     1634 2024-04-23 13:33:01.367831 semantha_sdk-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4900 2024-03-08 20:30:37.825616 semantha_sdk-7.1.0/README.md
+-rw-r--r--   0        0        0     2652 2024-03-18 16:02:42.701241 semantha_sdk-7.1.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0     2718 2024-04-19 15:21:08.756667 semantha_sdk-7.1.0/semantha_sdk/administration/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-19 15:21:08.138905 semantha_sdk-7.1.0/semantha_sdk/administration/administration.py
+-rw-r--r--   0        0        0      979 2024-04-19 15:21:08.734443 semantha_sdk-7.1.0/semantha_sdk/administration/administration_api.py
+-rw-r--r--   0        0        0      892 2024-04-19 15:21:08.161224 semantha_sdk-7.1.0/semantha_sdk/administration/domain.py
+-rw-r--r--   0        0        0      793 2024-04-19 15:21:08.150671 semantha_sdk-7.1.0/semantha_sdk/administration/domains.py
+-rw-r--r--   0        0        0      501 2024-04-19 15:21:08.653632 semantha_sdk-7.1.0/semantha_sdk/administration/model/error_field.py
+-rw-r--r--   0        0        0      697 2024-04-19 15:21:08.663188 semantha_sdk-7.1.0/semantha_sdk/administration/model/import_detail.py
+-rw-r--r--   0        0        0      577 2024-04-19 15:21:08.670250 semantha_sdk-7.1.0/semantha_sdk/administration/model/import_information.py
+-rw-r--r--   0        0        0      416 2024-04-19 15:21:08.677803 semantha_sdk-7.1.0/semantha_sdk/administration/model/role.py
+-rw-r--r--   0        0        0      758 2024-04-19 15:21:08.688917 semantha_sdk-7.1.0/semantha_sdk/administration/model/user.py
+-rw-r--r--   0        0        0      696 2024-04-19 15:21:08.698582 semantha_sdk-7.1.0/semantha_sdk/administration/model/user_create.py
+-rw-r--r--   0        0        0      713 2024-04-19 15:21:08.704532 semantha_sdk-7.1.0/semantha_sdk/administration/model/user_update.py
+-rw-r--r--   0        0        0     1025 2024-04-19 15:21:08.248606 semantha_sdk-7.1.0/semantha_sdk/administration/roles.py
+-rw-r--r--   0        0        0     2871 2024-04-19 15:21:08.240040 semantha_sdk-7.1.0/semantha_sdk/administration/transport.py
+-rw-r--r--   0        0        0     1611 2024-04-19 15:21:08.280509 semantha_sdk-7.1.0/semantha_sdk/administration/user.py
+-rw-r--r--   0        0        0     1830 2024-04-19 15:21:08.262373 semantha_sdk-7.1.0/semantha_sdk/administration/users.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:30:38.006648 semantha_sdk-7.1.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     2122 2024-03-20 09:22:23.597528 semantha_sdk-7.1.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0      954 2024-03-20 09:22:23.585002 semantha_sdk-7.1.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      791 2024-03-20 09:22:23.465373 semantha_sdk-7.1.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      773 2024-03-20 09:22:23.479496 semantha_sdk-7.1.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1807 2024-03-20 09:22:23.569425 semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1512 2024-03-20 09:22:23.525618 semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_documenttypes.py
+-rw-r--r--   0        0        0     1842 2024-03-20 09:22:23.527619 semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     4894 2024-03-20 09:22:23.515082 semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3272 2024-03-20 09:22:23.530618 semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1325 2024-03-20 09:22:23.483496 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      916 2024-03-20 09:22:23.467380 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1920 2024-03-20 09:22:23.464373 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1755 2024-03-20 09:22:23.559904 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2993 2024-03-20 09:22:23.473411 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      794 2024-03-20 09:22:23.500525 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1677 2024-03-20 09:22:23.502526 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1722 2024-03-20 09:22:23.561904 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1355 2024-03-20 09:22:23.544350 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1614 2024-03-20 09:22:23.571424 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1238 2024-03-20 09:22:23.454854 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1299 2024-03-20 09:22:23.469411 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1189 2024-03-20 09:22:23.428298 semantha_sdk-7.1.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0      980 2024-03-20 09:22:23.441820 semantha_sdk-7.1.0/semantha_sdk/api/celltypes.py
+-rw-r--r--   0        0        0     1253 2024-03-20 09:22:23.492012 semantha_sdk-7.1.0/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     1299 2024-03-20 09:22:23.425292 semantha_sdk-7.1.0/semantha_sdk/api/clone.py
+-rw-r--r--   0        0        0     6426 2024-03-20 09:22:23.493518 semantha_sdk-7.1.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1209 2024-03-20 09:22:23.477496 semantha_sdk-7.1.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1359 2024-03-20 09:22:23.594522 semantha_sdk-7.1.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     1144 2024-03-20 09:22:23.556907 semantha_sdk-7.1.0/semantha_sdk/api/docclass_customfields.py
+-rw-r--r--   0        0        0     2241 2024-03-20 09:22:23.591008 semantha_sdk-7.1.0/semantha_sdk/api/docclass_documentclasses.py
+-rw-r--r--   0        0        0     1749 2024-03-20 09:22:23.504036 semantha_sdk-7.1.0/semantha_sdk/api/docclass_referencedocuments.py
+-rw-r--r--   0        0        0     3956 2024-03-20 09:22:23.545351 semantha_sdk-7.1.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     2513 2024-03-20 09:22:23.537832 semantha_sdk-7.1.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1979 2024-03-20 09:22:23.489011 semantha_sdk-7.1.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     6591 2024-03-20 09:22:23.476495 semantha_sdk-7.1.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     1991 2024-03-20 09:22:23.490012 semantha_sdk-7.1.0/semantha_sdk/api/documenttype.py
+-rw-r--r--   0        0        0     2049 2024-03-20 09:22:23.509042 semantha_sdk-7.1.0/semantha_sdk/api/documenttypes.py
+-rw-r--r--   0        0        0     4751 2024-03-20 09:22:23.437821 semantha_sdk-7.1.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1241 2024-03-20 09:22:23.549355 semantha_sdk-7.1.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      941 2024-03-20 09:22:23.417779 semantha_sdk-7.1.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1678 2024-03-20 09:22:23.497525 semantha_sdk-7.1.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1546 2024-03-20 09:22:23.512043 semantha_sdk-7.1.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1087 2024-03-20 09:22:23.552351 semantha_sdk-7.1.0/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0      998 2024-03-20 09:22:23.435820 semantha_sdk-7.1.0/semantha_sdk/api/model_backups.py
+-rw-r--r--   0        0        0     1512 2024-03-20 09:22:23.541834 semantha_sdk-7.1.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1907 2024-03-20 09:22:23.419779 semantha_sdk-7.1.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2073 2024-03-20 09:22:23.511043 semantha_sdk-7.1.0/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1561 2024-03-20 09:22:23.565418 semantha_sdk-7.1.0/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      888 2024-03-20 09:22:23.427298 semantha_sdk-7.1.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5799 2024-03-20 09:22:23.508042 semantha_sdk-7.1.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      769 2024-03-20 09:22:23.529618 semantha_sdk-7.1.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1888 2024-03-20 09:22:23.595522 semantha_sdk-7.1.0/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2480 2024-03-20 09:22:23.574937 semantha_sdk-7.1.0/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0     1019 2024-03-20 09:22:23.430298 semantha_sdk-7.1.0/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0      908 2024-03-20 09:22:23.572424 semantha_sdk-7.1.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0     1037 2024-03-20 09:22:23.471406 semantha_sdk-7.1.0/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1942 2024-03-20 09:22:23.554904 semantha_sdk-7.1.0/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      904 2024-03-20 09:22:23.443326 semantha_sdk-7.1.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1956 2024-03-20 09:22:23.567424 semantha_sdk-7.1.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1549 2024-03-20 09:22:23.481495 semantha_sdk-7.1.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0     1056 2024-03-20 09:22:23.495526 semantha_sdk-7.1.0/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1543 2024-03-20 09:22:23.485012 semantha_sdk-7.1.0/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1450 2024-03-20 09:22:23.589009 semantha_sdk-7.1.0/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1830 2024-03-20 09:22:23.450341 semantha_sdk-7.1.0/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1495 2024-03-20 09:22:23.583489 semantha_sdk-7.1.0/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1884 2024-03-20 09:22:23.498526 semantha_sdk-7.1.0/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1435 2024-03-20 09:22:23.518089 semantha_sdk-7.1.0/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0     1070 2024-03-20 09:22:23.461860 semantha_sdk-7.1.0/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1938 2024-03-20 09:22:23.432330 semantha_sdk-7.1.0/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1500 2024-03-20 09:22:23.579944 semantha_sdk-7.1.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1889 2024-03-20 09:22:23.453846 semantha_sdk-7.1.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1480 2024-03-20 09:22:23.540832 semantha_sdk-7.1.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1863 2024-03-20 09:22:23.433813 semantha_sdk-7.1.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1277 2024-03-20 09:22:23.558904 semantha_sdk-7.1.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     4972 2024-03-20 09:22:23.575943 semantha_sdk-7.1.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1462 2024-03-20 09:22:23.520089 semantha_sdk-7.1.0/semantha_sdk/api/modelont_attribute.py
+-rw-r--r--   0        0        0     1881 2024-03-20 09:22:23.522090 semantha_sdk-7.1.0/semantha_sdk/api/modelont_attributes.py
+-rw-r--r--   0        0        0     1963 2024-03-20 09:22:23.524612 semantha_sdk-7.1.0/semantha_sdk/api/modelont_class.py
+-rw-r--r--   0        0        0     2460 2024-03-20 09:22:23.487015 semantha_sdk-7.1.0/semantha_sdk/api/modelont_classes.py
+-rw-r--r--   0        0        0     1501 2024-03-20 09:22:23.474496 semantha_sdk-7.1.0/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2594 2024-03-20 09:22:23.587009 semantha_sdk-7.1.0/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1269 2024-03-20 09:22:23.592008 semantha_sdk-7.1.0/semantha_sdk/api/modelontclass_instances.py
+-rw-r--r--   0        0        0     1848 2024-03-20 09:22:23.516089 semantha_sdk-7.1.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1831 2024-03-20 09:22:23.439821 semantha_sdk-7.1.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      795 2024-03-20 09:22:23.563410 semantha_sdk-7.1.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2545 2024-03-20 09:22:23.506043 semantha_sdk-7.1.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    16724 2024-03-20 09:22:23.533621 semantha_sdk-7.1.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    22091 2024-03-20 09:22:23.446341 semantha_sdk-7.1.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      895 2024-03-20 09:22:23.581489 semantha_sdk-7.1.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2430 2024-03-18 16:00:01.061363 semantha_sdk-7.1.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0     1091 2024-03-20 09:22:23.577944 semantha_sdk-7.1.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      788 2024-03-20 09:22:23.547350 semantha_sdk-7.1.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1664 2024-03-20 09:22:23.445335 semantha_sdk-7.1.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5082 2024-03-20 09:22:23.423285 semantha_sdk-7.1.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4589 2024-03-20 09:22:23.458860 semantha_sdk-7.1.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0     1071 2024-03-20 09:22:23.448341 semantha_sdk-7.1.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     2583 2024-03-28 16:09:02.684081 semantha_sdk-7.1.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      910 2024-03-20 09:22:23.451341 semantha_sdk-7.1.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1361 2024-03-20 09:22:23.456861 semantha_sdk-7.1.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1070 2024-03-20 09:22:23.460860 semantha_sdk-7.1.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1559 2024-03-20 09:22:23.421779 semantha_sdk-7.1.0/semantha_sdk/api/transactions.py
+-rw-r--r--   0        0        0     1338 2024-03-20 09:22:23.551352 semantha_sdk-7.1.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     6740 2024-03-18 16:00:01.028358 semantha_sdk-7.1.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      548 2024-03-27 10:40:51.164272 semantha_sdk-7.1.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      632 2024-03-27 10:40:51.167272 semantha_sdk-7.1.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      507 2024-03-27 10:40:51.171316 semantha_sdk-7.1.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      487 2024-03-27 10:40:51.174875 semantha_sdk-7.1.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      358 2024-03-27 10:40:51.177881 semantha_sdk-7.1.0/semantha_sdk/model/area.py
+-rw-r--r--   0        0        0      710 2024-03-27 10:40:51.181389 semantha_sdk-7.1.0/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      823 2024-03-27 10:40:51.184402 semantha_sdk-7.1.0/semantha_sdk/model/attribute.py
+-rw-r--r--   0        0        0      479 2024-03-27 10:40:51.187402 semantha_sdk-7.1.0/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      525 2024-03-27 10:40:51.190529 semantha_sdk-7.1.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      350 2024-03-27 10:40:51.193736 semantha_sdk-7.1.0/semantha_sdk/model/cell_type.py
+-rw-r--r--   0        0        0      972 2024-03-27 10:40:51.196966 semantha_sdk-7.1.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      751 2024-03-27 10:40:51.200983 semantha_sdk-7.1.0/semantha_sdk/model/classes_overview.py
+-rw-r--r--   0        0        0      799 2024-03-27 10:40:51.205516 semantha_sdk-7.1.0/semantha_sdk/model/clazz.py
+-rw-r--r--   0        0        0      557 2024-03-27 10:40:51.208514 semantha_sdk-7.1.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      640 2024-03-27 10:40:51.213038 semantha_sdk-7.1.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0      197 2024-03-18 16:03:00.140284 semantha_sdk-7.1.0/semantha_sdk/model/clusteringstructure_enum.py
+-rw-r--r--   0        0        0     1180 2024-03-27 10:40:51.216049 semantha_sdk-7.1.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      565 2024-03-27 10:40:51.219047 semantha_sdk-7.1.0/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      634 2024-03-27 10:40:51.221556 semantha_sdk-7.1.0/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      443 2024-03-27 10:40:51.224578 semantha_sdk-7.1.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      361 2024-03-27 10:40:51.228578 semantha_sdk-7.1.0/semantha_sdk/model/custom_field.py
+-rw-r--r--   0        0        0      575 2024-03-27 10:40:51.232098 semantha_sdk-7.1.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      348 2024-03-27 10:40:51.234620 semantha_sdk-7.1.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      471 2024-03-27 10:40:51.237619 semantha_sdk-7.1.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1372 2024-03-27 10:40:51.241135 semantha_sdk-7.1.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1110 2024-03-27 10:40:51.245149 semantha_sdk-7.1.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0     1043 2024-03-27 10:40:51.248146 semantha_sdk-7.1.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      654 2024-03-27 10:40:51.251654 semantha_sdk-7.1.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      647 2024-03-27 10:40:51.253674 semantha_sdk-7.1.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1134 2024-03-27 10:40:51.257675 semantha_sdk-7.1.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      437 2024-03-27 10:40:51.261201 semantha_sdk-7.1.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      432 2024-03-27 10:40:51.266910 semantha_sdk-7.1.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      452 2024-03-27 10:40:51.270919 semantha_sdk-7.1.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      632 2024-03-27 10:40:51.274952 semantha_sdk-7.1.0/semantha_sdk/model/document_type.py
+-rw-r--r--   0        0        0      797 2024-03-27 10:40:51.277951 semantha_sdk-7.1.0/semantha_sdk/model/document_type_change.py
+-rw-r--r--   0        0        0     1155 2024-03-27 10:40:51.281459 semantha_sdk-7.1.0/semantha_sdk/model/document_type_config.py
+-rw-r--r--   0        0        0      175 2024-03-18 16:03:00.143266 semantha_sdk-7.1.0/semantha_sdk/model/documentmode_enum.py
+-rw-r--r--   0        0        0      401 2024-03-27 10:40:51.284476 semantha_sdk-7.1.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      359 2024-03-27 10:40:51.287477 semantha_sdk-7.1.0/semantha_sdk/model/domain_info.py
+-rw-r--r--   0        0        0      374 2024-03-27 10:40:51.292010 semantha_sdk-7.1.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      621 2024-03-27 10:40:51.295019 semantha_sdk-7.1.0/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      529 2024-03-27 10:40:51.300403 semantha_sdk-7.1.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      725 2024-03-27 10:40:51.303942 semantha_sdk-7.1.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      479 2024-03-27 10:40:51.307942 semantha_sdk-7.1.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      909 2024-03-27 10:40:51.311450 semantha_sdk-7.1.0/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      742 2024-03-27 10:40:51.314470 semantha_sdk-7.1.0/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      855 2024-03-27 10:40:51.320976 semantha_sdk-7.1.0/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      656 2024-03-27 10:40:51.325998 semantha_sdk-7.1.0/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      874 2024-03-27 10:40:51.329001 semantha_sdk-7.1.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      326 2024-03-27 10:40:51.332535 semantha_sdk-7.1.0/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      455 2024-03-27 10:40:51.336545 semantha_sdk-7.1.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      441 2024-03-27 10:40:51.338542 semantha_sdk-7.1.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      421 2024-03-27 10:40:51.342069 semantha_sdk-7.1.0/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      372 2024-03-27 10:40:51.345076 semantha_sdk-7.1.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0     1018 2024-03-27 10:40:51.349599 semantha_sdk-7.1.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      471 2024-03-27 10:40:51.353124 semantha_sdk-7.1.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      513 2024-03-27 10:40:51.356138 semantha_sdk-7.1.0/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      329 2024-03-27 10:40:51.359156 semantha_sdk-7.1.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      354 2024-03-27 10:40:51.362302 semantha_sdk-7.1.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      442 2024-03-27 10:40:51.365306 semantha_sdk-7.1.0/semantha_sdk/model/link.py
+-rw-r--r--   0        0        0      527 2024-03-27 10:40:51.368302 semantha_sdk-7.1.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      417 2024-03-27 10:40:51.370303 semantha_sdk-7.1.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      397 2024-03-27 10:40:51.373824 semantha_sdk-7.1.0/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      542 2024-03-27 10:40:51.377335 semantha_sdk-7.1.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      442 2024-03-27 10:40:51.381075 semantha_sdk-7.1.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      338 2024-03-27 10:40:51.384252 semantha_sdk-7.1.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      351 2024-03-27 10:40:51.386250 semantha_sdk-7.1.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      338 2024-03-18 16:02:54.126838 semantha_sdk-7.1.0/semantha_sdk/model/mode_enum.py
+-rw-r--r--   0        0        0      673 2024-03-27 10:40:51.389251 semantha_sdk-7.1.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1547 2024-03-27 10:40:51.391764 semantha_sdk-7.1.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      446 2024-03-27 10:40:51.394790 semantha_sdk-7.1.0/semantha_sdk/model/model_metadata.py
+-rw-r--r--   0        0        0      311 2024-03-27 10:40:51.397793 semantha_sdk-7.1.0/semantha_sdk/model/name.py
+-rw-r--r--   0        0        0      421 2024-03-27 10:40:51.401299 semantha_sdk-7.1.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      417 2024-03-27 10:40:51.403308 semantha_sdk-7.1.0/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      778 2024-03-27 10:40:51.408311 semantha_sdk-7.1.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      470 2024-03-27 10:40:51.412977 semantha_sdk-7.1.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1031 2024-03-27 10:40:51.416988 semantha_sdk-7.1.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      420 2024-03-27 10:40:51.420987 semantha_sdk-7.1.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      463 2024-03-27 10:40:51.425129 semantha_sdk-7.1.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      519 2024-03-27 10:40:51.429130 semantha_sdk-7.1.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      432 2024-03-27 10:40:51.433663 semantha_sdk-7.1.0/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      196 2024-03-18 16:02:54.127838 semantha_sdk-7.1.0/semantha_sdk/model/range_enum.py
+-rw-r--r--   0        0        0      372 2024-03-27 10:40:51.437660 semantha_sdk-7.1.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      817 2024-03-27 10:40:51.442189 semantha_sdk-7.1.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      678 2024-03-27 10:40:51.446263 semantha_sdk-7.1.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      386 2024-03-27 10:40:51.449255 semantha_sdk-7.1.0/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      626 2024-03-27 10:40:51.452453 semantha_sdk-7.1.0/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      427 2024-03-27 10:40:51.455454 semantha_sdk-7.1.0/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      651 2024-03-27 10:40:51.458460 semantha_sdk-7.1.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      442 2024-03-27 10:40:51.461974 semantha_sdk-7.1.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      611 2024-03-27 10:40:51.464984 semantha_sdk-7.1.0/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      493 2024-03-27 10:40:51.467982 semantha_sdk-7.1.0/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      528 2024-03-27 10:40:51.470983 semantha_sdk-7.1.0/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      839 2024-03-27 10:40:51.474561 semantha_sdk-7.1.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      452 2024-03-27 10:40:51.478561 semantha_sdk-7.1.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      777 2024-03-27 10:40:51.482095 semantha_sdk-7.1.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1930 2024-03-27 10:40:51.485089 semantha_sdk-7.1.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      377 2024-03-27 10:40:51.488088 semantha_sdk-7.1.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      627 2024-03-27 10:40:51.491090 semantha_sdk-7.1.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      847 2024-03-27 10:40:51.494753 semantha_sdk-7.1.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      432 2024-03-27 10:40:51.498312 semantha_sdk-7.1.0/semantha_sdk/model/source_document.py
+-rw-r--r--   0        0        0      526 2024-03-27 10:40:51.501310 semantha_sdk-7.1.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      416 2024-03-27 10:40:51.505348 semantha_sdk-7.1.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      386 2024-03-27 10:40:51.508358 semantha_sdk-7.1.0/semantha_sdk/model/summarization.py
+-rw-r--r--   0        0        0      183 2024-03-18 16:02:54.129838 semantha_sdk-7.1.0/semantha_sdk/model/summarylength_enum.py
+-rw-r--r--   0        0        0      521 2024-03-27 10:40:51.511865 semantha_sdk-7.1.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      371 2024-03-27 10:40:51.514875 semantha_sdk-7.1.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      498 2024-03-27 10:40:51.517874 semantha_sdk-7.1.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      396 2024-03-27 10:40:51.519873 semantha_sdk-7.1.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      410 2024-03-27 10:40:51.523416 semantha_sdk-7.1.0/semantha_sdk/model/transaction_summary.py
+-rw-r--r--   0        0        0      173 2024-03-18 16:02:54.130839 semantha_sdk-7.1.0/semantha_sdk/model/type_enum.py
+-rw-r--r--   0        0        0      398 2024-03-27 10:40:51.527394 semantha_sdk-7.1.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       37 2024-03-08 20:30:39.116486 semantha_sdk-7.1.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0    11296 2024-04-23 13:30:21.794342 semantha_sdk-7.1.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0     4540 2024-03-08 20:30:39.129478 semantha_sdk-7.1.0/semantha_sdk/semantha/__init__.py
+-rw-r--r--   0        0        0     1741 2024-03-08 20:30:39.135482 semantha_sdk-7.1.0/semantha_sdk/semantha/compare/__init__.py
+-rw-r--r--   0        0        0     1199 2024-03-08 20:30:39.142482 semantha_sdk-7.1.0/semantha_sdk/semantha/customization.py
+-rw-r--r--   0        0        0     1765 2024-03-08 20:30:39.147483 semantha_sdk-7.1.0/semantha_sdk/semantha/domain/__init__.py
+-rw-r--r--   0        0        0      423 2024-03-08 20:30:39.152479 semantha_sdk-7.1.0/semantha_sdk/semantha/domain/settings.py
+-rw-r--r--   0        0        0      155 2024-03-08 20:30:39.158484 semantha_sdk-7.1.0/semantha_sdk/semantha/files.py
+-rw-r--r--   0        0        0    10217 2024-03-08 20:30:39.163486 semantha_sdk-7.1.0/semantha_sdk/semantha/library/__init__.py
+-rw-r--r--   0        0        0     3192 2024-03-08 20:30:39.169488 semantha_sdk-7.1.0/semantha_sdk/semantha/library/document.py
+-rw-r--r--   0        0        0     2165 2024-03-08 20:30:39.176037 semantha_sdk-7.1.0/semantha_sdk/semantha/library/documentiter.py
+-rw-r--r--   0        0        0     1210 2024-03-08 20:30:39.182027 semantha_sdk-7.1.0/semantha_sdk/semantha/library/documenttags.py
+-rw-r--r--   0        0        0     1319 2024-03-08 20:30:39.189036 semantha_sdk-7.1.0/semantha_sdk/semantha/library/metadata.py
+-rw-r--r--   0        0        0      799 2024-03-08 20:30:39.195022 semantha_sdk-7.1.0/semantha_sdk/semantha/library/reference.py
+-rw-r--r--   0        0        0      652 2024-03-08 20:30:39.201033 semantha_sdk-7.1.0/semantha_sdk/semantha/library/tags.py
+-rw-r--r--   0        0        0      393 2024-03-08 20:30:39.208014 semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/__init__.py
+-rw-r--r--   0        0        0      311 2024-03-08 20:30:39.214014 semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/dense.py
+-rw-r--r--   0        0        0      925 2024-03-08 20:30:39.219016 semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/hybrid.py
+-rw-r--r--   0        0        0      533 2024-03-08 20:30:39.224012 semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/sparse.py
+-rw-r--r--   0        0        0    26165 1970-01-01 00:00:00.000000 semantha_sdk-7.1.0/PKG-INFO
```

### Comparing `semantha_sdk-7.0.0/CHANGELOG.md` & `semantha_sdk-7.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog for the Python SDK for the semantha platform
 
+## [7.1.0] 2024-04-23
+### Added
+- Client for accessing "Administration Product" where you can create an export/import of the content of domain.
+
+### Fixed
+- Fixed a bug where list of strings as an input parameter was not serialized properly.
+
 ## [7.0.0] 2024-04-09
 - no changes
 
 ## [6.11.1] 2024-03-27
 ### Improved
 - Better handling of circular imports.
```

### Comparing `semantha_sdk-7.0.0/DOCU.md` & `semantha_sdk-7.1.0/DOCU.md`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/LICENSE` & `semantha_sdk-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/pyproject.toml` & `semantha_sdk-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "7.0.0"
+version = "7.1.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-7.0.0/README.md` & `semantha_sdk-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/answers.py` & `semantha_sdk-7.1.0/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulk.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_documenttypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_rules.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-7.1.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/celltypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/celltypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/child_extractorclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/child_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/clone.py` & `semantha_sdk-7.1.0/semantha_sdk/api/clone.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/clusters.py` & `semantha_sdk-7.1.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-7.1.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/diff.py` & `semantha_sdk-7.1.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/docclass_customfields.py` & `semantha_sdk-7.1.0/semantha_sdk/api/docclass_customfields.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/docclass_documentclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/docclass_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/docclass_referencedocuments.py` & `semantha_sdk-7.1.0/semantha_sdk/api/docclass_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documents.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documenttype.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documenttype.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/documenttypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/domain.py` & `semantha_sdk-7.1.0/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/domains.py` & `semantha_sdk-7.1.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/info.py` & `semantha_sdk-7.1.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/languages.py` & `semantha_sdk-7.1.0/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_attributes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_backups.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_backups.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_boostword.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_boostword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_dataproperties.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_dataproperty.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_dataproperty.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_extractorclass.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_extractorclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_extractorclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_extractors.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_extractors.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_formatters.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_formatters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_metadata.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_objectproperties.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_objectproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_onemetadata.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_onemetadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_regex.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_regex.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_regexes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_regexes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_relation.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_relations.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_relations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_rule.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_rulefunctions.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_rulefunctions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_rules.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_stopword.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_stopword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_synonym.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-7.1.0/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_attribute.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_attributes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_class.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_classes.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_instance.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelont_instances.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelont_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/modelontclass_instances.py` & `semantha_sdk-7.1.0/semantha_sdk/api/modelontclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-7.1.0/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-7.1.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-7.1.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-7.1.0/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-7.1.0/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/references.py` & `semantha_sdk-7.1.0/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/roles.py` & `semantha_sdk-7.1.0/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-7.1.0/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/sentence.py` & `semantha_sdk-7.1.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/sentences.py` & `semantha_sdk-7.1.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/settings.py` & `semantha_sdk-7.1.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-7.1.0/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-7.1.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/statistic.py` & `semantha_sdk-7.1.0/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/summarizations.py` & `semantha_sdk-7.1.0/semantha_sdk/api/summarizations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/tag.py` & `semantha_sdk-7.1.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-7.1.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/tags.py` & `semantha_sdk-7.1.0/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/transactions.py` & `semantha_sdk-7.1.0/semantha_sdk/api/transactions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/api/validation.py` & `semantha_sdk-7.1.0/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-7.1.0/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-7.1.0/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/argument.py` & `semantha_sdk-7.1.0/semantha_sdk/model/argument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/attribute.py` & `semantha_sdk-7.1.0/semantha_sdk/model/attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-7.1.0/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-7.1.0/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/classes_overview.py` & `semantha_sdk-7.1.0/semantha_sdk/model/classes_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/clazz.py` & `semantha_sdk-7.1.0/semantha_sdk/model/clazz.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/clustered_document.py` & `semantha_sdk-7.1.0/semantha_sdk/model/clustered_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-7.1.0/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-7.1.0/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/condition.py` & `semantha_sdk-7.1.0/semantha_sdk/model/condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/condition_value.py` & `semantha_sdk-7.1.0/semantha_sdk/model/condition_value.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/data_property.py` & `semantha_sdk-7.1.0/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_class.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_class_node.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_information.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_type.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_type.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_type_change.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_type_change.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/document_type_config.py` & `semantha_sdk-7.1.0/semantha_sdk/model/document_type_config.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/expression.py` & `semantha_sdk-7.1.0/semantha_sdk/model/expression.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extractor.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extractor.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extractor_attribute.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extractor_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extractor_class.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extractor_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/extractor_class_overview.py` & `semantha_sdk-7.1.0/semantha_sdk/model/extractor_class_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/features.py` & `semantha_sdk-7.1.0/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/instance.py` & `semantha_sdk-7.1.0/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/instance_overview.py` & `semantha_sdk-7.1.0/semantha_sdk/model/instance_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-7.1.0/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-7.1.0/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/model_class.py` & `semantha_sdk-7.1.0/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-7.1.0/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/page.py` & `semantha_sdk-7.1.0/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-7.1.0/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/process_information.py` & `semantha_sdk-7.1.0/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/reference.py` & `semantha_sdk-7.1.0/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-7.1.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/relation.py` & `semantha_sdk-7.1.0/semantha_sdk/model/relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-7.1.0/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/rule.py` & `semantha_sdk-7.1.0/semantha_sdk/model/rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/rule_overview.py` & `semantha_sdk-7.1.0/semantha_sdk/model/rule_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-7.1.0/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/sentence.py` & `semantha_sdk-7.1.0/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/settings.py` & `semantha_sdk-7.1.0/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-7.1.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-7.1.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/statistic.py` & `semantha_sdk-7.1.0/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/model/synonym.py` & `semantha_sdk-7.1.0/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/compare/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/compare/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/customization.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/customization.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/domain/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/__init__.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/document.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/documentiter.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/documentiter.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/documenttags.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/documenttags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/metadata.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/reference.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/library/tags.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/library/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/hybrid.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/hybrid.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/semantha_sdk/semantha/ranking/sparse.py` & `semantha_sdk-7.1.0/semantha_sdk/semantha/ranking/sparse.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-7.0.0/PKG-INFO` & `semantha_sdk-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 7.0.0
+Version: 7.1.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -135,14 +135,21 @@
 annotated_pdf = api.domains(domain).documentannotations.post_as_pdf(file=pdf, similaritythreshold=0.85)
 with open('annotated.pdf', 'wb') as annotated_file:
     annotated_file.write(annotated_pdf.getbuffer())
 ```
 
 # Changelog for the Python SDK for the semantha platform
 
+## [7.1.0] 2024-04-23
+### Added
+- Client for accessing "Administration Product" where you can create an export/import of the content of domain.
+
+### Fixed
+- Fixed a bug where list of strings as an input parameter was not serialized properly.
+
 ## [7.0.0] 2024-04-09
 - no changes
 
 ## [6.11.1] 2024-03-27
 ### Improved
 - Better handling of circular imports.
```

