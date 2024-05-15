# Comparing `tmp/forbidden-11.0.tar.gz` & `tmp/forbidden-11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forbidden-11.0.tar", last modified: Mon May 13 09:53:47 2024, max compression
+gzip compressed data, was "forbidden-11.1.tar", last modified: Wed May 15 11:07:31 2024, max compression
```

## Comparing `forbidden-11.0.tar` & `forbidden-11.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/
--rwxrwx---   0 root         (0) root         (0)     1090 2024-05-12 22:47:27.000000 forbidden-11.0/LICENSE
--rwxrwx---   0 root         (0) root         (0)      112 2024-05-12 22:47:28.000000 forbidden-11.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17214 2024-05-13 09:53:47.328743 forbidden-11.0/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    16508 2024-05-13 09:48:33.000000 forbidden-11.0/README.md
--rwxrwx---   0 root         (0) root         (0)      895 2024-05-12 11:34:17.000000 forbidden-11.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:53:47.328743 forbidden-11.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/forbidden/
--rwxrwx---   0 root         (0) root         (0)        0 2024-05-12 11:33:12.000000 forbidden-11.0/src/forbidden/__init__.py
--rwxrwx---   0 root         (0) root         (0)    72494 2024-05-13 09:39:28.000000 forbidden-11.0/src/forbidden/forbidden.py
--rwxrwx---   0 root         (0) root         (0)    11174 2024-05-12 11:33:12.000000 forbidden-11.0/src/forbidden/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/forbidden.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17214 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/stresser/
--rwxrwx---   0 root         (0) root         (0)        0 2024-05-12 11:33:12.000000 forbidden-11.0/src/stresser/__init__.py
--rwxrwx---   0 root         (0) root         (0)    43173 2024-05-13 09:39:20.000000 forbidden-11.0/src/stresser/stresser.py
--rwxrwx---   0 root         (0) root         (0)    11174 2024-05-12 11:33:12.000000 forbidden-11.0/src/stresser/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:07:31.749257 forbidden-11.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 07:36:25.000000 forbidden-11.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-15 07:36:25.000000 forbidden-11.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17214 2024-05-15 11:07:31.749257 forbidden-11.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16508 2024-05-15 07:36:25.000000 forbidden-11.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      895 2024-05-15 11:07:13.000000 forbidden-11.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 11:07:31.749257 forbidden-11.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:07:31.745255 forbidden-11.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:07:31.745255 forbidden-11.1/src/forbidden/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 07:36:25.000000 forbidden-11.1/src/forbidden/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74384 2024-05-15 10:58:54.000000 forbidden-11.1/src/forbidden/forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    11174 2024-05-15 07:36:25.000000 forbidden-11.1/src/forbidden/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:07:31.749257 forbidden-11.1/src/forbidden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17214 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 11:07:31.000000 forbidden-11.1/src/forbidden.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:07:31.749257 forbidden-11.1/src/stresser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 07:36:25.000000 forbidden-11.1/src/stresser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44090 2024-05-15 11:05:54.000000 forbidden-11.1/src/stresser/stresser.py
+-rw-r--r--   0 root         (0) root         (0)    11174 2024-05-15 07:36:25.000000 forbidden-11.1/src/stresser/user_agents.txt
```

### Comparing `forbidden-11.0/PKG-INFO` & `forbidden-11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 11.0
+Version: 11.1
 Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `forbidden-11.0/README.md` & `forbidden-11.1/README.md`

 * *Files identical despite different names*

### Comparing `forbidden-11.0/pyproject.toml` & `forbidden-11.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "forbidden"
-version = "11.0"
+version = "11.1"
 authors = [{ name = "Ivan Sincek" }]
 description = "Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `forbidden-11.0/src/forbidden/forbidden.py` & `forbidden-11.1/src/forbidden/forbidden.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 			open(out, "w").write(data)
 			print(("Results have been saved to '{0}'").format(out))
 		except FileNotFoundError:
 			print(("Cannot save results to '{0}'").format(out))
 
 # ----------------------------------------
 
-default_user_agent = "Forbidden/11.0"
+default_user_agent = "Forbidden/11.1"
 
 def get_all_user_agents():
 	tmp = []
 	file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 	if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 		with open(file, "r", encoding = default_encoding) as stream:
 			for line in stream:
@@ -360,15 +360,15 @@
 		self.__sleep           = sleep
 		self.__user_agents     = user_agents
 		self.__user_agents_len = len(self.__user_agents)
 		self.__proxy           = proxy
 		self.__show_table      = show_table
 		self.__debug           = debug
 		# --------------------------------
-		# NOTE: PycURL configuration.
+		# NOTE: cURL configuration.
 		self.__curl            = not ignore_curl
 		self.__verify          = False # NOTE: Ignore SSL/TLS verification.
 		self.__allow_redirects = True
 		self.__max_redirects   = 10
 		self.__connect_timeout = request_timeout
 		self.__read_timeout    = request_timeout
 		self.__encoding        = "UTF-8" # NOTE: ISO-8859-1 works better than UTF-8 when accessing files.
@@ -392,67 +392,72 @@
 		query    = {}
 		fragment = {}
 		query["parsed"   ] = {} if ignore_qsf else urllib.parse.parse_qs(url.query, keep_blank_values = True)
 		query["full"     ] = ("?{0}").format(urllib.parse.urlencode(query["parsed"], doseq = True)) if query["parsed"] else ""
 		fragment["parsed"] = {} # NOTE: Not used.
 		fragment["full"  ] = ("#{0}").format(url.fragment) if url.fragment else ""
 		# --------------------------------
-		tmp                        = {}
-		tmp["scheme"             ] = scheme
-		tmp["domain_no_port"     ] = domain.split(":", 1)[0]
-		tmp["port"               ] = port
-		tmp["domain"             ] = domain
-		tmp["domain_extended"    ] = get_all_domains(tmp["scheme"], tmp["domain_no_port"], tmp["port"])
-		# --------------------------------
-		tmp["ip_no_port"         ] = None
-		tmp["ip"                 ] = None
-		tmp["ip_extended"        ] = None
-		tmp["scheme_ip"          ] = None
-		# --------------------------------
-		tmp["scheme_domain"      ] = ("{0}://{1}").format(tmp["scheme"], tmp["domain"])
-		tmp["path"               ] = path
-		tmp["query"              ] = query
-		tmp["fragment"           ] = fragment
-		tmp["path_full"          ] = tmp["path"] + tmp["query"]["full"] + tmp["fragment"]["full"]
+		tmp                          = {}
+		tmp["scheme"               ] = scheme
+		tmp["port"                 ] = port
+		# --------------------------------
+		tmp["domain_no_port"       ] = domain.split(":", 1)[0]
+		tmp["domain"               ] = domain
+		tmp["domain_extended"      ] = get_all_domains(tmp["scheme"], tmp["domain_no_port"], tmp["port"])
+		tmp["scheme_domain"        ] = ("{0}://{1}").format(tmp["scheme"], tmp["domain"])
+		tmp["scheme_domain_no_port"] = ("{0}://{1}").format(tmp["scheme"], tmp["domain_no_port"])
+		# --------------------------------
+		tmp["ip_no_port"           ] = None
+		tmp["ip"                   ] = None
+		tmp["ip_extended"          ] = None
+		tmp["scheme_ip"            ] = None
+		tmp["scheme_ip_no_port"    ] = None
+		# --------------------------------
+		tmp["path"                 ] = path
+		tmp["query"                ] = query
+		tmp["fragment"             ] = fragment
+		tmp["path_full"            ] = tmp["path"] + tmp["query"]["full"] + tmp["fragment"]["full"]
 		# --------------------------------
 		tmp["urls"               ] = {
 			"base"  : tmp["scheme_domain"] + tmp["path_full"],
 			"domain": {
 				"https": get_base_https_url(tmp["scheme"], tmp["domain_no_port"], tmp["port"], tmp["path_full"]),
 				"http" : get_base_http_url(tmp["scheme"], tmp["domain_no_port"], tmp["port"], tmp["path_full"])
 			},
 			"ip"    : {
 				"https": None,
 				"http" : None
 			}
 		}
 		# --------------------------------
 		tmp["relative_paths"     ] = extend_path(tmp["path"]) + extend_path(tmp["path"], tmp["query"]["full"], tmp["fragment"]["full"])
