# Comparing `tmp/cargo_workspace-1.2.1.tar.gz` & `tmp/cargo_workspace-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cargo_workspace-1.2.1.tar", last modified: Mon Feb 26 16:59:43 2024, max compression
+gzip compressed data, was "cargo_workspace-1.2.4.tar", last modified: Wed May 15 10:18:54 2024, max compression
```

## Comparing `cargo_workspace-1.2.1.tar` & `cargo_workspace-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-02-26 16:59:43.270637 cargo_workspace-1.2.1/
--rw-r--r--   0 vados      (501) staff       (20)     1154 2024-02-26 16:59:43.270426 cargo_workspace-1.2.1/PKG-INFO
--rw-r--r--   0 vados      (501) staff       (20)      565 2024-02-24 14:50:43.000000 cargo_workspace-1.2.1/README.md
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-02-26 16:59:43.269223 cargo_workspace-1.2.1/cargo_workspace/
--rw-r--r--   0 vados      (501) staff       (20)       89 2024-02-23 13:18:28.000000 cargo_workspace-1.2.1/cargo_workspace/__init__.py
--rw-r--r--   0 vados      (501) staff       (20)     8451 2024-02-26 14:41:55.000000 cargo_workspace-1.2.1/cargo_workspace/parsing.py
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-02-26 16:59:43.270184 cargo_workspace-1.2.1/cargo_workspace.egg-info/
--rw-r--r--   0 vados      (501) staff       (20)     1154 2024-02-26 16:59:43.000000 cargo_workspace-1.2.1/cargo_workspace.egg-info/PKG-INFO
--rw-r--r--   0 vados      (501) staff       (20)      295 2024-02-26 16:59:43.000000 cargo_workspace-1.2.1/cargo_workspace.egg-info/SOURCES.txt
--rw-r--r--   0 vados      (501) staff       (20)        1 2024-02-26 16:59:43.000000 cargo_workspace-1.2.1/cargo_workspace.egg-info/dependency_links.txt
--rw-r--r--   0 vados      (501) staff       (20)       35 2024-02-26 16:59:43.000000 cargo_workspace-1.2.1/cargo_workspace.egg-info/requires.txt
--rw-r--r--   0 vados      (501) staff       (20)       16 2024-02-26 16:59:43.000000 cargo_workspace-1.2.1/cargo_workspace.egg-info/top_level.txt
--rw-r--r--   0 vados      (501) staff       (20)      708 2024-02-26 15:58:51.000000 cargo_workspace-1.2.1/pyproject.toml
--rw-r--r--   0 vados      (501) staff       (20)       38 2024-02-26 16:59:43.270676 cargo_workspace-1.2.1/setup.cfg
-drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-02-26 16:59:43.270017 cargo_workspace-1.2.1/tests/
--rw-r--r--   0 vados      (501) staff       (20)     5894 2024-02-26 14:39:22.000000 cargo_workspace-1.2.1/tests/test_parsing.py
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.337038 cargo_workspace-1.2.4/
+-rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-15 10:18:54.336847 cargo_workspace-1.2.4/PKG-INFO
+-rw-r--r--   0 vados      (501) staff       (20)      565 2024-02-24 14:50:43.000000 cargo_workspace-1.2.4/README.md
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.334950 cargo_workspace-1.2.4/cargo_workspace/
+-rw-r--r--   0 vados      (501) staff       (20)      247 2024-03-25 13:04:02.000000 cargo_workspace-1.2.4/cargo_workspace/__init__.py
+-rw-r--r--   0 vados      (501) staff       (20)      822 2024-03-25 11:26:03.000000 cargo_workspace-1.2.4/cargo_workspace/dependency.py
+-rw-r--r--   0 vados      (501) staff       (20)     8827 2024-05-15 10:13:02.000000 cargo_workspace-1.2.4/cargo_workspace/lib.py
+-rw-r--r--   0 vados      (501) staff       (20)     5613 2024-03-25 13:11:07.000000 cargo_workspace-1.2.4/cargo_workspace/version.py
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.336530 cargo_workspace-1.2.4/cargo_workspace.egg-info/
+-rw-r--r--   0 vados      (501) staff       (20)     1154 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/PKG-INFO
+-rw-r--r--   0 vados      (501) staff       (20)      344 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/SOURCES.txt
+-rw-r--r--   0 vados      (501) staff       (20)        1 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/dependency_links.txt
+-rw-r--r--   0 vados      (501) staff       (20)       35 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/requires.txt
+-rw-r--r--   0 vados      (501) staff       (20)       16 2024-05-15 10:18:54.000000 cargo_workspace-1.2.4/cargo_workspace.egg-info/top_level.txt
+-rw-r--r--   0 vados      (501) staff       (20)      708 2024-05-15 10:18:50.000000 cargo_workspace-1.2.4/pyproject.toml
+-rw-r--r--   0 vados      (501) staff       (20)       38 2024-05-15 10:18:54.337082 cargo_workspace-1.2.4/setup.cfg
+drwxr-xr-x   0 vados      (501) staff       (20)        0 2024-05-15 10:18:54.336185 cargo_workspace-1.2.4/tests/
+-rw-r--r--   0 vados      (501) staff       (20)    14405 2024-05-15 10:18:33.000000 cargo_workspace-1.2.4/tests/test_lib.py
```

### Comparing `cargo_workspace-1.2.1/PKG-INFO` & `cargo_workspace-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo_workspace
-Version: 1.2.1
+Version: 1.2.4
 Summary: Parse a cargo workspace and analyze its packages
 Author-email: Oliver Tale-Yazdi <oliver@tasty.limo>
 Project-URL: Homepage, https://github.com/ggwpez/py-cargo-workspace
 Keywords: cargo,rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cargo_workspace-1.2.1/README.md` & `cargo_workspace-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cargo_workspace-1.2.1/cargo_workspace/parsing.py` & `cargo_workspace-1.2.4/cargo_workspace/lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,214 +1,122 @@
 import os
 import toml
 
