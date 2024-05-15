# Comparing `tmp/aiida_workgraph-0.2.3.tar.gz` & `tmp/aiida_workgraph-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_workgraph-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_workgraph-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_workgraph-0.2.3.tar` & `aiida_workgraph-0.2.4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.3/LICENSE
--rw-r--r--   0        0        0     5175 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/README.md
--rw-r--r--   0        0        0      175 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/__init__.py
--rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/cli/__init__.py
--rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_graph.py
--rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_web.py
--rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_workgraph.py
--rw-r--r--   0        0        0     6587 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/cli/query_workgraph.py
--rw-r--r--   0        0        0     2342 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/collection.py
--rw-r--r--   0        0        0    16371 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/decorator.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/engine/__init__.py
--rw-r--r--   0        0        0    46841 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/engine/workgraph.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/executors/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/executors/builtin.py
--rw-r--r--   0        0        0      740 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/executors/qe.py
--rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/executors/test.py
--rw-r--r--   0        0        0     3313 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/node.py
--rw-r--r--   0        0        0      937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/nodes/__init__.py
--rw-r--r--   0        0        0     3957 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.3/aiida_workgraph/nodes/builtin.py
--rw-r--r--   0        0        0     5068 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/nodes/qe.py
--rw-r--r--   0        0        0     7233 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/nodes/test.py
--rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/orm/worktree.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/properties/__init__.py
--rw-r--r--   0        0        0     9603 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/properties/built_in.py
--rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/property.py
--rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/socket.py
--rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/sockets/__init__.py
--rw-r--r--   0        0        0     3628 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/sockets/built_in.py
--rw-r--r--   0        0        0     7824 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/utils/__init__.py
--rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/utils/analysis.py
--rw-r--r--   0        0        0     1754 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/utils/graph.py
--rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/README.md
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/api.py
--rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/daemon.py
--rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/datanode.py
--rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/utils.py
--rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/workgraph.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/backend/main.py
--rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/.gitignore
--rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/.rete-patch
--rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/README.md
--rw-r--r--   0        0        0      517 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-05-07 20:57:23.435997 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/favicon.ico
--rw-r--r--   0        0        0      654 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/index.html
--rw-r--r--   0        0        0      306 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/robots.txt
--rw-r--r--   0        0        0    18033 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
--rw-r--r--   0        0        0    46655 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
--rw-r--r--   0        0        0     4518 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
--rw-r--r--   0        0        0    10597 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
--rw-r--r--   0        0        0  3614868 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
--rw-r--r--   0        0        0     3456 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
--rw-r--r--   0        0        0 13934230 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
--rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/package-lock.json
--rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/package.json
--rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/index.html
--rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/robots.txt
--rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/App.css
--rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/App.js
--rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/AtomsItem.js
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Data.js
--rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNode.js
--rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
--rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
--rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
--rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Home.js
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Layout.css
--rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Layout.js
--rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/NodeDetails.js
--rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Settings.js
--rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
--rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
--rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
--rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
--rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
--rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
--rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
--rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
--rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
--rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/index.css
--rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/index.tsx
--rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/logo.svg
--rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/reportWebVitals.ts
--rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete.css
--rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization.ts
--rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
--rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
--rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
--rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
--rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/background.css
--rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
--rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/default.ts
--rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/index.ts
--rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/setupTests.ts
--rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/tsconfig.json
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/widget/.gitignore
--rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.3/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/widget/README.md
--rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/widget/__init__.py
--rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.3/aiida_workgraph/widget/js/default_rete.ts
--rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.3/aiida_workgraph/widget/js/widget.css
--rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.3/aiida_workgraph/widget/js/widget.tsx
--rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.3/aiida_workgraph/widget/package-lock.json
--rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.3/aiida_workgraph/widget/package.json
--rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/widget/pyproject.toml
--rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/__init__.py
--rw-r--r--   0        0        0      429 2024-05-07 20:57:15.636082 aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/static/widget.css
--rw-r--r--   0        0        0  1796776 2024-05-07 20:57:15.640082 aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/static/widget.js
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/utils.py
--rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.3/aiida_workgraph/widget/tsconfig.json
--rw-r--r--   0        0        0    14693 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.3/aiida_workgraph/workgraph.py
--rw-r--r--   0        0        0     2504 2024-05-07 20:56:57.580283 aiida_workgraph-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7214 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 13:46:15.010509 aiida_workgraph-0.2.4/aiida_workgraph/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_graph.py
+-rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_web.py
+-rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_workgraph.py
+-rw-r--r--   0        0        0     6587 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/query_workgraph.py
+-rw-r--r--   0        0        0     2342 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/collection.py
+-rw-r--r--   0        0        0    17099 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/engine/__init__.py
+-rw-r--r--   0        0        0    47604 2024-05-14 15:37:34.242235 aiida_workgraph-0.2.4/aiida_workgraph/engine/workgraph.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/executors/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/executors/builtin.py
+-rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/executors/qe.py
+-rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/executors/test.py
+-rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/node.py
+-rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/nodes/builtin.py
+-rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/nodes/qe.py
+-rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/nodes/test.py
+-rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/orm/worktree.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/properties/__init__.py
+-rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/properties/built_in.py
+-rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/property.py
+-rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/socket.py
+-rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/sockets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/sockets/built_in.py
+-rw-r--r--   0        0        0     7824 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/utils/__init__.py
+-rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/utils/analysis.py
+-rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/utils/graph.py
+-rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/api.py
+-rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/daemon.py
+-rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/datanode.py
+-rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/utils.py
+-rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/workgraph.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/main.py
+-rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/.gitignore
+-rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/.rete-patch
+-rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/README.md
+-rw-r--r--   0        0        0      517 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-07 20:57:23.435997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/favicon.ico
+-rw-r--r--   0        0        0      654 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/index.html
+-rw-r--r--   0        0        0      306 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/robots.txt
+-rw-r--r--   0        0        0    18033 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
+-rw-r--r--   0        0        0    46655 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
+-rw-r--r--   0        0        0     4518 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
+-rw-r--r--   0        0        0  3614868 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
+-rw-r--r--   0        0        0     3456 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
+-rw-r--r--   0        0        0 13934230 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
+-rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package-lock.json
+-rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package.json
+-rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/index.html
+-rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/robots.txt
+-rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.css
+-rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.js
+-rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/AtomsItem.js
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Data.js
+-rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNode.js
+-rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
+-rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
+-rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
+-rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Home.js
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.css
+-rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.js
+-rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/NodeDetails.js
+-rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Settings.js
+-rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
+-rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
+-rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
+-rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
+-rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
+-rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
+-rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
+-rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
+-rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
+-rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.css
+-rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.tsx
+-rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/reportWebVitals.ts
+-rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete.css
+-rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization.ts
+-rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
+-rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
+-rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
+-rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
+-rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/background.css
+-rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
+-rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/default.ts
+-rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/index.ts
+-rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/tsconfig.json
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/.gitignore
+-rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.4/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/README.md
+-rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/__init__.py
+-rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/default_rete.ts
+-rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.css
+-rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.tsx
+-rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.4/aiida_workgraph/widget/package-lock.json
+-rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.4/aiida_workgraph/widget/package.json
+-rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/pyproject.toml
+-rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-07 20:57:15.636082 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.css
+-rw-r--r--   0        0        0  1796776 2024-05-07 20:57:15.640082 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.js
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/utils.py
+-rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/tsconfig.json
+-rw-r--r--   0        0        0    14889 2024-05-13 04:17:07.626646 aiida_workgraph-0.2.4/aiida_workgraph/workgraph.py
+-rw-r--r--   0        0        0     2505 2024-05-15 13:45:46.436692 aiida_workgraph-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.4/PKG-INFO
```

### Comparing `aiida_workgraph-0.2.3/LICENSE` & `aiida_workgraph-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/README.md` & `aiida_workgraph-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # AiiDA-WorkGraph
 [![PyPI version](https://badge.fury.io/py/aiida-workgraph.svg)](https://badge.fury.io/py/aiida-workgraph)
 [![Unit test](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml)
+[![codecov](https://codecov.io/gh/superstar54/aiida-workgraph/branch/main/graph/badge.svg)](https://codecov.io/gh/superstar54/aiida-workgraph)
 [![Docs status](https://readthedocs.org/projects/aiida-workgraph/badge)](http://aiida-workgraph.readthedocs.io/)
 
 Provides the third workflow component: `WorkGraph`, to design flexible node-based workflows using AiiDA.
 
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-WorkGraph provides the third component: `WorkGraph`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_graph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_web.py` & `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_web.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/cli/cmd_workgraph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/cli/query_workgraph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/cli/query_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/collection.py` & `aiida_workgraph-0.2.4/aiida_workgraph/collection.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/decorator.py` & `aiida_workgraph-0.2.4/aiida_workgraph/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from typing import Any, Callable, Dict, List, Optional, Union, Tuple
 from aiida_workgraph.utils import get_executor
 from aiida.engine import calcfunction, workfunction, CalcJob, WorkChain
+from aiida import orm
 from aiida.orm.nodes.process.calculation.calcfunction import CalcFunctionNode
 from aiida.orm.nodes.process.workflow.workfunction import WorkFunctionNode
 from aiida.engine.processes.ports import PortNamespace
 from node_graph.decorator import create_node
 import cloudpickle as pickle
 from aiida_workgraph.node import Node
 
+node_types = {
+    CalcFunctionNode: "CALCFUNCTION",
+    WorkFunctionNode: "WORKFUNCTION",
+    CalcJob: "CALCJOB",
+    WorkChain: "WORKCHAIN",
+}
+
+aiida_socket_maping = {
+    orm.Int: "AiiDAInt",
+    orm.Float: "AiiDAFloat",
+    orm.Str: "AiiDAString",
+    orm.Bool: "AiiDABool",
+}
+
 
 def add_input_recursive(
     inputs: List[List[Union[str, Dict[str, Any]]]],
     port: PortNamespace,
     args: List,
     kwargs: List,
     prefix: Optional[str] = None,
@@ -38,29 +53,37 @@
             kwargs.append(port_name)
         for value in port.values():
             add_input_recursive(
                 inputs, value, args, kwargs, prefix=port_name, required=required
             )
     else:
         if port_name not in input_names:
-            inputs.append(["General", port_name])
+            # port.valid_type can be a single type or a tuple of types,
+            # we only support single type for now
+            if isinstance(port.valid_type, tuple) and len(port.valid_type) > 1:
+                socket_type = "General"
+            if isinstance(port.valid_type, tuple) and len(port.valid_type) == 1:
+                socket_type = aiida_socket_maping.get(port.valid_type[0], "General")
+            else:
+                socket_type = aiida_socket_maping.get(port.valid_type, "General")
+            inputs.append([socket_type, port_name])
         if required:
             args.append(port_name)
         else:
             kwargs.append(port_name)
     return inputs
 
 
 def add_output_recursive(
     outputs: List[List[Union[str, Dict[str, Any]]]],
     port: PortNamespace,
     prefix: Optional[str] = None,
     required: bool = True,
 ) -> List[List[Union[str, Dict[str, Any]]]]:
-    """Add input recursively."""
+    """Add output recursively."""
     if prefix is None:
         port_name = port.name
     else:
         port_name = f"{prefix}.{port.name}"
     required = port.required and required
     output_names = [output[1] for output in outputs]
     if isinstance(port, PortNamespace):
@@ -120,31 +143,28 @@
         and issubclass(executor, Node)
     ):
         return executor
     ndata = {}
     if inspect.isfunction(executor):
         # calcfunction and workfunction
         if getattr(executor, "node_class", False):
-            if executor.node_class is CalcFunctionNode:
-                ndata["node_type"] = "calcfunction"
-            elif executor.node_class is WorkFunctionNode:
-                ndata["node_type"] = "workfunction"
+            ndata["node_type"] = node_types.get(executor.node_class, "NORMAL")
             ndata["executor"] = executor
             return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
         else:
-            ndata["node_type"] = "normal"
+            ndata["node_type"] = "NORMAL"
             ndata["executor"] = executor
             return build_node_from_function(executor, inputs=inputs, outputs=outputs)
     else:
         if issubclass(executor, CalcJob):
-            ndata["node_type"] = "calcjob"
+            ndata["node_type"] = "CALCJOB"
             ndata["executor"] = executor
             return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
         elif issubclass(executor, WorkChain):
-            ndata["node_type"] = "workchain"
+            ndata["node_type"] = "WORKCHAIN"
             ndata["executor"] = executor
             return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
     raise ValueError("The executor is not supported.")
 
 
 def build_node_from_function(
     executor: Callable,
@@ -174,21 +194,24 @@
     args = []
     kwargs = []
     for _key, port in spec.inputs.ports.items():
         add_input_recursive(inputs, port, args, kwargs, required=port.required)
     for _key, port in spec.outputs.ports.items():
         add_output_recursive(outputs, port, required=port.required)
     if spec.inputs.dynamic:
-        name = (
-            executor.process_class._var_keyword
-            or executor.process_class._var_positional
-        )
+        if hasattr(executor.process_class, "_varargs"):
+            name = executor.process_class._varargs
+        else:
+            name = (
+                executor.process_class._var_keyword
+                or executor.process_class._var_positional
+            )
         ndata["var_kwargs"] = name
         inputs.append(["General", name, {"property": ["General", {"default": {}}]}])
-    if ndata["node_type"] in ["calcfunction", "workfunction"]:
+    if ndata["node_type"].upper() in ["CALCFUNCTION", "WORKFUNCTION"]:
         outputs = [["General", "result"]] if not outputs else outputs
     # print("kwargs: ", kwargs)
     # add built-in sockets
     outputs.append(["General", "_outputs"])
     outputs.append(["General", "_wait"])
     inputs.append(["General", "_wait", {"link_limit": 1e6}])
     ndata["node_class"] = Node
@@ -342,18 +365,15 @@
 
             if identifier is None:
                 identifier = func.__name__
 
             # Determine node_type based on AiiDA's node classes
             node_type = node_type
             if hasattr(func, "node_class"):
-                if func.node_class is CalcFunctionNode:
-                    node_type = "calcfunction"
-                elif func.node_class is WorkFunctionNode:
-                    node_type = "workfunction"
+                node_type = node_types.get(func.node_class, node_type)
             ndata = generate_ndata(
                 func,
                 identifier,
                 inputs or [],
                 outputs or [["General", "result"]],
                 properties or [],
                 catalog,
@@ -415,43 +435,43 @@
 
         return decorator
 
     @staticmethod
     def calcfunction(**kwargs: Any) -> Callable:
         def decorator(func):
             # First, apply the calcfunction decorator
-            calcfunc_decorated = calcfunction(func)
+            func_decorated = calcfunction(func)
             # Then, apply node decorator
             node_decorated = build_node_from_callable(
-                calcfunc_decorated,
+                func_decorated,
                 inputs=kwargs.get("inputs", []),
                 outputs=kwargs.get("outputs", []),
             )
             identifier = kwargs.get("identifier", None)
-            func.identifier = identifier if identifier else func.__name__
-            func.node = node_decorated
-            return func
+            func_decorated.identifier = identifier if identifier else func.__name__
+            func_decorated.node = node_decorated
+            return func_decorated
 
         return decorator
 
     @staticmethod
     def workfunction(**kwargs: Any) -> Callable:
         def decorator(func):
             # First, apply the workfunction decorator
-            calcfunc_decorated = workfunction(func)
+            func_decorated = workfunction(func)
             node_decorated = build_node_from_callable(
-                calcfunc_decorated,
+                func_decorated,
                 inputs=kwargs.get("inputs", []),
                 outputs=kwargs.get("outputs", []),
             )
             identifier = kwargs.get("identifier", None)
-            func.identifier = identifier if identifier else func.__name__
-            func.node = node_decorated
+            func_decorated.identifier = identifier if identifier else func.__name__
+            func_decorated.node = node_decorated
 
-            return func
+            return func_decorated
 
         return decorator
 
     # Making decorator_node accessible as 'node'
     node = decorator_node
 
     # Making decorator_graph_builder accessible as 'graph_builder'
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/engine/workgraph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/engine/workgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         result: t.Any = None
 
         try:
             self.continue_workgraph()
         except _PropagateReturn as exception:
             finished, result = True, exception.exit_code
         else:
-            finished = self.is_workgraph_finished()
+            finished, result = self.is_workgraph_finished()
 
         # If the workgraph is finished or the result is an ExitCode, we exit by returning
         if finished:
             if isinstance(result, ExitCode):
                 return result
             else:
                 return self.finalize()
@@ -469,38 +469,39 @@
 
     def set_node_result(self, node: t.Dict[str, t.Any]) -> None:
         name = node["name"]
         # print(f"set node result: {name}")
         if node.get("process"):
             # print(f"set node result: {name} process")
             state = node["process"].process_state.value.upper()
-            if state == "FINISHED":
+            if node["process"].is_finished_ok:
                 node["state"] = state
-                if node["metadata"]["node_type"] == "graph_builder":
+                if node["metadata"]["node_type"].upper() == "GRAPH_BUILDER":
                     # expose the outputs of workgraph
                     node["results"] = getattr(
                         node["process"].outputs, "group_outputs", None
                     )
                     # self.ctx.new_data[name] = outputs
-                elif node["metadata"]["node_type"] == "workgraph":
+                elif node["metadata"]["node_type"].upper() == "WORKGRAPH":
                     # expose the outputs of all the nodes in the workgraph
                     node["results"] = {}
                     outgoing = node["process"].base.links.get_outgoing()
                     for link in outgoing.all():
                         if isinstance(link.node, ProcessNode) and getattr(
                             link.node, "process_state", False
                         ):
                             node["results"][link.link_label] = link.node.outputs
                 else:
                     node["results"] = node["process"].outputs
                     # self.ctx.new_data[name] = node["results"]
                 self.ctx.nodes[name]["state"] = "FINISHED"
                 self.node_to_context(name)
                 self.report(f"Node: {name} finished.")
-            elif state == "EXCEPTED":
+            # all other states are considered as failed
+            else:
                 node["state"] = state
                 node["results"] = node["process"].outputs
                 # self.ctx.new_data[name] = node["results"]
                 self.ctx.nodes[name]["state"] = "FAILED"
                 # set child state to FAILED
                 self.set_node_state(self.ctx.connectivity["child_node"][name], "FAILED")
                 self.report(f"Node: {name} failed.")
@@ -556,49 +557,58 @@
             if ready and name not in exclude:
                 node_to_run.append(name)
         #
         self.report("nodes ready to run: {}".format(",".join(node_to_run)))
         self.run_nodes(node_to_run)
 
     def update_node_state(self, name: str) -> None:
-        """Update ndoe state if node is a Awaitable."""
+        """Update node state if node is a Awaitable."""
         print("update node state: ", name)
         node = self.ctx.nodes[name]
         if (
-            node["metadata"]["node_type"]
+            node["metadata"]["node_type"].upper()
             in [
-                "calcfunction",
-                "workfunction",
-                "calcjob",
-                "workchain",
-                "graph_builder",
-                "workgraph",
+                "CALCFUNCTION",
+                "WORKFUNCTION",
+                "CALCJOB",
+                "WORKCHAIN",
+                "GRAPH_BUILDER",
+                "WORKGRAPH",
             ]
             and node["state"] == "RUNNING"
         ):
             self.set_node_result(node)
 
     def is_workgraph_finished(self) -> bool:
         """Check if the workgraph is finished.
         For `while` workgraph, we need check its conditions"""
         is_finished = True
+        failed_nodes = []
         for name, node in self.ctx.nodes.items():
             # self.update_node_state(name)
             print("node: ", name, node["state"])
             if node["state"] in ["RUNNING", "CREATED", "READY"]:
                 is_finished = False
+            elif node["state"] == "FAILED":
+                failed_nodes.append(name)
         if is_finished:
             if self.ctx.workgraph["workgraph_type"].upper() == "WHILE":
                 should_run = self.check_while_conditions()
                 is_finished = not should_run
             if self.ctx.workgraph["workgraph_type"].upper() == "FOR":
                 should_run = self.check_for_conditions()
                 is_finished = not should_run
         print("is workgraph finished: ", is_finished)
-        return is_finished
+        if is_finished and len(failed_nodes) > 0:
+            message = f"WorkGraph finished, but nodes: {failed_nodes} failed."
+            self.report(message)
+            result = ExitCode(302, message)
+        else:
+            result = None
+        return is_finished, result
 
     def check_while_conditions(self) -> bool:
         """Check while conditions.
         Run all condition nodes and check if all the conditions are True.
         """
         print("Is a while workgraph")
         print(
@@ -660,19 +670,19 @@
             create_data_node,
             update_nested_dict_with_special_keys,
         )
 
         for name in names:
             print("-" * 60)
             node = self.ctx.nodes[name]
-            if node["metadata"]["node_type"] in [
-                "calcjob",
-                "workchain",
-                "graph_builder",
-                "workgraph",
+            if node["metadata"]["node_type"].upper() in [
+                "CALCJOB",
+                "WORKCHAIN",
+                "GRAPH_BUILDER",
+                "WORKGRAPH",
             ]:
                 if len(self._awaitables) > self.ctx.max_number_awaitables:
                     print(
                         MAX_NUMBER_AWAITABLES_MSG.format(
                             self.ctx.max_number_awaitables, name
                         )
                     )
@@ -689,41 +699,44 @@
             kwargs = update_nested_dict_with_special_keys(kwargs)
             # print("args: ", args)
             # print("kwargs: ", kwargs)
             # print("var_kwargs: ", var_kwargs)
             # kwargs["meta.label"] = name
             # output must be a Data type or a mapping of {string: Data}
             node["results"] = {}
-            if node["metadata"]["node_type"] == "node":
+            if node["metadata"]["node_type"].upper() == "NODE":
                 print("node  type: node.")
                 results = self.run_executor(executor, [], kwargs, var_args, var_kwargs)
                 node["process"] = results
                 node["results"] = {node["outputs"][0]["name"]: results}
                 self.ctx.input_nodes[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
                 self.node_to_context(name)
                 # ValueError: attempted to add an input link after the process node was already stored.
                 # self.node.base.links.add_incoming(results, "INPUT_WORK", name)
                 self.report(f"Node: {name} finished.")
                 if continue_workgraph:
                     self.continue_workgraph(names)
-            elif node["metadata"]["node_type"] == "data":
+            elif node["metadata"]["node_type"].upper() == "DATA":
                 print("node  type: data.")
                 for key in self.ctx.nodes[name]["metadata"]["args"]:
                     kwargs.pop(key, None)
                 results = create_data_node(executor, args, kwargs)
                 node["results"] = {node["outputs"][0]["name"]: results}
                 node["process"] = results
                 self.ctx.new_data[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
                 self.node_to_context(name)
                 self.report(f"Node: {name} finished.")
                 if continue_workgraph:
                     self.continue_workgraph(names)
-            elif node["metadata"]["node_type"] in ["calcfunction", "workfunction"]:
+            elif node["metadata"]["node_type"].upper() in [
+                "CALCFUNCTION",
+                "WORKFUNCTION",
+            ]:
                 print("node type: calcfunction/workfunction.")
                 kwargs.setdefault("metadata", {})
                 kwargs["metadata"].update({"call_link_label": name})
                 try:
                     # since aiida 2.5.0, we need to use args_dict to pass the args to the run_get_node
                     if var_kwargs is None:
                         results, process = run_get_node(executor, **kwargs)
@@ -750,38 +763,38 @@
                         self.ctx.connectivity["child_node"][name], "FAILED"
                     )
                     print(f"Node: {name} failed.")
                     self.report(f"Node: {name} failed.")
                 # exclude the current nodes from the next run
                 if continue_workgraph:
                     self.continue_workgraph(names)
-            elif node["metadata"]["node_type"] in ["calcjob", "workchain"]:
+            elif node["metadata"]["node_type"].upper() in ["CALCJOB", "WORKCHAIN"]:
                 # process = run_get_node(executor, *args, **kwargs)
                 print("node  type: calcjob/workchain.")
                 kwargs.setdefault("metadata", {})
                 kwargs["metadata"].update({"call_link_label": name})
                 # transfer the args to kwargs
                 process = self.submit(executor, **kwargs)
                 process.label = name
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
-            elif node["metadata"]["node_type"] in ["graph_builder"]:
+            elif node["metadata"]["node_type"].upper() in ["GRAPH_BUILDER"]:
                 print("node  type: graph_builder.")
                 wg = self.run_executor(executor, [], kwargs, var_args, var_kwargs)
                 wg.name = name
                 wg.group_outputs = self.ctx.nodes[name]["metadata"]["group_outputs"]
                 wg.parent_uuid = self.node.uuid
                 wg.save(metadata={"call_link_label": name})
                 print("submit workgraph: ")
                 process = self.submit(wg.process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
-            elif node["metadata"]["node_type"] in ["workgraph"]:
+            elif node["metadata"]["node_type"].upper() in ["WORKGRAPH"]:
                 from aiida_workgraph.utils import merge_properties
                 from aiida_workgraph.utils.analysis import WorkGraphSaver
 
                 print("node  type: workgraph.")
                 wgdata = node["executor"]["wgdata"]
                 wgdata["name"] = name
                 wgdata["metadata"]["group_outputs"] = self.ctx.nodes[name]["metadata"][
@@ -804,15 +817,15 @@
                 saver = WorkGraphSaver(process_inited.node, wgdata)
                 saver.save()
                 print("submit workgraph: ")
                 process = self.submit(process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
-            elif node["metadata"]["node_type"] in ["Normal"]:
+            elif node["metadata"]["node_type"].upper() in ["NORMAL"]:
                 print("node  type: Normal.")
                 # normal function does not have a process
                 if "context" in node["metadata"]["kwargs"]:
                     self.ctx.node_name = name
                     kwargs.update({"context": self.ctx})
                 for key in self.ctx.nodes[name]["metadata"]["args"]:
                     kwargs.pop(key, None)
@@ -948,20 +961,23 @@
             name = value[2:-2].strip()
             return get_nested_dict(self.ctx, name)
         return value
 
     def node_to_context(self, name: str) -> None:
         """Export node result to context."""
         from aiida_workgraph.utils import update_nested_dict
+        from aiida.common.exceptions import NotExistentKeyError
 
         items = self.ctx.nodes[name]["to_context"]
         for item in items:
-            update_nested_dict(
-                self.ctx, item[1], self.ctx.nodes[name]["results"][item[0]]
-            )
+            try:
+                result = self.ctx.nodes[name]["results"][item[0]]
+                update_nested_dict(self.ctx, item[1], result)
+            except NotExistentKeyError as e:
+                print(f"Warning: {e}. Skipping update for item {item[0]}")
 
     def check_node_state(self, name: str) -> None:
         """Check node states.
 
         - if all input nodes finished, launch node
         - if node is a scatter node, check if all scattered nodes finished
         """
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/executors/builtin.py` & `aiida_workgraph-0.2.4/aiida_workgraph/executors/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/executors/qe.py` & `aiida_workgraph-0.2.4/aiida_workgraph/executors/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/executors/test.py` & `aiida_workgraph-0.2.4/aiida_workgraph/executors/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/node.py` & `aiida_workgraph-0.2.4/aiida_workgraph/node.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,41 +3,49 @@
 from aiida_workgraph.sockets import socket_pool
 from aiida_workgraph.widget import NodeGraphWidget
 from aiida_workgraph.collection import (
     WorkGraphPropertyCollection,
     WorkGraphInputSocketCollection,
     WorkGraphOutputSocketCollection,
 )
-from typing import Any, Dict, Optional, Union, Callable
+import aiida
+from typing import Any, Dict, Optional, Union, Callable, List
 
 
 class Node(GraphNode):
     """Represent a Node in the AiiDA WorkGraph.
 
     The class extends from node_graph.node.Node and add new
     attributes to it.
     """
 
     property_pool = property_pool
     socket_pool = socket_pool
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        to_context: Optional[List[Any]] = None,
+        wait: List[Union[str, GraphNode]] = [],
+        process: Optional[aiida.orm.ProcessNode] = None,
+        pk: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
         Initialize a Node instance.
         """
         super().__init__(
             property_collection_class=WorkGraphPropertyCollection,
             input_collection_class=WorkGraphInputSocketCollection,
             output_collection_class=WorkGraphOutputSocketCollection,
             **kwargs
         )
-        self.to_context = None
-        self.wait = []
-        self.process = None
-        self.pk = None
+        self.to_context = [] if to_context is None else to_context
+        self.wait = [] if wait is None else wait
+        self.process = process
+        self.pk = pk
         self._widget = NodeGraphWidget(
             settings={"minmap": False},
             style={"width": "40%", "height": "600px"},
         )
 
     def to_dict(self) -> Dict[str, Any]:
         ndata = super().to_dict()
@@ -66,15 +74,25 @@
         """Create a node from a identifier."""
         from aiida_workgraph.nodes import node_pool
 
         return super().new(identifier, name=name, node_pool=node_pool)
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any], node_pool: Optional[Any] = None) -> "Node":
-        """Create a node from a dictionary."""
+        """Create a node from a dictionary. This method initializes a Node instance with properties and settings
+        defined within the provided data dictionary. If node_pool is not specified, the default node_pool from
+        aiida_workgraph.nodes is used.
+
+        Args:
+            data (Dict[str, Any]): A dictionary containing the node's configuration.
+            node_pool (Optional[Any]): A pool of node configurations, defaults to None
+            which will use the global node_pool.
+
+        Returns:
+            Node: An instance of Node initialized with the provided data."""
         from aiida_workgraph.nodes import node_pool
 
         node = super().from_dict(data, node_pool=node_pool)
         node.to_context = data.get("to_context", [])
         node.wait = data.get("wait", [])
         node.process = data.get("process", None)
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/nodes/__init__.py` & `aiida_workgraph-0.2.4/aiida_workgraph/nodes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,14 @@
     AiiDASumDiff,
     AiiDAArithmeticMultiplyAdd,
 )
 from .qe import (
     AiiDAKpoint,
     AiiDAPWPseudo,
     AiiDAStructure,
-    AiiDAPW,
-    AiiDADos,
-    AiiDAProjwfc,
 )
 
 node_list = [
     AiiDAGather,
     AiiDAToCtx,
     AiiDAFromCtx,
     AiiDAShell,
@@ -37,15 +34,12 @@
     AiiDAAdd,
     AiiDAGreater,
     AiiDASumDiff,
     AiiDAArithmeticMultiplyAdd,
     AiiDAKpoint,
     AiiDAPWPseudo,
     AiiDAStructure,
-    AiiDAPW,
-    AiiDADos,
-    AiiDAProjwfc,
 ]
 
 
 # should after node_list, otherwise circular import
 node_pool = get_entries(entry_point_name="aiida_workgraph.node")
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/nodes/builtin.py` & `aiida_workgraph-0.2.4/aiida_workgraph/nodes/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AiiDAGather(Node):
     """AiiDAGather"""
 
     identifier = "AiiDAGather"
     name = "AiiDAGather"
-    node_type = "workchain"
+    node_type = "WORKCHAIN"
     catalog = "AiiDA"
     kwargs = ["datas"]
 
     def create_sockets(self) -> None:
         self.inputs.clear()
         self.outputs.clear()
         inp = self.inputs.new("General", "datas")
@@ -130,15 +130,15 @@
 
 
 class AiiDAShell(Node):
     """AiiDAShell"""
 
     identifier = "AiiDAShell"
     name = "AiiDAShell"
-    node_type = "calcjob"
+    node_type = "CALCJOB"
     catalog = "AiiDA"
     kwargs = shelljob_inputs
 
     def create_sockets(self) -> None:
         self.inputs.clear()
         self.outputs.clear()
         for inp in shelljob_inputs:
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/nodes/test.py` & `aiida_workgraph-0.2.4/aiida_workgraph/nodes/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         }
 
 
 class AiiDAAdd(Node):
 
     identifier: str = "AiiDAAdd"
     name = "AiiDAAdd"
-    node_type = "calcfunction"
+    node_type = "CALCFUNCTION"
     catalog = "Test"
 
     args = ["x", "y"]
     kwargs = ["t"]
 
     def create_properties(self) -> None:
         self.properties.new("AiiDAFloat", "t", default=1.0)
@@ -196,15 +196,15 @@
         }
 
 
 class AiiDAGreater(Node):
 
     identifier: str = "AiiDAGreater"
     name = "AiiDAGreater"
-    node_type = "calcfunction"
+    node_type = "CALCFUNCTION"
     catalog = "Test"
     kwargs = ["x", "y"]
 
     def create_properties(self) -> None:
         pass
 
     def create_sockets(self) -> None:
@@ -221,15 +221,15 @@
         }
 
 
 class AiiDASumDiff(Node):
 
     identifier: str = "AiiDASumDiff"
     name = "AiiDASumDiff"
-    node_type = "calcfunction"
+    node_type = "CALCFUNCTION"
     catalog = "Test"
 
     args = ["x", "y"]
     kwargs = ["t"]
 
     def create_properties(self) -> None:
         self.properties.new("AiiDAFloat", "t", default=1.0)
@@ -251,15 +251,15 @@
         }
 
 
 class AiiDAArithmeticMultiplyAdd(Node):
 
     identifier: str = "AiiDAArithmeticMultiplyAdd"
     name = "AiiDAArithmeticMultiplyAdd"
-    node_type = "workchain"
+    node_type = "WORKCHAIN"
     catalog = "Test"
     kwargs = ["code", "x", "y", "z"]
 
     def create_properties(self) -> None:
         pass
 
     def create_sockets(self) -> None:
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/orm/worktree.py` & `aiida_workgraph-0.2.4/aiida_workgraph/orm/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/properties/built_in.py` & `aiida_workgraph-0.2.4/aiida_workgraph/properties/built_in.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,22 +35,26 @@
     identifier: str = "AiiDAInt"
     data_type = "Int"
 
     def __init__(
         self,
         name: str,
         description: str = "",
-        default: Union[int, None] = 0,
+        default: Union[int, None] = None,
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value: Union[int, orm.Int, str]) -> None:
         # run the callback function
-        if isinstance(value, int):
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif isinstance(value, int):
             self._value = orm.Int(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, orm.Int):
             self._value = value
             if self.update is not None:
                 self.update()
@@ -70,22 +74,26 @@
     identifier: str = "AiiDAFloat"
     data_type = "Float"
 
     def __init__(
         self,
         name: str,
         description: str = "",
-        default: Union[int, None] = 0.0,
+        default: Union[int, None] = None,
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value: Union[float, orm.Float, int, orm.Int, str]) -> None:
         # run the callback function
-        if isinstance(value, (int, float)):
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif isinstance(value, (int, float)):
             self._value = orm.Float(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, (orm.Int, orm.Float)):
             self._value = value
             if self.update is not None:
                 self.update()
@@ -105,22 +113,26 @@
     identifier: str = "AiiDABool"
     data_type = "Bool"
 
     def __init__(
         self,
         name: str,
         description: str = "",
-        default: Union[bool, None] = True,
+        default: Union[bool, None] = None,
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value: Union[bool, orm.Bool, int, str]) -> None:
         # run the callback function
-        if isinstance(value, (bool, int)):
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif isinstance(value, (bool, int)):
             self._value = orm.Bool(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, (orm.Bool)):
             self._value = value
             if self.update is not None:
                 self.update()
@@ -140,21 +152,25 @@
     identifier: str = "AiiDAString"
     data_type = "String"
 
     def __init__(
         self,
         name: str,
         description: str = "",
-        default: Union[str, orm.Str, None] = True,
+        default: Union[str, orm.Str, None] = None,
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value: Union[str, orm.Str]) -> None:
-        if isinstance(value, str):
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif isinstance(value, str):
             self._value = orm.Str(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, orm.Str):
             self._value = value
             if self.update is not None:
                 self.update()
@@ -180,15 +196,19 @@
         description: str = "",
         default: Union[dict, orm.Dict, None] = True,
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, default, update)
 
     def set_value(self, value: Union[Dict, orm.Dict, str]) -> None:
-        if isinstance(value, dict):
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif isinstance(value, dict):
             self._value = orm.Dict(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, orm.Dict):
             self._value = value
             if self.update is not None:
                 self.update()
@@ -216,15 +236,19 @@
         default: List[int] = [0, 0, 0],
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, size, default, update)
 
     def set_value(self, value: List[int]) -> None:
         # run the callback function
-        if len(value) == self.size:
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif len(value) == self.size:
             for i in range(self.size):
                 if isinstance(value[i], int):
                     self._value[i] = value[i]
                     if self.update is not None:
                         self.update()
                 else:
                     raise Exception(
@@ -250,15 +274,19 @@
         default: List[float] = [0.0, 0.0, 0.0],
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, size, default, update)
 
     def set_value(self, value: List[Union[int, float]]) -> None:
         # run the callback function
-        if len(value) == self.size:
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif len(value) == self.size:
             for i in range(self.size):
                 if isinstance(value[i], (int, float)):
                     self._value[i] = value[i]
                     if self.update is not None:
                         self.update()
                 else:
                     raise Exception("{} is not a float.".format(value[i]))
@@ -290,15 +318,19 @@
         default: List[bool] = [False, False, False],
         update: Callable = None,
     ) -> None:
         super().__init__(name, description, size, default, update)
 
     def set_value(self, value: List[Union[bool, int]]) -> None:
         # run the callback function
-        if len(value) == self.size:
+        if value is None:
+            self._value = value
+            if self.update is not None:
+                self.update()
+        elif len(value) == self.size:
             for i in range(self.size):
                 if isinstance(value[i], (bool, int)):
                     self._value[i] = value[i]
                     if self.update is not None:
                         self.update()
                 else:
                     raise Exception("{} is not a bool.".format(value[i]))
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/property.py` & `aiida_workgraph-0.2.4/aiida_workgraph/property.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/socket.py` & `aiida_workgraph-0.2.4/aiida_workgraph/socket.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/sockets/built_in.py` & `aiida_workgraph-0.2.4/aiida_workgraph/sockets/built_in.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import Optional, Any
 from aiida_workgraph.socket import NodeSocket
 from node_graph.serializer import SerializeJson, SerializePickle
 from node_graph.sockets.builtin import (
+    SocketInt,
+    SocketFloat,
+    SocketString,
+    SocketBool,
     SocketBaseDict,
     SocketBaseList,
 )
 
 
 class SocketGeneral(NodeSocket, SerializePickle):
     """General socket."""
@@ -131,14 +135,18 @@
     ) -> None:
         super().__init__(name, node, type, index, uuid=uuid)
         self.add_property("FloatVector", name, **kwargs)
 
 
 socket_list = [
     SocketGeneral,
+    SocketInt,
+    SocketFloat,
+    SocketString,
+    SocketBool,
     SocketBaseDict,
     SocketBaseList,
     SocketAiiDAInt,
     SocketAiiDAFloat,
     SocketAiiDAString,
     SocketAiiDABool,
     SocketAiiDAIntVector,
```

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/utils/__init__.py` & `aiida_workgraph-0.2.4/aiida_workgraph/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/utils/analysis.py` & `aiida_workgraph-0.2.4/aiida_workgraph/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/utils/graph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/utils/graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/README.md` & `aiida_workgraph-0.2.4/aiida_workgraph/web/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/api.py` & `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/api.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/daemon.py` & `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/datanode.py` & `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/datanode.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/utils.py` & `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/backend/app/workgraph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/README.md` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/asset-manifest.json` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/favicon.ico` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/index.html` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/package-lock.json` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/package.json` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/favicon.ico` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/public/index.html` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/App.css` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/App.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/AtomsItem.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/AtomsItem.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/DataNodeTable.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Layout.css` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Layout.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/NodeDetails.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/NodeDetails.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/Settings.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Settings.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/index.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/logo.svg` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization.ts` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/customization/background.css` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/background.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/default.ts` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/default.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/src/rete/index.ts` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/index.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/web/frontend/tsconfig.json` & `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/README.md` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/js/default_rete.ts` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/default_rete.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/js/widget.css` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/js/widget.tsx` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/package-lock.json` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/package.json` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/pyproject.toml` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/__init__.py` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/static/widget.js` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/widget/src/widget/utils.py` & `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.3/aiida_workgraph/workgraph.py` & `aiida_workgraph-0.2.4/aiida_workgraph/workgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import aiida.orm
 import node_graph
 import aiida
+from aiida.manage import get_manager
 from aiida_workgraph.nodes import node_pool
 import time
 from aiida_workgraph.collection import WorkGraphNodeCollection
 from aiida_workgraph.utils.graph import (
     node_deletion_hook,
     node_creation_hook,
     link_creation_hook,
@@ -58,30 +59,31 @@
     def run(self, inputs: Optional[Dict[str, Any]] = None) -> Any:
         """
         Run the AiiDA workgraph process and update the process status. The method uses AiiDA's engine to run
         the process and then calls the update method to update the state of the process.
         """
         from aiida_workgraph.engine.workgraph import WorkGraph as WorkGraphEngine
         from aiida_workgraph.utils import merge_properties
-        from aiida.manage import manager
 
         # set node inputs
         if inputs is not None:
             for name, input in inputs.items():
+                if name not in self.nodes.keys():
+                    raise KeyError(f"Node {name} not found in WorkGraph.")
                 self.nodes[name].set(input)
         # One can not run again if the process is alreay created. otherwise, a new process node will
         # be created again.
         if self.process is not None:
             print("Your workgraph is already created. Please use the submit() method.")
             return
         wgdata = self.to_dict()
         merge_properties(wgdata)
         inputs = {"wg": wgdata}
         # init a process
-        runner = manager.get_manager().get_runner()
+        runner = get_manager().get_runner()
         process_inited = WorkGraphEngine(runner=runner, inputs=inputs)
         self.process = process_inited.node
         # save workgraph data into process node
         self.save_to_base(wgdata)
         result = aiida.engine.run(process_inited)
         self.update()
         return result
@@ -97,19 +99,19 @@
         """Submit the AiiDA workgraph process and optionally wait for it to finish.
         Args:
             wait (bool): Wait for the process to finish.
             timeout (int): The maximum time in seconds to wait for the process to finish. Defaults to 60.
             restart (bool): Restart the process, and reset the modified nodes, then only re-run the modified nodes.
             new (bool): Submit a new process.
         """
-        from aiida.manage import get_manager
-
         # set node inputs
         if inputs is not None:
             for name, input in inputs.items():
+                if name not in self.nodes.keys():
+                    raise KeyError(f"Node {name} not found in WorkGraph.")
                 self.nodes[name].set(input)
 
         process_controller = get_manager().get_process_controller()
         # Create a new submission
         if self.process is not None and new:
             self.reset()
         # Create a restart submission
@@ -117,15 +119,15 @@
         # so that the WorkGraphSaver can compare the difference, and reset the modified nodes
         if restart:
             self.restart_process = self.process
             self.process = None
         # save the workgraph to the process node
         self.save()
         if self.process.process_state.value.upper() not in ["CREATED"]:
-            return "Error!!! The process has already been submitted and finished."
+            raise ValueError(f"Process {self.process.pk} has already been submitted.")
         # launch the process, send the task to RabbitMA
         # TODO in case of "[ERROR] Process<3705> is unreachable."
         process_controller.continue_process(self.process.pk)
         if wait:
             self.wait(timeout=timeout)
         return self.process
```

### Comparing `aiida_workgraph-0.2.3/pyproject.toml` & `aiida_workgraph-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Topic :: Scientific/Engineering"
 ]
 keywords = ["aiida", "workflows"]
 requires-python = ">=3.9"
 dependencies = [
     "numpy~=1.21",
     "node-graph>=0.0.6",
-    "anywidget==0.9.2",
+    "anywidget>=0.9.11",
     "aiida-core>=2.3",
     "cloudpickle",
     "aiida-pseudo",
     "aiida-quantumespresso",
     "aiida-shell",
     "fastapi",
     "uvicorn",
```

### Comparing `aiida_workgraph-0.2.3/PKG-INFO` & `aiida_workgraph-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-workgraph
-Version: 0.2.3
+Version: 0.2.4
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Keywords: aiida,workflows
 Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AiiDA
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: numpy~=1.21
 Requires-Dist: node-graph>=0.0.6
-Requires-Dist: anywidget==0.9.2
+Requires-Dist: anywidget>=0.9.11
 Requires-Dist: aiida-core>=2.3
 Requires-Dist: cloudpickle
 Requires-Dist: aiida-pseudo
 Requires-Dist: aiida-quantumespresso
 Requires-Dist: aiida-shell
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
@@ -47,14 +47,15 @@
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 # AiiDA-WorkGraph
 [![PyPI version](https://badge.fury.io/py/aiida-workgraph.svg)](https://badge.fury.io/py/aiida-workgraph)
 [![Unit test](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-workgraph/actions/workflows/ci.yaml)
+[![codecov](https://codecov.io/gh/superstar54/aiida-workgraph/branch/main/graph/badge.svg)](https://codecov.io/gh/superstar54/aiida-workgraph)
 [![Docs status](https://readthedocs.org/projects/aiida-workgraph/badge)](http://aiida-workgraph.readthedocs.io/)
 
 Provides the third workflow component: `WorkGraph`, to design flexible node-based workflows using AiiDA.
 
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-WorkGraph provides the third component: `WorkGraph`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
```

