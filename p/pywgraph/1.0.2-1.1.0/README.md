# Comparing `tmp/pywgraph-1.0.2.tar.gz` & `tmp/pywgraph-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywgraph-1.0.2.tar", last modified: Thu May  9 21:29:25 2024, max compression
+gzip compressed data, was "pywgraph-1.1.0.tar", last modified: Wed May 15 11:30:37 2024, max compression
```

## Comparing `pywgraph-1.0.2.tar` & `pywgraph-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-09 21:29:25.170613 pywgraph-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-09 21:29:21.000000 pywgraph-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.166613 pywgraph-1.0.2/pywgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/exceptions/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/groups/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/groups/_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:29:25.170613 pywgraph-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 21:29:21.000000 pywgraph-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_path_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_graph_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.922832 pywgraph-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-15 11:30:37.922832 pywgraph-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-05-15 11:30:34.000000 pywgraph-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.914832 pywgraph-1.1.0/pywgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.918832 pywgraph-1.1.0/pywgraph/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/exceptions/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.918832 pywgraph-1.1.0/pywgraph/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/graphs/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/graphs/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/graphs/_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.918832 pywgraph-1.1.0/pywgraph/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/groups/_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 11:30:34.000000 pywgraph-1.1.0/pywgraph/groups/_predefined_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.918832 pywgraph-1.1.0/pywgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-15 11:30:37.000000 pywgraph-1.1.0/pywgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 11:30:37.000000 pywgraph-1.1.0/pywgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:30:37.000000 pywgraph-1.1.0/pywgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 11:30:37.000000 pywgraph-1.1.0/pywgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 11:30:37.000000 pywgraph-1.1.0/pywgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:30:37.922832 pywgraph-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 11:30:34.000000 pywgraph-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:37.918832 pywgraph-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_path_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_path_finding_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_paths_and_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_weighted_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_weighted_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 11:30:34.000000 pywgraph-1.1.0/tests/test_weighted_directed_graph_arrays.py
```

### Comparing `pywgraph-1.0.2/PKG-INFO` & `pywgraph-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 Metadata-Version: 2.1
 Name: pywgraph
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python implementation of weighted directed graphs
 Home-page: https://github.com/josek98/pywgraph
 Author: josek98
 Author-email: josemmsscc98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # pywgraph
-A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group. 
+
+A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group.
 
 For this reason, this package also includes a basic abstraction of a group. The group definition is base on:
-*  The a function of two variables that return one element (the binary operation of the group).
-*  The inverse function of an element. This is, the function that given an element of the group returns it inverse. 
-*  The identity element of the group.
-*  Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one. 
+
+* The a function of two variables that return one element (the binary operation of the group).
+
+* The inverse function of an element. This is, the function that given an element of the group returns its inverse.
+
+* The identity element of the group.
+
+* Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one.
+
+* [New in `1.1.0`] Optional, a check function to check if an element belongs to the group.
 
 ## QUICKSTART
 
 ### Edges
 
-The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows: 
+The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows:
 
 ```python
 from pywgraph import WeightedDirectedEdge
 
 edge = WeightedDirectedEdge("A", "B", 0.5)
 ```
 
-The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication. 
+The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication.
 
 You can call the start and end nodes with `edge.start` and `edge.end`, respectevely. To get the weight, simply use `edge.weight`. You can also get the *inverse edge* with `edge.inverse`. This is, the edge that connects the end node of `edge` to the start node of `edge` and has `1/edge.weight` as weight (as said previously, in the future this is meant to be the inverse of the weight in the underlying group).
 
-Also, this class is hashable and iterable, yielding the start node, end node and weight. 
-
+Also, this class is hashable and iterable, yielding the start node, end node and weight.
 
 ### Graph
 
-The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication. 
+The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication.
 
 It is also possible, and more comfortable, to create the graph using the `WeightedDirectedGraph.from_dict` method, which instantiates the graph from a dictionary. The keys of the dictionary are the starting nodes. The values must consists of another dictionary, where the keys are the ending nodes and the value is the weight of the edge. It is important that all nodes of the graph must be keys in the dictionary. If, for example, there is a node "C" that has no children nodes, then the dictionary must have a key "C" with a value of `{}`.
-As always, if you want to use another group for the weights you should specify it here. 
+As always, if you want to use another group for the weights you should specify it here.
 
 ```python
 from pywgraph import WeightedDirectedGraph
 
 g = WeightedDirectedGraph.from_dict({
     "A": {"B": 0.5},
     "B": {"A": 0.5, "C": 1.0},
     "C": {}
 })
 ```
 
-The equivalent construction using set of nodes and set of edges is as follows: 
+The equivalent construction using set of nodes and set of edges is as follows:
 
-```python 
+```python
 from pywgraph import WeightedDirectedGraph
 
 graph = WeightedDirectedGraph(
     nodes={"A", "B", "C"},
     edges={
         WeightedDirectedEdge("A", "B", 0.5),
         WeightedDirectedEdge("B", "A", 0.5),
         WeightedDirectedEdge("B", "C", 1.0)
     }
 )
-``` 
+```
 
 You can instantiate a bad define graph by not writting all the nodes that appear in the edges in the nodes set. There is a method `check_defintion` that checks if the graph is well defined, but the check is not enforce. You can retrieve the nodes and edges by `graph.nodes` and `graph.edges`, respectively.
 
 You can also acces the children and the parents of a nodes with the methods `children` and `parents`, respectively.
 
 ```python
 graph.children("A")
@@ -82,110 +88,139 @@
 graph.parents("A")
 # {}
 
 graph.children("B")
 # {"A", "C"}
 ```
 
-The main use of this graph object is to work with their weights as group elements, so you should not add the reverse edge of an existing edge with a bad inverse weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`. 
+The main use of this graph object is to work with their weights as group elements, so normally, you want that reverse edges of existing ones have the inverse weight of the existing edge weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`.
 
 ```python
 graph_w_inverse_edges = graph.add_reverse_edges()
 
 # Updating the graph 
 graph.add_reverse_edges(inplace=True)
 ```
 
 ### Path finding
 
