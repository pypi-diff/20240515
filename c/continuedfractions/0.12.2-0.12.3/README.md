# Comparing `tmp/continuedfractions-0.12.2.tar.gz` & `tmp/continuedfractions-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.2.tar", last modified: Tue May 14 21:50:21 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.3.tar", last modified: Wed May 15 06:24:17 2024, max compression
```

## Comparing `continuedfractions-0.12.2.tar` & `continuedfractions-0.12.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.2/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.2/LICENSE
--rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.2/README.md
--rw-r--r--   0        0        0     3162 2024-05-14 16:54:10.646159 continuedfractions-0.12.2/README.md
--rw-r--r--   0        0        0     3506 2024-05-14 21:50:21.330172 continuedfractions-0.12.2/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.2/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.2/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40723 2024-05-14 21:10:28.678283 continuedfractions-0.12.2/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.2/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-14 18:44:49.078520 continuedfractions-0.12.2/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.3/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.3/LICENSE
+-rw-r--r--   0        0        0     3159 2024-05-15 05:58:00.271106 continuedfractions-0.12.3/README.md
+-rw-r--r--   0        0        0     3159 2024-05-15 05:58:00.271106 continuedfractions-0.12.3/README.md
+-rw-r--r--   0        0        0     3506 2024-05-15 06:24:17.210703 continuedfractions-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.3/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.3/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40745 2024-05-15 06:11:07.304519 continuedfractions-0.12.3/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.3/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-14 22:03:02.380992 continuedfractions-0.12.3/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24143 1970-01-01 00:00:00.000000 continuedfractions-0.12.3/PKG-INFO
```

### Comparing `continuedfractions-0.12.2/LICENSE` & `continuedfractions-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.2/README.md` & `continuedfractions-0.12.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 pip install continuedfractions
 ```
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
-The `continuedfractions` package is designed to:
+The `continuedfractions` package is designed for:
 
-* make it easy to work with (finite) continued fractions as Python objects
-* explore their key properties, such as elements/coefficients, convergents, segments, remainders, and others
-* operate on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
-* support approximations and experimental computations for irrational numbers
-* explore other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
+* working with (finite) continued fractions as Python objects
+* exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
+* operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
+* supporting approximations and experimental computations for irrational numbers
+* exploring other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

#### html2text {}

```diff
@@ -25,17 +25,16 @@
 the [API reference](https://continuedfractions.readthedocs.io/en/latest/
 sources/api-reference.html). [Continued fractions](https://en.wikipedia.org/
 wiki/Continued_fraction) are beautiful and interesting mathematical objects,
 with many connections in [number theory](https://en.wikipedia.org/wiki/
 Number_theory) and also very useful practical applications, including the
 [rational approximation of real numbers](https://en.wikipedia.org/wiki/
 Continued_fraction#Best_rational_approximations). The `continuedfractions`
-package is designed to: * make it easy to work with (finite) continued
-fractions as Python objects * explore their key properties, such as elements/
-coefficients, convergents, segments, remainders, and others * operate on them
-as rationals and instances of the standard library [`fractions.Fraction`]
-(https://docs.python.org/3/library/fractions.html#fractions.Fraction) class *
-support approximations and experimental computations for irrational numbers *
-explore other objects related to continued fractions, such as mediants,
-sequences of coprime integers, and Farey sequences The project is [licensed]
-(LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/
-licenses/MPL-2.0).
+package is designed for: * working with (finite) continued fractions as Python
+objects * exploring their key properties, such as elements/coefficients,
+convergents, segments, remainders, and others * operating on them as rationals
+and instances of the standard library [`fractions.Fraction`](https://
+docs.python.org/3/library/fractions.html#fractions.Fraction) class * supporting
+approximations and experimental computations for irrational numbers * exploring
+other objects related to continued fractions, such as mediants, sequences of
+coprime integers, and Farey sequences The project is [licensed](LICENSE) under
+the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

### Comparing `continuedfractions-0.12.2/pyproject.toml` & `continuedfractions-0.12.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.2"
+version = "0.12.3"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.2/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.3/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.2/src/continuedfractions/lib.py` & `continuedfractions-0.12.3/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.2/src/continuedfractions/sequences.py` & `continuedfractions-0.12.3/src/continuedfractions/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
        (a^\\prime, b^\\prime) = \\begin{cases}
                                 (2a - b, a), \\hskip{3em} \\text{ branch #} 1 \\\\
                                 (2a + b, a), \\hskip{3em} \\text{ branch #} 2 \\\\
                                 (a + 2b, b), \\hskip{3em} \\text{ branch #} 3                   
                                 \\end{cases}
 
-    where :math:`1 \\leq b < a`.
+    where :math:`1 \\leq b < a` and :math:`(a, b) = 1`.
 
     Generating coprime pairs can then be implemented by a generative search
     procedure that starts separately from the parents :math:`(2, 1)` and
     :math:`(3, 1)`, and applies the functions given by the mappings below to
     each parent:
 
     .. math::
@@ -594,15 +594,15 @@
         :math:`(3, 1)`, but can be any of their successor nodes.
 
         It is required that :math:`n \\geq 2`, otherwise a
         :py:class:`ValueError` is raised.
 
         The search implementation is an iterative version of a backtracking
         depth-first branch-and-bound search (DFS), in which nodes are traversed
-        in pre-order, NLMR (root -> left -> mid -> right) and bounds and checks
+        in NLMR pre-order (root -> left -> mid -> right) and bounds and checks
         are applied to the nodes, before further traversal or backtracking:
         
         #. Visit the current node :math:`(a, b)` and check :math:`a \\leq n`.
         #. If the check is successful iteratively traverse the current node's
            first child and its children, then the second child and its 
            children, and then the third child and its children, applying the
            check :math:`a \\leq n` to each visited node.
```

### Comparing `continuedfractions-0.12.2/src/continuedfractions/utils.py` & `continuedfractions-0.12.3/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.2/PKG-INFO` & `continuedfractions-0.12.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.2
+Version: 0.12.3
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -422,18 +422,18 @@
 pip install continuedfractions
 ```
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
-The `continuedfractions` package is designed to:
+The `continuedfractions` package is designed for:
 
-* make it easy to work with (finite) continued fractions as Python objects
-* explore their key properties, such as elements/coefficients, convergents, segments, remainders, and others
-* operate on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
-* support approximations and experimental computations for irrational numbers
-* explore other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
+* working with (finite) continued fractions as Python objects
+* exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
+* operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
+* supporting approximations and experimental computations for irrational numbers
+* exploring other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

