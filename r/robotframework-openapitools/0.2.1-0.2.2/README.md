# Comparing `tmp/robotframework_openapitools-0.2.1.tar.gz` & `tmp/robotframework_openapitools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapitools-0.2.1.tar", max compression
+gzip compressed data, was "robotframework_openapitools-0.2.2.tar", max compression
```

## Comparing `robotframework_openapitools-0.2.1.tar` & `robotframework_openapitools-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.2.1/LICENSE
--rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.2.1/docs/README.md
--rwxr-xr-x   0        0        0     3371 2024-04-18 10:12:45.018662 robotframework_openapitools-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.2.1/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32851 2024-04-12 12:59:35.488243 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_executors.py
--rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    28323 2024-04-18 10:17:56.759029 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    15214 2024-04-12 12:59:35.504855 robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.2.1/src/OpenApiDriver/py.typed
--rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.2.1/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0    11794 2024-04-18 09:40:15.299767 robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_base.py
--rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_utils.py
--rwxr-xr-x   0        0        0      379 2024-04-18 10:15:55.247807 robotframework_openapitools-0.2.1/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    33102 2024-04-18 10:17:56.170803 robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec
--rwxr-xr-x   0        0        0    65826 2024-04-18 10:15:55.249816 robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.2.1/src/OpenApiLibCore/py.typed
--rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.2.1/src/OpenApiLibCore/value_utils.py
--rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.2.1/src/roboswag/__init__.py
--rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.2.1/src/roboswag/__main__.py
--rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.2.1/src/roboswag/auth.py
--rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.2.1/src/roboswag/cli.py
--rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.2.1/src/roboswag/core.py
--rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.2.1/src/roboswag/generate/__init__.py
--rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.2.1/src/roboswag/generate/generate.py
--rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.2.1/src/roboswag/generate/models/__init__.py
--rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.2.1/src/roboswag/generate/models/api.py
--rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.2.1/src/roboswag/generate/models/definition.py
--rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.2.1/src/roboswag/generate/models/endpoint.py
--rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.2.1/src/roboswag/generate/models/parameter.py
--rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/response.py
--rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/tag.py
--rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/models/utils.py
--rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/api_init.jinja
--rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/models.jinja
--rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/generate/templates/paths.jinja
--rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.2.1/src/roboswag/logger.py
--rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/__init__.py
--rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/core.py
--rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/schema.py
--rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.1/src/roboswag/validate/text_response.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.2.2/LICENSE
+-rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.2.2/docs/README.md
+-rwxr-xr-x   0        0        0     3371 2024-05-15 18:43:37.237974 robotframework_openapitools-0.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.2.2/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    12260 2024-05-15 07:12:40.600674 robotframework_openapitools-0.2.2/src/OpenApiDriver/openapi_executors.py
+-rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.2.2/src/OpenApiDriver/openapi_reader.py
+-rwxr-xr-x   0        0        0    28322 2024-05-15 18:47:15.670699 robotframework_openapitools-0.2.2/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15214 2024-04-12 12:59:35.504855 robotframework_openapitools-0.2.2/src/OpenApiDriver/openapidriver.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.2.2/src/OpenApiDriver/py.typed
+-rw-r--r--   0        0        0     1604 2024-05-15 07:12:40.610185 robotframework_openapitools-0.2.2/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0    11792 2024-05-15 12:22:22.172918 robotframework_openapitools-0.2.2/src/OpenApiLibCore/dto_base.py
+-rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.2.2/src/OpenApiLibCore/dto_utils.py
+-rwxr-xr-x   0        0        0      379 2024-04-18 10:15:55.247807 robotframework_openapitools-0.2.2/src/OpenApiLibCore/oas_cache.py
+-rwxr-xr-x   0        0        0    39801 2024-05-15 18:47:15.049239 robotframework_openapitools-0.2.2/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    86685 2024-05-15 12:33:23.157719 robotframework_openapitools-0.2.2/src/OpenApiLibCore/openapi_libcore.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.2.2/src/OpenApiLibCore/py.typed
+-rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.2.2/src/OpenApiLibCore/value_utils.py
+-rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.2.2/src/roboswag/__init__.py
+-rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.2.2/src/roboswag/__main__.py
+-rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.2.2/src/roboswag/auth.py
+-rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.2.2/src/roboswag/cli.py
+-rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.2.2/src/roboswag/core.py
+-rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.2.2/src/roboswag/generate/__init__.py
+-rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.2.2/src/roboswag/generate/generate.py
+-rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.2.2/src/roboswag/generate/models/__init__.py
+-rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.2.2/src/roboswag/generate/models/api.py
+-rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.2.2/src/roboswag/generate/models/definition.py
+-rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.2.2/src/roboswag/generate/models/endpoint.py
+-rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.2.2/src/roboswag/generate/models/parameter.py
+-rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/models/response.py
+-rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/models/tag.py
+-rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/models/utils.py
+-rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/templates/api_init.jinja
+-rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/templates/models.jinja
+-rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/generate/templates/paths.jinja
+-rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.2.2/src/roboswag/logger.py
+-rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/validate/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/validate/core.py
+-rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/validate/schema.py
+-rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.2/src/roboswag/validate/text_response.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.2.2/PKG-INFO
```

### Comparing `robotframework_openapitools-0.2.1/LICENSE` & `robotframework_openapitools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/pyproject.toml` & `robotframework_openapitools-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapitools"
-version = "0.2.1"
+version = "0.2.2"
 description = "A set of Robot Framework libraries to test APIs for which the OAS is available."
 license = "Apache-2.0"
 authors = [
     "Bartlomiej Hirsz <bartek.hirsz@gmail.com>",
     "Mateusz Nojek <matnojek@gmail.com>",
     "Robin Mackaij <r.a.mackaij@gmail.com>"
 ]
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiDriver/__init__.py` & `robotframework_openapitools-0.2.2/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapitools-0.2.2/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.2/src/OpenApiDriver/openapidriver.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.2/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-18T10:17:57+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
-  <version>0.2.1</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-05-15T18:47:16+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
+  <version>0.2.2</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="144">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
@@ -282,15 +282,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Test Endpoint" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="175">
+    <kw name="Test Endpoint" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="156">
       <arguments repr="path: str, method: str, status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -302,15 +302,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
       <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
