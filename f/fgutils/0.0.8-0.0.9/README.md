# Comparing `tmp/fgutils-0.0.8.tar.gz` & `tmp/fgutils-0.0.9.tar.gz`

## Comparing `fgutils-0.0.8.tar` & `fgutils-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fgutils-0.0.8/.coveragerc
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 fgutils-0.0.8/lint.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fgutils-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 fgutils-0.0.8/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fgutils-0.0.8/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/__init__.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/fgconfig.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/mapping.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/parse.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/permutation.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/query.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/rdkit.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 fgutils-0.0.8/fgutils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/__init__.py
--rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_fgconfig.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_mapping.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_parse.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_permutation.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_query.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fgutils-0.0.8/test/test_utils.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 fgutils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fgutils-0.0.8/LICENSE
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fgutils-0.0.8/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fgutils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fgutils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fgutils-0.0.9/.coveragerc
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 fgutils-0.0.9/lint.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fgutils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 fgutils-0.0.9/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 fgutils-0.0.9/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/__init__.py
+-rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/fgconfig.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/mapping.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/parse.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/permutation.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/query.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/rdkit.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 fgutils-0.0.9/fgutils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_fgconfig.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_mapping.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_parse.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_permutation.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_query.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fgutils-0.0.9/test/test_utils.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 fgutils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fgutils-0.0.9/LICENSE
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fgutils-0.0.9/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fgutils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fgutils-0.0.9/PKG-INFO
```

### Comparing `fgutils-0.0.8/.github/workflows/publish-package.yml` & `fgutils-0.0.9/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/.github/workflows/test-and-lint.yml` & `fgutils-0.0.9/.github/workflows/test-and-lint.yml`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/fgutils/fgconfig.py` & `fgutils-0.0.9/fgutils/fgconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     {"name": "ester", "pattern": "RC(=O)OR", "group_atoms": [1, 2, 3]},
     {"name": "thioester", "pattern": "RC(=O)SR", "group_atoms": [1, 2, 3]},
     {"name": "anhydride", "pattern": "RC(=O)OC(=O)R", "group_atoms": [1, 2, 3, 4, 5]},
     {"name": "amine", "pattern": "RN(R)R", "group_atoms": [1]},
     {"name": "nitrile", "pattern": "RC#N", "group_atoms": [1, 2]},
     {"name": "nitrose", "pattern": "RN=O", "group_atoms": [1, 2]},
     {"name": "nitro", "pattern": "RN(=O)O", "group_atoms": [1, 2, 3]},
+    {"name": "peroxide", "pattern": "ROOR", "group_atoms": [1, 2]},
     {"name": "peroxy_acid", "pattern": "RC(=O)OOH", "group_atoms": [1, 2, 3, 4, 5]},
     {"name": "hemiketal", "pattern": "RC(OH)(OR)R", "group_atoms": [1, 2, 3, 4]},
     {"name": "phenol", "pattern": "C:COH", "group_atoms": [2, 3]},
     {"name": "anilin", "pattern": "C:CN(R)R", "group_atoms": [2]},
     {"name": "ketene", "pattern": "RC(R)=C=O", "group_atoms": [1, 3, 4]},
     {"name": "carbamate", "pattern": "ROC(=O)N(R)R", "group_atoms": [1, 2, 3, 4]},
     {"name": "acyl_chloride", "pattern": "RC(=O)Cl", "group_atoms": [1, 2, 3]},
```

### Comparing `fgutils-0.0.8/fgutils/mapping.py` & `fgutils-0.0.9/fgutils/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,23 +96,27 @@
     anchor: int,
     pattern: nx.Graph,
     mapper: PermutationMapper,
     pattern_anchor: None | int = None,
 ):
     if pattern_anchor is None:
         if len(pattern) == 0:
-            return True, []
+            return [(True, [])]
+        results = []
         for pidx in pattern.nodes:
             result = map_anchored_pattern(graph, anchor, pattern, pidx, mapper)
-            if result[0]:
-                return result
-        return False, []
+            results.append(result)
+        if len(results) > 0:
+            return results
+        else:
+            return [(False, [])]
     else:
-        return map_anchored_pattern(graph, anchor, pattern, pattern_anchor, mapper)
+        return [map_anchored_pattern(graph, anchor, pattern, pattern_anchor, mapper)]
 
 
 def map_to_entire_graph(graph: nx.Graph, pattern: nx.Graph, mapper: PermutationMapper):
     for i in range(len(graph)):
-        r, _ = map_pattern(graph, i, pattern, mapper)
-        if r is True:
-            return True
+        mappings = map_pattern(graph, i, pattern, mapper)
+        for r, _ in mappings:
+            if r is True:
+                return True
     return False
