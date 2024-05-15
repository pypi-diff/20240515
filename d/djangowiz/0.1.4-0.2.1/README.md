# Comparing `tmp/djangowiz-0.1.4.tar.gz` & `tmp/djangowiz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangowiz-0.1.4.tar", max compression
+gzip compressed data, was "djangowiz-0.2.1.tar", max compression
```

## Comparing `djangowiz-0.1.4.tar` & `djangowiz-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-05-14 04:51:54.451239 djangowiz-0.1.4/LICENSE
--rw-r--r--   0        0        0     3176 2024-05-14 04:51:54.451239 djangowiz-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-14 04:51:54.447239 djangowiz-0.1.4/djangowiz/__init__.py
--rw-r--r--   0        0        0     8218 2024-05-14 06:23:39.787520 djangowiz-0.1.4/djangowiz/generate.py
--rw-r--r--   0        0        0      472 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/Dockerfile.j2
--rw-r--r--   0        0        0      477 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/docker-compose.dev.yml.j2
--rw-r--r--   0        0        0      474 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/docker-compose.prod.yml.j2
--rw-r--r--   0        0        0       92 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/env.dev.j2
--rw-r--r--   0        0        0       93 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/env.prod.j2
--rw-r--r--   0        0        0      416 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/routes.py.j2
--rw-r--r--   0        0        0      229 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/serializer.py.j2
--rw-r--r--   0        0        0      138 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/urls.py.j2
--rw-r--r--   0        0        0      678 2024-05-14 04:51:54.451239 djangowiz-0.1.4/djangowiz/templates/viewset.py.j2
--rw-r--r--   0        0        0      829 2024-05-14 05:15:46.933115 djangowiz-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 djangowiz-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 04:51:54.451239 djangowiz-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4559 2024-05-15 14:46:16.352721 djangowiz-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 04:51:54.447239 djangowiz-0.2.1/djangowiz/__init__.py
+-rw-r--r--   0        0        0     3068 2024-05-15 12:36:29.463156 djangowiz-0.2.1/djangowiz/cli.py
+-rw-r--r--   0        0        0     7575 2024-05-15 13:59:13.591487 djangowiz-0.2.1/djangowiz/core.py
+-rw-r--r--   0        0        0      472 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      477 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/docker-compose.dev.yml.j2
+-rw-r--r--   0        0        0      474 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/docker-compose.prod.yml.j2
+-rw-r--r--   0        0        0       92 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/env.dev.j2
+-rw-r--r--   0        0        0       93 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/env.prod.j2
+-rw-r--r--   0        0        0      230 2024-05-15 10:36:24.947850 djangowiz-0.2.1/djangowiz/templates/multi/serializers.py.j2
+-rw-r--r--   0        0        0      609 2024-05-15 10:36:49.601144 djangowiz-0.2.1/djangowiz/templates/multi/viewsets.py.j2
+-rw-r--r--   0        0        0      416 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/routes.py.j2
+-rw-r--r--   0        0        0      188 2024-05-15 13:46:13.375896 djangowiz-0.2.1/djangowiz/templates/single/serializers.py.j2
+-rw-r--r--   0        0        0      402 2024-05-15 13:46:30.168354 djangowiz-0.2.1/djangowiz/templates/single/viewsets.py.j2
+-rw-r--r--   0        0        0      138 2024-05-14 04:51:54.451239 djangowiz-0.2.1/djangowiz/templates/urls.py.j2
+-rw-r--r--   0        0        0      824 2024-05-15 14:48:42.077125 djangowiz-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5433 1970-01-01 00:00:00.000000 djangowiz-0.2.1/PKG-INFO
```

### Comparing `djangowiz-0.1.4/LICENSE` & `djangowiz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangowiz-0.1.4/README.md` & `djangowiz-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,152 @@
-# DjangoWiz
+@@**_⚠️ Caution: This library is under heavy development and is not ready for production._**
 
-DjangoWiz is a simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects. This toolkit helps you quickly scaffold out necessary files based on your models, saving you time and effort.
+@@# DjangoWiz
 