-    <kw name="Test Forbidden" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="116">
+    <kw name="Test Forbidden" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="97">
       <arguments repr="path: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -318,15 +318,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request for &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; on the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt;, with the provided authorization.&lt;/p&gt;
 &lt;p&gt;This keyword only passes if the response code is 403: Forbidden.&lt;/p&gt;
 &lt;p&gt;For this keyword to pass, the authorization parameters used to initialize the library should grant insufficient access rights to the target endpoint. &amp;gt; Note: No headers or (json) body are send with the request. For security reasons, the access rights validation should be checked first.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for `method` on the `path`, with the provided authorization.</shortdoc>
     </kw>
-    <kw name="Test Invalid Url" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="133">
+    <kw name="Test Invalid Url" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="114">
       <arguments repr="path: str, method: str, expected_status_code: int = 404">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -340,15 +340,15 @@
       </arguments>
       <doc>&lt;p&gt;Perform a request for the provided 'path' and 'method' where the url for the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; is invalidated.&lt;/p&gt;
 &lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the path contains no parts that can be invalidated.&lt;/p&gt;
 &lt;p&gt;The optional &lt;span class=&quot;name&quot;&gt;expected_status_code&lt;/span&gt; parameter (default: 404) can be set to the expected status code for APIs that do not return a 404 on invalid urls.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: Depending on API design, the url may be validated before or after validation of headers, query parameters and / or (json) body. By default, no parameters are send with the request. The &lt;span class=&quot;name&quot;&gt;require_body_for_invalid_url&lt;/span&gt; parameter can be set to &lt;span class=&quot;name&quot;&gt;True&lt;/span&gt; if needed.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for the provided 'path' and 'method' where the url for the `path` is invalidated.</shortdoc>
     </kw>
-    <kw name="Test Unauthorized" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="95">
+    <kw name="Test Unauthorized" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="76">
       <arguments repr="path: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiDriver/openapidriver.py` & `robotframework_openapitools-0.2.2/src/OpenApiDriver/openapidriver.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/__init__.py` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-"""
