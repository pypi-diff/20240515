# Comparing `tmp/feliz_db-0.0.6.tar.gz` & `tmp/feliz_db-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feliz_db-0.0.6.tar", last modified: Tue Apr  2 04:14:58 2024, max compression
+gzip compressed data, was "feliz_db-0.0.8.tar", last modified: Fri Apr 12 09:33:41 2024, max compression
```

## Comparing `feliz_db-0.0.6.tar` & `feliz_db-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:14:58.704810 feliz_db-0.0.6/
--rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-02-20 04:51:52.000000 feliz_db-0.0.6/LICENSE
--rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-04-02 04:14:58.704683 feliz_db-0.0.6/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)       88 2024-02-20 04:51:52.000000 feliz_db-0.0.6/README.md
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:14:58.703710 feliz_db-0.0.6/feliz_db/
--rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-02-20 04:51:52.000000 feliz_db-0.0.6/feliz_db/__init__.py
--rw-r--r--   0 zenith3092   (501) staff       (20)    25593 2024-04-02 04:12:05.000000 feliz_db-0.0.6/feliz_db/mongo_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)    39839 2024-04-02 03:54:05.000000 feliz_db-0.0.6/feliz_db/postgres_tools.py
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:14:58.704514 feliz_db-0.0.6/feliz_db.egg-info/
--rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-04-02 04:14:58.000000 feliz_db-0.0.6/feliz_db.egg-info/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)      257 2024-04-02 04:14:58.000000 feliz_db-0.0.6/feliz_db.egg-info/SOURCES.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-04-02 04:14:58.000000 feliz_db-0.0.6/feliz_db.egg-info/dependency_links.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       36 2024-04-02 04:14:58.000000 feliz_db-0.0.6/feliz_db.egg-info/requires.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        9 2024-04-02 04:14:58.000000 feliz_db-0.0.6/feliz_db.egg-info/top_level.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-04-02 04:14:58.704850 feliz_db-0.0.6/setup.cfg
--rw-r--r--   0 zenith3092   (501) staff       (20)      908 2024-04-02 04:12:53.000000 feliz_db-0.0.6/setup.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 09:33:41.065273 feliz_db-0.0.8/
+-rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-02-20 04:51:52.000000 feliz_db-0.0.8/LICENSE
+-rw-r--r--   0 zenith3092   (501) staff       (20)     8500 2024-04-12 09:33:41.065086 feliz_db-0.0.8/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)     7981 2024-04-12 09:32:39.000000 feliz_db-0.0.8/README.md
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 09:33:41.063899 feliz_db-0.0.8/feliz_db/
+-rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-02-20 04:51:52.000000 feliz_db-0.0.8/feliz_db/__init__.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    26610 2024-04-12 09:32:39.000000 feliz_db-0.0.8/feliz_db/mongo_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    39839 2024-04-02 03:54:05.000000 feliz_db-0.0.8/feliz_db/postgres_tools.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 09:33:41.064905 feliz_db-0.0.8/feliz_db.egg-info/
+-rw-r--r--   0 zenith3092   (501) staff       (20)     8500 2024-04-12 09:33:41.000000 feliz_db-0.0.8/feliz_db.egg-info/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)      257 2024-04-12 09:33:41.000000 feliz_db-0.0.8/feliz_db.egg-info/SOURCES.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-04-12 09:33:41.000000 feliz_db-0.0.8/feliz_db.egg-info/dependency_links.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       36 2024-04-12 09:33:41.000000 feliz_db-0.0.8/feliz_db.egg-info/requires.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        9 2024-04-12 09:33:41.000000 feliz_db-0.0.8/feliz_db.egg-info/top_level.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-04-12 09:33:41.065314 feliz_db-0.0.8/setup.cfg
+-rw-r--r--   0 zenith3092   (501) staff       (20)      908 2024-04-12 09:32:39.000000 feliz_db-0.0.8/setup.py
```

### Comparing `feliz_db-0.0.6/LICENSE` & `feliz_db-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feliz_db-0.0.6/feliz_db/mongo_tools.py` & `feliz_db-0.0.8/feliz_db/mongo_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,19 +25,51 @@
     def format_and_validate_document(cls, data):
         ret = []
         for item in data:
             add_item = cls(**item)
             add_item.validate()
             ret.append(add_item)
         return ret