-		tmp["absolute_paths"     ] = append_paths(("{0}://{1}").format(tmp["scheme"], tmp["domain_no_port"]), tmp["relative_paths"]) + append_paths(tmp["scheme_domain"], tmp["relative_paths"])
+		tmp["absolute_paths"     ] = append_paths(tmp["scheme_domain_no_port"], tmp["relative_paths"]) + append_paths(tmp["scheme_domain"], tmp["relative_paths"])
 		# --------------------------------
 		for key in tmp:
 			if isinstance(tmp[key], list):
 				tmp[key] = unique(tmp[key])
 		return tmp
-		# --------------------------------
 
 	def __parse_ip(self, obj):
 		try:
-			obj["ip_no_port" ] = socket.gethostbyname(obj["domain_no_port"])
-			obj["ip"         ] = ("{0}:{1}").format(obj["ip_no_port"], obj["port"])
-			obj["ip_extended"] = get_all_domains(obj["scheme"], obj["ip_no_port"], obj["port"])
-			obj["scheme_ip"  ] = ("{0}://{1}").format(obj["scheme"], obj["ip"])
-			obj["urls"]["ip" ] = {
+			obj["ip_no_port"       ] = socket.gethostbyname(obj["domain_no_port"])
+			obj["ip"               ] = ("{0}:{1}").format(obj["ip_no_port"], obj["port"])
+			obj["ip_extended"      ] = get_all_domains(obj["scheme"], obj["ip_no_port"], obj["port"])
+			obj["scheme_ip"        ] = ("{0}://{1}").format(obj["scheme"], obj["ip"])
+			obj["scheme_ip_no_port"] = ("{0}://{1}").format(obj["scheme"], obj["ip_no_port"])
+			obj["urls"]["ip"       ] = {
 				"https": get_base_https_url(obj["scheme"], obj["ip_no_port"], obj["port"], obj["path_full"]),
 				"http" : get_base_http_url(obj["scheme"], obj["ip_no_port"], obj["port"], obj["path_full"])
 			}
 		except socket.error as ex:
 			self.__print_debug(ex)
 		return obj
 
+	# ------------------------------------
+
 	def __add_content_lengths(self, content_lengths):
 		if not isinstance(content_lengths, list):
 			content_lengths = [content_lengths]
 		self.__content_lengths = unique(self.__content_lengths + content_lengths)
 
 	def get_results(self):
 		return self.__collection
@@ -476,118 +481,119 @@
 
 	def __decode(self, values):
 		if isinstance(values, list):
 			return [value.decode(self.__encoding) for value in values]
 		else:
 			return values.decode(self.__encoding)
 
+	# ------------------------------------
+
 	def run(self):
 		self.__validate_inaccessible_and_evil_urls()
 		if not self.__error:
 			self.__fetch_inaccessible_and_evil_ips()
 			if not self.__error:
 				self.__validate_accessible_urls()
 				self.__set_allowed_http_methods()
 				self.__prepare_collection()
 				if not self.__collection:
 					print("No test records were created")
 				else:
-					self.__filter_collection()
+					self.__remove_duplicates()
 					print_cyan(("Number of created test records: {0}").format(len(self.__collection)))
 					self.__run_tests()
 					self.__validate_results()
 
 	def __validate_inaccessible_and_evil_urls(self):
-		# --------------------------------
 		print_cyan(("Normalized inaccessible URL: {0}").format(self.__url["urls"]["base"]))
 		print_time(("Validating the inaccessible URL using HTTP {0} method...").format(self.__force if self.__force else self.__default_method))
-		record = self.__fetch(url = self.__url["urls"]["base"], method = self.__force if self.__force else self.__default_method)
-		if not (record["code"] > 0):
+		record = self.__fetch(url = self.__url["urls"]["base"], method = self.__force if self.__force else self.__default_method, ignore = False)
+		if record["code"] <= 0:
 			self.__print_error("Cannot validate the inaccessible URL, script will exit shortly...")
 		elif "base" in self.__content_lengths:
 			print_green(("Ignoring the inaccessible URL response content length: {0}").format(record["length"]))
 			self.__content_lengths.pop(self.__content_lengths.index("base"))
 			self.__add_content_lengths(record["length"])
 		# --------------------------------
 		if not self.__error and self.__check_tests(["headers", "auths", "redirects", "parsers", "all"]):
 			print_cyan(("Normalized evil URL: {0}").format(self.__evil["urls"]["base"]))
 			print_time(("Validating the evil URL using HTTP {0} method...").format(self.__default_method))
 			record = self.__fetch(url = self.__evil["urls"]["base"], method = self.__default_method)
-			if not (record["code"] > 0):
+			if record["code"] == IGNORED:
+				self.__print_error("Evil URL is ignored, script will exit shortly...")
+			elif record["code"] <= 0:
 				self.__print_error("Cannot validate the evil URL, script will exit shortly...")
-		# --------------------------------
 
 	def __fetch_inaccessible_and_evil_ips(self):
-		# --------------------------------
 		print_time("Fetching the IP of inaccessible URL...")
 		self.__url = self.__parse_ip(copy.deepcopy(self.__url))
 		if not self.__url["ip_no_port"]:
 			self.__print_error("Cannot fetch the IP of inaccessible URL, script will exit shortly...")
 		# --------------------------------
 		if not self.__error and self.__check_tests(["headers", "auths", "redirects", "parsers", "all"]):
 			print_time("Fetching the IP of evil URL...")
 			self.__evil = self.__parse_ip(copy.deepcopy(self.__evil))
 			if not self.__evil["ip_no_port"]:
 				self.__print_error("Cannot fetch the IP of evil URL, script will exit shortly...")
-		# --------------------------------
 
 	# NOTE: Proceed with the first valid accessible URL.
 	def __validate_accessible_urls(self):
-		if self.__check_tests(["headers", "all"]):
+		if self.__check_tests(["headers", "all"]): # NOTE: Only tests that use the accessible URL.
 			print_time(("Validating the accessible URLs using HTTP {0} method...").format(self.__default_method))
 			for url in copy.deepcopy(self.__accessible):
 				self.__accessible = ""
 				record = self.__fetch(url = url, method = self.__default_method)
-				if record["code"] >= 200 and record["code"] < 400:
+				if record["code"] == IGNORED:
+					print_yellow(("Valid accessible URL ignored: {0}").format(record["url"]))
+				elif record["code"] >= 200 and record["code"] < 300:
 					print_green(("Valid accessible URL found: {0}").format(record["url"]))
 					self.__accessible = record["url"]
 					if "path" in self.__content_lengths:
 						print_green(("Ignoring the accessible URL response content length: {0}").format(record["length"]))
 						self.__content_lengths.pop(self.__content_lengths.index("path"))
 						self.__add_content_lengths(record["length"])
 					break
 			if not self.__accessible:
 				print_cyan("No valid accessible URLs were found, moving on...")
 
 	def __set_allowed_http_methods(self):
-		# --------------------------------
 		if self.__force:
 			print_cyan(("Forcing HTTP {0} method for all non-specific test cases...").format(self.__force))
 			self.__allowed_methods = [self.__force]
-		# --------------------------------
-		elif self.__check_tests(["methods", "method-overrides", "all"]):
+		elif self.__check_tests(["methods", "method-overrides", "all"]): # NOTE: Only tests that use multiple HTTP methods.
 			print_time("Fetching allowed HTTP methods...")
-			record = self.__fetch(url = self.__url["urls"]["base"], method = "OPTIONS")
+			record = self.__fetch(url = self.__url["urls"]["base"], method = "OPTIONS", ignore = False, response_headers = True)
 			if record["code"] > 0:
 				if record["curl"]:
-					methods = re.search(r"(?<=^allow\:).+", record["response_headers"], self.__regex_flags)
+					methods = re.search(r"(?<=^allow\:).+", record["response_headers"], self.__regex_flags) # NOTE: HTTP response headers are returned in plaintext.
 					if methods:
 						for method in methods[0].split(","):
 							method = method.strip().upper()
 							if method not in self.__allowed_methods:
 								self.__allowed_methods.append(method)
 				else:
-					for key in record["response_headers"]:
+					for key in record["response_headers"]: # NOTE: HTTP response headers are returned as dictionary.
 						if key.lower() == "allow":
 							for method in record["response_headers"][key].split(","):
 								method = method.strip().upper()
 								if method not in self.__allowed_methods:
 									self.__allowed_methods.append(method)
 							break
 			if not self.__allowed_methods:
-				print_cyan("Cannot fetch allowed HTTP methods, moving on...")
+				print_cyan("Cannot fetch allowed HTTP methods, using all built-in HTTP methods...")
 				self.__allowed_methods = self.__get_methods()
-				# TO DO: Brute-force allowed HTTP methods.
+				# TO DO: Validate (brute-force) all built-in HTTP methods.
 			else:
 				print_green(("Allowed HTTP methods: [{0}]").format((", ").join(self.__allowed_methods)))
-		# --------------------------------
 
-	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
+	# ------------------------------------
+
+	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, ignore = True, response_headers = False, response_body = False):
 		record = self.__record("SYSTEM-0", url, method, headers, cookies, body, user_agent, proxy, curl)