-## Features
+@@DjangoWiz is a simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects. This toolkit helps you quickly scaffold out necessary files based on your models, saving you time and effort.
 
-- Automatically generates serializers, viewsets, and URLs based on your Django models.
-- Supports generation of Dockerfile and Docker Compose configurations for development and production environments.
-- Skips non-serializable classes and abstract models.
-- Includes customizable templates using Jinja2.
-- Provides flexible commands to generate different components individually or all together.
+@@## Features
 
-## Installation
+@@- Automatically generates serializers, viewsets, and URLs based on your Django models.
+@@- Supports generation of Dockerfile and Docker Compose configurations for development and production environments.
+@@- Skips non-serializable classes and abstract models.
+@@- Includes customizable templates using Jinja2.
+@@- Provides flexible commands to generate different components individually or all together.
+@@- Supports custom templates and single file mode.
+@@- Can be used in other Python scripts.
 
-1. **Install via pip:**
-    ```bash
-    pip install DjangoWiz
-    ```
+@@## Installation
 
-2. **Alternatively, clone the repository:**
-    ```bash
-    git clone https://github.com/yourusername/DjangoWiz.git
-    cd DjangoWiz
-    ```
+@@1. **Install via pip:**
+@@    ```bash
+@@    pip install DjangoWiz
+@@    ```
 
-3. **Install dependencies:**
-    Ensure you have Python and Poetry installed, then run:
-    ```bash
-    poetry install
-    ```
+@@2. **Alternatively, clone the repository:**
+@@    ```bash
+@@    git clone https://github.com/tavallie/DjangoWiz.git
+@@    cd DjangoWiz
+@@    ```
 
-## Usage
+@@3. **Install dependencies:**
+@@    Ensure you have Python and Poetry installed, then run:
+@@    ```bash
+@@    poetry install
+@@    ```
 
-### Generate All Files
+@@## Usage
 
-Generate serializers, viewsets, routes, URLs, Dockerfile, and Docker Compose configurations:
+@@### Generate All Files
 
-```bash
-djangowiz generate-files <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@Generate serializers, viewsets, routes, URLs, Dockerfile, and Docker Compose configurations:
 
-### Generate Core Files Only
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-Generate serializers, viewsets, and routes without Docker-related files:
+@@### Generate Core Files Only
 
-```bash
-djangowiz generate_core_files <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@Generate serializers, viewsets, and routes without Docker-related files:
 
-### Generate Individual Components
+@@```bash
+@@djangowiz generate_core_files <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-#### Generate Serializers
+@@### Generate Individual Components
 
-```bash
-djangowiz generate_serializers <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Serializers
 
-#### Generate Viewsets
+@@```bash
+@@djangowiz generate_serializers <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_viewsets <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Viewsets
 
-#### Generate URLs
+@@```bash
+@@djangowiz generate_viewsets <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_urls <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate URLs
 
-#### Generate Routes
+@@```bash
+@@djangowiz generate_urls <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_routes <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Routes
 
-## Directory Structure
+@@```bash
+@@djangowiz generate_routes <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-Ensure your project directory is structured as follows:
+@@### Using Custom Templates
 
-```
-DjangoWiz/
-├── DjangoWiz/
-│   ├── __init__.py
-│   ├── generate.py
-│   ├── templates/
-│       ├── docker-compose.dev.yml.j2
-│       ├── docker-compose.prod.yml.j2
-│       ├── Dockerfile.j2
-│       ├── env.dev.j2
-│       ├── env.prod.j2
-│       ├── serializer.py.j2
-│       ├── viewset.py.j2
-│       ├── urls.py.j2
-│       ├── routes.py.j2
-├── pyproject.toml
-├── README.md
-├── LICENSE
-```
+@@You can specify a custom template directory with the `--template-dir` option. If a custom template is not provided, the default templates will be used.
 
-## Customizing Templates
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite --template-dir path/to/custom_templates
+@@```
 
-The templates used for generating files are located in the `DjangoWiz/templates` directory. You can customize these templates to fit your project's specific requirements. The templates use Jinja2 for rendering.
+@@### Using Single File Mode
 
-## License
+@@You can generate all serializers and viewsets in a single file using the `--single-file` option.
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite --single-file
+@@```
 
