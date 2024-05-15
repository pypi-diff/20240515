# Comparing `tmp/utk_exodus-0.1.6.tar.gz` & `tmp/utk_exodus-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.6.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.7.tar", max compression
```

## Comparing `utk_exodus-0.1.6.tar` & `utk_exodus-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     3403 2024-05-10 17:15:08.669580 utk_exodus-0.1.6/README.md
--rw-r--r--   0        0        0      654 2024-05-10 17:15:08.669872 utk_exodus-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      539 2024-05-10 17:15:08.670127 utk_exodus-0.1.6/utk_exodus/__init__.py
--rw-r--r--   0        0        0     2387 2024-05-10 00:17:11.629365 utk_exodus-0.1.6/utk_exodus/config/samvera_default.yml
--rw-r--r--   0        0        0    12260 2024-05-10 00:17:11.629691 utk_exodus-0.1.6/utk_exodus/config/utk_dc.yml
--rw-r--r--   0        0        0    11044 2024-05-10 00:17:11.629996 utk_exodus-0.1.6/utk_exodus/config/utk_dc_no_uris.yml
--rw-r--r--   0        0        0     7824 2024-05-10 00:17:11.630293 utk_exodus-0.1.6/utk_exodus/config/utk_no_uris_no_names.yml
--rw-r--r--   0        0        0       79 2024-05-10 00:17:11.630638 utk_exodus-0.1.6/utk_exodus/controller/__init__.py
--rw-r--r--   0        0        0     6203 2024-05-10 17:15:08.670522 utk_exodus-0.1.6/utk_exodus/controller/controller.py
--rw-r--r--   0        0        0       59 2024-05-10 00:17:11.630872 utk_exodus-0.1.6/utk_exodus/curate/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.6/utk_exodus/curate/curate.py
--rw-r--r--   0        0        0     3997 2024-05-10 00:17:11.631147 utk_exodus-0.1.6/utk_exodus/exodus.py
--rw-r--r--   0        0        0       61 2024-05-10 00:17:11.631361 utk_exodus-0.1.6/utk_exodus/fedora/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-10 16:33:04.511046 utk_exodus-0.1.6/utk_exodus/fedora/fedora.py
--rw-r--r--   0        0        0       63 2024-05-10 00:17:11.631585 utk_exodus-0.1.6/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18702 2024-05-10 00:17:11.631880 utk_exodus-0.1.6/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.6/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.6/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.6/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    39221 2024-05-09 19:07:23.849346 utk_exodus-0.1.6/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0      103 2024-05-10 17:15:08.670786 utk_exodus-0.1.6/utk_exodus/restrict/__init__.py
--rw-r--r--   0        0        0     4324 2024-05-10 17:15:08.671022 utk_exodus-0.1.6/utk_exodus/restrict/restrict.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.6/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0    10393 2024-05-10 13:15:07.969877 utk_exodus-0.1.6/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.6/utk_exodus/validate/__init__.py
--rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.6/utk_exodus/validate/validate.py
--rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 utk_exodus-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3755 2024-05-15 15:33:14.611533 utk_exodus-0.1.7/README.md
+-rw-r--r--   0        0        0      654 2024-05-15 15:33:14.611849 utk_exodus-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-05-15 15:33:14.612191 utk_exodus-0.1.7/utk_exodus/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-15 14:25:18.889957 utk_exodus-0.1.7/utk_exodus/combine/__init__.py
+-rw-r--r--   0        0        0     1868 2024-05-15 14:25:18.890339 utk_exodus-0.1.7/utk_exodus/combine/combine.py
+-rw-r--r--   0        0        0     2387 2024-05-10 00:17:11.629365 utk_exodus-0.1.7/utk_exodus/config/samvera_default.yml
+-rw-r--r--   0        0        0    12260 2024-05-10 00:17:11.629691 utk_exodus-0.1.7/utk_exodus/config/utk_dc.yml
+-rw-r--r--   0        0        0    11044 2024-05-10 00:17:11.629996 utk_exodus-0.1.7/utk_exodus/config/utk_dc_no_uris.yml
+-rw-r--r--   0        0        0     7824 2024-05-10 00:17:11.630293 utk_exodus-0.1.7/utk_exodus/config/utk_no_uris_no_names.yml
+-rw-r--r--   0        0        0       79 2024-05-10 00:17:11.630638 utk_exodus-0.1.7/utk_exodus/controller/__init__.py
+-rw-r--r--   0        0        0     6346 2024-05-15 14:25:18.891011 utk_exodus-0.1.7/utk_exodus/controller/controller.py
+-rw-r--r--   0        0        0       59 2024-05-10 00:17:11.630872 utk_exodus-0.1.7/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.7/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     5724 2024-05-15 15:33:14.612699 utk_exodus-0.1.7/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       61 2024-05-10 00:17:11.631361 utk_exodus-0.1.7/utk_exodus/fedora/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-10 16:33:04.511046 utk_exodus-0.1.7/utk_exodus/fedora/fedora.py
+-rw-r--r--   0        0        0       63 2024-05-10 00:17:11.631585 utk_exodus-0.1.7/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18702 2024-05-10 00:17:11.631880 utk_exodus-0.1.7/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.7/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.7/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.7/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    47840 2024-05-14 12:54:12.683039 utk_exodus-0.1.7/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0      103 2024-05-10 17:15:08.670786 utk_exodus-0.1.7/utk_exodus/restrict/__init__.py
+-rw-r--r--   0        0        0     4324 2024-05-10 17:15:08.671022 utk_exodus-0.1.7/utk_exodus/restrict/restrict.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.7/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0    11179 2024-05-15 14:25:18.891820 utk_exodus-0.1.7/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       65 2024-05-15 14:25:18.892035 utk_exodus-0.1.7/utk_exodus/template/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-15 14:25:18.892200 utk_exodus-0.1.7/utk_exodus/template/template.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.7/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.7/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 utk_exodus-0.1.7/PKG-INFO
```

### Comparing `utk_exodus-0.1.6/README.md` & `utk_exodus-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -58,14 +58,26 @@
 
 If for some reason you need to create a files sheet for  works after the fact, use:
 
 ```shell
 exodus add_files --sheet path/to/sheet.csv --files_sheet path/to/files_sheet.csv 
 ```
 
