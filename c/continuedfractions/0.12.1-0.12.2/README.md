# Comparing `tmp/continuedfractions-0.12.1.tar.gz` & `tmp/continuedfractions-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.1.tar", last modified: Tue May 14 17:14:45 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.2.tar", last modified: Tue May 14 21:50:21 2024, max compression
```

## Comparing `continuedfractions-0.12.1.tar` & `continuedfractions-0.12.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.1/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.1/LICENSE
--rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.1/README.md
--rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.1/README.md
--rw-r--r--   0        0        0     3506 2024-05-14 17:14:45.815444 continuedfractions-0.12.1/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.1/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.1/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40513 2024-05-14 17:09:06.012944 continuedfractions-0.12.1/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.1/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-14 17:08:51.169656 continuedfractions-0.12.1/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.2/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.2/LICENSE
+-rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.2/README.md
+-rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.2/README.md
+-rw-r--r--   0        0        0     3506 2024-05-14 21:50:21.330172 continuedfractions-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.2/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.2/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40723 2024-05-14 21:10:28.678283 continuedfractions-0.12.2/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.2/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-14 18:44:49.078520 continuedfractions-0.12.2/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.2/PKG-INFO
```

### Comparing `continuedfractions-0.12.1/LICENSE` & `continuedfractions-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.1/README.md` & `continuedfractions-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.1/pyproject.toml` & `continuedfractions-0.12.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.1"
+version = "0.12.2"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.1/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.2/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.1/src/continuedfractions/lib.py` & `continuedfractions-0.12.2/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.1/src/continuedfractions/sequences.py` & `continuedfractions-0.12.2/src/continuedfractions/sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,47 +269,48 @@
 [coprime_integers(n) for n in range(1, 1001)]
 [coprime_integers(10 ** k) for k in range(4, 8)]
 
 
 class KSRMTree:
     """An implicit/generative tree class implementation of the Kanga-Saunders-Randall-Mitchell (KSRM) disjointed ternary tree for pairs of (positive) coprime integers.
 
-    The term "KSRM tree" is the author's, and refers to a single tree
-    that combines the trees presented in the following papers:
+    The term "KSRM trees" is the author's, and refers to the trees presented in the following papers:
 
-    #. A. R. Kanga, *The Family Tree of Pythagorean Triplets*, Bulletin of the Institute of Mathematics and Its Applications **26**, 15 (1990).
-    #. R. Saunders and T. Randall, *The Family Tree of the Pythagorean Triplets Revisited*, The Mathematical Gazette **78**, 190 (1994).
-    #. D. W. Mitchell, *An Alternative Characterisation of All Primitive Pythagorean Triples*, The Mathematical Gazette **85**, 273 (2001).
+    * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
+    * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
+    * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
 
     .. note::
 
-       The author could not access the Kanga paper, but the core result is
-       described clearly in the papers of Saunders and Randall, and of
+       The class is named ``KSRMTree`` purely for convenience, but it is
+       actually a representation of two (ternary) subtrees.
+
+    .. note::
+
+       The author could not access the Kanga paper online, but the core result
+       is described clearly in the papers of Saunders and Randall, and of
        Mitchell.
 
-    The trees presented in these papers are directly related to so-called
-    `primitive Pythagorean triples <https://en.wikipedia.org/wiki/Pythagorean_triple#Elementary_properties_of_primitive_Pythagorean_triples>`_,
+    These trees are directly related to so-called `primitive Pythagorean triples <https://en.wikipedia.org/wiki/Pythagorean_triple#Elementary_properties_of_primitive_Pythagorean_triples>`_,
     but have a fundamental consequence for the generation of coprime pairs: all
     pairs of (positive) coprime integers :math:`(a, b)`, where
-    :math:`1 \\leq b < a`, can be represented as nodes in a disjoint ternary
-    tree, with two "parents" (root nodes), :math:`(2, 1)` and :math:`(3, 1)`,
-    in which each parent node has exactly three child nodes of the form:
+    :math:`1 \\leq b < a`, can be represented as nodes in one of two ternary
+    trees, the first which has the "parent" node :math:`(2, 1)` and the second
+    which has the parent node :math:`(3, 1)`. Each node has three children
+    given by the relations:
 
     .. math::
 
        (a^\\prime, b^\\prime) = \\begin{cases}
                                 (2a - b, a), \\hskip{3em} \\text{ branch #} 1 \\\\
                                 (2a + b, a), \\hskip{3em} \\text{ branch #} 2 \\\\
                                 (a + 2b, b), \\hskip{3em} \\text{ branch #} 3                   
                                 \\end{cases}
 
-    where :math:`1 \\leq b < a`, with two pairs of initial values given by
-    :math:`(a=2, b=1)`, and :math:`(a=3, b=1)`. Each node in the tree is the
-    parent of all nodes that branch from it, but the nodes :math:`(2, 1)` and
-    :math:`(3, 1)` are canonical.
+    where :math:`1 \\leq b < a`.
 
     Generating coprime pairs can then be implemented by a generative search
     procedure that starts separately from the parents :math:`(2, 1)` and
     :math:`(3, 1)`, and applies the functions given by the mappings below to
     each parent:
 
     .. math::
@@ -324,22 +325,22 @@
     repeated ad infinitum as required.
 
     .. note::
 
        The tree starting at the root :math:`(3, 1)` will only contain pairs of
        odd coprimes, under the maps described above.
 
-    If we let :math:`k = 1` denote the 1st generation consisting only of the
-    two roots :math:`(2, 1)` and :math:`(3, 1)`, then the :math:`k`-th
-    generation for either tree will have a total of :math:`3^{k - 1}`
-    children, the total number of all members up to and including the
-    :math:`k`-generation will be
-    :math:`1 + 3 + 3^2 + \\ldots 3^{k - 1} = \\frac{3^k - 1}{2}`, and the
+    If we let :math:`k = 0` denote the :math:`0`-th generation consisting only
+    of the two roots :math:`(2, 1)` and :math:`(3, 1)`, then for
+    :math:`k \\geq 1` the :math:`k`-th generation, for either tree, will have a
+    total of :math:`3^k` children, the total number of all members up to and
+    including the :math:`k`-th generation will be
+    :math:`1 + 3 + 3^2 + \\ldots + 3^k = \\frac{3^{k + 1} - 1}{2}`, and the
     total number of all members in both trees up to and including the
-    :math:`k`-th generation will be :math:`3^k - 1`.
+    :math:`k`-th generation will be :math:`3^{k + 1} - 1`.
 
     The number of coprime pairs generated for a given :math:`n \\geq 1` is
     given by:
 
     .. math::
 
        \\phi(1) + \\phi(2) + \\cdots + \\phi(n) = \\sum_{k = 1}^n \\phi(k)
@@ -377,48 +378,48 @@
             NamedCallableProxy(lambda x, y: (x + 2 * y, y), name="KSRM tree branch #3: (x, y) |--> (x + 2y, y)")
         )
 
         return self
 
     @property
     def roots(self) -> Literal[tuple([(2, 1), (3, 1)])]:
-        """:py:class:`tuple`: The tuple of roots of the KSRM tree, which are :math:`(2, 1)` and :math:`(3, 1)`.
+        """:py:class:`tuple`: The tuple of roots of the KSRM trees, which are :math:`(2, 1)` and :math:`(3, 1)`.
 
         For more details see the following papers:
 
-        #. A. R. Kanga, *The Family Tree of Pythagorean Triplets*, Bulletin of the Institute of Mathematics and Its Applications **26**, 15 (1990).
-        #. R. Saunders and T. Randall, *The Family Tree of the Pythagorean Triplets Revisited*, The Mathematical Gazette **78**, 190 (1994).
-        #. D. W. Mitchell, *An Alternative Characterisation of All Primitive Pythagorean Triples*, The Mathematical Gazette **85**, 273 (2001).
+        * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
+        * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
+        * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
 
         Examples
         --------
         >>> KSRMTree().roots
         ((2, 1), (3, 1))
         """
         return self._roots
 
     @property
     def branches(self) -> tuple[KSRMBranch]:    # noqa: F821