-There is a method `find_path` that finds one of the shortest path between two nodes. This method returns a list of edges that represents the path. The method has two parameters: `start` and `end`. Both must be nodes of the graph. If not, an error is raised. If there is not path between the given nodes the empty list will be return. 
+There is a method `find_paths` that finds all paths between two gven nodes. This method have many options to modify the behaviour of the search. Its parameters are:
+
+* `start`: The node of the graph where the algorithm starts the search.
+* `end`: The target node of the graph to reach.
+* `general_max_visitations`: A non negative integer that specifies the maximum number of times that nodes can be visited along the path. By default is set to one.
+* `specific_max_visitations`: A dictionary whose keys are nodes and values are non negative integers. This specifies the maximum number of times that the key node can be visited along the path, overriding what is set in the `genera_max_visitations` parameter. By default is set to the empty dictionary. You can use this parameter to find paths that avoid one node by setting `genera_max_visitations={"AvoidNode":0}`. You can also use it to find cycles by setting the same starting and ending node and allowing to visit it two times. There is an specific method to find cycles.
+* `max_iter`: A non negative integer that limits the number of iterations of the search algorithm. The algorithm should always finish, but for large and complex paths it can take a lot of iterations. You can use this parameter to limit the amount of iterations to perform. By default is set to the factorial of the number of nodes in the graph. A warning will be raised if the maximum number of iterations is reached.
+* `max_paths`: A non negative integer that limits the number of paths that the method will return. By default is set to infinity, so it will return all the possible paths. If you are interested in finding only one path you can set this parameter to one and the algorithm will finish after finding it.
+
+The result of this method will be a list of `Paths` objects, which is just a direct subclass of `list[str]` that is used to represent a path. If no path was found the result will be an empty list.
 
 ```python
 dictionary = {
-    "A": {"B": 1.0, "C": 2.5},
-    "B": {"C": 2.5},
-    "C": {"A": 1 / 2.5, "D": 1.3},
-    "D": {"E": 3.4},
-    "E": {"C": 1 / (1.3 * 3.4), "A": 13.0},
+    "A": {"B": 1},
+    "B": {"C": 2.5, "A": 1},
+    "C": {},
     "Z": {},
 }
 graph = WeightedDirectedGraph.from_dict(dictionary)
 
-graph.find_path("A", "B")
-# ["A", "B]
+graph.find_paths("A", "B")
+# [["A", "B]]
 
-graph.find_path("A", "Z")
+graph.find_paths("A", "Z")
 # []
 
-graph.find_path("A", "E")
-# ["A", "C", "D", "E"]
+graph.find_paths("A", "C")
+# [["A", "B", "C"]]
+
+graph.find_paths("A", "A")
+# [["A"]]
+
+graph.find_paths("A", "A", general_max_visitations=2)
+# [['A'], ['A','B','A'], ['A','B','C','B','A']]
 
-graph.find_path("A", "A")
-# ["A"]
+graph.find_paths("A", "B", general_max_visitations=2)
+# [['A','B'], ['A','B','A','B], ['A','B','C','B']]
+
+graph.find_paths("A", "B", specific_max_visitations={"B":2})
+# [['A','B'], ['A','B','C','B']
 ```
 
-There are also methods to get the weight of following a path. This methods are `path_weight` and `weight_between`. The first one receives a path (a list of consecutive nodes) and returns the weight of the path (the product of the weights). If the given path does not exists an exception will be raised. If the empty path is given the return weight will be `0`. The second method receives the start and end nodes and returns the weight of one of the shortest paths between them. If there is not path between the given nodes the return weight will be `0`. The weight between a node an itself will be `1`. 
+There is also a method to get the weight of following a path. This method is call `path_weight`. It receives a `Path` object or `list[str]` and returns the weight of the path (the product of the weights). You can set a default value (like the python `dict.get`) that will be return if the path is empty. By default it is set to `None`. If the given path does not exists an exception will be raised. If the given path consists of just one node, the identity element of the group (1.0 for standard graphs) will be return.
 
 ```python
-graph.path_weight([])
-# 0.0
+graph.path_weight([], "Helo World")
+# "Helo World"
 
 graph.path_weight(["A", "B"])
 # 1.0
 
 graph.path_weight(["A", "B", "C"])
 # 2.5
 
-grap.weight_between("A", "C")
-# 2.5
-
-grap.weight_between("A", "Z")
-# 0.0
-
-grap.weight_between("A", "A")
+graph.path_weight(["Z"])
 # 1.0
 ```
 
-**WARNING**: Currently, if a path that contains a cycle is given the method `path_weight` will raise an error. In future this behaviour will be change to allow cycles. 
-
 ### Graphs and groups
 
 #### Introduction to the `Group` class
-As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows. 
+
+As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows.
 
 ```python
+import numpy as np
 from pywgraph import Group
 
 group = Group(
     name="R^2 under addition",
     operation=lambda x, y: x + y,
     inverse_function=lambda x: -x,
     identity=np.zeros(2),
     hash_function=lambda x: hash(tuple(x))
 )
 ```
 
-This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. 
+You can also provide a check function that checks if an object belongs to the group. In the above case, a checker function could be defined by:
+
+```python
+def r_2_check(weight: Any) -> bool:
+    if not isinstance(weight, np.ndarray): 
+        return False
+    if len(weight) != 2:
+        return False
+    if not all(isinstance(x, (int, float)) for x in weight):
+        return False
+    return True
+```
+
+This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. If provided a check function, you can check if an object belongs to the group with the method `Group.check`.
 
 ```python
 import numpy as np 
 vector_1 = np.array([1, 3])
 vector_2 = np.arra([-1, 7])
 
 group(vector_1, vector_2)
 # np.array([0, 10])
 
 group.operation(vector_1, vector_2)
 # np.array([0, 10])
 
-group.inverse_operation(vector_1, vector_2)
-# np.array([2, -4])
+group.inverse(vector_1)
+# np.array([-1, -3])
 
-group.neutral_element
+group.identity
 # np.array([0, 0])
+
+group.check(vector_1)
+# True
+
+group.check(23)
+# False
 ```
 
 #### General weights for edges
 
 Now that we introduce how to construct a group we will se how to use it to provide elements of an arbitrary group as weights of an edge. To do so you just need to create the group and add it as a parameter in the constructor of edge.
 
 ```python
@@ -199,28 +234,28 @@
     hash_function=lambda x: hash(tuple(x))
 )
 weight_of_edge = np.array([1, 2])
 
 edge = WeightedDirectedEdge("A", "B", weight_of_edge, group)
 ```
 
-With the group information given, now this edge instance knows how to construct the inverse edge. 
+With the group information given, now this edge instance knows how to construct the inverse edge.
 
 ```python
 edge.inverse
 # WeightedDirectedEdge("B", "A", np.array([-1, -2]), group)
 ```
 
-Is important to notice that there is no checking of wether the provide weight is a valid element of the given group. In the future there will be an option to implement an element checker in the group definition. 
+Is important to notice that there is no checking of wether the provide weight is a valid element of the given group.
 
 #### General weighted graphs
 
-Now for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter. 
+Now, for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter.
 