+If you need to remove unused values from an import or work sheet, you can:
+
+```shell
+exodus remove_old_values --sheet path/to/sheet.csv --old_sheet path/to/old_sheet.csv --new_sheet path/to/new_sheet.csv
+```
+
+If you want to generate a full template for a metadata import, use:
+
+```shell
+exodus generate_template --model book -o /path/to/sheet.csv
+```
+
 ## What's Missing Here Right Now
 
 * The ability to create pcdm:Collection objects.
 * The ability to create a new metadata import from a previous import
 
 ## Understanding Configs
```

### Comparing `utk_exodus-0.1.6/pyproject.toml` & `utk_exodus-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utk-exodus"
-version = "0.1.6"
+version = "0.1.7"
 description = "A tool for building import sheets from UTK legacy systems"
 authors = ["Mark Baggett <mbagget1@utk.edu>"]
 readme = "README.md"
 include = [
     { path = "utk_exodus/config", format = ["sdist", "wheel"] }
 ]
```

### Comparing `utk_exodus-0.1.6/utk_exodus/__init__.py` & `utk_exodus-0.1.7/utk_exodus/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from .metadata import MetadataMapping
 from .risearch import ResourceIndexSearch
 from .finder import FileOrganizer
 from .curate import FileCurator
 from .validate import ValidateMigration
 from .fedora import FedoraObject
 from .controller import InterfaceController
+from .combine import ImportRefactor
+from .template import ImportTemplate
 from .restrict import Restrictions, RestrictionsSheet
 
 __all__ = [
     "FedoraObject",
     "FileCurator",
     "FileOrganizer",
+    "ImportRefactor",
+    "ImportTemplate",
     "InterfaceController",
     "MetadataMapping",
     "ResourceIndexSearch",
     "Restrictions",
     "RestrictionsSheet",
     "ValidateMigration",
 ]
