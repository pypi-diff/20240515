# Comparing `tmp/quanthon-0.3.6.6.tar.gz` & `tmp/quanthon-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanthon-0.3.6.6.tar", last modified: Mon Apr 29 06:18:42 2024, max compression
+gzip compressed data, was "quanthon-0.3.7.tar", last modified: Tue May 14 23:52:24 2024, max compression
```

## Comparing `quanthon-0.3.6.6.tar` & `quanthon-0.3.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.495130 quanthon-0.3.6.6/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.6.6/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-29 06:18:42.494908 quanthon-0.3.6.6/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.492718 quanthon-0.3.6.6/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.6.6/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-25 10:06:17.000000 quanthon-0.3.6.6/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     7244 2024-04-29 06:12:42.000000 quanthon-0.3.6.6/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-25 10:06:05.000000 quanthon-0.3.6.6/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 quanthon-0.3.6.6/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.6.6/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.6.6/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.6.6/Quanthon/mappers_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.6.6/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.6.6/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 quanthon-0.3.6.6/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.6.6/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6569 2024-04-18 11:08:36.000000 quanthon-0.3.6.6/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.494673 quanthon-0.3.6.6/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      557 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-29 06:18:42.000000 quanthon-0.3.6.6/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.6.6/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-29 06:18:42.495174 quanthon-0.3.6.6/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-29 06:16:24.000000 quanthon-0.3.6.6/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-29 06:18:42.494378 quanthon-0.3.6.6/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.6.6/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.6.6/tests/test_mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.6.6/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.6.6/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:52:24.049523 quanthon-0.3.7/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.7/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-05-14 23:52:24.049272 quanthon-0.3.7/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:52:24.046745 quanthon-0.3.7/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.7/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-29 12:30:59.000000 quanthon-0.3.7/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)    10022 2024-05-14 11:12:34.000000 quanthon-0.3.7/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5413 2024-05-14 23:35:06.000000 quanthon-0.3.7/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12678 2024-05-14 23:51:46.000000 quanthon-0.3.7/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.7/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)      465 2024-05-01 13:34:06.000000 quanthon-0.3.7/Quanthon/history.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.7/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.7/Quanthon/mappers_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.7/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.7/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1560 2024-05-04 17:32:55.000000 quanthon-0.3.7/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.7/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     7204 2024-05-14 23:52:14.000000 quanthon-0.3.7/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:52:24.049023 quanthon-0.3.7/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2519 2024-05-14 23:52:24.000000 quanthon-0.3.7/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      577 2024-05-14 23:52:24.000000 quanthon-0.3.7/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-05-14 23:52:24.000000 quanthon-0.3.7/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-05-14 23:52:24.000000 quanthon-0.3.7/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-05-14 23:52:24.000000 quanthon-0.3.7/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.7/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-05-14 23:52:24.049572 quanthon-0.3.7/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-05-14 23:35:18.000000 quanthon-0.3.7/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:52:24.048503 quanthon-0.3.7/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.7/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.7/tests/test_mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.7/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.7/tests/test_vqes.py
```

### Comparing `quanthon-0.3.6.6/PKG-INFO` & `quanthon-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6.6
+Version: 0.3.7
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.6.6/Quanthon/Models.py` & `quanthon-0.3.7/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/algorithms.py` & `quanthon-0.3.7/Quanthon/algorithms.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from scipy.optimize import minimize, Bounds
 import numpy as np
 import warnings
 from .expectation import cal_expectation
 from .utils import pauli_sum
 from .base import Qubits
+from .history import AdaptHistory
 
 class VQE():
         def __init__(self, ansatz, init_points, optimiser=minimize):
             '''
             args:
                 ansatz: a parametriced circuit that takes parmas: theta and phi
                 init_points: a list of initial points, must match the number of the parameters in the ansatz
@@ -37,35 +38,40 @@
             
             energy = self.expectation(qc, self.H, self.num_shots)
 
             # self.H_mat = pauli_sum(self.H)
             # energy = self.ansatz.qubits.state.conj().T @ self.H_mat @ self.ansatz.qubits.state
             return energy
 
-        def minimise_eigenvalue(self, H_pauli_str, num_shots=10000):
+        def minimise_eigenvalue(self, H_pauli_str, num_shots=10000, method='powell'):
             '''
             Rotates the parametrised circuit to find the minimised energy using classical 
             minimisation algorithms.
-            Inputs:
-            H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
-            num_shots: (int) number of shots,
-            return: (float) minimised energy eigenvalues.'''
+            args:
+                H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
+                num_shots: (int) number of shots,
+
+            return: (tuple) optimal parameters, minimised energy eigenvalues.'''
             self.H = H_pauli_str
 
             self.num_shots = num_shots
 
             lb = -np.pi * np.ones(len(self.params))
             ub = np.pi * np.ones(len(self.params))
             bounds = Bounds(lb, ub)
             