-With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method. 
+With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method.
 
 ```python
 from pywgraph import WeightedDirectedGraph, Group
 import numpy as np 
 group = Group(
     "R^2 under addition",
     lambda x, y: x + y,
@@ -241,34 +276,35 @@
 # Creates the graph
 
 graph.path_weight(["A", "C"])
 # np.array([-1, 3.4])
 
 graph.path_weight(["A", "B", "C"])
 # np.array([1, 2.5]) + np.array([2.5, -1]) = np.array([3.5, 1.5])
-
-graph.weight_between("A", "C")
-# np.array([-1, 3.4])
-
-graph.weight_between("A", "Z")
-# np.array([0, 0])
-
-graph.weight_between("A", "Z")
-# None
-
-graph.weight_between("A", "Z", np.array([1,1]))
-# np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
-- Added a method to `WeightedDirectedGraph` to add a new node. 
-- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+* Added a method to `WeightedDirectedGraph` to add a new node.
+* Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
 
 ### Version 1.0.2 (2024-05-09)
 
-- Added a method to `WeightedDirectedGraph` to remove a node. 
-- Added a method to `WeightedDirectedGraph` to remove an edge. 
+* Added a method to `WeightedDirectedGraph` to remove a node.
+* Added a method to `WeightedDirectedGraph` to remove an edge.
+
+### Version 1.1.0 (2024-05-15)
+
+* The `Group` class now has a `group_checker` optional parameter that consists of a function to check wether an element belongs to the group or not.
+
+* Add the method `WeightedDirectedGraph.find_paths` to find all paths between two given nodes.
+* The method `WeightedDirectedGraph.find_path` is deprecated and will be removed, use `find_paths` with `max_paths=1` to replicate `WeightedDirectedGraph.find_path` behaviour.
+* Add `Path` and `Cycle` classes to represent an abstraction of a node path and a node cycle.
+* Add method `WeightedDirectedGraph.get_node_cycles` to find all cycles that contains the node.
+* Add property `WeightedDirectedGraph.cycles` that returns the set of all simple cycles of the graph.
+* Add the property `WeightedDirectedGraph.is_conmutative` that checks it the graph is conmutative.
+* The method `WeightedDirectedGraph.weight_between` is deprecated and will be removed. Combine `WeightedDirectedGraph.find_paths` with `WeightedDirectedGraph.path_weight` to replicate `WeightedDirectedGraph.weight_between` behaviour.
+* The behaviour of `WeightedDirectedGraph.add_edge` when no weight and path is given is deprecated and will be removed. Either give a weight or seach for a path.
```

### Comparing `pywgraph-1.0.2/README.md` & `pywgraph-1.1.0/pywgraph.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,85 @@
+Metadata-Version: 2.1
+Name: pywgraph
+Version: 1.1.0
+Summary: A python implementation of weighted directed graphs
+Home-page: https://github.com/josek98/pywgraph
+Author: josek98
+Author-email: josemmsscc98@gmail.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Requires-Dist: pytest>=7.0; extra == "dev"
+Requires-Dist: twine>=4.0.2; extra == "dev"
+
 # pywgraph
-A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group. 
+
+A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group.
 
 For this reason, this package also includes a basic abstraction of a group. The group definition is base on:
-*  The a function of two variables that return one element (the binary operation of the group).
-*  The inverse function of an element. This is, the function that given an element of the group returns it inverse. 
-*  The identity element of the group.
-*  Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one. 
+
+* The a function of two variables that return one element (the binary operation of the group).
+
+* The inverse function of an element. This is, the function that given an element of the group returns its inverse.
+
+* The identity element of the group.
+
+* Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one.
+
+* [New in `1.1.0`] Optional, a check function to check if an element belongs to the group.
 
 ## QUICKSTART
 
 ### Edges
 
-The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows: 
+The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows:
 
 ```python
 from pywgraph import WeightedDirectedEdge
 
 edge = WeightedDirectedEdge("A", "B", 0.5)
 ```
 
-The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication. 
+The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication.
 
 You can call the start and end nodes with `edge.start` and `edge.end`, respectevely. To get the weight, simply use `edge.weight`. You can also get the *inverse edge* with `edge.inverse`. This is, the edge that connects the end node of `edge` to the start node of `edge` and has `1/edge.weight` as weight (as said previously, in the future this is meant to be the inverse of the weight in the underlying group).
 
-Also, this class is hashable and iterable, yielding the start node, end node and weight. 
-
+Also, this class is hashable and iterable, yielding the start node, end node and weight.
 
 ### Graph
 
-The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication. 
+The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication.
 
 It is also possible, and more comfortable, to create the graph using the `WeightedDirectedGraph.from_dict` method, which instantiates the graph from a dictionary. The keys of the dictionary are the starting nodes. The values must consists of another dictionary, where the keys are the ending nodes and the value is the weight of the edge. It is important that all nodes of the graph must be keys in the dictionary. If, for example, there is a node "C" that has no children nodes, then the dictionary must have a key "C" with a value of `{}`.
-As always, if you want to use another group for the weights you should specify it here. 
+As always, if you want to use another group for the weights you should specify it here.
 
 ```python
 from pywgraph import WeightedDirectedGraph
 
 g = WeightedDirectedGraph.from_dict({
     "A": {"B": 0.5},
     "B": {"A": 0.5, "C": 1.0},
     "C": {}
 })
 ```
 
-The equivalent construction using set of nodes and set of edges is as follows: 
+The equivalent construction using set of nodes and set of edges is as follows:
 
-```python 
+```python
 from pywgraph import WeightedDirectedGraph
 
 graph = WeightedDirectedGraph(
     nodes={"A", "B", "C"},
     edges={
         WeightedDirectedEdge("A", "B", 0.5),
         WeightedDirectedEdge("B", "A", 0.5),
         WeightedDirectedEdge("B", "C", 1.0)
     }
 )
-``` 
+```
 
 You can instantiate a bad define graph by not writting all the nodes that appear in the edges in the nodes set. There is a method `check_defintion` that checks if the graph is well defined, but the check is not enforce. You can retrieve the nodes and edges by `graph.nodes` and `graph.edges`, respectively.
 
 You can also acces the children and the parents of a nodes with the methods `children` and `parents`, respectively.
 
 ```python
 graph.children("A")
@@ -69,110 +88,139 @@
 graph.parents("A")
 # {}
 
 graph.children("B")
 # {"A", "C"}
 ```
 
-The main use of this graph object is to work with their weights as group elements, so you should not add the reverse edge of an existing edge with a bad inverse weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`. 
+The main use of this graph object is to work with their weights as group elements, so normally, you want that reverse edges of existing ones have the inverse weight of the existing edge weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`.
 
 ```python
 graph_w_inverse_edges = graph.add_reverse_edges()
 
 # Updating the graph 
 graph.add_reverse_edges(inplace=True)
 ```
 
 ### Path finding
 
