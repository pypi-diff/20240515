# Comparing `tmp/cognite_neat-0.77.1.tar.gz` & `tmp/cognite_neat-0.77.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.77.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.77.2.tar", max compression
```

## Comparing `cognite_neat-0.77.1.tar` & `cognite_neat-0.77.2.tar`

### file list

```diff
@@ -1,278 +1,278 @@
--rw-r--r--   0        0        0    11351 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/README.md
--rw-r--r--   0        0        0       61 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-14 14:34:35.464744 cognite_neat-0.77.1/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-14 14:34:35.468744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-14 14:34:35.476744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-14 14:34:35.476744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-14 14:34:35.500744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-14 14:34:35.500744 cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-14 14:34:35.508744 cognite_neat-0.77.1/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-14 14:34:35.512744 cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-14 14:34:35.516744 cognite_neat-0.77.1/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-14 14:34:35.520744 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-14 14:34:35.524745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19584 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13688 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    14934 2024-05-14 14:34:35.528745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    18274 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6717 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7591 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7786 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7437 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6925 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11882 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    22035 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    12288 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13936 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    10876 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5706 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    18903 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    15568 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13620 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    41973 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6668 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    14141 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2993 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16395 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      195 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0     7964 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    15546 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0     7157 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0     5831 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_classes.py
--rw-r--r--   0        0        0      483 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-14 14:34:35.532745 cognite_neat-0.77.1/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22898 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10338 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4844 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-14 14:34:35.536745 cognite_neat-0.77.1/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4591 2024-05-14 14:34:35.928751 cognite_neat-0.77.1/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/README.md
+-rw-r--r--   0        0        0       61 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.738420 cognite_neat-0.77.2/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-14 16:50:45.742420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-14 16:50:45.750420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-14 16:50:45.750420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-14 16:50:45.774420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-14 16:50:45.774420 cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-14 16:50:45.782420 cognite_neat-0.77.2/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-14 16:50:45.782420 cognite_neat-0.77.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-14 16:50:45.782420 cognite_neat-0.77.2/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-14 16:50:45.782420 cognite_neat-0.77.2/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-14 16:50:45.786420 cognite_neat-0.77.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-14 16:50:45.790420 cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-14 16:50:45.794420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-14 16:50:45.798420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19584 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13688 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14934 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20120 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    18274 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6717 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7591 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7786 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7437 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6925 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11882 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    22893 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12288 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13936 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    10876 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-05-14 16:50:45.802420 cognite_neat-0.77.2/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5706 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    18903 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    15568 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13633 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    41973 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6668 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    14589 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2993 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    16395 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      195 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0     7964 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    15546 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0     7157 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0     5831 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_classes.py
+-rw-r--r--   0        0        0      483 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    22898 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    10338 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4844 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-14 16:50:45.806420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-14 16:50:45.810420 cognite_neat-0.77.2/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4591 2024-05-14 16:50:46.194415 cognite_neat-0.77.2/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.2/PKG-INFO
```

### Comparing `cognite_neat-0.77.1/LICENSE` & `cognite_neat-0.77.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/README.md` & `cognite_neat-0.77.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/configuration.py` & `cognite_neat-0.77.2/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.77.2/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/explorer.py` & `cognite_neat-0.77.2/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.77.2/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.77.2/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.77.2/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.77.2/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.77.2/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.77.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/config.py` & `cognite_neat-0.77.2/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/constants.py` & `cognite_neat-0.77.2/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.2/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.2/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.77.2/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.77.2/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.77.2/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.77.2/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.77.2/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/base.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/dms.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,34 @@
         output = super().dump()
         output["view_id"] = self.view_id.dump()
         output["container_ids"] = [container_id.dump() for container_id in self.container_ids]
         return output
 
 
 @dataclass(frozen=True)
