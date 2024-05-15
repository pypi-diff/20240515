# Comparing `tmp/airbyte_source_pokeapi-0.2.0.dev202405091538.tar.gz` & `tmp/airbyte_source_pokeapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pokeapi-0.2.0.dev202405091538.tar", last modified: Thu May  9 15:38:55 2024, max compression
+gzip compressed data, was "airbyte_source_pokeapi-0.2.1.tar", max compression
```

## Comparing `airbyte_source_pokeapi-0.2.0.dev202405091538.tar` & `airbyte_source_pokeapi-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/
--rw-r--r--   0 root         (0) root         (0)     4211 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4022 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4211 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-09 15:38:55.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/airbyte_source_pokeapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      243 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4091 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      919 2024-05-09 15:38:53.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/
--rw-r--r--   0 root         (0) root         (0)      126 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:38:55.450921 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/schemas/
--rw-r--r--   0 root         (0) root         (0)     8544 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/schemas/pokemon.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/source.py
--rw-r--r--   0 root         (0) root         (0)    17094 2024-05-09 08:04:30.000000 airbyte_source_pokeapi-0.2.0.dev202405091538/source_pokeapi/spec.yaml
+-rw-r--r--   0        0        0     4527 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/README.md
+-rw-r--r--   0        0        0      135 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/main.py
+-rw-r--r--   0        0        0      761 2024-05-15 15:25:43.988231 airbyte_source_pokeapi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/__init__.py
+-rw-r--r--   0        0        0    29310 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/run.py
+-rw-r--r--   0        0        0      476 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/source.py
+-rw-r--r--   0        0        0     5232 1970-01-01 00:00:00.000000 airbyte_source_pokeapi-0.2.1/PKG-INFO
```

### Comparing `airbyte_source_pokeapi-0.2.0.dev202405091538/PKG-INFO` & `airbyte_source_pokeapi-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pokeapi
-Version: 0.2.0.dev202405091538
-Summary: Source implementation for Pokeapi.
+Version: 0.2.1
+Summary: Source implementation for pokeapi.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pokeapi
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Pokeapi Source
 
 This is the repository for the Pokeapi configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pokeapi).
 
+## Local development
 
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pokeapi)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pokeapi/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `source_pokeapi/manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pokeapi test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-pokeapi spec
+poetry run source-pokeapi check --config secrets/config.json
+poetry run source-pokeapi discover --config secrets/config.json
+poetry run source-pokeapi read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Running tests
 
-```bash
-airbyte-ci connectors --name=source-pokeapi build
-```
+To run tests locally, from the connector directory run:
 
-An image will be built with the tag `airbyte/source-pokeapi:dev`.
+```
+poetry run pytest tests
+```
 
-**Via `docker build`:**
+### Building the docker image
 
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-pokeapi:dev .
+airbyte-ci connectors --name=source-pokeapi build
 ```
 
+An image will be available on your host with the tag `airbyte/source-pokeapi:dev`.
 
-Then run any of the connector commands as follows:
 
+### Running as a docker container
+
+Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pokeapi:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pokeapi:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pokeapi:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pokeapi:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
-
 ```bash
 airbyte-ci connectors --name=source-pokeapi test
 ```
 
+### Customizing acceptance Tests
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
+### Dependency Management
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-- required for the testing need to go to `TEST_REQUIREMENTS` list
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
-
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pokeapi test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pokeapi.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pokeapi.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_pokeapi-0.2.0.dev202405091538/README.md` & `airbyte_source_pokeapi-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,103 @@
 # Pokeapi Source
 
 This is the repository for the Pokeapi configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pokeapi).
 
 ## Local development
 
-#### Create credentials
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pokeapi)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pokeapi/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `source_pokeapi/manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pokeapi test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
 
-#### Build
+```
+poetry run source-pokeapi spec
+poetry run source-pokeapi check --config secrets/config.json
+poetry run source-pokeapi discover --config secrets/config.json
+poetry run source-pokeapi read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Running tests
 
-```bash
-airbyte-ci connectors --name=source-pokeapi build
-```
+To run tests locally, from the connector directory run:
 
-An image will be built with the tag `airbyte/source-pokeapi:dev`.
+```
+poetry run pytest tests
+```
 
-**Via `docker build`:**
+### Building the docker image
 
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-pokeapi:dev .
+airbyte-ci connectors --name=source-pokeapi build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-pokeapi:dev`.
 
-Then run any of the connector commands as follows:
 
+### Running as a docker container
+
+Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pokeapi:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pokeapi:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pokeapi:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pokeapi:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
-
 ```bash
 airbyte-ci connectors --name=source-pokeapi test
 ```
 
 ### Customizing acceptance Tests
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
+### Dependency Management
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-- required for the testing need to go to `TEST_REQUIREMENTS` list
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
-
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pokeapi test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pokeapi.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pokeapi.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