-There is a method `find_path` that finds one of the shortest path between two nodes. This method returns a list of edges that represents the path. The method has two parameters: `start` and `end`. Both must be nodes of the graph. If not, an error is raised. If there is not path between the given nodes the empty list will be return. 
+There is a method `find_paths` that finds all paths between two gven nodes. This method have many options to modify the behaviour of the search. Its parameters are:
+
+* `start`: The node of the graph where the algorithm starts the search.
+* `end`: The target node of the graph to reach.
+* `general_max_visitations`: A non negative integer that specifies the maximum number of times that nodes can be visited along the path. By default is set to one.
+* `specific_max_visitations`: A dictionary whose keys are nodes and values are non negative integers. This specifies the maximum number of times that the key node can be visited along the path, overriding what is set in the `genera_max_visitations` parameter. By default is set to the empty dictionary. You can use this parameter to find paths that avoid one node by setting `genera_max_visitations={"AvoidNode":0}`. You can also use it to find cycles by setting the same starting and ending node and allowing to visit it two times. There is an specific method to find cycles.
+* `max_iter`: A non negative integer that limits the number of iterations of the search algorithm. The algorithm should always finish, but for large and complex paths it can take a lot of iterations. You can use this parameter to limit the amount of iterations to perform. By default is set to the factorial of the number of nodes in the graph. A warning will be raised if the maximum number of iterations is reached.
+* `max_paths`: A non negative integer that limits the number of paths that the method will return. By default is set to infinity, so it will return all the possible paths. If you are interested in finding only one path you can set this parameter to one and the algorithm will finish after finding it.
+
+The result of this method will be a list of `Paths` objects, which is just a direct subclass of `list[str]` that is used to represent a path. If no path was found the result will be an empty list.
 
 ```python
 dictionary = {
-    "A": {"B": 1.0, "C": 2.5},
-    "B": {"C": 2.5},
-    "C": {"A": 1 / 2.5, "D": 1.3},
-    "D": {"E": 3.4},
-    "E": {"C": 1 / (1.3 * 3.4), "A": 13.0},
+    "A": {"B": 1},
+    "B": {"C": 2.5, "A": 1},
+    "C": {},
     "Z": {},
 }
 graph = WeightedDirectedGraph.from_dict(dictionary)
 
-graph.find_path("A", "B")
-# ["A", "B]
+graph.find_paths("A", "B")
+# [["A", "B]]
 
-graph.find_path("A", "Z")
+graph.find_paths("A", "Z")
 # []
 
-graph.find_path("A", "E")
-# ["A", "C", "D", "E"]
+graph.find_paths("A", "C")
+# [["A", "B", "C"]]
+
+graph.find_paths("A", "A")
+# [["A"]]
+
+graph.find_paths("A", "A", general_max_visitations=2)
+# [['A'], ['A','B','A'], ['A','B','C','B','A']]
 
-graph.find_path("A", "A")
-# ["A"]
+graph.find_paths("A", "B", general_max_visitations=2)
+# [['A','B'], ['A','B','A','B], ['A','B','C','B']]
+
+graph.find_paths("A", "B", specific_max_visitations={"B":2})
+# [['A','B'], ['A','B','C','B']
 ```
 
-There are also methods to get the weight of following a path. This methods are `path_weight` and `weight_between`. The first one receives a path (a list of consecutive nodes) and returns the weight of the path (the product of the weights). If the given path does not exists an exception will be raised. If the empty path is given the return weight will be `0`. The second method receives the start and end nodes and returns the weight of one of the shortest paths between them. If there is not path between the given nodes the return weight will be `0`. The weight between a node an itself will be `1`. 
+There is also a method to get the weight of following a path. This method is call `path_weight`. It receives a `Path` object or `list[str]` and returns the weight of the path (the product of the weights). You can set a default value (like the python `dict.get`) that will be return if the path is empty. By default it is set to `None`. If the given path does not exists an exception will be raised. If the given path consists of just one node, the identity element of the group (1.0 for standard graphs) will be return.
 
 ```python
-graph.path_weight([])
-# 0.0
+graph.path_weight([], "Helo World")
+# "Helo World"
 
 graph.path_weight(["A", "B"])
 # 1.0
 
 graph.path_weight(["A", "B", "C"])
 # 2.5
 
-grap.weight_between("A", "C")
-# 2.5
-
-grap.weight_between("A", "Z")
-# 0.0
-
-grap.weight_between("A", "A")
+graph.path_weight(["Z"])
 # 1.0
 ```
 
-**WARNING**: Currently, if a path that contains a cycle is given the method `path_weight` will raise an error. In future this behaviour will be change to allow cycles. 
-
 ### Graphs and groups
 
 #### Introduction to the `Group` class
-As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows. 
+
+As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows.
 
 ```python
+import numpy as np
 from pywgraph import Group
 
 group = Group(
     name="R^2 under addition",
     operation=lambda x, y: x + y,
     inverse_function=lambda x: -x,
     identity=np.zeros(2),
     hash_function=lambda x: hash(tuple(x))
 )
 ```
 
-This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. 
+You can also provide a check function that checks if an object belongs to the group. In the above case, a checker function could be defined by:
+
+```python
+def r_2_check(weight: Any) -> bool:
+    if not isinstance(weight, np.ndarray): 
+        return False
+    if len(weight) != 2:
+        return False
+    if not all(isinstance(x, (int, float)) for x in weight):
+        return False
+    return True
+```
+
+This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. If provided a check function, you can check if an object belongs to the group with the method `Group.check`.
 
 ```python
 import numpy as np 
 vector_1 = np.array([1, 3])
 vector_2 = np.arra([-1, 7])
 
 group(vector_1, vector_2)
 # np.array([0, 10])
 
 group.operation(vector_1, vector_2)
 # np.array([0, 10])
 
-group.inverse_operation(vector_1, vector_2)
-# np.array([2, -4])
+group.inverse(vector_1)
+# np.array([-1, -3])
 
-group.neutral_element
+group.identity
 # np.array([0, 0])
+
+group.check(vector_1)
+# True
+
+group.check(23)
+# False
 ```
 
 #### General weights for edges
 
 Now that we introduce how to construct a group we will se how to use it to provide elements of an arbitrary group as weights of an edge. To do so you just need to create the group and add it as a parameter in the constructor of edge.
 
 ```python
@@ -186,28 +234,28 @@
     hash_function=lambda x: hash(tuple(x))
 )
 weight_of_edge = np.array([1, 2])
 
 edge = WeightedDirectedEdge("A", "B", weight_of_edge, group)
 ```
 