-        """:py:class:`tuple`: The tuple of three branch generating functions of the KSRM tree.
+        """:py:class:`tuple`: The tuple of three branch generating functions of the KSRM trees.
 
         There are three branch generating functions, given by the mappings:
 
         .. math::
 
            \\begin{align}
            (a, b) &\\longmapsto (2a - b, a) \\\\
            (a, b) &\\longmapsto (2a + b, a) \\\\
            (a, b) &\\longmapsto (a + 2b, b)
            \\end{align}
 
         For more details see the following papers:
 
-        #. A. R. Kanga, *The Family Tree of Pythagorean Triplets*, Bulletin of the Institute of Mathematics and Its Applications **26**, 15 (1990).
-        #. R. Saunders and T. Randall, *The Family Tree of the Pythagorean Triplets Revisited*, The Mathematical Gazette **78**, 190 (1994).
-        #. D. W. Mitchell, *An Alternative Characterisation of All Primitive Pythagorean Triples*, The Mathematical Gazette **85**, 273 (2001).
+        * Kanga, A. R. (1990). The Family Tree of Pythagorean Triplets. The Mathematical Gazette, 26(15), 15-17.
+        * Mitchell, D. W. (2001). An Alternative Characterisation of All Primitive Pythagorean Triples. The Mathematical Gazette, 85(503), 273-275. https://doi.org/10.2307/3622017
+        * Saunders, R., & Randall, T. (1994). The family tree of the Pythagorean triplets revisited. The Mathematical Gazette, 78(482), 190-193. https://doi.org/10.2307/3618576
 
         Examples
         --------
         Generating the first two generations of children for the parent
         :math:`(2, 1)`.
 
         >>> tree = KSRMTree()