```

### Comparing `utk_exodus-0.1.6/utk_exodus/config/samvera_default.yml` & `utk_exodus-0.1.7/utk_exodus/config/samvera_default.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/config/utk_dc.yml` & `utk_exodus-0.1.7/utk_exodus/config/utk_dc.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/config/utk_dc_no_uris.yml` & `utk_exodus-0.1.7/utk_exodus/config/utk_dc_no_uris.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/config/utk_no_uris_no_names.yml` & `utk_exodus-0.1.7/utk_exodus/config/utk_no_uris_no_names.yml`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/controller/controller.py` & `utk_exodus-0.1.7/utk_exodus/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,30 @@
     def __get_mods(collection, work_type):
         click.echo(click.style("Finding MODS files ...", fg="red", bold=True))
         risearch = ResourceIndexSearch().get_works_based_on_type_and_collection(
             work_type, collection
         )
         return risearch
 
-    def __grab_file_info(self):
-        click.echo(click.style("Grabbing file info ...", fg="yellow", bold=True))
-        x = FileOrganizer("tmp/works.csv", ["filesets", "attachments"], self.remote)
-        x.write_csv(f"{self.output}/{self.output.split('/')[-1]}.csv")
+    @staticmethod
+    def __get_m3():
         r = requests.get(
             "https://raw.githubusercontent.com/utkdigitalinitiatives/m3_profiles/main/maps/utk.yml"
         )
         with open("tmp/m3.yml", "wb") as f:
             f.write(r.content)
         return
 
+    def __grab_file_info(self):
+        click.echo(click.style("Grabbing file info ...", fg="yellow", bold=True))
+        x = FileOrganizer("tmp/works.csv", ["filesets", "attachments"], self.remote)
+        x.write_csv(f"{self.output}/{self.output.split('/')[-1]}.csv")
+        self.__get_m3()
+        return
+
     def __validate_import(self):
         click.echo(click.style("Validating import ...", fg="blue", bold=True))
         validator = ValidateMigration(
             profile="tmp/m3.yml",
             migration_sheet=f"{self.output}/{self.output.split('/')[-1]}.csv",
         )
         validator.iterate()
@@ -145,13 +150,14 @@
         shutil.rmtree("tmp/mods_downloads/current_collection")
         self.__download_policies(collection, work_type)
         self.__grab_file_info()
         self.restrict_files_and_works(
             f"{self.output}/{self.output.split('/')[-1]}.csv",
             "tmp/policy_downloads/current_collection",
         )
+        shutil.rmtree("tmp/policy_downloads/current_collection")
         self.__validate_import()
         self.__curate_filesets_and_attachments(
             f"{self.output}/{self.output.split('/')[-1]}_visibility.csv"
         )
         click.echo(click.style("Done ...", fg="cyan", bold=True))
         return
```

### Comparing `utk_exodus-0.1.6/utk_exodus/curate/curate.py` & `utk_exodus-0.1.7/utk_exodus/curate/curate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/fedora/fedora.py` & `utk_exodus-0.1.7/utk_exodus/fedora/fedora.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/finder/finder.py` & `utk_exodus-0.1.7/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/metadata/__init__.py` & `utk_exodus-0.1.7/utk_exodus/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.7/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.7/utk_exodus/metadata/metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,14 +53,26 @@
         # Retrieve text content based on the given xpath expression.
         return [
             element.text
             for element in self.root.xpath(xpath_expr, namespaces=self.namespaces)
         ]
 
     def find(self):
+        """
+        Handles the mapping of different types of titles based on the provided XML data.
+
+        Returns:
+            dict: A dictionary containing the mapped titles.
+
+        Example:
+             >>> titles = TitleProperty("tests/fixtures/utsmc_17870.xml", {"mods": "http://www.loc.gov/mods/v3"})
+             >>> titles.find()
+             ... #doctest: +NORMALIZE_WHITESPACE
+             {'title': ['Prussian heroes march'], 'alternative_title': ['Prussian heroes: Prussen helden march']}
+        """
         titles = []
         alternatives = []
         titles_data = self.various_titles
 
         # Handle supplied and plain titles mapping to dcterms:title and dcterms:alternative.
         if titles_data["supplied"] and titles_data["plain"]:
             titles.extend(titles_data["supplied"])
@@ -93,14 +105,25 @@
                 return [all_names]
             else:
                 return ["Problem"]
         else:
             return []
 
     def find(self):
+        """
+        Find all names and roles in the XML file.
+
+        Returns:
+            dict: A dictionary containing the roles and names.
+
+        Examples:
+            >>> roles_and_names = RoleAndNameProperty("tests/fixtures/harp_1.xml")
+            >>> roles_and_names.find()
+            {'utk_composer': ['Swan, W. H. (William H.)', 'Swan, Marcus Lafayette'], 'utk_compiler': ['Swan, W. H. (William H.)', 'Swan, Marcus Lafayette']}
+        """
         roles_and_names = {}
         for name in self.all_names:
             local_roles = []
             try:
                 local_roles.append(
                     f"utk_{name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_')}"
                 )