-With the group information given, now this edge instance knows how to construct the inverse edge. 
+With the group information given, now this edge instance knows how to construct the inverse edge.
 
 ```python
 edge.inverse
 # WeightedDirectedEdge("B", "A", np.array([-1, -2]), group)
 ```
 
-Is important to notice that there is no checking of wether the provide weight is a valid element of the given group. In the future there will be an option to implement an element checker in the group definition. 
+Is important to notice that there is no checking of wether the provide weight is a valid element of the given group.
 
 #### General weighted graphs
 
-Now for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter. 
+Now, for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter.
 
-With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method. 
+With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method.
 
 ```python
 from pywgraph import WeightedDirectedGraph, Group
 import numpy as np 
 group = Group(
     "R^2 under addition",
     lambda x, y: x + y,
@@ -228,34 +276,35 @@
 # Creates the graph
 
 graph.path_weight(["A", "C"])
 # np.array([-1, 3.4])
 
 graph.path_weight(["A", "B", "C"])
 # np.array([1, 2.5]) + np.array([2.5, -1]) = np.array([3.5, 1.5])
-
-graph.weight_between("A", "C")
-# np.array([-1, 3.4])
-
-graph.weight_between("A", "Z")
-# np.array([0, 0])
-
-graph.weight_between("A", "Z")
-# None
-
-graph.weight_between("A", "Z", np.array([1,1]))
-# np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
-- Added a method to `WeightedDirectedGraph` to add a new node. 
-- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+* Added a method to `WeightedDirectedGraph` to add a new node.
+* Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
 
 ### Version 1.0.2 (2024-05-09)
 
-- Added a method to `WeightedDirectedGraph` to remove a node. 
-- Added a method to `WeightedDirectedGraph` to remove an edge. 
+* Added a method to `WeightedDirectedGraph` to remove a node.
+* Added a method to `WeightedDirectedGraph` to remove an edge.
+
+### Version 1.1.0 (2024-05-15)
+
+* The `Group` class now has a `group_checker` optional parameter that consists of a function to check wether an element belongs to the group or not.
+
+* Add the method `WeightedDirectedGraph.find_paths` to find all paths between two given nodes.
+* The method `WeightedDirectedGraph.find_path` is deprecated and will be removed, use `find_paths` with `max_paths=1` to replicate `WeightedDirectedGraph.find_path` behaviour.
+* Add `Path` and `Cycle` classes to represent an abstraction of a node path and a node cycle.
+* Add method `WeightedDirectedGraph.get_node_cycles` to find all cycles that contains the node.
+* Add property `WeightedDirectedGraph.cycles` that returns the set of all simple cycles of the graph.
+* Add the property `WeightedDirectedGraph.is_conmutative` that checks it the graph is conmutative.
+* The method `WeightedDirectedGraph.weight_between` is deprecated and will be removed. Combine `WeightedDirectedGraph.find_paths` with `WeightedDirectedGraph.path_weight` to replicate `WeightedDirectedGraph.weight_between` behaviour.
+* The behaviour of `WeightedDirectedGraph.add_edge` when no weight and path is given is deprecated and will be removed. Either give a weight or seach for a path.
```

### Comparing `pywgraph-1.0.2/pywgraph/exceptions/_exceptions.py` & `pywgraph-1.1.0/pywgraph/exceptions/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.2/pywgraph/graphs/_edge.py` & `pywgraph-1.1.0/pywgraph/graphs/_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from typing import TypeVar
-from ..groups import Group
+from ..groups import Group, real_multiplicative_group
 
 T = TypeVar("T")
-_default_group = Group(
-    "Real numbers with multiplication", 1.0, lambda x, y: x * y, lambda x: 1 / x
-)
 
 
 class DirectedEdge:
 
     def __init__(self, start: str, end: str) -> None:
         if start == end:
             raise ValueError("Start and end vertices must be different")
@@ -42,17 +39,22 @@
     def __repr__(self) -> str:
         return f"{self._start} -> {self._end}"
 
 
 class WeightedDirectedEdge(DirectedEdge):
 
     def __init__(
-        self, start: str, end: str, weight: T, group: Group = _default_group
+        self,
+        start: str,
+        end: str,
+        weight: T,
+        group: Group = real_multiplicative_group,
     ) -> None:
         super().__init__(start, end)
+
         self._weight = weight
         self._group = group
 
     @property
     def weight(self) -> T:  # type: ignore
         return self._weight
```

### Comparing `pywgraph-1.0.2/pywgraph.egg-info/PKG-INFO` & `pywgraph-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,72 @@
-Metadata-Version: 2.1
-Name: pywgraph
-Version: 1.0.2
-Summary: A python implementation of weighted directed graphs
-Home-page: https://github.com/josek98/pywgraph
-Author: josek98
-Author-email: josemmsscc98@gmail.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Requires-Dist: pytest>=7.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
-
 # pywgraph
-A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group. 
+
+A library to manipulate weighted graphs in python. This library focus on directed graphs whose edges have weights. The weights of the graph can be any elements of a fixed mathematical group. By default, the underlying group is set to be the real numbers with the multiplication. Thus, when trasversing the graph, the weight of the path is the product of the weights of the edges, but in general, it is the product under the binary operation of the group.
 
 For this reason, this package also includes a basic abstraction of a group. The group definition is base on:
-*  The a function of two variables that return one element (the binary operation of the group).
-*  The inverse function of an element. This is, the function that given an element of the group returns it inverse. 
-*  The identity element of the group.
-*  Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one. 
+
+* The a function of two variables that return one element (the binary operation of the group).
+
+* The inverse function of an element. This is, the function that given an element of the group returns its inverse.
+
+* The identity element of the group.
+
+* Optional, a hash function for the elements of the group. By default it is taken the standard python hash function. If your group contains not hashable elements you should provide one.
+
+* [New in `1.1.0`] Optional, a check function to check if an element belongs to the group.
 
 ## QUICKSTART
 
 ### Edges
 
-The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows: 
+The main object to construct the graph is the `WeightedDirectedEdge` class. This represents a directed edge with a weight. The construction basic construction is as follows:
 
 ```python
 from pywgraph import WeightedDirectedEdge
 
 edge = WeightedDirectedEdge("A", "B", 0.5)
 ```
 
-The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication. 
+The first two parameters are the nodes that the edge connects. The last parameter is the weight. It is important to notice that, since this is a directed edge, the order of the nodes is important. Since we do have not specify any group, the default group is the real numbers with the multiplication.
 
 You can call the start and end nodes with `edge.start` and `edge.end`, respectevely. To get the weight, simply use `edge.weight`. You can also get the *inverse edge* with `edge.inverse`. This is, the edge that connects the end node of `edge` to the start node of `edge` and has `1/edge.weight` as weight (as said previously, in the future this is meant to be the inverse of the weight in the underlying group).
 
