# Comparing `tmp/rov_db_access-0.1.7.tar.gz` & `tmp/rov_db_access-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-0.1.7.tar", max compression
+gzip compressed data, was "rov_db_access-0.1.8.tar", max compression
```

## Comparing `rov_db_access-0.1.7.tar` & `rov_db_access-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      453 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.7/README.md
--rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.7/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.7/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.7/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.7/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0     1122 2024-05-08 20:09:03.118984 rov_db_access-0.1.7/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.7/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     7207 2024-05-08 20:09:03.119358 rov_db_access-0.1.7/rov_db_access/gis/models.py
--rw-r--r--   0        0        0    25083 2024-05-14 15:53:52.686829 rov_db_access-0.1.7/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.7/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.7/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.7/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0     1531 2024-05-08 20:09:03.120864 rov_db_access-0.1.7/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.7/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      453 2024-05-15 19:14:44.176545 rov_db_access-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.8/README.md
+-rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.8/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.8/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.8/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.8/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-0.1.8/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0     1115 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.8/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     7617 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0    25385 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.8/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.8/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.8/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0     1522 2024-05-15 19:14:44.177669 rov_db_access-0.1.8/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.8/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.8/PKG-INFO
```

### Comparing `rov_db_access-0.1.7/rov_db_access/authentication/models.py` & `rov_db_access-0.1.8/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.7/rov_db_access/authentication/worker.py` & `rov_db_access-0.1.8/rov_db_access/authentication/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.7/rov_db_access/config/db_utils.py` & `rov_db_access-0.1.8/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.7/rov_db_access/config/settings.py` & `rov_db_access-0.1.8/rov_db_access/config/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,12 +40,13 @@
 
     geoserver_api_url: str
 
     gis_inference_bucket: str
     gis_inference_region: str
 
     run_results_bucket: str
-    run_results_region: str
+
+    s3_region: str
 
     sentinel_bucket: str
     sentinel_user: str
     sentinel_password: str
```

### Comparing `rov_db_access-0.1.7/rov_db_access/gis/models.py` & `rov_db_access-0.1.8/rov_db_access/gis/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 
     user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
     user: Mapped["User"] = relationship()
 
     organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
     organization: Mapped["Organization"] = relationship()
 
+    run: Mapped[Optional["Run"]] = relationship(
+        back_populates="input"
+    )
+
     def __repr__(self) -> str:
         return f"Input (id={self.id!r}, user_id={self.user_id!r}, organization_id={self.organization_id!r})"
 
 
 class InferenceModel(Base):
     __tablename__ = "inference_model"
     __table_args__ = {"schema": "gis"}
@@ -74,15 +78,15 @@
     __table_args__ = {"schema": "gis"}
     id: Mapped[int] = mapped_column(primary_key=True)
     name: Mapped[str]
     status: Mapped[str] = mapped_column(server_default="queued")
     type: Mapped[str] = mapped_column(server_default="on demand")
     created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
     finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
-    time: Mapped[float] = mapped_column(server_default="0")
+    runtime: Mapped[int] = mapped_column(server_default="0")
     area: Mapped[float] = mapped_column(server_default="0")
     cost_estimated: Mapped[float] = mapped_column(server_default="0")
 
     data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
 
     geom: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
     mask: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
@@ -94,78 +98,83 @@
     organization: Mapped["Organization"] = relationship()
 
     user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
     user: Mapped["User"] = relationship()
 
     runs: Mapped[List["Run"]] = relationship(
        back_populates="process",
-       order_by="Run.id"
+       order_by="Run.id",
+       cascade="all, delete"
     )
 
     def __repr__(self) -> str:
         return f"Process(id={self.id!r}, name={self.name!r}, status={self.status!r}, inference_model_id={self.inference_model_id!r}), user_id={self.user_id!r})"
 
 
 class ResultsRaster(Base):
     __tablename__ = "results_raster"
     __table_args__ = {"schema": "gis"}
     id: Mapped[int] = mapped_column(primary_key=True)
     url: Mapped[str]
     data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
     bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
 