+class RawFilterAppliedToViewWarning(DMSSchemaWarning):
+    description = "Raw filter is applied to a view, which is against the neat data modeling lifecycle."
+    fix = "Do not use raw filter, instead use HasData filter or nodeType filter or change the data model design."
+    error_name: ClassVar[str] = "RawFilterAppliedToView"
+    view_id: dm.ViewId
+
+    def message(self) -> str:
+        return (
+            f"RawFilter applied to the view {self.view_id}."
+            " The usage of RawFilter is against the neat team recommendations and the neat data modeling lifecycle."
+            " When opting for raw filter, the user is responsible for any errors that arise in neat."
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["view_id"] = self.view_id.dump()
+        return output
+
+
+@dataclass(frozen=True)
 class NodeTypeFilterOnParentViewWarning(DMSSchemaWarning):
     description = (
         "Setting a node type filter on a parent view. This is not "
         "recommended as parent views are typically used for multiple type of nodes."
     )
     fix = "Use a HasData filter instead"
     error_name: ClassVar[str] = "NodeTypeFilterOnParentViewWarning"
```

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.77.2/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/_base.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 class DMSViewInput:
     view: str
     class_: str | None = None
     name: str | None = None
     description: str | None = None
     implements: str | None = None
     reference: str | None = None
-    filter_: Literal["hasData", "nodeType"] | None = None
+    filter_: Literal["hasData", "nodeType", "rawFilter"] | None = None
     in_model: bool = True
 
     @classmethod
     @overload
     def load(cls, data: None) -> None: ...
 
     @classmethod
```

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/dms/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cognite.client import data_modeling as dm
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models._base import ExtensionCategory, SchemaCompleteness
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.entities import ContainerEntity
+from cognite.neat.rules.models.wrapped_entities import RawFilter
 
 from ._rules import DMSProperty, DMSRules
 
 
 class DMSPostValidation:
     """This class does all the validation of the DMS rules that have dependencies between
     components."""
@@ -21,14 +22,15 @@
         self.metadata = rules.metadata
         self.properties = rules.properties
         self.containers = rules.containers
         self.views = rules.views
         self.issue_list = IssueList()
 
     def validate(self) -> IssueList:
+        self._validate_best_practices()
         self._consistent_container_properties()
         self._referenced_views_and_containers_are_existing()
         self._validate_extension()
         self._validate_schema()
         self._validate_performance()
         return self.issue_list
 
@@ -237,14 +239,23 @@
                     self.issue_list.append(
                         issues.dms.HasDataFilterAppliedToTooManyContainersWarning(
                             view_id=view_id,
                             container_ids=mapped_containers,
                         )
                     )
 
+    def _validate_best_practices(self) -> None:
+        for view in self.views:
+            if view.filter_ and isinstance(view.filter_, RawFilter):
+                self.issue_list.append(
+                    issues.dms.RawFilterAppliedToViewWarning(
+                        view_id=view.view.as_id(),
+                    )
+                )
+
     @staticmethod
     def _changed_attributes_and_properties(
         new_dumped: dict[str, Any], existing_dumped: dict[str, Any]
     ) -> tuple[list[str], list[str]]:
         """Helper method to find the changed attributes and properties between two containers or views."""
         new_attributes = {key: value for key, value in new_dumped.items() if key != "properties"}
         existing_attributes = {key: value for key, value in existing_dumped.items() if key != "properties"}
```

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/domain.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/domain.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/entities.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/information/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/information/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.77.2/cognite/neat/rules/models/wrapped_entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf_classes.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.77.2/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/exceptions.py` & `cognite_neat-0.77.2/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.77.2/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/text.py` & `cognite_neat-0.77.2/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/utils.py` & `cognite_neat-0.77.2/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/utils/xml.py` & `cognite_neat-0.77.2/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.77.2/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/base.py` & `cognite_neat-0.77.2/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.77.2/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/manager.py` & `cognite_neat-0.77.2/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.77.2/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.77.2/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/model.py` & `cognite_neat-0.77.2/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.77.2/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/tasks.py` & `cognite_neat-0.77.2/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/cognite/neat/workflows/triggers.py` & `cognite_neat-0.77.2/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.1/pyproject.toml` & `cognite_neat-0.77.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.77.1"
+version = "0.77.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.77.1/PKG-INFO` & `cognite_neat-0.77.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.77.1
+Version: 0.77.2
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

