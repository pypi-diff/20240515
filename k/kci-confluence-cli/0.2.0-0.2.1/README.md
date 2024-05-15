# Comparing `tmp/kci_confluence_cli-0.2.0.tar.gz` & `tmp/kci_confluence_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kci_confluence_cli-0.2.0.tar", max compression
+gzip compressed data, was "kci_confluence_cli-0.2.1.tar", max compression
```

## Comparing `kci_confluence_cli-0.2.0.tar` & `kci_confluence_cli-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1744 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/README.md
--rw-r--r--   0        0        0       71 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/__init__.py
--rw-r--r--   0        0        0     1672 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/__main__.py
--rw-r--r--   0        0        0      131 2024-05-09 06:19:22.324425 kci_confluence_cli-0.2.0/confluence/__version__.py
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/__init__.py
--rw-r--r--   0        0        0     4938 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/create_attachment.py
--rw-r--r--   0        0        0     3816 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/delete_attachment.py
--rw-r--r--   0        0        0     2015 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/get_attachment.py
--rw-r--r--   0        0        0     1020 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/attachment/subcommand.py
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/__init__.py
--rw-r--r--   0        0        0     6889 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/api.py
--rw-r--r--   0        0        0     9560 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/cli.py
--rw-r--r--   0        0        0     2441 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/common/utils.py
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/__init__.py
--rw-r--r--   0        0        0     1412 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/get_content_by_id.py
--rw-r--r--   0        0        0      840 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/content/subcommand.py
--rw-r--r--   0        0        0      462 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/data/logging.yaml
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/__init__.py
--rw-r--r--   0        0        0     3591 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/convert_html_to_xml.py
--rw-r--r--   0        0        0      859 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/local/subcommand.py
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/__init__.py
--rw-r--r--   0        0        0     1680 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/get_page_body.py
--rw-r--r--   0        0        0      907 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/subcommand.py
--rw-r--r--   0        0        0     1838 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/page/update_page.py
--rw-r--r--   0        0        0        0 2024-05-09 06:19:07.244381 kci_confluence_cli-0.2.0/confluence/py.typed
--rw-r--r--   0        0        0     4057 2024-05-09 06:19:22.320425 kci_confluence_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 kci_confluence_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1744 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/README.md
+-rw-r--r--   0        0        0       71 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/__init__.py
+-rw-r--r--   0        0        0     1672 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/__main__.py
+-rw-r--r--   0        0        0      131 2024-05-15 06:37:30.108139 kci_confluence_cli-0.2.1/confluence/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/attachment/__init__.py
+-rw-r--r--   0        0        0     4969 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/attachment/create_attachment.py
+-rw-r--r--   0        0        0     3832 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/attachment/delete_attachment.py
+-rw-r--r--   0        0        0     2015 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/attachment/get_attachment.py
+-rw-r--r--   0        0        0     1020 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/attachment/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/common/__init__.py
+-rw-r--r--   0        0        0     6889 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/common/api.py
+-rw-r--r--   0        0        0     9560 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/common/cli.py
+-rw-r--r--   0        0        0     2441 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/common/utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/content/__init__.py
+-rw-r--r--   0        0        0     1412 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/content/get_content_by_id.py
+-rw-r--r--   0        0        0      840 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/content/subcommand.py
+-rw-r--r--   0        0        0      462 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/data/logging.yaml
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/local/__init__.py
+-rw-r--r--   0        0        0     4281 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/local/convert_html_to_xml.py
+-rw-r--r--   0        0        0      859 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/local/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/page/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/page/get_page_body.py
+-rw-r--r--   0        0        0      907 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/page/subcommand.py
+-rw-r--r--   0        0        0     1838 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/page/update_page.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:37:20.692106 kci_confluence_cli-0.2.1/confluence/py.typed
+-rw-r--r--   0        0        0     4057 2024-05-15 06:37:30.108139 kci_confluence_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 kci_confluence_cli-0.2.1/PKG-INFO
```

### Comparing `kci_confluence_cli-0.2.0/README.md` & `kci_confluence_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/__main__.py` & `kci_confluence_cli-0.2.1/confluence/__main__.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/attachment/create_attachment.py` & `kci_confluence_cli-0.2.1/confluence/attachment/create_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,19 @@
 
     file_group = parser.add_mutually_exclusive_group(required=True)
     file_group.add_argument("--file", type=Path, nargs="+", help="アップロードするファイル")
     file_group.add_argument("--dir", type=Path, help="アップロードするディレクトリ")
 
     parser.add_argument("--mime_type", type=str, help="ファイル名からMIMEタイプが判別できないときに、この値を添付ファイルのMIMEタイプとします。")
 