+    
+    @classmethod
+    def _process_id_condition(cls, conditions: dict) -> dict:
+        if conditions.get("_id"):
+            id_condition = conditions["_id"]
+            if isinstance(id_condition, str):
+                # {_id: "123456"} -> {_id: ObjectId("123456")}
+                id_condition = ObjectId(id_condition)
+            elif isinstance(id_condition, dict):
+                for key, value in id_condition.items():
+                    if isinstance(value, str):
+                        # {_id: {"$eq": "123456"}} -> {_id: {"$eq": ObjectId("123456")}}
+                        id_condition[key] = ObjectId(value)
+                    elif isinstance(value, list):
+                        # {_id: {"$in": ["123456", "789012"]}} -> {_id: {"$in": [ObjectId("123456"), ObjectId("789012")]
+                        id_condition[key] = [ObjectId(v) if isinstance(v, str) else v for v in value]
+                    elif isinstance(value, dict):
+                        # {_id: {"$not": {"$eq": "123456"}}} -> {_id: {"$not": {"$eq": ObjectId("123456")}}
+                        id_condition[key] = cls._process_id_condition(value)
+            conditions["_id"] = id_condition
+        else:
+            for key, value in conditions.items():
+                if key.startswith("$"):
+                    if isinstance(value, str):
+                        # {"#eq": "123456} -> {"#eq": ObjectId("123456")}
+                        conditions[key] = ObjectId(value)
+                    elif isinstance(value, list):
+                        # {"$or": [{"_id": "123456"}, {"_id": "789012"}]} -> {"$or": [{"_id": ObjectId("123456")}, {"_id": ObjectId("789012")}]
+                        for item in value:
+                            # {"_id": "123456"} -> {"_id": ObjectId("123456")}
+                            item = cls._process_id_condition(item)
+        return conditions
 
     @classmethod
-    def handle_modified_time(cls, data: list) -> list:
+    def handle_modified_time(cls, data: list, time_format="%Y%m%d%H%M%S%f") -> list:
         for item in data:
-            item["modified_time"] = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:-3]
+            item["modified_time"] = datetime.datetime.now().strftime(time_format)[:-3]
         return data
 
     @classmethod
     def get_headers(cls):
         return list(cls._fields_ordered)
 
     @classmethod
@@ -45,36 +77,33 @@
         add_data = cls.format_and_validate_document(data)
         ret = cls.objects.insert(add_data)
         return cls.format_data_list(ret)
 
     @classmethod
     def get_data(cls, conditions, order_by_list=[]):
         if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
+            conditions = cls._process_id_condition(conditions)
             raw_data = cls.objects(__raw__=conditions)
         else:
             raw_data = cls.objects
         return cls.format_data_list(raw_data.order_by(*order_by_list))
     
     @classmethod
     def update_data(cls, conditions, update_data):
         if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
+            conditions = cls._process_id_condition(conditions)
             raw_data = cls.objects(__raw__=conditions)
         else:
             raw_data = cls.objects
         return cls.format_data(raw_data.modify(__raw__={"$set": update_data}, new=True))
     
     @classmethod
     def delete_data(cls, conditions):
         if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
+            conditions = cls._process_id_condition(conditions)
             raw_data = cls.objects(__raw__=conditions)
         else:
             raw_data = cls.objects
         
         return raw_data.delete()
 
 class MongoHandler:
@@ -221,15 +250,15 @@
                 $meta: control the metadata returned in a text search (e.g. {"$text": {"$search": "John", "$meta": "textScore"}})
             - projection operators:
                 $slice: limit the number of elements in an array that a $push operation inserts (e.g. {"$push": {"favorite": {"$each": [{"title": "react"}, {"title": "linux"}], "$slice": 2}}})
                 $sort: sort elements in an array during a $push operation (e.g. {"$push": {"favorite": {"$each": [{"title": "react"}, {"title": "linux"}], "$sort": {"title": 1}}}})
         TIPS:
             $or can be replaced by $in, e.g. {"$or": [{"name": "John"}, {"name": "Peter"}]} can be replaced by {"name": {"$in": ["John", "Peter"]}}
             $and can be replaced by $all, e.g. {"$and": [{"name": "John"}, {"age": 18}]} can be replaced by {"$all": [{"name": "John"}, {"age": 18}]}