-class Version:
-	def __init__(self, x, y=0, z=0, suffix=None):
-		self._x = x
-		self._y = y
-		self._z = z
-		self._suffix = suffix
-	
-	def __str__(self):
-		su = f"-{self._suffix}" if self._suffix is not None else ""
-
-		return f"{self._x}.{self._y}.{self._z}{su}"
-	
-	def __eq__(self, other):
-		return (self._x == other._x) and (self._y == other._y) and (self._z == other._z) and (self._suffix == other._suffix)
-
-	def from_str(s):
-		if '-' in s:
-			splits = s.partition('-')
-			ver = splits[0]
-			suffix = splits[2]
-		else:
-			ver = s
-			suffix = None
-
-		v = Version.from_str_no_suffix(ver)
-		v._suffix = suffix
-		
-		return v
-	
-	def from_str_no_suffix(s):
-		parts = s.split('.')
-		if len(parts) == 1:
-			return Version(int(parts[0]))
-		if len(parts) == 2:
-			return Version(int(parts[0]), int(parts[1]))
-		if len(parts) == 3:
-			return Version(int(parts[0]), int(parts[1]), int(parts[2]))
-		raise ValueError(f'Invalid version string: {s}')
-	
-	def cargo_convention(self):
-		return CargoVersion(self)
-	
-	def is_stable(self):
-		return self._suffix is None and self._x > 0
-	
-	def __getattr__(self, name):
-		if name == 'x':
-			return self._x
-		if name == 'y':
-			return self._y
-		if name == 'z':
-			return self._z
-		if name == 'suffix':
-			return self._suffix
-		
-		raise AttributeError(f'No such attribute: {name}')
-class CargoVersion:
-	def __init__(self, version):
-		self._version = version
-	
-	def __eq__(self, other):
-		return self._version == other._version
-
-	def __str__(self):
-		return str(self._version)
-
-	def is_stable(self):
-		return self._version.is_stable()
-
-	def diff(self, other):
-		return CargoVersionBump(self, other)
-
-	def __getattr__(self, name):
-		if name == 'major':
-			return self._major()
-		if name == 'minor':
-			return self._minor()
-		if name == 'patch':
-			return self._patch()
-		if name == 'suffix':
-			return self._suffix()
-		
-		raise AttributeError(f'No such attribute: {name}')
-
-	def _major(self):
-		if self._version.x > 0:
-			return self._version.x
-		if self._version.y > 0:
-			return self._version.y
-		return self._version.z
-	
-	def _minor(self):
-		if self._version.x > 0:
-			return self._version.y
-		if self._version.y > 0:
-			return self._version.z
-		return None
-	
-	def _patch(self):
-		if self._version.x > 0:
-			return self._version.z
-		return None
-	
-	def _suffix(self):
-		return self._version.suffix()
-
-class CargoVersionBump:
-	def __init__(self, old, new):
-		self._old = old
-		self._new = new
-	
-	def is_stable(self):
-		return self._old.is_stable() and self._new.is_stable()
-	
-	def is_empty(self):
-		return self._old == self._new
-	
-	def is_major(self):
-		return self._old.major != self._new.major
-	
-	def is_strict_major(self):
-		return self.is_major() and (self._old.minor == 0) and (self._old.patch == 0)
-	
-	def is_minor(self):
-		return (self._old.major == self._new.major) and (self._old.minor != self._new.minor)
-	
-	def is_strict_minor(self):
-		return self.is_minor() and (self._old.patch == 0)
-	
-	def is_patch(self):
-		return (self._old.major == self._new.major) and (self._old.minor == self._new.minor) and (self._old.patch != self._new.patch)
+from .dependency import Dependencies
+from .version import Version, CargoVersion, CargoVersionBump
 
 class Crate:
-	def __init__(self, manifest, path):
+	def __init__(self, manifest, path, root_dir=None):
+		Crate.__ensure_is_manifest(manifest)
 		self._manifest = manifest
 		self._path = path
+		self._root_dir = root_dir
 
-	def from_path(path):
-		# check if the file exists
-		if not os.path.exists(path):
-			raise ValueError(f'Could not load crate manifest at {path}')
+	def from_path(path, root_dir=None):
+		abs_path = os.path.join(root_dir, path) if root_dir else path
+		if not os.path.exists(abs_path):
+			raise ValueError(f'Could not load crate manifest at {abs_path}')
 
 		try:
-			with open(path, 'r') as f:
-				return Crate.from_raw_manifest(f.read(), path)
+			with open(abs_path, 'r') as f:
+				return Crate.from_raw_manifest(f.read(), path, root_dir)
 		except FileNotFoundError:
-			raise ValueError(f'Could not load crate manifest at {path}')
+			raise ValueError(f'Could not load crate manifest at {abs_path}')
 	
-	def from_raw_manifest(content, path):
+	def from_raw_manifest(content, path, root_dir=None):
 		manifest = toml.loads(content)
-		return Crate(manifest, path)
+		return Crate(manifest, path, root_dir)
 
-	def is_crate_manifest(manifest):
+	def __ensure_is_manifest(manifest):
 		if 'workspace' in manifest:
-			return ValueError(f'A single crate was expected at {path}, but it does contain a workspace section')
+			raise ValueError(f'A single crate was expected, but it does contain a workspace section')
 		if not 'package' in manifest:
-			return ValueError(f'Could not find package in crate manifest at {path}')
+			raise ValueError(f'Could not find package in crate manifest')
+		if not 'name' in manifest['package']:
+			raise ValueError(f'Could not find name in crate manifest')
 
 	def __getattr__(self, name):
 		# Not using 'match' here since it requires python version 3.10.
 		if name == 'name':
 			return self._crate()['name']
 		if name == 'version':
 			return self._get_version()
-		if name == 'path':
+		if name == 'rel_path':
 			return self._path
+		if name == 'full_path':
+			return os.path.join(self._root_dir, self._path) if self._root_dir else self._path
+		if name == 'abs_path' or name == 'path':
+			return os.path.abspath(self.full_path)
 		if name == 'metadata':
 			return self._get_metadata()
 		if name == 'publish':
 			return self._get_publish()
+		if name == 'description':
+			return self._crate().get('description', None)
+		if name == 'edition':
+			return self._crate().get('edition', None)
+		if name == 'authors':
+			return self._crate().get('authors', [])
+		if name == 'dependencies':
+			return self.dependencies_by_kinds()
 
 		raise AttributeError(f'No such attribute: {name}')
 
+	def dependencies_by_kinds(self, kinds=['normal', 'build', 'dev']):
+		deps = {}
+		for kind in kinds:
+			table = f"{kind}-dependencies" if kind != 'normal' else 'dependencies'
+			table = self._manifest.get(table, None)
+			if table is None:
+				continue
+   
+			for dep in table:
+				if not kind in deps:
+					deps[kind] = []
+				deps[kind].append(dep)
+		return Dependencies.from_map(deps)
+
 	def _get_version(self):
 		if not 'version' in self._crate():
 			raise ValueError(f'Could not find version in crate manifest at {self._path}')
-		return Version.from_str(self._crate()['version'])
+		return Version.from_str(self._crate()['version']).cargo_convention()
 
 	def _get_metadata(self):
 		return Metadata(self._crate().get('metadata', {}))
 
 	def _crate(self):
 		if not 'package' in self._manifest:
 			raise ValueError(f'Could not find package in crate manifest at {self._path}')