+            if method == 'powell':
+                bounds = None
+            
             result = self.minimise(self._objective, 
                                    self.params, 
+                                   method=method,
                                 #    method='Powell',
                                 #    method='Nelder-Mead',
-                                     method='COBYLA',
+                                    #  method='COBYLA',
                                     #  method='TNC',
                                    bounds=bounds, 
                                    options= {"maxiter": 100}
                                    )
             min_params = result.x
             min_energy = result.fun
             
@@ -87,14 +93,16 @@
         '''
         self.old_params = [] # list of parameters for the adapt circuit 
         # self.old_gates = []
         self.ansatz = ansatz
         self.expectation = cal_expectation
 
         self.minimise = optimiser
+        self.estimate_energy = estimate_energy
+        self.hist = AdaptHistory()
         
     
     def gradient(self, A):
         
         '''
         A: the operator whose gradient is calculated.
         '''
@@ -115,15 +123,16 @@
         
         '''
             Append a new operator to the ansatz which has the largest greadient ~ [H, A]
             return:
                 True if largest gradient is < eps and a new operator is added, False otherwise.
         '''
 
-        op_cand = self.ansatz.pool[0]
+        rng = np.random.default_rng(4418)
+        op_cand = rng.choice(self.ansatz.pool, 1).tolist()[0]
         max_abs_grad = 0
 
         # print(op_cand)
         
         for op in self.ansatz.pool:
             op_mat = pauli_sum([(op.strip('i'), 1j)])
             op_grad = self.gradient(op_mat)
@@ -131,38 +140,45 @@
             
             # print(f"op: {op}, grad: {op_grad}")
 
             if abs_grad > max_abs_grad:
                 op_cand = op
                 max_abs_grad = abs_grad
         
-        print("max_abs_grad: ", max_abs_grad)
         
         if max_abs_grad < eps:
             print(f"end of adapt, grad = {max_abs_grad}")
             return False # gradient = 0, end of adapt  
         # print(f"appending, op: {op_cand}, grad: {max_abs_grad}")
         # grow the ansatz
         # self.old_gates.append(op_cand) # type(op_cand) == str
+        print("max_abs_grad: ", max_abs_grad)
         self.params = np.append(self.params, 0)
         self.ansatz.append_op(op_cand)
 
+        self.hist.update_grad(max_abs_grad)
+        self.hist.update_operators(op_cand)
+        
+
         return True
     
     def _objective(self, params):
         # print("called _objective")
         state = self.ansatz.run_without_update(params)
         qc = Qubits(self.ansatz.qubits.n_qubit)
         qc.set_state(state)
 
-        energy = self.expectation(qc, self.H_str, self.num_shots)
-        # energy = state.conj().T @ self.H_mat @ state
+        if self.estimate_energy:
+            energy = self.expectation(qc, self.H_str, self.num_shots)
+        else:
+            energy = state.conj().T @ self.H_mat @ state
+
         return energy
     
-    def run_adapt_circuit(self, H, num_shots=10000, max_iter=100, grad_eps=1e-4):
+    def run_adapt_circuit(self, H, num_shots=10000, max_iter=100, grad_eps=1e-4, method='COBYLA'):
         '''
         args:
             H: list of 2-tuple such as [('II', 0.5)]
             num_shots: number of shots,
             max_iter: maximum number of iterations,
         
         return: 
@@ -171,33 +187,96 @@
         self.H_mat = pauli_sum(H)
         self.H_str = H
         self.params = np.array([])
         for i in range(max_iter): 
             # need to update the state too
             # print(self.ansatz.qubits)
             # self.ansatz.run(self.params) # ??????
-            old_params, energy = self.minimise_eigenvalue(num_shots) # state is not updated here
+            old_params, energy = self.minimise_eigenvalue(num_shots, method=method) # state is not updated here
             self.params = old_params
             print(f"i: {i}, min_energy = {energy}")
-            
+            self.hist.update_energies(energy)
 
             if not self._append_operator(eps=grad_eps): # new parameter is added here 
                 break
             
         if i == max_iter - 1:
-            warnings.warn('Adapt circuit did not converge.')
+            print("Maximum adapt iteration reached, energy did not converge.")
+            # warnings.warn('Adapt circuit did not converge.')
         self.ansatz.run(self.params) # update the state with the final parameters
         return self.ansatz, energy
     
 