-            $not can be replaced by $ne, e.g. {"name": {"$not": {"$eq": "John"}}} can be replaced by {"name": {"$ne": "John"}}
+            $not + $eq can be replaced by $ne, e.g. {"name": {"$not": {"$eq": "John"}}} can be replaced by {"name": {"$ne": "John"}}
             $nor can be replaced by $nin, e.g. {"$nor": [{"name": "John"}, {"name": "Peter"}]} can be replaced by {"name": {"$nin": ["John", "Peter"]}}
         """
         self.connect()
 
         try:
             schema: DocumentHandler = self.__dict__[schema_name]
 
@@ -401,14 +430,49 @@
         for key, value in data_dict.items():
             if isinstance(value, ObjectId):
                 data_dict[key] = str(value)
             elif isinstance(value, datetime.datetime):
                 data_dict[key] = value.timestamp()
         return data_dict
 
+    def _process_id_condition(self, conditions: dict) -> dict:
+        if conditions.get("_id", None):
+            id_condition = conditions["_id"]
+            if isinstance(id_condition, str):
+                # {_id: "123456"} -> {_id: ObjectId("123456")}
+                id_condition = ObjectId(id_condition)
+            elif isinstance(id_condition, dict):
+                for key, value in id_condition.items():
+                    if isinstance(value, str):
+                        # {_id: {"$eq": "123456"}} -> {_id: {"$eq": ObjectId("123456")}}
+                        id_condition[key] = ObjectId(value)
+                    elif isinstance(value, list):
+                        # {_id: {"$in": ["123456", "789012"]}} -> {_id: {"$in": [ObjectId("123456"), ObjectId("789012")]
+                        # id_condition[key] = [ObjectId(v) for v in value]
+                        id_condition[key] = [ObjectId(v) if isinstance(v, str) else v for v in value]
+                    elif isinstance(value, dict):
+                        # {_id: {"$not": {"$eq": "123456"}}} -> {_id: {"$not": {"$eq": ObjectId("123456")}}
+                        id_condition[key] = self._process_id_condition(value)
+            conditions["_id"] = id_condition
+        else:
+            for key, value in conditions.items():
+                if key.startswith("$"):
+                    if isinstance(value, str):
+                        # {_id: {"$not": {"$eq": "123456"}}} -> {_id: {"$not": {"$eq": ObjectId("123456")}}
+                        #     |
+                        #     v
+                        # {"#eq": "123456} -> {"#eq": ObjectId("123456")}
+                        conditions[key] = ObjectId(value)
+                    elif isinstance(value, list):
+                        # {"$or": [{"_id": "123456"}, {"_id": "789012"}]} -> {"$or": [{"_id": ObjectId("123456")}, {"_id": ObjectId("789012")}]
+                        for item in value:
+                            # {"_id": "123456"} -> {"_id": ObjectId("123456")}
+                            item = self._process_id_condition(item)
+        return conditions
+
     def get_data(self, collection: str, conditions={}, order_by_list=[], ret_type="original") -> dict:
         """
         Get data from MongoDB
         
         Args:
             collection (str): name of collection
             conditions (dict): conditions of query (follow MongoDB query syntax)
@@ -417,56 +481,58 @@
                                            e.g. [("modified_time", -1)]
             ret_type (str, optional): return type. Defaults to "original". Should be one of ["jsonable", "original"].
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list[dict]
+                "formatted_data": list[dict]
             }
         """
         self.connect()
         try:
             indicator = True
             message = "Get data from MongoDB successfully"
             if ret_type not in self.__class__._valid_ret_type_list:
                 raise ValueError("Invalid ret_type: {}".format(ret_type))
             elif ret_type == "empty":
                 raise ValueError("ret_type cannot be 'empty' for get_data() function.")
             
+            conditions = self._process_id_condition(conditions)
+            
             if order_by_list:
                 data = list(self.client[self.database][collection].find(conditions).sort(order_by_list))
             else:
                 data = list(self.client[self.database][collection].find(conditions))
 
             if ret_type == "jsonable":
                 for item in data:
                     item = self.form_jsonable_data(item)
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Get data from MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
         self.disconnect()
-        return {"indicator": indicator, "message": message, "data": data}
+        return {"indicator": indicator, "message": message, "formatted_data": data}
     
     def _add_data(self, collection: str, data: list[dict], ret_type="original") -> dict:
         """
         Add data to MongoDB
         
         Args:
             collection (str): name of collection
             data (list[dict]): data to add
             ret_type (str, optional): return type. Defaults to "original". Should be one of ["empty", "jsonable", "original"].
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list[dict]
+                "formatted_data": list[dict]
             }
         """
         self.connect()
 
         try:
             indicator = True
             message = "Add data to MongoDB successfully"
@@ -486,15 +552,15 @@
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Add data to MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
         
         self.disconnect()
-        return {"indicator": indicator, "message": message, "data": ret}
+        return {"indicator": indicator, "message": message, "formatted_data": ret}
 
     def _update_data(self, collection: str, conditions: dict, update_data: dict, ret_type="original") -> dict:
         """
         Update data in MongoDB
         
         Args:
             collection (str): name of collection