-    parser.add_argument("--allow_duplicated", action="store_true", help="指定した場合は、アップロード先にすでに同じファイルが存在している場合に上書きます。指定しない場合は、400 Errorが発生します。")
+    parser.add_argument(
+        "--allow_duplicated",
+        action="store_true",
+        help="指定した場合は、アップロード先にすでに同じファイルが存在している場合に上書きます。指定しない場合は、400 Errorが発生します。",
+    )
 
     parser.add_argument("--filename_pattern", help="glob形式のパターンに一致するファイル名だけアップロードします。(ex) '*.png'")
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: argparse._SubParsersAction | None = None) -> argparse.ArgumentParser:
     subcommand_name = "create"
```

### Comparing `kci_confluence_cli-0.2.0/confluence/attachment/delete_attachment.py` & `kci_confluence_cli-0.2.1/confluence/attachment/delete_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     logger.info(f"page title='{page['title']}'の添付ファイル{len(results)}件を削除します。")
 
     is_purged = args.purge
     success_count = 0
 
     all_yes = False
+    yes = False
     for index, attachment in enumerate(results):
         attachment_id = attachment["id"]
         attachment_title = attachment["title"]
         try:
             if not all_yes:
                 confirm_message = f"id='{attachment_id}', title='{attachment_title}'を削除しますか？"
                 if is_purged:
```

### Comparing `kci_confluence_cli-0.2.0/confluence/attachment/get_attachment.py` & `kci_confluence_cli-0.2.1/confluence/attachment/get_attachment.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/attachment/subcommand.py` & `kci_confluence_cli-0.2.1/confluence/attachment/subcommand.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/common/api.py` & `kci_confluence_cli-0.2.1/confluence/common/api.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/common/cli.py` & `kci_confluence_cli-0.2.1/confluence/common/cli.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/common/utils.py` & `kci_confluence_cli-0.2.1/confluence/common/utils.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/content/get_content_by_id.py` & `kci_confluence_cli-0.2.1/confluence/content/get_content_by_id.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/content/subcommand.py` & `kci_confluence_cli-0.2.1/confluence/content/subcommand.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/local/subcommand.py` & `kci_confluence_cli-0.2.1/confluence/local/subcommand.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/page/get_page_body.py` & `kci_confluence_cli-0.2.1/confluence/page/get_page_body.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/page/subcommand.py` & `kci_confluence_cli-0.2.1/confluence/page/subcommand.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/confluence/page/update_page.py` & `kci_confluence_cli-0.2.1/confluence/page/update_page.py`

 * *Files identical despite different names*

### Comparing `kci_confluence_cli-0.2.0/pyproject.toml` & `kci_confluence_cli-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kci-confluence-cli"
-version = "0.2.0"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+version = "0.2.1"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。"
 authors = ["Kurusugawa Computer Inc."]
 license = "MIT"
 packages = [
     { include = "confluence" }
 ]
 readme="README.md"
```

### Comparing `kci_confluence_cli-0.2.0/PKG-INFO` & `kci_confluence_cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kci-confluence-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: 来栖川電算が利用しているConfluence v6.15.7を操作するためのCLIです。
 Home-page: https://github.com/kurusugawa-computer/confluence-cli
 License: MIT
 Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

