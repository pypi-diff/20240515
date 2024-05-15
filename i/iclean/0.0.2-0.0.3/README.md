# Comparing `tmp/iclean-0.0.2.tar.gz` & `tmp/iclean-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iclean-0.0.2.tar", last modified: Tue May 14 16:53:53 2024, max compression
+gzip compressed data, was "iclean-0.0.3.tar", last modified: Wed May 15 10:26:26 2024, max compression
```

## Comparing `iclean-0.0.2.tar` & `iclean-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-14 16:53:53.648101 iclean-0.0.2/
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    35149 2024-05-08 18:25:37.000000 iclean-0.0.2/LICENSE
--rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-14 16:53:53.648101 iclean-0.0.2/PKG-INFO
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      478 2024-05-14 16:22:30.000000 iclean-0.0.2/README.md
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    10041 2024-05-14 16:53:31.000000 iclean-0.0.2/clean.py
-drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-14 16:53:53.648101 iclean-0.0.2/iclean.egg-info/
--rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-14 16:53:53.000000 iclean-0.0.2/iclean.egg-info/PKG-INFO
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      194 2024-05-14 16:53:53.000000 iclean-0.0.2/iclean.egg-info/SOURCES.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        1 2024-05-14 16:53:53.000000 iclean-0.0.2/iclean.egg-info/dependency_links.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-14 16:53:53.000000 iclean-0.0.2/iclean.egg-info/entry_points.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        6 2024-05-14 16:53:53.000000 iclean-0.0.2/iclean.egg-info/top_level.txt
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      392 2024-05-10 20:37:30.000000 iclean-0.0.2/pyproject.toml
--rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-14 16:53:53.648101 iclean-0.0.2/setup.cfg
+drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-15 10:26:26.268011 iclean-0.0.3/
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    35149 2024-05-08 18:25:37.000000 iclean-0.0.3/LICENSE
+-rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-15 10:26:26.268011 iclean-0.0.3/PKG-INFO
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      478 2024-05-14 16:22:30.000000 iclean-0.0.3/README.md
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)    10937 2024-05-15 10:26:13.000000 iclean-0.0.3/clean.py
+drwxrwxr-x   0 kaliv0    (1000) kaliv0    (1000)        0 2024-05-15 10:26:26.264011 iclean-0.0.3/iclean.egg-info/
+-rw-r--r--   0 kaliv0    (1000) kaliv0    (1000)    41205 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/PKG-INFO
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      194 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        1 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/entry_points.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)        6 2024-05-15 10:26:26.000000 iclean-0.0.3/iclean.egg-info/top_level.txt
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)      392 2024-05-10 20:37:30.000000 iclean-0.0.3/pyproject.toml
+-rw-rw-r--   0 kaliv0    (1000) kaliv0    (1000)       38 2024-05-15 10:26:26.268011 iclean-0.0.3/setup.cfg
```

### Comparing `iclean-0.0.2/LICENSE` & `iclean-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iclean-0.0.2/PKG-INFO` & `iclean-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iclean
-Version: 0.0.2
+Version: 0.0.3
 Summary: Import cleaner
 Author: kaliv0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `iclean-0.0.2/clean.py` & `iclean-0.0.3/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import TextIO
 
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 # ### constants ###
 @dataclass(frozen=True)
 class Patterns:
     LOG_FORMAT = "%(levelname)s: %(message)s"
     TEMP = "{file}.swap"
@@ -26,25 +26,30 @@
     CLEANUP_FAILED_ERROR = "Something went wrong while cleaning up unused imports:"
     CLEANUP_SUCCESSFUL = "Cleaned up {file}"
     NON_EXISTENT_PATH = "{path} doesn't exist"
     SKIP_PATH = "Skipping {path}"
     NOT_PY_FILE = "{path} is not a python file"
 
 
-# TODO: package inside a dataclass?
-COMMENT = "#"
-WILDCARD = "*"
-ALIAS = " as "
-IMPORT = "import "
-IMPORT_LEN = len(IMPORT)
-ALIAS_LEN = len(ALIAS)
-NEW_LINE = "\n"
-DELIMITER = ","
-CWD = "."
-PY_EXT = ".py"
+@dataclass(frozen=True)
+class Tokens:
+    COMMENT = "#"
+    WILDCARD = "*"
+    ALIAS = " as "
+    IMPORT = "import "
+    NEW_LINE = "\n"
+    LEFT_PAREN = "(\n"
+    RIGHT_PAREN = ")\n"
+    DELIMITER = ","
+    CWD = "."
+    PY_EXT = ".py"
+
+
+IMPORT_LEN = len(Tokens.IMPORT)
+ALIAS_LEN = len(Tokens.ALIAS)
 
 # based on .gitignore
 DEFAULT_SKIP_LIST = {
     "build",
     "develop-eggs",
     "dist",
     "downloads",
@@ -119,29 +124,29 @@
             self.lines = f.readlines()
         self.line_num = -1
         self.import_lines = []
 
     # ### main logic ###
     def process_paths(self, path_list: list[str], dir_level: str, verbose: bool) -> None:
         for path in path_list:
-            if path != CWD:
+            if path != Tokens.CWD:
                 path = os.path.join(dir_level, path)
 
             if os.path.exists(path) is False:
                 self.logger.warning(Messages.NON_EXISTENT_PATH.format(path=path))
                 continue
             if self._should_skip_path(os.path.basename(path)):
                 if verbose:
                     self.logger.warning(Messages.SKIP_PATH.format(path=path))
                 continue
             if os.path.isdir(path):
                 nested_paths = os.listdir(path)
                 self.process_paths(nested_paths, dir_level=path, verbose=verbose)
                 continue
-            if path.endswith(PY_EXT) is False:
+            if path.endswith(Tokens.PY_EXT) is False:
                 self.logger.warning(Messages.NOT_PY_FILE.format(path=path))
                 continue
 
             self.set_up(path)
             self.clean_imports()
 
     def _should_skip_path(self, path: str) -> re.Match[str] | bool:
@@ -165,32 +170,47 @@
                 os.remove(self.temp_file)
         else:
             os.replace(self.temp_file, self.file)
             self.logger.info(Messages.CLEANUP_SUCCESSFUL.format(file=self.file))
 
     # ### parse file ###
     def read_imports(self) -> None:
-        for line in self.lines:
-            self.line_num += 1
-            if line.startswith(NEW_LINE):
+        i = -1
+        while i < len(self.lines):
+            i += 1
+            line = self.lines[i]
+            if line.startswith(Tokens.NEW_LINE):
                 self._handle_non_analysed_imports(line, ImportLineType.NEW_LINE)
-            elif line.startswith(COMMENT):
+            elif line.startswith(Tokens.COMMENT):
                 self._handle_non_analysed_imports(line, ImportLineType.COMMENT)
-            elif (idx := line.find(ALIAS)) >= 0:
+            elif (idx := line.find(Tokens.ALIAS)) >= 0:
                 import_boundary = idx + ALIAS_LEN
                 imported = line[import_boundary:]
                 self._handle_aliases(line, imported)
-            elif (idx := line.find(IMPORT)) >= 0:
+            elif (idx := line.find(Tokens.LEFT_PAREN)) >= 0:
+                header = line[:idx]
+                i, imported = self._get_multiline_imports(i)
+                self._handle_import_line(header, imported)
+            elif (idx := line.find(Tokens.IMPORT)) >= 0:
                 import_boundary = idx + IMPORT_LEN
                 header = line[:import_boundary]
                 imported = line[import_boundary:]
                 self._handle_regular_imports(header, imported)
             else:
+                self.line_num = i
                 break
 
+    def _get_multiline_imports(self, i: int) -> tuple[int, list[str]]:
+        imported = []
+        i += 1
+        while (line := self.lines[i]) != Tokens.RIGHT_PAREN:
+            imported.append(line.strip().rstrip(","))  # FIXME
+            i += 1
+        return i, imported
+
     def _handle_non_analysed_imports(self, line_literal: str, line_type: ImportLineType) -> None:
         self.import_lines.append(
             ImportLine(
                 literal=line_literal,
                 import_data=[],
                 import_list=[],
                 type=line_type,
@@ -206,33 +226,35 @@
             import_list=[],
             type=ImportLineType.ALIAS,
         )
         self.import_lines.append(import_line)
 
     def _handle_regular_imports(self, line_literal: str, imported: str) -> None:
         import_names = imported.strip()
-        if import_names.startswith(WILDCARD):
+        if import_names.startswith(Tokens.WILDCARD):
             raise ValueError(Messages.BAD_PRACTICE_ERROR)
 
-        import_list = import_names.split(DELIMITER)
+        import_list = import_names.split(Tokens.DELIMITER)
+        self._handle_import_line(line_literal, import_list)
+
+    def _handle_import_line(self, line_literal: str, import_list: list[str]) -> None:
         import_line = ImportLine(
             literal=line_literal,
             import_data=[],
             import_list=[],
             type=ImportLineType.MULTI_IMPORT if len(import_list) > 1 else ImportLineType.REGULAR,
         )
-
         for import_literal in import_list:
             import_data = ImportData(name=import_literal.strip(), count=0)
             import_line.import_data.append(import_data)
         self.import_lines.append(import_line)
 
     def read_rest_of_file(self) -> None:
         for line in self.lines[self.line_num :]:
-            if line.strip().startswith(COMMENT):
+            if line.strip().startswith(Tokens.COMMENT):
                 continue
 
             for imp_line in self.import_lines:
                 for imported in imp_line.import_data:
                     if re.search(Patterns.IMPORT.format(imported=imported.name), line):
                         # track import usage
                         imported.count += 1
@@ -278,24 +300,24 @@
     def _should_write_import_line(line: ImportLine) -> bool:
         return line.type == ImportLineType.COMMENT or not (
             line.type == ImportLineType.MULTI_IMPORT or line.type == ImportLineType.NEW_LINE
         )
 
     @staticmethod
     def _prepare_import_line(line_literal: str, import_list: list[str]) -> str:
-        return line_literal + f"{DELIMITER} ".join(import_list) + NEW_LINE
+        return line_literal + f"{Tokens.DELIMITER} ".join(import_list) + Tokens.NEW_LINE
 
     def write_rest_of_file(self, file_writer: TextIO) -> None:
         for line in self.lines[self.line_num :]:
             file_writer.write(line)
 
 
 def main() -> None:
     path_list, skip_list, verbose = read_input()
-    Cleaner(skip_list).process_paths(path_list, dir_level=CWD, verbose=verbose)
+    Cleaner(skip_list).process_paths(path_list, dir_level=Tokens.CWD, verbose=verbose)
 
 
 def read_input() -> tuple[list[str], list[str], bool]:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "target", nargs="+", help="path or list of paths to file or directory to parse"
     )
```

### Comparing `iclean-0.0.2/iclean.egg-info/PKG-INFO` & `iclean-0.0.3/iclean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iclean
-Version: 0.0.2
+Version: 0.0.3
 Summary: Import cleaner
 Author: kaliv0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

