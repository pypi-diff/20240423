# Comparing `tmp/cognite_neat-0.74.0.tar.gz` & `tmp/cognite_neat-0.75.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.74.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.75.1.tar", max compression
```

## Comparing `cognite_neat-0.74.0.tar` & `cognite_neat-0.75.1.tar`

### file list

```diff
@@ -1,236 +1,257 @@
--rw-r--r--   0        0        0    11351 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/README.md
--rw-r--r--   0        0        0       61 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3583 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     7915 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-23 08:07:37.409094 cognite_neat-0.74.0/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-23 08:07:37.413094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1421276 2024-04-23 08:07:37.421094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js
--rw-r--r--   0        0        0     2667 2024-04-23 08:07:37.421094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.LICENSE.txt
--rw-r--r--   0        0        0  6279450 2024-04-23 08:07:37.445094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.map
--rw-r--r--   0        0        0   240334 2024-04-23 08:07:37.445094 cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-23 08:07:37.453094 cognite_neat-0.74.0/cognite/neat/config.py
--rw-r--r--   0        0        0     1205 2024-04-23 08:07:37.453094 cognite_neat-0.74.0/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-23 08:07:37.453094 cognite_neat-0.74.0/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-23 08:07:37.453094 cognite_neat-0.74.0/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-23 08:07:37.457094 cognite_neat-0.74.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11720 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17652 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-23 08:07:37.461094 cognite_neat-0.74.0/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    36770 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8305 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11854 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13146 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19922 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7713 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10427 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-23 08:07:37.465094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7791 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7120 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11481 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15314 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1299 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    16681 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    11025 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    55886 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    30418 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2566 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    21653 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4395 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-23 08:07:37.469094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6288 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18679 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12522 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-23 08:07:37.473094 cognite_neat-0.74.0/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4540 2024-04-23 08:07:37.857093 cognite_neat-0.74.0/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.74.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/README.md
+-rw-r--r--   0        0        0       61 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-23 12:35:18.753248 cognite_neat-0.75.1/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3533 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13661 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8107 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-23 12:35:18.757248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1421276 2024-04-23 12:35:18.765248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js
+-rw-r--r--   0        0        0     2667 2024-04-23 12:35:18.765248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.LICENSE.txt
+-rw-r--r--   0        0        0  6279450 2024-04-23 12:35:18.789248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.map
+-rw-r--r--   0        0        0   240334 2024-04-23 12:35:18.789248 cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-23 12:35:18.797248 cognite_neat-0.75.1/cognite/neat/config.py
+-rw-r--r--   0        0        0     1227 2024-04-23 12:35:18.797248 cognite_neat-0.75.1/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-23 12:35:18.797248 cognite_neat-0.75.1/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-23 12:35:18.797248 cognite_neat-0.75.1/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-23 12:35:18.801248 cognite_neat-0.75.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14947 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-23 12:35:18.805248 cognite_neat-0.75.1/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14909 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23859 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2399 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40480 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22715 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12995 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-23 12:35:18.809248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14738 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36814 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5783 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7727 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-23 12:35:18.813248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19612 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11853 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13145 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19900 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4090 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4267 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10425 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12553 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6924 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11925 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     7118 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11480 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4197 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15314 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     4893 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/models/_entity.py
+-rw-r--r--   0        0        0     7228 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-04-23 12:35:18.817248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    11024 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    55890 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    30417 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2567 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    21658 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0     1299 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0    12212 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_value.py
+-rw-r--r--   0        0        0       68 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18678 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7325 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29416 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27324 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12728 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2361 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20706 2024-04-23 12:35:18.821248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28111 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-23 12:35:18.825248 cognite_neat-0.75.1/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4540 2024-04-23 12:35:19.209247 cognite_neat-0.75.1/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.1/PKG-INFO
```

### Comparing `cognite_neat-0.74.0/LICENSE` & `cognite_neat-0.75.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/README.md` & `cognite_neat-0.75.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/configuration.py` & `cognite_neat-0.75.1/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.75.1/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.75.1/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/explorer.py` & `cognite_neat-0.75.1/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from pathlib import Path
 from typing import cast
 
 from fastapi import APIRouter, UploadFile
 
 from cognite.neat.app.api.configuration import NEAT_APP
 from cognite.neat.rules import exporters, importers
-from cognite.neat.rules.models._rules import DMSRules
-from cognite.neat.rules.models._rules.base import RoleTypes
+from cognite.neat.rules.models.rules import DMSRules, RoleTypes
 
 router = APIRouter()
 
 
 @router.post("/api/core/convert")
 async def convert_data_model_to_rules(file: UploadFile):
     suffix = Path(cast(str, file.filename)).suffix
```

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/data_exploration.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     DatatypePropertyRequest,
     NodesAndEdgesRequest,
     QueryRequest,
     RuleRequest,
 )
 from cognite.neat.app.api.utils.data_mapping import rdf_result_to_api_response
 from cognite.neat.app.api.utils.query_templates import query_templates
-from cognite.neat.graph.transformation import query_generator
+from cognite.neat.legacy.graph.transformations import query_generator
 from cognite.neat.utils.utils import remove_namespace
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 
 router = APIRouter()
 
 
 @router.get("/api/list-queries")
```

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from typing import Any, cast
 
 from fastapi import APIRouter, Response
 from rdflib import Namespace
 
 from cognite.neat.app.api.configuration import NEAT_APP
 from cognite.neat.app.api.data_classes.rest import TransformationRulesUpdateRequest
-from cognite.neat.rules import exporter, importer, importers
-from cognite.neat.rules.models._base import EntityTypes
-from cognite.neat.rules.models._rules.base import RoleTypes
-from cognite.neat.rules.models.rules import Class, Classes, Metadata, Properties, Property, Rules
+from cognite.neat.legacy.rules import exporters as legacy_exporters
+from cognite.neat.legacy.rules import importers as legacy_importers
+from cognite.neat.legacy.rules.models._base import EntityTypes
+from cognite.neat.legacy.rules.models.rules import Class, Classes, Metadata, Properties, Property, Rules
+from cognite.neat.rules import importers
+from cognite.neat.rules.models.rules import RoleTypes
 from cognite.neat.workflows.steps.data_contracts import RulesData
 from cognite.neat.workflows.steps.lib.rules_exporter import RulesToExcel
 from cognite.neat.workflows.steps.lib.rules_importer import ExcelToRules
 from cognite.neat.workflows.steps.lib.v1.rules_importer import ImportExcelToRules
 from cognite.neat.workflows.utils import get_file_hash
 
 router = APIRouter()
@@ -86,15 +88,17 @@
     error_text = ""
     properties = []
     classes = []
     remaped_rules = {}
     try:
         # Trying to load rules V1
         if rules_schema_version == "" or rules_schema_version == "v1":