-## Contributing
+@@### Using as a Python Library
 
-Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.
+@@You can use DjangoWiz in your own Python scripts:
 
-## Author
+@@```python
+@@from djangowiz.core import ModelExtractor, ProjectGenerator
 
-Ali Tavallaie - [a.tavallaie@gmail.com](mailto:a.tavallaie@gmail.com)
+@@model_file = 'path/to/models.py'
+@@model_names = ModelExtractor.extract_model_names(model_file)
+@@generator = ProjectGenerator('your_app', 'your_project', model_names, template_dir='path/to/custom_templates')
+@@generator.generate_all(single_file=True, overwrite=True)
+@@```
 
----
+@@## Directory Structure
 
-Happy coding!
+@@Ensure your project directory is structured as follows:
+
+@@```
+@@DjangoWiz/
+@@├── djangowiz/
+@@│   ├── __init__.py
+@@│   ├── core.py
+@@│   ├── cli.py
+@@│   ├── templates/
+@@│       ├── docker-compose.dev.yml.j2
+@@│       ├── docker-compose.prod.yml.j2
+@@│       ├── Dockerfile.j2
+@@│       ├── env.dev.j2
+@@│       ├── env.prod.j2
+@@│       ├── serializer.py.j2
+@@│       ├── viewset.py.j2
+@@│       ├── urls.py.j2
+@@│       ├── routes.py.j2
+@@├── pyproject.toml
+@@├── README.md
+@@├── LICENSE
+@@```
+
+@@## Customizing Templates
+
+@@The templates used for generating files are located in the `djangowiz/templates` directory. You can customize these templates to fit your project's specific requirements. The templates use Jinja2 for rendering.
+
+@@## License
+
+@@This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
+@@## Contributing
+
+@@Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.
+
+@@## Author
+
+@@Ali Tavallaie - [a.tavallaie@gmail.com](mailto:a.tavallaie@gmail.com)
+
+@@---
+
+@@Happy coding!
```

### Comparing `djangowiz-0.1.4/djangowiz/generate.py` & `djangowiz-0.2.1/djangowiz/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import os
-import re
-import typer
-from jinja2 import Environment, FileSystemLoader
-from typing import List
 import ast
-
-
-app = typer.Typer()
+from jinja2 import Environment, FileSystemLoader, ChoiceLoader
+from typing import List
 
 
 class ModelExtractor:
     @staticmethod
     def extract_model_names(file_path: str) -> List[str]:
         model_names = []
         with open(file_path, "r") as file:
@@ -23,74 +18,107 @@
                 ]
                 if "Model" in bases or any(base for base in bases):
                     model_names.append(node.name)
         return model_names
 
 
 class ProjectGenerator:
-    def __init__(self, app_name: str, project_name: str, model_names: List[str]):
+    def __init__(
+        self,
+        app_name: str,
+        project_name: str,
+        model_names: List[str],
+        template_dir: str = None,
+    ):
         self.app_name = app_name
         self.project_name = project_name
         self.model_names = model_names
-        self.env = Environment(
-            loader=FileSystemLoader(
-                os.path.join(os.path.dirname(__file__), "templates")
-            )
-        )
+
+        # Use default template directory if no custom template directory is provided
+        default_template_dir = os.path.join(os.path.dirname(__file__), "templates")
+        loaders = [FileSystemLoader(default_template_dir)]
+        if template_dir:
+            loaders.insert(0, FileSystemLoader(template_dir))
+        self.env = Environment(loader=ChoiceLoader(loaders))
 
     def write_file(self, file_path: str, content: str, overwrite: bool = False):
         if not overwrite and os.path.exists(file_path):
             print(f"Skipping existing file: {file_path}")
             return
         os.makedirs(os.path.dirname(file_path), exist_ok=True)
         with open(file_path, "w") as file:
             file.write(content)
         print(f"Generated file: {file_path}")
 