-Also, this class is hashable and iterable, yielding the start node, end node and weight. 
-
+Also, this class is hashable and iterable, yielding the start node, end node and weight.
 
 ### Graph
 
-The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication. 
+The graph is represented by the `WeightedDirectedGraph` class. This is the main class of the package. The graph itself is a set of nodes and a set of `WeightedDirectedEdge`s. If you don`t specify it, the underlying group for the weights as said would be the real numbers with the multiplication.
 
 It is also possible, and more comfortable, to create the graph using the `WeightedDirectedGraph.from_dict` method, which instantiates the graph from a dictionary. The keys of the dictionary are the starting nodes. The values must consists of another dictionary, where the keys are the ending nodes and the value is the weight of the edge. It is important that all nodes of the graph must be keys in the dictionary. If, for example, there is a node "C" that has no children nodes, then the dictionary must have a key "C" with a value of `{}`.
-As always, if you want to use another group for the weights you should specify it here. 
+As always, if you want to use another group for the weights you should specify it here.
 
 ```python
 from pywgraph import WeightedDirectedGraph
 
 g = WeightedDirectedGraph.from_dict({
     "A": {"B": 0.5},
     "B": {"A": 0.5, "C": 1.0},
     "C": {}
 })
 ```
 
-The equivalent construction using set of nodes and set of edges is as follows: 
+The equivalent construction using set of nodes and set of edges is as follows:
 
-```python 
+```python
 from pywgraph import WeightedDirectedGraph
 
 graph = WeightedDirectedGraph(
     nodes={"A", "B", "C"},
     edges={
         WeightedDirectedEdge("A", "B", 0.5),
         WeightedDirectedEdge("B", "A", 0.5),
         WeightedDirectedEdge("B", "C", 1.0)
     }
 )
-``` 
+```
 
 You can instantiate a bad define graph by not writting all the nodes that appear in the edges in the nodes set. There is a method `check_defintion` that checks if the graph is well defined, but the check is not enforce. You can retrieve the nodes and edges by `graph.nodes` and `graph.edges`, respectively.
 
 You can also acces the children and the parents of a nodes with the methods `children` and `parents`, respectively.
 
 ```python
 graph.children("A")
@@ -82,110 +75,139 @@
 graph.parents("A")
 # {}
 
 graph.children("B")
 # {"A", "C"}
 ```
 
-The main use of this graph object is to work with their weights as group elements, so you should not add the reverse edge of an existing edge with a bad inverse weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`. 
+The main use of this graph object is to work with their weights as group elements, so normally, you want that reverse edges of existing ones have the inverse weight of the existing edge weight. For this, there is the method `add_reverse_edges` that returns a new graph with the original graph with all the reverse edges added. You can also modify the graph directly with the paremeter `inplace=True`.
 
 ```python
 graph_w_inverse_edges = graph.add_reverse_edges()
 
 # Updating the graph 
 graph.add_reverse_edges(inplace=True)
 ```
 
 ### Path finding
 
-There is a method `find_path` that finds one of the shortest path between two nodes. This method returns a list of edges that represents the path. The method has two parameters: `start` and `end`. Both must be nodes of the graph. If not, an error is raised. If there is not path between the given nodes the empty list will be return. 
+There is a method `find_paths` that finds all paths between two gven nodes. This method have many options to modify the behaviour of the search. Its parameters are:
+
+* `start`: The node of the graph where the algorithm starts the search.
+* `end`: The target node of the graph to reach.
+* `general_max_visitations`: A non negative integer that specifies the maximum number of times that nodes can be visited along the path. By default is set to one.
+* `specific_max_visitations`: A dictionary whose keys are nodes and values are non negative integers. This specifies the maximum number of times that the key node can be visited along the path, overriding what is set in the `genera_max_visitations` parameter. By default is set to the empty dictionary. You can use this parameter to find paths that avoid one node by setting `genera_max_visitations={"AvoidNode":0}`. You can also use it to find cycles by setting the same starting and ending node and allowing to visit it two times. There is an specific method to find cycles.
+* `max_iter`: A non negative integer that limits the number of iterations of the search algorithm. The algorithm should always finish, but for large and complex paths it can take a lot of iterations. You can use this parameter to limit the amount of iterations to perform. By default is set to the factorial of the number of nodes in the graph. A warning will be raised if the maximum number of iterations is reached.
+* `max_paths`: A non negative integer that limits the number of paths that the method will return. By default is set to infinity, so it will return all the possible paths. If you are interested in finding only one path you can set this parameter to one and the algorithm will finish after finding it.
+
+The result of this method will be a list of `Paths` objects, which is just a direct subclass of `list[str]` that is used to represent a path. If no path was found the result will be an empty list.
 
 ```python
 dictionary = {
-    "A": {"B": 1.0, "C": 2.5},
-    "B": {"C": 2.5},
-    "C": {"A": 1 / 2.5, "D": 1.3},
-    "D": {"E": 3.4},
-    "E": {"C": 1 / (1.3 * 3.4), "A": 13.0},
+    "A": {"B": 1},
+    "B": {"C": 2.5, "A": 1},
+    "C": {},
     "Z": {},
 }
 graph = WeightedDirectedGraph.from_dict(dictionary)
 
-graph.find_path("A", "B")
-# ["A", "B]
+graph.find_paths("A", "B")
+# [["A", "B]]
 
-graph.find_path("A", "Z")
+graph.find_paths("A", "Z")
 # []
 
-graph.find_path("A", "E")
-# ["A", "C", "D", "E"]
+graph.find_paths("A", "C")
+# [["A", "B", "C"]]
+
+graph.find_paths("A", "A")
+# [["A"]]
+
+graph.find_paths("A", "A", general_max_visitations=2)
+# [['A'], ['A','B','A'], ['A','B','C','B','A']]
 
-graph.find_path("A", "A")
-# ["A"]
+graph.find_paths("A", "B", general_max_visitations=2)
+# [['A','B'], ['A','B','A','B], ['A','B','C','B']]
+
+graph.find_paths("A", "B", specific_max_visitations={"B":2})
+# [['A','B'], ['A','B','C','B']
 ```
 
