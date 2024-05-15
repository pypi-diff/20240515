# Comparing `tmp/solarlog_cli-0.1.4.tar.gz` & `tmp/solarlog_cli-0.1.5.tar.gz`

## Comparing `solarlog_cli-0.1.4.tar` & `solarlog_cli-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/src/solarlog_cli/__init__.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/src/solarlog_cli/solarlog_client.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/src/solarlog_cli/solarlog_connector.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/src/solarlog_cli/solarlog_exceptions.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/src/solarlog_cli/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/src/solarlog_cli/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/src/solarlog_cli/solarlog_client.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/src/solarlog_cli/solarlog_connector.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/src/solarlog_cli/solarlog_exceptions.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/src/solarlog_cli/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/LICENSE
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.5/PKG-INFO
```

### Comparing `solarlog_cli-0.1.4/.github/workflows/pylint.yml` & `solarlog_cli-0.1.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/.github/workflows/python-publish.yml` & `solarlog_cli-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/.github/workflows/ruff.yml` & `solarlog_cli-0.1.5/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/src/solarlog_cli/solarlog_client.py` & `solarlog_cli-0.1.5/src/solarlog_cli/solarlog_client.py`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/src/solarlog_cli/solarlog_connector.py` & `solarlog_cli-0.1.5/src/solarlog_cli/solarlog_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,26 +46,25 @@
         if self.extended_data:
             data |= await self.client.get_energy()
             if self._device_enabled != {} and self._device_enabled is not None:
                 data |= {"devices": await self.update_inverter_data()}
             # print(f"extended data updated: {data}")
 
         #calculated values (for downward compatibility)
+        data |= {"alternator_loss": data.get("power_dc") - data.get("power_ac")}
         if data.get("power_dc") != 0:
             data |= {"efficiency": data.get("power_ac") / data.get("power_dc")}
         if data.get("power_ac") != 0:
             data |= {"usage": data.get("consumption_ac") / data.get("power_ac")}
             data |= {"power_available": data.get("power_ac") - data.get("consumption_ac")}
         else:
             data |= {"usage": 0.0}
             data |= {"power_available": 0.0}
-        data |= {"alternator_loss": data.get("power_dc") - data.get("power_ac")}
-
         if data.get("total_power") != 0:
-            data |= {"capacity": - data.get("power_dc") / data.get("total_power")}
+            data |= {"capacity": data.get("power_dc") / data.get("total_power")}
 
         return data
 
     async def update_device_list(self) -> dict[int, dict[str, str | bool]]:
         """Update list of devices."""
         if not self.extended_data:
             return {}
```

### Comparing `solarlog_cli-0.1.4/src/solarlog_cli/utils.py` & `solarlog_cli-0.1.5/src/solarlog_cli/utils.py`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/LICENSE` & `solarlog_cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.4/pyproject.toml` & `solarlog_cli-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solarlog_cli"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the Solar-Log"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

### Comparing `solarlog_cli-0.1.4/PKG-INFO` & `solarlog_cli-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solarlog_cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library to access the Solar-Log
 Project-URL: Repository, https://github.com/dontinelli/solarlog_cli.git
 Project-URL: Issues, https://github.com/dontinelli/solarlog_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/solarlog_cli/blob/master/CHANGELOG.md
 Project-URL: Solar-Log homepage, https://www.solar-log.com/
 Project-URL: API Documentation (inofficial), https://github.com/iobroker-community-adapters/ioBroker.solarlog/blob/master/docs/solarlog_dataobjects.md
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