@@ -455,29 +456,29 @@
         self,
         n: int,
         visited: list[tuple[KSRMNode, KSRMBranch]],     # noqa: F821
         /,
         *,
         node_bound: int = None
     ) -> tuple[KSRMNode, KSRMBranch, int, KSRMBranch]:  # noqa: F821
-        """Backtracks on the KSRM coprime pairs tree.
+        """Backtracks on the KSRM coprime pairs trees.
 
-        A private function that backtracks on the KSRM coprime pairs tree: the
+        A private function that backtracks on the KSRM coprime pairs trees: the
         procedure is that, given a (positive) integer :math:`n > 2`, for which
         coprime pairs are being sought, and a sequence (list) of pairs of
         visited nodes and their associated generating branches in the KSRM
         tree, and assuming that the last element of the visited sequence
         contains the node that "failed", the function identifies the nearest
         previously visited node whose first component satisifes the test
         :math:`< n` **and** and whose associated generating branch is not equal
         to the third branch given by :math:`(x, y) \\longmapsto (x + 2y, y)`.
 
         .. note::
 
-           One key property of the KSRM tree is that, for a given search value
+           One key property of the KSRM trees is that, for a given search value
            :math:`n`, if the current node is :math:`(a, b) = (n, b)` and the
            successor node on the first branch, :math:`(2a - b, a)`, fails the
            test :math:`2a - b \\leq n`, then so will the successor nodes on
            the second and third branches.
 
            This means in the case of a node failure in the search on the first
            branch, all three branches of the predecessor node of the failed
@@ -583,15 +584,15 @@
             last_branch = visited[cur_index + 1][1]
 
         # Return the current node, generating branch, index and the generating
         # branch of the last visited node before the current node.
         return cur_node, cur_branch, cur_index, last_branch
 
     def search_root(self, n: int, root: KSRMNode, /) -> Generator[KSRMNode, None, None]:
-        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs tree from the given root node to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
+        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs trees from the given root node to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
 
         The given root node need not be the canonical roots, :math:`(2, 1)`,
         :math:`(3, 1)`, but can be any of their successor nodes.
 
         It is required that :math:`n \\geq 2`, otherwise a
         :py:class:`ValueError` is raised.
 
@@ -611,15 +612,15 @@
            nodes after the backtracked target node and leading up to the failed
            node, including the failed node. By design the backtracked target
            node will have untraversed children on at least one branch, and the
            traversal can begin again, as described above.
 
         .. note::
 
-           One key property of the KSRM tree used in this implementation is
+           One key property of the KSRM trees used in this implementation is
            that for a given integer :math:`n \\geq 1`, if the current node is
            :math:`(a, b) = (n, b)` and the child node on the first branch,
            :math:`(2a - b, a)`, fails the test :math:`2a - b \\leq n`, then
            so will the child nodes on the second and third branches, and
            thus all three children can be pruned.
 
         Parameters
@@ -750,15 +751,15 @@
                 continue
 
         # Not strictly required, but this has been inserted to make
         # debugging easier.
         return
 
     def search(self, n: int, /) -> Generator[KSRMNode, None, None]:
-        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs tree to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
+        """Backtracking depth-first branch-and-bound search (in pre-order, NLMR) of the KSRM coprime pairs trees to find all pairs of coprime (positive) integers not exceeding the given integer :math:`n \\geq 1`.
     
         See the :py:meth:`~continuedfractions.sequences.KSRMTree.search_root`
         method for details of the implementation for the root-based search.
 
         This method mainly calls the root-based search method for the two
         canonical roots :math:`(2, 1)` and :math:`(3, 1)`.
 
@@ -814,16 +815,18 @@
             yield from tuple(product([n], coprime_integers(n)))
 
 
 @functools.cache
 def coprime_pairs(n: int, /) -> tuple[KSRMNode]:
     """A function wrapper to return a sequence (tuple) of all pairs of (positive) coprime integers :math:`<= n`.
 
-    Calls the :py:meth:`continuedfractions.sequences.KSRMTree.search` to
-    perform the search.
+    Calls the KSRM tree :py:meth:`~continuedfractions.sequences.KSRMTree.search`
+    to perform the search up to :math:`n - 1` and then uses
+    :py:func:`~continuedfractions.sequences.coprime_integers` for the search
+    for pairs involving :math:`n`.
 
     A :py:class:`ValueError` is raised if ``n`` is not an :py:class:`int`
     or is an :py:class:`int` less than :math:`1`.
 
     Parameters
     ----------
     n : int
```

### Comparing `continuedfractions-0.12.1/src/continuedfractions/utils.py` & `continuedfractions-0.12.2/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.1/PKG-INFO` & `continuedfractions-0.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.1
+Version: 0.12.2
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
```