-    def minimise_eigenvalue(self, num_shots=10000):
+    def minimise_eigenvalue(self, num_shots=10000, method='SLSQP'):
+
+
+        '''
+            Rotates the parametrised circuit to find the minimised energy using classical 
+            minimisation algorithms.
+            args:
+                H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
+                num_shots: (int) number of shots,
 
+            return: (tuple) optimal parameters, minimised energy eigenvalues.
+        '''
         self.num_shots = num_shots
         
         # print(self.params)
-        result = self.minimise(self._objective, self.params, method='Powell', options= {"maxiter": 100000})
-        min_params = result.x
+
+        lb = -np.pi * np.ones(len(self.params))
+        ub = np.pi * np.ones(len(self.params))
+        bounds = Bounds(lb, ub)
+
+        # old_energy = self._objective(self.params)
+        # min_energy = old_energy
+
+        if self.params.size == 0:
+            result = self.minimise(self._objective, 
+                                0, 
+                                method=method, 
+                                #    bounds=bounds,
+                                options= {"maxiter": 100000}
+                                )
+        else:
+            result = self.minimise(self._objective, 
+                                self.params, 
+                                method=method, 
+                                #    bounds=bounds,
+                                options= {"maxiter": 100000}
+                                )
+
         min_energy = result.fun
+        min_params = result.x
+
+        old_energy = self._objective(self.params)
+        print(f"old energy: {old_energy}")
+        print(f"min_energy: {min_energy}")
+        if old_energy < min_energy:
+            warnings.warn("New energy is higher than the old energy.")
 
         # self.ansatz.run(min_params) # update the state using only the optimal parameters
          