@@ -153,14 +176,25 @@
                 return [all_names]
             else:
                 return ['Problem']
         else:
             return []
 
     def find(self):
+        """
+        Find all names in the XML file.
+
+        Returns:
+            dict: A dictionary containing the names.
+
+        Examples:
+            >>> names = NameProperty("tests/fixtures/harp_1.xml")
+            >>> names.find()
+            {'composer': ['http://id.loc.gov/authorities/names/no2002022963', 'http://id.loc.gov/authorities/names/n78013127'], 'compiler': ['http://id.loc.gov/authorities/names/no2002022963', 'http://id.loc.gov/authorities/names/n78013127']}
+        """
         roles_and_names = {}
         for name in self.all_names:
             roles = []
             local_roles = []
             try:
                 roles.append(name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_'))
                 local_roles.append(f"utk_{name['mods:role']['mods:roleTerm']['#text'].lower().replace(' ', '_')}")
@@ -207,18 +241,42 @@
                     roles_and_names[role] = [name_value]
                 elif not name_value.startswith('http'):
                     roles_and_names[role].append(name_value)
         return roles_and_names
 
 
 class GeoNamesProperty(BaseProperty):
+    """
+    Handles the mapping of different types of geonames based on the provided XML data.
+
+    Args:
+        path (str): The path to the XML file.
+        namespaces (dict): A dictionary containing the namespaces used in the XML file.
+    """
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self, name):
+        """
+        Find all geonames in the XML file.
+
+        Args:
+            name (str): The name of the geoname.
+
+        Returns:
+            dict: A dictionary containing the geoname mappings.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> geonames = GeoNamesProperty("tests/fixtures/webster_1127.xml", NAMESPACES)
+            >>> geonames.find("spatial")
+            {'spatial': ['http://sws.geonames.org/4050810', 'http://sws.geonames.org/4609260', 'http://id.loc.gov/authorities/subjects/sh85057008']}
+        """
         uris = [
             uri.replace("about.rdf", "")
             for uri in self.root.xpath(
                 "mods:subject/mods:geographic/@valueURI", namespaces=self.namespaces
             )
         ]
         lc_uris = [
@@ -263,14 +321,28 @@
                     "University of Tennessee, Knoxville. Special Collections"
                 )
             else:
                 all_repositories.append(value)
         return all_repositories
 
     def find(self):
+        """
+        Find all locations properties in the XML file.
+
+        Returns:
+            dict: A dictionary containing location properties.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> physical_location = PhysicalLocationsProperties("tests/fixtures/civilwar_1438.xml", NAMESPACES)
+            >>> physical_location.find()
+            {'repository': ['University of Tennessee, Knoxville. Special Collections'], 'archival_collection': ['O. P. Temple Papers,1862']}
+        """
         return {
             "repository": self.__find_repositories(),
             "archival_collection": self.__find_archival_collections(),
         }
 
     def __find_archival_collections(self):
         all_archival_collections = []