@@ -502,15 +568,15 @@
             update_data (dict): data to update
             ret_type (str, optional): return type. Defaults to "original". Should be one of ["empty", "jsonable", "original"].
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list
+                "formatted_data": list
             }
         """
         self.connect()
 
         try:
             indicator = True
             message = "Update data in MongoDB successfully"
@@ -528,29 +594,29 @@
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Update data in MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
         
         self.disconnect()
-        return {"indicator": indicator, "message": message, "data": ret}
+        return {"indicator": indicator, "message": message, "formatted_data": ret}
 
     def _delete_data(self, collection: str, conditions: dict):
         """
         Delete data from MongoDB
         
         Args:
             collection (str): name of collection
             conditions (dict): conditions of query (follow MongoDB query syntax)
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list
+                "formatted_data": list
             }
         """
         self.connect()
 
         try:
             indicator = True
             message = "Delete data from MongoDB successfully"
@@ -558,98 +624,8 @@
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Delete data from MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
         
         self.disconnect()
-        return {"indicator": indicator, "message": message, "data": ret}
-
-# if __name__ == '__main__':
-#     # ========== MongoWidget Example ==========
-
-#     configs = {
-#                 "host": "localhost",
-#                 "port": 48763,
-#                 "database": "trigger",
-#                 "username": "test",
-#                 "password": "mongodb",
-#               }
-    
-#     mw = MongoWidget(**configs)
-#     res = mw.get_data("user", order_by_list=[("modified_time", -1)])
-#     print(res["data"])
-
-    # ========== MongoHandler Example ==========
-
-    # Schema Example (Before using MongoHandler, you need to define schemas first):
-
-    # class User(DocumentHandler):
-    #     account_id = mongo.StringField(required=True)
-    #     username = mongo.StringField(required=True)
-    #     password = mongo.StringField(required=True)
-    #     update_state = mongo.BooleanField(required=True, default=False)
-    #     permission = mongo.StringField(required=True)
-    #     favorite = mongo.ListField(field=mongo.DictField(), required=False)
-    #     modified_time = mongo.StringField(required=True)
-    #     comments = mongo.StringField(required=False, default="")
-    #     meta = {"db_alias": "trigger"}
-
-    # # Construct MongoHandler:
-
-    # configs = {
-    #             "alias": "trigger",
-    #             "host": "localhost",
-    #             "port": 5445,
-    #             "database": "trigger",
-    #             "username": "test",
-    #             "password": "test",
-    #             "schemas": {"user": User}
-    #           }
-    # mh = MongoHandler(**configs)
-
-    # # Get Data
-
-    # conditions = {"update_state": False, "favorite": {"$elemMatch": {"title": "react"}}}
-    # order_by_list = ["-modified_time"]
-    # res = mh.get_data("user", conditions, order_by_list)
-    # if res["indicator"]:
-    #     print(res["formatted_data"])
-    # else:
-    #     print(res["message"])
-    
-#     # Add Data
-
-#     data = [{
-#             'account_id': 'charlie_sysadmin',
-#             'username': 'Charlie SysAdmin',
-#             'password': 'charlie_password',
-#             'update_state': False,
-#             'permission': 'a',
-#             'favorite': [{'title': 'linux', 'author': 'open_source_guru'}],
-#             "modified_time": datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:-3],
-#             'comments': 'System administrator specializing in Linux.'
-#             }]
-#     res = mh.add_data("user", data)
-#     if res["indicator"]:
-#         print(res["formatted_data"])
-#     else:
-#         print(res["message"])
-    
-#     # Update Data
-
-#     update_query = {"account_id": "charlie_sysadmin"}
-#     update_data =  {"update_state": True}
-#     res = mh.update_data("user", update_query, update_data)
-#     if res["indicator"]:
-#         print(res["formatted_data"])
-#     else:
-#         print(res["message"])
-    
-#     # Delete Data
-
-#     delete_query = {"account_id": "charlie_sysadmin"}
-#     res = mh.delete_data("user", delete_query)
-#     if res["indicator"]:
-#         print(res["formatted_data"])
-#     else:
-#         print(res["message"])
+        return {"indicator": indicator, "message": message, "formatted_data": ret}
```

### Comparing `feliz_db-0.0.6/feliz_db/postgres_tools.py` & `feliz_db-0.0.8/feliz_db/postgres_tools.py`

 * *Files identical despite different names*

### Comparing `feliz_db-0.0.6/setup.py` & `feliz_db-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open(os.path.join(os.path.dirname(__file__), "requirements.txt"), "r") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="feliz_db",
-    version="0.0.6",
+    version="0.0.8",
     author="Vincent Wu, Linga Chen, Brian Yin",
     author_email="zenith3092@gmail.com",
     description="A framework designed to assist in using databases and compatible with feliz framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zenith3092/feliz_db",
     license="MIT",
```