-            rules = cast(Rules, importer.ExcelImporter(path).to_rules(return_report=False, skip_validation=False))
+            rules = cast(
+                Rules, legacy_importers.ExcelImporter(path).to_rules(return_report=False, skip_validation=False)
+            )
             properties = [
                 {
                     "class": value.class_id,
                     "property": value.property_id,
                     "property_description": value.description,
                     "property_type": (
                         value.expected_value_type.versioned_id
@@ -144,15 +148,17 @@
     }
 
 
 @router.get("/api/rules/from_file")
 def get_original_rules_from_file(file_name: str):
     # """Endpoint for retrieving raw transformation from file"""
     path = Path(NEAT_APP.config.rules_store_path) / file_name
-    rules = cast(Rules, importer.ExcelImporter(filepath=path).to_rules(return_report=False, skip_validation=False))
+    rules = cast(
+        Rules, legacy_importers.ExcelImporter(filepath=path).to_rules(return_report=False, skip_validation=False)
+    )
     return Response(content=rules.model_dump_json(), media_type="application/json")
 
 
 @router.get("/api/rules/from_workflow")
 def get_original_rules_from_workflow(workflow_name: str):
     """Endpoing for retrieving transformation from memmory"""
     workflow = NEAT_APP.workflow_manager.get_workflow(workflow_name)
@@ -189,9 +195,9 @@
     if request.output_format == "excel":
         rules_file = Path(request.file_name)
         if str(rules_file.parent) == ".":
             path = Path(NEAT_APP.config.rules_store_path) / rules_file
         else:
             path = Path(NEAT_APP.config.data_store_path) / rules_file
 
-        exporter.ExcelExporter(rules=rules).export_to_file(path)
+        legacy_exporters.ExcelExporter(rules=rules).export_to_file(path)
     return {"status": "ok"}
```

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.75.1/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.75.1/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.75.1/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.75.1/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.75.1/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.LICENSE.txt` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.map` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/js/main.25d27396.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.75.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/config.py` & `cognite_neat-0.75.1/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/constants.py` & `cognite_neat-0.75.1/cognite/neat/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from rdflib import DCTERMS, OWL, RDF, RDFS, SKOS, XSD, Namespace
 
 from cognite import neat
 
 PACKAGE_DIRECTORY = Path(neat.__file__).parent
 
 
-EXAMPLE_RULES = PACKAGE_DIRECTORY / "rules" / "examples"
-EXAMPLE_GRAPHS = PACKAGE_DIRECTORY / "graph" / "examples"
+EXAMPLE_RULES = PACKAGE_DIRECTORY / "legacy" / "rules" / "examples"
+EXAMPLE_GRAPHS = PACKAGE_DIRECTORY / "legacy" / "graph" / "examples"
 EXAMPLE_WORKFLOWS = PACKAGE_DIRECTORY / "workflows" / "examples"
 
 DEFAULT_NAMESPACE = Namespace("http://purl.org/cognite/neat#")
 
 PREFIXES = {
     "rdf": RDF._NS,
     "rdfs": RDFS._NS,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/exceptions.py` & `cognite_neat-0.75.1/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/exceptions.py` & `cognite_neat-0.75.1/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 from xml.etree.ElementTree import Element
 
 from rdflib import OWL, RDF, RDFS, SKOS, XSD, Literal, Namespace, URIRef
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.graph.models import Triple
-from cognite.neat.rules.models._base import ALLOWED_PATTERN
+from cognite.neat.legacy.graph.models import Triple
+from cognite.neat.legacy.rules.models._base import ALLOWED_PATTERN
 from cognite.neat.utils.utils import get_namespace, remove_namespace
 from cognite.neat.utils.xml import get_children, iterate_tree
 
 from ._base import BaseExtractor
 
 _DEXPI_PREFIXES = {
     "dexpi": Namespace("http://sandbox.dexpi.org/rdl/"),
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from openpyxl.cell import Cell
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
 from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.datavalidation import DataValidation
 from openpyxl.worksheet.worksheet import Worksheet
 from rdflib import RDF, XSD, Literal, Namespace, URIRef
 
-from cognite.neat.graph import exceptions
-from cognite.neat.graph.exceptions import NamespaceRequired
-from cognite.neat.graph.models import Triple
-from cognite.neat.rules.analysis import get_defined_classes, to_class_property_pairs
-from cognite.neat.rules.exporter._rules2rules import to_dms_name
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph import exceptions
+from cognite.neat.legacy.graph.exceptions import NamespaceRequired
+from cognite.neat.legacy.graph.models import Triple
+from cognite.neat.legacy.rules.analysis import get_defined_classes, to_class_property_pairs
+from cognite.neat.legacy.rules.exporters._rules2rules import to_dms_name
+from cognite.neat.legacy.rules.models.rules import Rules
 
 from ._base import BaseExtractor
 
 
 class GraphCapturingSheet(BaseExtractor):
     """
     Graph capturing sheet class that provides methods for creating a graph capturing sheet and extracting RDF triples.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """This module is used to generate mock graph data for purposes of testing of NEAT.
 """
+
 import logging
 import random
 import warnings
 from collections import OrderedDict
 
 import numpy
 import pandas as pd
 from prometheus_client import Gauge
 from rdflib import RDF, Literal, Namespace, URIRef
 
-from cognite.neat.graph.models import Triple
-from cognite.neat.rules.analysis import (
+from cognite.neat.legacy.graph.models import Triple
+from cognite.neat.legacy.rules.analysis import (
     get_class_linkage,
     get_classes_with_properties,
     get_defined_classes,
     get_symmetric_pairs,
 )
-from cognite.neat.rules.exporter._rules2rules import subset_rules
-from cognite.neat.rules.models import Rules
-from cognite.neat.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.legacy.rules.exporters._rules2rules import subset_rules
+from cognite.neat.legacy.rules.models import Rules
+from cognite.neat.legacy.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
 from cognite.neat.utils.utils import remove_namespace
 
 from ._base import BaseExtractor
 
 neat_total_processed_mock_triples = Gauge(
     "neat_total_processed_mock_triples", "Number of processed mock triples", ["state"]
 )
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.1/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from typing import cast
 
 import numpy
 import pandas as pd
 from rdflib import RDF, Literal, Namespace, URIRef
 
 from cognite.neat.graph.models import Triple
-from cognite.neat.rules._analysis._information_rules import InformationArchitectRulesAnalysis
-from cognite.neat.rules.models._rules import DMSRules, InformationRules
-from cognite.neat.rules.models._rules._types import ClassEntity, EntityTypes, XSDValueType
-from cognite.neat.rules.models._rules.information_rules import InformationProperty
+from cognite.neat.rules.analysis import InformationArchitectRulesAnalysis
+from cognite.neat.rules.models.rules import DMSRules, InformationRules
+from cognite.neat.rules.models.rules._information_rules import InformationProperty
+from cognite.neat.rules.models.rules._types import ClassEntity, EntityTypes, XSDValueType
 from cognite.neat.utils.utils import remove_namespace
 
 from ._base import BaseExtractor
 
 
 class MockGraphGenerator(BaseExtractor):
     """
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cognite.neat.graph.loader.core.labels import upload_labels
+from cognite.neat.legacy.graph.loaders.core.labels import upload_labels
 
 from ._asset_loader import AssetLoader
 from ._base import BaseLoader, CogniteLoader
 from .core.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
 from .core.rdf_to_relationships import categorize_relationships, rdf2relationships, upload_relationships
 from .rdf_to_dms import DMSLoader, upload_edges, upload_nodes
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from typing import Any, Literal, overload
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetWrite, LabelDefinitionWrite, RelationshipWrite, RelationshipWriteList
 from pydantic_core import ErrorDetails
 from rdflib.query import ResultRow
 
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.rules.models import Rules
-from cognite.neat.rules.models.rules import Property
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.rules.models import Rules
+from cognite.neat.legacy.rules.models.rules import Property
 from cognite.neat.utils import remove_namespace
 from cognite.neat.utils.utils import epoch_now_ms
 
 from ._base import CogniteLoader
 
 if sys.version_info >= (3, 11):
     from datetime import UTC
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from typing import Generic, Literal, TypeVar, overload
 
 from cognite.client import CogniteClient
 from pydantic_core import ErrorDetails
 
-from cognite.neat.graph.models import Triple
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.graph.transformation.query_generator.sparql import build_construct_query
-from cognite.neat.rules.models import Rules
+from cognite.neat.legacy.graph.models import Triple
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.graph.transformations.query_generator.sparql import build_construct_query
+from cognite.neat.legacy.rules.models import Rules
 
 T_Output = TypeVar("T_Output")
 
 
 class BaseLoader(ABC, Generic[T_Output]):
     """Base class for all loaders.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import traceback
 from typing import cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelDefinition, LabelDefinitionList
 
-from cognite.neat.rules.exporter._core import get_labels
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.exporters._core import get_labels
+from cognite.neat.legacy.rules.models.rules import Rules
 
 
 def upload_labels(
     client: CogniteClient,
     rules: Rules,
     data_set_id: int,
     extra_labels: list | None = None,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from typing import ClassVar
 
 from pydantic import BaseModel, ConfigDict, root_validator, validator
 from rdflib import Namespace
 
-from cognite.neat.rules.models.rules import METADATA_VALUE_MAX_LENGTH
+from cognite.neat.legacy.rules.models.rules import METADATA_VALUE_MAX_LENGTH
 
 
 class AssetClassMapping(BaseModel):
     external_id: str
     name: str
     parent_external_id: str | None = None
     description: str | None = None
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList, AssetUpdate
 from cognite.client.exceptions import CogniteDuplicatedError
 from deepdiff import DeepDiff  # type: ignore[import]
 from rdflib import Graph
 from rdflib.term import URIRef
 
-from cognite.neat.graph.loader.core.models import AssetTemplate
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.rules.models.rules import Property, Rules
+from cognite.neat.legacy.graph.loaders.core.models import AssetTemplate
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.rules.models.rules import Property, Rules
 from cognite.neat.utils.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
 if sys.version_info >= (3, 11):
     from datetime import UTC
     from typing import Self
 else:
     from datetime import timezone
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from warnings import warn
 
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelFilter, Relationship, RelationshipUpdate
 from cognite.client.exceptions import CogniteDuplicatedError
 
-from cognite.neat.graph.exceptions import NamespaceRequired
-from cognite.neat.graph.loader.core.models import RelationshipDefinition, RelationshipDefinitions
-from cognite.neat.graph.loader.core.rdf_to_assets import _categorize_cdf_assets
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph.exceptions import NamespaceRequired
+from cognite.neat.legacy.graph.loaders.core.models import RelationshipDefinition, RelationshipDefinitions
+from cognite.neat.legacy.graph.loaders.core.rdf_to_assets import _categorize_cdf_assets
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.rules.models.rules import Rules
 from cognite.neat.utils.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
 
 
 def define_relationships(rules: Rules, data_set_id: int, stop_on_exception: bool = False) -> RelationshipDefinitions:
     """Define relationships from transformation rules
 
     Args:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from typing import Literal, cast, overload
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes.data_modeling import EdgeApply, InstanceApply, NodeApply
 from pydantic_core import ErrorDetails
 
 from cognite.neat.exceptions import NeatException
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.graph.transformation.query_generator.sparql import triples2dictionary
-from cognite.neat.rules.exporter._rules2dms import DMSSchemaComponents
-from cognite.neat.rules.exporter._rules2pydantic_models import add_class_prefix_to_xid, rules_to_pydantic_models
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.graph.transformations.query_generator.sparql import triples2dictionary
+from cognite.neat.legacy.rules.exporters._rules2dms import DMSSchemaComponents
+from cognite.neat.legacy.rules.exporters._rules2pydantic_models import add_class_prefix_to_xid, rules_to_pydantic_models
+from cognite.neat.legacy.rules.models.rules import Rules
 from cognite.neat.utils.utils import chunker, datetime_utc_now, retry_decorator
 
 from ._base import CogniteLoader
 
 
 class DMSLoader(CogniteLoader[InstanceApply]):
     """Loads a Neat Graph into CDF as nodes and edges.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/stores/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 import pandas as pd
 from prometheus_client import Gauge, Summary
 from rdflib import Graph, Namespace, URIRef
 from rdflib.query import Result, ResultRow
 
 from cognite.neat.constants import DEFAULT_NAMESPACE, PREFIXES
-from cognite.neat.graph.models import Triple
-from cognite.neat.graph.stores._rdf_to_graph import rdf_file_to_graph
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph.models import Triple
+from cognite.neat.legacy.graph.stores._rdf_to_graph import rdf_file_to_graph
+from cognite.neat.legacy.rules.models.rules import Rules
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-prom_qsm = Summary("store_query_time_summary", "Time spent processing queries", ["query"])
-prom_sq = Gauge("store_single_query_time", "Time spent processing a single query", ["query"])
+prom_qsm = Summary("store_query_time_summary_legacy", "Time spent processing queries", ["query"])
+prom_sq = Gauge("store_single_query_time_legacy", "Time spent processing a single query", ["query"])
 
 MIMETypes: TypeAlias = Literal[
     "application/rdf+xml", "text/turtle", "application/n-triple", "application/n-quads", "application/trig"
 ]
 
 
 class NeatGraphStoreBase(ABC):
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.1/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import cast
 
 from rdflib import Literal, URIRef
 
-from cognite.neat.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
 
 
 def simple_entity_matcher(
     graph_store: NeatGraphStoreBase,
     source_class: str,
     source_property: str,
     source_value_type: str = "single_value_str",
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from collections.abc import Iterable
 from typing import cast
 
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.rules.analysis import get_classes_with_properties
-from cognite.neat.rules.models._base import Triple
-from cognite.neat.rules.models.rdfpath import (
+from cognite.neat.legacy.rules.analysis import get_classes_with_properties
+from cognite.neat.legacy.rules.models._base import Triple
+from cognite.neat.legacy.rules.models.rdfpath import (
     AllProperties,
     AllReferences,
     Hop,
     SingleProperty,
     Step,
     TransformationRuleType,
     Traversal,
     parse_rule,
     parse_traversal,
 )
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.rules import Rules
 from cognite.neat.utils.utils import remove_namespace
 
 
 def _generate_prefix_header(prefixes: dict[str, Namespace] = PREFIXES) -> str:
     """Generate prefix header which is added to SPARQL query and allows for shorten query statements
 
     Parameters
@@ -425,17 +425,19 @@
     else:
         query_template = query_template.replace("insert_filter", "")
     return query_template
 
 
 def _triples2sparql_statement(triples: list[Triple]):
     return [
-        f"OPTIONAL {{ {triple.subject} {triple.predicate} {triple.object} . }}"
-        if triple.optional
-        else f"{triple.subject} {triple.predicate} {triple.object} ."
+        (
+            f"OPTIONAL {{ {triple.subject} {triple.predicate} {triple.object} . }}"
+            if triple.optional
+            else f"{triple.subject} {triple.predicate} {triple.object} ."
+        )
         for triple in triples
     ]
 
 
 def _to_construct_triples(
     graph: Graph, class_: str, transformation_rules: Rules, properties_optional: bool = True
 ) -> tuple[list[Triple], list[Triple]]:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.75.1/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,26 @@
 import pandas as pd
 from cognite.client import CogniteClient
 from prometheus_client import Gauge
 from pydantic import BaseModel
 from rdflib import RDF, Graph
 from rdflib.term import Literal, Node
 
-from cognite.neat.graph.exceptions import NamespaceRequired
-from cognite.neat.graph.transformation.query_generator.sparql import build_sparql_query
-from cognite.neat.rules.models._base import EntityTypes
-from cognite.neat.rules.models.rdfpath import AllProperties, AllReferences, Query, RawLookup, Traversal, parse_rule
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph.exceptions import NamespaceRequired
+from cognite.neat.legacy.graph.transformations.query_generator.sparql import build_sparql_query
+from cognite.neat.legacy.rules.models._base import EntityTypes
+from cognite.neat.legacy.rules.models.rdfpath import (
+    AllProperties,
+    AllReferences,
+    Query,
+    RawLookup,
+    Traversal,
+    parse_rule,
+)
+from cognite.neat.legacy.rules.models.rules import Rules
 from cognite.neat.utils.utils import remove_namespace
 
 prom_total_proc_rules_g = Gauge("neat_total_processed_rules", "Number of processed rules", ["state"])
 rules_processing_timing_metric = Gauge(
     "neat_rules_processing_timing", "Transformation rules processing timing metrics", ["aggregation"]
 )
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.75.1/cognite/neat/rules/analysis/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules._types import ClassEntity
+from cognite.neat.rules.models.rules._types import ClassEntity
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 else:
     from backports.strenum import StrEnum
 
 T_Rules = TypeVar("T_Rules", bound=Rules)
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/analysis/_information_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import warnings
 from collections import defaultdict
 from typing import Any, cast
 
 import pandas as pd
 from pydantic import ValidationError
 
-from cognite.neat.rules.models._rules._types._base import ClassEntity, EntityTypes, ParentClassEntity, ReferenceEntity
-from cognite.neat.rules.models._rules.base import SchemaCompleteness
-from cognite.neat.rules.models._rules.information_rules import InformationClass, InformationProperty, InformationRules
 from cognite.neat.rules.models.rdfpath import TransformationRuleType
+from cognite.neat.rules.models.rules._base import SchemaCompleteness
+from cognite.neat.rules.models.rules._information_rules import InformationClass, InformationProperty, InformationRules
+from cognite.neat.rules.models.rules._types._base import ClassEntity, EntityTypes, ParentClassEntity, ReferenceEntity
 from cognite.neat.utils.utils import get_inheritance_path
 
 from ._base import BaseAnalysis, DataModelingScenario
 
 
 class InformationArchitectRulesAnalysis(BaseAnalysis):
     def __init__(self, rules: InformationRules):
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/analysis.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 from collections import defaultdict
 
 import pandas as pd
 
-from cognite.neat.rules.models.rdfpath import TransformationRuleType
-from cognite.neat.rules.models.rules import Property, Rules
+from cognite.neat.legacy.rules.models.rdfpath import TransformationRuleType
+from cognite.neat.legacy.rules.models.rules import Property, Rules
 
 
 def get_defined_classes(transformation_rules: Rules) -> set[str]:
     """Returns classes that have properties defined for them in the data model.
 
     Args:
         transformation_rules: Instance of TransformationRules holding the data model
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exceptions.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Generic, TypeVar
 
-from cognite.neat.rules.models.raw_rules import RawRules
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.raw_rules import RawRules
+from cognite.neat.legacy.rules.models.rules import Rules
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 T_Export = TypeVar("T_Export")
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.rules import Rules
 
 
 def get_labels(transformation_rules: Rules) -> set[str]:
     """
     Return CDF labels for classes and relationships.
 
     Args:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
 from typing import ClassVar, Literal, cast, no_type_check
 
 import yaml
 
-from cognite.neat.rules.models.value_types import ValueTypeMapping
+from cognite.neat.legacy.rules.models.value_types import ValueTypeMapping
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 from cognite.client import CogniteClient
@@ -37,19 +37,19 @@
 from cognite.client.data_classes.data_modeling.views import (
     ConnectionDefinitionApply,
     SingleHopConnectionDefinitionApply,
 )
 from cognite.client.exceptions import CogniteAPIError
 from pydantic import BaseModel, ConfigDict, field_validator
 
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.exporter._base import BaseExporter
-from cognite.neat.rules.exporter._validation import are_entity_names_dms_compliant
-from cognite.neat.rules.models._base import ContainerEntity, EntityTypes, ParentClass
-from cognite.neat.rules.models.rules import Class, Property, Rules
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.exporters._base import BaseExporter
+from cognite.neat.legacy.rules.exporters._validation import are_entity_names_dms_compliant
+from cognite.neat.legacy.rules.models._base import ContainerEntity, EntityTypes, ParentClass
+from cognite.neat.legacy.rules.models.rules import Class, Property, Rules
 from cognite.neat.utils.utils import generate_exception_report
 
 if sys.version_info < (3, 11):
     from exceptiongroup import ExceptionGroup
 
 
 @dataclass
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import cast
 
 from openpyxl import Workbook
 from openpyxl.cell import Cell
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
 from openpyxl.worksheet.worksheet import Worksheet
 
-from cognite.neat.rules.models._base import EntityTypes
+from cognite.neat.legacy.rules.models._base import EntityTypes
 
 from ._base import BaseExporter
 
 
 class ExcelExporter(BaseExporter[Workbook]):
     """Class for exporting transformation rules object to excel file."""
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from typing import TYPE_CHECKING
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.analysis import to_class_property_pairs
-from cognite.neat.rules.exporter._validation import are_entity_names_dms_compliant, are_properties_redefined
-from cognite.neat.rules.models.rules import Rules
-from cognite.neat.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.analysis import to_class_property_pairs
+from cognite.neat.legacy.rules.exporters._validation import are_entity_names_dms_compliant, are_properties_redefined
+from cognite.neat.legacy.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
 from cognite.neat.utils.utils import generate_exception_report
 
 from ._base import BaseExporter
 
 if TYPE_CHECKING:
     from jinja2 import Template
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from pathlib import Path
 from typing import ClassVar
 
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 from rdflib import DCTERMS, OWL, RDF, RDFS, XSD, BNode, Graph, Literal, Namespace, URIRef
 from rdflib.collection import Collection as GraphCollection
 
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.analysis import to_class_property_pairs, to_property_dict
-from cognite.neat.rules.exporter._base import BaseExporter
-from cognite.neat.rules.exporter._validation import are_properties_redefined
-from cognite.neat.rules.models.rules import Class, Metadata, Property, Rules
-from cognite.neat.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.analysis import to_class_property_pairs, to_property_dict
+from cognite.neat.legacy.rules.exporters._base import BaseExporter
+from cognite.neat.legacy.rules.exporters._validation import are_properties_redefined
+from cognite.neat.legacy.rules.models.rules import Class, Metadata, Property, Rules
+from cognite.neat.legacy.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
 from cognite.neat.utils.utils import generate_exception_report, remove_namespace
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from cognite.client.data_classes.data_modeling import EdgeApply, MappedPropertyApply, NodeApply, NodeOrEdgeData, ViewId
 from cognite.client.data_classes.data_modeling.views import SingleHopConnectionDefinitionApply, ViewApply
 from pydantic import BaseModel, ConfigDict, Field, create_model
 from pydantic._internal._model_construction import ModelMetaclass
 from rdflib import Graph, URIRef
 from typing_extensions import TypeAliasType
 
-from cognite.neat.graph.loader.core.rdf_to_assets import NeatMetadataKeys
-from cognite.neat.graph.transformation.query_generator.sparql import build_construct_query, triples2dictionary
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.analysis import define_class_asset_mapping, to_class_property_pairs
-from cognite.neat.rules.exporter._rules2dms import DMSSchemaComponents
-from cognite.neat.rules.exporter._validation import are_entity_names_dms_compliant
-from cognite.neat.rules.models.rules import Property, Rules
-from cognite.neat.rules.models.value_types import ValueTypeMapping
+from cognite.neat.legacy.graph.loaders.core.rdf_to_assets import NeatMetadataKeys
+from cognite.neat.legacy.graph.transformations.query_generator.sparql import build_construct_query, triples2dictionary
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.analysis import define_class_asset_mapping, to_class_property_pairs
+from cognite.neat.legacy.rules.exporters._rules2dms import DMSSchemaComponents
+from cognite.neat.legacy.rules.exporters._validation import are_entity_names_dms_compliant
+from cognite.neat.legacy.rules.models.rules import Property, Rules
+from cognite.neat.legacy.rules.models.value_types import ValueTypeMapping
 from cognite.neat.utils.utils import generate_exception_report
 
 if sys.version_info >= (3, 11):
     from datetime import UTC
 else:
     from datetime import timezone
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """This module provides set of methods that perform conversion of TransformationRules
 to TransformationRules for purpose of for example:
 
 - subsetting the data model to only include desired classes and their properties
 - converting classes/properties ids/names to DMS compliant format
 """
+
 import logging
 import re
 import warnings
 from typing import Any
 
-from cognite.neat.rules.analysis import get_defined_classes
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.analysis import get_defined_classes
+from cognite.neat.legacy.rules.models.rules import Rules
 
 
 def subset_rules(rules: Rules, desired_classes: set, skip_validation: bool = False) -> Rules:
     """
     Subset transformation rules to only include desired classes and their properties.
 
     Args:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 
 from rdflib.term import Node
 
-from cognite.neat.rules.exporter._base import BaseExporter
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.rules import Rules
+
+from ._base import BaseExporter
 
 
 class TripleExporter(BaseExporter[list[tuple[Node, Node, Node]]]):
     """
     Exporter for transformation rules instances sheet to RDF triples
     """
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import warnings
 from typing import Literal, overload
 
 from cognite.neat.exceptions import wrangle_warnings
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.models.rules import (
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.models.rules import (
     Rules,
     dms_property_id_compliance_regex,
     value_id_compliance_regex,
     view_id_compliance_regex,
 )
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Generic, TypeVar
 
 from cognite.client import CogniteClient
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules import DMSRules, InformationRules, RoleTypes
+from cognite.neat.rules.models.rules import DMSRules, InformationRules, RoleTypes
 
 from ._models import UploadResult
 
 T_Export = TypeVar("T_Export")
 
 
 class BaseExporter(ABC, Generic[T_Export]):
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import Literal, TypeAlias, cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes._base import CogniteResourceList
 from cognite.client.exceptions import CogniteAPIError
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules import InformationRules
-from cognite.neat.rules.models._rules.base import ExtensionCategory, SheetList
-from cognite.neat.rules.models._rules.dms_architect_rules import DMSContainer, DMSRules
-from cognite.neat.rules.models._rules.dms_schema import DMSSchema, PipelineSchema
+from cognite.neat.rules.models.rules import InformationRules
+from cognite.neat.rules.models.rules._base import ExtensionCategory, SheetList
+from cognite.neat.rules.models.rules._dms_architect_rules import DMSContainer, DMSRules
+from cognite.neat.rules.models.rules._dms_schema import DMSSchema, PipelineSchema
 from cognite.neat.utils.cdf_loaders import (
     ContainerLoader,
     DataModelingLoader,
     DataModelLoader,
     RawDatabaseLoader,
     RawTableLoader,
     ResourceLoader,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from openpyxl import Workbook
 from openpyxl.cell import MergedCell
 from openpyxl.styles import Alignment, Border, Font, PatternFill, Side
 from openpyxl.worksheet.worksheet import Worksheet
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules import DMSRules, DomainRules, InformationRules
-from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness, SheetEntity
+from cognite.neat.rules.models.rules import DMSRules, DomainRules, InformationRules
+from cognite.neat.rules.models.rules._base import RoleTypes, SchemaCompleteness, SheetEntity
 
 from ._base import BaseExporter
 
 
 class ExcelExporter(BaseExporter[Workbook]):
     """Export rules to Excel.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 from rdflib import DCTERMS, OWL, RDF, RDFS, XSD, BNode, Graph, Literal, Namespace, URIRef
 from rdflib.collection import Collection as GraphCollection
 
 from cognite.neat.constants import DEFAULT_NAMESPACE as NEAT_NAMESPACE
 from cognite.neat.rules import exceptions
-from cognite.neat.rules._analysis._information_rules import InformationArchitectRulesAnalysis
-from cognite.neat.rules.models._rules import DMSRules
-from cognite.neat.rules.models._rules._types import XSD_VALUE_TYPE_MAPPINGS, EntityTypes
-from cognite.neat.rules.models._rules.information_rules import (
+from cognite.neat.rules.analysis import InformationArchitectRulesAnalysis
+from cognite.neat.rules.models.rules import DMSRules
+from cognite.neat.rules.models.rules._information_rules import (
     InformationClass,
     InformationMetadata,
     InformationProperty,
     InformationRules,
 )
+from cognite.neat.rules.models.rules._types import XSD_VALUE_TYPE_MAPPINGS, EntityTypes
 from cognite.neat.utils.utils import generate_exception_report, remove_namespace
 
 from ._base import BaseExporter
 from ._validation import are_properties_redefined
 
 if sys.version_info >= (3, 11):
     from typing import Self
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import warnings
 from pathlib import Path
 from typing import Literal, get_args
 
 import yaml
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules.base import RoleTypes
+from cognite.neat.rules.models.rules._base import RoleTypes
 
 from ._base import BaseExporter
 
 
 class YAMLExporter(BaseExporter[str]):
     """Export rules to YAML.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.75.1/cognite/neat/rules/exporters/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import warnings
 from typing import Literal, overload
 
 from cognite.neat.exceptions import wrangle_warnings
 from cognite.neat.rules import exceptions
-from cognite.neat.rules.models._rules import InformationRules
-from cognite.neat.rules.models._rules._types._base import DMS_PROPERTY_ID_COMPLIANCE_REGEX, VIEW_ID_COMPLIANCE_REGEX
+from cognite.neat.rules.models.rules import InformationRules
+from cognite.neat.rules.models.rules._types._base import DMS_PROPERTY_ID_COMPLIANCE_REGEX, VIEW_ID_COMPLIANCE_REGEX
 
 
 @overload
 def are_entity_names_dms_compliant(rules: InformationRules, return_report: Literal[True]) -> tuple[bool, list[dict]]:
     ...
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import getpass
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 import pandas as pd
 from pydantic_core import ErrorDetails
 
-from cognite.neat.rules.models.raw_rules import RawRules
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.raw_rules import RawRules
+from cognite.neat.legacy.rules.models.rules import Rules
 
 
 class BaseImporter(ABC):
     """
     BaseImporter class which all importers inherit from.
     """
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timezone
 from typing import Any, Literal
 
 import pandas as pd
 
-from cognite.neat.rules.models.tables import Tables
+from cognite.neat.legacy.rules.models.tables import Tables
 
 from ._base import BaseImporter
 
 
 class ArbitraryDictImporter(BaseImporter):
     """
     Importer for an arbitrary dictionary.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     EdgeConnection,
     MappedProperty,
     SingleHopConnectionDefinition,
     View,
 )
 from cognite.client.data_classes.data_modeling.ids import DataModelIdentifier, ViewId
 
-from cognite.neat.rules.models.tables import Tables
-from cognite.neat.rules.models.value_types import DMS_VALUE_TYPE_MAPPINGS, XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.legacy.rules.models.tables import Tables
+from cognite.neat.legacy.rules.models.value_types import DMS_VALUE_TYPE_MAPPINGS, XSD_VALUE_TYPE_MAPPINGS
 
 from ._base import BaseImporter
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from datetime import datetime
 from typing import cast
 
 import pandas as pd
 from rdflib import Graph, Literal, Namespace, URIRef
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.exporter._rules2rules import to_dms_name
-from cognite.neat.rules.importer._base import BaseImporter
-from cognite.neat.rules.models.tables import Tables
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.exporters._rules2rules import to_dms_name
+from cognite.neat.legacy.rules.models.tables import Tables
 from cognite.neat.utils.utils import get_namespace, remove_namespace, uri_to_short_form
 
+from ._base import BaseImporter
+
 
 class GraphImporter(BaseImporter):
     """
     Convert RDF graph, containing nodes and edges, to tables/ transformation rules / Excel file.
 
     Args:
         graph: RDF graph to be imported
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import re
 
 import pandas as pd
 from rdflib import Graph, Namespace
 
-from cognite.neat.rules.models.rules import (
+from cognite.neat.legacy.rules.models.rules import (
     cdf_space_compliance_regex,
     data_model_id_compliance_regex,
     prefix_compliance_regex,
     version_compliance_regex,
 )
 from cognite.neat.utils.utils import convert_rdflib_content, remove_none_elements_from_set
 
@@ -62,20 +62,24 @@
             "cdfSpaceName": results[3].pop(),
             "version": results[4].pop(),
             "isCurrentVersion": results[5].pop(),
             "created": results[6].pop(),
             "updated": results[7].pop(),
             "title": results[8].pop(),
             "description": results[9].pop(),
-            "creator": ", ".join(remove_none_elements_from_set(results[10]))
-            if remove_none_elements_from_set(results[10])
-            else None,
-            "contributor": ", ".join(remove_none_elements_from_set(results[11]))
-            if remove_none_elements_from_set(results[11])
-            else None,
+            "creator": (
+                ", ".join(remove_none_elements_from_set(results[10]))
+                if remove_none_elements_from_set(results[10])
+                else None
+            ),
+            "contributor": (
+                ", ".join(remove_none_elements_from_set(results[11]))
+                if remove_none_elements_from_set(results[11])
+                else None
+            ),
             "rights": results[12].pop(),
             "license": results[13].pop(),
         }
     )
 
     if make_compliant:
         clean_list.pop("created")
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from pathlib import Path
 
 import pandas as pd
 from pydantic_core import ErrorDetails
 from rdflib import DC, DCTERMS, OWL, RDF, RDFS, SKOS, Graph
 
-from cognite.neat.rules.importer._base import BaseImporter
-from cognite.neat.rules.models.raw_rules import RawRules
-from cognite.neat.rules.models.rules import Rules
-from cognite.neat.rules.models.tables import Tables
-from cognite.neat.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.legacy.rules.importers._base import BaseImporter
+from cognite.neat.legacy.rules.models.raw_rules import RawRules
+from cognite.neat.legacy.rules.models.rules import Rules
+from cognite.neat.legacy.rules.models.tables import Tables
+from cognite.neat.legacy.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS
 
 from ._owl2classes import parse_owl_classes
 from ._owl2metadata import parse_owl_metadata
 from ._owl2properties import parse_owl_properties
 
 
 class OWLImporter(BaseImporter):
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """This module performs importing of graph to TransformationRules pydantic class.
 In more details, it traverses the graph and abstracts class and properties, basically
 generating a list of rules based on which nodes that form the graph are made.
 """
 
-
 from pathlib import Path
 
 import pandas as pd
 from openpyxl import Workbook, load_workbook
 
-from cognite.neat.rules.importer._base import BaseImporter
 from cognite.neat.utils.auxiliary import local_import
 
+from ._base import BaseImporter
+
 
 class ExcelImporter(BaseImporter):
     def __init__(self, filepath: Path):
         self.filepath = filepath
 
     def to_tables(self) -> dict[str, pd.DataFrame]:
         workbook: Workbook = load_workbook(self.filepath)
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Literal
 
 import yaml
 
-from cognite.neat.rules.importer._dict2rules import ArbitraryDictImporter
+from ._dict2rules import ArbitraryDictImporter
 
 
 class ArbitraryYAMLImporter(ArbitraryDictImporter):
     """
     Importer for data given in a YAML file or string.
 
     This importer infers the data model from the YAML string based on the shape of the data.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Literal, overload
 
 from pydantic import ValidationError
 from rdflib import Namespace
 
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.issues.base import IssueList, NeatValidationError, ValidationWarning
-from cognite.neat.rules.models._rules import DMSRules, InformationRules, RoleTypes
+from cognite.neat.rules.models.rules import DMSRules, InformationRules, RoleTypes
 
 
 class BaseImporter(ABC):
     """
     BaseImporter class which all importers inherit from.
     """
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from cognite.client.data_classes.data_modeling import DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
 from cognite.client.utils import ms_to_datetime
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.importers._base import BaseImporter, Rules
 from cognite.neat.rules.issues import IssueList
-from cognite.neat.rules.models._rules import DMSRules, DMSSchema, RoleTypes
-from cognite.neat.rules.models._rules._types import (
+from cognite.neat.rules.models.rules import DMSRules, DMSSchema, RoleTypes
+from cognite.neat.rules.models.rules._base import ExtensionCategory, SchemaCompleteness
+from cognite.neat.rules.models.rules._dms_architect_rules import (
+    DMSContainer,
+    DMSMetadata,
+    DMSProperty,
+    DMSView,
+    SheetList,
+)
+from cognite.neat.rules.models.rules._types import (
     ClassEntity,
     ContainerEntity,
     DMSValueType,
     Undefined,
     Unknown,
     ViewEntity,
     ViewPropEntity,
 )
-from cognite.neat.rules.models._rules.base import ExtensionCategory, SchemaCompleteness
-from cognite.neat.rules.models._rules.dms_architect_rules import (
-    DMSContainer,
-    DMSMetadata,
-    DMSProperty,
-    DMSView,
-    SheetList,
-)
 
 
 class DMSImporter(BaseImporter):
     def __init__(self, schema: DMSSchema, metadata: DMSMetadata | None = None):
         self.schema = schema
         self.metadata = metadata
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     PropertyV2,
     Relationship,
     Schema,
     Telemetry,
     TelemetryV2,
 )
 from cognite.neat.rules.issues import IssueList, ValidationIssue
-from cognite.neat.rules.models._rules._types import (
+from cognite.neat.rules.models.rules._information_rules import InformationClass, InformationProperty
+from cognite.neat.rules.models.rules._types import (
     XSD_VALUE_TYPE_MAPPINGS,
     ClassEntity,
     ParentClassEntity,
     XSDValueType,
 )
-from cognite.neat.rules.models._rules.information_rules import InformationClass, InformationProperty
 
 
 class _DTDLConverter:
     def __init__(self, issues: list[ValidationIssue] | None = None) -> None:
         self.issues: IssueList = IssueList(issues or [])
         self.properties: list[InformationProperty] = []
         self.classes: list[InformationClass] = []
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from cognite.neat.rules import issues
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.importers._base import BaseImporter, _handle_issues
 from cognite.neat.rules.importers._dtdl2rules.dtdl_converter import _DTDLConverter
 from cognite.neat.rules.importers._dtdl2rules.spec import DTDL_CLS_BY_TYPE_BY_SPEC, DTDLBase, Interface
 from cognite.neat.rules.issues import IssueList, ValidationIssue
-from cognite.neat.rules.models._rules import InformationRules, RoleTypes
-from cognite.neat.rules.models._rules.base import SchemaCompleteness, SheetList
-from cognite.neat.rules.models._rules.information_rules import InformationClass, InformationProperty
+from cognite.neat.rules.models.rules import InformationRules, RoleTypes
+from cognite.neat.rules.models.rules._base import SchemaCompleteness, SheetList
+from cognite.neat.rules.models.rules._information_rules import InformationClass, InformationProperty
 from cognite.neat.utils.text import to_pascal
 
 
 class DTDLImporter(BaseImporter):
     """Importer for DTDL (Digital Twin Definition Language).
 
     This importer supports DTDL v2.0 and v3.0.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import re
 import warnings
 from abc import ABC
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, TypeAlias
 
 from pydantic import BaseModel, Field, field_validator, model_serializer, model_validator
 
-from cognite.neat.rules.models._rules._types import ClassEntity
+from cognite.neat.rules.models.rules._types import ClassEntity
 
 if TYPE_CHECKING:
     from pydantic.type_adapter import IncEx
 
 
 # Regex is from the spec: https://github.com/Azure/opendigitaltwins-dtdl/blob/master/DTMI/README.md#validation-regular-expressions
 _DTMI_REGEX = (
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import cast
 
 import numpy as np
 import pandas as pd
 from rdflib import OWL, Graph
 
-from cognite.neat.rules.models._rules.base import MatchType
+from cognite.neat.rules.models.rules._base import MatchType
 from cognite.neat.utils.utils import remove_namespace
 
 
 def parse_owl_classes(graph: Graph, make_compliant: bool = False, language: str = "en") -> list[dict]:
     """Parse owl classes from graph to pandas dataframe.
 
     Args:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import re
 
 from rdflib import Graph, Namespace
 
 from cognite.neat.constants import DEFAULT_NAMESPACE
-from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness
-from cognite.neat.rules.models.rules import (
-    prefix_compliance_regex,
-    version_compliance_regex,
+from cognite.neat.rules.models.rules._base import RoleTypes, SchemaCompleteness
+from cognite.neat.rules.models.rules._types._base import (
+    PREFIX_COMPLIANCE_REGEX,
+    VERSION_COMPLIANCE_REGEX,
 )
 from cognite.neat.utils.utils import convert_rdflib_content, remove_none_elements_from_set
 
 
 def parse_owl_metadata(graph: Graph, make_compliant: bool = False) -> dict:
     """Parse owl metadata from graph to dict.
 
@@ -144,15 +144,15 @@
     else:
         metadata["description"] = default
     return metadata
 
 
 def fix_prefix(metadata: dict, default: str = "neat") -> dict:
     if prefix := metadata.get("prefix", None):
-        if not isinstance(prefix, str) or not re.match(prefix_compliance_regex, prefix):
+        if not isinstance(prefix, str) or not re.match(PREFIX_COMPLIANCE_REGEX, prefix):
             metadata["prefix"] = default
     else:
         metadata["prefix"] = default
     return metadata
 
 
 def fix_namespace(metadata: dict, default: Namespace) -> dict:
@@ -189,15 +189,15 @@
         metadata[date_type] = default
 
     return metadata
 
 
 def fix_version(metadata: dict, default: str = "1.0.0") -> dict:
     if version := metadata.get("version", None):
-        if not re.match(version_compliance_regex, version):
+        if not re.match(VERSION_COMPLIANCE_REGEX, version):
             metadata["version"] = default
     else:
         metadata["version"] = default
 
     return metadata
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import cast
 
 import numpy as np
 import pandas as pd
 from rdflib import Graph
 
-from cognite.neat.rules.models._rules.base import MatchType
+from cognite.neat.rules.models.rules._base import MatchType
 from cognite.neat.utils.utils import remove_namespace
 
 from ._owl2classes import _data_type_property_class, _object_property_class, _thing_class
 
 
 def parse_owl_properties(graph: Graph, make_compliant: bool = False, language: str = "en") -> list[dict]:
     """Parse owl properties from graph to pandas dataframe.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from pathlib import Path
 from typing import Literal, overload
 
 from rdflib import DC, DCTERMS, OWL, RDF, RDFS, SKOS, Graph
 
 from cognite.neat.rules.importers._base import BaseImporter, Rules
 from cognite.neat.rules.issues import IssueList
-from cognite.neat.rules.models._rules import InformationRules, RoleTypes
-from cognite.neat.rules.models._rules._types import XSD_VALUE_TYPE_MAPPINGS
+from cognite.neat.rules.models.rules import InformationRules, RoleTypes
+from cognite.neat.rules.models.rules._types import XSD_VALUE_TYPE_MAPPINGS
 
 from ._owl2classes import parse_owl_classes
 from ._owl2metadata import parse_owl_metadata
 from ._owl2properties import parse_owl_properties
 
 
 class OWLImporter(BaseImporter):
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import Literal, cast, overload
 
 import pandas as pd
 from pandas import ExcelFile
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
-from cognite.neat.rules.models._rules import RULES_PER_ROLE, DMSRules, DomainRules, InformationRules
-from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness
+from cognite.neat.rules.models.rules import RULES_PER_ROLE, DMSRules, DomainRules, InformationRules
+from cognite.neat.rules.models.rules._base import RoleTypes, SchemaCompleteness
 from cognite.neat.utils.auxiliary import local_import
 from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_individual_sheet
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 SOURCE_SHEET__TARGET_FIELD__HEADERS = [
     ("Properties", "Properties", "Class"),
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any, Literal, overload
 
 import yaml
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList, NeatValidationError, ValidationIssue
-from cognite.neat.rules.models._rules import RULES_PER_ROLE, RoleTypes
+from cognite.neat.rules.models.rules import RULES_PER_ROLE, RoleTypes
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 
 class YAMLImporter(BaseImporter):
     """Imports the rules from a YAML file.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/base.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.75.1/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_base.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .base import RoleTypes
-from .dms_architect_rules import DMSRules
-from .dms_schema import DMSSchema
-from .domain_rules import DomainRules
-from .information_rules import InformationRules
+from ._base import RoleTypes
+from ._dms_architect_rules import DMSRules
+from ._dms_schema import DMSSchema
+from ._domain_rules import DomainRules
+from ._information_rules import InformationRules
 
 RULES_PER_ROLE: dict[RoleTypes, type[DomainRules] | type[InformationRules] | type[DMSRules]] = {
     RoleTypes.domain_expert: DomainRules,
     RoleTypes.information_architect: InformationRules,
     RoleTypes.dms_architect: DMSRules,
 }
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,49 @@
 import re
 import sys
-from functools import total_ordering
 from typing import Any, ClassVar, Literal, cast, overload
 
 from cognite.client.data_classes.data_modeling import ContainerId, DataModelId, PropertyId, ViewId
-from pydantic import BaseModel
 
+from cognite.neat.rules.models._entity import (
+    ENTITY_ID_REGEX_COMPILED,
+    PREFIX_REGEX,
+    PROPERTY_REGEX,
+    SUFFIX_REGEX,
+    VERSION_REGEX,
+    VERSIONED_ENTITY_REGEX_COMPILED,
+    Entity,
+    EntityTypes,
+    Undefined,
+    Unknown,
+)
 from cognite.neat.rules.models.rdfpath import (
     SINGLE_PROPERTY_REGEX_COMPILED,
     AllReferences,
     RDFPath,
     SingleProperty,
     TransformationRuleType,
     parse_rule,
 )
 
 if sys.version_info >= (3, 11):
-    from enum import StrEnum
     from typing import Self
 else:
-    from backports.strenum import StrEnum
     from typing_extensions import Self
 
 
-class EntityTypes(StrEnum):
-    subject = "subject"
-    predicate = "predicate"
-    object = "object"
-    class_ = "class"
-    parent_class = "parent_class"
-    property_ = "property"
-    object_property = "ObjectProperty"
-    data_property = "DatatypeProperty"
-    annotation_property = "AnnotationProperty"
-    object_value_type = "object_value_type"
-    data_value_type = "data_value_type"  # these are strings, floats, ...
-    xsd_value_type = "xsd_value_type"
-    dms_value_type = "dms_value_type"
-    view = "view"
-    view_prop = "view_prop"
-    reference_entity = "reference_entity"
-    container = "container"
-    datamodel = "datamodel"
-    undefined = "undefined"
-
-
-# ALLOWED
-ALLOWED_PATTERN = r"[^a-zA-Z0-9-_.]"
-
-# FOR PARSING STRINGS:
-PREFIX_REGEX = r"[a-zA-Z]+[a-zA-Z0-9-_.]*[a-zA-Z0-9]+"
-SUFFIX_REGEX = r"[a-zA-Z0-9-_.]+[a-zA-Z0-9]|[-_.]*[a-zA-Z0-9]+"
-VERSION_REGEX = r"[a-zA-Z0-9]([.a-zA-Z0-9_-]{0,41}[a-zA-Z0-9])?"
-PROPERTY_REGEX = r"[a-zA-Z0-9][a-zA-Z0-9_-]*[a-zA-Z0-9]?"
-ENTITY_ID_REGEX = rf"{PREFIX_REGEX}:({SUFFIX_REGEX})"
-ENTITY_ID_REGEX_COMPILED = re.compile(rf"^(?P<prefix>{PREFIX_REGEX}):(?P<suffix>{SUFFIX_REGEX})$")
-VERSIONED_ENTITY_REGEX_COMPILED = re.compile(
-    rf"^(?P<prefix>{PREFIX_REGEX}):(?P<suffix>{SUFFIX_REGEX})\(version=(?P<version>{VERSION_REGEX})\)$"
-)
+VERSION_ID_REGEX = rf"\(version=(?P<version>{VERSION_REGEX})\)"
+
+
 PROPERTY_ENTITY_REGEX_COMPILED = re.compile(
     rf"^((?P<prefix>{PREFIX_REGEX}):)?(?P<suffix>{SUFFIX_REGEX})"
     rf"\((version=(?P<version>{VERSION_REGEX}), )?property=(?P<property>{PROPERTY_REGEX})\)$"
 )
-CLASS_ID_REGEX = rf"(?P<{EntityTypes.class_}>{ENTITY_ID_REGEX})"
-CLASS_ID_REGEX_COMPILED = re.compile(rf"^{CLASS_ID_REGEX}$")
-PROPERTY_ID_REGEX = rf"\((?P<{EntityTypes.property_}>{ENTITY_ID_REGEX})\)"
-VERSION_ID_REGEX = rf"\(version=(?P<version>{VERSION_REGEX})\)"
+
+
 MORE_THAN_ONE_NONE_ALPHANUMERIC_REGEX = r"([_-]{2,})"
 PREFIX_COMPLIANCE_REGEX = r"^([a-zA-Z]+)([a-zA-Z0-9]*[_-]{0,1}[a-zA-Z0-9_-]*)([a-zA-Z0-9]*)$"
 DATA_MODEL_ID_COMPLIANCE_REGEX = r"^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$"
 CDF_SPACE_COMPLIANCE_REGEX = (
     r"(?!^(space|cdf|dms|pg3|shared|system|node|edge)$)(^[a-zA-Z][a-zA-Z0-9_-]{0,41}[a-zA-Z0-9]?$)"
 )
 VIEW_ID_COMPLIANCE_REGEX = (
@@ -83,104 +57,14 @@
     r"(^[a-zA-Z][a-zA-Z0-9_]{0,253}[a-zA-Z0-9]?$)"
 )
 CLASS_ID_COMPLIANCE_REGEX = r"(?!^(Class|class)$)(^[a-zA-Z][a-zA-Z0-9._-]{0,253}[a-zA-Z0-9]?$)"
 PROPERTY_ID_COMPLIANCE_REGEX = r"^(\*)|(?!^(Property|property)$)(^[a-zA-Z][a-zA-Z0-9._-]{0,253}[a-zA-Z0-9]?$)"
 VERSION_COMPLIANCE_REGEX = r"^[a-zA-Z0-9]([.a-zA-Z0-9_-]{0,41}[a-zA-Z0-9])?$"
 
 
-Undefined = type(object())
-Unknown = type(object())
-
-
-# mypy does not like the sentinel value, and it is not possible to ignore only the line with it below.
-# so we ignore all errors beyond this point.
-# mypy: ignore-errors
-@total_ordering
-class Entity(BaseModel, arbitrary_types_allowed=True):
-    """Entity is a class or property in OWL/RDF sense."""
-
-    type_: ClassVar[EntityTypes] = EntityTypes.undefined
-    prefix: str | Undefined = Undefined
-    suffix: str | Unknown
-    version: str | None = None
-    name: str | None = None
-    description: str | None = None
-
-    def __lt__(self, other: object) -> bool:
-        if type(self) is not type(other) or not isinstance(other, Entity):
-            return NotImplemented
-        return self.versioned_id < other.versioned_id
-
-    def __eq__(self, other: object) -> bool:
-        if type(self) is not type(other) or not isinstance(other, Entity):
-            return NotImplemented
-        return self.versioned_id == other.versioned_id
-
-    def __hash__(self) -> int:
-        return hash(self.versioned_id)
-
-    def as_non_versioned_entity(self) -> Self:
-        return self.from_string(f"{self.prefix}:{self.suffix}")
-
-    @property
-    def id(self) -> str:
-        if self.suffix is Unknown:
-            return "#N/A"
-        elif self.prefix is Undefined:
-            return self.suffix
-        else:
-            return f"{self.prefix}:{self.suffix}"
-
-    @property
-    def versioned_id(self) -> str:
-        if self.version is None:
-            return self.id
-        else:
-            return f"{self.id}(version={self.version})"
-
-    @property
-    def space(self) -> str:
-        """Returns entity space in CDF."""
-        return self.prefix
-
-    @property
-    def external_id(self) -> str:
-        """Returns entity external id in CDF."""
-        return self.suffix
-
-    def __repr__(self):
-        return self.versioned_id
-
-    def __str__(self):
-        return self.versioned_id
-
-    @classmethod
-    def from_string(cls, entity_string: str, base_prefix: str | None = None) -> Self:
-        if entity_string == "#N/A":
-            return cls(prefix=Undefined, suffix=Unknown)
-        elif result := VERSIONED_ENTITY_REGEX_COMPILED.match(entity_string):
-            return cls(
-                prefix=result.group("prefix"),
-                suffix=result.group("suffix"),
-                version=result.group("version"),
-            )
-        elif result := ENTITY_ID_REGEX_COMPILED.match(entity_string):
-            return cls(prefix=result.group("prefix"), suffix=result.group("suffix"))
-        elif base_prefix and re.match(SUFFIX_REGEX, entity_string) and re.match(PREFIX_REGEX, base_prefix):
-            return cls(prefix=base_prefix, suffix=entity_string)
-        else:
-            raise ValueError(f"{cls.__name__} is expected to be prefix:suffix, got {entity_string}")
-
-    @classmethod
-    def from_list(cls, entity_strings: list[str], base_prefix: str | None = None) -> list[Self]:
-        return [
-            cls.from_string(entity_string=entity_string, base_prefix=base_prefix) for entity_string in entity_strings
-        ]
-
-
 class ContainerEntity(Entity):
     type_: ClassVar[EntityTypes] = EntityTypes.container
 
     @classmethod
     def from_raw(cls, value: Any) -> "ContainerEntity":
         if not value:
             return ContainerEntity(prefix=Undefined, suffix=value)
@@ -289,15 +173,15 @@
             return cls(prefix=Undefined, suffix=value)
 
     @classmethod
     def from_prop_id(cls, prop_id: PropertyId) -> "ViewPropEntity":
         return ViewPropEntity(
             prefix=prop_id.source.space,
             suffix=prop_id.source.external_id,
-            version=prop_id.source.version,
+            version=cast(ViewId, prop_id.source).version,
             property_=prop_id.property,
         )
 
     def as_prop_id(self, default_space: str | None = None, default_version: str | None = None) -> PropertyId:
         if self.property_ is None:
             raise ValueError("property is required to create PropertyId")
         return PropertyId(source=self.as_id(False, default_space, default_version), property=self.property_)
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     constr,
     field_validator,
     model_serializer,
     model_validator,
 )
 from pydantic.fields import FieldInfo
 
-from cognite.neat.rules.models._rules._types import ClassType
+from cognite.neat.rules.models.rules._types import ClassType
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
     from typing_extensions import Self
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 from cognite.client.data_classes.data_modeling.views import SingleReverseDirectRelationApply, ViewPropertyApply
 from pydantic import Field, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo, ValidationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.rules import issues
-from cognite.neat.rules.models._rules.domain_rules import DomainRules
+from cognite.neat.rules.models.rules._domain_rules import DomainRules
 
+from ._base import BaseMetadata, BaseRules, ExtensionCategory, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
+from ._dms_schema import DMSSchema, PipelineSchema
 from ._types import (
     CdfValueType,
     ClassEntity,
     ContainerEntity,
     ContainerListType,
     ContainerType,
     DMSValueType,
@@ -36,19 +38,17 @@
     VersionType,
     ViewEntity,
     ViewListType,
     ViewPropEntity,
     ViewType,
     XSDValueType,
 )
-from .base import BaseMetadata, BaseRules, ExtensionCategory, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
-from .dms_schema import DMSSchema, PipelineSchema
 
 if TYPE_CHECKING:
-    from .information_rules import InformationRules
+    from ._information_rules import InformationRules
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
@@ -1059,15 +1059,15 @@
     def as_information_architect_rules(
         self,
         created: datetime | None = None,
         updated: datetime | None = None,
         name: str | None = None,
         namespace: Namespace | None = None,
     ) -> "InformationRules":
-        from .information_rules import InformationClass, InformationMetadata, InformationProperty, InformationRules
+        from ._information_rules import InformationClass, InformationMetadata, InformationProperty, InformationRules
 
         dms = self.dms.metadata
         prefix = dms.space
 
         metadata = InformationMetadata(
             schema_=dms.schema_,
             prefix=prefix,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     MissingContainerPropertyError,
     MissingEdgeViewError,
     MissingParentViewError,
     MissingSourceViewError,
     MissingSpaceError,
     MissingViewError,
 )
-from cognite.neat.rules.models._rules._types._value import DMS_VALUE_TYPE_MAPPINGS
+from cognite.neat.rules.models.rules._types._value import DMS_VALUE_TYPE_MAPPINGS
 from cognite.neat.utils.cdf_loaders import ViewLoader
 from cognite.neat.utils.cdf_loaders.data_classes import RawTableWrite, RawTableWriteList
 from cognite.neat.utils.text import to_camel
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import math
 from typing import Any, ClassVar
 
 from pydantic import Field, field_serializer, field_validator, model_serializer
 from pydantic_core.core_schema import SerializationInfo
 
-from ._types import ParentClassType, PropertyType, SemanticValueType, StrOrListType
-from .base import (
+from ._base import (
     BaseMetadata,
     RoleTypes,
     RuleModel,
     SheetEntity,
     SheetList,
 )
+from ._types import ParentClassType, PropertyType, SemanticValueType, StrOrListType
 
 
 class DomainMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.domain_expert
     creator: StrOrListType
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.75.1/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,26 @@
     SingleProperty,
     SPARQLQuery,
     TransformationRuleType,
     Traversal,
     parse_rule,
 )
 
+from ._base import (
+    BaseMetadata,
+    ExtensionCategory,
+    ExtensionCategoryType,
+    MatchType,
+    RoleTypes,
+    RuleModel,
+    SchemaCompleteness,
+    SheetEntity,
+    SheetList,
+)
+from ._domain_rules import DomainRules
 from ._types import (
     ClassEntity,
     ContainerEntity,
     Entity,
     EntityTypes,
     NamespaceType,
     ParentClassEntity,
@@ -41,29 +53,17 @@
     Undefined,
     VersionType,
     ViewEntity,
     ViewPropEntity,
     XSDValueType,
 )
 from ._types._base import Unknown
-from .base import (
-    BaseMetadata,
-    ExtensionCategory,
-    ExtensionCategoryType,
-    MatchType,
-    RoleTypes,
-    RuleModel,
-    SchemaCompleteness,
-    SheetEntity,
-    SheetList,
-)
-from .domain_rules import DomainRules
 
 if TYPE_CHECKING:
-    from .dms_architect_rules import DMSProperty, DMSRules
+    from ._dms_architect_rules import DMSProperty, DMSRules
 
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
@@ -376,15 +376,15 @@
     def __init__(self, information: InformationRules):
         self.information = information
 
     def as_domain_rules(self) -> DomainRules:
         raise NotImplementedError("DomainRules not implemented yet")
 
     def as_dms_architect_rules(self, created: datetime | None = None, updated: datetime | None = None) -> "DMSRules":
-        from .dms_architect_rules import DMSContainer, DMSMetadata, DMSProperty, DMSRules, DMSView
+        from ._dms_architect_rules import DMSContainer, DMSMetadata, DMSProperty, DMSRules, DMSView
 
         info_metadata = self.information.metadata
 
         space = self._to_space(info_metadata.prefix)
 
         metadata = DMSMetadata(
             schema_=info_metadata.schema_,
@@ -454,15 +454,15 @@
             is_reference=self.information.is_reference,
         )
 
     @classmethod
     def _as_dms_property(cls, prop: InformationProperty) -> "DMSProperty":
         """This creates the first"""
 
-        from .dms_architect_rules import DMSProperty
+        from ._dms_architect_rules import DMSProperty
 
         # returns property type, which can be ObjectProperty or DatatypeProperty
         if isinstance(prop.value_type, XSDValueType):
             value_type = cast(XSDValueType, prop.value_type).dms._type.casefold()  # type: ignore[attr-defined]
         elif isinstance(prop.value_type, ClassEntity):
             value_type = ViewPropEntity(
                 prefix=prop.value_type.prefix, suffix=prop.value_type.suffix, version=prop.value_type.version
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from pydantic import field_validator
 from pydantic_core import ErrorDetails, ValidationError
 from rdflib import Namespace
 
 from cognite.neat.constants import PREFIXES
 from cognite.neat.exceptions import wrangle_warnings
 
+# rules model and model components:
+from cognite.neat.legacy.rules.models.rules import Class, Metadata, Property, RuleModel, Rules
+from cognite.neat.legacy.rules.models.tables import Tables
+
 # importers:
 from cognite.neat.rules import exceptions
-
-# rules model and model components:
-from cognite.neat.rules.models.rules import Class, Metadata, Property, RuleModel, Rules
-from cognite.neat.rules.models.tables import Tables
 from cognite.neat.utils.utils import generate_exception_report
 
 __all__ = ["RawRules"]
 
 
 class RawRules(RuleModel):
     """
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import sys
 from collections import Counter
 from typing import Literal
 
 from pydantic import BaseModel, field_validator
 
-from cognite.neat.rules import exceptions
+from cognite.neat.legacy.rules import exceptions
 
 from ._base import (
     CLASS_ID_REGEX,
     CLASS_ID_REGEX_COMPILED,
     ENTITY_ID_REGEX,
     PROPERTY_ID_REGEX,
     SUFFIX_REGEX,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/rules.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/models/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,34 +26,34 @@
     model_validator,
     validator,
 )
 from pydantic.fields import FieldInfo
 from rdflib import XSD, Literal, Namespace, URIRef
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.rules import exceptions
-from cognite.neat.rules.models._base import (
+from cognite.neat.legacy.rules import exceptions
+from cognite.neat.legacy.rules.models._base import (
     ENTITY_ID_REGEX_COMPILED,
     VERSIONED_ENTITY_REGEX_COMPILED,
     ContainerEntity,
     EntityTypes,
     ParentClass,
 )
-from cognite.neat.rules.models.rdfpath import (
+from cognite.neat.legacy.rules.models.rdfpath import (
     AllReferences,
     Entity,
     Hop,
     RawLookup,
     SingleProperty,
     SPARQLQuery,
     TransformationRuleType,
     Traversal,
     parse_rule,
 )
-from cognite.neat.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS, ValueType
+from cognite.neat.legacy.rules.models.value_types import XSD_VALUE_TYPE_MAPPINGS, ValueType
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 __all__ = [
```

### Comparing `cognite_neat-0.74.0/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.75.1/cognite/neat/legacy/rules/models/value_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     SequenceReference,
     Text,
     TimeSeriesReference,
     Timestamp,
 )
 from pydantic import BaseModel
 
-from cognite.neat.rules.models._base import Entity, EntityTypes
+from cognite.neat.legacy.rules.models._base import Entity, EntityTypes
 
 
 class ValueTypeMapping(BaseModel):
     """Mapping between XSD, Python, DMS and Graphql types."""
 
     xsd: str
     python: type
```

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/cdf.py` & `cognite_neat-0.75.1/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.75.1/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/exceptions.py` & `cognite_neat-0.75.1/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.75.1/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/text.py` & `cognite_neat-0.75.1/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/utils.py` & `cognite_neat-0.75.1/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/utils/xml.py` & `cognite_neat-0.75.1/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.75.1/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/base.py` & `cognite_neat-0.75.1/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.75.1/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.75.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/manager.py` & `cognite_neat-0.75.1/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.75.1/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.75.1/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/model.py` & `cognite_neat-0.75.1/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/data_contracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetUpdate, Relationship, RelationshipUpdate
 from cognite.client.data_classes.data_modeling import EdgeApply, NodeApply
 
-from cognite.neat.graph.stores import NeatGraphStoreBase
-from cognite.neat.rules.exporter._rules2dms import DMSSchemaComponents
-from cognite.neat.rules.models._rules import DMSRules, DomainRules, InformationRules
-from cognite.neat.rules.models.rules import Rules
+from cognite.neat.legacy.graph.stores import NeatGraphStoreBase
+from cognite.neat.legacy.rules.exporters._rules2dms import DMSSchemaComponents
+from cognite.neat.legacy.rules.models.rules import Rules
+from cognite.neat.rules.models.rules import DMSRules, DomainRules, InformationRules
 from cognite.neat.workflows.steps.step_model import DataContract
 
 
 class RulesData(DataContract):
     """
     This represents the TransformationRules object.
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from pathlib import Path
 from typing import ClassVar, cast
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.graph import stores
+from cognite.neat.legacy.graph import stores
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = ["GraphStoreConfiguration", "GraphStoreReset"]
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from pathlib import Path
 from typing import ClassVar, Literal, cast
 
 from cognite.neat.rules import exporters
 from cognite.neat.rules._shared import DMSRules, InformationRules, Rules
-from cognite.neat.rules.models._rules import RoleTypes
+from cognite.neat.rules.models.rules import RoleTypes
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import CogniteClient, MultiRuleData
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = [
     "RulesToDMS",
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import ClassVar
 
 from cognite.client import CogniteClient
 
 from cognite.neat.rules import importers
 from cognite.neat.rules.issues.formatters import FORMATTER_BY_NAME
-from cognite.neat.rules.models._rules import RoleTypes
-from cognite.neat.rules.models._rules._types import DataModelEntity, Undefined
+from cognite.neat.rules.models.rules import RoleTypes
+from cognite.neat.rules.models.rules._types import DataModelEntity, Undefined
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import MultiRuleData
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title()
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import ClassVar
 
 from cognite.client import CogniteClient
 
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.issues.dms import MissingContainerError, MissingSpaceError, MissingViewError
 from cognite.neat.rules.issues.formatters import FORMATTER_BY_NAME
-from cognite.neat.rules.models._rules import DMSRules
-from cognite.neat.rules.models._rules.base import SchemaCompleteness
+from cognite.neat.rules.models.rules import DMSRules
+from cognite.neat.rules.models.rules._base import SchemaCompleteness
 from cognite.neat.utils import cdf_loaders
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import MultiRuleData
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title()
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import ClassVar, cast
 
-from cognite.neat.graph.transformation.entity_matcher import simple_entity_matcher
+from cognite.neat.legacy.graph.transformations.entity_matcher import simple_entity_matcher
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.steps.data_contracts import SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = ["SimpleGraphEntityMatcher"]
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title() + " [VERSION 1]"
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 from typing import ClassVar, cast
 
 from rdflib import RDF, XSD, Literal, Namespace, URIRef
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.graph import extractor
-from cognite.neat.graph.extractor._mock_graph_generator import generate_triples as generate_mock_triples
-from cognite.neat.rules.exporter._rules2triples import get_instances_as_triples
+from cognite.neat.legacy.graph import extractors
+from cognite.neat.legacy.graph.extractors._mock_graph_generator import generate_triples as generate_mock_triples
+from cognite.neat.legacy.rules.exporters._rules2triples import get_instances_as_triples
 from cognite.neat.utils.utils import create_sha256_hash
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = [
@@ -110,15 +110,15 @@
         if self.configs is None or self.data_store_path is None:
             raise StepNotInitialized(type(self).__name__)
 
         file_path = self.configs.get("file_path")
         base_namespace = self.configs.get("base_namespace", None)
 
         if file_path:
-            triples = extractor.DexpiXML(self.data_store_path / Path(file_path), base_namespace).extract()
+            triples = extractors.DexpiXML(self.data_store_path / Path(file_path), base_namespace).extract()
             source_graph.graph.add_triples(triples, verbose=True)
 
             logging.info(f"Loaded {file_path} into source graph.")
         else:
             raise ValueError("You need a source_rdf_store.file specified")
 
         return FlowMessage(output_text="Instances loaded to source graph")
@@ -158,15 +158,15 @@
             raise StepNotInitialized(type(self).__name__)
 
         file_path = self.configs.get("file_path")
 
         if file_path:
             logging.info(f"Processing graph capture sheet {self.data_store_path / Path(file_path)}")
 
-            triples = extractor.GraphCapturingSheet(
+            triples = extractors.GraphCapturingSheet(
                 rules=rules.rules,
                 filepath=self.data_store_path / Path(file_path),
                 namespace=self.configs.get("base_namespace", None),
                 use_source_ids=True,
             ).extract()
 
         else:
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from pathlib import Path
 from typing import Any, ClassVar, cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetFilter
 from prometheus_client import Gauge
 
-from cognite.neat.graph import loader as graph_loader
-from cognite.neat.graph.loader import upload_labels
-from cognite.neat.graph.loader.core.rdf_to_assets import (
+from cognite.neat.legacy.graph import loaders as graph_loader
+from cognite.neat.legacy.graph.loaders import upload_labels
+from cognite.neat.legacy.graph.loaders.core.rdf_to_assets import (
     NeatMetadataKeys,
     categorize_assets,
     rdf2assets,
     remove_non_existing_labels,
     unique_asset_labels,
     upload_assets,
 )
-from cognite.neat.graph.loader.core.rdf_to_relationships import (
+from cognite.neat.legacy.graph.loaders.core.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
-from cognite.neat.graph.loader.rdf_to_dms import upload_edges, upload_nodes
-from cognite.neat.graph.loader.validator import validate_asset_hierarchy
-from cognite.neat.rules.models.rdfpath import TransformationRuleType
+from cognite.neat.legacy.graph.loaders.rdf_to_dms import upload_edges, upload_nodes
+from cognite.neat.legacy.graph.loaders.validator import validate_asset_hierarchy
+from cognite.neat.legacy.rules.models.rdfpath import TransformationRuleType
 from cognite.neat.utils.utils import generate_exception_report
 from cognite.neat.workflows._exceptions import StepFlowContextNotInitialized, StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import (
     CategorizedAssets,
     CategorizedRelationships,
     Edges,
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from pathlib import Path
 from typing import ClassVar, cast
 
 from cognite.neat.constants import PREFIXES
-from cognite.neat.graph import stores
+from cognite.neat.legacy.graph import stores
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = ["ResetGraphStores", "ConfigureGraphStore"]
 
@@ -258,14 +258,20 @@
         new_graph_store = store_cls(prefixes=prefixes, base_prefix="neat", namespace=PREFIXES["neat"])
         new_graph_store.init_graph(
             self.configs["sparql_query_url"],
             self.configs["sparql_update_url"],
             "neat-tnt",
             internal_storage_dir=store_dir,
         )
+        logging.info(50 * "*")
+        logging.info(50 * "*")
+        logging.info(50 * "*")
+        logging.info(type(new_graph_store))
+        logging.info(50 * "*")
+        logging.info(50 * "*")
 
         return (
             FlowMessage(output_text="Graph store configured successfully"),
             SourceGraph(graph=new_graph_store) if graph_name == "SourceGraph" else SolutionGraph(graph=new_graph_store),
         )
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import ClassVar
 
 from cognite.client import CogniteClient
 
-from cognite.neat.graph.transformation.transformer import RuleProcessingReport, domain2app_knowledge_graph
-from cognite.neat.rules.exporter._rules2triples import get_instances_as_triples
+from cognite.neat.legacy.graph.transformations.transformer import RuleProcessingReport, domain2app_knowledge_graph
+from cognite.neat.legacy.rules.exporters._rules2triples import get_instances_as_triples
 from cognite.neat.workflows.model import FlowMessage
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = ["TransformSourceToSolutionGraph"]
 
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title() + " [VERSION 1]"
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import time
 import warnings
 from pathlib import Path
 from typing import ClassVar, Literal, cast
 
 from cognite.client import data_modeling as dm
 
-import cognite.neat.graph.extractor._graph_capturing_sheet
+import cognite.neat.legacy.graph.extractors._graph_capturing_sheet
 from cognite.neat.exceptions import wrangle_warnings
-from cognite.neat.rules import exporter
-from cognite.neat.rules.exporter._rules2dms import DMSSchemaComponents
-from cognite.neat.rules.exporter._rules2graphql import GraphQLSchema
-from cognite.neat.rules.exporter._rules2ontology import Ontology
+from cognite.neat.legacy.rules import exporters
+from cognite.neat.legacy.rules.exporters._rules2dms import DMSSchemaComponents
+from cognite.neat.legacy.rules.exporters._rules2graphql import GraphQLSchema
+from cognite.neat.legacy.rules.exporters._rules2ontology import Ontology
 from cognite.neat.utils.utils import generate_exception_report
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import CogniteClient, DMSSchemaComponentsData, RulesData
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 __all__ = [
@@ -481,15 +481,15 @@
         logging.info(f"Auto identifier type {auto_identifier_type}")
         staging_dir = self.data_store_path / Path(staging_dir_str)
 
         staging_dir.mkdir(parents=True, exist_ok=True)
 
         data_capture_sheet_path = staging_dir / sheet_name
 
-        cognite.neat.graph.extractor._graph_capturing_sheet.rules2graph_capturing_sheet(
+        cognite.neat.legacy.graph.extractors._graph_capturing_sheet.rules2graph_capturing_sheet(
             rules.rules, data_capture_sheet_path, auto_identifier_type=auto_identifier_type
         )
 
         output_text = (
             "Data capture sheet generated and can be downloaded here : "
             f'<a href="/data/{staging_dir_str}/{sheet_name}?{time.time()}" target="_blank">'
             f"{sheet_name}</a>"
@@ -505,9 +505,9 @@
         Configurable(
             name="output_file_path", value="rules/custom-rules.xlsx", label="File path to the generated Excel file"
         )
     ]
 
     def run(self, rules_data: RulesData) -> FlowMessage:  # type: ignore[override, syntax]
         full_path = Path(self.data_store_path) / Path(self.configs["output_file_path"])
-        exporter.ExcelExporter.from_rules(rules=rules_data.rules).export_to_file(filepath=full_path)
+        exporters.ExcelExporter.from_rules(rules=rules_data.rules).export_to_file(filepath=full_path)
         return FlowMessage(output_text="Generated Excel file from rules")
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from pathlib import Path
 from typing import ClassVar, cast
 
 import yaml
 from prometheus_client import Gauge
 from rdflib import Namespace
 
-from cognite.neat.rules import exporter, importer
-from cognite.neat.rules.models.rdfpath import TransformationRuleType
-from cognite.neat.rules.models.rules import Class, Classes, Metadata, Properties, Property, Rules
-from cognite.neat.rules.models.value_types import ValueType
+from cognite.neat.legacy.rules import exporters, importers
+from cognite.neat.legacy.rules.models.rdfpath import TransformationRuleType
+from cognite.neat.legacy.rules.models.rules import Class, Classes, Metadata, Properties, Property, Rules
+from cognite.neat.legacy.rules.models.value_types import ValueType
 from cognite.neat.utils.utils import generate_exception_report
 from cognite.neat.workflows import utils
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.cdf_store import CdfStore
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import RulesData, SolutionGraph, SourceGraph
 from cognite.neat.workflows.steps.step_model import Configurable, Step
@@ -89,15 +89,15 @@
         elif rules_file_path.exists() and version:
             hash = utils.get_file_hash(rules_file_path)
             if hash != version:
                 store.load_rules_file_from_cdf(str(rules_file), version)
         else:
             store.load_rules_file_from_cdf(str(rules_file), version)
 
-        raw_rules = importer.ExcelImporter(rules_file_path).to_raw_rules()
+        raw_rules = importers.ExcelImporter(rules_file_path).to_raw_rules()
         rules, errors, _ = raw_rules.to_rules(return_report=True, skip_validation=False)
         report = "# RULES VALIDATION REPORT\n\n" + generate_exception_report(errors, "Errors")
 
         report_full_path.write_text(report)
 
         text_for_report = (
             "<p></p>"
@@ -153,23 +153,23 @@
     def run(self) -> FlowMessage:  # type: ignore[override, syntax]
         ontology_file_path = self.data_store_path / Path(self.configs["ontology_file_path"])
         excel_file_path = self.data_store_path / Path(self.configs["excel_file_path"])
         report_file_path = excel_file_path.parent / f"report_{excel_file_path.stem}.txt"
 
         make_compliant = self.configs["make_compliant"] == "True"
         try:
-            rules = importer.OWLImporter(ontology_file_path).to_rules(make_compliant=make_compliant)
+            rules = importers.OWLImporter(ontology_file_path).to_rules(make_compliant=make_compliant)
         except Exception:
-            rules = importer.OWLImporter(ontology_file_path).to_rules(
+            rules = importers.OWLImporter(ontology_file_path).to_rules(
                 skip_validation=True, make_compliant=make_compliant
             )
         assert isinstance(rules, Rules)
-        exporter.ExcelExporter.from_rules(rules).export_to_file(excel_file_path)
+        exporters.ExcelExporter.from_rules(rules).export_to_file(excel_file_path)
 
-        if report := importer.ExcelImporter(filepath=excel_file_path).to_raw_rules().validate_rules():
+        if report := importers.ExcelImporter(filepath=excel_file_path).to_raw_rules().validate_rules():
             report_file_path.write_text(report)
 
         relative_excel_file_path = str(excel_file_path).split("/data/")[1]
         relative_report_file_path = str(report_file_path).split("/data/")[1]
 
         output_text = (
             "<p></p>"
@@ -577,26 +577,26 @@
     ]
 
     def run(self, graph_store: SourceGraph | SolutionGraph) -> FlowMessage:  # type: ignore[override, syntax]
         excel_file_path = self.data_store_path / Path(self.configs["excel_file_path"])
         report_file_path = excel_file_path.parent / f"report_{excel_file_path.stem}.txt"
 
         try:
-            rules = importer.GraphImporter(
+            rules = importers.GraphImporter(
                 graph_store.graph.graph, int(self.configs["max_number_of_instances"])
             ).to_rules()
         except Exception:
-            rules = importer.GraphImporter(
+            rules = importers.GraphImporter(
                 graph_store.graph.graph, int(self.configs["max_number_of_instances"])
             ).to_rules(skip_validation=True)
 
         assert isinstance(rules, Rules)
-        exporter.ExcelExporter.from_rules(rules).export_to_file(excel_file_path)
+        exporters.ExcelExporter.from_rules(rules).export_to_file(excel_file_path)
 
-        if report := importer.ExcelImporter(filepath=excel_file_path).to_raw_rules().validate_rules():
+        if report := importers.ExcelImporter(filepath=excel_file_path).to_raw_rules().validate_rules():
             report_file_path.write_text(report)
 
         relative_excel_file_path = str(excel_file_path).split("/data/")[1]
         relative_report_file_path = str(report_file_path).split("/data/")[1]
 
         output_text = (
             "<p></p>"
```

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.75.1/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/tasks.py` & `cognite_neat-0.75.1/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/cognite/neat/workflows/triggers.py` & `cognite_neat-0.75.1/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.74.0/pyproject.toml` & `cognite_neat-0.75.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.74.0"
+version = "0.75.1"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.74.0/PKG-INFO` & `cognite_neat-0.75.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.74.0
+Version: 0.75.1
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

