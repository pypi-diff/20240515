# Comparing `tmp/almirah-0.3.0.tar.gz` & `tmp/almirah-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almirah-0.3.0.tar", max compression
+gzip compressed data, was "almirah-0.4.0.tar", max compression
```

## Comparing `almirah-0.3.0.tar` & `almirah-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1072 2024-04-22 22:37:55.424893 almirah-0.3.0/LICENSE
--rw-r--r--   0        0        0      963 2024-04-22 22:37:55.424893 almirah-0.3.0/README.md
--rw-r--r--   0        0        0      335 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/__init__.py
--rw-r--r--   0        0        0     5268 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/configs/bids.yaml
--rw-r--r--   0        0        0      119 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/__init__.py
--rw-r--r--   0        0        0     1829 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/base.py
--rw-r--r--   0        0        0     1079 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/db.py
--rw-r--r--   0        0        0     3213 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/uniquify.py
--rw-r--r--   0        0        0    18179 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/database.py
--rw-r--r--   0        0        0     3557 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/dataset.py
--rw-r--r--   0        0        0     2479 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/indexer.py
--rw-r--r--   0        0        0     8541 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/layout.py
--rw-r--r--   0        0        0    12416 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/specification.py
--rw-r--r--   0        0        0        0 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/__init__.py
--rw-r--r--   0        0        0     8117 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/convert.py
--rw-r--r--   0        0        0     2363 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/df.py
--rw-r--r--   0        0        0     3611 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/gen.py
--rw-r--r--   0        0        0     1766 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/lib.py
--rw-r--r--   0        0        0     1648 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/logging.py
--rw-r--r--   0        0        0     1471 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/sqlalchemy.py
--rw-r--r--   0        0        0     1086 2024-04-22 22:37:55.428892 almirah-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 almirah-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 19:34:47.916747 almirah-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1023 2024-05-15 19:34:47.916747 almirah-0.4.0/README.md
+-rw-r--r--   0        0        0      335 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/core/__init__.py
+-rw-r--r--   0        0        0     1829 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/core/base.py
+-rw-r--r--   0        0        0      950 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/core/db.py
+-rw-r--r--   0        0        0     3213 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/core/uniquify.py
+-rw-r--r--   0        0        0    20725 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/database.py
+-rw-r--r--   0        0        0     3839 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/dataset.py
+-rw-r--r--   0        0        0     2479 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/indexer.py
+-rw-r--r--   0        0        0     9062 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/layout.py
+-rw-r--r--   0        0        0    12416 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/specification.py
+-rw-r--r--   0        0        0      167 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/__init__.py
+-rw-r--r--   0        0        0     8146 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/convert.py
+-rw-r--r--   0        0        0     2978 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/df.py
+-rw-r--r--   0        0        0     3672 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/gen.py
+-rw-r--r--   0        0        0     2286 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/lib.py
+-rw-r--r--   0        0        0     1648 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/logging.py
+-rw-r--r--   0        0        0     1474 2024-05-15 19:34:47.916747 almirah-0.4.0/almirah/utils/sqlalchemy.py
+-rw-r--r--   0        0        0     1228 2024-05-15 19:34:47.924747 almirah-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 almirah-0.4.0/PKG-INFO
```

### Comparing `almirah-0.3.0/LICENSE` & `almirah-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/README.md` & `almirah-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 <br />
 <div align="center">
 
   <h3 align="center">almirah</h3>
 
   <p align="center">
-	a wardrobe for datasets
 	<br />
 	<a href="https://girishmm.github.io/almirah"><strong>Explore the docs »</strong></a>
 	<br />
 	<br />
 	<a href="https://github.com/girishmm/almirah/issues">Report Bug</a>
 	·
 	<a href="https://github.com/girishmm/almirah/issues">Request Feature</a>
   </p>
 </div>
 
 ## About The Project
 