-    run_id: Mapped[int] = mapped_column(ForeignKey("gis.run.id"))
+    run_id: Mapped[int] = mapped_column(ForeignKey("gis.run.id", ondelete="CASCADE"))
     run: Mapped["Run"] = relationship(back_populates="results_raster")
 
     def __repr__(self) -> str:
         return f"ResultsRaster(id={self.id!r}, url={self.url!r}, run_id={self.run_id!r})"
 
 
 class ResultsRaw(Base):
     __tablename__ = "results_raw"
     __table_args__ = {"schema": "gis"}
     id: Mapped[int] = mapped_column(primary_key=True)
     data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
     geom: Mapped[Geometry] = mapped_column(Geometry("MULTIPOLYGON", srid=4326))
 
-    run_id: Mapped[int] = mapped_column(ForeignKey("gis.run.id"))
+    run_id: Mapped[int] = mapped_column(ForeignKey("gis.run.id", ondelete="CASCADE"))
     run: Mapped["Run"] = relationship(back_populates="results_raw")
 
     def __repr__(self) -> str:
         return f"ResultsRaw(id={self.id!r}, data={self.data!r}, geom={self.geom!r}, run_id={self.run_id!r})"
 
 
 class Run(Base):
     __tablename__ = "run"
     __table_args__ = {"schema": "gis"}
     id: Mapped[int] = mapped_column(primary_key=True)
     status: Mapped[str] = mapped_column(server_default="queued")
     created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
     finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
     engine: Mapped[str] = mapped_column(server_default="local")
-    runtime: Mapped[float] = mapped_column(server_default="0")
+    runtime: Mapped[int] = mapped_column(server_default="0")
     cost: Mapped[float] = mapped_column(server_default="0")
     filepath: Mapped[Optional[str]]
 
     data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
 
-    input_id: Mapped[Optional[int]] = mapped_column(ForeignKey("gis.input.id"), nullable=True)
-    input: Mapped[Optional["Input"]] = relationship()
+    input_id: Mapped[Optional[int]] = mapped_column(ForeignKey("gis.input.id", ondelete="CASCADE"), nullable=True)
+    input: Mapped[Optional["Input"]] = relationship(back_populates="run", uselist=False, cascade="all, delete")
 
     inference_model_id: Mapped[int] = mapped_column(ForeignKey("gis.inference_model.id"))
     inference_model: Mapped["InferenceModel"] = relationship()
 
-    process_id: Mapped[int] = mapped_column(ForeignKey("gis.process.id"))
+    process_id: Mapped[int] = mapped_column(ForeignKey("gis.process.id", ondelete="CASCADE"))
     process: Mapped["Process"] = relationship()
 
+    bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+
     results_raw: Mapped[List["ResultsRaw"]] = relationship(
        back_populates="run",
-       order_by="ResultsRaw.id"
+       order_by="ResultsRaw.id",
+       cascade="all, delete"
     )
 
     results_raster: Mapped[List["ResultsRaster"]] = relationship(
         back_populates="run",
-        order_by="ResultsRaster.id"
+        order_by="ResultsRaster.id",
+        cascade="all, delete"
     )
 
     def __repr__(self) -> str:
         return f"Run(id={self.id!r}, status={self.status!r}, process_id={self.process_id!r}) inference_model_id={self.inference_model_id!r})"