-        return min_params, min_energy
+        return min_params, min_energy
+
+
+def qft(qubits, is_inverse=False, is_swap=True):
+
+    def nth_root_of_unity(self, n):
+        return 2j * n * np.pi / (2 ** self.qubits.n_qubit)
+    
+    if is_inverse:
+        for i in range(qubits.n_qubit):
+            for j in range(i):
+                qubits.cp(-np.pi / 2 ** (i - j), j, i)
+            qubits.H(i)
+    else:
+        for i in range(qubits.n_qubit):
+            qubits.H(i)
+            for j in range(i+1, qubits.n_qubit):
+                qubits.CP(nth_root_of_unity(j), j, i) # phi, controlled, target
+    
+    if is_swap:
+        for i in range(qubits.n_qubit/2):
+            qubits.SWAP(i, qubits.n_qubits-1) 
+
+def qpe():
+    raise NotImplementedError("Quantum Phase Estimation is not implemented yet.")
```

### Comparing `quanthon-0.3.6.6/Quanthon/ansatzs.py` & `quanthon-0.3.7/Quanthon/ansatzs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,228 @@
 '''Doc:
-    Ansatz for VQE calculations. Can grow if needs be. Parametrise the qubits object.
-    parameters are taken as arguments to the circuit at every iteration'''
+	Ansatz for VQE calculations. Can grow if needs be. Parametrise the qubits object.
+	parameters are taken as arguments to the circuit at every iteration'''
 
 # TODO: add init_state to HardwareEfficientAnsatz too
 
 # DEBUGGER
 
 def qprint(msg):
-    
-    print("QubitAdaptAnsatz")
-    print(msg)
+	
+	print("QubitAdaptAnsatz")
+	print(msg)
 
 
 import numpy as np
 from scipy.linalg import expm
 
 
 from .base import Qubits, Gate
 from .utils import pauli_sum
 
 class Ansatz:
 
-    '''Should work for any type of ansatz that are not evolving, do not use on its own.'''
-    def __init__(self, n_qubits, reps=1) -> None:
+	'''Should work for any type of ansatz that are not evolving, do not use on its own.'''
+	def __init__(self, n_qubits, reps=1) -> None:
 
-        self.n_qubits = n_qubits
-        self.reps = reps
-        self.n_params = 2 * n_qubits * reps
+		self.n_qubits = n_qubits
+		self.reps = reps
+		self.n_params = 2 * n_qubits * reps
 
   
 class HardwareEfficientAnsatz(Ansatz):
 
-    def __init__(self, n_qubits, reps=1) -> None:
-        super().__init__(n_qubits, reps)
+	def __init__(self, n_qubits, reps=1) -> None:
+		super().__init__(n_qubits, reps)
 
 
-    def create_circuit(self, init_params):
-        
-        self.qubits = Qubits(self.n_qubits)
-        if len(init_params) != self.n_params:
-            raise ValueError(f'Initial parameters do not match the number of parameters required for the ansatz: {len(init_params)} != {self.n_params}')
-        
-        reshaped_params = init_params.reshape(self.reps, 2*self.n_qubits)
-        
-        for r in range(self.reps):
-            for i in range(self.n_qubits):
-                # check if the parameters are real
-                if reshaped_params[r, i] != reshaped_params[r, i].real:
-                    raise ValueError(f'Parameter {[r,i]} is not real.')
-                self.qubits.Rx(reshaped_params[r, i], i)
-                self.qubits.Ry(reshaped_params[r, i + self.n_qubits], i)
-        
-        for r in range(self.reps):
-            for i in range(self.n_qubits):
-                if i != self.n_qubits - 1:
-                    self.qubits.CNOT(i, i+1)
-
-        # self.qubits.draw()
-
-    def run(self):
-        self.qubits.run()
-    
+	def create_circuit(self, init_params):
+		
+		self.qubits = Qubits(self.n_qubits)
+		if len(init_params) != self.n_params:
+			raise ValueError(f'Initial parameters do not match the number of parameters required for the ansatz: {len(init_params)} != {self.n_params}')
+		
+		reshaped_params = init_params.reshape(self.reps, 2*self.n_qubits)
+		
+		for r in range(self.reps):
+			for i in range(self.n_qubits):
+				# check if the parameters are real
+				if reshaped_params[r, i] != reshaped_params[r, i].real:
+					raise ValueError(f'Parameter {[r,i]} is not real.')
+				self.qubits.Rx(reshaped_params[r, i], i)
+				self.qubits.Ry(reshaped_params[r, i + self.n_qubits], i)
+		
+		for r in range(self.reps):
+			for i in range(self.n_qubits):
+				if i != self.n_qubits - 1:
+					self.qubits.CNOT(i, i+1)
+
+		# self.qubits.draw()
+
+	def run(self):
+		self.qubits.run()
+	
 
 
 class QubitAdaptAnsatz:
 
-    def __init__(self, n_qubits, pool='V', init_state=None) -> None:
+	def __init__(self, n_qubits, pool='V', init_state=None) -> None:
 
-        '''Ansatz for the Adapt-VQE calculation.'''
+		'''Ansatz for the Adapt-VQE calculation.
+		args:
+			n_qubits: int, number of qubits in the system
+			pool: str, the pool of operators to choose from, default is 'V' pool which can't be used fewer than 3 qubits!!.
+			init_state: np.array, the initial state of the system, default is None
+		'''
+
+		self.qubits = Qubits(n_qubits)
+
+		if init_state is None:
+			# initial state not sepcified, initialise randomly
+			# init_state = np.random.rand(2**n_qubits) + 1j * np.random.rand(2**n_qubits)
+			init_state = np.ones(2**n_qubits)
+			init_state = init_state / np.linalg.norm(init_state) 
+		
+		self.init_state = init_state
+		self.qubits.set_state(init_state)
+
+		if pool == 'V':
+			self.pool = self.create_complete_V_pool(n_qubits)
+		
+		elif pool == 'Vx':
+			self.pool = self.create_complete_Vx_pool(n_qubits)
+			
+		elif pool == 'G':
+			self.pool = self.create_complete_G_pool()
+		
+		else:
+			self.pool = pool # custom pool, doens't have to be complete
+			
+		
+
+	def __repr__(self) -> str:
+		
+		return f"QubitAdaptAnsatz of {self.qubits} qubits and pool: {self.pool}."
+	
+	def create_complete_V_pool(self, n):
+		
+		if n == 1:
+			return ['iY', 'Z'] 
+		
+		if n == 2:
+			return ['iYZ', 'iIY']
+
+		prev_set = self.create_complete_V_pool(n - 1)
+		new_pool = [] # set()
+
+		for prev_op in prev_set:
+			new_op = prev_op + 'Z'
+			new_pool.append(new_op)
+
+
+		new_pool.append('i' + (n-1) * 'I' + 'Y')
+		new_pool.append('i' + (n-2) * 'I' + 'YI')
+
+
+		return new_pool
+		
+	def create_complete_Vx_pool(self, n):
+		
+		if n == 1:
+			return ['iY', 'X'] 
+		
+		if n == 2:
+			return ['iYX', 'iIY']
+
+		prev_set = self.create_complete_Vx_pool(n - 1)
+		new_pool = [] # set()
+
+		for prev_op in prev_set:
+			new_op = prev_op + 'X'
+			new_pool.append(new_op)
+
+
+		new_pool.append('i' + (n-1) * 'I' + 'Y')
+		new_pool.append('i' + (n-2) * 'I' + 'YI')
+
+
+		return new_pool
+	
+	def create_complete_G_pool(self, n):
+		
+		pool = self._get_ys(n)
+		pool.extend(self._get_zy(n))
+		return pool
+
+	
+	def _get_ys(self,n):
+		'''Get a list of all the operators with a single Y in them'''
+		op = n*'I'
+		ops = []
+		for i in range(1, n):
+			y_op = list(op)
+			y_op[i] = 'Y'
+			ops.append(''.join(y_op))
+		
+		return ops
+
+	def _get_zys(self, n):
+		op = n*'I'
+		ops = []
+		for i in range(n-1):
+			yz_op = list(op)
+			yz_op[i] = 'Y'
+			yz_op[i+1] = 'Z'
+			ops.append(''.join(yz_op))
+		
+		return ops
+
+	def append_op(self, op):
+
+		'''
+		op: string, representing one of the operators in the pool
+		
+		'''
+		# no longer need to append all the gates since they are now saved
+
+		qprint(f"append_op op: {op}")
+		op_mat = pauli_sum([(op.strip('i'), 1j)])
+
+		def parametrised_mat(param, op_mat):
+			return expm(param * op_mat)
+		
+		# self.params.append(0) # the corresponding parameter for the gate, initialised to 0.
+		
+		adapt_gate = Gate(f'exp({op})', matrix=lambda param: parametrised_mat(param, op_mat), n_qubits=self.qubits.n_qubit)
+		self.qubits.circuit.append(adapt_gate)
+		
+	
+	def run(self, params):
+		for i, gate in enumerate(self.qubits.circuit):
+			# print(gate.matrix(params[i]))
+			self.qubits.state = gate.act(self.qubits.state, params[i])
+		
+		# print(self.qubits.circuit)
+	
+	def run_without_update(self, params):
+		'''Run the circuit without updating the state.'''
+		old_state = self.qubits.state
+		for i, gate in enumerate(self.qubits.circuit):
+			self.qubits.state = gate.act(self.qubits.state, params[i])
+			if not np.isclose(np.linalg.norm(self.qubits.state), 1):
+				raise ValueError(f"Probability does not sum to unity, prob: {self.qubits.prob}, state: {self.qubits.state}.")
+		
+		new_state = self.qubits.state
+		self.qubits.state = old_state # return to the new state while returning the result of the circuit
+		return new_state
 
-        self.qubits = Qubits(n_qubits)
 
-        if init_state is None:
-            # initial state not sepcified, initialise randomly
-            init_state = np.random.rand(2**n_qubits) + 1j * np.random.rand(2**n_qubits)
-            init_state = init_state / np.linalg.norm(init_state) 
-        
-        self.init_state = init_state
-        self.qubits.set_state(init_state)
-
-        if pool == 'V':
-            self.pool = self.create_complete_V_pool(n_qubits)
-        
-        elif pool == 'G':
-            self.pool = self.create_complete_G_pool()
-        
-        else:
-            self.pool = pool # custom pool, doens't have to be complete
-            
-        
-
-    def __repr__(self) -> str:
-        
-        return f"QubitAdaptAnsatz of {self.qubits} qubits and pool: {self.pool}."
-    
-    def create_complete_V_pool(self, n):
-        
-        if n == 2:
-            return ['iYZ', 'iIY']
-
-        prev_set = self.create_complete_V_pool(n - 1)
-        new_pool = [] # set()
-
-        for prev_op in prev_set:
-            new_op = prev_op + 'Z'
-            new_pool.append(new_op)
-
-
-        new_pool.append('i' + (n-1) * 'I' + 'Y')
-        new_pool.append('i' + (n-2) * 'I' + 'YI')
-
-
-        return new_pool
-        
-
-    def create_complete_G_pool(self):
-        raise NotImplementedError('Not implemented yet')
-
-
-    def append_op(self, op):
-
-        '''
-        op: string, representing one of the operators in the pool
-        
-        '''
-        # no longer need to append all the gates since they are now saved
-
-        qprint(f"append_op op: {op}")
-        op_mat = pauli_sum([(op.strip('i'), 1j)])
-
-        def parametrised_mat(param, op_mat):
-            return expm(param * op_mat)
-        
-        # self.params.append(0) # the corresponding parameter for the gate, initialised to 0.
-        
-        adapt_gate = Gate(f'exp({op})', matrix=lambda param: parametrised_mat(param, op_mat), n_qubits=self.qubits.n_qubit)
-        self.qubits.circuit.append(adapt_gate)
-        
-    
-    def run(self, params):
-        for i, gate in enumerate(self.qubits.circuit):
-            # print(gate.matrix(params[i]))
-            self.qubits.state = gate.act(self.qubits.state, params[i])
-        
-        # print(self.qubits.circuit)
-    
-    def run_without_update(self, params):
-        '''Run the circuit without updating the state.'''
-        old_state = self.qubits.state
-        for i, gate in enumerate(self.qubits.circuit):
-            self.qubits.state = gate.act(self.qubits.state, params[i])
-        
-        new_state = self.qubits.state
-        self.qubits.state = old_state # return to the new state while returning the result of the circuit
-        return new_state
 
+	
 
+		
 
-    
 
-        
 
-
-
-    
+
```

### Comparing `quanthon-0.3.6.6/Quanthon/base.py` & `quanthon-0.3.7/Quanthon/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''The basic classes for quantum computing. Replaced base.py, which was discontinued after Quanthon 0.3.0'''
 
 # TODO: Add n dimension rotation 
 
 import numpy as np
 from collections import Counter
