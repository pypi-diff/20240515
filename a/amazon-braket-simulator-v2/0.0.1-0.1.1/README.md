# Comparing `tmp/amazon_braket_simulator_v2-0.0.1.tar.gz` & `tmp/amazon_braket_simulator_v2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_braket_simulator_v2-0.0.1.tar", last modified: Thu May  9 20:31:16 2024, max compression
+gzip compressed data, was "amazon_braket_simulator_v2-0.1.1.tar", last modified: Tue May 14 19:14:27 2024, max compression
```

## Comparing `amazon_braket_simulator_v2-0.0.1.tar` & `amazon_braket_simulator_v2-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 krneta     (504) staff       (20)        0 2024-05-09 20:31:16.680467 amazon_braket_simulator_v2-0.0.1/
--rw-r--r--   0 krneta     (504) staff       (20)    10142 2024-04-24 21:02:58.000000 amazon_braket_simulator_v2-0.0.1/LICENSE
--rw-r--r--   0 krneta     (504) staff       (20)       67 2024-04-24 21:02:58.000000 amazon_braket_simulator_v2-0.0.1/NOTICE
--rw-r--r--   0 krneta     (504) staff       (20)    13008 2024-05-09 20:31:16.680245 amazon_braket_simulator_v2-0.0.1/PKG-INFO
--rw-r--r--   0 krneta     (504) staff       (20)      306 2024-05-09 16:57:30.000000 amazon_braket_simulator_v2-0.0.1/README.md
--rw-r--r--   0 krneta     (504) staff       (20)     1055 2024-05-09 20:23:24.000000 amazon_braket_simulator_v2-0.0.1/pyproject.toml
--rw-r--r--   0 krneta     (504) staff       (20)       26 2024-05-09 20:23:06.000000 amazon_braket_simulator_v2-0.0.1/requirements.txt
--rw-r--r--   0 krneta     (504) staff       (20)      317 2024-05-09 20:31:16.681009 amazon_braket_simulator_v2-0.0.1/setup.cfg
--rw-r--r--   0 krneta     (504) staff       (20)      236 2024-05-08 22:51:16.000000 amazon_braket_simulator_v2-0.0.1/setup.py
-drwxr-xr-x   0 krneta     (504) staff       (20)        0 2024-05-09 20:31:16.666270 amazon_braket_simulator_v2-0.0.1/src/
-drwxr-xr-x   0 krneta     (504) staff       (20)        0 2024-05-09 20:31:16.677531 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/
--rw-r--r--   0 krneta     (504) staff       (20)    13008 2024-05-09 20:31:16.000000 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/PKG-INFO
--rw-r--r--   0 krneta     (504) staff       (20)      451 2024-05-09 20:31:16.000000 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt
--rw-r--r--   0 krneta     (504) staff       (20)        1 2024-05-09 20:31:16.000000 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/dependency_links.txt
--rw-r--r--   0 krneta     (504) staff       (20)      218 2024-05-09 20:31:16.000000 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/requires.txt
--rw-r--r--   0 krneta     (504) staff       (20)        7 2024-05-09 20:31:16.000000 amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/top_level.txt
-drwxr-xr-x   0 krneta     (504) staff       (20)        0 2024-05-09 20:31:16.666427 amazon_braket_simulator_v2-0.0.1/src/braket/
-drwxr-xr-x   0 krneta     (504) staff       (20)        0 2024-05-09 20:31:16.676366 amazon_braket_simulator_v2-0.0.1/src/braket/simulator_v2/
--rw-r--r--   0 krneta     (504) staff       (20)       49 2024-05-09 20:24:41.000000 amazon_braket_simulator_v2-0.0.1/src/braket/simulator_v2/__init__.py
--rw-r--r--   0 krneta     (504) staff       (20)       22 2024-05-09 20:25:32.000000 amazon_braket_simulator_v2-0.0.1/src/braket/simulator_v2/_version.py
--rw-r--r--   0 krneta     (504) staff       (20)       42 2024-05-09 20:23:47.000000 amazon_braket_simulator_v2-0.0.1/src/braket/simulator_v2/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:14:27.376004 amazon_braket_simulator_v2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-14 19:14:27.376004 amazon_braket_simulator_v2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 19:14:27.376004 amazon_braket_simulator_v2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:14:27.372004 amazon_braket_simulator_v2-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:14:27.376004 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 19:14:27.000000 amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:14:27.372004 amazon_braket_simulator_v2-0.1.1/src/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/juliapkg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:14:27.376004 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/base_simulator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/density_matrix_simulator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/julia_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-14 19:14:18.000000 amazon_braket_simulator_v2-0.1.1/src/braket/simulator_v2/state_vector_simulator_v2.py
```

### Comparing `amazon_braket_simulator_v2-0.0.1/LICENSE` & `amazon_braket_simulator_v2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.0.1/PKG-INFO` & `amazon_braket_simulator_v2-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-simulator-v2
-Version: 0.0.1
+Version: 0.1.1
 Summary: Local simulation of quantum circuits
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -182,14 +182,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: juliacall==0.9.19
+Requires-Dist: numpy
+Requires-Dist: amazon-braket-default-simulator>=1.21.2
+Requires-Dist: amazon-braket-schemas>=1.20.2
 Requires-Dist: amazon-braket-sdk>=1.76.0
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: flake8-rst-docstrings; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
@@ -200,23 +204,93 @@
 Requires-Dist: pytest-rerunfailures; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-rtd-theme; extra == "test"
 Requires-Dist: sphinxcontrib-apidoc; extra == "test"
 Requires-Dist: tox; extra == "test"
 