@@ -314,14 +386,28 @@
 
 
 class DataProvider(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all data providers in the XML file.
+
+        Returns:
+            dict: A dictionary containing data provider information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> dataProvider = DataProvider("tests/fixtures/egypt_224.xml", NAMESPACES)
+            >>> dataProvider.find()
+            {'provider': ['University of Tennessee, Knoxville. Libraries'], 'intermediate_provider': ['Frank H. McClung Museum of Natural History and Culture']}
+        """
         values = [
             value.text
             for value in self.root.xpath(
                 "mods:recordInfo/mods:recordContentSource", namespaces=self.namespaces
             )
         ]
         return {
@@ -335,14 +421,28 @@
 
 
 class MachineDate(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all machine date information in the XML file.
+
+        Returns:
+            dict: A dictionary containing machine date information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> machineDate = MachineDate("tests/fixtures/volvoices_2993.xml", NAMESPACES)
+            >>> machineDate.find()
+            {'date_created_d': ['1948-01'], 'date_issued_d': ['1948'], 'date_other_d': []}
+        """
         date_created = [
             value.text
             for value in self.root.xpath(
                 'mods:originInfo/mods:dateCreated[@encoding="edtf"]',
                 namespaces=self.namespaces,
             )
         ]
@@ -472,14 +572,28 @@
 
 
 class TypesProperties(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all types properties information in the XML file.
+
+        Returns:
+            dict: A dictionary containing types properties information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> types = TypesProperties("tests/fixtures/utsmc_17870.xml", NAMESPACES)
+            >>> types.find()
+            {'form': ['http://vocab.getty.edu/aat/300026430'], 'resource_type': ['http://id.loc.gov/vocabulary/resourceTypes/not', 'http://id.loc.gov/vocabulary/resourceTypes/txt'], 'form_local': []}
+        """
         return {
             "form": self.__find_edm_has_type(),
             "resource_type": self.__find_dcterms_type(),
             "form_local": self.__find_local_form(),
         }
 
     def __find_dcterms_type(self):
@@ -613,14 +727,28 @@
 
 
 class LocalTypesProperties(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all local types properties information in the XML file.
+
+        Returns:
+            dict: A dictionary containing local types properties information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> local_types = LocalTypesProperties("tests/fixtures/egypt_224.xml", NAMESPACES)
+            >>> local_types.find()
+            {'resource_type_local': ['still image'], 'form_local': ['platinum prints']}
+        """
         return {
             "resource_type_local": self.__find_dcterms_type(),
             "form_local": self.__find_local_form(),
         }
 
     def __find_dcterms_type(self):
         genre_uris = {
@@ -732,14 +860,28 @@
 
 
 class PublisherProperty(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all publisher property information in the XML file.
+
+        Returns:
+            dict: A dictionary containing publisher property information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> publisher = PublisherProperty("tests/fixtures/playbills:1052.xml", NAMESPACES)
+            >>> publisher.find()
+            {'publisher': []}
+        """
         return {
             "publisher": [
                 uri
                 for uri in self.root.xpath(
                     "mods:originInfo/mods:publisher/@valueURI",
                     namespaces=self.namespaces,
                 )
@@ -748,14 +890,28 @@
 
 
 class RightsOrLicenseProperties(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all rights or liscense property information in the XML file.
+
+        Returns:
+            dict: A dictionary containing rights or license property information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> rights = RightsOrLicenseProperties("tests/fixtures/heilman:1010.xml", NAMESPACES)
+            >>> rights.find()
+            {'license': ['http://creativecommons.org/licenses/by-nc-nd/3.0/'], 'rights_statement': ['http://rightsstatements.org/vocab/InC/1.0/']}
+        """
         final = {}
         rights = [
             uri
             for uri in self.root.xpath(
                 'mods:accessCondition[not(@type="restriction on access")]/@xlink:href',
                 namespaces=self.namespaces,
             )
@@ -786,14 +942,28 @@
 
 
 class PublicationPlaceProperty(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find(self):
+        """
+        Find all publication place property information in the XML file.
+
+        Returns:
+            dict: A dictionary containing publication place property information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> publication_place = PublicationPlaceProperty("tests/fixtures/volvoices_2495.xml", NAMESPACES)
+            >>> publication_place.find()
+            {'publication_place': ['http://id.loc.gov/authorities/names/n82063401']}
+        """
         return {
             "publication_place": [
                 uri
                 for uri in self.root.xpath(
                     "mods:originInfo/mods:place/mods:placeTerm/@valueURI",
                     namespaces=self.namespaces,
                 )
@@ -802,14 +972,28 @@
 
 
 class LanguageURIProperty(BaseProperty):
     def __init__(self, path, namespaces):
         super().__init__(path, namespaces)
 
     def find_term(self):
+        """
+        Find all language URI properties in the XML file.
+
+        Returns:
+            dict: A dictionary containing language URI property information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> language_uri = LanguageURIProperty("tests/fixtures/utsmc:725.xml", NAMESPACES)
+            >>> language_uri.find_term()
+            {'language': ['http://id.loc.gov/vocabulary/iso639-2/fre', 'http://id.loc.gov/vocabulary/iso639-2/ita']}
+        """
         terms_and_uris = {
             "English": "http://id.loc.gov/vocabulary/iso639-2/eng",
             "French": "http://id.loc.gov/vocabulary/iso639-2/fre",
             "German": "http://id.loc.gov/vocabulary/iso639-2/ger",
             "Italian": "http://id.loc.gov/vocabulary/iso639-2/ita",
             "Latin": "http://id.loc.gov/vocabulary/iso639-2/lat",
             "No linguistic content": "http://id.loc.gov/vocabulary/iso639-2/zxx",
@@ -828,19 +1012,40 @@
         for language in language_terms:
             if language in terms_and_uris:
                 lanuage_uris.append(terms_and_uris[language])
         return {"language": lanuage_uris}
 
 
 class ExtentProperty(BaseProperty):
+    """
+    Class to Handle Extent Information.
+
+    Args:
+        path (str): The path to the file.
+        namespaces (dict): Namespaces to be used in the XPath queries.
+    """
     def __init__(self, path: str, namespaces: dict):
         super().__init__(path, namespaces)
 
     def find(self):
-        """Finds and returns a dictionary containing the extent information of a record."""
+        """
+        Finds and returns a dictionary containing the extent information of a record.
+
+        Returns:
+            dict: A dictionary containing the extent information.
+
+        Examples:
+            >>> NAMESPACES = {
+            ... 'mods': 'http://www.loc.gov/mods/v3', 
+            ... 'xlink': 'http://www.w3.org/1999/xlink' }
+            >>> extent_property = ExtentProperty("tests/fixtures/knoxgardens_125.xml", NAMESPACES)
+            >>> extent_property.find()
+            {'extent': ['3 1/4 x 5 inches']}
+
+        """
         extents_without_units = [
             text.text
             for text in self.root.xpath(
                 "mods:physicalDescription/mods:extent[not(@unit)]",
                 namespaces=self.namespaces,
             )
         ]
@@ -977,47 +1182,49 @@
             "Pdf": "https://ontology.lib.utk.edu/works#PDFWork",
             "Video": "https://ontology.lib.utk.edu/works#VideoWork",
         }
         return ontology_values[model]
 
     @staticmethod
     def __lookup_special_property(special_property, file, namespaces, name):
-        match special_property:
-            case "TitleProperty":
-                return TitleProperty(file, namespaces).find()
-            case "NameProperty":
-                return NameProperty(file).find()
-            case "RoleAndNameProperty":
-                return RoleAndNameProperty(file).find()
-            case "GeoNamesProperty":
-                return GeoNamesProperty(file, namespaces).find(name)
-            case "DataProvider":
-                return DataProvider(file, namespaces).find()
-            case "PhysicalLocationsProperties":
-                return PhysicalLocationsProperties(file, namespaces).find()
-            case "SubjectProperty":
-                return SubjectProperty(file, namespaces).find_topic()
-            case "KeywordProperty":
-                return KeywordProperty(file, namespaces).find_topic()
-            case "TypesProperties":
-                return TypesProperties(file, namespaces).find()
-            case "LocalTypesProperties":
-                return LocalTypesProperties(file, namespaces).find()
-            case "LanguageURIProperty":
-                return LanguageURIProperty(file, namespaces).find_term()
-            case "PublisherProperty":
-                return PublisherProperty(file, namespaces).find()
-            case "PublicationPlaceProperty":
-                return PublicationPlaceProperty(file, namespaces).find()
-            case "RightsOrLicenseProperties":
-                return RightsOrLicenseProperties(file, namespaces).find()
-            case "ExtentProperty":
-                return ExtentProperty(file, namespaces).find()
-            case "MachineDate":
-                return MachineDate(file, namespaces).find()
+        if special_property == "TitleProperty":
+            return TitleProperty(file, namespaces).find()
+        elif special_property == "NameProperty":
+            return NameProperty(file).find()
+        elif special_property == "RoleAndNameProperty":
+            return RoleAndNameProperty(file).find()
+        elif special_property == "GeoNamesProperty":
+            return GeoNamesProperty(file, namespaces).find(name)
+        elif special_property == "DataProvider":
+            return DataProvider(file, namespaces).find()
+        elif special_property == "PhysicalLocationsProperties":
+            return PhysicalLocationsProperties(file, namespaces).find()
+        elif special_property == "SubjectProperty":
+            return SubjectProperty(file, namespaces).find_topic()
+        elif special_property == "KeywordProperty":
+            return KeywordProperty(file, namespaces).find_topic()
+        elif special_property == "TypesProperties":
+            return TypesProperties(file, namespaces).find()
+        elif special_property == "LocalTypesProperties":
+            return LocalTypesProperties(file, namespaces).find()
+        elif special_property == "LanguageURIProperty":
+            return LanguageURIProperty(file, namespaces).find_term()
+        elif special_property == "PublisherProperty":
+            return PublisherProperty(file, namespaces).find()
+        elif special_property == "PublicationPlaceProperty":
+            return PublicationPlaceProperty(file, namespaces).find()
+        elif special_property == "RightsOrLicenseProperties":
+            return RightsOrLicenseProperties(file, namespaces).find()
+        elif special_property == "ExtentProperty":
+            return ExtentProperty(file, namespaces).find()
+        elif special_property == "MachineDate":
+            return MachineDate(file, namespaces).find()
+        else:
+            # Handle unknown special property
+            raise ValueError(f"Unknown special property: {special_property}")
 
     def write_csv(self, filename):
         with open(filename, "w", newline="") as bulkrax_sheet:
             writer = csv.DictWriter(
                 bulkrax_sheet, fieldnames=self.fieldnames, quoting=csv.QUOTE_MINIMAL
             )
             writer.writeheader()
```

### Comparing `utk_exodus-0.1.6/utk_exodus/restrict/restrict.py` & `utk_exodus-0.1.7/utk_exodus/restrict/restrict.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.7/utk_exodus/risearch/risearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         return all_pages
 
     @staticmethod
     def __lookup_work_type(work_type):
         work_types = {
             "book": "info:fedora/islandora:bookCModel",
             "image": "info:fedora/islandora:sp_basic_image",
+            "large_image": "info:fedora/islandora:sp_large_image_cmodel",
             "compound": "info:fedora/islandora:compoundCModel",
             "audio": "info:fedora/islandora:sp-audioCModel",
             "video": "info:fedora/islandora:sp_videoCModel",
             "pdf": "info:fedora/islandora:sp_pdf",
             "page": "info:fedora/islandora:pageCModel",
         }
         return work_types.get(work_type, "unknown")
@@ -223,12 +224,30 @@
             all_policies_from_book = []
             books = [result for result in results.split("\n") if result != "" and result != '"pid"']
             for book in books:
                 all_policies_from_book.append(book)
                 all_policies_from_book.extend(self.get_policies_for_pages_in_book(book))
             return all_policies_from_book
 
+    def get_parent_book(self, pid):
+        query = quote(
+            f"SELECT ?book FROM <#ri> WHERE {{"
+            f"<info:fedora/{pid}> <http://islandora.ca/ontology/relsext#isPageOf> ?book ."
+            f"}}"
+        )
+        results = requests.get(f"{self.base_url}&query={query}").content.decode("utf-8")
+        return results.split("\n")[1]
+
+    def get_page_number(self, pid):
+        query = quote(
+            f"SELECT ?page FROM <#ri> WHERE {{"
+            f"<info:fedora/{pid}> <http://islandora.ca/ontology/relsext#isPageNumber> ?page ."
+            f"}}"
+        )
+        results = requests.get(f"{self.base_url}&query={query}").content.decode("utf-8")
+        return results.split("\n")[1]
+
 
 if __name__ == "__main__":
     risearch = ResourceIndexSearch()
     x = risearch.get_policies_based_on_type_and_collection("book", "collections:galston")
     print(x)
```

### Comparing `utk_exodus-0.1.6/utk_exodus/validate/validate.py` & `utk_exodus-0.1.7/utk_exodus/validate/validate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.6/PKG-INFO` & `utk_exodus-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utk-exodus
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool for building import sheets from UTK legacy systems
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -82,14 +82,26 @@
 
 If for some reason you need to create a files sheet for  works after the fact, use:
 
 ```shell
 exodus add_files --sheet path/to/sheet.csv --files_sheet path/to/files_sheet.csv 
 ```
 
+If you need to remove unused values from an import or work sheet, you can:
+
+```shell
+exodus remove_old_values --sheet path/to/sheet.csv --old_sheet path/to/old_sheet.csv --new_sheet path/to/new_sheet.csv
+```
+
+If you want to generate a full template for a metadata import, use:
+
+```shell
+exodus generate_template --model book -o /path/to/sheet.csv
+```
+
 ## What's Missing Here Right Now
 
 * The ability to create pcdm:Collection objects.
 * The ability to create a new metadata import from a previous import
 
 ## Understanding Configs
```

