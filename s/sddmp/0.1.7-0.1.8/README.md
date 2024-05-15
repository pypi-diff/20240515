# Comparing `tmp/sddmp-0.1.7.tar.gz` & `tmp/sddmp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddmp-0.1.7.tar", max compression
+gzip compressed data, was "sddmp-0.1.8.tar", max compression
```

## Comparing `sddmp-0.1.7.tar` & `sddmp-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0     7777 2024-03-18 22:27:03.937756 sddmp-0.1.7/README.md
--rw-r--r--   0        0        0      637 2024-03-19 11:57:04.181387 sddmp-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3838 2024-03-18 22:19:29.247902 sddmp-0.1.7/src/sddmp/demo.py
--rw-r--r--   0        0        0       91 2024-03-18 08:32:14.485219 sddmp-0.1.7/src/sddmp/filesystem/__init__.py
--rw-r--r--   0        0        0     7110 2024-03-19 11:54:56.202738 sddmp-0.1.7/src/sddmp/filesystem/directory.py
--rw-r--r--   0        0        0     4929 2024-03-18 22:19:29.247902 sddmp-0.1.7/src/sddmp/filesystem/file.py
--rw-r--r--   0        0        0     2806 2024-03-18 08:32:14.486219 sddmp-0.1.7/src/sddmp/filesystem/filesystem.py
--rw-r--r--   0        0        0     1665 2024-03-18 08:32:14.487219 sddmp-0.1.7/src/sddmp/filesystem/filetree.py
--rw-r--r--   0        0        0     3488 2024-03-19 11:54:56.203738 sddmp-0.1.7/src/sddmp/generate.py
--rw-r--r--   0        0        0       84 2024-03-18 08:32:14.487219 sddmp-0.1.7/src/sddmp/metadata/__init__.py
--rw-r--r--   0        0        0     7162 2024-03-19 09:22:56.367357 sddmp-0.1.7/src/sddmp/metadata/metadata.py
--rw-r--r--   0        0        0     3408 2024-03-18 08:32:14.488219 sddmp-0.1.7/src/sddmp/metadata/person.py
--rw-r--r--   0        0        0     5560 2024-03-18 08:32:14.489219 sddmp-0.1.7/src/sddmp/metadata/schema_org_validator.py
--rw-r--r--   0        0        0     3348 2024-03-18 08:32:14.489219 sddmp-0.1.7/src/sddmp/metadata/thing.py
--rw-r--r--   0        0        0       84 2024-03-18 22:19:29.247902 sddmp-0.1.7/src/sddmp/outputs/__init__.py
--rw-r--r--   0        0        0     2564 2024-03-18 22:19:29.248901 sddmp-0.1.7/src/sddmp/outputs/directory_page.py
--rw-r--r--   0        0        0     2327 2024-03-19 11:54:56.203738 sddmp-0.1.7/src/sddmp/outputs/html_page.py
--rw-r--r--   0        0        0       92 2024-03-18 08:32:14.490219 sddmp-0.1.7/src/sddmp/outputs/plots/__init__.py
--rw-r--r--   0        0        0     2517 2024-03-18 08:32:14.490219 sddmp-0.1.7/src/sddmp/outputs/plots/base_plot.py
--rw-r--r--   0        0        0      466 2024-03-18 08:32:14.491219 sddmp-0.1.7/src/sddmp/outputs/plots/palette.py
--rw-r--r--   0        0        0     1468 2024-03-18 08:32:14.491219 sddmp-0.1.7/src/sddmp/outputs/plots/pie_plot.py
--rw-r--r--   0        0        0     3221 2024-03-19 11:54:56.204738 sddmp-0.1.7/src/sddmp/outputs/plots/plot_generator.py
--rw-r--r--   0        0        0      974 2024-03-18 22:19:29.249902 sddmp-0.1.7/src/sddmp/outputs/reference_page.py
--rw-r--r--   0        0        0    21372 2024-03-18 08:32:14.492219 sddmp-0.1.7/src/sddmp/outputs/static/js/jquery-ui.min.js
--rw-r--r--   0        0        0     1535 2024-03-18 08:32:14.493219 sddmp-0.1.7/src/sddmp/outputs/static/js/script.js
--rw-r--r--   0        0        0     1386 2024-03-18 08:32:14.493219 sddmp-0.1.7/src/sddmp/outputs/static/styles/custom.css
--rw-r--r--   0        0        0   270348 2024-03-18 08:32:14.495219 sddmp-0.1.7/src/sddmp/outputs/static/styles/styles.css
--rw-r--r--   0        0        0      178 2024-03-18 08:32:14.495219 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/heading.html.j2
--rw-r--r--   0        0        0      544 2024-03-18 09:35:19.402598 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/large_card.html.j2
--rw-r--r--   0        0        0     1514 2024-03-18 08:32:14.497219 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/person_card.html.j2
--rw-r--r--   0        0        0      467 2024-03-18 08:32:14.497219 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/plot_div.html.j2
--rw-r--r--   0        0        0      731 2024-03-18 08:32:14.498219 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/small_card.html.j2
--rw-r--r--   0        0        0     2692 2024-03-18 08:32:14.498219 sddmp-0.1.7/src/sddmp/outputs/templates/components/body/table.html.j2
--rw-r--r--   0        0        0      305 2024-03-18 08:32:14.498219 sddmp-0.1.7/src/sddmp/outputs/templates/components/topbar/nav_alert.html.j2
--rw-r--r--   0        0        0     4454 2024-03-18 22:19:29.249902 sddmp-0.1.7/src/sddmp/outputs/templates/directory.html.j2
--rw-r--r--   0        0        0      179 2024-03-18 08:32:14.499219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/footer.html.j2
--rw-r--r--   0        0        0     1543 2024-03-18 08:32:14.499219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/head.html.j2
--rw-r--r--   0        0        0      620 2024-03-18 08:32:14.499219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/layout.html.j2
--rw-r--r--   0        0        0      279 2024-03-18 08:32:14.500219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/scripts.html.j2
--rw-r--r--   0        0        0     5231 2024-03-18 08:32:14.500219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/side_nav.html.j2
--rw-r--r--   0        0        0     1235 2024-03-18 08:32:14.501219 sddmp-0.1.7/src/sddmp/outputs/templates/partials/top_nav.html.j2
--rw-r--r--   0        0        0     4781 2024-03-18 09:35:19.403598 sddmp-0.1.7/src/sddmp/outputs/templates/reference.html.j2
--rw-r--r--   0        0        0     2243 2024-03-18 08:32:14.501219 sddmp-0.1.7/src/sddmp/resources/README_example.yaml
--rw-r--r--   0        0        0      294 2024-03-18 08:32:14.501219 sddmp-0.1.7/src/sddmp/resources/demo_structure.txt
--rw-r--r--   0        0        0     8459 1970-01-01 00:00:00.000000 sddmp-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     7777 2024-03-18 22:27:03.937756 sddmp-0.1.8/README.md
+-rw-r--r--   0        0        0      654 2024-05-15 10:01:59.862120 sddmp-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1394 2024-05-15 08:56:20.004666 sddmp-0.1.8/src/sddmp/common.py
+-rw-r--r--   0        0        0     4196 2024-05-15 08:41:49.869251 sddmp-0.1.8/src/sddmp/config.py
+-rw-r--r--   0        0        0     3507 2024-05-08 13:03:34.592566 sddmp-0.1.8/src/sddmp/demo.py
+-rw-r--r--   0        0        0       91 2024-03-18 08:32:14.485219 sddmp-0.1.8/src/sddmp/filesystem/__init__.py
+-rw-r--r--   0        0        0     7703 2024-05-14 11:17:11.792390 sddmp-0.1.8/src/sddmp/filesystem/directory.py
+-rw-r--r--   0        0        0     4929 2024-03-18 22:19:29.247902 sddmp-0.1.8/src/sddmp/filesystem/file.py
+-rw-r--r--   0        0        0     4164 2024-05-14 11:11:48.042178 sddmp-0.1.8/src/sddmp/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1665 2024-03-18 08:32:14.487219 sddmp-0.1.8/src/sddmp/filesystem/filetree.py
+-rw-r--r--   0        0        0     4266 2024-05-15 08:41:49.869251 sddmp-0.1.8/src/sddmp/generate.py
+-rw-r--r--   0        0        0       84 2024-03-18 08:32:14.487219 sddmp-0.1.8/src/sddmp/metadata/__init__.py
+-rw-r--r--   0        0        0     7142 2024-05-08 13:03:34.592566 sddmp-0.1.8/src/sddmp/metadata/metadata.py
+-rw-r--r--   0        0        0     3408 2024-03-18 08:32:14.488219 sddmp-0.1.8/src/sddmp/metadata/person.py
+-rw-r--r--   0        0        0     5560 2024-03-18 08:32:14.489219 sddmp-0.1.8/src/sddmp/metadata/schema_org_validator.py
+-rw-r--r--   0        0        0     3348 2024-03-18 08:32:14.489219 sddmp-0.1.8/src/sddmp/metadata/thing.py
+-rw-r--r--   0        0        0       84 2024-03-18 22:19:29.247902 sddmp-0.1.8/src/sddmp/outputs/__init__.py
+-rw-r--r--   0        0        0     2647 2024-05-15 08:10:25.705596 sddmp-0.1.8/src/sddmp/outputs/directory_page.py
+-rw-r--r--   0        0        0     2183 2024-05-15 08:10:25.705596 sddmp-0.1.8/src/sddmp/outputs/html_page.py
+-rw-r--r--   0        0        0       92 2024-03-18 08:32:14.490219 sddmp-0.1.8/src/sddmp/outputs/plots/__init__.py
+-rw-r--r--   0        0        0     2517 2024-03-18 08:32:14.490219 sddmp-0.1.8/src/sddmp/outputs/plots/base_plot.py
+-rw-r--r--   0        0        0      466 2024-03-18 08:32:14.491219 sddmp-0.1.8/src/sddmp/outputs/plots/palette.py
+-rw-r--r--   0        0        0     1468 2024-03-18 08:32:14.491219 sddmp-0.1.8/src/sddmp/outputs/plots/pie_plot.py
+-rw-r--r--   0        0        0     3106 2024-05-15 08:10:25.705596 sddmp-0.1.8/src/sddmp/outputs/plots/plot_generator.py
+-rw-r--r--   0        0        0      878 2024-05-15 08:10:25.705596 sddmp-0.1.8/src/sddmp/outputs/reference_page.py
+-rw-r--r--   0        0        0    21372 2024-03-18 08:32:14.492219 sddmp-0.1.8/src/sddmp/outputs/static/js/jquery-ui.min.js
+-rw-r--r--   0        0        0     1535 2024-03-18 08:32:14.493219 sddmp-0.1.8/src/sddmp/outputs/static/js/script.js
+-rw-r--r--   0        0        0     1386 2024-03-18 08:32:14.493219 sddmp-0.1.8/src/sddmp/outputs/static/styles/custom.css
+-rw-r--r--   0        0        0   270348 2024-03-18 08:32:14.495219 sddmp-0.1.8/src/sddmp/outputs/static/styles/styles.css
+-rw-r--r--   0        0        0      178 2024-03-18 08:32:14.495219 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/heading.html.j2
+-rw-r--r--   0        0        0      544 2024-03-18 09:35:19.402598 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/large_card.html.j2
+-rw-r--r--   0        0        0     1514 2024-03-18 08:32:14.497219 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/person_card.html.j2
+-rw-r--r--   0        0        0      467 2024-03-18 08:32:14.497219 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/plot_div.html.j2
+-rw-r--r--   0        0        0      731 2024-03-18 08:32:14.498219 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/small_card.html.j2
+-rw-r--r--   0        0        0     2692 2024-03-18 08:32:14.498219 sddmp-0.1.8/src/sddmp/outputs/templates/components/body/table.html.j2
+-rw-r--r--   0        0        0      305 2024-03-18 08:32:14.498219 sddmp-0.1.8/src/sddmp/outputs/templates/components/topbar/nav_alert.html.j2
+-rw-r--r--   0        0        0     4454 2024-03-18 22:19:29.249902 sddmp-0.1.8/src/sddmp/outputs/templates/directory.html.j2
+-rw-r--r--   0        0        0      179 2024-03-18 08:32:14.499219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/footer.html.j2
+-rw-r--r--   0        0        0     1543 2024-03-18 08:32:14.499219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/head.html.j2
+-rw-r--r--   0        0        0      620 2024-03-18 08:32:14.499219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/layout.html.j2
+-rw-r--r--   0        0        0      279 2024-03-18 08:32:14.500219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/scripts.html.j2
+-rw-r--r--   0        0        0     5231 2024-03-18 08:32:14.500219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/side_nav.html.j2
+-rw-r--r--   0        0        0     1235 2024-03-18 08:32:14.501219 sddmp-0.1.8/src/sddmp/outputs/templates/partials/top_nav.html.j2
+-rw-r--r--   0        0        0     4781 2024-03-18 09:35:19.403598 sddmp-0.1.8/src/sddmp/outputs/templates/reference.html.j2
+-rw-r--r--   0        0        0     2243 2024-03-18 08:32:14.501219 sddmp-0.1.8/src/sddmp/resources/README_example.yaml
+-rw-r--r--   0        0        0      294 2024-03-18 08:32:14.501219 sddmp-0.1.8/src/sddmp/resources/demo_structure.txt
+-rw-r--r--   0        0        0     6343 2024-05-15 08:49:35.973369 sddmp-0.1.8/src/sddmp/util/file_operations.py
+-rw-r--r--   0        0        0     8498 1970-01-01 00:00:00.000000 sddmp-0.1.8/PKG-INFO
```

### Comparing `sddmp-0.1.7/README.md` & `sddmp-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/pyproject.toml` & `sddmp-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "sddmp"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Self Documenting Data Management Plan (SDDMP)"
 authors = ["Jonathan Hartman <hartman@itc.rwth-aachen.de>"]
 readme = "README.md"
 include = ["src/sddmp/outputs/static/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyyaml = "^6.0.1"
 pandas = "^2.1.3"
 rdflib = "^7.0.0"
 requests = "^2.31.0"
 jinja2 = "^3.1.3"
 plotly = "^5.18.0"
+toml = "^0.10.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pylint = "^3.0.3"
 flake8 = "^7.0.0"
 black = "^24.1.1"
```

### Comparing `sddmp-0.1.7/src/sddmp/demo.py` & `sddmp-0.1.8/src/sddmp/demo.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,48 +6,31 @@
 
 The script can be run from the command line using the following command:
 ```
 python -m sddmp.demo -o example_project -i example_structure.txt
 ```
 """
 
-import argparse
 import logging
 from pathlib import Path
 import shutil
 import sys
 
+from .common import _common_cli, _logging_setup
+
 logger = logging.getLogger(__name__)
 
 
-def _parse_cli():
-    parser = argparse.ArgumentParser(
-        description="Create a demonstration project directory structure for testing."
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=str,
-        default="example_project",
-        help="The output directory to create and write the demonstration project to.",
-    )
-    parser.add_argument(
-        "-i",
-        "--input",
-        type=str,
-        help=(
-            "A Text file containing a directory structure to build the demonstration project "
-            "from."
-        ),
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="Print verbose output.",
+def cli():
+    """
+    Create a CLI for the demo script.
+    """
+
+    parser = _common_cli(
+        "Create a demonstration project directory structure for testing."
     )
     parser.add_argument(
         "--dry_run",
         action="store_true",
         help="Print the output without writing to the file system.",
     )
     return parser.parse_args()
@@ -78,39 +61,49 @@
         path = Path(base_path, *path_stack)
         log_func = logger.info if dry_run else logger.debug
         log_func("Creating %s", path)
         if not dry_run:
             path.mkdir(parents=True, exist_ok=True)
 
 
-if __name__ == "__main__":
-    args = _parse_cli()
-
-    # Set up logging.
-    if args.verbose:
-        logging.basicConfig(level=logging.DEBUG)
-    else:
-        logging.basicConfig(level=logging.INFO)
+def get_structure(file_path: str) -> str:
+    """
+    Get the structure from the user.
 
-    print(f"Creating example project at {args.output}")
+    Args:
+        file_path (str): The path to the file to load the directory structure from.
 
-    structure = ""
-    if args.input:
-        print(f"Using input file {args.input}")
-        with open(args.input, encoding="utf-8") as f:
-            structure = f.read()
+    Returns:
+        str: The directory structure as a string.
+    """
+    if file_path:
+        with open(file_path, encoding="utf-8") as f:
+            return f.read()
     else:
         print(
             "Please paste a directory structure into the terminal here (Press Enter to finish):"
         )
+        user_input = ""
         while True:
             text = input()
             if text == "":
                 break
-            structure += text + "\n"
+            user_input += text + "\n"
+        return user_input
+
+
+if __name__ == "__main__":
+    args = cli()
+
+    # Set up logging.
+    _logging_setup(args.verbose)
+
+    print(f"Creating example project at {args.output}")
+
+    structure = get_structure(args.input)
 
     # Let the user see the structure that will be created.
     print("The following directory structure will be created:")
     print(structure)
     if input("Is this correct? (y/n): ").lower() != "y":
         print("Exiting.")
         sys.exit()
```

### Comparing `sddmp-0.1.7/src/sddmp/filesystem/directory.py` & `sddmp-0.1.8/src/sddmp/filesystem/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,22 +61,21 @@
         The metadata of the directory.
         """
         if self._metadata is None:
             self._metadata = self.get_metadata()
         return self._metadata
 
     @property
-    def all_descendants(self):
+    def self_and_descendants(self):
         """
         All descendant directories of this directory.
         """
         descendants = [self]
         for child in self.children:
-            descendants.append(child)
-            descendants.extend(child.all_descendants)
+            descendants.extend(child.self_and_descendants)
         return descendants
 
     @property
     def filetree(self) -> str:
         """
         Get the filetree of the directory as a string.
         """
@@ -113,14 +112,24 @@
 
         action = self.metadata["Dataset"].get("potentialAction", [{"name": "include"}])
         return {
             "action": action[0]["name"],
             "pattern": action[0].get("pattern", ".*"),
         }
 
+    @property
+    def path_depth(self) -> int:
+        """
+        Get the number of folders that appear above this one in the directory tree.
+        """
+        if self.parent == self:
+            return 0
+
+        return self.parent.path_depth + 1
+
     def __post_init__(self):
         # If the directory has no parent, it is the root directory.
         if self.parent is None:
             self.parent = self
 
         # If the directory has no children, it is a leaf directory.
         if self.children is None:
@@ -134,20 +143,32 @@
 
         self._filetree = FileTree(self.path)
 
         logger.debug("Created directory object %s", self.path)
 
     @property
     def file_dataframe(self) -> pd.DataFrame:
+        """
+        Get a dataframe of all files in the directory tree.
+
+        Returns:
+            pd.DataFrame: A dataframe of all files in the directory tree.
+        """
         df = pd.DataFrame([file.get_file_metadata() for file in self.files])
         full_df = pd.concat([df] + [child.file_dataframe for child in self.children])
         return full_df
 
     @property
     def num_excluded_files(self) -> int:
+        """
+        Get the number of files in the directory tree that are excluded.
+
+        Returns:
+            int: The number of files in the directory tree that are excluded.
+        """
         if "Action" not in self.file_dataframe:
             return 0
 
         return sum(self.file_dataframe["Action"] == "exclude")
 
     def get_metadata(self) -> Metadata:
         """
```

### Comparing `sddmp-0.1.7/src/sddmp/filesystem/file.py` & `sddmp-0.1.8/src/sddmp/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/filesystem/filetree.py` & `sddmp-0.1.8/src/sddmp/filesystem/filetree.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/generate.py` & `sddmp-0.1.8/src/sddmp/generate.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,116 +3,134 @@
 
 Usage:
     python create_html_files.py -i data -o docs
 """
 
 import shutil
 
-import argparse
+from importlib import resources
 import logging
 from pathlib import Path
-import pkg_resources
+import re
+import sys
 
 from sddmp.filesystem import FileSystem
 from sddmp.outputs import DirectoryPage, ReferencePage
+from sddmp.util.file_operations import FileOperations
+
+from .common import _common_cli, _logging_setup
+from .config import load_config
 
 logger = logging.getLogger(__name__)
 
 
-def _parse_cli():
-    parser = argparse.ArgumentParser(
-        description="Create static html files for displaying in GitHub Pages."
-    )
-    parser.add_argument(
-        "-i",
-        "--input",
-        type=str,
-        default="data",
-        help="The input directory to create html files for.",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=str,
-        default="docs",
-        help="The output directory for the html files.",
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="Print verbose output.",
-    )
+def cli():
+    """
+    Create a CLI for the generate script.
+    """
+    parser = _common_cli("Create static html files for displaying in GitHub Pages.")
     parser.add_argument(
         "--source_prefix",
         default="",
         help="The prefix to add to the source path when loading the static files",
     )
     return parser.parse_args()
 
 
-def create_index(root_directory, output_directory):
+def clear_output_directory(file_operations, output):
     """
-    Create a simple index page for navigating around the html files.
+    Clear the output directory of a previous run of this script.
 
-    THIS IS NOT A FINAL IMPLEMENTATION. This is just a quick and dirty way to create an index page.
+    Args:
+        file_operations (FileOperations):
+            The file operations object to use for deleting the files.
+        output (str):
+            The output directory to clear.
     """
-    # Create a simple html file that contains links to all of the directories.
-    html = "<ul>"
-    for my_directory in root_directory.all_descendants:
-        html += (
-            f'<li><a href="{my_directory.path}/index.html">{my_directory.path}</a></li>'
-        )
-    html += "</ul>"
 
-    # Create the path to the html file.
-    my_path = Path(output_directory) / "index.html"
+    created_files = [
+        ".*index.html$",
+        rf"^{output}\\.*\\reference.html$",
+        rf"^{output}\\static\\js\\jquery-ui.min.js$",
+        rf"^{output}\\static\\js\\script.js$",
+        rf"^{output}\\static\\styles\\custom.css$",
+        rf"^{output}\\static\\styles\\styles.css$",
+    ]
+
+    for path in Path(output).rglob("*"):
+        if path.is_file():
+            if any(re.match(pattern, str(path)) for pattern in created_files):
+                file_operations.register_deleted_file(path)
+            else:
+                logger.error(
+                    (
+                        "File %s was not created by a previous run of this script. "
+                        "Please check that the output directory does not contain any "
+                        "files not created by this script."
+                    ),
+                    path,
+                )
+                sys.exit(1)
+        elif path.is_dir():
+            file_operations.register_deleted_directory(path)
+
 
-    # Write the html file.
-    with open(my_path, "w", encoding="utf-8") as f:
-        f.write(html)
+def move_static_files(file_operations, output):
+    """
+    Move Static files from the sddmp package to the output directory.
+
+    Args:
+        file_operations (FileOperations):
+            The file operations object to use for moving the static files.
+        output (str):
+            The output directory to move the static files to.
+    """
+    source_dir = resources.files("sddmp") / "outputs/static"
+    logger.info("Copying static files from %s to %s/static", source_dir, output)
 
-    print(f"Created index file at {my_path}")
+    # Iterate over all of the files in the static folder and add them to the operations
+    for file in source_dir.rglob("*"):
+        if file.is_file():
+            with open(file, "rb") as source:
+                target_path = Path("static") / file.relative_to(source_dir)
+                with file_operations.new_file(target_path, "wb") as f:
+                    shutil.copyfileobj(source, f)
 
 
 if __name__ == "__main__":
-    args = _parse_cli()
+    args = cli()
 
     # Set up logging.
-    if args.verbose:
-        logging.basicConfig(level=logging.DEBUG)
-    else:
-        logging.basicConfig(level=logging.INFO)
+    _logging_setup(args.verbose)
 
-    fs = FileSystem()
+    config = load_config()
+    if args.output:
+        config.set_output_directory(args.output)
+
+    operations = FileOperations(
+        dry_run=args.dry_run, target_directory=config.output_directory
+    )
+    if args.clean:
+        clear_output_directory(operations, config.output_directory)
+
+    fs = FileSystem(config)
     root = fs.read_directory(args.input)
 
     DirectoryPage.directory_structure = fs.get_directory_structure(root)["children"]
     ReferencePage.directory_structure = fs.get_directory_structure(root)["children"]
 
     # Delete the output directory if it exists.
-    if Path(args.output).exists():
-        logger.info("Deleting existing output directory at %s", args.output)
-        for path in Path(args.output).glob("*"):
-            if path.is_file():
-                path.unlink()
-            else:
-                shutil.rmtree(path)
-        Path(args.output).mkdir(exist_ok=True, parents=True)
 
     # Move the static directory to the output directory.
-    source_dir = pkg_resources.resource_filename(__name__, "/outputs/static/")
-    logger.info("Copying static files from %s to %s/static", source_dir, args.output)
-    shutil.copytree(source_dir, Path(args.output) / "static")
+    move_static_files(operations, output=config.output_directory)
 
     # Create a reference page
-    reference = ReferencePage(args.input, args.output)
-    reference.generate()
+    reference = ReferencePage(args.input)
+    reference.generate(operations)
 
     # Start with the root and iterate recursively through all directories.
     # For each directory, create an html file.
-    for directory in root.all_descendants:
-        page = DirectoryPage(directory, args.output)
-        page.generate()
+    for directory in root.self_and_descendants:
+        page = DirectoryPage(directory)
+        page.generate(operations)
 
-    # Create an index to help navigate around
-    create_index(root, args.output)
+    operations.execute()
```

### Comparing `sddmp-0.1.7/src/sddmp/metadata/metadata.py` & `sddmp-0.1.8/src/sddmp/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
     def is_valid(self) -> bool:
         """
         Determines whether the metadata is valid based on the schema.org vocabulary.
 
         Returns:
             bool: True if the metadata is valid, otherwise False.
         """
-        return True
         return all(value["valid"] for value in self.validate_keys().values())
 
     def supplement(self, other: "Metadata") -> None:
         """
         Supplements the content of the metadata with the content of another metadata object.
 
         Args:
```

### Comparing `sddmp-0.1.7/src/sddmp/metadata/person.py` & `sddmp-0.1.8/src/sddmp/metadata/person.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/metadata/schema_org_validator.py` & `sddmp-0.1.8/src/sddmp/metadata/schema_org_validator.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/metadata/thing.py` & `sddmp-0.1.8/src/sddmp/metadata/thing.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/directory_page.py` & `sddmp-0.1.8/src/sddmp/outputs/directory_page.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 from pathlib import Path
 
 from ..filesystem import Directory
 from .html_page import HTMLPage
 from .plots.plot_generator import PlotGenerator
+from ..util.file_operations import FileOperations
 
 
 class DirectoryPage(HTMLPage):
     """
     Represents an HTML page for a directory in the file system.
 
     Attributes:
@@ -19,57 +20,59 @@
         output_directory (Path): The directory in which the HTML page is to be saved.
 
     Methods:
         generate: Generates the HTML page for the directory.
         generate_pie_plot: Generates a pie plot for a column in the dataframe.
     """
 
-    def __init__(self, directory: Directory, output_directory: Path):
-        super().__init__("directory.html.j2", output_directory)
+    def __init__(self, directory: Directory):
+        super().__init__("directory.html.j2")
         self.directory = directory
 
     def get_relative_path_to_root(self) -> str:
         """
         Returns the relative path from the output directory to the root directory.
         """
-        num_path_parts = len(self.directory.path.parts)
+        num_path_parts = self.directory.path_depth + 1
         if num_path_parts == 1:
             return ".."
 
         return "../" * (num_path_parts)
 
     def get_path(self) -> Path:
         """
         Returns the path to the HTML file.
         """
-        return self.output_directory / self.directory.path / "index.html"
+        return self.directory.path / "index.html"
 
     def get_depth(self) -> int:
         """
         Returns the depth of the page in the directory structure.
         """
         return len(self.directory.path.parts)
 
-    def generate(self) -> None:
+    def generate(self, operations: FileOperations, **kwargs) -> None:
         """
         Generates the HTML page for the directory and saves it in the output directory.
         """
         file_records_df = self.directory.file_records_dataframe()
 
         plot_generator = PlotGenerator(file_records_df)
 
         # Render the template with the dataframe.
         super().generate(
+            operations=operations,
             project_title=self.directory.metadata["ResearchProject"]["name"],
             my_path=self.directory.path.as_posix(),
             num_files=len(file_records_df),
             num_excluded_files=self.directory.num_excluded_files,
-            num_directories=len(self.directory.all_descendants) + 1,
+            num_directories=len(self.directory.self_and_descendants) + 1,
             people=self.directory.metadata.get_people(),
             filetree=self.directory.filetree,
             plots={
                 name: plot.as_json()
                 for name, plot in plot_generator.all_plots().items()
             },
             metadata=self.directory.metadata_as_plaintext(),
             file_records_df=file_records_df,
+            **kwargs,
         )
```

### Comparing `sddmp-0.1.7/src/sddmp/outputs/html_page.py` & `sddmp-0.1.8/src/sddmp/outputs/html_page.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 
 This class is not intended to be used directly, but rather to be subclassed by classes that
 generate specific types of HTML pages.
 """
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-import pkg_resources
+from importlib import resources
 
 from jinja2 import Environment, FileSystemLoader
 
+from ..util.file_operations import FileOperations
+
 
 class HTMLPage(ABC):
     """
     This is an abstract base class containing common methods and properties for generating HTML
     pages.
     """
 
     # Class Variable for storing the directory structure
     directory_structure = None
 
-    def __init__(self, template_name: str, output_directory: Path):
-        self.output_directory = output_directory
-        template_dir = pkg_resources.resource_filename(__name__, "/templates")
+    def __init__(self, template_name: str):
+        template_dir = resources.files("sddmp") / "outputs/templates"
         self.jinja_env = Environment(
             loader=FileSystemLoader(template_dir), autoescape=True
         )
         self.template = self.jinja_env.get_template(template_name)
 
     @abstractmethod
     def get_relative_path_to_root(self) -> str:
@@ -53,24 +54,21 @@
     def get_depth(self) -> int:
         """
         Returns the depth of the page in the directory structure.
 
         TODO: I honestly can't remember why we have both this and relative path to root
         """
 
-    def generate(self, **kwargs) -> None:
+    def generate(self, operations: FileOperations, **kwargs) -> None:
         """
         Generate an HTML page.
         """
         html = self.template.render(
             directory_structure=self.directory_structure,
             relative_path_to_root=self.get_relative_path_to_root(),
             depth=self.get_depth(),
             **kwargs
         )
 
-        # Create the directory for the html file if it does not exist.
-        Path(self.get_path()).parent.mkdir(parents=True, exist_ok=True)
-
         # Write the html file.
-        with open(self.get_path(), "w", encoding="utf-8") as f:
+        with operations.new_file(self.get_path()) as f:
             f.write(html)
```

### Comparing `sddmp-0.1.7/src/sddmp/outputs/plots/base_plot.py` & `sddmp-0.1.8/src/sddmp/outputs/plots/base_plot.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/plots/pie_plot.py` & `sddmp-0.1.8/src/sddmp/outputs/plots/pie_plot.py`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/plots/plot_generator.py` & `sddmp-0.1.8/src/sddmp/outputs/plots/plot_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 class PlotGenerator:
     """
     Class for generating plots from a dataframe for use in the HTML page.
     """
 
     def __init__(self, df):
-        logger.debug("Creating a PlotGenerator object.")
-        logger.debug("Dataframe columns: %s", df.columns)
         self.df = df
 
     def generate_pie_plot(self, column: str) -> PiePlot:
         """
         Generates a pie plot for a column in the dataframe.
 
         Args:
```

### Comparing `sddmp-0.1.7/src/sddmp/outputs/reference_page.py` & `sddmp-0.1.8/src/sddmp/outputs/reference_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 class ReferencePage(HTMLPage):
     """
     This is a class for generating an HTML page for the glossary of terms and special keys used in
     the project. Presents similar information to the project README file, but will be included in
     the output files.
     """
 
-    def __init__(self, input_directory: Path, output_directory: Path):
-        super().__init__("reference.html.j2", output_directory)
+    def __init__(self, input_directory: Path):
+        super().__init__("reference.html.j2")
         self.input_directory = input_directory
 
     def get_relative_path_to_root(self) -> str:
         return ".."
 
     def get_path(self) -> Path:
-        return (
-            Path(self.output_directory) / Path(self.input_directory) / "reference.html"
-        )
+        return Path(self.input_directory) / "reference.html"
 
     def get_depth(self) -> int:
         return 0
```

### Comparing `sddmp-0.1.7/src/sddmp/outputs/static/js/jquery-ui.min.js` & `sddmp-0.1.8/src/sddmp/outputs/static/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/static/js/script.js` & `sddmp-0.1.8/src/sddmp/outputs/static/js/script.js`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/static/styles/custom.css` & `sddmp-0.1.8/src/sddmp/outputs/static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/static/styles/styles.css` & `sddmp-0.1.8/src/sddmp/outputs/static/styles/styles.css`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/components/body/large_card.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/components/body/large_card.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/components/body/person_card.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/components/body/person_card.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/components/body/small_card.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/components/body/small_card.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/components/body/table.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/components/body/table.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/directory.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/directory.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/partials/head.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/partials/head.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/partials/layout.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/partials/layout.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/partials/side_nav.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/partials/side_nav.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/partials/top_nav.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/partials/top_nav.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/outputs/templates/reference.html.j2` & `sddmp-0.1.8/src/sddmp/outputs/templates/reference.html.j2`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/src/sddmp/resources/README_example.yaml` & `sddmp-0.1.8/src/sddmp/resources/README_example.yaml`

 * *Files identical despite different names*

### Comparing `sddmp-0.1.7/PKG-INFO` & `sddmp-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: sddmp
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Self Documenting Data Management Plan (SDDMP)
 Author: Jonathan Hartman
 Author-email: hartman@itc.rwth-aachen.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Self Documenting Data Management Plan
 
 |         |                                                                                                                                                                                                                                                                                                                                 |
 | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Build   | [![pipeline status](https://git.rwth-aachen.de/dl/productivity-tools/self-documenting-data-management-plan/badges/main/pipeline.svg)](https://git.rwth-aachen.de/dl/productivity-tools/self-documenting-data-management-plan/-/commits/main)                                                                                    |
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1 Name: sddmp Version: 0.1.7 Summary: A Self Documenting
+Metadata-Version: 2.1 Name: sddmp Version: 0.1.8 Summary: A Self Documenting
 Data Management Plan (SDDMP) Author: Jonathan Hartman Author-email:
 hartman@itc.rwth-aachen.de Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: jinja2 (>=3.1.3,<4.0.0) Requires-
 Dist: pandas (>=2.1.3,<3.0.0) Requires-Dist: plotly (>=5.18.0,<6.0.0) Requires-
 Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rdflib (>=7.0.0,<8.0.0) Requires-
-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/markdown # Self
-Documenting Data Management Plan | | | | ------- | ----------------------------
+Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Description-Content-Type: text/markdown # Self Documenting Data Management Plan
+| | | | ------- | -------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------------------------- | | Build | [![pipeline
-status](https://git.rwth-aachen.de/dl/productivity-tools/self-documenting-data-
-management-plan/badges/main/pipeline.svg)](https://git.rwth-aachen.de/dl/
-productivity-tools/self-documenting-data-management-plan/-/commits/main) | |
-Release | [![RWTH Release](https://git.rwth-aachen.de/dl/productivity-tools/
-self-documenting-data-management-plan/-/badges/
-release.svg?key_text=RWTH%20GitLab)](https://git.rwth-aachen.de/dl/
-productivity-tools/self-documenting-data-management-plan/-/releases) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/sddmp) | | Package | [!
-[PyPI Release](https://img.shields.io/pypi/v/sddmp.svg)](https://pypi.org/
-project/sddmp/) | - [Self Documenting Data Management Plan](#self-documenting-
-data-management-plan) - [Installation](#installation) - [Usage](#usage) -
-[Setup](#setup) - [Special Keys](#special-keys) - [Include / Exclude / Redact
-files from a report](#include--exclude--redact-files-from-a-report) - [People]
-(#people) - [Output](#output) - [Demonstration](#demonstration) ## Installation
-This package is available on PyPI and can be installed with the following
-command: ```bash pip install sddmp ``` If you encounter any issues during the
-installation, please check the Python documentation on installing packages. ##
-Usage The package includes a script that will generate a simple html report
-from a directory structure. To use this script, run the following command:
-`python -m sddmp.generate --input "example_project" --output "docs"` `--output`
-is optional. By default, it will create a directory called "docs" in the
-current working directory. ## Setup We expect a directory that contains one or
-more sub-directories, and one or more files. In the root directory, place a
-file called "README.yaml" that contains any common metadata that should apply
-to all files in the directory in yaml format. **The README files are expected
-to comply with the structures dictated on [Schema.org](https://schema.org/).**
-Example: ```yaml DigitalDocument: name: Self Documenting Data Management Plan
-maintainer: - name: email: description: | "Responsible for the content and
-maintenance of the automated data management plan" ResearchProject: name:
+--------------------- | | Build | [![pipeline status](https://git.rwth-
+aachen.de/dl/productivity-tools/self-documenting-data-management-plan/badges/
+main/pipeline.svg)](https://git.rwth-aachen.de/dl/productivity-tools/self-
+documenting-data-management-plan/-/commits/main) | | Release | [![RWTH Release]
+(https://git.rwth-aachen.de/dl/productivity-tools/self-documenting-data-
+management-plan/-/badges/release.svg?key_text=RWTH%20GitLab)](https://git.rwth-
+aachen.de/dl/productivity-tools/self-documenting-data-management-plan/-/
+releases) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+sddmp) | | Package | [![PyPI Release](https://img.shields.io/pypi/v/sddmp.svg)]
+(https://pypi.org/project/sddmp/) | - [Self Documenting Data Management Plan]
+(#self-documenting-data-management-plan) - [Installation](#installation) -
+[Usage](#usage) - [Setup](#setup) - [Special Keys](#special-keys) - [Include /
+Exclude / Redact files from a report](#include--exclude--redact-files-from-a-
+report) - [People](#people) - [Output](#output) - [Demonstration]
+(#demonstration) ## Installation This package is available on PyPI and can be
+installed with the following command: ```bash pip install sddmp ``` If you
+encounter any issues during the installation, please check the Python
+documentation on installing packages. ## Usage The package includes a script
+that will generate a simple html report from a directory structure. To use this
+script, run the following command: `python -m sddmp.generate --input
+"example_project" --output "docs"` `--output` is optional. By default, it will
+create a directory called "docs" in the current working directory. ## Setup We
+expect a directory that contains one or more sub-directories, and one or more
+files. In the root directory, place a file called "README.yaml" that contains
+any common metadata that should apply to all files in the directory in yaml
+format. **The README files are expected to comply with the structures dictated
+on [Schema.org](https://schema.org/).** Example: ```yaml DigitalDocument: name:
+Self Documenting Data Management Plan maintainer: - name: email: description: |
+"Responsible for the content and maintenance of the automated data management
+plan" ResearchProject: name:
  email: jobTitle: Principal Investigator - name: email: jobTitle: Maintainer
 description: "Root folder for Example Project" Dataset: description: | This is
 the readme for the example project and this is the abstract for the dataset.
 conditionsOfAccess: "public" license: "CC-BY-4.0" version: "1.0" ``` In any
 subfolder, we can place another file that contains any subset of this
 information. Example: in example_project/20-29 Communication/20 Internal we
 place a README.yaml that looks like this: ```yaml Dataset: description: This
```