```

### Comparing `fgutils-0.0.8/fgutils/parse.py` & `fgutils-0.0.9/fgutils/parse.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/fgutils/permutation.py` & `fgutils-0.0.9/fgutils/permutation.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/fgutils/query.py` & `fgutils-0.0.9/fgutils/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,37 +7,42 @@
 from fgutils.fgconfig import FGConfig, FGConfigProvider, FGTreeNode
 
 
 def is_functional_group(graph, index: int, config: FGConfig, mapper: PermutationMapper):
     max_id = len(graph)
     graph = add_implicit_hydrogens(copy.deepcopy(graph))
 
-    is_fg, mapping = map_pattern(graph, index, config.pattern, mapper)
+    is_fg = False
     fg_indices = []
-    if is_fg:
-        fg_indices = [
-            m_id
-            for m_id, fg_id in mapping
-            if fg_id in config.group_atoms and m_id < max_id
-        ]
-        is_fg = index in fg_indices
+    mappings = map_pattern(graph, index, config.pattern, mapper)
+    for _is_fg, _mapping in mappings:
+        if _is_fg:
+            fg_indices = [
+                m_id
+                for m_id, fg_id in _mapping
+                if fg_id in config.group_atoms and m_id < max_id
+            ]
+            is_fg = index in fg_indices
+            if is_fg:
+                break
 
     if is_fg:
         last_len = config.max_pattern_size
         for apattern, apattern_size in sorted(
             [(m, m.number_of_nodes()) for m in config.anti_pattern],
             key=lambda x: x[1],
             reverse=True,
         ):
             if last_len > apattern_size:
                 last_len = apattern_size
-            is_match, _ = map_pattern(graph, index, apattern, mapper)
-            is_fg = is_fg and not is_match
-            if not is_fg:
-                break
+            mappings = map_pattern(graph, index, apattern, mapper)
+            for _is_fg, _ in mappings:
+                is_fg = is_fg and not _is_fg
+                if not is_fg:
+                    break
     return is_fg, sorted(fg_indices)
 
 
 class FGQuery:
     def __init__(
         self,
         use_smiles=False,
@@ -59,14 +64,15 @@
     def __find_best_node_rec(self, nodes: list[FGTreeNode], graph, idx):
         best_node = None
         node_indices = []
         for node in nodes:
             is_fg, fg_indices = is_functional_group(
                 graph, idx, node.fgconfig, mapper=self.mapper
             )
+            print("Is fg {} {}".format(node.fgconfig.name, is_fg))
             if is_fg:
                 r_node, r_indices = self.__find_best_node_rec(
                     node.children,
                     graph,
                     idx,
                 )
                 if r_node is None:
```

### Comparing `fgutils-0.0.8/fgutils/rdkit.py` & `fgutils-0.0.9/fgutils/rdkit.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/fgutils/utils.py` & `fgutils-0.0.9/fgutils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import networkx as nx
 
 
 def print_graph(graph):
     print(
         "Graph Nodes: {}".format(
             " ".join(
@@ -19,14 +20,15 @@
             )
         )
     )
 
 
 def add_implicit_hydrogens(graph: nx.Graph) -> nx.Graph:
     valence_dict = {
+        3: ["B"],
         4: ["C", "Si"],
         5: ["N", "P"],
         6: ["O", "S"],
         7: ["F", "Cl", "Br", "I"],
     }
     valence_table = {}
     for v, elmts in valence_dict.items():
@@ -39,12 +41,13 @@
     ]
     for n_id, n_sym in nodes:
         assert (
             n_sym in valence_table.keys()
         ), "Element {} not found in valence table.".format(n_sym)
         bond_cnt = sum([b for _, _, b in graph.edges(n_id, data="bond")])  # type: ignore
         # h_cnt can be negative; aromaticity is complicated, we just ignore that
-        h_cnt = int(8 - valence_table[n_sym] - bond_cnt)
+        valence = valence_table[n_sym]
+        h_cnt = int(np.min([8, 2 * valence]) - valence - bond_cnt)
         for h_id in range(len(graph), len(graph) + h_cnt):
             graph.add_node(h_id, symbol="H")
             graph.add_edge(n_id, h_id, bond=1)
     return graph
```

### Comparing `fgutils-0.0.8/test/test_fgconfig.py` & `fgutils-0.0.9/test/test_fgconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,10 +276,12 @@
             fg.pattern_str, fg.name
         )
         pattern_list.append(fg.pattern_str)
     assert len(_default_fg_config) == len(pattern_list)
 
 
 # def test_build_tree():