-There are also methods to get the weight of following a path. This methods are `path_weight` and `weight_between`. The first one receives a path (a list of consecutive nodes) and returns the weight of the path (the product of the weights). If the given path does not exists an exception will be raised. If the empty path is given the return weight will be `0`. The second method receives the start and end nodes and returns the weight of one of the shortest paths between them. If there is not path between the given nodes the return weight will be `0`. The weight between a node an itself will be `1`. 
+There is also a method to get the weight of following a path. This method is call `path_weight`. It receives a `Path` object or `list[str]` and returns the weight of the path (the product of the weights). You can set a default value (like the python `dict.get`) that will be return if the path is empty. By default it is set to `None`. If the given path does not exists an exception will be raised. If the given path consists of just one node, the identity element of the group (1.0 for standard graphs) will be return.
 
 ```python
-graph.path_weight([])
-# 0.0
+graph.path_weight([], "Helo World")
+# "Helo World"
 
 graph.path_weight(["A", "B"])
 # 1.0
 
 graph.path_weight(["A", "B", "C"])
 # 2.5
 
-grap.weight_between("A", "C")
-# 2.5
-
-grap.weight_between("A", "Z")
-# 0.0
-
-grap.weight_between("A", "A")
+graph.path_weight(["Z"])
 # 1.0
 ```
 
-**WARNING**: Currently, if a path that contains a cycle is given the method `path_weight` will raise an error. In future this behaviour will be change to allow cycles. 
-
 ### Graphs and groups
 
 #### Introduction to the `Group` class
-As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows. 
+
+As said in the introduction, there is also an abstraction of a mathematical group. This object is call simply `Group`. To initialize it you need to provide a description of the group (string), the binary operation, the inverse operation and the identity element. If the elements of the group are not hashable, you should provide a hash function. One example could be an implementation of $\mathbb{R^2}$ under addition. For this we could represent vectors with numpy arrays, which are not hashable. We can construct this group as follows.
 
 ```python
+import numpy as np
 from pywgraph import Group
 
 group = Group(
     name="R^2 under addition",
     operation=lambda x, y: x + y,
     inverse_function=lambda x: -x,
     identity=np.zeros(2),
     hash_function=lambda x: hash(tuple(x))
 )
 ```
 
-This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. 
+You can also provide a check function that checks if an object belongs to the group. In the above case, a checker function could be defined by:
+
+```python
+def r_2_check(weight: Any) -> bool:
+    if not isinstance(weight, np.ndarray): 
+        return False
+    if len(weight) != 2:
+        return False
+    if not all(isinstance(x, (int, float)) for x in weight):
+        return False
+    return True
+```
+
+This group instance is callable. The call gets two variables as inputs and return the operation between them. Since there is no type checking, the user is responsible of using it with valid inputs. You can also call the group operation with the property `Group.operation` and the inverse operation by `Group.inverse_function`. The identity element is stored in the property `Group.identity`. If you need to, you can also get back the hash function with the property `Group.hash_function`. If provided a check function, you can check if an object belongs to the group with the method `Group.check`.
 
 ```python
 import numpy as np 
 vector_1 = np.array([1, 3])
 vector_2 = np.arra([-1, 7])
 
 group(vector_1, vector_2)
 # np.array([0, 10])
 
 group.operation(vector_1, vector_2)
 # np.array([0, 10])
 
-group.inverse_operation(vector_1, vector_2)
-# np.array([2, -4])
+group.inverse(vector_1)
+# np.array([-1, -3])
 
-group.neutral_element
+group.identity
 # np.array([0, 0])
+
+group.check(vector_1)
+# True
+
+group.check(23)
+# False
 ```
 
 #### General weights for edges
 
 Now that we introduce how to construct a group we will se how to use it to provide elements of an arbitrary group as weights of an edge. To do so you just need to create the group and add it as a parameter in the constructor of edge.
 
 ```python
@@ -199,28 +221,28 @@
     hash_function=lambda x: hash(tuple(x))
 )
 weight_of_edge = np.array([1, 2])
 
 edge = WeightedDirectedEdge("A", "B", weight_of_edge, group)
 ```
 
-With the group information given, now this edge instance knows how to construct the inverse edge. 
+With the group information given, now this edge instance knows how to construct the inverse edge.
 
 ```python
 edge.inverse
 # WeightedDirectedEdge("B", "A", np.array([-1, -2]), group)
 ```
 
-Is important to notice that there is no checking of wether the provide weight is a valid element of the given group. In the future there will be an option to implement an element checker in the group definition. 
+Is important to notice that there is no checking of wether the provide weight is a valid element of the given group.
 
 #### General weighted graphs
 
-Now for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter. 
+Now, for constructing a weighted directed graph whose weights are elements of a specific group you just need to define the group and create the graph adding the group as parameter. The edges of the graph need to include the group as well, as seen before. A better way to construct the graph is to use the method `WeightedDirectedGraph.from_dict`. Now this works exactly the same but adding the group as a new parameter.
 
-With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method. 
+With this implementation any method that concerns weights uses the group operation to handle it. For example, the weight of a given path that the `WeightedDirectedGraph.path_weight` yields is obtain with the consecutive application of the group operation. The same happens with the `WeightedDirectedGraph.weight_between` method.
 
 ```python
 from pywgraph import WeightedDirectedGraph, Group
 import numpy as np 
 group = Group(
     "R^2 under addition",
     lambda x, y: x + y,
@@ -241,34 +263,35 @@
 # Creates the graph
 
 graph.path_weight(["A", "C"])
 # np.array([-1, 3.4])
 
 graph.path_weight(["A", "B", "C"])
 # np.array([1, 2.5]) + np.array([2.5, -1]) = np.array([3.5, 1.5])
-
-graph.weight_between("A", "C")
-# np.array([-1, 3.4])
-
-graph.weight_between("A", "Z")
-# np.array([0, 0])
-
-graph.weight_between("A", "Z")
-# None
-
-graph.weight_between("A", "Z", np.array([1,1]))
-# np.array([1,1])
 ```
 
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
-- Added a method to `WeightedDirectedGraph` to add a new node. 
-- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+* Added a method to `WeightedDirectedGraph` to add a new node.
+* Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights.
 
 ### Version 1.0.2 (2024-05-09)
 
-- Added a method to `WeightedDirectedGraph` to remove a node. 
-- Added a method to `WeightedDirectedGraph` to remove an edge. 
+* Added a method to `WeightedDirectedGraph` to remove a node.
+* Added a method to `WeightedDirectedGraph` to remove an edge.
+
+### Version 1.1.0 (2024-05-15)
+
+* The `Group` class now has a `group_checker` optional parameter that consists of a function to check wether an element belongs to the group or not.
+
+* Add the method `WeightedDirectedGraph.find_paths` to find all paths between two given nodes.
+* The method `WeightedDirectedGraph.find_path` is deprecated and will be removed, use `find_paths` with `max_paths=1` to replicate `WeightedDirectedGraph.find_path` behaviour.
+* Add `Path` and `Cycle` classes to represent an abstraction of a node path and a node cycle.
+* Add method `WeightedDirectedGraph.get_node_cycles` to find all cycles that contains the node.
+* Add property `WeightedDirectedGraph.cycles` that returns the set of all simple cycles of the graph.
+* Add the property `WeightedDirectedGraph.is_conmutative` that checks it the graph is conmutative.
+* The method `WeightedDirectedGraph.weight_between` is deprecated and will be removed. Combine `WeightedDirectedGraph.find_paths` with `WeightedDirectedGraph.path_weight` to replicate `WeightedDirectedGraph.weight_between` behaviour.
+* The behaviour of `WeightedDirectedGraph.add_edge` when no weight and path is given is deprecated and will be removed. Either give a weight or seach for a path.
```

### Comparing `pywgraph-1.0.2/pywgraph.egg-info/SOURCES.txt` & `pywgraph-1.1.0/pywgraph.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 README.md
 setup.py
 pywgraph/__init__.py