-## My Project
+# Amazon Simulator Version 2
 
-TODO: Fill this README out!
+This Amazon Braket Simulator is a second generation of our Python open source library that provides an
+implementation of a quantum simulators that you can run locally. You can use the simulator to test quantum tasks
+that you construct for the [Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) before you submit them to the Amazon Braket service for execution.
 
-Be sure to:
+## Setting up this Amazon Braket Simulator
+You must have the [Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) installed to use the local simulator.
+Follow the instructions in the [README](https://github.com/amazon-braket/amazon-braket-sdk-python/blob/main/README.md) for setup.
 
-* Change the title in this README
-* Edit your repository description on GitHub
+## Usage
 
+**Running this simulator for the first time will install additional libraries and may take a few additional minutes. 
+This will not be needed for subsequent runs.**
+
+The quantum simulator implementations `StateVectorSimulatorV2` and `DensityMatrixSimulatorV2` plug into the `LocalSimulator` interface in 
+[Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python), with the `backend` parameters as `"braket_sv_v2"` and `"braket_dm_v2"`, respectively.
+
+Executing a circuit using the simulator:
+```python
+from braket.circuits import Circuit
+from braket.devices import LocalSimulator
+
+device = LocalSimulator("braket_sv_v2")
+
+bell = Circuit().h(0).cnot(0, 1)
+print(device.run(bell, shots=100).result().measurement_counts)
+```
+
+## Documentation
+
+Detailed documentation, including the API reference, can be found on [Read the Docs](https://amazon-braket-simulator-v2-python.readthedocs.io/en/latest/)
+
+**To generate the API Reference HTML in your local environment**
+
+First, install tox:
+
+```bash
+pip install tox
+```
+
+To generate the HTML, first change directories (`cd`) to position the cursor in the `amazon-braket-simulator-v2-python`
+directory. Then, run the following command to generate the HTML documentation files:
+
+```bash
+tox -e docs
+```
+
+To view the generated documentation, open the following file in a browser:
+`../amazon-braket-simulator-v2-python/build/documentation/html/index.html`
+
+## Testing
+
+If you want to contribute to the project, be sure to run unit tests and get a successful result 
+before you submit a pull request. To run the unit tests, first install the test dependencies using the following command:
+
+```bash
+pip install -e ".[test]"
+```
+
+To run the unit tests:
+
+```bash
+tox -e unit-tests
+```
+
+You can also pass in various pytest arguments to run selected tests:
+
+```bash
+tox -e unit-tests -- your-arguments
+```
+
+For more information, please see [pytest usage](https://docs.pytest.org/en/stable/usage.html).
+
+To run linters and doc generators and unit tests:
+
+```bash
+tox
+```
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

### Comparing `amazon_braket_simulator_v2-0.0.1/pyproject.toml` & `amazon_braket_simulator_v2-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amazon-braket-simulator-v2"
-version = "0.0.1"
 description = "Local simulation of quantum circuits"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License"
 ]
-dynamic = ["dependencies"]
+dynamic = ["version", "dependencies"]
+
+[project.entry-points."braket.simulators"]
+braket_sv_v2 = "braket.simulator_v2.state_vector_simulator_v2:StateVectorSimulatorV2"
+braket_dm_v2 = "braket.simulator_v2.density_matrix_simulator_v2:DensityMatrixSimulatorV2"
 
 [project.optional-dependencies]
 test = [
     "black",
     "flake8",
     "flake8-rst-docstrings",
     "isort",
```

### Comparing `amazon_braket_simulator_v2-0.0.1/src/amazon_braket_simulator_v2.egg-info/PKG-INFO` & `amazon_braket_simulator_v2-0.1.1/src/amazon_braket_simulator_v2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-simulator-v2
-Version: 0.0.1
+Version: 0.1.1
 Summary: Local simulation of quantum circuits
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -182,14 +182,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: juliacall==0.9.19
+Requires-Dist: numpy
+Requires-Dist: amazon-braket-default-simulator>=1.21.2
+Requires-Dist: amazon-braket-schemas>=1.20.2
 Requires-Dist: amazon-braket-sdk>=1.76.0
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: flake8-rst-docstrings; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
@@ -200,23 +204,93 @@
 Requires-Dist: pytest-rerunfailures; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-rtd-theme; extra == "test"
 Requires-Dist: sphinxcontrib-apidoc; extra == "test"
 Requires-Dist: tox; extra == "test"
 
-## My Project
+# Amazon Simulator Version 2
 
-TODO: Fill this README out!
+This Amazon Braket Simulator is a second generation of our Python open source library that provides an
+implementation of a quantum simulators that you can run locally. You can use the simulator to test quantum tasks
+that you construct for the [Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) before you submit them to the Amazon Braket service for execution.
 
-Be sure to:
+## Setting up this Amazon Braket Simulator
+You must have the [Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) installed to use the local simulator.
+Follow the instructions in the [README](https://github.com/amazon-braket/amazon-braket-sdk-python/blob/main/README.md) for setup.
 
-* Change the title in this README
-* Edit your repository description on GitHub
+## Usage
 
+**Running this simulator for the first time will install additional libraries and may take a few additional minutes. 
+This will not be needed for subsequent runs.**
+
+The quantum simulator implementations `StateVectorSimulatorV2` and `DensityMatrixSimulatorV2` plug into the `LocalSimulator` interface in 
+[Amazon Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python), with the `backend` parameters as `"braket_sv_v2"` and `"braket_dm_v2"`, respectively.
+
+Executing a circuit using the simulator:
+```python
+from braket.circuits import Circuit
+from braket.devices import LocalSimulator
+
+device = LocalSimulator("braket_sv_v2")
+
+bell = Circuit().h(0).cnot(0, 1)
+print(device.run(bell, shots=100).result().measurement_counts)
+```
+
+## Documentation
+
+Detailed documentation, including the API reference, can be found on [Read the Docs](https://amazon-braket-simulator-v2-python.readthedocs.io/en/latest/)
+
+**To generate the API Reference HTML in your local environment**
+
+First, install tox:
+
+```bash
+pip install tox
+```
+
+To generate the HTML, first change directories (`cd`) to position the cursor in the `amazon-braket-simulator-v2-python`
+directory. Then, run the following command to generate the HTML documentation files:
+
+```bash
+tox -e docs
+```
+
+To view the generated documentation, open the following file in a browser:
+`../amazon-braket-simulator-v2-python/build/documentation/html/index.html`
+
+## Testing
+
+If you want to contribute to the project, be sure to run unit tests and get a successful result 
+before you submit a pull request. To run the unit tests, first install the test dependencies using the following command:
+
+```bash
+pip install -e ".[test]"
+```
+
+To run the unit tests:
+
+```bash
+tox -e unit-tests
+```
+
+You can also pass in various pytest arguments to run selected tests:
+
+```bash
+tox -e unit-tests -- your-arguments
+```
+
+For more information, please see [pytest usage](https://docs.pytest.org/en/stable/usage.html).
+
+To run linters and doc generators and unit tests:
+
+```bash
+tox
+```
 ## Security
 
 See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
```