-from .utils import one_fixed_bit, flip_bit, swap_bits
+from .utils import one_fixed_bit, flip_bit, swap_bits, get_bit, make_op_mat, is_valid_state
 
 # Constants
 rng = np.random.default_rng()
 rangle = '\u27E9'
 
 class Gate:
 
@@ -28,31 +28,39 @@
 
     def __repr__(self):
         return f"Gate: {self.name} \n Matrix: \n {self.matrix} \n"
     
     def _check_is_unitary(self, matrix):
 
         if not np.allclose(matrix @ matrix.conj().T, np.eye(matrix.shape[0])):
-            raise ValueError(f"{self.name} is not unitary.")
+            raise ValueError(f"{self.name} is not unitary, matrix: {matrix}.")
     
     def act(self, state, param=None):
         if param is not None:
             self._check_is_unitary(self.matrix(param))
-            return self.matrix(param) @ state
-        self._check_is_unitary(self.matrix)
-        return self.matrix @ state
+            result = self.matrix(param) @ state
+        
+        else:
+            self._check_is_unitary(self.matrix)
+            result = self.matrix @ state
+        
 
+        if is_valid_state(result):
+            return result
+        else:
+            raise ValueError(f"Invalid state. {result} {np.abs(result**2)}")
+    
     
 class Qubits:
 
     def __init__(self,n):
         self.state = np.zeros(2**n, dtype=np.complex_)
         self.state[0] = 1
         self.n_qubit = n