-		return self.__send_curl(record, passthrough) if record["curl"] else self.__send_request(record, passthrough)
+		return self.__send_curl(record, ignore, response_headers, response_body) if record["curl"] else self.__send_request(record, ignore, response_headers, response_body)
 
 	def __records(self, identifier, urls, methods = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None):
 		if not isinstance(urls, list):
 			urls = [urls]
 		if not isinstance(methods, list):
 			methods = [methods]
 		if headers:
@@ -607,15 +613,15 @@
 		self.__identifier += 1
 		identifier = ("{0}-{1}").format(self.__identifier, identifier)
 		if not method:
 			method = self.__force if self.__force else self.__default_method
 		headers = self.__inspect_headers(headers)
 		cookies = self.__inspect_cookies(cookies)
 		if not user_agent:
-			user_agent = self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
+			user_agent = self.__get_user_agent()
 		if not proxy:
 			proxy = self.__proxy
 		if not curl and curl is not False:
 			curl = self.__curl
 		record = {
 			"raw"             : self.__identifier,
 			"id"              : identifier,
@@ -662,14 +668,17 @@
 					tmp.append(format_cookie_key_value(key, value))
 		for cookie in self.__cookies:
 			key, value = get_cookie_key_value(cookie)
 			if key and key.lower() not in exists: # NOTE: Extra HTTP cookies cannot override test HTTP cookies.
 				tmp.append(format_cookie_key_value(key, value))
 		return tmp
 
+	def __get_user_agent(self):
+		return self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
+
 	def __build_command(self, record):
 		tmp = ["curl", ("--connect-timeout {0}").format(self.__connect_timeout), ("-m {0}").format(self.__read_timeout), "-iskL", ("--max-redirs {0}").format(self.__max_redirects), "--path-as-is"]
 		if record["body"]:
 			tmp.append(set_param(record["body"], "-d"))
 		if record["proxy"]:
 			tmp.append(set_param(record["proxy"], "-x"))
 		if record["user_agent"]:
@@ -680,16 +689,17 @@
 		if record["cookies"]:
 			tmp.append(set_param(("; ").join(record["cookies"]), "-b"))
 		tmp.append(set_param(record["method"], "-X"))
 		tmp.append(set_param(record["url"]))
 		tmp = (" ").join(tmp)
 		return tmp
 
-	# NOTE: Remove duplicate test records.
-	def __filter_collection(self):
+	# ------------------------------------
+
+	def __remove_duplicates(self):
 		tmp = []
 		exists = set()
 		for record in self.__collection:
 			command = re.sub((" -A \\{0}.+?\\{0} ").format(default_quotes), " ", record["command"])
 			if command not in exists and not exists.add(command):
 				tmp.append(record)
 		self.__collection = tmp
@@ -708,15 +718,17 @@
 				for subprocess in concurrent.futures.as_completed(subprocesses):
 					results.append(subprocess.result())
 					progress.show()
 			except KeyboardInterrupt:
 				executor.shutdown(wait = True, cancel_futures = True)
 		self.__collection = results
 
-	def __send_curl(self, record, passthrough = False):
+	# ------------------------------------
+
+	def __send_curl(self, record, ignore = True, response_headers = False, response_body = False):
 		if self.__sleep:
 			time.sleep(self.__sleep)
 		curl = None
 		cookiefile = None
 		headers = None
 		response = None
 		try:
@@ -724,15 +736,15 @@
 			curl = pycurl.Curl()
 			# ----------------------------
 			cookiefile = tempfile.NamedTemporaryFile(mode = "r") # NOTE: Important! Store and pass HTTP cookies on HTTP redirects.
 			curl.setopt(pycurl.COOKIESESSION, True)
 			curl.setopt(pycurl.COOKIEFILE, cookiefile.name)
 			curl.setopt(pycurl.COOKIEJAR, cookiefile.name)
 			# ----------------------------
-			if passthrough:
+			if response_headers:
 				headers = io.BytesIO()
 				curl.setopt(pycurl.HEADERFUNCTION, headers.write)
 			# ----------------------------
 			response = io.BytesIO()
 			curl.setopt(pycurl.WRITEFUNCTION, response.write)
 			# ----------------------------
 			curl.setopt(pycurl.HTTP_VERSION, pycurl.CURL_HTTP_VERSION_1_1)
@@ -763,19 +775,22 @@
 			if record["proxy"]:
 				curl.setopt(pycurl.PROXY, record["proxy"])
 			# ----------------------------
 			curl.perform()
 			# ----------------------------
 			record["code"] = int(curl.getinfo(pycurl.RESPONSE_CODE))
 			record["length"] = int(curl.getinfo(pycurl.SIZE_DOWNLOAD))
-			if passthrough:
+			record["response"] = self.__decode(response.getvalue())
+			if response_headers:
 				record["response_headers"] = self.__decode(headers.getvalue())
-				# record["response"] = self.__decode(response.getvalue())
-			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(response.getvalue()), self.__regex_flags)):
-				record["code"] = IGNORED
+			if ignore:
+				if record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, record["response"], self.__regex_flags)):
+					record["code"] = IGNORED
+			if not response_body:
+				record["response"] = ""
 			# ----------------------------
 		except pycurl.error as ex:
 			# ----------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -789,15 +804,15 @@
 				curl.close()
 			# ----------------------------
 			if cookiefile:
 				cookiefile.close() # NOTE: Important! Close the file handle strictly after closing the cURL handle.
 			# ----------------------------
 		return record
 
-	def __send_request(self, record, passthrough = False):
+	def __send_request(self, record, ignore = True, response_headers = False, response_body = False):
 		if self.__sleep:
 			time.sleep(self.__sleep)
 		session = None
 		response = None
 		try:
 			# ----------------------------
 			session = requests.Session()
@@ -828,19 +843,22 @@
 				verify = self.__verify,
 				allow_redirects = self.__allow_redirects,
 				timeout = (self.__connect_timeout, self.__read_timeout)
 			)
 			# ----------------------------
 			record["code"] = int(response.status_code)
 			record["length"] = len(response.content)
