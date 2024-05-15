# Comparing `tmp/quasim-0.1.0.tar.gz` & `tmp/quasim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasim-0.1.0.tar", last modified: Thu May  2 13:45:16 2024, max compression
+gzip compressed data, was "quasim-0.2.0.tar", last modified: Wed May 15 07:03:38 2024, max compression
```

## Comparing `quasim-0.1.0.tar` & `quasim-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-02 13:45:16.489313 quasim-0.1.0/
--rw-r--r--   0 christophstein   (501) staff       (20)     1087 2024-05-02 10:37:17.000000 quasim-0.1.0/LICENSE
--rw-r--r--   0 christophstein   (501) staff       (20)     4792 2024-05-02 13:45:16.488356 quasim-0.1.0/PKG-INFO
--rw-r--r--   0 christophstein   (501) staff       (20)     2711 2024-05-02 13:12:22.000000 quasim-0.1.0/README.md
--rw-r--r--   0 christophstein   (501) staff       (20)     1034 2024-05-02 10:57:15.000000 quasim-0.1.0/pyproject.toml
-drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-02 13:45:16.458072 quasim-0.1.0/quasim/
--rw-r--r--   0 christophstein   (501) staff       (20)       59 2024-05-02 10:57:18.000000 quasim-0.1.0/quasim/__init__.py
--rw-r--r--   0 christophstein   (501) staff       (20)     2480 2024-05-02 13:39:09.000000 quasim-0.1.0/quasim/circuit.py
-drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-02 13:45:16.482032 quasim-0.1.0/quasim/gates/
--rw-r--r--   0 christophstein   (501) staff       (20)      241 2024-04-29 14:09:39.000000 quasim-0.1.0/quasim/gates/__init__.py
--rw-r--r--   0 christophstein   (501) staff       (20)     1140 2024-04-29 09:51:22.000000 quasim-0.1.0/quasim/gates/_matrices.py
--rw-r--r--   0 christophstein   (501) staff       (20)     3692 2024-05-02 13:31:04.000000 quasim-0.1.0/quasim/gates/controlled_gates.py
--rw-r--r--   0 christophstein   (501) staff       (20)     1318 2024-05-02 13:31:52.000000 quasim-0.1.0/quasim/gates/double_controlled_gates.py
--rw-r--r--   0 christophstein   (501) staff       (20)      341 2024-05-02 13:32:20.000000 quasim-0.1.0/quasim/gates/interface.py
--rw-r--r--   0 christophstein   (501) staff       (20)     2996 2024-05-02 13:30:43.000000 quasim-0.1.0/quasim/gates/single_qubit_gates.py
--rw-r--r--   0 christophstein   (501) staff       (20)      640 2024-05-02 13:21:07.000000 quasim-0.1.0/quasim/gates/swap.py
--rw-r--r--   0 christophstein   (501) staff       (20)     5620 2024-05-02 13:34:55.000000 quasim-0.1.0/quasim/gates/utils.py
--rw-r--r--   0 christophstein   (501) staff       (20)     7239 2024-05-02 13:40:48.000000 quasim-0.1.0/quasim/simulator.py
--rw-r--r--   0 christophstein   (501) staff       (20)     1613 2024-05-02 13:42:43.000000 quasim-0.1.0/quasim/utils.py
-drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-02 13:45:16.484089 quasim-0.1.0/quasim.egg-info/
--rw-r--r--   0 christophstein   (501) staff       (20)     4792 2024-05-02 13:45:16.000000 quasim-0.1.0/quasim.egg-info/PKG-INFO
--rw-r--r--   0 christophstein   (501) staff       (20)      482 2024-05-02 13:45:16.000000 quasim-0.1.0/quasim.egg-info/SOURCES.txt
--rw-r--r--   0 christophstein   (501) staff       (20)        1 2024-05-02 13:45:16.000000 quasim-0.1.0/quasim.egg-info/dependency_links.txt
--rw-r--r--   0 christophstein   (501) staff       (20)       96 2024-05-02 13:45:16.000000 quasim-0.1.0/quasim.egg-info/requires.txt
--rw-r--r--   0 christophstein   (501) staff       (20)        7 2024-05-02 13:45:16.000000 quasim-0.1.0/quasim.egg-info/top_level.txt
--rw-r--r--   0 christophstein   (501) staff       (20)       38 2024-05-02 13:45:16.489531 quasim-0.1.0/setup.cfg
+drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-15 07:03:38.613814 quasim-0.2.0/
+-rw-r--r--   0 christophstein   (501) staff       (20)     1087 2024-05-02 10:37:17.000000 quasim-0.2.0/LICENSE
+-rw-r--r--   0 christophstein   (501) staff       (20)     5445 2024-05-15 07:03:38.613299 quasim-0.2.0/PKG-INFO
+-rw-r--r--   0 christophstein   (501) staff       (20)     3364 2024-05-14 13:17:42.000000 quasim-0.2.0/README.md
+-rw-r--r--   0 christophstein   (501) staff       (20)     1034 2024-05-14 13:19:14.000000 quasim-0.2.0/pyproject.toml
+drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-15 07:03:38.594050 quasim-0.2.0/quasim/
+-rw-r--r--   0 christophstein   (501) staff       (20)       59 2024-05-02 10:57:18.000000 quasim-0.2.0/quasim/__init__.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     2480 2024-05-02 13:39:09.000000 quasim-0.2.0/quasim/circuit.py
+drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-15 07:03:38.610911 quasim-0.2.0/quasim/gates/
+-rw-r--r--   0 christophstein   (501) staff       (20)      241 2024-04-29 14:09:39.000000 quasim-0.2.0/quasim/gates/__init__.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     1140 2024-04-29 09:51:22.000000 quasim-0.2.0/quasim/gates/_matrices.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     3692 2024-05-02 13:31:04.000000 quasim-0.2.0/quasim/gates/controlled_gates.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     1318 2024-05-02 13:31:52.000000 quasim-0.2.0/quasim/gates/double_controlled_gates.py
+-rw-r--r--   0 christophstein   (501) staff       (20)      341 2024-05-02 13:32:20.000000 quasim-0.2.0/quasim/gates/interface.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     2996 2024-05-02 13:30:43.000000 quasim-0.2.0/quasim/gates/single_qubit_gates.py
+-rw-r--r--   0 christophstein   (501) staff       (20)      640 2024-05-02 13:21:07.000000 quasim-0.2.0/quasim/gates/swap.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     5620 2024-05-02 13:34:55.000000 quasim-0.2.0/quasim/gates/utils.py
+-rw-r--r--   0 christophstein   (501) staff       (20)    10895 2024-05-14 13:14:03.000000 quasim-0.2.0/quasim/simulator.py
+-rw-r--r--   0 christophstein   (501) staff       (20)     6491 2024-05-14 13:07:57.000000 quasim-0.2.0/quasim/utils.py
+drwxr-xr-x   0 christophstein   (501) staff       (20)        0 2024-05-15 07:03:38.612055 quasim-0.2.0/quasim.egg-info/
+-rw-r--r--   0 christophstein   (501) staff       (20)     5445 2024-05-15 07:03:38.000000 quasim-0.2.0/quasim.egg-info/PKG-INFO
+-rw-r--r--   0 christophstein   (501) staff       (20)      482 2024-05-15 07:03:38.000000 quasim-0.2.0/quasim.egg-info/SOURCES.txt
+-rw-r--r--   0 christophstein   (501) staff       (20)        1 2024-05-15 07:03:38.000000 quasim-0.2.0/quasim.egg-info/dependency_links.txt
+-rw-r--r--   0 christophstein   (501) staff       (20)       96 2024-05-15 07:03:38.000000 quasim-0.2.0/quasim.egg-info/requires.txt
+-rw-r--r--   0 christophstein   (501) staff       (20)        7 2024-05-15 07:03:38.000000 quasim-0.2.0/quasim.egg-info/top_level.txt
+-rw-r--r--   0 christophstein   (501) staff       (20)       38 2024-05-15 07:03:38.613976 quasim-0.2.0/setup.cfg
```

### Comparing `quasim-0.1.0/LICENSE` & `quasim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/PKG-INFO` & `quasim-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasim
-Version: 0.1.0
+Version: 0.2.0
 Summary: Efficient simulation of quantum computing circuits.
 Author: Christoph Stein
 License: The MIT License (MIT)
         Copyright © 2024 Christoph Stein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -33,14 +33,26 @@
 [QuaSim](https://github.com/westoun/quasim) is a Python library for
 simulating quantum circuits. It was created partly as a learning project,
 partly out of necessity.
 For my master thesis, I required a quantum circuit simulator that was easy
 to set up, had low overhead, and was comparatively faster than [Qiskit](https://www.ibm.com/quantum/qiskit)
 on the amount of qubits that my experiments required.
 
+| qubit_num\simulator | qiskit 0.45.1 | quasim 0.1.0 | quasim 0.2.0 |
+| :-----------------: | -------------:| ------------:| ------------:|
+| 3                   | 15.06s        | 3.15s        | 2.71s        | 
+| 4                   | 15.20s        | 4.43s        | 3.83s        | 
+| 5                   | 15.06s        | 5.03s        | 3.76s        | 
+| 6                   | 14.16s        | 7.76s        | 4.69s        | 
+| 7                   | 14.36s        | 13.60s       | 6.32s        | 
+| 8                   | 15.28s        | 30.61s       | 8.75s        | 
+
+
+**Table 1:** Execution time on 1000 randomly generated circuits with 40 gates each.
+
 Aside from a low degree of overhead and dependencies (numpy only), QuaSim's speed gain
 comes down to the way it detects and handles entanglement, since entanglement is the
 reason why quantum circuits experience exponential resource growth when simulated
 on classical computers.
 
 Unless a qubit has been entangled with other qubits through the use of a controlled gate,
 QuaSim stores and evolves its state independently from all other qubits.
```

### Comparing `quasim-0.1.0/README.md` & `quasim-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 [QuaSim](https://github.com/westoun/quasim) is a Python library for
 simulating quantum circuits. It was created partly as a learning project,
 partly out of necessity.
 For my master thesis, I required a quantum circuit simulator that was easy
 to set up, had low overhead, and was comparatively faster than [Qiskit](https://www.ibm.com/quantum/qiskit)
 on the amount of qubits that my experiments required.
 
+| qubit_num\simulator | qiskit 0.45.1 | quasim 0.1.0 | quasim 0.2.0 |
+| :-----------------: | -------------:| ------------:| ------------:|
+| 3                   | 15.06s        | 3.15s        | 2.71s        | 
+| 4                   | 15.20s        | 4.43s        | 3.83s        | 
+| 5                   | 15.06s        | 5.03s        | 3.76s        | 
+| 6                   | 14.16s        | 7.76s        | 4.69s        | 
+| 7                   | 14.36s        | 13.60s       | 6.32s        | 
+| 8                   | 15.28s        | 30.61s       | 8.75s        | 
+
+
+**Table 1:** Execution time on 1000 randomly generated circuits with 40 gates each.
+
 Aside from a low degree of overhead and dependencies (numpy only), QuaSim's speed gain
 comes down to the way it detects and handles entanglement, since entanglement is the
 reason why quantum circuits experience exponential resource growth when simulated
 on classical computers.
 
 Unless a qubit has been entangled with other qubits through the use of a controlled gate,
 QuaSim stores and evolves its state independently from all other qubits.
```

### Comparing `quasim-0.1.0/pyproject.toml` & `quasim-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["quasim", "quasim.gates"]
 
 [project]
 name = "quasim"
-version = "0.1.0"
+version = "0.2.0"
 description = "Efficient simulation of quantum computing circuits."
 readme = "README.md"
 authors = [{ name = "Christoph Stein"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quasim-0.1.0/quasim/circuit.py` & `quasim-0.2.0/quasim/circuit.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/_matrices.py` & `quasim-0.2.0/quasim/gates/_matrices.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/controlled_gates.py` & `quasim-0.2.0/quasim/gates/controlled_gates.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/double_controlled_gates.py` & `quasim-0.2.0/quasim/gates/double_controlled_gates.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/single_qubit_gates.py` & `quasim-0.2.0/quasim/gates/single_qubit_gates.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/swap.py` & `quasim-0.2.0/quasim/gates/swap.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/gates/utils.py` & `quasim-0.2.0/quasim/gates/utils.py`

 * *Files identical despite different names*

### Comparing `quasim-0.1.0/quasim/simulator.py` & `quasim-0.2.0/quasim/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,146 @@
 #!/usr/bin/env python3
 
+from dataclasses import dataclass
+import math
 import numpy as np
-from typing import List, Dict
+from typing import List
+import warnings
 
-from .circuit import Circuit
-from .gates import IGate, Swap, Gate, CGate, CCGate
+from .gates import Swap, Gate, CGate, CCGate
 from .gates.utils import (
     create_double_controlled_matrix,
     create_controlled_matrix,
     create_matrix,
 )
-from .utils import QubitGroup
 
 QUBIT_STARTING_STATE = np.zeros(2, dtype=np.complex128)
 QUBIT_STARTING_STATE[0] = 1
 
 
-def apply_swap_gate(qubit_groups: List[QubitGroup], gate: Swap) -> None:
-    """Swap the indices of the qubits targetted by the swap gate
-    in place.
+@dataclass
+class QubitGroup:
+    """Helper class used in the simulator to keep track
+    of which qubit sets have been entangled (for the sake
+    of faster computation)."""
+
+    qubits: List[int]
+    state: np.ndarray
+
+    def __hash__(self) -> int:
+        qubit_string = ",".join([str(qubit) for qubit in self.qubits])
+        return hash(qubit_string)
+
+
+def probabilities_from_state(state: np.ndarray) -> np.ndarray:
+    """Returns the probabilities corresponding to a quantum
+    system state."""
+
+    conjugate = state.conjugate()
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+
+        # Ignore "np.complex128Warning: Casting np.complex128 values to real discards the imaginary part"
+        # since that is precisely what we want.
+        probabilities = np.multiply(state, conjugate).astype(float)
+
+    return probabilities
+
+
+def probability_dict_from_state(state: np.ndarray) -> np.ndarray:
+    """Returns a dictionary of the probabilities corresponding
+    to the specified state. States with a probability of 0 are
+    omitted.
     """
-    for qubit_group in qubit_groups:
-        for i in range(len(qubit_group.qubits)):
-            if qubit_group.qubits[i] == gate.qubit1:
-                qubit_group.qubits[i] = gate.qubit2
 
-            elif qubit_group.qubits[i] == gate.qubit2:
-                qubit_group.qubits[i] = gate.qubit1
+    qubit_num = int(math.log2(len(state)))
+
+    probabilities = probabilities_from_state(state)
+
+    probability_dict = {}
+    for i, probability in enumerate(probabilities):
+
+        if probability == 0:
+            continue
+
+        state: str = ""
+
+        remainder = i
+        for j in reversed(range(qubit_num)):
+
+            if remainder >= 2**j:
+                state += "1"
+                remainder -= 2**j
+            else:
+                state += "0"
+
+        probability_dict[state] = probability
+
+    return probability_dict
+
+
+def is_in_ket0(qubit_group: QubitGroup) -> bool:
+    """Indicate if a specified qubit group is in ket0 state.
+    If the qubit group contains more than 1 qubit, a
+    NotImplementedError is raised.
+    """
+
+    if len(qubit_group.qubits) != 1:
+        raise NotImplementedError()
+
+    return qubit_group.state.tolist()[0] == 1
+
+
+def is_in_ket1(qubit_group: QubitGroup) -> bool:
+    """Indicate if a specified qubit group is in ket1 state.
+    If the qubit group contains more than 1 qubit, a
+    NotImplementedError is raised.
+    """
+
+    if len(qubit_group.qubits) != 1:
+        raise NotImplementedError()
+
+    return qubit_group.state.tolist()[1] == 1
 
 
 def initialize_qubit_groups(qubit_num: int) -> List[QubitGroup]:
     """Create a list of qubit groups where each qubit group contains
     exactly one qubit id.
     """
     qubit_groups: List[QubitGroup] = []
     for i in range(qubit_num):
         qubit_groups.append(QubitGroup(qubits=[i], state=QUBIT_STARTING_STATE))
     return qubit_groups
 
 
-def select_affected_qubit_groups(
-    qubit_groups: List[QubitGroup], gate: IGate
-) -> List[QubitGroup]:
-    """Select the subset of qubit groups whose qubit ids
-    are affected by the specified gate.
+def get_sorted_state(qubit_group: QubitGroup) -> np.ndarray:
+    """Return a sorted version of the state of a qubit group
+    based on the order of the group's qubit ids.
     """
+    qubit_num = len(qubit_group.qubits)
 
-    relevant_qubit_groups: List[QubitGroup] = []
-    for qubit_group in qubit_groups:
-        for qubit in qubit_group.qubits:
-            if qubit in gate.qubits:
-                if qubit_group not in relevant_qubit_groups:
-                    relevant_qubit_groups.append(qubit_group)
-
-                break
-
-    return relevant_qubit_groups
+    sorting_order = [0] * (2**qubit_num)
+    for i in range(2**qubit_num):
 
+        remainder = i
+        for j in reversed(range(qubit_num)):
 
-def merge_qubit_groups(
-    relevant_groups: List[QubitGroup], total_groups: List[QubitGroup]
-) -> QubitGroup:
-    """Merge selected (relevant) qubit groups into a single qubit group
-    and remove the previous qubit groups from the list of all qubit groups.
-    The removal happens in place, while the merged qubit group is returned.
-    """
-    merged_qubit_group = relevant_groups[0]
-    for qubit_group in relevant_groups[1:]:
-        merged_qubit_group.qubits.extend(qubit_group.qubits)
-        merged_qubit_group.state = np.kron(merged_qubit_group.state, qubit_group.state)
+            if remainder >= 2**j:
+                sorting_order[i] += 2 ** (
+                    qubit_num - qubit_group.qubits[qubit_num - j - 1] - 1
+                )
+                remainder -= 2**j
 
-        total_groups.remove(qubit_group)
+    sorted_state = [0] * 2**qubit_num
+    for i in range(2**qubit_num):
+        sorted_state[sorting_order[i]] = qubit_group.state[i]
 
-    return merged_qubit_group
+    sorted_state = np.asarray(sorted_state, dtype=np.complex128)
+    return sorted_state
 
 
 def apply_gate(relevant_qubit_group: QubitGroup, gate: Gate) -> None:
     """Apply the action of the specified gate onto the selected
     qubit group in place.
     """
     target_qubit = relevant_qubit_group.qubits.index(gate.target_qubit)
@@ -116,100 +180,33 @@
         control_qubit2=control_qubit2,
         target_qubit=target_qubit,
         qubit_num=len(relevant_qubit_group.qubits),
     )
     relevant_qubit_group.state = np.matmul(matrix, relevant_qubit_group.state)
 
 
-def aggregate_qubit_groups(qubit_groups: List[QubitGroup]) -> QubitGroup:
-    """Combine a list of qubit groups into a new joined qubit group."""
-    aggregated_qubit_group = qubit_groups[0]
-    for qubit_group in qubit_groups[1:]:
-        aggregated_qubit_group.qubits.extend(qubit_group.qubits)
-        aggregated_qubit_group.state = np.kron(
-            aggregated_qubit_group.state, qubit_group.state
-        )
-    return aggregated_qubit_group
-
-
-def get_sorted_state(qubit_group: QubitGroup) -> np.ndarray:
-    """Return a sorted version of the state of a qubit group
-    based on the order of the group's qubit ids.
+def apply_swap_gate(qubit_groups: List[QubitGroup], gate: Swap) -> None:
+    """Swap the indices of the qubits targetted by the swap gate
+    in place.
     """
-    qubit_num = len(qubit_group.qubits)
-
-    sorting_order = [0] * (2**qubit_num)
-    for i in range(2**qubit_num):
-
-        remainder = i
-        for j in reversed(range(qubit_num)):
-
-            if remainder >= 2**j:
-                sorting_order[i] += 2 ** (
-                    qubit_num - qubit_group.qubits[qubit_num - j - 1] - 1
-                )
-                remainder -= 2**j
-
-    sorted_state = [0] * 2**qubit_num
-    for i in range(2**qubit_num):
-        sorted_state[sorting_order[i]] = qubit_group.state[i]
+    for qubit_group in qubit_groups:
+        for i in range(len(qubit_group.qubits)):
+            if qubit_group.qubits[i] == gate.qubit1:
+                qubit_group.qubits[i] = gate.qubit2
 
-    sorted_state = np.asarray(sorted_state, dtype=np.complex128)
-    return sorted_state
+            elif qubit_group.qubits[i] == gate.qubit2:
+                qubit_group.qubits[i] = gate.qubit1
 
 
-class QuaSim:
-    """Quantum circuit simulator used to evaluate quantum
-    circuits.
+def select_affected_qubit_group(
+    qubit_groups: List[QubitGroup], qubit_id: int
+) -> QubitGroup:
+    """Select the qubit group whose qubit id
+    is affected by the specified gate. Raise ValueError
+    if no matching qubit group is found.
     """
 
-    def __init__(self) -> None:
-        pass
-
-    def evaluate(self, circuits: List[Circuit]) -> None:
-        """Evaluates a list of quantum circuits and stores the
-        state at the end of each circuit in circuit.state."""
-
-        for circuit in circuits:
-            self.evaluate_circuit(circuit)
-
-    def evaluate_circuit(self, circuit: Circuit) -> None:
-        """Evaluates a quantum circuit and stores the
-        state at the end of the circuit in circuit.state."""
-
-        if circuit.state is not None:
-            return circuit.state
-
-        qubit_groups = initialize_qubit_groups(circuit.qubit_num)
-
-        for gate in circuit.gates:
-            if type(gate) == Swap:
-                apply_swap_gate(qubit_groups, gate)
-                continue
-
-            relevant_qubit_groups: List[QubitGroup] = select_affected_qubit_groups(
-                qubit_groups, gate
-            )
-
-            relevant_qubit_group = merge_qubit_groups(
-                relevant_groups=relevant_qubit_groups, total_groups=qubit_groups
-            )
-
-            if issubclass(gate.__class__, Gate):
-                apply_gate(relevant_qubit_group, gate)
-
-            elif issubclass(gate.__class__, CGate):
-                apply_cgate(relevant_qubit_group, gate)
-
-            elif issubclass(gate.__class__, CCGate):
-                apply_ccgate(relevant_qubit_group, gate)
-
-            else:
-                raise NotImplementedError(
-                    f"Unknown gate type for {gate} ({type(gate)})"
-                )
-
-        aggregated_qubit_group = aggregate_qubit_groups(qubit_groups)
-
-        sorted_state = get_sorted_state(aggregated_qubit_group)
+    for qubit_group in qubit_groups:
+        if qubit_id in qubit_group.qubits:
+            return qubit_group
 
-        circuit.set_state(sorted_state)
+    raise ValueError(f"No matching qubit group found for qubit '{qubit_id}'")
```

### Comparing `quasim-0.1.0/quasim.egg-info/PKG-INFO` & `quasim-0.2.0/quasim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasim
-Version: 0.1.0
+Version: 0.2.0
 Summary: Efficient simulation of quantum computing circuits.
 Author: Christoph Stein
 License: The MIT License (MIT)
         Copyright © 2024 Christoph Stein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -33,14 +33,26 @@
 [QuaSim](https://github.com/westoun/quasim) is a Python library for
 simulating quantum circuits. It was created partly as a learning project,
 partly out of necessity.
 For my master thesis, I required a quantum circuit simulator that was easy
 to set up, had low overhead, and was comparatively faster than [Qiskit](https://www.ibm.com/quantum/qiskit)
 on the amount of qubits that my experiments required.
 
+| qubit_num\simulator | qiskit 0.45.1 | quasim 0.1.0 | quasim 0.2.0 |
+| :-----------------: | -------------:| ------------:| ------------:|
+| 3                   | 15.06s        | 3.15s        | 2.71s        | 
+| 4                   | 15.20s        | 4.43s        | 3.83s        | 
+| 5                   | 15.06s        | 5.03s        | 3.76s        | 
+| 6                   | 14.16s        | 7.76s        | 4.69s        | 
+| 7                   | 14.36s        | 13.60s       | 6.32s        | 
+| 8                   | 15.28s        | 30.61s       | 8.75s        | 
+
+
+**Table 1:** Execution time on 1000 randomly generated circuits with 40 gates each.
+
 Aside from a low degree of overhead and dependencies (numpy only), QuaSim's speed gain
 comes down to the way it detects and handles entanglement, since entanglement is the
 reason why quantum circuits experience exponential resource growth when simulated
 on classical computers.
 
 Unless a qubit has been entangled with other qubits through the use of a controlled gate,
 QuaSim stores and evolves its state independently from all other qubits.
```

