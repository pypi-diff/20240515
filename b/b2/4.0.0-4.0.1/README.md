# Comparing `tmp/b2-4.0.0.tar.gz` & `tmp/b2-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2-4.0.0.tar", last modified: Mon May 13 08:03:01 2024, max compression
+gzip compressed data, was "b2-4.0.1.tar", last modified: Wed May 15 15:12:49 2024, max compression
```

## Comparing `b2-4.0.0.tar` & `b2-4.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1350 2024-05-13 08:02:34.888871 b2-4.0.0/LICENSE
--rw-r--r--   0        0        0     7546 2024-05-13 08:02:34.888871 b2-4.0.0/README.md
-lrwxr-xr-x   0        0        0        0 2024-05-13 08:02:34.888871 b2-4.0.0/b2/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0      554 2024-05-13 08:02:34.888871 b2-4.0.0/b2/__init__.py
--rw-r--r--   0        0        0      291 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/__init__.py
--rw-r--r--   0        0        0      422 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/__init__.py
--rw-r--r--   0        0        0     2100 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/arg_parser_types.py
--rw-r--r--   0        0        0     3345 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/argcompleters.py
--rw-r--r--   0        0        0     5262 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/autocomplete_cache.py
--rw-r--r--   0        0        0    11621 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/autocomplete_install.py
--rw-r--r--   0        0        0     1898 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/b2api.py
--rw-r--r--   0        0        0     6817 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/b2args.py
--rw-r--r--   0        0        0     1129 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/const.py
--rw-r--r--   0        0        0     2415 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/obj_dumps.py
--rw-r--r--   0        0        0     1865 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/obj_loads.py
--rw-r--r--   0        0        0      977 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/shell.py
--rw-r--r--   0        0        0      298 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/__init__.py
--rw-r--r--   0        0        0     1595 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/python_compat.py
--rw-r--r--   0        0        0     7443 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/uri.py
--rw-r--r--   0        0        0     9135 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/arg_parser.py
--rw-r--r--   0        0        0      378 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/__init__.py
--rw-r--r--   0        0        0      349 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/__main__.py
--rw-r--r--   0        0        0     4272 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/registry.py
--rw-r--r--   0        0        0     1506 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/rm.py
--rw-r--r--   0        0        0      446 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/sync.py
--rw-r--r--   0        0        0      378 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/__init__.py
--rw-r--r--   0        0        0      349 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/__main__.py
--rw-r--r--   0        0        0     2230 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/registry.py
--rw-r--r--   0        0        0   193002 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/console_tool.py
--rw-r--r--   0        0        0     1027 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/json_encoder.py
--rw-r--r--   0        0        0      435 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/version.py
--rw-r--r--   0        0        0      918 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/version_listing.py
--rw-r--r--   0        0        0   157370 2024-05-13 08:02:59.952895 b2-4.0.0/b2/licenses_output.txt
--rw-r--r--   0        0        0     5432 2024-05-13 08:03:01.464897 b2-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     9947 1970-01-01 00:00:00.000000 b2-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1350 2024-05-15 15:12:16.963832 b2-4.0.1/LICENSE
+-rw-r--r--   0        0        0     7546 2024-05-15 15:12:16.963832 b2-4.0.1/README.md
+lrwxr-xr-x   0        0        0        0 2024-05-15 15:12:16.963832 b2-4.0.1/b2/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      554 2024-05-15 15:12:16.963832 b2-4.0.1/b2/__init__.py
+-rw-r--r--   0        0        0      291 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/__init__.py
+-rw-r--r--   0        0        0     2100 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/arg_parser_types.py
+-rw-r--r--   0        0        0     3388 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/argcompleters.py
+-rw-r--r--   0        0        0     5262 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/autocomplete_cache.py
+-rw-r--r--   0        0        0    11621 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/autocomplete_install.py
+-rw-r--r--   0        0        0     1898 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/b2api.py
+-rw-r--r--   0        0        0     6817 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/b2args.py
+-rw-r--r--   0        0        0     1129 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/const.py
+-rw-r--r--   0        0        0     2415 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/obj_dumps.py
+-rw-r--r--   0        0        0     1865 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/obj_loads.py
+-rw-r--r--   0        0        0      977 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_cli/shell.py
+-rw-r--r--   0        0        0      298 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_utils/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_utils/python_compat.py
+-rw-r--r--   0        0        0     7374 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/_utils/uri.py
+-rw-r--r--   0        0        0     9135 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/arg_parser.py
+-rw-r--r--   0        0        0      378 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v3/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v3/__main__.py
+-rw-r--r--   0        0        0     4887 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v3/registry.py
+-rw-r--r--   0        0        0     2367 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v3/rm.py
+-rw-r--r--   0        0        0      446 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v3/sync.py
+-rw-r--r--   0        0        0      378 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v4/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v4/__main__.py
+-rw-r--r--   0        0        0     2230 2024-05-15 15:12:16.963832 b2-4.0.1/b2/_internal/b2v4/registry.py
+-rw-r--r--   0        0        0   192798 2024-05-15 15:12:16.967832 b2-4.0.1/b2/_internal/console_tool.py
+-rw-r--r--   0        0        0     1027 2024-05-15 15:12:16.967832 b2-4.0.1/b2/_internal/json_encoder.py
+-rw-r--r--   0        0        0      435 2024-05-15 15:12:16.967832 b2-4.0.1/b2/_internal/version.py
+-rw-r--r--   0        0        0      918 2024-05-15 15:12:16.967832 b2-4.0.1/b2/_internal/version_listing.py
+-rw-r--r--   0        0        0   157370 2024-05-15 15:12:47.920118 b2-4.0.1/b2/licenses_output.txt
+-rw-r--r--   0        0        0     5432 2024-05-15 15:12:49.448132 b2-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9947 1970-01-01 00:00:00.000000 b2-4.0.1/PKG-INFO
```

### Comparing `b2-4.0.0/LICENSE` & `b2-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/README.md` & `b2-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/__init__.py` & `b2-4.0.1/b2/__init__.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/arg_parser_types.py` & `b2-4.0.1/b2/_internal/_cli/arg_parser_types.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/argcompleters.py` & `b2-4.0.1/b2/_internal/_cli/argcompleters.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     api = _get_b2api_for_profile(parsed_args.profile)
     bucket = api.get_bucket_by_name(parsed_args.bucketName)
     file_versions = bucket.ls(
         getattr(parsed_args, 'folderName', None) or '',
         latest_only=True,
         recursive=False,
         fetch_count=LIST_FILE_NAMES_MAX_LIMIT,
+        folder_to_list_can_be_a_file=True,
     )
     return [
         unprintable_to_hex(folder_name or file_version.file_name)
         for file_version, folder_name in islice(file_versions, LIST_FILE_NAMES_MAX_LIMIT)
     ]