-Clothes can be organized, maintained, and easily accessed from a
-wardrobe. [almirah](https://github.com/girishmm/almirah) serves the
-same purpose for datasets.
-
-You can define the method to follow to stack your contents on the
-almirah, and even tag. [almirah](https://github.com/girishmm/almirah)
-hopes to make working with datasets easier.
+[almirah](https://github.com/girishmm/almirah) is designed to help
+organize, maintain, and access datasets efficiently. It provides tools
+for defining how data is stored, tagged, and retrieved, making it
+easier to work with complex data collections.
+
+For more information on how to use
+[almirah](https://github.com/girishmm/almirah) for your data projects,
+please see the [documentation](https://girishmm.github.io/almirah/).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Acknowledgments
 
 Thanks to Upi and Bhalla lab members for their inputs and help.
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 
                                ******** aallmmiirraahh ********
-                           a wardrobe for datasets
+
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
-## About The Project Clothes can be organized, maintained, and easily accessed
-from a wardrobe. [almirah](https://github.com/girishmm/almirah) serves the same
-purpose for datasets. You can define the method to follow to stack your
-contents on the almirah, and even tag. [almirah](https://github.com/girishmm/
-almirah) hopes to make working with datasets easier.
+## About The Project [almirah](https://github.com/girishmm/almirah) is designed
+to help organize, maintain, and access datasets efficiently. It provides tools
+for defining how data is stored, tagged, and retrieved, making it easier to
+work with complex data collections. For more information on how to use
+[almirah](https://github.com/girishmm/almirah) for your data projects, please
+see the [documentation](https://girishmm.github.io/almirah/).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments Thanks to Upi and Bhalla lab members for their inputs and
 help.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `almirah-0.3.0/almirah/core/base.py` & `almirah-0.4.0/almirah/core/base.py`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/almirah/core/db.py` & `almirah-0.4.0/almirah/core/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,15 @@
     """Manages database connections and sessions."""
 
     Session = None
 
     def __init__(self, url: str):
         self.engine = create_engine(url)
         self.metadata = MetaData()
-        self.reflect()
-
-    def reflect(self) -> None:
-        """Reflects the database schema into metadata."""
-        self.metadata = self.metadata.reflect(bind=self.engine)
+        self.metadata.reflect(bind=self.engine)
 
     @property
     def connection(self) -> Connection:
         """Provides a context-managed connection to the database."""
         return self.engine.connect()
 
     @property
```

### Comparing `almirah-0.3.0/almirah/core/uniquify.py` & `almirah-0.4.0/almirah/core/uniquify.py`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/almirah/database.py` & `almirah-0.4.0/almirah/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Database functionality for data write and access."""
 
 import logging
+import requests
 import numpy as np
 import pandas as pd
 
 from sqlalchemy import URL
 from sqlalchemy import Table
 from sqlalchemy import Column
 from sqlalchemy import ForeignKey
@@ -17,16 +18,19 @@
 from .core import uniquify
 from .core import DBManager
 from .indexer import index
 from .dataset import Component
 
 from .utils.df import common_rows
 from .utils.df import convert_column_type
+from .utils.df import python_to_pandas_type
+
 from .utils.logging import log_df
 from .utils.logging import log_col
+
 from .utils.sqlalchemy import get_sql_type
 
 
 @uniquify(index)
 class Database(Component):
     """Generic database representation."""
 
@@ -44,24 +48,46 @@
     def __init__(self, *, name, host, backend):
         self.name = name
         self.host = host
         self.backend = backend
 
     @property
     def connection(self):
-        if not self.db:
+        if self.backend in ["request", "gsheet"]:
+            raise TypeError("Connection only permissible in connection mode")
+
+        if not getattr(self, "db", None):
             raise TypeError(f"Connection to {self} not established")
         return self.db.connection
 
     @property
-    def meta(self):
-        if not self.db:
+    def worksheet(self):
+        if self.backend != "gsheet":
+            raise TypeError("Worksheet only permissible in google sheets mode")
+
+        if not getattr(self, "client"):
             raise TypeError(f"Connection to {self} not established")
+
+    @property
+    def meta(self):
+        if self.backend in ["request", "gsheet"]:
+            raise TypeError("Metadata only permissible in connection mode")
+
+        if not getattr(self, "db"):
+            raise ValueError(f"Connection to {self} not established")
         return self.db.metadata
 
+    @property
+    def token(self):
+        if self.backend != "request":
+            raise TypeError("Token only permissible in request mode")
+
+        if not getattr(self, "_token"):
+            raise TypeError(f"Connection to {self} not established")
+
     def build_column(self, name, dtype, **kwargs):
         """Build SQLalchemy Column object given column description."""
         primary = kwargs.get("primary", False)
         fk = [ForeignKey(f)] if (f := kwargs.get("refs")) else []
         return Column(name, get_sql_type(dtype), *fk, primary_key=primary)
 
     def build_constraint(self, cols, links):
@@ -82,39 +108,60 @@
             List of table constraints.
         """
         cls = [self.build_column(**c) for c in cols]
         cns = [self.build_constraint(**r) for r in refs]
         table = Table(table, self.meta, *cls, *cns, extend_existing=True)
         table.create(bind=self.connection, checkfirst=True)
 
-    def connect(self, username, password):
+    def connect(self, username=None, password=None, keyfile=None):
         """
         Establish a connection to the database.
 
         Parameters
         ----------
         username : str
             The database username.
         password : str
             The database password.
+        keyfile : str
+            Path to the service account keyfile. Required if backend is gsheet.
 
         Raises
         ------
         SQLAlchemyError
-            If the connection cannot be established.
+            If the connection cannot be established at database.
+        ValueError
+            If the connection cannot be established at URL endpoint.
         """
-        url = URL.create(
-            self.backend,
-            username=username,
-            password=password,
-            host=self.host,
-            database=self.name,
-        )
 
-        self.db = DBManager(url)
+        if self.backend == "request":
+            data = {"username": username, "password": password}
+            response = requests.post(f"{self.host}authenticate/", data=data).json()
+
+            if "error" in response:
+                raise ValueError(response["error"])
+
+            self._token = response["token"]
+
+        elif self.backend == "gsheet":
+            import gspread
+
+            self._client = gspread.service_account(keyfile)
+            self.spreadsheet = self._client.open_by_url(self.host)
+
+        else:
+            url = URL.create(
+                self.backend,
+                username=username,
+                password=password,
+                host=self.host,
+                database=self.name,
+            )
+
+            self.db = DBManager(url)
 
     def get_primary(self, table):
         """Return priamry keys for table."""
 
         return [c.name for c in self.meta.tables[table].primary_key]
 
     def get_records(self, table, cols=None):
@@ -123,15 +170,37 @@
         Parameters
         ----------
         table : str
             Table in database from which to retrieve records.
         cols : list of str
             Column names to select from table.
         """
-        return pd.read_sql_table(table, self.connection, columns=cols)
+        if self.backend == "request":
+            data = {"table": table, "cols": cols}
+            header = {"Authorization": f"Bearer {self.token}"}
+            response = requests.post(self.host, data=data, headers=header)
+            records = pd.DataFrame(response.json())
+
+        elif self.backend == "gsheet":
+            data = self.spreadsheet.worksheet(table).get_all_values()
+            headers = data.pop(0)
+            records = pd.DataFrame(data, columns=headers)
+
+            if cols:
+                records = records[cols]
+
+        else:
+            dtype = {}
+            for column in self.meta.tables[table].columns:
+                generic_type = column.type.as_generic()
+                dtype[column.name] = python_to_pandas_type(generic_type.python_type)
+            records = pd.read_sql_table(table, self.connection, columns=cols)
+            records = records.astype(dtype)
+
+        return records
 
     def to_table(
         self,
         df,
         table,
         check_dups=True,
         resolve_dups=False,
@@ -322,15 +391,18 @@
     def query(self, returns=None, **filters):
         """Return table records that fit filter criteria."""
         table = filters.pop("table", None)
         if not table:
             return None
 
         df = self.get_records(table, returns)
-        df = df[np.logical_and.reduce([df[k] == v for k, v in filters.items()])]
+
+        if filters:
+            df = df[np.logical_and.reduce([df[k] == v for k, v in filters.items()])]
+
         return df
 
     def __repr__(self):
         return f"<Database url: '{self.backend}:{self.name}@{self.host}'>"
 
 
 def check_for_key(key, mapping):
@@ -436,27 +508,27 @@
     if len(result) > 1:
         logging.error(f"Non-unique mappings for value '{value}' in {file}")
         return
 
     return result.at[0, mapping]
 
 
-def replace_column(series, column, mapping, file, strict=True):
+def replace_column(series, value, to, file, strict=True):
     """Replace values in series based on mapping in file."""
 
     # Load file into dataframe
     df = pd.read_csv(file, dtype=str)
-    logging.info(f"Replacing values in '{column}' with '{mapping}' from {file}")
+    mapping = pd.Series(df[to].values, index=df[value].values)
+    logging.info(f"Replacing values in '{value}' with '{to}' from {file}")
 
     # Stop if non-unique mappings
-    if df.duplicated([column]).any():
+    if df.duplicated([value]).any():
         raise ValueError(f"Non-unique mappings found in file {file}")
 
-    df = pd.Series(df[mapping], index=df[column])
-    replaced = series.map(df)
+    replaced = series.map(mapping)
 
     # Retain original value if replacement not strict
     if not strict:
         replaced.fillna(series, inplace=True)
 
     return replaced
 
@@ -485,19 +557,19 @@
     s, error = series.copy(deep=True), series.isna()
 
     if pat := kwargs.get("extract"):
         s = s.astype(str).str.extract(pat, expand=False)
         logging.info(f"Extracting and replacing based on pattern {pat}")
 
     if rep := kwargs.get("replace"):
-        if "field" in rep:
-            replace_column(s, **rep)
+        if "file" in rep:
+            s = replace_column(s, **rep)
             logging.info("Replacing values with mapping in external file")
         else:
-            s = s.replace({k["value"]: k["with"] for k in rep})
+            s = s.replace({k["value"]: k["to"] for k in rep})
             logging.info("Replacing values with given in config")
 
     if ca := kwargs.get("case"):
         s = s.str.upper() if ca == "upper" else s.str.lower()
         logging.info(f"Changing case to {ca}")
 
     s = convert_column_type(s, kwargs["dtype"], **dtype_kws)
```

### Comparing `almirah-0.3.0/almirah/dataset.py` & `almirah-0.4.0/almirah/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ Model classes to represent a dataset and its components."""
 
-from typing import Set
+import pandas as pd
+
 from typing import List
 from typing import Optional
 
 from sqlalchemy import ForeignKey
 
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm import mapped_column
 
 from .core import Base
 from .core import uniquify
-
 from .indexer import index
 
 
 class Component(Base):
     """Generic component representation within the dataset architecture."""
 
     __tablename__ = "components"
@@ -35,15 +35,15 @@
     """Represents a collection of components as a dataset."""
 
     __tablename__ = "datasets"
     __identifier_attrs__ = {"name"}
 
     id: Mapped[int] = mapped_column(ForeignKey("components.id"), primary_key=True)
     name: Mapped[str] = mapped_column(unique=True, nullable=False)
-    components: Mapped[Set["Component"]] = relationship(secondary="collections")
+    components: Mapped[List["Component"]] = relationship(secondary="collections")
 
     __mapper_args__ = {"polymorphic_identity": "dataset"}
 
     def __init__(self, *, name: str) -> None:
         self.name = name
 
     def add(self, *components: Component) -> None:
@@ -59,15 +59,22 @@
         ------
         TypeError
             If a dataset is added to itself or circular references are detected.
         """
         if any(c == self or self in getattr(c, "components", []) for c in components):
             raise TypeError("Dataset cannot include itself as a component")
 
-        self.components.update(components)
+        self.components.extend(components)
+
+    def index(self, **kwargs):
+        """Perform indexing on components."""
+
+        for c in self.components:
+            if index := callable(getattr(c, "index")):
+                index(c, **kwargs)
 
     def report(self) -> None:
         """Generate report for dataset."""
         print(f"Components of {self}:")
 
         for c in self.components:
             print("{!r:5}".format(c))
@@ -87,18 +94,25 @@
             Filter conditions to apply on the query.
 
         Returns
         -------
         list
             List of components or queried data meeting the filter criteria.
         """
-        results = [r for c in self.components if (r := c.query(returns, **filters))]
-        if "table" in filters and results:
-            return results[0]
-        return [i for result in results for i in result]
+        results = list()
+        for c in self.components:
+            result = c.query(returns, **filters)
+
+            if isinstance(result, pd.DataFrame) and not result.empty:
+                return result
+
+            if result:
+                results.extend(result)
+
+        return results
 
     def __repr__(self) -> str:
         return f"<Dataset name: '{self.name}'>"
 
 
 class Collection(Base):
     """
```

### Comparing `almirah-0.3.0/almirah/indexer.py` & `almirah-0.4.0/almirah/indexer.py`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/almirah/layout.py` & `almirah-0.4.0/almirah/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,18 @@
             raise TypeError(f"Found file outside layout scope of {self.root}")
         self.files.extend(files)
 
     def clone(self, url=None):
         """Clone Layout from datalad url."""
         if not self.url and not url:
             raise ValueError(f"Remote url for {self} not set")
-        self.url = url
+
+        if not self.url:
+            self.url = url
+
         clone(source=self.url, path=self.root)
 
     def index(self, root=None, metadata=False, valid_only=True, reset=False, **funcs):
         """Perform indexing to add files in root to index."""
 
         # Start from scratch if reset set
         if reset:
@@ -126,18 +129,14 @@
                 self.index(path, metadata, valid_only, reset, **funcs)
 
             if path_valid:
                 file = File(path=path)
                 self.add(file)
                 file.index(metadata, reset, **funcs)
 
-    def report(self):
-        """Generate report for the Layout."""
-        pass
-
     def query(self, returns="file", **filters):
         """Return File instances that fit filter criteria."""
 
         if not returns:
             returns = "file"
 
         filters = listify(filters)
@@ -145,15 +144,15 @@
         # Combine table for consolidated view
         combine = select(File).join(Marking).join(Tag)
 
         # Dynamically add conditions for filtering
         conditions = [and_(Tag.name == n, Tag.value.in_(v)) for n, v in filters.items()]
 
         # Combine conditions using AND to find matches
-        match = combine.where(or_(*conditions))
+        match = combine.where(File.root == self.root).where(or_(*conditions))
 
         # Trim down matches to only those that have all mentioned tags
         trim = match.group_by(File).having(func.count(Tag.name) == len(filters))
 
         # Retrieve File objects
         files = index.retrieve(trim).all()
 
@@ -162,16 +161,29 @@
 
         elif returns == "path":
             return [f.path for f in files]
 
         elif returns == "rel_path":
             return [f.rel_path for f in files]
 
+        returns = [returns] if isinstance(returns, str) else returns
         return [[f.tags.get(t) for t in returns] for f in files]
 
+    def move_root(self, path):
+        """Abstractly move Layout and its entries to path."""
+        for file in self.files:
+            file.path = os.path.join(path, file.rel_path)
+            file.root = path
+
+        self.root = path
+
+    def report(self):
+        """Generate report for the Layout."""
+        pass
+
     def __repr__(self):
         return f"<Layout root: '{self.root}'>"
 
 
 @uniquify(index)
 class File(Base):
     """Generic file representation."""
@@ -200,21 +212,27 @@
     @property
     def attached(self):
         return True if self.layout else False
 
     @property
     def rel_path(self):
         if not self.attached:
-            raise TypeError("File not attached to a Layout")
+            raise TypeError(f"{self} not attached to a Layout")
         return os.path.relpath(self.path, self.root)
 
     def download(self):
         """Download file from remote dataset."""
-        if self.attached and self.layout.url:
-            get(self.path, dataset=self.layout.root)
+
+        if not self.attached:
+            raise TypeError(f"{self} not attached to a Layout")
+
+        if not self.layout.url:
+            raise ValueError(f"Remote url for {self.layout} not set")
+
+        get(self.path, dataset=self.layout.root)
 
     def index(self, metadata=False, reset=False, **funcs):
         """Perform indexing to add tags marking the file to index."""
 
         # Start from scratch if reset set
         if reset:
             self.tags = {}
```

### Comparing `almirah-0.3.0/almirah/specification.py` & `almirah-0.4.0/almirah/specification.py`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/almirah/utils/convert.py` & `almirah-0.4.0/almirah/utils/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """File format conversion utility functions."""
 
 import os
-import mne
 import shlex
 import logging
-import mne_bids
-import mne_nirs
 
 from .gen import run_shell
 
 
 def dcm2nii(files, out, dst, **kwargs):
     """
     Convert DICOM files to NIfTI and write to disk.
@@ -118,14 +115,17 @@
         logging.info(f"Converted {file.path} and stored to {new_path}")
     logging.info("Conversion to asc complete")
 
 
 def nirx2snirf(files, out, dst, **kwargs):
     """Convert NIRS data format and write to disk."""
 
+    import mne
+    import mne_nirs
+
     for file in files:
         raw = mne.io.read_raw_nirx(file.path)
         raw.anonymize(**kwargs.get("anonymize", {}))
         new_path = os.path.join(
             dst,
             file.build_modified_path(
                 extension="snirf",
@@ -137,14 +137,17 @@
         logging.info(f"Converted {file.path} and stored to {new_path}")
     logging.info("Conversion to snirf complete")
 
 
 def eeg_converter(files, out, dst, **kwargs):
     """Convert EEG data format and write to disk."""
 
+    import mne
+    import mne_bids
+
     # Set conversion logging level
     verbose = kwargs.get("logging", "INFO")
 
     # Set power line frequency to default if not provided
     line_freq = kwargs.get("line_freq", 50)
     logging.info(f"Using value of {line_freq} Hz for power line frequency")
```

### Comparing `almirah-0.3.0/almirah/utils/df.py` & `almirah-0.4.0/almirah/utils/df.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,56 @@
 """Dataframe manipulation utility functions."""
 
 import pandas as pd
 
 from typing import Any
 
+from datetime import date
+from datetime import datetime
+
 from .lib import extract_dtype_from_db_type_string
 
 
+def common_rows(
+    child: pd.DataFrame,
+    parent: pd.DataFrame,
+    child_on: Any = None,
+    parent_on: Any = None,
+) -> pd.Series:
+    """
+    Return boolean mask where True if record common in Child and Parent.
+
+    Parameters
+    ----------
+    child : pd.DataFrame
+        The child dataframe.
+    parent : pd.DataFrame
+        The parent dataframe.
+    child_on : Any
+        Column or index level names in child to join on.
+    parent_on : Any
+        Column or index level names in parent to join on.
+
+    Returns
+    -------
+    pd.Series
+        A Boolean series indicating common rows.
+    """
+
+    merged = pd.merge(
+        child.reset_index(),
+        parent,
+        how="left",
+        left_on=child_on,
+        right_on=parent_on,
+        indicator=True,
+    ).set_index("index")
+    return merged["_merge"].eq("both")
+
+
 def convert_column_type(
     series: pd.Series,
     type_string: str,
     **kwargs,
 ) -> pd.Series:
     """
     Convert series to pandas dtype specified in type string representation.
@@ -30,15 +70,15 @@
     -------
     pd.Series
         The converted series with the appropriate dtype.
     """
     dtype, _ = extract_dtype_from_db_type_string(type_string)
 
     dtype_conversion_map = {
-        str: lambda x: x.astype(dtype),
+        "str": lambda x: x.astype(dtype),
         "datetime": lambda x: pd.to_datetime(x, errors="coerce", **kwargs),
         "float": lambda x: pd.to_numeric(x, errors="coerce", downcast="float"),
         "integer": lambda x: pd.to_numeric(x, errors="coerce", downcast="integer"),
         "boolean": lambda x: x.replace(
             {
                 "1": True,
                 "0": False,
@@ -49,42 +89,29 @@
             }
         ).astype(dtype),
     }
 
     return dtype_conversion_map.get(dtype, lambda x: x)(series).convert_dtypes()
 
 
-def common_rows(
-    child: pd.DataFrame,
-    parent: pd.DataFrame,
-    child_on: Any = None,
-    parent_on: Any = None,
-) -> pd.Series:
-    """
-    Return boolean mask where True if record common in Child and Parent.
+def python_to_pandas_type(python_type: Any) -> str:
+    """Return pandas type equivalent of python type.
 
     Parameters
     ----------
-    child : pd.DataFrame
-        The child dataframe.
-    parent : pd.DataFrame
-        The parent dataframe.
-    child_on : Any
-        Column or index level names in child to join on.
-    parent_on : Any
-        Column or index level names in parent to join on.
+    python_type: Any
+        Python type for which pandas equivalent is required.
 
     Returns
     -------
-    pd.Series
-        A Boolean series indicating common rows.
+    str
+        String representation of a pandas dtype.
     """
-
-    merged = pd.merge(
-        child.reset_index(),
-        parent,
-        how="left",
-        left_on=child_on,
-        right_on=parent_on,
-        indicator=True,
-    )
-    return merged["_merge"].eq("both").set_index("index")
+    PANDAS_TYPE_EQUIVALENT = {
+        int: "Int64",
+        str: "string",
+        bool: "boolean",
+        float: "float",
+        date: "datetime64[ns]",
+        datetime: "datetime64[ns]",
+    }
+    return PANDAS_TYPE_EQUIVALENT[python_type]
```

### Comparing `almirah-0.3.0/almirah/utils/gen.py` & `almirah-0.4.0/almirah/utils/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     """Return keys whose value are None."""
     return [k for k, v in dict.items() if v is None]
 
 
 def get_metadata(path: str) -> Dict[str, Any]:
     """Return dict equivalent of json in file."""
     path = Path(path).with_suffix(".json")
+
+    if not path.exists:
+        return dict()
+
     with open(path) as file:
         content = json.load(file)
         return content
 
 
 def listify(dictionary: dict) -> Dict[str, List]:
     """Return dict with value type always List."""
@@ -101,15 +105,15 @@
     with open(os.path.expanduser(path)) as file:
         return yaml.safe_load(file)
 
 
 def read_multi_yaml(path: str) -> List[Dict[Any, Any]]:
     """Return list of dict equivalents of yamls in file."""
     with open(os.path.expanduser(path)) as file:
-        return yaml.safe_load_all(file)
+        return [f for f in yaml.safe_load_all(file)]
 
 
 def run_shell(cmd: str, suppress_output: bool = True) -> subprocess.CompletedProcess:
     """Execute shell command in background."""
     return subprocess.run(
         cmd, shell=True, stdout=subprocess.DEVNULL if suppress_output else None
     )
```

### Comparing `almirah-0.3.0/almirah/utils/lib.py` & `almirah-0.4.0/almirah/utils/lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 """Library-specific utility functins."""
 
-import os
 import re
 from typing import Tuple
-
-from os.path import dirname as up
-
-from .gen import copy
+from pathlib import Path
 
 
 def extract_dtype_from_db_type_string(
     type_string: str, default_length: int = 250
 ) -> Tuple[str, int]:
     """
     Extract supported dtype and length from type string representation.
@@ -31,15 +27,15 @@
     ------
     TypeError
         If the data type is not supported.
     ValueError
         If a non-string data type incorrectly specifies a length.
     """
 
-    SUPPORTED_DTYPES = {"boolean", "datetime", "float", "integer", "str"}
+    SUPPORTED_DTYPES = {"str", "date", "float", "boolean", "integer", "datetime"}
 
     match = re.match(r"(\w+).?(\d+)?", type_string)
     if not match:
         raise ValueError(f"Invalid type string format: {type_string}")
 
     dtype, length = match.groups()
     if dtype not in SUPPORTED_DTYPES:
@@ -50,21 +46,36 @@
 
     if length is None and dtype == "str":
         length = default_length
 
     return dtype, int(length) if length else None
 
 
-def get_tutorial_dataset(dst: str) -> None:
+def create_tutorial_dataset(root: str) -> None:
     """
-    Copies the tutorial dataset to destination.
+    Create tutorial dataset at root.
 
     Parameters
     ----------
-    dst : str
-        The destination path where the dataset will be copied.
+    root : str
+        The path where the dataset will be created.
     """
 
-    from almirah import __file__ as this_file
-
-    path = os.path.join(up(up(this_file)), "tests/data/tutorial")
-    copy(path, dst)
+    # Define the structure of directories and files
+    structure = {
+        "": ["DAY01_G171_20180101.npy", "Day2_171_20180102.npy"],
+        "72": ["DAY01_G72_20180201.npy", "DAY02_G72_20180202.npy"],
+        "G433": ["DAY_G433_20180301.npy", "day02_G433_20180301.npy"],
+    }
+
+    # Ensure the root directory exists
+    root_path = Path(root)
+    root_path.mkdir(parents=True, exist_ok=True)
+
+    # Loop through the structure dictionary to create files
+    for directory, files in structure.items():
+        dir_path = root_path / directory
+        dir_path.mkdir(parents=True, exist_ok=True)
+
+        for file_name in files:
+            file_path = dir_path / file_name
+            file_path.touch()
```

### Comparing `almirah-0.3.0/almirah/utils/logging.py` & `almirah-0.4.0/almirah/utils/logging.py`

 * *Files identical despite different names*

### Comparing `almirah-0.3.0/almirah/utils/sqlalchemy.py` & `almirah-0.4.0/almirah/utils/sqlalchemy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """SQLAlchemy utility functions."""
 
 from typing import Type
-from typing import Union
 
+from sqlalchemy.types import Date
 from sqlalchemy.types import Float
 from sqlalchemy.types import String
 from sqlalchemy.types import Boolean
 from sqlalchemy.types import Integer
 from sqlalchemy.types import DateTime
+from sqlalchemy.types import TypeEngine
 
 from .lib import extract_dtype_from_db_type_string
 
 
-def get_sql_type(
-    type_string: str, default_length: int = 250
-) -> Union[Type[Float], Type[String], Type[Boolean], Type[Integer], Type[DateTime]]:
+def get_sql_type(type_string: str, default_length: int = 250) -> Type[TypeEngine]:
     """
     Return the SQLAlchemy type equivalent for a given type string representation.
 
     Parameters
     ----------
     type_string : str
         The string representation of the data type.
@@ -33,19 +32,20 @@
     Raises
     ------
     ValueError
         If the type string does not correspond to a supported SQLAlchemy type.
     """
 
     SQL_TYPE_EQUIVALENT = {
-        "boolean": Boolean,
-        "datetime": DateTime,
+        "str": String,
+        "date": Date,
         "float": Float,
+        "boolean": Boolean,
         "integer": Integer,
-        "str": String,
+        "datetime": DateTime,
     }
 
     dtype, length = extract_dtype_from_db_type_string(type_string, default_length)
     if dtype not in SQL_TYPE_EQUIVALENT:
         raise ValueError(f"Unsupported dtype '{dtype}' encountered.")
 
     sql_type = SQL_TYPE_EQUIVALENT[dtype]
```

### Comparing `almirah-0.3.0/pyproject.toml` & `almirah-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [tool.poetry]
 name = "almirah"
-version = "0.3.0"
-description = "a wardrobe for datasets"
+version = "0.4.0"
+description = "a dataset management tool"
 authors = ["girish <girishmm@ncbs.res.in>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.1.4"
 pyyaml = "^6.0.1"
 datalad = "^0.19.3"
-sqlalchemy = "^2.0.19"
+requests = "^2.31.0"
+sqlalchemy = "^2.0.30"
 sqlalchemy-json = "^0.7.0"
 
+[tool.poetry.group.gsheet.dependencies]
+gspread = "^6.1.0"
+
+[tool.poetry.group.mysql.dependencies]
+pymysql = "^1.1.0"
+
 [tool.poetry.group.mri.dependencies]
 nibabel = "^5.2.0"
 dcm2bids = "^3.1.1"
 pydeface = "^2.0.2"
 
 [tool.poetry.group.eeg.dependencies]
 mne = "^1.6.0"
```

### Comparing `almirah-0.3.0/PKG-INFO` & `almirah-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: almirah
-Version: 0.3.0
-Summary: a wardrobe for datasets
+Version: 0.4.0
+Summary: a dataset management tool
 License: MIT
 Author: girish
 Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datalad (>=0.19.3,<0.20.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: sqlalchemy-json (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 
 <br />
 <div align="center">
 
   <h3 align="center">almirah</h3>
 
   <p align="center">
-	a wardrobe for datasets
 	<br />
 	<a href="https://girishmm.github.io/almirah"><strong>Explore the docs »</strong></a>
 	<br />
 	<br />
 	<a href="https://github.com/girishmm/almirah/issues">Report Bug</a>
 	·
 	<a href="https://github.com/girishmm/almirah/issues">Request Feature</a>
   </p>
 </div>
 
 ## About The Project
 
-Clothes can be organized, maintained, and easily accessed from a
-wardrobe. [almirah](https://github.com/girishmm/almirah) serves the
-same purpose for datasets.
-
-You can define the method to follow to stack your contents on the
-almirah, and even tag. [almirah](https://github.com/girishmm/almirah)
-hopes to make working with datasets easier.
+[almirah](https://github.com/girishmm/almirah) is designed to help
+organize, maintain, and access datasets efficiently. It provides tools
+for defining how data is stored, tagged, and retrieved, making it
+easier to work with complex data collections.
+
+For more information on how to use
+[almirah](https://github.com/girishmm/almirah) for your data projects,
+please see the [documentation](https://girishmm.github.io/almirah/).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Acknowledgments
 
 Thanks to Upi and Bhalla lab members for their inputs and help.
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: almirah Version: 0.3.0 Summary: a wardrobe for
-datasets License: MIT Author: girish Author-email: girishmm@ncbs.res.in
+Metadata-Version: 2.1 Name: almirah Version: 0.4.0 Summary: a dataset
+management tool License: MIT Author: girish Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: datalad (>=0.19.3,<0.20.0) Requires-
 Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
-Dist: sqlalchemy (>=2.0.19,<3.0.0) Requires-Dist: sqlalchemy-json
-(>=0.7.0,<0.8.0) Description-Content-Type: text/markdown
+Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
+Requires-Dist: sqlalchemy-json (>=0.7.0,<0.8.0) Description-Content-Type: text/
+markdown
 
                                ******** aallmmiirraahh ********
-                           a wardrobe for datasets
+
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
-## About The Project Clothes can be organized, maintained, and easily accessed
-from a wardrobe. [almirah](https://github.com/girishmm/almirah) serves the same
-purpose for datasets. You can define the method to follow to stack your
-contents on the almirah, and even tag. [almirah](https://github.com/girishmm/
-almirah) hopes to make working with datasets easier.
+## About The Project [almirah](https://github.com/girishmm/almirah) is designed
+to help organize, maintain, and access datasets efficiently. It provides tools
+for defining how data is stored, tagged, and retrieved, making it easier to
+work with complex data collections. For more information on how to use
+[almirah](https://github.com/girishmm/almirah) for your data projects, please
+see the [documentation](https://girishmm.github.io/almirah/).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Acknowledgments Thanks to Upi and Bhalla lab members for their inputs and
 help.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