-        self.opeartor_size = 2**n
+        self.operator_size = 2**n
 
         self.I = np.eye(2)
         self.h = 1/np.sqrt(2) * np.array([[1, 1], [1, -1]])
         self.x = np.array([[0, 1], [1, 0]])
         self.y = np.array([[0, -1j], [1j, 0]])
         self.z = np.array([[1, 0], [0, -1]])
         self.s = np.array([[1, 0], [0, 1j]])
@@ -137,79 +145,89 @@
             amplitude = self.state[idx]
             computational_str += f"{amplitude:.2f}|{binary_str}⟩ + "
 
         computational_str = computational_str.rstrip("+ ")
 
         # Return the computational basis notation
         return computational_str
-    
-    def _make_op_mat(self, op, indx): 
-        ''' Operates the qubit with the given operator and index. '''
-        result = np.eye(2**indx)
-        result = np.kron(result, op)
-        # print(op)
-        # rest_of_indices = int(self.n_qubit - indx - np.sqrt(len(op)))
-        rest_of_indices = int(self.n_qubit - indx - np.log2(len(op)))
-        for _ in range(rest_of_indices):
-            result = np.kron(result, np.eye(2))
-        
-        return result
-        # self.state = result @ self.state
 
     def H(self,i):
         # self.operate(self.h,i)
-        matrix = self._make_op_mat(self.h, i)
+        matrix = make_op_mat(self.n_qubit, self.h, i)
         self.circuit.append(Gate('H', matrix, self.n_qubit))
         self._update_gate_history('H', i)
     
     def X(self,i):
         # self.operate(self.x, i)
-        matrix = self._make_op_mat(self.x, i)
+        matrix = make_op_mat(self.n_qubit, self.x, i)
         self.circuit.append(Gate('X', matrix, self.n_qubit))
         self._update_gate_history('X', i)
 
     def Y(self,i):
         # self.operate(self.y, i)
-        matrix = self._make_op_mat(self.y, i)
+        matrix = make_op_mat(self.n_qubit, self.y, i)
         self.circuit.append(Gate('Y', matrix, self.n_qubit))
         self._update_gate_history('Y', i)
 
     def Z(self,i):
         # self.operate(self.z, i)
-        matrix = self._make_op_mat(self.z, i)
+        matrix = make_op_mat(self.n_qubit, self.z, i)
         self.circuit.append(Gate('Z', matrix, self.n_qubit))
         self._update_gate_history('Z', i)
     
     def Sdag(self,i):
         # self.operate(self.s.conj(), i)
-        matrix = self._make_op_mat(self.s.conj(), i)
+        matrix = make_op_mat(self.n_qubit, self.s.conj(), i)
         self.circuit.append(Gate('Sdag', matrix, self.n_qubit))
         self._update_gate_history('Sdag', i)
 
     def Rx(self, theta, i):
 
         rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
         # self.operate(Rx, i) 
