# Comparing `tmp/poetry_dockerize_plugin-0.6.1.tar.gz` & `tmp/poetry_dockerize_plugin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dockerize_plugin-0.6.1.tar", max compression
+gzip compressed data, was "poetry_dockerize_plugin-1.0.0.tar", max compression
```

## Comparing `poetry_dockerize_plugin-0.6.1.tar` & `poetry_dockerize_plugin-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/LICENSE
--rw-r--r--   0        0        0     4471 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/README.md
--rw-r--r--   0        0        0        0 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/__init__.py
--rw-r--r--   0        0        0    13196 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/builder.py
--rw-r--r--   0        0        0     1239 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/plugin.py
--rw-r--r--   0        0        0     1997 2024-05-14 10:39:56.962105 poetry_dockerize_plugin-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4734 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/poetry_dockerize_plugin/__init__.py
+-rw-r--r--   0        0        0    13499 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/poetry_dockerize_plugin/builder.py
+-rw-r--r--   0        0        0     1239 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/poetry_dockerize_plugin/plugin.py
+-rw-r--r--   0        0        0     1997 2024-05-14 13:27:39.098034 poetry_dockerize_plugin-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6563 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-1.0.0/PKG-INFO
```

### Comparing `poetry_dockerize_plugin-0.6.1/LICENSE` & `poetry_dockerize_plugin-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.6.1/README.md` & `poetry_dockerize_plugin-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -97,29 +97,34 @@
 labels = {"MY_APP_LABEL" = "dev"}
 apt-packages = ["curl"]
 extra-run-instructions = ["RUN curl https://huggingface.co/transformers/"]
 
 # Only for build docker layer
 build-apt-packages = ["gcc"]
 extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
+build-poetry-install-args = ["-E", "all", "--no-root"]
 
 ```
 
 * `name` customizes the docker image name. 
 * `python` python version to use. If not specified, will try to be extracted from `tool.poetry.dependencies.python`. Default is `3.11`
 * `base-image` customizes the base image. If not defined, the default base image is `python:<python-version>-slim-buster`. 
 * `tags` declares a list of tags for the image.
 * `entrypoint` customizes the entrypoint of the image. If not provided, the default entrypoint is retrieved from the `packages` configuration.
 * `ports` exposes ports
 * `env` declares environment variables inside the docker image.
 * `labels` append labels to the docker image. Default labels are added following the opencontainers specification.
 * `apt-packages` installs apt packages inside the docker image.
-* `extra-build-instructions` adds extra instructions to the docker build (before poetry install). Any modification to the filesystem will be lost after the poetry install. If you need to add files to the image, use the `extra-run-instructions`.
 * `extra-run-instructions` adds extra instructions to the docker run (after poetry install). Any modification to the filesystem will be kept after the poetry install.
 
+For the build step:
+* `build-apt-packages` installs apt packages inside the build docker container.
+* `extra-build-instructions` adds extra instructions to the docker build (before poetry install). Any modification to the filesystem will be lost after the poetry install. If you need to add files to the image, use the `extra-run-instructions`.
+* `build-poetry-install-args` adds additional arguments to the `poetry install` command in the build step.
+
 
 ## Command-Line options
 
 All command line options provided by the `poetry-dockerize-plugin` may be accessed by typing:
 
 ```bash
 poetry dockerize --help