```

### Comparing `b2-4.0.0/b2/_internal/_cli/autocomplete_cache.py` & `b2-4.0.1/b2/_internal/_cli/autocomplete_cache.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/autocomplete_install.py` & `b2-4.0.1/b2/_internal/_cli/autocomplete_install.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/b2api.py` & `b2-4.0.1/b2/_internal/_cli/b2api.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/b2args.py` & `b2-4.0.1/b2/_internal/_cli/b2args.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/const.py` & `b2-4.0.1/b2/_internal/_cli/const.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/obj_dumps.py` & `b2-4.0.1/b2/_internal/_cli/obj_dumps.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/obj_loads.py` & `b2-4.0.1/b2/_internal/_cli/obj_loads.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_cli/shell.py` & `b2-4.0.1/b2/_internal/_cli/shell.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_utils/python_compat.py` & `b2-4.0.1/b2/_internal/_utils/python_compat.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/_utils/uri.py` & `b2-4.0.1/b2/_internal/_utils/uri.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,23 +190,23 @@
         return self.get_download_url_for_file_name(uri.bucket_name, uri.path, *args, **kwargs)
 
     @get_download_url_by_uri.register
     def _(self, uri: B2FileIdURI, *args, **kwargs) -> str:
         return self.get_download_url_for_fileid(uri.file_id, *args, **kwargs)
 
     @singledispatchmethod
-    def list_file_versions_by_uri(self, uri, *args, **kwargs):
+    def ls(self, uri, *args, **kwargs):
         raise NotImplementedError(f"Unsupported URI type: {type(uri)}")
 