-        matrix = self._make_op_mat(rx, i)
+        matrix = make_op_mat(self.n_qubit, rx, i)
         self.circuit.append(Gate('Rx', matrix, self.n_qubit))
         self._update_gate_history(f'Rx_{theta}', i)
 
     def Ry(self, phi, i):
         ry = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
         # self.operate(Ry, i)
-        matrix = self._make_op_mat(ry, i)
+        matrix = make_op_mat(self.n_qubit, ry, i)
         self.circuit.append(Gate('Ry', matrix, self.n_qubit))
         self._update_gate_history(f'Ry_{phi}', i)
 
+    def controlled_U1(self, op, control, target):
+        '''
+        Apply the two-qubit controlled gate. Control before target. '''
+        if self.n_qubit == 1:
+            raise ValueError("The CNOT gate can not be applied to a single qubit.")
+
+        active_op_size = np.log2(op.shape[0])
+        matrix = np.eye(self.operator_size)
+        indices = one_fixed_bit(self.n_qubit, self.n_qubit - control - 1, is_decimal=True) # we do n-c cuz our 0th bit is on the left
+        
+        # if the target is 0
+        for i in indices:
+            if get_bit(i, self.n_qubit - target - 1) == 0:
+                matrix[i, i] = 0
+                matrix[i, i] = 1
+
+        # I 0
+        # 0 U
+
+        # U 0
+        # 0 I
+
+
     def CNOT(self, control, target):
 
         if self.n_qubit == 1:
             raise ValueError("The CNOT gate can not be applied to a single qubit.")
         
-        matrix = np.eye(self.opeartor_size)
+        matrix = np.eye(self.operator_size)
 
         indices = one_fixed_bit(self.n_qubit, self.n_qubit - control - 1, is_decimal=True) # we do n-c cuz our 0th bit is on the left
 
         for i in indices:
             # print(i)
             f = flip_bit(i, self.n_qubit - target - 1) # same reason
             # print(f)
@@ -223,49 +241,55 @@
 
 
     def SWAP(self, qubit1, qubit2):
         if self.n_qubit == 1:
             raise ValueError("The SWAP gate can not be applied to a single qubit.")
         
 
-        matrix = np.zeros((self.opeartor_size, self.opeartor_size))
-        for i in range(self.opeartor_size):
+        matrix = np.zeros((self.operator_size, self.operator_size))
+        for i in range(self.operator_size):
             j = swap_bits(i, self.n_qubit - qubit1 - 1, self.n_qubit - qubit2 - 1)
             matrix[i, j] = 1
             matrix[j, i] = 1
 
         # self.state = matrix @ self.state
         self.circuit.append(Gate('SWAP', matrix, self.n_qubit))
         self._update_gate_history("SWAP", (qubit1, qubit2))
     
     def run(self):
         
-        '''Execute the circuit. Return the result.'''
+        '''
+        Execute the circuit. Return the result.
+        '''
         for gate in self.circuit:
             self.state = gate.act(self.state)
-        
+         
     def run_and_reset(self):
         '''Execute the circuit and reset the circuit. Return the result.'''
         self.run()
         state = self.state
         self.reset_circuit()
         return state
 
     def prob(self):
         prob = np.abs(self.state**2)
+        
         return prob
 
     def measure(self, n_shots=1):
         ''' n: number of shots 
             indexs: the index of the qubit(s) being measured '''
         
         prob = self.prob()
         allowed_outcomes = np.arange(len(self.state))
         # print(self.state)
-        outcomes = np.random.choice(allowed_outcomes, p=prob, size = n_shots)
+        try:
+            outcomes = np.random.choice(allowed_outcomes, p=prob, size = n_shots)
+        except ValueError:
+            raise ValueError(f"Prob: {prob}.")
         
         self.state = np.zeros_like(self.state)
         self.state[outcomes[-1]] = 1
         counts = Counter(outcomes)
         
         outcomes_count = np.zeros((len(self.state),2)) # 2: state and count
         for i in range(len(self.state)):
```

### Comparing `quanthon-0.3.6.6/Quanthon/expectation.py` & `quanthon-0.3.7/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/mappers.py` & `quanthon-0.3.7/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/mappers_utils.py` & `quanthon-0.3.7/Quanthon/mappers_utils.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/ut_pyscf_mel.py` & `quanthon-0.3.7/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/ut_qiskit_hamiltonian.py` & `quanthon-0.3.7/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,14 @@
             u[int(label[0]), int(label[1]), int(label[2]), int(label[3])] = coeff
         else:
             raise ValueError("Label not recognized")
         # print(f"{coeff:+.8f} * '{label}'")
 
     return h, u
 