```

#### html2text {}

```diff
@@ -22,30 +22,33 @@
 Configuration API Reference This examples shows a complete configuration of the
 docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
 "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
 ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
 = {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
 ["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
 build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
-http-basic.foo "] ``` * `name` customizes the docker image name. * `python`
-python version to use. If not specified, will try to be extracted from
-`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
-the base image. If not defined, the default base image is `python:-slim-
-buster`. * `tags` declares a list of tags for the image. * `entrypoint`
-customizes the entrypoint of the image. If not provided, the default entrypoint
-is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
-declares environment variables inside the docker image. * `labels` append
-labels to the docker image. Default labels are added following the
-opencontainers specification. * `apt-packages` installs apt packages inside the
-docker image. * `extra-build-instructions` adds extra instructions to the
-docker build (before poetry install). Any modification to the filesystem will
-be lost after the poetry install. If you need to add files to the image, use
-the `extra-run-instructions`. * `extra-run-instructions` adds extra
-instructions to the docker run (after poetry install). Any modification to the
-filesystem will be kept after the poetry install. ## Command-Line options All
-command line options provided by the `poetry-dockerize-plugin` may be accessed
-by typing: ```bash poetry dockerize --help ``` ## Troubleshooting To
-troubleshoot the plugin, you can use the `--debug` flag to get more information
-about the execution. ```bash poetry dockerize --debug ``` ## Generate
-Dockerfile To store the generated Dockerfile, you can use the `--generate`
-flag. ```bash poetry dockerize --generate ``` ## License This project is
-licensed under the terms of the MIT license.
+http-basic.foo "] build-poetry-install-args = ["-E", "all", "--no-root"] ``` *
+`name` customizes the docker image name. * `python` python version to use. If
+not specified, will try to be extracted from `tool.poetry.dependencies.python`.
+Default is `3.11` * `base-image` customizes the base image. If not defined, the
+default base image is `python:-slim-buster`. * `tags` declares a list of tags
+for the image. * `entrypoint` customizes the entrypoint of the image. If not
+provided, the default entrypoint is retrieved from the `packages`
+configuration. * `ports` exposes ports * `env` declares environment variables
+inside the docker image. * `labels` append labels to the docker image. Default
+labels are added following the opencontainers specification. * `apt-packages`
+installs apt packages inside the docker image. * `extra-run-instructions` adds
+extra instructions to the docker run (after poetry install). Any modification
+to the filesystem will be kept after the poetry install. For the build step: *
+`build-apt-packages` installs apt packages inside the build docker container. *
+`extra-build-instructions` adds extra instructions to the docker build (before
+poetry install). Any modification to the filesystem will be lost after the
+poetry install. If you need to add files to the image, use the `extra-run-
+instructions`. * `build-poetry-install-args` adds additional arguments to the
+`poetry install` command in the build step. ## Command-Line options All command
+line options provided by the `poetry-dockerize-plugin` may be accessed by
+typing: ```bash poetry dockerize --help ``` ## Troubleshooting To troubleshoot
+the plugin, you can use the `--debug` flag to get more information about the
+execution. ```bash poetry dockerize --debug ``` ## Generate Dockerfile To store
+the generated Dockerfile, you can use the `--generate` flag. ```bash poetry
+dockerize --generate ``` ## License This project is licensed under the terms of
+the MIT license.
```

### Comparing `poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/builder.py` & `poetry_dockerize_plugin-1.0.0/poetry_dockerize_plugin/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,29 @@
     entrypoint_cmd: List[str] = []
     python: str = ""
     ports: List[int] = []
     envs: dict[str, str] = {}
     labels: dict[str, str] = {}
     apt_packages: List[str] = []
     build_apt_packages: List[str] = []
+    build_poetry_install_args: List[str] = []
     base_image: str = ""
     extra_build_instructions: List[str] = []
     extra_runtime_instructions: List[str] = []
 
 
 class ProjectConfiguration:
     image_name: str
     image_tags: List[str]
     entrypoint: List[str]
     ports: List[int] = []
     envs: dict[str, str] = {}
     labels: dict[str, str]
     build_apt_packages: List[str] = []
+    build_poetry_install_args: List[str] = []
     runtime_apt_packages: List[str] = []
     base_image: str = ""
     extra_build_instructions: List[str] = []
     extra_runtime_instructions: List[str] = []
     deps_packages: List[str] = []
     app_packages: List[str] = []
 
@@ -61,14 +63,15 @@
     config.entrypoint_cmd = get_list_or_str_from_dict(dict, "entrypoint", split_by=" ")
     config.python = dict.get("python")
     config.ports = dict.get("ports")
     config.envs = dict.get("env")
     config.labels = dict.get("labels")
     config.apt_packages = dict.get("apt-packages")
     config.build_apt_packages = dict.get("build-apt-packages")
+    config.build_poetry_install_args = dict.get("build-poetry-install-args")
     config.base_image = dict.get("base-image")
     config.extra_build_instructions = dict.get("extra-build-instructions")
     config.extra_runtime_instructions = dict.get("extra-runtime-instructions")
     return config
 
 
 def extract_python_version(pyversion: str) -> Optional[str]:
@@ -114,14 +117,15 @@
             config.entrypoint = ["python", "-m", name]
 
     if not config.entrypoint:
         raise ValueError('No package found in pyproject.toml and no entrypoint specified in dockerize section')
 
     config.runtime_apt_packages = dockerize_section.apt_packages or []
     config.build_apt_packages = dockerize_section.build_apt_packages or []
+    config.build_poetry_install_args = dockerize_section.build_poetry_install_args or []
     if 'packages' in tool_poetry:
         config.app_packages += [package["include"] for package in tool_poetry['packages']]
 
     if "dependencies" in tool_poetry:
         for dep in tool_poetry["dependencies"]:
             if isinstance(tool_poetry["dependencies"][dep], dict):
                 if 'path' in tool_poetry["dependencies"][dep]:
@@ -222,15 +226,15 @@
 
 {generate_apt_packages_str(config.build_apt_packages)}
 {generate_add_project_toml_str(config, real_context_path)}
 
 {generate_add_packages_str(config, real_context_path)}
 {generate_extra_instructions_str(config.extra_build_instructions)}
 
-RUN cd /app && poetry install --no-interaction --no-ansi
+RUN cd /app && poetry install --no-interaction --no-ansi {" ".join(config.build_poetry_install_args)}
 
 FROM {config.base_image} as runtime
 {generate_apt_packages_str(config.runtime_apt_packages)}
 {labels_str}
 
 ENV PATH="/app/.venv/bin:$PATH"
 ENV PYTHONUNBUFFERED=1
```

### Comparing `poetry_dockerize_plugin-0.6.1/poetry_dockerize_plugin/plugin.py` & `poetry_dockerize_plugin-1.0.0/poetry_dockerize_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.6.1/pyproject.toml` & `poetry_dockerize_plugin-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dockerize-plugin"
-version = "0.6.1"
+version = "1.0.0"
 description = "Poetry application to Docker, automatically."
 authors = ["Nicolò Boschi <boschi1997@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["poetry", "packaging", "docker"]
 repository = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
 documentation = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
```

### Comparing `poetry_dockerize_plugin-0.6.1/PKG-INFO` & `poetry_dockerize_plugin-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dockerize-plugin
-Version: 0.6.1
+Version: 1.0.0
 Summary: Poetry application to Docker, automatically.
 Home-page: https://github.com/nicoloboschi/poetry-dockerize-plugin
 License: MIT
 Keywords: poetry,packaging,docker
 Author: Nicolò Boschi
 Author-email: boschi1997@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -136,29 +136,34 @@
 labels = {"MY_APP_LABEL" = "dev"}
 apt-packages = ["curl"]
 extra-run-instructions = ["RUN curl https://huggingface.co/transformers/"]
 
 # Only for build docker layer
 build-apt-packages = ["gcc"]
 extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
+build-poetry-install-args = ["-E", "all", "--no-root"]
 
 ```
 
 * `name` customizes the docker image name. 
 * `python` python version to use. If not specified, will try to be extracted from `tool.poetry.dependencies.python`. Default is `3.11`
 * `base-image` customizes the base image. If not defined, the default base image is `python:<python-version>-slim-buster`. 
 * `tags` declares a list of tags for the image.
 * `entrypoint` customizes the entrypoint of the image. If not provided, the default entrypoint is retrieved from the `packages` configuration.
 * `ports` exposes ports
 * `env` declares environment variables inside the docker image.
 * `labels` append labels to the docker image. Default labels are added following the opencontainers specification.
 * `apt-packages` installs apt packages inside the docker image.
-* `extra-build-instructions` adds extra instructions to the docker build (before poetry install). Any modification to the filesystem will be lost after the poetry install. If you need to add files to the image, use the `extra-run-instructions`.
 * `extra-run-instructions` adds extra instructions to the docker run (after poetry install). Any modification to the filesystem will be kept after the poetry install.
 
+For the build step:
+* `build-apt-packages` installs apt packages inside the build docker container.
+* `extra-build-instructions` adds extra instructions to the docker build (before poetry install). Any modification to the filesystem will be lost after the poetry install. If you need to add files to the image, use the `extra-run-instructions`.
+* `build-poetry-install-args` adds additional arguments to the `poetry install` command in the build step.
+
 
 ## Command-Line options
 
 All command line options provided by the `poetry-dockerize-plugin` may be accessed by typing:
 
 ```bash
 poetry dockerize --help
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 0.6.1 Summary:
+Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 1.0.0 Summary:
 Poetry application to Docker, automatically. Home-page: https://github.com/
 nicoloboschi/poetry-dockerize-plugin License: MIT Keywords:
 poetry,packaging,docker Author: NicolÃ² Boschi Author-email:
 boschi1997@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
@@ -46,30 +46,33 @@
 Configuration API Reference This examples shows a complete configuration of the
 docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
 "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
 ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
 = {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
 ["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
 build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
-http-basic.foo "] ``` * `name` customizes the docker image name. * `python`
-python version to use. If not specified, will try to be extracted from
-`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
-the base image. If not defined, the default base image is `python:-slim-
-buster`. * `tags` declares a list of tags for the image. * `entrypoint`
-customizes the entrypoint of the image. If not provided, the default entrypoint
-is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
-declares environment variables inside the docker image. * `labels` append
-labels to the docker image. Default labels are added following the
-opencontainers specification. * `apt-packages` installs apt packages inside the
-docker image. * `extra-build-instructions` adds extra instructions to the
-docker build (before poetry install). Any modification to the filesystem will
-be lost after the poetry install. If you need to add files to the image, use
-the `extra-run-instructions`. * `extra-run-instructions` adds extra
-instructions to the docker run (after poetry install). Any modification to the
-filesystem will be kept after the poetry install. ## Command-Line options All
-command line options provided by the `poetry-dockerize-plugin` may be accessed
-by typing: ```bash poetry dockerize --help ``` ## Troubleshooting To
-troubleshoot the plugin, you can use the `--debug` flag to get more information
-about the execution. ```bash poetry dockerize --debug ``` ## Generate
-Dockerfile To store the generated Dockerfile, you can use the `--generate`
-flag. ```bash poetry dockerize --generate ``` ## License This project is
-licensed under the terms of the MIT license.
+http-basic.foo "] build-poetry-install-args = ["-E", "all", "--no-root"] ``` *
+`name` customizes the docker image name. * `python` python version to use. If
+not specified, will try to be extracted from `tool.poetry.dependencies.python`.
+Default is `3.11` * `base-image` customizes the base image. If not defined, the
+default base image is `python:-slim-buster`. * `tags` declares a list of tags
+for the image. * `entrypoint` customizes the entrypoint of the image. If not
+provided, the default entrypoint is retrieved from the `packages`
+configuration. * `ports` exposes ports * `env` declares environment variables
+inside the docker image. * `labels` append labels to the docker image. Default
+labels are added following the opencontainers specification. * `apt-packages`
+installs apt packages inside the docker image. * `extra-run-instructions` adds
+extra instructions to the docker run (after poetry install). Any modification
+to the filesystem will be kept after the poetry install. For the build step: *
+`build-apt-packages` installs apt packages inside the build docker container. *
+`extra-build-instructions` adds extra instructions to the docker build (before
+poetry install). Any modification to the filesystem will be lost after the
+poetry install. If you need to add files to the image, use the `extra-run-
+instructions`. * `build-poetry-install-args` adds additional arguments to the
+`poetry install` command in the build step. ## Command-Line options All command
+line options provided by the `poetry-dockerize-plugin` may be accessed by
+typing: ```bash poetry dockerize --help ``` ## Troubleshooting To troubleshoot
+the plugin, you can use the `--debug` flag to get more information about the
+execution. ```bash poetry dockerize --debug ``` ## Generate Dockerfile To store
+the generated Dockerfile, you can use the `--generate` flag. ```bash poetry
+dockerize --generate ``` ## License This project is licensed under the terms of
+the MIT license.
```