```

### Comparing `rov_db_access-0.1.7/rov_db_access/gis/worker.py` & `rov_db_access-0.1.8/rov_db_access/gis/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
             return {
                 "id": process.id,
                 "name": process.name,
                 "status": process.status,
                 "type": process.type,
                 "created_at": process.created_at.strftime("%d/%m/%Y: %H:%M"),
                 "finished_at": finished_time,
-                "time": process.time,
+                "runtime": process.runtime,
                 "area": process.area,
                 "cost_estimated": process.cost_estimated,
                 "data": process.data,
                 "user": process.user.username,
                 "inference_model_id": process.inference_model_id,
                 "geom": geom,
                 "mask": mask,
@@ -436,15 +436,15 @@
             result.append({
                 "id": process.id,
                 "name": process.name,
                 "status": process.status,
                 "type": process.type,
                 "created_at": process.created_at.strftime("%d/%m/%Y: %H:%M"),
                 "finished_at": finished_time,
-                "time": process.time,
+                "runtime": process.runtime,
                 "area": process.area,
                 "cost_estimated": process.cost_estimated,
                 "data": process.data,
                 "user": process.user.username,
                 "inference_model_id": process.inference_model_id,
                 "geom": geom,
                 "mask": mask,
@@ -580,35 +580,35 @@
             user_id=user.id,
             organization_id=user.organization_id
         )
         self.session.add(new_image)
         self.session.commit()
         return new_image
 
-    def upload_run_results(self, run_id: int, runtime: float, files_path: str, raster_name: str=None, file_names: list[str]=[], data: dict=None, bbox: str=None):
+    def upload_run_results(self, run_id: int, runtime: int, bbox: str, files_path: str, raster_name: str=None, file_names: list[str]=[], data: dict=None):
         """
         Uploads the files to the S3 bucket and updates the run status to finished
 
         Args:
             run_id: The id of the run
+            bbox: The bbox of the raster
             files_path: The path where the files are located
             runtime: The runtime of the run
             raster_name: The name of the raster file
             file_names: Array with the names of additional files to upload
             data: additional data to store in the results raster table
-            bbox: The bbox of the raster
         """
         assert isinstance(run_id, int), 'Invalid run_id!'
+        assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
         assert isinstance(runtime, (int, float)), 'Invalid runtime!'
-        runtime = float(runtime)
+        runtime = int(runtime)
         assert isinstance(files_path, str), 'Invalid files_path!'
         assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
         assert isinstance(file_names, list), 'Invalid file_names!'
         assert data is None or isinstance(data, dict), 'Invalid data!'
-        assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
 
         assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
 
         self.check_db_connection()
 
         # actual function
         query = (
@@ -647,16 +647,19 @@
             object_key = bucket_base_directory + raster_name
             file_path = os.path.join(files_path, raster_name)
             s3_client.upload_file(file_path, object_key)
             print(f'File uploaded to S3 with key: {object_key}')
             self.add_results_raster(run_id, object_key, data, bbox)
 
         # update run status
+        # when all runs of a process are finished, an SQL trigger will update the process status
         run.status = 'finished'
         run.finished_at = func.now()
+        run.bbox = bbox
+        # SQL trigger will update the process runtime
         run.runtime = runtime
         run.filepath = bucket_base_directory
         self.session.commit()
 
         return True
 
     def add_results_raster(self, run_id, object_key, data=None, bbox=None):
@@ -666,30 +669,32 @@
             bbox=bbox,
             run_id=run_id
         )
         self.session.add(new_result)
         self.session.commit()
         return new_result
 
-    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished']):
+    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished', 'failed', 'canceled']):
         """
         Updates the status of the run
 
         Args:
             run_id: The id of the run
             status: The new status of the run
         """
         assert isinstance(run_id, int), 'Invalid run_id!'
-        assert status in ['queued', 'running', 'finished'], 'Invalid status!'
+        assert status in ['queued', 'running', 'finished', 'failed', 'canceled'], 'Invalid status!'
 
         query = (
             select(Run)
             .where(Run.id == run_id)
             .limit(1)
         )
         run = self.session.scalar(query)
         if run is None:
             print(f'No run with id ${run_id} found!')
             return False
         run.status = status
+        if status == 'running':
+            run.process.status = 'running'
         self.session.commit()
         return True
```

### Comparing `rov_db_access-0.1.7/rov_db_access/sentinel/worker.py` & `rov_db_access-0.1.8/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.7/rov_db_access/utils/s3_utils.py` & `rov_db_access-0.1.8/rov_db_access/utils/s3_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rov_db_access.config.settings import Settings
 
 settings = Settings()
 
 
 class S3Client:
     def __init__(self):
-        self.region = settings.run_results_region
+        self.region = settings.s3_region
         self.bucket_name = settings.run_results_bucket
         self.access_key_id = settings.aws_key
         self.secret_access_key = settings.aws_secret
 
         self.s3 = boto3.client(
             "s3",
             aws_access_key_id=self.access_key_id,
```

### Comparing `rov_db_access-0.1.7/rov_db_access/utils/utils.py` & `rov_db_access-0.1.8/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-0.1.7/PKG-INFO` & `rov_db_access-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

