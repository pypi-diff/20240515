# Comparing `tmp/docmesh_cli-0.0.5.tar.gz` & `tmp/docmesh_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.5.tar` & `docmesh_cli-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.5/README.md
--rw-r--r--   0        0        0       83 2024-05-14 11:31:42.168306 docmesh_cli-0.0.5/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     6566 2024-05-14 10:51:34.334757 docmesh_cli-0.0.5/docmesh_cli/client.py
--rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.5/docmesh_cli/logos.py
--rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.6/README.md
+-rw-r--r--   0        0        0       83 2024-05-15 03:02:58.425080 docmesh_cli-0.0.6/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     6368 2024-05-15 03:00:43.919410 docmesh_cli-0.0.6/docmesh_cli/client.py
+-rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.6/docmesh_cli/logos.py
+-rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.6/PKG-INFO
```

### Comparing `docmesh_cli-0.0.5/docmesh_cli/client.py` & `docmesh_cli-0.0.6/docmesh_cli/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 RC_FILE = os.path.expanduser("~/.docmeshrc")
 PARSER = configparser.ConfigParser()
 
 ADMIN_SHORTCUTS = {
     "/add_entity": {
         "path": "/add_entity",
         "args": "entity_name",
-        "description": "add a new entity, usage: /add_entity [entity_name]",
+        "description": "add a new entity, usage: /add_entity ENTITY_NAME",
     },
     "/update": {
         "path": "/update_embeddings",
         "args": "",
         "description": "update papers embeddings, usage: /update_embeddings",
     },
 }
 
 SHORTCUTS = {
     "/add": {
         "path": "/add_paper",
         "args": "paper",
-        "description": "add a new paper, usage: /add [paper title / arxiv id]",
+        "description": "add a new paper, usage: /add PAPER_TITLE/ARXIV_ID",
     },
     "/read": {
         "path": "/read_paper",
         "args": "paper_id",
-        "description": "read a paper, usage: /read [paper id]",
+        "description": "read a paper, usage: /read PAPER_ID",
     },
     "/help": {
         "description": "show this help menu",
     },
     "/clear": {
         "description": "clear the session memory",
     },
@@ -92,15 +92,15 @@
 
             return server, access_token
         else:
             return _create_profile()
 
 
 def _show_shortcut() -> str:
-    help_menu = [f"{k}, {SHORTCUTS[k]['description']}" for k in SHORTCUTS.keys()]
+    help_menu = [f"{k}, {SHORTCUTS[k]['description']}" for k in SHORTCUTS]
     return "\n".join(help_menu)
 
 
 def _shortcut(
     server: str,
     path: str,
     headers: dict[str, str],
@@ -174,19 +174,16 @@
             if query in ("/end", "/exit"):
                 break
 
             try:
                 query_splitted = query.split(" ")
                 if len(query_splitted) == 1:
                     shortcut_cmd, shortcut_args = query_splitted[0], None
-                elif len(query_splitted) == 2:
-                    shortcut_cmd, shortcut_args = query_splitted[0], query_splitted[1]
                 else:
-                    print(f"{TermColor.red}You enter an invalid shortcut {query}\n{_show_shortcut()}{TermColor.end}")
-                    continue
+                    shortcut_cmd, shortcut_args = query_splitted[0], " ".join(query_splitted[1:])
 
                 if shortcut_cmd in ADMIN_SHORTCUTS:
                     path, args = ADMIN_SHORTCUTS[shortcut_cmd]["path"], ADMIN_SHORTCUTS[shortcut_cmd]["args"]
                 elif shortcut_cmd in SHORTCUTS:
                     path, args = SHORTCUTS[shortcut_cmd]["path"], SHORTCUTS[shortcut_cmd]["args"]
                 else:
                     print(f"{TermColor.red}You enter an invalid shortcut {query}\n{_show_shortcut()}{TermColor.end}")
```

### Comparing `docmesh_cli-0.0.5/docmesh_cli/logos.py` & `docmesh_cli-0.0.6/docmesh_cli/logos.py`

 * *Files identical despite different names*

### Comparing `docmesh_cli-0.0.5/pyproject.toml` & `docmesh_cli-0.0.6/pyproject.toml`

 * *Files identical despite different names*