-    @list_file_versions_by_uri.register
+    @ls.register
     def _(self, uri: B2URI, *args, filters: Sequence[Filter] = (), **kwargs):
         bucket = self.api.get_bucket_by_name(uri.bucket_name)
         try:
             yield from bucket.ls(uri.path, *args, filters=filters, **kwargs)
         except ValueError as error:
             # Wrap these errors into B2Error. At the time of writing there's
             # exactly one – `with_wildcard` being passed without `recursive` option.
             raise B2Error(error.args[0])
 
-    @list_file_versions_by_uri.register
+    @ls.register
     def _(self, uri: B2FileIdURI, *args, **kwargs):
         yield self.get_file_info_by_uri(uri), None
```

### Comparing `b2-4.0.0/b2/_internal/arg_parser.py` & `b2-4.0.1/b2/_internal/arg_parser.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/b2v3/registry.py` & `b2-4.0.1/b2/_internal/b2v3/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 ######################################################################
 
 # ruff: noqa: F405
 from b2._internal.b2v4.registry import *  # noqa
 from b2._internal._cli.b2api import _get_b2api_for_profile
 from b2._internal.arg_parser import enable_camel_case_arguments
-from .rm import Rm
+from .rm import Rm, B2URIMustPointToFolderMixin
 from .sync import Sync
 
 enable_camel_case_arguments()
 
 
 class ConsoleTool(ConsoleTool):
     # same as original console tool, but does not use InMemoryAccountInfo and InMemoryCache
@@ -41,15 +41,15 @@
     sys.stderr.flush()
 
     logging.shutdown()
 
     os._exit(exit_status)
 
 
-class Ls(B2URIBucketNFolderNameArgMixin, BaseLs):
+class Ls(B2URIMustPointToFolderMixin, B2URIBucketNFolderNameArgMixin, BaseLs):
     """
     {BaseLs}
 
     Examples
 
     .. note::
 
@@ -88,14 +88,32 @@
 
     - **listFiles**
     - **listBuckets** (if bucket name is not provided)
     """
     ALLOW_ALL_BUCKETS = True
 
 
+class HyphenFilenameMixin:
+    def get_input_stream(self, filename):
+        if filename == '-' and os.path.exists('-'):
+            self._print_stderr(
+                "WARNING: Filename `-` won't be supported in the future and will always be treated as stdin alias."
+            )
+            return '-'
+        return super().get_input_stream(filename)
+
+
+class UploadUnboundStream(HyphenFilenameMixin, UploadUnboundStream):
+    __doc__ = UploadUnboundStream.__doc__
+
+
+class UploadFile(HyphenFilenameMixin, UploadFile):
+    __doc__ = UploadFile.__doc__
+
+
 B2.register_subcommand(AuthorizeAccount)
 B2.register_subcommand(CancelAllUnfinishedLargeFiles)
 B2.register_subcommand(CancelLargeFile)
 B2.register_subcommand(ClearAccount)
 B2.register_subcommand(CopyFileById)
 B2.register_subcommand(CreateBucket)
 B2.register_subcommand(CreateKey)
```

### Comparing `b2-4.0.0/b2/_internal/b2v4/registry.py` & `b2-4.0.1/b2/_internal/b2v4/registry.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/console_tool.py` & `b2-4.0.1/b2/_internal/console_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -2383,20 +2383,21 @@
         if args.escape_control_characters:
             name = escape_control_chars(name)
         self._print(name)
 
     def _get_ls_generator(self, args, b2_uri: B2URI | None = None):
         b2_uri = b2_uri or self.get_b2_uri_from_arg(args)
         try:
-            yield from self.api.list_file_versions_by_uri(
+            yield from self.api.ls(
                 b2_uri,
                 latest_only=not args.versions,
                 recursive=args.recursive,
                 with_wildcard=args.with_wildcard,
                 filters=args.filters,
+                folder_to_list_can_be_a_file=True,
             )
         except Exception as err:
             raise CommandError(unprintable_to_hex(str(err))) from err
 
     def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI:
         raise NotImplementedError
 
@@ -3429,20 +3430,15 @@
         kwargs["buffers_count"] = kwargs["threads"] + 1
         kwargs["read_size"] = kwargs["min_part_size"] or DEFAULT_MIN_PART_SIZE
         return kwargs
 
     def get_input_stream(self, filename: str) -> str | int | io.BinaryIO:
         """Get input stream IF filename points to a FIFO or stdin."""
         if filename == "-":
-            if os.path.exists('-'):
-                self._print_stderr(
-                    "WARNING: Filename `-` won't be supported in the future and will always be treated as stdin alias."
-                )
-            else:
-                return sys.stdin.buffer if platform.system() == "Windows" else sys.stdin.fileno()
+            return sys.stdin.buffer if platform.system() == "Windows" else sys.stdin.fileno()
         elif points_to_fifo(pathlib.Path(filename)):
             return filename
 
         raise self.NotAnInputStream()
 
     def file_identifier_to_read_stream(self, file_id: str | int | BinaryIO, buffering) -> BinaryIO:
         if isinstance(file_id, (str, int)):
```

### Comparing `b2-4.0.0/b2/_internal/json_encoder.py` & `b2-4.0.1/b2/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/_internal/version_listing.py` & `b2-4.0.1/b2/_internal/version_listing.py`

 * *Files identical despite different names*

### Comparing `b2-4.0.0/b2/licenses_output.txt` & `b2-4.0.1/b2/licenses_output.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9275,15 +9275,15 @@
 000243a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000243b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
 000243c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000243d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000243e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000243f0: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020 2020  ------+.|       
 00024400: 6232 7364 6b20 2020 2020 2020 207c 2020  b2sdk        |  
-00024410: 2020 322e 322e 3120 2020 207c 2020 2020    2.2.1    |    
+00024410: 2020 322e 332e 3020 2020 207c 2020 2020    2.3.0    |    
 00024420: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
 00024430: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
 00024440: 2020 207c 2020 4261 636b 626c 617a 6520     |  Backblaze 
 00024450: 496e 6320 3c73 7570 706f 7274 4062 6163  Inc <support@bac
 00024460: 6b62 6c61 7a65 2e63 6f6d 3e20 2020 7c20  kblaze.com>   | 
 00024470: 2020 2020 2020 2068 7474 7073 3a2f 2f67         https://g
 00024480: 6974 6875 622e 636f 6d2f 4261 636b 626c  ithub.com/Backbl
```

### Comparing `b2-4.0.0/pyproject.toml` & `b2-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "argcomplete>=2,<4",
     "arrow>=1.0.2,<2.0.0",
-    "b2sdk>=2.2.1,<3",
+    "b2sdk>=2.3.0,<3",
     "docutils>=0.18.1",
     "idna~=3.4; platform_system == 'Java'",
     "importlib-metadata>=3.3; python_version < '3.8'",
     "phx-class-registry>=4.0,<5",
     "rst2ansi==0.1.5",
     "tabulate==0.9.0",
     "tqdm>=4.65.0,<5",
     "platformdirs>=3.11.0,<5",
     "setuptools>=60; python_version < '3.10'",
 ]
-version = "4.0.0"
+version = "4.0.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 doc = [
     "sadisplay>=0.4.9; python_version>='3.9'",
```

### Comparing `b2-4.0.0/PKG-INFO` & `b2-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2
-Version: 4.0.0
+Version: 4.0.1
 Summary: Command Line Tool for Backblaze B2
 Keywords: backblaze b2 cloud storage
 Author-Email: Backblaze Inc <support@backblaze.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/Backblaze/B2_Command_Line_Tool
 Requires-Python: >=3.7
 Requires-Dist: argcomplete<4,>=2
 Requires-Dist: arrow<2.0.0,>=1.0.2
-Requires-Dist: b2sdk<3,>=2.2.1
+Requires-Dist: b2sdk<3,>=2.3.0
 Requires-Dist: docutils>=0.18.1
 Requires-Dist: idna~=3.4; platform_system == "Java"
 Requires-Dist: importlib-metadata>=3.3; python_version < "3.8"
 Requires-Dist: phx-class-registry<5,>=4.0
 Requires-Dist: rst2ansi==0.1.5
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tqdm<5,>=4.65.0
```