-    def generate_serializers(self, overwrite: bool = False):
-        for model_name in self.model_names:
-            template = self.env.get_template("serializer.py.j2")
-            content = template.render(app_name=self.app_name, model_name=model_name)
+    def generate_serializers(self, single_file: bool, overwrite: bool = False):
+        if single_file:
+            imports = f'from rest_framework import serializers\nfrom {self.app_name}.models import {", ".join(self.model_names)}\n\n'
+            template = self.env.get_template("single/serializers.py.j2")
+            content = imports + template.render(
+                app_name=self.app_name, model_names=self.model_names
+            )
+            self.write_file(
+                os.path.join(self.app_name, "serializers.py"), content, overwrite
+            )
+        else:
+            for model_name in self.model_names:
+                template = self.env.get_template("multi/serializers.py.j2")
+                content = template.render(app_name=self.app_name, model_name=model_name)
+                self.write_file(
+                    os.path.join(
+                        self.app_name, "serializers", f"{model_name.lower()}.py"
+                    ),
+                    content,
+                    overwrite,
+                )
+            serializer_init_content = "\n".join(
+                [
+                    f"from .{model_name.lower()} import {model_name}Serializer"
+                    for model_name in self.model_names
+                ]
+            )
             self.write_file(
-                os.path.join(self.app_name, "serializers", f"{model_name.lower()}.py"),
-                content,
+                os.path.join(self.app_name, "serializers", "__init__.py"),
+                serializer_init_content,
                 overwrite,
             )
-        serializer_init_content = "\n".join(
-            [
-                f"from .{model_name.lower()} import {model_name}Serializer"
-                for model_name in self.model_names
-            ]
-        )
-        self.write_file(
-            os.path.join(self.app_name, "serializers", "__init__.py"),
-            serializer_init_content,
-            overwrite,
-        )
 
-    def generate_viewsets(self, overwrite: bool = False):
-        for model_name in self.model_names:
-            template = self.env.get_template("viewset.py.j2")
-            content = template.render(app_name=self.app_name, model_name=model_name)
+    def generate_viewsets(self, single_file: bool, overwrite: bool = False):
+        if single_file:
+            model_imports = f'from rest_framework import generics\nfrom {self.app_name}.models import {", ".join(self.model_names)}\n'
+            serializer_imports = f'from {self.app_name}.serializers import {", ".join([model_name + "Serializer" for model_name in self.model_names])}\n\n'
+            template = self.env.get_template("single/viewsets.py.j2")
+            content = (
+                model_imports
+                + serializer_imports
+                + template.render(app_name=self.app_name, model_names=self.model_names)
+            )
+            self.write_file(
+                os.path.join(self.app_name, "viewsets.py"), content, overwrite
+            )
+        else:
+            for model_name in self.model_names:
+                template = self.env.get_template("multi/viewsets.py.j2")
+                content = template.render(app_name=self.app_name, model_name=model_name)
+                self.write_file(
+                    os.path.join(self.app_name, "viewsets", f"{model_name.lower()}.py"),
+                    content,
+                    overwrite,
+                )
+            viewset_init_content = "\n".join(
+                [
+                    f"from .{model_name.lower()} import {model_name}ListCreateAPIView, {model_name}RetrieveUpdateDestroyAPIView"
+                    for model_name in self.model_names
+                ]
+            )
             self.write_file(
-                os.path.join(self.app_name, "viewsets", f"{model_name.lower()}.py"),
-                content,
+                os.path.join(self.app_name, "viewsets", "__init__.py"),
+                viewset_init_content,
                 overwrite,
             )
-        viewset_init_content = "\n".join(
-            [
-                f"from .{model_name.lower()} import {model_name}ListCreateAPIView, {model_name}RetrieveUpdateDestroyAPIView"
-                for model_name in self.model_names
-            ]
-        )
-        self.write_file(
-            os.path.join(self.app_name, "viewsets", "__init__.py"),
-            viewset_init_content,
-            overwrite,
-        )
 
     def generate_urls(self, overwrite: bool = False):
         template = self.env.get_template("urls.py.j2")
         content = template.render(app_name=self.app_name, model_names=self.model_names)
         self.write_file(os.path.join(self.app_name, "urls.py"), content, overwrite)
 
     def generate_routes(self, overwrite: bool = False):