-#     tree = build_FG_tree()
+#     from fgutils.fgconfig import print_tree
+#     provider = FGConfigProvider()
+#     tree = provider.get_tree()
 #     print_tree(tree)
 #     assert False
```

### Comparing `fgutils-0.0.8/test/test_mapping.py` & `fgutils-0.0.9/test/test_mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,148 @@
 from fgutils.permutation import PermutationMapper
 from fgutils.parse import parse
 from fgutils.mapping import map_anchored_pattern, map_pattern
 
 default_mapper = PermutationMapper(wildcard="R", ignore_case=True)
 
 
-def _assert_mapping(mapping, valid, exp_mapping=[]):
+def _assert_anchored_mapping(mapping, valid, exp_mapping=[]):
     assert mapping[0] == valid
     for emap in exp_mapping:
         assert emap in mapping[1]
 
 
+def _assert_mapping(mapping, valid, exp_mapping=[], index=0):
+    assert mapping[index][0] == valid
+    for emap in exp_mapping:
+        assert emap in mapping[index][1]
+
+
 def test_simple_match():
     exp_mapping = [(1, 0), (2, 1)]
     g = parse("CCO")
     p = parse("RO")
     m = map_anchored_pattern(g, 2, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_branched_match():
     exp_mapping = [(0, 0), (1, 1), (2, 2), (3, 3)]
     g = parse("CC(=O)O")
     p = parse("RC(=O)O")
     m = map_anchored_pattern(g, 2, p, 2, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_ring_match():
     exp_mapping = [(0, 2), (1, 1), (2, 0)]
     g = parse("C1CO1")
     p = parse("R1CC1")
     m = map_anchored_pattern(g, 1, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_not_match():
     g = parse("CC=O")
     p = parse("RC(=O)NR")
     m = map_anchored_pattern(g, 2, p, 2, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_1():
     g = parse("CC=O")
     p = parse("RC(=O)R")
     m = map_anchored_pattern(g, 0, p, 3, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_2():
     exp_mapping = [(0, 0), (1, 1), (2, 2)]
     g = parse("CC=O")
     p = parse("RC=O")
     m = map_anchored_pattern(g, 2, p, 2, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_ignore_aromaticity():
     exp_mapping = [(1, 0), (2, 1)]
     g = parse("c1c(=O)cccc1")
     p = parse("C=O")
     m = map_anchored_pattern(g, 2, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_3():
     exp_mapping = [(0, 4), (1, 3), (2, 1), (4, 2), (3, 0)]
     g = parse("COC(C)=O")
     p = parse("RC(=O)OR")
     m = map_anchored_pattern(g, 4, p, 2, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_explore_wrong_branch():
     exp_mapping = [(0, 2), (1, 1), (2, 0), (3, 3)]
     g = parse("COCO")
     p = parse("C(OR)O")
     m = map_anchored_pattern(g, 1, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_match_pattern_to_mol():
     exp_mapping = [(0, 2), (1, 0), (2, 1)]
     g = parse("NC(=O)C")
     p = parse("C(=O)N")
     m = map_anchored_pattern(g, 2, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_match_hydrogen():
     # H must be explicit
     g = parse("C=O")
     p = parse("C(H)=O")
     m = map_anchored_pattern(g, 1, p, 2, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_match_implicit_hydrogen():
     exp_mapping = [(0, 0), (1, 2)]
     g = parse("C=O")
     p = parse("C(H)=O")
     mapper = PermutationMapper(can_map_to_nothing=["H"])
     m = map_anchored_pattern(g, 1, p, 2, mapper=mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_invalid_bond_match():
     g = parse("C=O")
     p = parse("CO")
     m = map_anchored_pattern(g, 0, p, 0, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_match_not_entire_pattern():
     g = parse("C=O")
     p = parse("C(=O)C")
     m = map_anchored_pattern(g, 0, p, 0, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_start_with_match_to_nothing():
     g = parse("CCO")
     p = parse("HO")
     m = map_anchored_pattern(g, 2, p, 0, mapper=default_mapper)
-    _assert_mapping(m, False)
+    _assert_anchored_mapping(m, False)
 
 
 def test_match_explicit_hydrogen():
     exp_mapping = [(2, 1), (3, 0)]
     g = parse("CCOH")
     p = parse("HO")
     m = map_anchored_pattern(g, 2, p, 1, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_anchored_mapping(m, True, exp_mapping)
 
 
 def test_map_pattern_with_anchor():
     exp_mapping = [(2, 1), (1, 0)]
     g = parse("CCO")
     p = parse("CO")
     m = map_pattern(g, 2, p, pattern_anchor=1, mapper=default_mapper)
@@ -144,15 +150,15 @@
 
 
 def test_map_pattern_without_anchor():
     exp_mapping = [(2, 1), (1, 0)]
     g = parse("CCO")
     p = parse("CO")
     m = map_pattern(g, 2, p, mapper=default_mapper)
-    _assert_mapping(m, True, exp_mapping)
+    _assert_mapping(m, True, exp_mapping, index=1)
 
 
 def test_map_empty_pattern():
     exp_mapping = []
     g = parse("CCO")
     p = parse("")
     m = map_pattern(g, 2, p, mapper=default_mapper)
```

### Comparing `fgutils-0.0.8/test/test_parse.py` & `fgutils-0.0.9/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/test/test_permutation.py` & `fgutils-0.0.9/test/test_permutation.py`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/test/test_query.py` & `fgutils-0.0.9/test/test_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 @pytest.mark.parametrize(
     "name,smiles,anchor,exp_indices",
     [
         ("carbonyl", "CC(=O)O", 2, [1, 2]),
         ("carboxylic_acid", "CC(=O)O", 2, [1, 2, 3]),
         ("amide", "C(=O)N", 2, [0, 1, 2]),
         ("acyl_chloride", "CC(=O)[Cl]", 3, [1, 2, 3]),
+        ("ether", "COOC", 1, [1]),
+        ("ether", "COOC", 2, [2]),
     ],
 )
 def test_get_functional_group(name, smiles, anchor, exp_indices):
     fg = default_config_provider.get_by_name(name)
     mol = mol_to_graph(rdmolfiles.MolFromSmiles(smiles))
     is_fg, indices = is_functional_group(mol, anchor, fg, mapper=default_mapper)
     assert is_fg
@@ -65,16 +67,30 @@
         ),
         pytest.param(
             "O=C(C)Oc1ccccc1C(=O)O",
             ["ester", "carboxylic_acid"],
             [[0, 1, 3], [10, 11, 12]],
             id="Acetylsalicylic acid",
         ),
+        pytest.param("[NH]1cccc1O", ["phenol"], [[5]], id="Phenol"),
+        pytest.param(
+            "CC(C)(C)OO", ["peroxide"], [[4, 5]], id="tert-Butyl hydroperoxide"
+        ),
+        pytest.param(
+            "C(C)(C)OO", ["peroxide"], [[3, 4]], id="tert-Butyl hydroperoxide"
+        ),
+        pytest.param("CC(=O)OO", ["peroxy_acid"], [[1, 2, 3, 4]], id="Peracid"),
         # pytest.param("", [""], [[]], id=""),
     ],
 )
 def test_functional_group_on_compound(smiles, functional_groups, exp_indices):
     assert len(functional_groups) == len(exp_indices)
     mol = mol_to_graph(rdmolfiles.MolFromSmiles(smiles))
     groups = default_query.get(mol)
     for fg, indices in zip(functional_groups, exp_indices):
         assert (fg, indices) in groups
+
+
+def test_non_carbon_atom_without_functional_group():
+    mol = parse("N(H):1C:C:C:C1")
+    groups = default_query.get(mol)
+    assert 0 == len(groups)
```

### Comparing `fgutils-0.0.8/test/test_utils.py` & `fgutils-0.0.9/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,7 +67,17 @@
     assert 11 == len(graph)
     _assert_Hs(graph, 0, 1)
     _assert_Hs(graph, 1, 1)
     _assert_Hs(graph, 2, 1)
     _assert_Hs(graph, 3, 0)
     _assert_Hs(graph, 4, 1)
     _assert_Hs(graph, 5, 1)
+
+
+def test_boric_acid():
+    graph = parse("OB(O)O")
+    graph = add_implicit_hydrogens(graph)
+    assert 7 == len(graph)
+    _assert_Hs(graph, 0, 1)
+    _assert_Hs(graph, 1, 0)
+    _assert_Hs(graph, 2, 1)
+    _assert_Hs(graph, 3, 1)
```

### Comparing `fgutils-0.0.8/.gitignore` & `fgutils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/LICENSE` & `fgutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/README.md` & `fgutils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fgutils-0.0.8/pyproject.toml` & `fgutils-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fgutils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}]
 description = "Library to get functional groups from molecular graphs."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `fgutils-0.0.8/PKG-INFO` & `fgutils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fgutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to get functional groups from molecular graphs.
 Project-URL: homepage, https://github.com/klausweinbauer/FGUtils
 Project-URL: source, https://github.com/klausweinbauer/FGUtils
 Project-URL: issues, https://github.com/klausweinbauer/FGUtils/issues
 Author-email: Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