-			if passthrough:
+			record["response"] = self.__decode(response.content)
+			if response_headers:
 				record["response_headers"] = dict(response.headers)
-				# record["response"] = self.__decode(response.content)
-			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(response.content), self.__regex_flags)):
-				record["code"] = IGNORED
+			if ignore:
+				if record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, record["response"], self.__regex_flags)):
+					record["code"] = IGNORED
+			if not response_body:
+				record["response"] = ""
 			# ----------------------------
 		except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException) as ex:
 			# ----------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -852,22 +870,26 @@
 			# ----------------------------
 		return record
 
 	def __set_double_headers(self, request, headers):
 		exists = set()
 		for header in headers:
 			key, value = get_header_key_value(header)
-			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value) # NOTE: Allows double headers.
+			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value)
+
+	# ------------------------------------
 
 	def __validate_results(self):
 		print_time("Validating results...")
 		output = Output(self.__collection)
 		self.__collection = output.results_table() if self.__show_table else output.results_json()
 		output.stats_table()
 
+	# ------------------------------------
+
 	def __check_tests(self, array):
 		return any(test in array for test in self.__tests)
 
 	def __prepare_collection(self):
 		print_time("Preparing test records...")
 		# --------------------------------
 		if self.__check_tests(["base", "all"]):
@@ -1064,16 +1086,18 @@
 			# NOTE: Test broken URL parsers, OOB, and SSRF.
 			self.__records(
 				identifier = "PARSERS-2",
 				urls       = self.__url["urls"]["base"],
 				headers    = self.__get_ip_headers(self.__get_broken_urls(scheme = False, ip = False) + self.__get_broken_urls(scheme = False, ip = True))
 			)
 
+	# ------------------------------------
+
 	def __get_methods(self):
-		tmp = [
+		return unique([
 			"ACL",
 			"ARBITRARY",
 			"BASELINE-CONTROL",
 			"BIND",
 			"CHECKIN",
 			"CHECKOUT",
 			"CONNECT",
@@ -1111,16 +1135,15 @@
 			"UNBIND",
 			"UNCHECKOUT",
 			"UNLINK",
 			"UNLOCK",
 			"UPDATE",
 			"UPDATEREDIRECTREF",
 			"VERSION-CONTROL"
-		]
-		return unique(tmp)
+		])
 
 	def __get_file_upload_urls(self, files):
 		tmp = []
 		scheme_domain_paths = append_paths(self.__url["scheme_domain"], get_recursive_paths(self.__url["path"]))
 		scheme_domain_path_files = append_paths(scheme_domain_paths, files)
 		for scheme_domain_path_file in scheme_domain_path_files:
 			tmp.append(scheme_domain_path_file + self.__url["query"]["full"] + self.__url["fragment"]["full"])
@@ -1193,15 +1216,14 @@
 		for header in headers:
 			for port in [self.__url["port"], 80, 443, 4443, 8008, 8080, 8403, 8443, 9008, 9080, 9403, 9443]:
 				tmp.append(("{0}: {1}").format(header, port))
 		return unique(tmp)
 
 	def __get_url_headers(self, values):
 		tmp = []
-		# --------------------------------
 		headers = [
 			"19-Profile",
 			"Base-URL",
 			"Destination",
 			"Origin",
 			"Profile",
 			"Proxy",
@@ -1218,15 +1240,14 @@
 			"X-Referer",
 			"X-Rewrite-URL",
 			"X-Wap-Profile"
 		]
 		for header in headers:
 			for value in values:
 				tmp.append(("{0}: {1}").format(header, value))