-The OpenApiLibCore package is intended to be used as a dependency for other
-Robot Framework libraries that facilitate the testing of OpenAPI / Swagger APIs.
-The following classes and constants are exposed to be used by the library user:
-- OpenApiLibCore: The class to be imported in the Robot Framework library.
-- IdDependency, IdReference, PathPropertiesConstraint, PropertyValueConstraint,
-    UniquePropertyValueConstraint: Classes to be subclassed by the library user
-    when implementing a custom mapping module (advanced use).
-- Dto, Relation: Base classes that can be used for type annotations.
-- IGNORE: A special constant that can be used as a value in the PropertyValueConstraint.
-"""
-
-from importlib.metadata import version
-
-from OpenApiLibCore.dto_base import (
-    Dto,
-    IdDependency,
-    IdReference,
-    PathPropertiesConstraint,
-    PropertyValueConstraint,
-    Relation,
-    UniquePropertyValueConstraint,
-    resolve_schema,
-)
-from OpenApiLibCore.dto_utils import DefaultDto
-from OpenApiLibCore.openapi_libcore import OpenApiLibCore, RequestData, RequestValues
-from OpenApiLibCore.value_utils import IGNORE
-
-try:
-    __version__ = version("robotframework-openapi-libcore")
-except Exception:  # pragma: no cover
-    pass
-
-__all__ = [
-    "Dto",
-    "IdDependency",
-    "IdReference",
-    "PathPropertiesConstraint",
-    "PropertyValueConstraint",
-    "Relation",
-    "UniquePropertyValueConstraint",
-    "DefaultDto",
-    "OpenApiLibCore",
-    "RequestData",
-    "RequestValues",
-    "resolve_schema",
-    "IGNORE",
-]
+"""
+The OpenApiLibCore package is intended to be used as a dependency for other
+Robot Framework libraries that facilitate the testing of OpenAPI / Swagger APIs.
+The following classes and constants are exposed to be used by the library user:
+- OpenApiLibCore: The class to be imported in the Robot Framework library.
+- IdDependency, IdReference, PathPropertiesConstraint, PropertyValueConstraint,
+    UniquePropertyValueConstraint: Classes to be subclassed by the library user
+    when implementing a custom mapping module (advanced use).
+- Dto, Relation: Base classes that can be used for type annotations.
+- IGNORE: A special constant that can be used as a value in the PropertyValueConstraint.
+"""
+
+from importlib.metadata import version
+
+from OpenApiLibCore.dto_base import (
+    Dto,
+    IdDependency,
+    IdReference,
+    PathPropertiesConstraint,
+    PropertyValueConstraint,
+    Relation,
+    UniquePropertyValueConstraint,
+    resolve_schema,
+)
+from OpenApiLibCore.dto_utils import DefaultDto
+from OpenApiLibCore.openapi_libcore import (
+    OpenApiLibCore,
+    RequestData,
+    RequestValues,
+    ValidationLevel,
+)
+from OpenApiLibCore.value_utils import IGNORE
+
+try:
+    __version__ = version("robotframework-openapi-libcore")
+except Exception:  # pragma: no cover
+    pass
+
+__all__ = [
+    "Dto",
+    "IdDependency",
+    "IdReference",
+    "PathPropertiesConstraint",
+    "PropertyValueConstraint",
+    "Relation",
+    "UniquePropertyValueConstraint",
+    "DefaultDto",
+    "OpenApiLibCore",
+    "RequestData",
+    "RequestValues",
+    "ValidationLevel",
+    "resolve_schema",
+    "IGNORE",
+]
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_base.py` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/dto_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
             if isinstance(value, dict):
                 # if the key holds a dict, merge the values (e.g. 'properties')
                 merged_schema[key].update(value)
             elif isinstance(value, list):
                 # if the key holds a list, extend the values (e.g. 'required')
                 merged_schema[key].extend(value)
             elif value != merged_schema[key]:
-                logger.warning(
-                    f"key '{key}' with value '{merged_schema[key]}' not "
-                    f"updated to '{value}'"
+                logger.debug(
+                    f"key '{key}' with value '{merged_schema[key]}'"
+                    f" not updated to '{value}'"
                 )
         else:
             merged_schema[key] = value
     return merged_schema
 
 
 class ResourceRelation(ABC):  # pylint: disable=too-few-public-methods
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 11% similar despite different names*

#### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-18T10:17:56+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="415">
-  <version>0.2.1</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-05-15T18:47:15+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="430">
+  <version>0.2.2</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
-    <init name="__init__" lineno="423">
+    <init name="__init__" lineno="438">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
@@ -194,15 +194,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1591">
+    <kw name="Authorized Request" lineno="1607">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -288,39 +288,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1495">
+    <kw name="Ensure In Use" lineno="1511">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type name="IdReference">IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="866">
+    <kw name="Get Ids From Url" lineno="882">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1272">
+    <kw name="Get Invalid Json Data" lineno="1288">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -335,40 +335,40 @@
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1320">
+    <kw name="Get Invalidated Parameters" lineno="1336">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1238">
+    <kw name="Get Invalidated Url" lineno="1254">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="1114">
+    <kw name="Get Json Data For Dto Class" lineno="1130">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type name="Dict" typedoc="dictionary">
             Dict[str, Any]
             <type name="str" typedoc="string">str</type>
             <type name="Any" typedoc="Any">Any</type>
@@ -390,15 +390,15 @@
           <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1539">
+    <kw name="Get Json Data With Conflict" lineno="1555">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -412,54 +412,54 @@
           <name>conflict_status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1260">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1276">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="906">
+    <kw name="Get Request Data" lineno="922">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="770">
+    <kw name="Get Valid Id For Endpoint" lineno="786">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="730">
+    <kw name="Get Valid Url" lineno="746">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -467,38 +467,153 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;This keyword returns a valid url for the given &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; and &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;If the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; contains path parameters the Get Valid Id For Endpoint keyword will be executed to retrieve valid ids for the path parameters.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: if valid ids cannot be retrieved within the scope of the API, the &lt;span class=&quot;name&quot;&gt;PathPropertiesConstraint&lt;/span&gt; Relation can be used. More information can be found &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;</doc>
       <shortdoc>This keyword returns a valid url for the given `endpoint` and `method`.</shortdoc>
     </kw>
-    <kw name="Set Origin" lineno="592">
+    <kw name="Perform Validated Request" lineno="1645">
+      <arguments repr="path: str, status_code: int, request_values: RequestValues, original_data: Dict[str, Any] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
+          <type name="str" typedoc="string">str</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
+          <name>status_code</name>
+          <type name="int" typedoc="integer">int</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_values: RequestValues">
+          <name>request_values</name>
+          <type name="RequestValues">RequestValues</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="original_data: Dict[str, Any] | None = None">
+          <name>original_data</name>
+          <type name="Union" union="true">
+            Dict[str, Any] | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, Any]
+              <type name="str" typedoc="string">str</type>
+              <type name="Any" typedoc="Any">Any</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
+          <default>None</default>
+        </arg>
+      </arguments>
+      <doc>&lt;p&gt;This keyword first calls the Authorized Request keyword, then the Validate Response keyword and finally validates, for &lt;span class=&quot;name&quot;&gt;DELETE&lt;/span&gt; operations, whether the target resource was indeed deleted (OK response) or not (error responses).&lt;/p&gt;</doc>
+      <shortdoc>This keyword first calls the Authorized Request keyword, then the Validate Response keyword and finally validates, for `DELETE` operations, whether the target resource was indeed deleted (OK response) or not (error responses).</shortdoc>
+    </kw>
+    <kw name="Set Origin" lineno="607">
       <arguments repr="origin: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="origin: str">
           <name>origin</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Update the &lt;span class=&quot;name&quot;&gt;origin&lt;/span&gt; after the library is imported.&lt;/p&gt;
 &lt;p&gt;This can be done during the &lt;span class=&quot;name&quot;&gt;Suite setup&lt;/span&gt; when using DataDriver in situations where the OpenAPI document is available on disk but the target host address is not known before the test starts.&lt;/p&gt;
 &lt;p&gt;In combination with OpenApiLibCore, the &lt;span class=&quot;name&quot;&gt;origin&lt;/span&gt; can be used at any point to target another server that hosts an API that complies to the same OAS.&lt;/p&gt;</doc>
       <shortdoc>Update the `origin` after the library is imported.</shortdoc>
     </kw>
+    <kw name="Validate Resource Properties" lineno="1871">
+      <arguments repr="resource: Dict[str, Any], schema: Dict[str, Any]">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource: Dict[str, Any]">
+          <name>resource</name>
+          <type name="Dict" typedoc="dictionary">
+            Dict[str, Any]
+            <type name="str" typedoc="string">str</type>
+            <type name="Any" typedoc="Any">Any</type>
+          </type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
+          <name>schema</name>
+          <type name="Dict" typedoc="dictionary">
+            Dict[str, Any]
+            <type name="str" typedoc="string">str</type>
+            <type name="Any" typedoc="Any">Any</type>
+          </type>
+        </arg>
+      </arguments>
+      <doc>&lt;p&gt;Validate that the &lt;span class=&quot;name&quot;&gt;resource&lt;/span&gt; does not contain any properties that are not defined in the &lt;span class=&quot;name&quot;&gt;schema_properties&lt;/span&gt;.&lt;/p&gt;</doc>
+      <shortdoc>Validate that the `resource` does not contain any properties that are not defined in the `schema_properties`.</shortdoc>
+    </kw>
+    <kw name="Validate Response" lineno="1719">
+      <arguments repr="path: str, response: Response, original_data: Dict[str, Any] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
+          <type name="str" typedoc="string">str</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="response: Response">
+          <name>response</name>
+          <type name="Response">Response</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="original_data: Dict[str, Any] | None = None">
+          <name>original_data</name>
+          <type name="Union" union="true">
+            Dict[str, Any] | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, Any]
+              <type name="str" typedoc="string">str</type>
+              <type name="Any" typedoc="Any">Any</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
+          <default>None</default>
+        </arg>
+      </arguments>
+      <doc>&lt;p&gt;Validate the &lt;span class=&quot;name&quot;&gt;response&lt;/span&gt; by performing the following validations:&lt;/p&gt;
+&lt;ul&gt;
+&lt;li&gt;validate the &lt;span class=&quot;name&quot;&gt;response&lt;/span&gt; against the openapi schema for the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;&lt;/li&gt;
+&lt;li&gt;validate that the response does not contain extra properties&lt;/li&gt;
+&lt;li&gt;validate that a href, if present, refers to the correct resource&lt;/li&gt;
+&lt;li&gt;validate that the value for a property that is in the response is equal to the property value that was send&lt;/li&gt;
+&lt;li&gt;validate that no &lt;span class=&quot;name&quot;&gt;original_data&lt;/span&gt; is preserved when performing a PUT operation&lt;/li&gt;
+&lt;li&gt;validate that a PATCH operation only updates the provided properties&lt;/li&gt;
+&lt;/ul&gt;</doc>
+      <shortdoc>Validate the `response` by performing the following validations: - validate the `response` against the openapi schema for the `endpoint` - validate that the response does not contain extra properties - validate that a href, if present, refers to the correct resource - validate that the value for a property that is in the response is equal to     the property value that was send - validate that no `original_data` is preserved when performing a PUT operation - validate that a PATCH operation only updates the provided properties</shortdoc>
+    </kw>
+    <kw name="Validate Send Response" lineno="1989">
+      <arguments repr="response: Response, original_data: Dict[str, Any] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="response: Response">
+          <name>response</name>
+          <type name="Response">Response</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="original_data: Dict[str, Any] | None = None">
+          <name>original_data</name>
+          <type name="Union" union="true">
+            Dict[str, Any] | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, Any]
+              <type name="str" typedoc="string">str</type>
+              <type name="Any" typedoc="Any">Any</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
+          <default>None</default>
+        </arg>
+      </arguments>
+      <doc>&lt;p&gt;Validate that each property that was send that is in the response has the value that was send. In case a PATCH request, validate that only the properties that were patched have changed and that other properties are still at their pre-patch values.&lt;/p&gt;</doc>
+      <shortdoc>Validate that each property that was send that is in the response has the value that was send. In case a PATCH request, validate that only the properties that were patched have changed and that other properties are still at their pre-patch values.</shortdoc>
+    </kw>
   </keywords>
   <datatypes/>
   <typedocs>
     <type name="Any" type="Standard">
       <doc>&lt;p&gt;Any value is accepted. No conversion is done.&lt;/p&gt;</doc>
       <accepts>
         <type>Any</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Authorized Request</usage>
         <usage>Get Json Data For Dto Class</usage>
+        <usage>Perform Validated Request</usage>
+        <usage>Validate Resource Properties</usage>
+        <usage>Validate Response</usage>
+        <usage>Validate Send Response</usage>
       </usages>
     </type>
     <type name="boolean" type="Standard">
       <doc>&lt;p&gt;Strings &lt;code&gt;TRUE&lt;/code&gt;, &lt;code&gt;YES&lt;/code&gt;, &lt;code&gt;ON&lt;/code&gt; and &lt;code&gt;1&lt;/code&gt; are converted to Boolean &lt;code&gt;True&lt;/code&gt;, the empty string as well as strings &lt;code&gt;FALSE&lt;/code&gt;, &lt;code&gt;NO&lt;/code&gt;, &lt;code&gt;OFF&lt;/code&gt; and &lt;code&gt;0&lt;/code&gt; are converted to Boolean &lt;code&gt;False&lt;/code&gt;, and the string &lt;code&gt;NONE&lt;/code&gt; is converted to the Python &lt;code&gt;None&lt;/code&gt; object. Other strings and other accepted values are passed as-is, allowing keywords to handle them specially if needed. All string comparisons are case-insensitive.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;TRUE&lt;/code&gt; (converted to &lt;code&gt;True&lt;/code&gt;), &lt;code&gt;off&lt;/code&gt; (converted to &lt;code&gt;False&lt;/code&gt;), &lt;code&gt;example&lt;/code&gt; (used as-is)&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
@@ -519,14 +634,18 @@
         <type>string</type>
         <type>Mapping</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Authorized Request</usage>
         <usage>Get Json Data For Dto Class</usage>
+        <usage>Perform Validated Request</usage>
+        <usage>Validate Resource Properties</usage>
+        <usage>Validate Response</usage>
+        <usage>Validate Send Response</usage>
       </usages>
     </type>
     <type name="float" type="Standard">
       <doc>&lt;p&gt;Conversion is done using Python's &lt;a href=&quot;https://docs.python.org/library/functions.html#float&quot;&gt;float&lt;/a&gt; built-in function.&lt;/p&gt;
 &lt;p&gt;Starting from RF 4.1, spaces and underscores can be used as visual separators for digit grouping purposes.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;3.14&lt;/code&gt;, &lt;code&gt;2.9979e8&lt;/code&gt;, &lt;code&gt;10 000.000 01&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
@@ -548,14 +667,15 @@
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Authorized Request</usage>
         <usage>Get Invalid Json Data</usage>
         <usage>Get Invalidated Parameters</usage>
         <usage>Get Json Data With Conflict</usage>
+        <usage>Perform Validated Request</usage>
       </usages>
     </type>
     <type name="list" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#list&quot;&gt;list&lt;/a&gt; literals. They are converted to actual lists using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including lists and other containers.&lt;/p&gt;
 &lt;p&gt;If the type has nested types like &lt;code&gt;list[int]&lt;/code&gt;, items are converted to those types automatically. This in new in Robot Framework 6.0.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;['one', 'two']&lt;/code&gt;, &lt;code&gt;[('one', 1), ('two', 2)]&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
@@ -571,14 +691,17 @@
       <doc>&lt;p&gt;String &lt;code&gt;NONE&lt;/code&gt; (case-insensitive) is converted to Python &lt;code&gt;None&lt;/code&gt; object. Other values cause an error.&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Authorized Request</usage>
+        <usage>Perform Validated Request</usage>
+        <usage>Validate Response</usage>
+        <usage>Validate Send Response</usage>
       </usages>
     </type>
     <type name="Path" type="Standard">
       <doc>&lt;p&gt;Strings are converted &lt;a href=&quot;https://docs.python.org/library/pathlib.html&quot;&gt;Path&lt;/a&gt; objects. On Windows &lt;code&gt;/&lt;/code&gt; is converted to &lt;code&gt;\&lt;/code&gt; automatically.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;/tmp/absolute/path&lt;/code&gt;, &lt;code&gt;relative/path/to/file.ext&lt;/code&gt;, &lt;code&gt;name.txt&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
@@ -602,15 +725,19 @@
         <usage>Get Invalidated Url</usage>
         <usage>Get Json Data For Dto Class</usage>
         <usage>Get Json Data With Conflict</usage>
         <usage>Get Parameterized Endpoint From Url</usage>
         <usage>Get Request Data</usage>
         <usage>Get Valid Id For Endpoint</usage>
         <usage>Get Valid Url</usage>
+        <usage>Perform Validated Request</usage>
         <usage>Set Origin</usage>
+        <usage>Validate Resource Properties</usage>
+        <usage>Validate Response</usage>
+        <usage>Validate Send Response</usage>
       </usages>
     </type>
     <type name="tuple" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#tuple&quot;&gt;tuple&lt;/a&gt; literals. They are converted to actual tuples using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including tuples and other containers.&lt;/p&gt;
 &lt;p&gt;If the type has nested types like &lt;code&gt;tuple[str, int, int]&lt;/code&gt;, items are converted to those types automatically. This in new in Robot Framework 6.0.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;('one', 'two')&lt;/code&gt;, &lt;code&gt;(('one', 1), ('two', 2))&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 15% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 """
 
 import json as _json
 import re
 import sys
 from copy import deepcopy
 from dataclasses import Field, dataclass, field, make_dataclass