-pywgraph/_utils.py
+pywgraph/_wrappers.py
 pywgraph.egg-info/PKG-INFO
 pywgraph.egg-info/SOURCES.txt
 pywgraph.egg-info/dependency_links.txt
 pywgraph.egg-info/requires.txt
 pywgraph.egg-info/top_level.txt
 pywgraph/exceptions/__init__.py
 pywgraph/exceptions/_exceptions.py
 pywgraph/graphs/__init__.py
 pywgraph/graphs/_edge.py
 pywgraph/graphs/_graph.py
+pywgraph/graphs/_paths.py
 pywgraph/groups/__init__.py
 pywgraph/groups/_groups.py
+pywgraph/groups/_predefined_groups.py
 tests/__init__.py
 tests/test_directed_edge.py
 tests/test_path_finding.py
+tests/test_path_finding_new.py
+tests/test_paths_and_cycles.py
 tests/test_weighted_directed_edge.py
 tests/test_weighted_directed_graph.py
 tests/test_weighted_directed_graph_arrays.py
```

### Comparing `pywgraph-1.0.2/setup.py` & `pywgraph-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages #type: ignore
 
 with open("README.md", "r",) as f: 
     long_description = f.read()
 
 setup(
     name="pywgraph",
-    version="1.0.2",
+    version="1.1.0",
     description="A python implementation of weighted directed graphs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="josek98",
     author_email="josemmsscc98@gmail.com",
     url="https://github.com/josek98/pywgraph",
     packages=find_packages(),
```

### Comparing `pywgraph-1.0.2/tests/test_directed_edge.py` & `pywgraph-1.1.0/tests/test_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.2/tests/test_weighted_directed_edge.py` & `pywgraph-1.1.0/tests/test_weighted_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.2/tests/test_weighted_directed_graph.py` & `pywgraph-1.1.0/tests/test_weighted_directed_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,38 @@
     def test_edges(self):
         assert graph().edges == {
             WeightedDirectedEdge("A", "B", 7),
             WeightedDirectedEdge("A", "C", 9),
             WeightedDirectedEdge("B", "C", 10),
         }
 
+    @pytest.mark.deprecated
     def test_well_defined(self):
         assert graph().check_definition()
 
+    def test_well_defined_property(self): 
+        assert graph().is_well_defined
+
+    @pytest.mark.deprecated
     def test_bad_defined(self):
         assert (
             WeightedDirectedGraph(
                 {"A"}, {WeightedDirectedEdge("A", "B", 7)}
             ).check_definition()
             == False
         )
 
+    def test_bad_defined_property(self):
+        assert (
+            WeightedDirectedGraph(
+                {"A"}, {WeightedDirectedEdge("A", "B", 7)}
+            ).is_well_defined
+            == False
+        )
+
     def test_children(self):
         assert graph().children("A") == {"B", "C"}
 
     def test_parents(self):
         assert graph().parents("C") == {"A", "B"}
 
     def test_equal(self):
@@ -218,21 +231,23 @@
         new_graph = graph_copy.add_edge(
             start="C", end="B", path=path, inplace=False, allow_inverse=True
         )
         update_dict = _dict_graph.copy()
         update_dict["C"] = update_dict["C"] | {"B": (1/9) * 7}
         assert WeightedDirectedGraph.from_dict(update_dict) == new_graph
 
+    @pytest.mark.deprecated
     def test_add_edge_find_path(self): 
         graph_copy = graph()
         new_graph = graph_copy.add_edge(start="C", end="A", inplace=False, allow_inverse=True)
         update_dict = _dict_graph.copy()
         update_dict["C"] = update_dict["C"] | {"A": 1/9}
         assert WeightedDirectedGraph.from_dict(update_dict) == new_graph
 
+    @pytest.mark.deprecated
     def test_add_edge_find_non_existing_path(self): 
         graph_copy = graph()
         assert graph_copy == graph_copy.add_edge(start="C", end="A", inplace=False, allow_inverse=False)
 
     def test_add_edge_bad_nodes(self): 
         graph_copy = graph()
         with pytest.raises(NodeNotFound):
```

### Comparing `pywgraph-1.0.2/tests/test_weighted_directed_graph_arrays.py` & `pywgraph-1.1.0/tests/test_weighted_directed_graph_arrays.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pywgraph import WeightedDirectedGraph, Group, WeightedDirectedEdge
 import numpy as np
+import pytest
 from typing import Any  # for typing purposes
 
 
 def vector_group_multiplication() -> Group:
     group = Group(
         name="Vectors of dimension 2 with multiplication",
         identity=np.ones(2),
@@ -74,17 +75,21 @@
                 "B", "D", np.array([2, 1]), vector_group_multiplication()
             ),
             WeightedDirectedEdge(
                 "C", "D", np.array([-1, 1]), vector_group_multiplication()
             ),
         }
 
+    @pytest.mark.deprecated
     def test_well_defined(self):
         assert multiplication_graph().check_definition()
 
+    def test_well_defined_property(self):
+        assert multiplication_graph().is_well_defined
+
     def test_fill_reverse_edge_multiplication(self):
         complete_dict = _array_dict_graph.copy()
         complete_dict["B"] = complete_dict["B"] | {"A": np.array([1, 1 / 2])}
         complete_dict["C"] = complete_dict["C"] | {
             "A": np.array([1 / 3, 1 / 4]),
             "B": np.array([-1 / 5, 1 / 1.3]),
         }
@@ -107,10 +112,8 @@
         complete_dict["D"] = complete_dict["D"] | {
             "B": np.array([-2, -1]),
             "C": np.array([1, -1]),
         }
         filled_graph = WeightedDirectedGraph.from_dict(
             complete_dict, vector_group_addition()
         )
-        print(filled_graph)
-        print(addition_graph().add_reverse_edges())
         assert filled_graph == addition_graph().add_reverse_edges()
```