@@ -122,17 +150,17 @@
         for env in ["dev", "prod"]:
             template = self.env.get_template(f"env.{env}.j2")
             content = template.render(
                 db_name=db_name, db_user=db_user, db_password=db_password
             )
             self.write_file(f".env.{env}", content, overwrite)
 
-    def generate_all(self, overwrite: bool = False):
-        self.generate_serializers(overwrite)
-        self.generate_viewsets(overwrite)
+    def generate_all(self, single_file: bool, overwrite: bool = False):
+        self.generate_serializers(single_file, overwrite)
+        self.generate_viewsets(single_file, overwrite)
         self.generate_urls(overwrite)
         self.generate_routes(overwrite)
         self.generate_dockerfile(overwrite)
         self.generate_docker_compose(
             db_name="your_db",
             db_user="your_user",
             db_password="your_password",
@@ -141,83 +169,11 @@
         self.generate_env_files(
             db_name="your_db",
             db_user="your_user",
             db_password="your_password",
             overwrite=overwrite,
         )
 
-    def generate_core_files(self, overwrite: bool = False):
-        self.generate_serializers(overwrite)
-        self.generate_viewsets(overwrite)
+    def generate_core_files(self, single_file: bool, overwrite: bool = False):
+        self.generate_serializers(single_file, overwrite)
+        self.generate_viewsets(single_file, overwrite)
         self.generate_routes(overwrite)
-
-
-@app.command()
-def generate_files(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_all(overwrite)
-    print(
-        f"Files for {len(model_names)} models have been generated in the {app_name} directory."
-    )
-
-
-@app.command()
-def generate_core_files(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_core_files(overwrite)
-    print(
-        f"Serializers, viewsets, and routes for {len(model_names)} models have been generated in the {app_name} directory."
-    )
-
-
-@app.command()
-def generate_serializers(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_serializers(overwrite)
-    print(
-        f"Serializers for {len(model_names)} models have been generated in the {app_name} directory."
-    )
-
-
-@app.command()
-def generate_viewsets(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_viewsets(overwrite)
-    print(
-        f"Viewsets for {len(model_names)} models have been generated in the {app_name} directory."
-    )
-
-
-@app.command()
-def generate_urls(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_urls(overwrite)
-    print(f"URLs have been generated in the {app_name} directory.")
-
-
-@app.command()
-def generate_routes(
-    app_name: str, project_name: str, model_file: str, overwrite: bool = False
-):
-    model_names = ModelExtractor.extract_model_names(model_file)
-    generator = ProjectGenerator(app_name, project_name, model_names)
-    generator.generate_routes(overwrite)
-    print(f"Routes have been generated in the {app_name} directory.")
-
-
-if __name__ == "__main__":
-    app()
```

### Comparing `djangowiz-0.1.4/djangowiz/templates/viewset.py.j2` & `djangowiz-0.2.1/djangowiz/templates/multi/viewsets.py.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from rest_framework.generics import ListCreateAPIView, RetrieveUpdateDestroyAPIView
 from rest_framework.permissions import IsAuthenticated
 from {{ app_name }}.models import {{ model_name }}
 from {{ app_name }}.serializers import {{ model_name }}Serializer
 
-class {{ model_name }}ListCreateAPIView(ListCreateAPIView):
+class {{ model_name }}ListCreateAPIView(generics.ListCreateAPIView):
     queryset = {{ model_name }}.objects.all()
     serializer_class = {{ model_name }}Serializer
-    permission_classes = [IsAuthenticated]
 
-class {{ model_name }}RetrieveUpdateDestroyAPIView(RetrieveUpdateDestroyAPIView):
+class {{ model_name }}RetrieveUpdateDestroyAPIView(generics.RetrieveUpdateDestroyAPIView):
     queryset = {{ model_name }}.objects.all()
-    serializer_class = {{ model_name }}Serializer
-    permission_classes = [IsAuthenticated]
+    serializer_class = {{ model_name }}Serializer
```

### Comparing `djangowiz-0.1.4/pyproject.toml` & `djangowiz-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "djangowiz"
-version = "0.1.4"
+version = "0.2.1"
 description = "DjangoWiz: A simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects."
 authors = ["Ali Tavallaie <a.tavallaie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tavallaie/DjangoWiz"
 repository = "https://github.com/tavallaie/DjangoWiz"
 keywords = ["django", "automation", "toolkit", "code-generation", "web-development"]
 
 [tool.poetry.scripts]
-djangowiz = "djangowiz.generate:app"
+djangowiz = "djangowiz.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.12.3"}
 jinja2 = "^3.1.4"
```

### Comparing `djangowiz-0.1.4/PKG-INFO` & `djangowiz-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangowiz
-Version: 0.1.4
+Version: 0.2.1
 Summary: DjangoWiz: A simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects.
 Home-page: https://github.com/tavallaie/DjangoWiz
 License: MIT
 Keywords: django,automation,toolkit,code-generation,web-development
 Author: Ali Tavallaie
 Author-email: a.tavallaie@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -14,126 +14,160 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/tavallaie/DjangoWiz
 Description-Content-Type: text/markdown
 
-# DjangoWiz
+@@**_⚠️ Caution: This library is under heavy development and is not ready for production._**
 
-DjangoWiz is a simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects. This toolkit helps you quickly scaffold out necessary files based on your models, saving you time and effort.
+@@# DjangoWiz
 
-## Features
+@@DjangoWiz is a simple and powerful toolkit to automate the generation of serializers, viewsets, URLs, and Docker configurations for your Django projects. This toolkit helps you quickly scaffold out necessary files based on your models, saving you time and effort.
 
-- Automatically generates serializers, viewsets, and URLs based on your Django models.
-- Supports generation of Dockerfile and Docker Compose configurations for development and production environments.
-- Skips non-serializable classes and abstract models.
-- Includes customizable templates using Jinja2.
-- Provides flexible commands to generate different components individually or all together.
+@@## Features
 
-## Installation
+@@- Automatically generates serializers, viewsets, and URLs based on your Django models.
+@@- Supports generation of Dockerfile and Docker Compose configurations for development and production environments.
+@@- Skips non-serializable classes and abstract models.
+@@- Includes customizable templates using Jinja2.
+@@- Provides flexible commands to generate different components individually or all together.
+@@- Supports custom templates and single file mode.
+@@- Can be used in other Python scripts.
 
-1. **Install via pip:**
-    ```bash
-    pip install DjangoWiz
-    ```
+@@## Installation
 
-2. **Alternatively, clone the repository:**
-    ```bash
-    git clone https://github.com/yourusername/DjangoWiz.git
-    cd DjangoWiz
-    ```
+@@1. **Install via pip:**
+@@    ```bash
+@@    pip install DjangoWiz
+@@    ```
 
-3. **Install dependencies:**
-    Ensure you have Python and Poetry installed, then run:
-    ```bash
-    poetry install
-    ```
+@@2. **Alternatively, clone the repository:**
+@@    ```bash
+@@    git clone https://github.com/tavallie/DjangoWiz.git
+@@    cd DjangoWiz
+@@    ```
 
-## Usage
+@@3. **Install dependencies:**
+@@    Ensure you have Python and Poetry installed, then run:
+@@    ```bash
+@@    poetry install
+@@    ```
 
-### Generate All Files
+@@## Usage
 
-Generate serializers, viewsets, routes, URLs, Dockerfile, and Docker Compose configurations:
+@@### Generate All Files
 
-```bash
-djangowiz generate-files <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@Generate serializers, viewsets, routes, URLs, Dockerfile, and Docker Compose configurations:
 
-### Generate Core Files Only
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-Generate serializers, viewsets, and routes without Docker-related files:
+@@### Generate Core Files Only
 
-```bash
-djangowiz generate_core_files <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@Generate serializers, viewsets, and routes without Docker-related files:
 
-### Generate Individual Components
+@@```bash
+@@djangowiz generate_core_files <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-#### Generate Serializers
+@@### Generate Individual Components
 
-```bash
-djangowiz generate_serializers <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Serializers
 
-#### Generate Viewsets
+@@```bash
+@@djangowiz generate_serializers <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_viewsets <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Viewsets
 
-#### Generate URLs
+@@```bash
+@@djangowiz generate_viewsets <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_urls <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate URLs
 
-#### Generate Routes
+@@```bash
+@@djangowiz generate_urls <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-```bash
-djangowiz generate_routes <your_app> <your_project> <path/to/models.py> --overwrite
-```
+@@#### Generate Routes
 
-## Directory Structure
+@@```bash
+@@djangowiz generate_routes <your_app> <your_project> <path/to/models.py> --overwrite
+@@```
 
-Ensure your project directory is structured as follows:
+@@### Using Custom Templates
 
-```
-DjangoWiz/
-├── DjangoWiz/
-│   ├── __init__.py
-│   ├── generate.py
-│   ├── templates/
-│       ├── docker-compose.dev.yml.j2
-│       ├── docker-compose.prod.yml.j2
-│       ├── Dockerfile.j2
-│       ├── env.dev.j2
-│       ├── env.prod.j2
-│       ├── serializer.py.j2
-│       ├── viewset.py.j2
-│       ├── urls.py.j2
-│       ├── routes.py.j2
-├── pyproject.toml
-├── README.md
-├── LICENSE
-```
+@@You can specify a custom template directory with the `--template-dir` option. If a custom template is not provided, the default templates will be used.
 
-## Customizing Templates
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite --template-dir path/to/custom_templates
+@@```
 
-The templates used for generating files are located in the `DjangoWiz/templates` directory. You can customize these templates to fit your project's specific requirements. The templates use Jinja2 for rendering.
+@@### Using Single File Mode
 
-## License
+@@You can generate all serializers and viewsets in a single file using the `--single-file` option.
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
+@@```bash
+@@djangowiz generate_files <your_app> <your_project> <path/to/models.py> --overwrite --single-file
+@@```
 
-## Contributing
+@@### Using as a Python Library
 
-Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.
+@@You can use DjangoWiz in your own Python scripts:
 
-## Author
+@@```python
+@@from djangowiz.core import ModelExtractor, ProjectGenerator
 
-Ali Tavallaie - [a.tavallaie@gmail.com](mailto:a.tavallaie@gmail.com)
+@@model_file = 'path/to/models.py'
+@@model_names = ModelExtractor.extract_model_names(model_file)
+@@generator = ProjectGenerator('your_app', 'your_project', model_names, template_dir='path/to/custom_templates')
+@@generator.generate_all(single_file=True, overwrite=True)
+@@```
 
----
+@@## Directory Structure
 
-Happy coding!
+@@Ensure your project directory is structured as follows:
+
+@@```
+@@DjangoWiz/
+@@├── djangowiz/
+@@│   ├── __init__.py
+@@│   ├── core.py
+@@│   ├── cli.py
+@@│   ├── templates/
+@@│       ├── docker-compose.dev.yml.j2
+@@│       ├── docker-compose.prod.yml.j2
+@@│       ├── Dockerfile.j2
+@@│       ├── env.dev.j2
+@@│       ├── env.prod.j2
+@@│       ├── serializer.py.j2
+@@│       ├── viewset.py.j2
+@@│       ├── urls.py.j2
+@@│       ├── routes.py.j2
+@@├── pyproject.toml
+@@├── README.md
+@@├── LICENSE
+@@```
+
+@@## Customizing Templates
+
+@@The templates used for generating files are located in the `djangowiz/templates` directory. You can customize these templates to fit your project's specific requirements. The templates use Jinja2 for rendering.
+
+@@## License
+
+@@This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
+@@## Contributing
+
+@@Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.
+
+@@## Author
+
+@@Ali Tavallaie - [a.tavallaie@gmail.com](mailto:a.tavallaie@gmail.com)
+
+@@---
+
+@@Happy coding!
```