-		# --------------------------------
 		return unique(tmp)
 
 	def __get_ip_headers(self, values):
 		tmp = []
 		# --------------------------------
 		headers = [
 			"CF-Connecting-IP",
@@ -1327,63 +1348,75 @@
 		return get_all_domains(self.__url["scheme"], ["localhost", "127.0.0.1", unicode_encode("127.0.0.1"), "127.000.000.001"], self.__url["port"])
 
 	def __get_random_values(self):
 		return get_all_domains(self.__url["scheme"], ["192.168.1.1", "172.16.1.1", "173.245.48.1", "10.1.1.1", "169.254.169.254"], self.__url["port"])
 
 	def __get_all_values(self, scheme = True, ip = False):
 		tmp = []
+		# --------------------------------
 		domain_extended = "ip_extended" if ip else "domain_extended"
-		localhost = "127.0.0.1" if ip else "localhost"
+		localhost       = "127.0.0.1"   if ip else "localhost"
+		# --------------------------------
 		temp = strip_url_schemes(self.__get_localhost_values() + self.__get_random_values() + self.__url[domain_extended])
 		if scheme:
 			tmp.extend([("{0}://{1}").format(self.__url["scheme"], entry + self.__url["path_full"]) for entry in temp])
 		else:
 			tmp += temp
+		# --------------------------------
 		temp = strip_url_schemes(self.__evil[domain_extended])
 		if scheme:
 			tmp.extend([("{0}://{1}").format(self.__evil["scheme"], entry + self.__url["path_full"]) for entry in temp])
 		else:
 			tmp += temp
+		# --------------------------------
 		if not scheme:
 			for override in strip_url_schemes(self.__url[domain_extended] + self.__evil[domain_extended]):
 				for initial in strip_url_schemes([localhost, ("{0}:{1}").format(localhost, self.__url["port"])]):
 					tmp.append(("{0},{1}").format(initial, override))
+		# --------------------------------
 		return unique(tmp)
 
 	def __get_double_host_header(self, ip = False):
 		tmp = []
+		# --------------------------------
 		domain_extended = "ip_extended" if ip else "domain_extended"
+		# --------------------------------
 		exists = set()
 		for override in strip_url_schemes(self.__evil[domain_extended]):
 			for initial in strip_url_schemes(self.__url[domain_extended]):
 				exist = initial + override
 				if exist not in exists and not exists.add(exist):
 					tmp.append([
 						("Host: {0}").format(initial),
 						("Host: {0}").format(override)
 					])
+		# --------------------------------
 		return tmp
 
 	def __get_path_bypass_urls(self, sniper = False):
 		path_bypasses = []
 		# --------------------------------
 		path = self.__url["path"].strip(path_const)
 		# --------------------------------
 		# NOTE: Inject at the beginning, end, and both, beginning and end of the URL path.
 		# NOTE: Use one payload set to test all positions simultaneously (sniper) or test using every possible combination of payload set (cluster bomb - default).
 		injections = []
 		for i in ["", "%09", "%20", "%23", "%2e", "%a0", "*", ".", "..", ";", ".;", "..;", "/;/", ";/../../", ";foo=bar;"]:
 			injections.extend([path_const + i + path_const, i + path_const, path_const + i, i])
 		if sniper:
 			for i in injections:
-				path_bypasses.extend([path + i, i + path, i + path + i])
+				path_bypasses.extend([path + i, i + path])
+				if path:
+					path_bypasses.extend([i + path + i])
 		else:
 			for i in injections:
-				for j in injections:
-					path_bypasses.extend([i + path + j])
+				path_bypasses.extend([path + i, i + path])
+				if path:
+					for j in injections:
+						path_bypasses.extend([i + path + j])
 		# --------------------------------
 		# NOTE: Inject at the end of the URL path.
 		injections = []
 		for i in ["#", "*", ".", "?", "~"]:
 			injections.extend([i, i + i, ("{0}random").format(i)])
 		paths = [path, path + path_const]
 		for p in paths:
@@ -1416,15 +1449,15 @@
 		return unique(tmp)
 
 	def __get_basic_auth_headers(self):
 		tmp = []
 		headers = [
 			"Authorization"
 		]
-		values = ["", "null", "None", "nil"]
+		values    = ["", "null", "None", "nil"]
 		usernames = ["admin", "cisco", "gateway", "guest", "jigsaw", "root", "router", "switch", "tomcat", "wampp", "xampp", "sysadmin"]
 		passwords = ["admin", "cisco", "default", "gateway", "guest", "jigsaw", "password", "root", "router", "secret", "switch", "tomcat", "toor", "wampp", "xampp", "sysadmin"]
 		for username in usernames:
 			for password in passwords:
 				values.append(b64(("{0}:{1}").format(username, password)))
 		for header in headers:
 			for value in values:
@@ -1452,38 +1485,45 @@
 		for header in headers:
 			for value in values:
 				tmp.append(("{0}: Bearer {1}").format(header, value))
 		return unique(tmp)
 
 	def __get_redirect_urls(self, scheme = True, ip = False):
 		tmp = []
+		# --------------------------------
 		domain_extended = "ip_extended" if ip else "domain_extended"
-		domain_no_port = "ip_no_port" if ip else "domain_no_port"
+		domain_no_port  = "ip_no_port"  if ip else "domain_no_port"
+		# --------------------------------
 		injections = [path_const, ("{0}.").format(path_const)]
 		for override in strip_url_schemes(self.__evil[domain_extended]):
 			tmp.append(override)
 			for injection in injections:
 				tmp.append(override + injection + self.__url[domain_no_port])
 			if not ip:
 				tmp.append(("{0}.{1}").format(self.__url[domain_no_port], override))
+		# --------------------------------
 		if scheme:
 			tmp = [("{0}://{1}").format(self.__evil["scheme"], entry + self.__url["path_full"]) for entry in tmp]
+		# --------------------------------
 		return unique(tmp)
 
 	def __get_broken_urls(self, scheme = True, ip = False):
 		tmp = []
+		# --------------------------------
 		domain_extended = "ip_extended" if ip else "domain_extended"
-		at_const = "@"
-		injections = [at_const, (" {0}").format(at_const), ("#{0}").format(at_const)]
+		# --------------------------------
+		injections = ["@", " @", "#@"]
 		for override in strip_url_schemes(self.__evil[domain_extended]):
 			for initial in strip_url_schemes(self.__url[domain_extended]):
 				for injection in injections:
 					tmp.append(initial + injection + override)
+		# --------------------------------
 		if scheme:
 			tmp = [("{0}://{1}").format(self.__evil["scheme"], entry + self.__url["path_full"]) for entry in tmp]
+		# --------------------------------
 		return unique(tmp)
 
 # ----------------------------------------
 
 class Output:
 
 	def __init__(self, collection):
@@ -1492,15 +1532,15 @@
 
 	def __color(self, value, color):
 		return ("{0}{1}{2}").format(color, value, colorama.Style.RESET_ALL)
 
 	def __results_row(self, record, color):
 		return [self.__color(record[key], color) for key in ["id", "code", "length", "command"]]
 
-	def results_table(self):
+	def results_table(self): # NOTE: To see more or less results, comment in or out 'continue' line.
 		tmp = []; table = []
 		for record in self.__collection:
 			if record["code"] < 100 or record["code"] >= 600:
 				continue
 			elif record["code"] >= 500:
 				continue
 				table.append(self.__results_row(record, colorama.Fore.CYAN))
@@ -1592,15 +1632,15 @@
 			self.__count += 1
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("Forbidden v11.0 ( github.com/ivan-sincek/forbidden )")
+		print("Forbidden v11.1 ( github.com/ivan-sincek/forbidden )")
 		print("")
 		print("Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path ] [-o out         ]")
 		print("Example: forbidden -u https://example.com/admin -t all   [-f POST ] [-v values.txt] [-p /home] [-o results.json]")
 		print("")
 		print("DESCRIPTION")
 		print("    Bypass 4xx HTTP response status codes and more")
 		print("URL")
@@ -1747,46 +1787,46 @@
 
 	def __print_error(self, msg):
 		print(("ERROR: {0}").format(msg))
 
 	def __parse_url(self, value, key):
 		data = {
 			"url": {
-				"schemes": ["http", "https"],
-				"scheme_error": [
-					"Inaccessible URL: Scheme is required",
-					"Inaccessible URL: Supported schemes are 'http' and 'https'"
-				],
+				"schemes"     : ["http", "https"],
+				"scheme_error": {
+					"required"   : "Inaccessible URL: Scheme is required",
+					"unsupported": "Inaccessible URL: Supported schemes are 'http' and 'https'"
+				},
 				"domain_error": "Inaccessible URL: Invalid domain name",
-				"port_error": "Inaccessible URL: Port number is out of range"
+				"port_error"  : "Inaccessible URL: Port number is out of range"
 			},
 			"evil": {
-				"schemes": ["http", "https"],
-				"scheme_error": [
-					"Evil URL: Scheme is required",
-					"Evil URL: Supported schemes are 'http' and 'https'"
-				],
+				"schemes"     : ["http", "https"],
+				"scheme_error": {
+					"required"   : "Evil URL: Scheme is required",
+					"unsupported": "Evil URL: Supported schemes are 'http' and 'https'"
+				},
 				"domain_error": "Evil URL: Invalid domain name",
-				"port_error": "Evil URL: Port number is out of range"
+				"port_error"  : "Evil URL: Port number is out of range"
 			},
 			"proxy": {
-				"schemes": ["http", "https", "socks4", "socks4h", "socks5", "socks5h"],
-				"scheme_error": [
-					"Proxy URL: Scheme is required",
-					"Proxy URL: Supported schemes are 'http[s]', 'socks4[h]', and 'socks5[h]'"
-				],
+				"schemes"     : ["http", "https", "socks4", "socks4h", "socks5", "socks5h"],
+				"scheme_error": {
+					"required"   : "Proxy URL: Scheme is required",
+					"unsupported": "Proxy URL: Supported schemes are 'http[s]', 'socks4[h]', and 'socks5[h]'"
+				},
 				"domain_error": "Proxy URL: Invalid domain name",
-				"port_error": "Proxy URL: Port number is out of range"
+				"port_error"  : "Proxy URL: Port number is out of range"
 			}
 		}
 		tmp = urllib.parse.urlsplit(value)
 		if not tmp.scheme:
-			self.__error(data[key]["scheme_error"][0])
+			self.__error(data[key]["scheme_error"]["required"])
 		elif tmp.scheme not in data[key]["schemes"]:
-			self.__error(data[key]["scheme_error"][1])
+			self.__error(data[key]["scheme_error"]["unsupported"])
 		elif not tmp.netloc:
 			self.__error(data[key]["domain_error"])
 		elif tmp.port and (tmp.port < 1 or tmp.port > 65535):
 			self.__error(data[key]["port_error"])
 		return value
 
 	def __parse_tests(self, value):
@@ -1905,15 +1945,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                             Forbidden v11.0                             #")
+		print("#                             Forbidden v11.1                             #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Bypass 4xx HTTP response status codes and more.                         #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                  #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `forbidden-11.0/src/forbidden/user_agents.txt` & `forbidden-11.1/src/forbidden/user_agents.txt`

 * *Files identical despite different names*

### Comparing `forbidden-11.0/src/forbidden.egg-info/PKG-INFO` & `forbidden-11.1/src/forbidden.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 11.0
+Version: 11.1
 Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `forbidden-11.0/src/stresser/stresser.py` & `forbidden-11.1/src/stresser/stresser.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 			open(out, "w").write(data)
 			print(("Results have been saved to '{0}'").format(out))
 		except FileNotFoundError:
 			print(("Cannot save results to '{0}'").format(out))
 
 # ----------------------------------------
 
-default_user_agent = "Stresser/11.0"
+default_user_agent = "Stresser/11.1"
 
 def get_all_user_agents():
 	tmp = []
 	file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 	if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 		with open(file, "r", encoding = default_encoding) as stream:
 			for line in stream:
@@ -225,15 +225,15 @@
 		self.__user_agents     = user_agents
 		self.__user_agents_len = len(self.__user_agents)
 		self.__proxy           = proxy
 		self.__show_table      = show_table
 		self.__directory       = directory
 		self.__debug           = debug
 		# --------------------------------
-		# NOTE: PycURL configuration.
+		# NOTE: cURL configuration.
 		self.__curl            = not ignore_curl
 		self.__verify          = False # NOTE: Ignore SSL/TLS verification.
 		self.__allow_redirects = True
 		self.__max_redirects   = 10
 		self.__connect_timeout = request_timeout
 		self.__read_timeout    = request_timeout
 		self.__encoding        = "UTF-8" # NOTE: ISO-8859-1 works better than UTF-8 when accessing files.
@@ -257,67 +257,72 @@
 		query    = {}
 		fragment = {}
 		query["parsed"   ] = {} if ignore_qsf else urllib.parse.parse_qs(url.query, keep_blank_values = True)
 		query["full"     ] = ("?{0}").format(urllib.parse.urlencode(query["parsed"], doseq = True)) if query["parsed"] else ""
 		fragment["parsed"] = {} # NOTE: Not used.
 		fragment["full"  ] = ("#{0}").format(url.fragment) if url.fragment else ""
 		# --------------------------------
-		tmp                        = {}
-		tmp["scheme"             ] = scheme
-		tmp["domain_no_port"     ] = domain.split(":", 1)[0]
-		tmp["port"               ] = port
-		tmp["domain"             ] = domain
-		tmp["domain_extended"    ] = get_all_domains(tmp["scheme"], tmp["domain_no_port"], tmp["port"])
-		# --------------------------------
-		tmp["ip_no_port"         ] = None
-		tmp["ip"                 ] = None
-		tmp["ip_extended"        ] = None
-		tmp["scheme_ip"          ] = None
-		# --------------------------------
-		tmp["scheme_domain"      ] = ("{0}://{1}").format(tmp["scheme"], tmp["domain"])
-		tmp["path"               ] = path
-		tmp["query"              ] = query
-		tmp["fragment"           ] = fragment
-		tmp["path_full"          ] = tmp["path"] + tmp["query"]["full"] + tmp["fragment"]["full"]
+		tmp                          = {}
+		tmp["scheme"               ] = scheme
+		tmp["port"                 ] = port
+		# --------------------------------
+		tmp["domain_no_port"       ] = domain.split(":", 1)[0]
+		tmp["domain"               ] = domain
+		tmp["domain_extended"      ] = get_all_domains(tmp["scheme"], tmp["domain_no_port"], tmp["port"])
+		tmp["scheme_domain"        ] = ("{0}://{1}").format(tmp["scheme"], tmp["domain"])
+		tmp["scheme_domain_no_port"] = ("{0}://{1}").format(tmp["scheme"], tmp["domain_no_port"])
+		# --------------------------------
+		tmp["ip_no_port"           ] = None
+		tmp["ip"                   ] = None
+		tmp["ip_extended"          ] = None
+		tmp["scheme_ip"            ] = None
+		tmp["scheme_ip_no_port"    ] = None
+		# --------------------------------
+		tmp["path"                 ] = path
+		tmp["query"                ] = query
+		tmp["fragment"             ] = fragment
+		tmp["path_full"            ] = tmp["path"] + tmp["query"]["full"] + tmp["fragment"]["full"]
 		# --------------------------------
 		tmp["urls"               ] = {
 			"base"  : tmp["scheme_domain"] + tmp["path_full"],
 			"domain": {
 				"https": get_base_https_url(tmp["scheme"], tmp["domain_no_port"], tmp["port"], tmp["path_full"]),
 				"http" : get_base_http_url(tmp["scheme"], tmp["domain_no_port"], tmp["port"], tmp["path_full"])
 			},
 			"ip"    : {
 				"https": None,
 				"http" : None
 			}
 		}
 		# --------------------------------
 		tmp["relative_paths"     ] = extend_path(tmp["path"]) + extend_path(tmp["path"], tmp["query"]["full"], tmp["fragment"]["full"])
-		tmp["absolute_paths"     ] = append_paths(("{0}://{1}").format(tmp["scheme"], tmp["domain_no_port"]), tmp["relative_paths"]) + append_paths(tmp["scheme_domain"], tmp["relative_paths"])
+		tmp["absolute_paths"     ] = append_paths(tmp["scheme_domain_no_port"], tmp["relative_paths"]) + append_paths(tmp["scheme_domain"], tmp["relative_paths"])
 		# --------------------------------
 		for key in tmp:
 			if isinstance(tmp[key], list):
 				tmp[key] = unique(tmp[key])
 		return tmp
-		# --------------------------------
 
 	def __parse_ip(self, obj):
 		try:
-			obj["ip_no_port" ] = socket.gethostbyname(obj["domain_no_port"])
-			obj["ip"         ] = ("{0}:{1}").format(obj["ip_no_port"], obj["port"])
-			obj["ip_extended"] = get_all_domains(obj["scheme"], obj["ip_no_port"], obj["port"])
-			obj["scheme_ip"  ] = ("{0}://{1}").format(obj["scheme"], obj["ip"])
-			obj["urls"]["ip" ] = {
+			obj["ip_no_port"       ] = socket.gethostbyname(obj["domain_no_port"])
+			obj["ip"               ] = ("{0}:{1}").format(obj["ip_no_port"], obj["port"])
+			obj["ip_extended"      ] = get_all_domains(obj["scheme"], obj["ip_no_port"], obj["port"])
+			obj["scheme_ip"        ] = ("{0}://{1}").format(obj["scheme"], obj["ip"])
+			obj["scheme_ip_no_port"] = ("{0}://{1}").format(obj["scheme"], obj["ip_no_port"])
+			obj["urls"]["ip"       ] = {
 				"https": get_base_https_url(obj["scheme"], obj["ip_no_port"], obj["port"], obj["path_full"]),
 				"http" : get_base_http_url(obj["scheme"], obj["ip_no_port"], obj["port"], obj["path_full"])
 			}
 		except socket.error as ex:
 			self.__print_debug(ex)
 		return obj
 
+	# ------------------------------------
+
 	def __add_content_lengths(self, content_lengths):
 		if not isinstance(content_lengths, list):
 			content_lengths = [content_lengths]
 		self.__content_lengths = unique(self.__content_lengths + content_lengths)
 
 	def get_results(self):
 		return self.__collection
@@ -341,14 +346,16 @@
 
 	def __decode(self, values):
 		if isinstance(values, list):
 			return [value.decode(self.__encoding) for value in values]
 		else:
 			return values.decode(self.__encoding)
 
+	# ------------------------------------
+
 	def run(self):
 		self.__validate_inaccessible_url()
 		if not self.__error:
 			self.__fetch_inaccessible_ip()
 			if not self.__error:
 				self.__set_allowed_http_methods()
 				self.__prepare_collection()
@@ -356,70 +363,64 @@
 					print("No test records were created")
 				else:
 					print_cyan(("Number of created test records: {0}").format(len(self.__collection)))
 					self.__run_tests()
 					self.__validate_results()
 
 	def __validate_inaccessible_url(self):
-		# --------------------------------
 		print_cyan(("Normalized inaccessible URL: {0}").format(self.__url["urls"]["base"]))
 		print_time(("Validating the inaccessible URL using HTTP {0} method...").format(self.__force if self.__force else self.__default_method))
-		record = self.__fetch(url = self.__url["urls"]["base"], method = self.__force if self.__force else self.__default_method)
-		if not (record["code"] > 0):
+		record = self.__fetch(url = self.__url["urls"]["base"], method = self.__force if self.__force else self.__default_method, ignore = False)
+		if record["code"] <= 0:
 			self.__print_error("Cannot validate the inaccessible URL, script will exit shortly...")
 		elif "base" in self.__content_lengths:
 			print_green(("Ignoring the inaccessible URL response content length: {0}").format(record["length"]))
 			self.__content_lengths.pop(self.__content_lengths.index("base"))
 			self.__add_content_lengths(record["length"])
-		# --------------------------------
 
 	def __fetch_inaccessible_ip(self):
-		# --------------------------------
 		print_time("Fetching the IP of inaccessible URL...")
 		self.__url = self.__parse_ip(copy.deepcopy(self.__url))
 		if not self.__url["ip_no_port"]:
 			self.__print_error("Cannot fetch the IP of inaccessible URL, script will exit shortly...")
-		# --------------------------------
 
 	def __set_allowed_http_methods(self):
-		# --------------------------------
 		if self.__force:
 			print_cyan(("Forcing HTTP {0} method for all non-specific test cases...").format(self.__force))
 			self.__allowed_methods = [self.__force]
-		# --------------------------------
 		else:
 			print_time("Fetching allowed HTTP methods...")
-			record = self.__fetch(url = self.__url["urls"]["base"], method = "OPTIONS")
+			record = self.__fetch(url = self.__url["urls"]["base"], method = "OPTIONS", ignore = False, response_headers = True)
 			if record["code"] > 0:
 				if record["curl"]:
-					methods = re.search(r"(?<=^allow\:).+", record["response_headers"], self.__regex_flags)
+					methods = re.search(r"(?<=^allow\:).+", record["response_headers"], self.__regex_flags) # NOTE: HTTP response headers are returned in plaintext.
 					if methods:
 						for method in methods[0].split(","):
 							method = method.strip().upper()
 							if method not in self.__allowed_methods:
 								self.__allowed_methods.append(method)
 				else:
-					for key in record["response_headers"]:
+					for key in record["response_headers"]: # NOTE: HTTP response headers are returned as dictionary.
 						if key.lower() == "allow":
 							for method in record["response_headers"][key].split(","):
 								method = method.strip().upper()
 								if method not in self.__allowed_methods:
 									self.__allowed_methods.append(method)
 							break
 			if not self.__allowed_methods:
-				print_cyan(("Cannot fetch allowed HTTP methods, defaulting to HTTP {0} method for all non-specific test cases...").format(self.__default_method))
+				print_cyan(("Cannot fetch allowed HTTP methods, using default HTTP {0} method...").format(self.__default_method))
 				self.__allowed_methods = [self.__default_method]
-				# TO DO: Brute-force allowed HTTP methods.
 			else:
 				print_green(("Allowed HTTP methods: [{0}]").format((", ").join(self.__allowed_methods)))
-		# --------------------------------
 
-	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
+	# ------------------------------------
+
+	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, ignore = True, response_headers = False, response_body = False, save = False):
 		record = self.__record("SYSTEM-0", url, method, headers, cookies, body, user_agent, proxy, curl)
-		return self.__send_curl(record, passthrough) if record["curl"] else self.__send_request(record, passthrough)
+		return self.__send_curl(record, ignore, response_headers, response_body, save) if record["curl"] else self.__send_request(record, ignore, response_headers, response_body, save)
 
 	def __records(self, identifier, urls, methods = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, repeat = None):
 		if not isinstance(urls, list):
 			urls = [urls]
 		if not isinstance(methods, list):
 			methods = [methods]
 		if not repeat:
@@ -443,15 +444,15 @@
 		self.__identifier += 1
 		# identifier = ("{0}-{1}").format(self.__identifier, identifier)
 		if not method:
 			method = self.__force if self.__force else self.__default_method
 		headers = self.__inspect_headers(headers)
 		cookies = self.__inspect_cookies(cookies)
 		if not user_agent:
-			user_agent = self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
+			user_agent = self.__get_user_agent()
 		if not proxy:
 			proxy = self.__proxy
 		if not curl and curl is not False:
 			curl = self.__curl
 		record = {
 			"raw"             : self.__identifier,
 			"id"              : identifier,
@@ -498,14 +499,17 @@
 					tmp.append(format_cookie_key_value(key, value))
 		for cookie in self.__cookies:
 			key, value = get_cookie_key_value(cookie)
 			if key and key.lower() not in exists: # NOTE: Extra HTTP cookies cannot override test HTTP cookies.
 				tmp.append(format_cookie_key_value(key, value))
 		return tmp
 
+	def __get_user_agent(self):
+		return self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
+
 	def __build_command(self, record):
 		tmp = ["curl", ("--connect-timeout {0}").format(self.__connect_timeout), ("-m {0}").format(self.__read_timeout), "-iskL", ("--max-redirs {0}").format(self.__max_redirects), "--path-as-is"]
 		if record["body"]:
 			tmp.append(set_param(record["body"], "-d"))
 		if record["proxy"]:
 			tmp.append(set_param(record["proxy"], "-x"))
 		if record["user_agent"]:
@@ -516,14 +520,16 @@
 		if record["cookies"]:
 			tmp.append(set_param(("; ").join(record["cookies"]), "-b"))
 		tmp.append(set_param(record["method"], "-X"))
 		tmp.append(set_param(record["url"]))
 		tmp = (" ").join(tmp)
 		return tmp
 
+	# ------------------------------------
+
 	def __run_tests(self):
 		results = []
 		print_time(("Running tests with {0} engine...").format("PycURL" if self.__curl else "Python Requests"))
 		print("Press CTRL + C to exit early - results will be saved")
 		progress = Progress(len(self.__collection), self.__print_lock)
 		progress.show()
 		with concurrent.futures.ThreadPoolExecutor(max_workers = self.__threads) as executor:
@@ -534,29 +540,31 @@
 				for subprocess in concurrent.futures.as_completed(subprocesses):
 					results.append(subprocess.result())
 					progress.show()
 			except KeyboardInterrupt:
 				executor.shutdown(wait = True, cancel_futures = True)
 		self.__collection = results
 
-	def __send_curl(self, record, passthrough = False):
+	# ------------------------------------
+
+	def __send_curl(self, record, ignore = True, response_headers = False, response_body = False, save = True):
 		curl = None
 		cookiefile = None
 		headers = None
 		response = None
 		try:
 			# ----------------------------
 			curl = pycurl.Curl()
 			# ----------------------------
 			cookiefile = tempfile.NamedTemporaryFile(mode = "r") # NOTE: Important! Store and pass HTTP cookies on HTTP redirects.
 			curl.setopt(pycurl.COOKIESESSION, True)
 			curl.setopt(pycurl.COOKIEFILE, cookiefile.name)
 			curl.setopt(pycurl.COOKIEJAR, cookiefile.name)
 			# ----------------------------
-			if passthrough:
+			if response_headers:
 				headers = io.BytesIO()
 				curl.setopt(pycurl.HEADERFUNCTION, headers.write)
 			# ----------------------------
 			response = io.BytesIO()
 			curl.setopt(pycurl.WRITEFUNCTION, response.write)
 			# ----------------------------
 			curl.setopt(pycurl.HTTP_VERSION, pycurl.CURL_HTTP_VERSION_1_1)
@@ -587,26 +595,27 @@
 			if record["proxy"]:
 				curl.setopt(pycurl.PROXY, record["proxy"])
 			# ----------------------------
 			curl.perform()
 			# ----------------------------
 			record["code"] = int(curl.getinfo(pycurl.RESPONSE_CODE))
 			record["length"] = int(curl.getinfo(pycurl.SIZE_DOWNLOAD))
+			record["response"] = self.__decode(response.getvalue())
 			record["id"] = ("{0}-{1}-{2}").format(record["code"], record["length"], record["id"])
-			content = response.getvalue()
-			if passthrough:
+			if response_headers:
 				record["response_headers"] = self.__decode(headers.getvalue())
-				# record["response"] = self.__decode(content)
-			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(content), self.__regex_flags)):
-				record["code"] = IGNORED
-			# NOTE: Additional validation to prevent congestion from writing large and usless data to files.
-			elif record["code"] >= 200 and record["code"] < 400:
+			if ignore:
+				if record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, record["response"], self.__regex_flags)):
+					record["code"] = IGNORED
+			if save and record["code"] >= 200 and record["code"] < 400: # NOTE: Additional validation to prevent congestion from writing large and usless data to files.
 				file = os.path.join(self.__directory, ("{0}.txt").format(record["id"]))
 				if not os.path.exists(file):
-					open(file, "wb").write(content)
+					open(file, "w").write(record["response"])
+			if not response_body:
+				record["response"] = ""
 			# ----------------------------
 		except (pycurl.error, FileNotFoundError) as ex:
 			# --------------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -620,15 +629,15 @@
 				curl.close()
 			# ----------------------------
 			if cookiefile:
 				cookiefile.close() # NOTE: Important! Close the file handle strictly after closing the cURL handle.
 			# ----------------------------
 		return record
 
-	def __send_request(self, record, passthrough = False):
+	def __send_request(self, record, ignore = True, response_headers = False, response_body = False, save = True):
 		session = None
 		response = None
 		try:
 			# ----------------------------
 			session = requests.Session()
 			session.max_redirects = self.__max_redirects
 			# ----------------------------
@@ -657,26 +666,27 @@
 				verify = self.__verify,
 				allow_redirects = self.__allow_redirects,
 				timeout = (self.__connect_timeout, self.__read_timeout)
 			)
 			# ----------------------------
 			record["code"] = int(response.status_code)
 			record["length"] = len(response.content)
+			record["response"] = self.__decode(response.content)
 			record["id"] = ("{0}-{1}-{2}").format(record["code"], record["length"], record["id"])
-			content = response.content
-			if passthrough:
+			if response_headers:
 				record["response_headers"] = dict(response.headers)
-				# record["response"] = self.__decode(content)
-			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(content), self.__regex_flags)):
-				record["code"] = IGNORED
-			# NOTE: Additional validation to prevent congestion from writing large and usless data to files.
-			elif record["code"] >= 200 and record["code"] < 400:
+			if ignore:
+				if record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, record["response"], self.__regex_flags)):
+					record["code"] = IGNORED
+			if save and record["code"] >= 200 and record["code"] < 400: # NOTE: Additional validation to prevent congestion from writing large and usless data to files.
 				file = os.path.join(self.__directory, ("{0}.txt").format(record["id"]))
 				if not os.path.exists(file):
-					open(file, "wb").write(content)
+					open(file, "w").write(record["response"])
+			if not response_body:
+				record["response"] = ""
 			# ----------------------------
 		except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException, FileNotFoundError) as ex:
 			# ----------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -688,15 +698,17 @@
 			# ----------------------------
 		return record
 
 	def __set_double_headers(self, request, headers):
 		exists = set()
 		for header in headers:
 			key, value = get_header_key_value(header)
-			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value) # NOTE: Allows double headers.
+			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value)
+
+	# ------------------------------------
 
 	def __validate_results(self):
 		print_time("Validating results...")
 		self.__mark_duplicates()
 		output = Output(self.__collection)
 		self.__collection = output.results_table() if self.__show_table else output.results_json()
 		output.stats_table()
@@ -704,14 +716,16 @@
 	def __mark_duplicates(self):
 		exists = set()
 		for record in self.__collection:
 			if record["id"] not in exists and not exists.add(record["id"]):
 				continue
 			record["code"] = DUPLICATE
 
+	# ------------------------------------
+
 	def __prepare_collection(self):
 		print_time("Preparing test records...")
 		# --------------------------------
 		# NOTE: Stress testing.
 		self.__records(
 			identifier = "STRESS-1",
 			urls       = self.__url["urls"]["base"]
@@ -727,15 +741,15 @@
 
 	def __color(self, value, color):
 		return ("{0}{1}{2}").format(color, value, colorama.Style.RESET_ALL)
 
 	def __results_row(self, record, color):
 		return [self.__color(record[key], color) for key in ["id", "code", "length", "command"]]
 
-	def results_table(self):
+	def results_table(self): # NOTE: To see more or less results, comment in or out 'continue' line.
 		tmp = []; table = []
 		for record in self.__collection:
 			if record["code"] < 100 or record["code"] >= 600:
 				continue
 			elif record["code"] >= 500:
 				continue
 				table.append(self.__results_row(record, colorama.Fore.CYAN))
@@ -829,15 +843,15 @@
 			self.__count += 1
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
 
 	def print_help(self):
-		print("Stresser v11.0 ( github.com/ivan-sincek/forbidden )")
+		print("Stresser v11.1 ( github.com/ivan-sincek/forbidden )")
 		print("")
 		print("Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]")
 		print("Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]")
 		print("")
 		print("DESCRIPTION")
 		print("    Bypass 4xx HTTP response status codes with stress testing")
 		print("URL")
@@ -958,37 +972,37 @@
 
 	def __print_error(self, msg):
 		print(("ERROR: {0}").format(msg))
 
 	def __parse_url(self, value, key):
 		data = {
 			"url": {
-				"schemes": ["http", "https"],
-				"scheme_error": [
-					"Inaccessible URL: Scheme is required",
-					"Inaccessible URL: Supported schemes are 'http' and 'https'"
-				],
+				"schemes"     : ["http", "https"],
+				"scheme_error": {
+					"required"   : "Inaccessible URL: Scheme is required",
+					"unsupported": "Inaccessible URL: Supported schemes are 'http' and 'https'"
+				},
 				"domain_error": "Inaccessible URL: Invalid domain name",
-				"port_error": "Inaccessible URL: Port number is out of range"
+				"port_error"  : "Inaccessible URL: Port number is out of range"
 			},
 			"proxy": {
-				"schemes": ["http", "https", "socks4", "socks4h", "socks5", "socks5h"],
-				"scheme_error": [
-					"Proxy URL: Scheme is required",
-					"Proxy URL: Supported schemes are 'http[s]', 'socks4[h]', and 'socks5[h]'"
-				],
+				"schemes"     : ["http", "https", "socks4", "socks4h", "socks5", "socks5h"],
+				"scheme_error": {
+					"required"   : "Proxy URL: Scheme is required",
+					"unsupported": "Proxy URL: Supported schemes are 'http[s]', 'socks4[h]', and 'socks5[h]'"
+				},
 				"domain_error": "Proxy URL: Invalid domain name",
-				"port_error": "Proxy URL: Port number is out of range"
+				"port_error"  : "Proxy URL: Port number is out of range"
 			}
 		}
 		tmp = urllib.parse.urlsplit(value)
 		if not tmp.scheme:
-			self.__error(data[key]["scheme_error"][0])
+			self.__error(data[key]["scheme_error"]["required"])
 		elif tmp.scheme not in data[key]["schemes"]:
-			self.__error(data[key]["scheme_error"][1])
+			self.__error(data[key]["scheme_error"]["unsupported"])
 		elif not tmp.netloc:
 			self.__error(data[key]["domain_error"])
 		elif tmp.port and (tmp.port < 1 or tmp.port > 65535):
 			self.__error(data[key]["port_error"])
 		return value
 
 	def __parse_header(self, headers):
@@ -1079,15 +1093,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                             Stresser v11.0                             #")
+		print("#                             Stresser v11.1                             #")
 		print("#                                 by Ivan Sincek                         #")
 		print("#                                                                        #")
 		print("# Bypass 4xx HTTP response status codes  with stress testing.            #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                 #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
```

### Comparing `forbidden-11.0/src/stresser/user_agents.txt` & `forbidden-11.1/src/stresser/user_agents.txt`

 * *Files identical despite different names*