+from enum import Enum
 from functools import cached_property
 from itertools import zip_longest
 from logging import getLogger
 from pathlib import Path
 from random import choice, sample
 from typing import (
     Any,
@@ -143,19 +144,24 @@
 from uuid import uuid4
 
 from openapi_core import Config, OpenAPI, Spec
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
-from prance import ResolvingParser, ValidationError
+from openapi_core.exceptions import OpenAPIError
+from openapi_core.validation.exceptions import ValidationError
+from openapi_core.validation.response.exceptions import ResponseValidationError
+from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
+from prance import ResolvingParser
 from prance.util.url import ResolutionError
 from requests import Response, Session
 from requests.auth import AuthBase, HTTPBasicAuth
 from requests.cookies import RequestsCookieJar as CookieJar
+from robot.api import Failure
 from robot.api.deco import keyword, library
 from robot.libraries.BuiltIn import BuiltIn
 
 from OpenApiLibCore import value_utils
 from OpenApiLibCore.dto_base import (
     NOT_SET,
     Dto,
@@ -177,14 +183,23 @@
 from OpenApiLibCore.value_utils import FAKE, IGNORE, JSON
 
 run_keyword = BuiltIn().run_keyword
 
 logger = getLogger(__name__)
 
 
+class ValidationLevel(str, Enum):
+    """The available levels for the response_validation parameter."""
+
+    DISABLED = "DISABLED"
+    INFO = "INFO"
+    WARN = "WARN"
+    STRICT = "STRICT"
+
+
 def get_safe_key(key: str) -> str:
     """
     Helper function to convert a valid JSON property name to a string that can be used
     as a Python variable or function / method name.
     """
     key = key.replace("-", "_")
     key = key.replace("@", "_")
@@ -639,15 +654,16 @@
             if content_dict is None:
                 for value in item.values():
                     yield from self._get_json_types(value)
 
             else:
                 for content_type in content_dict:
                     if "json" in content_type:
-                        yield content_type
+                        content_type_without_charset, _, _ = content_type.partition(";")
+                        yield content_type_without_charset
 
         if isinstance(item, list):
             for list_item in item:
                 yield from self._get_json_types(list_item)
 
     def _load_specs_and_validator(
         self,
@@ -1620,7 +1636,461 @@
             auth=self.auth,
             proxies=self.proxies,
             verify=self.verify,
             cert=self.cert,
         )
         logger.debug(f"Response text: {response.text}")
         return response
+
+    @keyword
+    def perform_validated_request(
+        self,
+        path: str,
+        status_code: int,
+        request_values: RequestValues,
+        original_data: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """
+        This keyword first calls the Authorized Request keyword, then the Validate
+        Response keyword and finally validates, for `DELETE` operations, whether
+        the target resource was indeed deleted (OK response) or not (error responses).
+        """
+        response = run_keyword(
+            "authorized_request",
+            request_values.url,
+            request_values.method,
+            request_values.params,
+            request_values.headers,
+            request_values.json_data,
+        )
+        if response.status_code != status_code:
+            try:
+                response_json = response.json()
+            except Exception as _:  # pylint: disable=broad-except
+                logger.info(
+                    f"Failed to get json content from response. "
+                    f"Response text was: {response.text}"
+                )
+                response_json = {}
+            if not response.ok:
+                if description := response_json.get("detail"):
+                    pass
+                else:
+                    description = response_json.get(
+                        "message", "response contains no message or detail."
+                    )
+                logger.error(f"{response.reason}: {description}")
+
+            logger.debug(
+                f"\nSend: {_json.dumps(request_values.json_data, indent=4, sort_keys=True)}"
+                f"\nGot: {_json.dumps(response_json, indent=4, sort_keys=True)}"
+            )
+            raise AssertionError(
+                f"Response status_code {response.status_code} was not {status_code}"
+            )
+
+        run_keyword("validate_response", path, response, original_data)
+
+        if request_values.method == "DELETE":
+            get_request_data = self.get_request_data(endpoint=path, method="GET")
+            get_params = get_request_data.params
+            get_headers = get_request_data.headers
+            get_response = run_keyword(
+                "authorized_request", request_values.url, "GET", get_params, get_headers
+            )
+            if response.ok:
+                if get_response.ok:
+                    raise AssertionError(
+                        f"Resource still exists after deletion. Url was {request_values.url}"
+                    )
+                # if the path supports GET, 404 is expected, if not 405 is expected
+                if get_response.status_code not in [404, 405]:
+                    logger.warning(
+                        f"Unexpected response after deleting resource: Status_code "
+                        f"{get_response.status_code} was received after trying to get {request_values.url} "
+                        f"after sucessfully deleting it."
+                    )
+            elif not get_response.ok:
+                raise AssertionError(
+                    f"Resource could not be retrieved after failed deletion. "
+                    f"Url was {request_values.url}, status_code was {get_response.status_code}"
+                )
+
+    @keyword
+    def validate_response(
+        self,
+        path: str,
+        response: Response,
+        original_data: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        """
+        Validate the `response` by performing the following validations:
+        - validate the `response` against the openapi schema for the `endpoint`
+        - validate that the response does not contain extra properties
+        - validate that a href, if present, refers to the correct resource
+        - validate that the value for a property that is in the response is equal to
+            the property value that was send
+        - validate that no `original_data` is preserved when performing a PUT operation
+        - validate that a PATCH operation only updates the provided properties
+        """
+        if response.status_code == 204:
+            assert not response.content
+            return None
+
+        try:
+            self._validate_response_against_spec(response)
+        except OpenAPIError as exception:
+            raise Failure(f"Response did not pass schema validation: {exception}")
+
+        request_method = response.request.method
+        if request_method is None:
+            logger.warning(
+                f"Could not validate response for path {path}; no method found "
+                f"on the request property of the provided response."
+            )
+            return None
+
+        response_spec = self._get_response_spec(
+            path=path,
+            method=request_method,
+            status_code=response.status_code,
+        )
+
+        content_type_from_response = response.headers.get("Content-Type", "unknown")
+        mime_type_from_response, _, _ = content_type_from_response.partition(";")
+
+        if not response_spec.get("content"):
+            logger.warning(
+                "The response cannot be validated: 'content' not specified in the OAS."
+            )
+            return None
+
+        # multiple content types can be specified in the OAS
+        content_types = list(response_spec["content"].keys())
+        supported_types = [
+            ct for ct in content_types if ct.partition(";")[0].endswith("json")
+        ]
+        if not supported_types:
+            raise NotImplementedError(
+                f"The content_types '{content_types}' are not supported. "
+                f"Only json types are currently supported."
+            )
+        content_type = supported_types[0]
+        mime_type = content_type.partition(";")[0]
+
+        if mime_type != mime_type_from_response:
+            raise ValueError(
+                f"Content-Type '{content_type_from_response}' of the response "
+                f"does not match '{mime_type}' as specified in the OpenAPI document."
+            )
+
+        json_response = response.json()
+        response_schema = resolve_schema(
+            response_spec["content"][content_type]["schema"]
+        )
+
+        response_type = response_schema.get("type", "undefined")
+        if response_type not in ["object", "array"]:
+            self._validate_value_type(value=json_response, expected_type=response_type)
+            return None
+
+        if list_item_schema := response_schema.get("items"):
+            if not isinstance(json_response, list):
+                raise AssertionError(
+                    f"Response schema violation: the schema specifies an array as "
+                    f"response type but the response was of type {type(json_response)}."
+                )
+            type_of_list_items = list_item_schema.get("type")
+            if type_of_list_items == "object":
+                for resource in json_response:
+                    run_keyword(
+                        "validate_resource_properties", resource, list_item_schema
+                    )
+            else:
+                for item in json_response:
+                    self._validate_value_type(
+                        value=item, expected_type=type_of_list_items
+                    )
+            # no further validation; value validation of individual resources should
+            # be performed on the endpoints for the specific resource
+            return None
+
+        run_keyword("validate_resource_properties", json_response, response_schema)
+        # ensure the href is valid if present in the response
+        if href := json_response.get("href"):
+            self._assert_href_is_valid(href, json_response)
+        # every property that was sucessfully send and that is in the response
+        # schema must have the value that was send
+        if response.ok and response.request.method in ["POST", "PUT", "PATCH"]:
+            run_keyword("validate_send_response", response, original_data)
+        return None
+
+    def _assert_href_is_valid(self, href: str, json_response: Dict[str, Any]) -> None:
+        url = f"{self.origin}{href}"
+        path = url.replace(self.base_url, "")
+        request_data = self.get_request_data(endpoint=path, method="GET")
+        params = request_data.params
+        headers = request_data.headers
+        get_response = run_keyword("authorized_request", url, "GET", params, headers)
+        assert (
+            get_response.json() == json_response
+        ), f"{get_response.json()} not equal to original {json_response}"
+
+    def _validate_response_against_spec(self, response: Response) -> None:
+        try:
+            self.validate_response_vs_spec(
+                request=RequestsOpenAPIRequest(response.request),
+                response=RequestsOpenAPIResponse(response),
+            )
+        except ResponseValidationError as exception:
+            errors: List[InvalidSchemaValue] = exception.__cause__
+            validation_errors: Optional[List[ValidationError]] = getattr(
+                errors, "schema_errors", None
+            )
+            if validation_errors:
+                error_message = "\n".join(
+                    [
+                        f"{list(error.schema_path)}: {error.message}"
+                        for error in validation_errors
+                    ]
+                )
+            else:
+                error_message = str(exception)
+
+            if response.status_code == self.invalid_property_default_response:
+                logger.debug(error_message)
+                return
+            if self.response_validation == ValidationLevel.STRICT:
+                logger.error(error_message)
+                raise exception
+            if self.response_validation == ValidationLevel.WARN:
+                logger.warning(error_message)
+            elif self.response_validation == ValidationLevel.INFO:
+                logger.info(error_message)
+
+    @keyword
+    def validate_resource_properties(
+        self, resource: Dict[str, Any], schema: Dict[str, Any]
+    ) -> None:
+        """
+        Validate that the `resource` does not contain any properties that are not
+        defined in the `schema_properties`.
+        """
+        schema_properties = schema.get("properties", {})
+        property_names_from_schema = set(schema_properties.keys())
+        property_names_in_resource = set(resource.keys())
+
+        if property_names_from_schema != property_names_in_resource:
+            # The additionalProperties property determines whether properties with
+            # unspecified names are allowed. This property can be boolean or an object
+            # (dict) that specifies the type of any additional properties.
+            additional_properties = schema.get("additionalProperties", True)
+            if isinstance(additional_properties, bool):
+                allow_additional_properties = additional_properties
+                allowed_additional_properties_type = None
+            else:
+                allow_additional_properties = True
+                allowed_additional_properties_type = additional_properties["type"]
+
+            extra_property_names = property_names_in_resource.difference(
+                property_names_from_schema
+            )
+            if allow_additional_properties:
+                # If a type is defined for extra properties, validate them
+                if allowed_additional_properties_type:
+                    extra_properties = {
+                        key: value
+                        for key, value in resource.items()
+                        if key in extra_property_names
+                    }
+                    self._validate_type_of_extra_properties(
+                        extra_properties=extra_properties,
+                        expected_type=allowed_additional_properties_type,
+                    )
+                # If allowed, validation should not fail on extra properties
+                extra_property_names = set()
+
+            required_properties = set(schema.get("required", []))
+            missing_properties = required_properties.difference(
+                property_names_in_resource
+            )
+
+            if extra_property_names or missing_properties:
+                extra = (
+                    f"\n\tExtra properties in response: {extra_property_names}"
+                    if extra_property_names
+                    else ""
+                )
+                missing = (
+                    f"\n\tRequired properties missing in response: {missing_properties}"
+                    if missing_properties
+                    else ""
+                )
+                raise AssertionError(
+                    f"Response schema violation: the response contains properties that are "
+                    f"not specified in the schema or does not contain properties that are "
+                    f"required according to the schema."
+                    f"\n\tReceived in the response: {property_names_in_resource}"
+                    f"\n\tDefined in the schema:    {property_names_from_schema}"
+                    f"{extra}{missing}"
+                )
+
+    @staticmethod
+    def _validate_value_type(value: Any, expected_type: str) -> None:
+        type_mapping = {
+            "string": str,
+            "number": float,
+            "integer": int,
+            "boolean": bool,
+            "array": list,
+            "object": dict,
+        }
+        python_type = type_mapping.get(expected_type, None)
+        if python_type is None:
+            raise AssertionError(
+                f"Validation of type '{expected_type}' is not supported."
+            )
+        if not isinstance(value, python_type):
+            raise AssertionError(f"{value} is not of type {expected_type}")
+
+    @staticmethod
+    def _validate_type_of_extra_properties(
+        extra_properties: Dict[str, Any], expected_type: str
+    ) -> None:
+        type_mapping = {
+            "string": str,
+            "number": float,
+            "integer": int,
+            "boolean": bool,
+            "array": list,
+            "object": dict,
+        }
+
+        python_type = type_mapping.get(expected_type, None)
+        if python_type is None:
+            logger.warning(
+                f"Additonal properties were not validated: "
+                f"type '{expected_type}' is not supported."
+            )
+            return
+
+        invalid_extra_properties = {
+            key: value
+            for key, value in extra_properties.items()
+            if not isinstance(value, python_type)
+        }
+        if invalid_extra_properties:
+            raise AssertionError(
+                f"Response contains invalid additionalProperties: "
+                f"{invalid_extra_properties} are not of type {expected_type}."
+            )
+
+    @staticmethod
+    @keyword
+    def validate_send_response(
+        response: Response, original_data: Optional[Dict[str, Any]] = None
+    ) -> None:
+        """
+        Validate that each property that was send that is in the response has the value
+        that was send.
+        In case a PATCH request, validate that only the properties that were patched
+        have changed and that other properties are still at their pre-patch values.
+        """
+
+        def validate_list_response(
+            send_list: List[Any], received_list: List[Any]
+        ) -> None:
+            for item in send_list:
+                if item not in received_list:
+                    raise AssertionError(
+                        f"Received value '{received_list}' does "
+                        f"not contain '{item}' in the {response.request.method} request."
+                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+
+        def validate_dict_response(
+            send_dict: Dict[str, Any], received_dict: Dict[str, Any]
+        ) -> None:
+            for send_property_name, send_property_value in send_dict.items():
+                # sometimes, a property in the request is not in the response, e.g. a password
+                if send_property_name not in received_dict.keys():
+                    continue
+                if send_property_value is not None:
+                    # if a None value is send, the target property should be cleared or
+                    # reverted to the default value (which cannot be specified in the
+                    # openapi document)
+                    received_value = received_dict[send_property_name]
+                    # In case of lists / arrays, the send values are often appended to
+                    # existing data
+                    if isinstance(received_value, list):
+                        validate_list_response(
+                            send_list=send_property_value, received_list=received_value
+                        )
+                        continue
+
+                    # when dealing with objects, we'll need to iterate the properties
+                    if isinstance(received_value, dict):
+                        validate_dict_response(
+                            send_dict=send_property_value, received_dict=received_value
+                        )
+                        continue
+
+                    assert received_value == send_property_value, (
+                        f"Received value for {send_property_name} '{received_value}' does not "
+                        f"match '{send_property_value}' in the {response.request.method} request."
+                        f"\nSend: {_json.dumps(send_json, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+
+        if response.request.body is None:
+            logger.warning(
+                "Could not validate send response; the body of the request property "
+                "on the provided response was None."
+            )
+            return None
+        if isinstance(response.request.body, bytes):
+            send_json = _json.loads(response.request.body.decode("UTF-8"))
+        else:
+            send_json = _json.loads(response.request.body)
+
+        response_data = response.json()
+        # POST on /resource_type/{id}/array_item/ will return the updated {id} resource
+        # instead of a newly created resource. In this case, the send_json must be
+        # in the array of the 'array_item' property on {id}
+        send_path: str = response.request.path_url
+        response_path = response_data.get("href", None)
+        if response_path and send_path not in response_path:
+            property_to_check = send_path.replace(response_path, "")[1:]
+            if response_data.get(property_to_check) and isinstance(
+                response_data[property_to_check], list
+            ):
+                item_list: List[Dict[str, Any]] = response_data[property_to_check]
+                # Use the (mandatory) id to get the POSTed resource from the list
+                [response_data] = [
+                    item for item in item_list if item["id"] == send_json["id"]
+                ]
+
+        # incoming arguments are dictionaries, so they can be validated as such
+        validate_dict_response(send_dict=send_json, received_dict=response_data)
+
+        # In case of PATCH requests, ensure that only send properties have changed
+        if original_data:
+            for send_property_name, send_value in original_data.items():
+                if send_property_name not in send_json.keys():
+                    assert send_value == response_data[send_property_name], (
+                        f"Received value for {send_property_name} '{response_data[send_property_name]}' does not "
+                        f"match '{send_value}' in the pre-patch data"
+                        f"\nPre-patch: {_json.dumps(original_data, indent=4, sort_keys=True)}"
+                        f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
+                    )
+        return None
+
+    def _get_response_spec(
+        self, path: str, method: str, status_code: int
+    ) -> Dict[str, Any]:
+        method = method.lower()
+        status = str(status_code)
+        spec: Dict[str, Any] = {**self.openapi_spec}["paths"][path][method][
+            "responses"
+        ][status]
+        return spec
```

### Comparing `robotframework_openapitools-0.2.1/src/OpenApiLibCore/value_utils.py` & `robotframework_openapitools-0.2.2/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/auth.py` & `robotframework_openapitools-0.2.2/src/roboswag/auth.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/cli.py` & `robotframework_openapitools-0.2.2/src/roboswag/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/core.py` & `robotframework_openapitools-0.2.2/src/roboswag/core.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/generate.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/generate.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/api.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/api.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/definition.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/definition.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/endpoint.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/parameter.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/parameter.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/tag.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/tag.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/models/utils.py` & `robotframework_openapitools-0.2.2/src/roboswag/generate/models/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/templates/api_init.jinja` & `robotframework_openapitools-0.2.2/src/roboswag/generate/templates/api_init.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/generate/templates/paths.jinja` & `robotframework_openapitools-0.2.2/src/roboswag/generate/templates/paths.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/logger.py` & `robotframework_openapitools-0.2.2/src/roboswag/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/validate/schema.py` & `robotframework_openapitools-0.2.2/src/roboswag/validate/schema.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/src/roboswag/validate/text_response.py` & `robotframework_openapitools-0.2.2/src/roboswag/validate/text_response.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.2.1/PKG-INFO` & `robotframework_openapitools-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapitools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of Robot Framework libraries to test APIs for which the OAS is available.
 Home-page: https://github.com/MarketSquare/robotframework-openapitools
 License: Apache-2.0
 Author: Bartlomiej Hirsz
 Author-email: bartek.hirsz@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