-def remove_non_num(string):
-
-    for char in string:
-        if char not in '0123456789':
-            string = string.replace(char, '')
-    return string
 
 
 if __name__ == "__main__":
     h, u  = get_h2()
 
     u_list = []
     for i in range(4):
```

### Comparing `quanthon-0.3.6.6/Quanthon/ut_test_jw.py` & `quanthon-0.3.7/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/Quanthon/utils.py` & `quanthon-0.3.7/Quanthon/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # Utils
 import numpy as np
 from itertools import product
+
+def make_op_mat(n, op, indx): 
+    ''' Operates the qubit with the given operator and index. '''
+    result = np.eye(2**indx) # everything upto index
+    result = np.kron(result, op) # the operator on the index
+    
+    rest_of_indices = int(n - indx - np.log2(len(op)))
+    for _ in range(rest_of_indices):
+        result = np.kron(result, np.eye(2))
+    
+    return result
+
 def get_pauli(basis_name):
     pauli_matrices = {'I': np.eye(2, dtype=np.complex128), 
                       'X': np.array([[0, 1], [1, 0]], dtype=np.complex128), 
                       'Y': np.array([[0, -1j], [1j, 0]]), 
                       'Z': np.array([[1, 0], [0, -1]],dtype=np.complex128)}
 
     # Check if basis_name is a valid combination
@@ -85,15 +97,16 @@
     '''generate the bit string of length n such that the cth bit is always 1.
 
     args:
         n: int, length of the bit string.
         c: the index of the bit to be fixed to 1
         
     return:
-        combinations: string, list of all the bit stirngs of length n whose cth bit is 1.
+        combinations: list, list of all the bit strings of length n whose cth bit is 1. if is_decimal 
+        is set to true than returns the decimal representations.
     
     N.B. 
         to convert to int, specify int(bit_sting, 2) for binary input.'''
 
     combinations = []
     for i in range(2 ** n):
         bit_string = f'{i:0{n}b}'
@@ -126,14 +139,17 @@
     """
     if (val >> i) & 1 != (val >> j) & 1:
         mask = (1 << i) | (1 << j)
         val ^= mask
 
     return val
 
+def get_bit(i, n):
+    '''return the nth bit of integer i'''
+    return (i >> n) & 1
 
 def get_all_paulis(n):
     '''
     args: 
         n: the number of qubits.
     
     return: list of all the possible Pauli strings of length n.
@@ -144,14 +160,17 @@
 
 def is_hermitian(mat):
     return np.allclose(mat, mat.T.conj())
 
 def is_unitary(mat):
     return np.allclose(mat @ mat.T.conj(), np.eye(len(mat)))
 
+def is_valid_state(state):
+    # print(state)
+    return np.isclose(sum(np.abs((state**2))), 1)
     
 if __name__ == "__main__":
     # Test Pauli operators
     # pauli_ops = [('IZZZ', 3), ('ZXYI', 2)]
     qubit_op = [('IIIIII', 0.1875), ('IIIIIZ', -0.5625), 
                     ('IIIIZI', -0.0625), ('IIIZII', 0.4375), 
                     ('IIZIII', -0.5625), ('IIZIIZ', 0.0625), 
@@ -193,8 +212,7 @@
         
         i = int(i, 2)
         flipped_i = flip_bit(int(i), c) 
         print(f'{flipped_i:0{n}b}')
         if f'{flipped_i:0{n}b}'[-(c+1)] != '0':
             raise Exception('WRONG')
 
-
```

### Comparing `quanthon-0.3.6.6/Quanthon.egg-info/PKG-INFO` & `quanthon-0.3.7/Quanthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.6.6
+Version: 0.3.7
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.6.6/Quanthon.egg-info/SOURCES.txt` & `quanthon-0.3.7/Quanthon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 Quanthon/Models.py
 Quanthon/__init__.py
 Quanthon/algorithms.py
 Quanthon/ansatzs.py
 Quanthon/base.py
 Quanthon/expectation.py
+Quanthon/history.py
 Quanthon/mappers.py
 Quanthon/mappers_utils.py
 Quanthon/physics.py
 Quanthon/ut_pyscf_mel.py
 Quanthon/ut_qiskit_hamiltonian.py
 Quanthon/ut_test_jw.py
 Quanthon/utils.py
```

### Comparing `quanthon-0.3.6.6/README.md` & `quanthon-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/setup.py` & `quanthon-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.6.6" #####
+version = "0.3.7" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `quanthon-0.3.6.6/tests/test_cmp_qk.py` & `quanthon-0.3.7/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/tests/test_mappers.py` & `quanthon-0.3.7/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.6.6/tests/test_vqes.py` & `quanthon-0.3.7/tests/test_vqes.py`

 * *Files identical despite different names*