-		return self._manifest['package']		
-	
+		return self._manifest['package']
+
 	def _get_publish(self):
 		if not 'publish' in self._crate():
 			return True
 
 		return bool(self._crate()['publish'])
 
 class Manifest:
 	def __init__(self, content, path):
 		self._content = content
 		self._path = path
 	
+	def from_parsed(content, path):
+		return Manifest(content, path)
+
+	def from_raw(content, path):
+		parsed = toml.loads(content)
+		return Manifest.from_parsed(parsed, path)
+
 	def from_path(path):
 		with open(path, 'rb') as f:
-			manifest = toml.load(f)
-		return Manifest(manifest, path)
+			raw = f.read()
+			return Manifest.from_raw(raw, path)
 	
-	def into_crate(self, path):
-		return Crate(self._content, path)
+	def into_crate(self):
+		return Crate(self._content, self._path)
 
 class Metadata:
 	'''
 	A typed wrapper around a dictionary that represents the metadata section of a crate manifest.
 	'''
 
 	def __init__(self, content):
@@ -221,20 +129,92 @@
 		for split in splits:
 			if split in obj:
 				obj = obj[split]
 			else:
 				return default
 		return obj
 
+class CratesCollection:
+	def __init__(self, crates):
+		self._crates = crates
+
+	def inner(self):
+		'''
+		Escape hatch to get the inner raw value.
+		'''
+
+		return self._crates
+
+	def without_by_name(self, names):
+		'''
+		Removes crates by name from the collection.
+		'''
+
+		return CratesCollection([crate for crate in self._crates if crate.name not in names])
+
+	def without(self, pred):
+		'''
+		Removes crates from the collection that satisfy the predicate.
+		'''
+
+		return CratesCollection([crate for crate in self._crates if not pred(crate)])
+
+	def find_by_name(self, name):
+		'''
+		Finds a crate by name.
+		'''
+
+		for crate in self._crates:
+			if crate.name == name:
+				return crate
+		return None
+
+	def __len__(self):
+		return len(self._crates)
+
+	def __iter__(self):
+		return iter(self._crates)
+
+	def __getitem__(self, index):
+		return self._crates[index]
+
+	def __getattr__(self, name):
+		if name == 'rel_paths':
+			return [crate.rel_path for crate in self._crates]
+		if name == 'abs_paths':
+			return [crate.abs_path for crate in self._crates]
+		if name == 'names':
+			return [crate.name for crate in self._crates]
+		
+		raise AttributeError(f'No such attribute: {name}')
+	
+	def into_linter(self):
+		return CratesLinter(self._crates)
+
+class CratesLinter:
+	def __init__(self, crates):
+		self._crates = crates
+		
+	def ensure_uses_workspace_inheritance(self, attribute):
+		good = {'workspace': True}
+
+		for crate in self._crates:
+			got = getattr(crate, attribute, None)
+			if got != good:
+				raise ValueError(f'Attribute {attribute} is not inherited from the workspace in {crate.path} but instead set to {got}')
+
 class Workspace:
 	def __init__(self, manifest, root_path=None):
 		self._manifest = manifest
 		self._root_dir = root_path or os.getcwd()
 		self._crates = Workspace.__crates_from_manifest(manifest, self._root_dir)
 
+	def __str__(self):
+		return f'workspace at {self._root_dir} with {len(self._crates)} crates'
+
 	def from_raw_manifest(content, root_dir):
 		manifest = toml.loads(content)
 		return Workspace(manifest, root_dir)
 
 	def from_path(path, allow_dir=True):
 		if not path.endswith('Cargo.toml') and allow_dir:
 			path = os.path.join(path, 'Cargo.toml')
@@ -251,83 +231,96 @@
 		crates = []
 
 		if 'workspace' not in manifest or 'members' not in manifest['workspace']:
 			return		
 
 		# Go through the list of members and create Crate objects:
 		for path in manifest['workspace']['members']:
-			path = os.path.join(root_dir, path)
 			path = os.path.join(path, 'Cargo.toml')
 
-			crate = Crate.from_path(path)
+			crate = Crate.from_path(path, root_dir=root_dir)
 			crates.append(crate)
 		
-		Workspace.__check_no_duplicate_paths(crates)
 		return crates
 	
-	def __check_no_duplicate_paths(crates):
+	def __getattr__(self, name):
+		if name == 'path':
+			return self._root_dir
+		if name == 'crates':
+			return CratesCollection(self._crates)
+		if name == 'manifest':
+			return self._manifest
+
+		raise AttributeError(f'No such attribute: {name}')
+
+	def crate_by_name(self, name):
+		found = []
+		for crate in self.crates:
+			if crate.name == name:
+				found.append(crate)
+		
+		if len(found) > 1:
+			raise ValueError(f'Found multiple crates with name {name}')
+		if len(found) == 0:
+			return None
+		return found[0]
+
+	def into_linter(self):
+		return WorkspaceLinter(self)
+
+class WorkspaceLinter:
+	def __init__(self, workspace):
+		self._workspace = workspace
+	
+	def ensure_no_stray_manifest_files(self, excluded_crates=[]):
+		stray = self.__find_stray_manifests()
+		stray.sort()
+		excluded_crates.sort()
+
+		bad = []
+		for path in stray:
+			if path not in excluded_crates:
+				bad.append(path)
+
+		if len(bad) > 0:
+			raise ValueError(f'Found stray manifests: {bad}')
+
+	def ensure_no_duplicate_crate_paths(self):
 		paths = set()
-		for crate in crates:
-			path = os.path.abspath(crate.path)
+		for crate in self._workspace.crates:
+			path = os.path.abspath(crate.rel_path)
 			if path in paths:
-				raise ValueError(f'There are two crates with the same absolute path {path}')
+				raise ValueError(f'There are two crates with the same absolute path {self._workspace.path}')
 
 			paths.add(path)
-
-	def ensure_no_stray_manifests(self):
-		stray = self.find_stray_manifests()
-
-		if stray is not None:
-			raise ValueError(f'Found stray manifest(s) at: {stray}')
 	
-	def find_stray_manifests(self, excluded_crates=None):
-		all_paths = Workspace.find_manifest_paths(self._root_dir, exclude_dirs=["target"])
-		workspace_paths = [os.path.abspath(crate.path) for crate in self.crates]
+	def __find_stray_manifests(self, excluded_crates=None):
+		all_paths = WorkspaceLinter.__find_manifest_paths(self._workspace.path, exclude_dirs=["target"])
+		workspace_paths = self._workspace.crates.abs_paths
 		stray_paths = []
 
 		for path in all_paths:
 			if os.path.abspath(path) not in workspace_paths:
 				stray_paths.append(path)
 		
-		stray_paths.remove(os.path.join(self._root_dir, 'Cargo.toml'))
+		stray_paths.remove(os.path.join(self._workspace.path, 'Cargo.toml'))
 		stray_paths.sort()
 
 		if len(stray_paths) > 0:
 			return stray_paths
 		return None
-	
-	def find_manifest_paths(root_dir, exclude_dirs):
+
+	def __find_manifest_paths(root_dir, exclude_dirs):
 		paths = []
 		for root, dirs, files in os.walk(root_dir):
 			if any(exclude in root for exclude in exclude_dirs):
 				continue
 			if 'Cargo.toml' in files:
 				path = os.path.join(root, 'Cargo.toml')
 
 				if os.path.islink(path):
 					raise ValueError(f'Found symlinked manifest at {path}')
 
 				paths.append(path)
 
 		paths.sort()
 		return paths
-	
-	def __getattr__(self, name):
-		if name == 'path':
-			return self._root_dir
-		if name == 'crates':
-			return self._crates
-
-		raise AttributeError(f'No such attribute: {name}')
-
-	def crate_by_name(self, name):
-		found = []
-		for crate in self.crates():
-			if crate.name() == name:
-				found.append(crate)
-		
-		if len(found) > 1:
-			raise ValueError(f'Found multiple crates with name {name}')
-		if len(found) == 0:
-			return None
-		return found[0]
-
```

### Comparing `cargo_workspace-1.2.1/cargo_workspace.egg-info/PKG-INFO` & `cargo_workspace-1.2.4/cargo_workspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo_workspace
-Version: 1.2.1
+Version: 1.2.4
 Summary: Parse a cargo workspace and analyze its packages
 Author-email: Oliver Tale-Yazdi <oliver@tasty.limo>
 Project-URL: Homepage, https://github.com/ggwpez/py-cargo-workspace
 Keywords: cargo,rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cargo_workspace-1.2.1/pyproject.toml` & `cargo_workspace-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cargo_workspace"
-version = "1.2.1"
+version = "1.2.4"
 requires-python = ">=3.6"
 authors = [
     { name = "Oliver Tale-Yazdi", email="oliver@tasty.limo" },
 ]
 description = "Parse a cargo workspace and analyze its packages"
 classifiers = [
     "Programming Language :: Python :: 3",
```

