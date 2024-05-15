# Comparing `tmp/medicafe-0.240515.0.tar.gz` & `tmp/medicafe-0.240515.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240515.0.tar", last modified: Wed May 15 17:25:59 2024, max compression
+gzip compressed data, was "medicafe-0.240515.1.tar", last modified: Wed May 15 18:59:00 2024, max compression
```

## Comparing `medicafe-0.240515.0.tar` & `medicafe-0.240515.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 17:25:59.096000 medicafe-0.240515.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-15 17:25:58.214000 medicafe-0.240515.0/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    12886 2024-05-15 17:19:29.000000 medicafe-0.240515.0/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17162 2024-05-15 16:23:06.000000 medicafe-0.240515.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8605 2024-05-15 16:21:09.000000 medicafe-0.240515.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:25:58.843000 medicafe-0.240515.0/MediLink/
--rw-rw-rw-   0        0        0    20198 2024-05-15 16:36:41.000000 medicafe-0.240515.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    42599 2024-05-15 16:56:55.000000 medicafe-0.240515.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     5834 2024-05-15 17:02:29.000000 medicafe-0.240515.0/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.0/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.0/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.0/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.0/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-15 17:25:59.080000 medicafe-0.240515.0/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 17:25:59.060000 medicafe-0.240515.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-15 17:25:57.000000 medicafe-0.240515.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-15 17:25:57.000000 medicafe-0.240515.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 17:25:57.000000 medicafe-0.240515.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-15 17:25:57.000000 medicafe-0.240515.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 17:25:57.000000 medicafe-0.240515.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 17:25:59.092000 medicafe-0.240515.0/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-15 17:25:54.000000 medicafe-0.240515.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.670000 medicafe-0.240515.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-15 18:58:59.621000 medicafe-0.240515.1/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14539 2024-05-15 18:56:28.000000 medicafe-0.240515.1/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8605 2024-05-15 16:21:09.000000 medicafe-0.240515.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.402000 medicafe-0.240515.1/MediLink/
+-rw-rw-rw-   0        0        0    20303 2024-05-15 18:53:31.000000 medicafe-0.240515.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    41978 2024-05-15 18:52:35.000000 medicafe-0.240515.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.1/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.1/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.1/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-15 18:59:00.619000 medicafe-0.240515.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.599000 medicafe-0.240515.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:59:00.665000 medicafe-0.240515.1/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-15 18:58:57.000000 medicafe-0.240515.1/setup.py
```

### Comparing `medicafe-0.240515.0/LICENSE` & `medicafe-0.240515.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot.bat` & `medicafe-0.240515.1/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot.py` & `medicafe-0.240515.1/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot_Charges.py` & `medicafe-0.240515.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240515.1/MediBot/MediBot_Crosswalk_Library.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,53 +17,89 @@
     from MediLink_APIs import fetch_payer_name_from_api
 except ImportError:
     from MediLink import MediLink_APIs
     fetch_payer_name_from_api = MediLink_APIs.fetch_payer_name_from_api
 
 try:
     from MediBot import MediBot_Preprocessor_lib
-    load_data_sources = MediBot_Preprocessor_lib.load_data_sources, 
-    load_historical_payer_to_patient_mappings = MediBot_Preprocessor_lib.load_historical_payer_to_patient_mappings, 
-    load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains, 
-    map_payer_ids_to_insurance_ids = MediBot_Preprocessor_lib.map_payer_ids_to_insurance_ids, 
-    parse_z_dat = MediBot_Preprocessor_lib.parse_z_dat
 except ImportError:
-    from MediBot_Preprocessor_lib import load_data_sources, load_historical_payer_to_patient_mappings, load_insurance_data_from_mains, map_payer_ids_to_insurance_ids, parse_z_dat
+    import MediBot_Preprocessor_lib
+
+def check_and_initialize_crosswalk(config):
+    """
+    Checks if the 'payer_id' key exists in the crosswalk. If not, prompts the user
+    to initialize the crosswalk.
+
+    Args:
+        config (dict): Configuration settings.
+
+    Returns:
+        boolean: True if succeeded.
+    """
+    # Reload for safety
+    config, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
+    
+    try:
+        # Attempt to access the 'payer_id' key to ensure it exists
+        if 'payer_id' not in crosswalk:
+            raise KeyError("Missing 'payer_id' key in crosswalk.")
+    except KeyError:
+        error_message = "The 'payer_id' key does not exist in the crosswalk configuration. " \
+                        "This could be because the crosswalk is not initialized. " \
+                        "Consider running the Crosswalk initializer."
+        print(error_message)
+        MediLink_ConfigLoader.log(error_message, config, level="ERROR")
+        
+        # Prompt user to initialize crosswalk
+        initialize_choice = input("\nADVANCED OPTION: The crosswalk is not initialized. Do you want to initialize it now? (yes/no): ").strip().lower()
+        if initialize_choice == 'yes':
+            initialize_crosswalk_from_mapat()
+            _, crosswalk = MediLink_ConfigLoader.load_configuration() # Reload crosswalk
+            MediLink_ConfigLoader.log("Crosswalk reloaded successfully.", config, level="INFO")
+        else:
+            raise KeyError(error_message)
+    
+    return True
 
 def validate_and_correct_payer_ids(crosswalk, config):
     """Validates payer IDs via API and handles invalid IDs through user intervention."""
     for payer_id in list(crosswalk['payer_id'].keys()):
         try:
             fetch_payer_name_from_api(payer_id, config, primary_endpoint=None)
             MediLink_ConfigLoader.log("Payer ID {} validated successfully.".format(payer_id), config, level="INFO")
         except Exception as e:
             MediLink_ConfigLoader.log("Payer ID validation failed for {}: {}".format(payer_id, e), config, level="WARNING")
-            corrected_payer_id = input("Invalid Payer ID {}. Please enter the correct Payer ID for replacement: ".format(payer_id))
             
-            if corrected_payer_id:
-                try:
-                    fetch_payer_name_from_api(corrected_payer_id, config, primary_endpoint=None)
-                    MediLink_ConfigLoader.log("Corrected Payer ID {} validated successfully.".format(corrected_payer_id), config, level="INFO")
-                    if update_crosswalk_with_corrected_payer_id(payer_id, corrected_payer_id, config, crosswalk):
-                        # Add to csv_replacements
-                        if 'csv_replacements' not in crosswalk:
-                            crosswalk['csv_replacements'] = {}
-                        crosswalk['csv_replacements'][payer_id] = corrected_payer_id
-                        MediLink_ConfigLoader.log("Added replacement filter: {} -> {}".format(payer_id, corrected_payer_id), config, level="INFO")
-                    else:
-                        print("Failed to update crosswalk with the corrected Payer ID {}.".format(corrected_payer_id))
-                        MediLink_ConfigLoader.log("Failed to update crosswalk with the corrected Payer ID {}.".format(corrected_payer_id), config, level="ERROR")
-                except Exception as e:
-                    print("Corrected Payer ID {} validation failed: {}".format(corrected_payer_id, e))
-                    MediLink_ConfigLoader.log("Corrected Payer ID {} validation failed: {}".format(corrected_payer_id, e), config, level="ERROR")
+            while True:
+                corrected_payer_id = input("WWARNING: Invalid Payer ID {}. Enter the correct Payer ID for replacement or type 'FORCE' to continue with the unresolved Payer ID: ".format(payer_id))
+                
+                if corrected_payer_id.strip().upper() == 'FORCE':
+                    MediLink_ConfigLoader.log("User opted to force-continue with unresolved Payer ID {}. Warning: This may indicate an underlying issue.".format(payer_id), config, level="WARNING")
+                    break
+
+                if corrected_payer_id:
+                    try:
+                        fetch_payer_name_from_api(corrected_payer_id, config, primary_endpoint=None)
+                        MediLink_ConfigLoader.log("Corrected Payer ID {} validated successfully.".format(corrected_payer_id), config, level="INFO")
+                        
+                        if update_crosswalk_with_corrected_payer_id(payer_id, corrected_payer_id, config, crosswalk):
+                            if 'csv_replacements' not in crosswalk:
+                                crosswalk['csv_replacements'] = {}
+                            crosswalk['csv_replacements'][payer_id] = corrected_payer_id
+                            MediLink_ConfigLoader.log("Added replacement filter: {} -> {}".format(payer_id, corrected_payer_id), config, level="INFO")
+                        else:
+                            print("Failed to update crosswalk with the corrected Payer ID {}.".format(corrected_payer_id))
+                            MediLink_ConfigLoader.log("Failed to update crosswalk with the corrected Payer ID {}.".format(corrected_payer_id), config, level="ERROR")
+                        break
+                    except Exception as e:
+                        print("Corrected Payer ID {} validation failed: {}".format(corrected_payer_id, e))
+                        MediLink_ConfigLoader.log("Corrected Payer ID {} validation failed: {}".format(corrected_payer_id, e), config, level="ERROR")
+                else:
+                    print("Exiting initialization. Please correct the Payer ID and retry.")
                     sys.exit(1)
-            else:
-                print("Exiting initialization. Please correct the Payer ID and retry.")
-                sys.exit(1)
-
 
 def initialize_crosswalk_from_mapat():
     """
     Input: Historical Carol's CSVs and MAPAT data.
 
     Process:
         Extract mappings from Carol's old CSVs to identify Payer IDs and associated Patient IDs.
@@ -72,31 +108,33 @@
 
     Output: A fully populated crosswalk.json file that serves as a baseline for future updates.
     """
     config, crosswalk = MediLink_ConfigLoader.load_configuration()
     
     # Load historical mappings
     try:
-        patient_id_to_insurance_id, payer_id_to_patient_ids = load_data_sources(config)
+        patient_id_to_insurance_id, payer_id_to_patient_ids = MediBot_Preprocessor_lib.load_data_sources(config, crosswalk)
     except ValueError as e:
         print(e)
         sys.exit(1)
     
     # Map Payer IDs to Insurance IDs
-    payer_id_to_details = map_payer_ids_to_insurance_ids(patient_id_to_insurance_id, payer_id_to_patient_ids)
+    payer_id_to_details = MediBot_Preprocessor_lib.map_payer_ids_to_insurance_ids(patient_id_to_insurance_id, payer_id_to_patient_ids)
     
     # Update the crosswalk for payer IDs only, retaining other mappings
     crosswalk['payer_id'] = payer_id_to_details
     
     # Validate payer IDs via API and handle invalid IDs
     validate_and_correct_payer_ids(crosswalk, config)
     
     # Save the initial crosswalk
     if save_crosswalk(config['MediLink_Config']['crosswalkPath'], crosswalk):
-        MediLink_ConfigLoader.log("Crosswalk initialized with mappings for {} payers.".format(len(crosswalk.get('payer_id', {}))), config, level="INFO")
+        message = "Crosswalk initialized with mappings for {} payers.".format(len(crosswalk.get('payer_id', {})))
+        print(message)
+        MediLink_ConfigLoader.log(message, config, level="INFO")
     else:
         print("Failed to save the crosswalk.")
         sys.exit(1)
     return payer_id_to_details
 
 def crosswalk_update(config, crosswalk):
     """
@@ -115,25 +153,25 @@
         config (dict): Configuration dictionary containing paths and other settings.
         crosswalk (dict): Existing crosswalk mapping Payer IDs to sets of Insurance IDs.
 
     Returns:
         bool: True if the crosswalk was successfully updated and saved, False otherwise.
     """    
     # Load insurance mappings from MAINS (Insurance Name to Insurance ID)
-    insurance_name_to_id = load_insurance_data_from_mains(config)
+    insurance_name_to_id = MediBot_Preprocessor_lib.load_insurance_data_from_mains(config)
     MediLink_ConfigLoader.log("Loaded insurance data from MAINS...")
     
     # Load new Patient ID to Payer ID mappings from Carol's CSV (if necessary)
     # TODO This is a low performance strategy.
-    patient_id_to_payer_id = load_historical_payer_to_patient_mappings(config)
+    patient_id_to_payer_id = MediBot_Preprocessor_lib.load_historical_payer_to_patient_mappings(config)
     MediLink_ConfigLoader.log("Loaded historical mappings...")
   
     # Load incremental mapping data from Z.dat (Patient ID to Insurance Name)
     # TODO This may be a redundant approach?
-    patient_id_to_insurance_name = parse_z_dat(config['MediLink_Config']['Z_DAT_PATH'], config['MediLink_Config'])
+    patient_id_to_insurance_name = MediBot_Preprocessor_lib.parse_z_dat(config['MediLink_Config']['Z_DAT_PATH'], config['MediLink_Config'])
     MediLink_ConfigLoader.log("Parsed Z data...")
 
     # Update the crosswalk with new or revised mappings
     for patient_id, payer_id in patient_id_to_payer_id.items():
         insurance_name = patient_id_to_insurance_name.get(patient_id)
         if insurance_name and insurance_name in insurance_name_to_id:
             insurance_id = insurance_name_to_id[insurance_name]
@@ -178,15 +216,15 @@
     
     # Save the updated crosswalk
     return save_crosswalk(config['MediLink_Config']['crosswalkPath'], crosswalk)
 
 def update_crosswalk_with_new_payer_id(insurance_name, payer_id, config):
     """Updates the crosswalk with a new payer ID."""
     _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
-    medisoft_id = load_insurance_data_from_mains(config).get(insurance_name)
+    medisoft_id = MediBot_Preprocessor_lib.load_insurance_data_from_mains(config).get(insurance_name)
     
     if medisoft_id:
         medisoft_id_str = str(medisoft_id)
         if payer_id not in crosswalk['payer_id']:
             crosswalk['payer_id'][payer_id] = {"medisoft_id": [medisoft_id_str], "medisoft_medicare_id": []}
         else:
             crosswalk['payer_id'][payer_id]['medisoft_id'].append(medisoft_id_str)
```

### Comparing `medicafe-0.240515.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240515.1/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240515.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,17 +173,17 @@
                     crosswalk['payer_id'] = {}
                 crosswalk['payer_id'][ins1_payer_id] = {
                     'medisoft_id': [],
                     'medisoft_medicare_id': [],
                     'endpoint': 'OPTUMEDI' # Default probably should be a flag for the crosswalk update function to deal with. BUG HARDCODE THERE ARE 3 of these defaults
                 } 
 
-def load_data_sources(config):
+def load_data_sources(config, crosswalk):
     """Loads historical mappings from MAPAT and Carol's CSVs."""
-    patient_id_to_insurance_id = load_insurance_data_from_mapat(config)
+    patient_id_to_insurance_id = load_insurance_data_from_mapat(config, crosswalk)
     if not patient_id_to_insurance_id:
         raise ValueError("Failed to load historical Patient ID to Insurance ID mappings from MAPAT.")
 
     payer_id_to_patient_ids = load_historical_payer_to_patient_mappings(config)
     if not payer_id_to_patient_ids:
         raise ValueError("Failed to load historical Carol's CSVs.")
```

### Comparing `medicafe-0.240515.0/MediBot/MediBot_UI.py` & `medicafe-0.240515.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240515.1/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240515.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/update_json.py` & `medicafe-0.240515.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediBot/update_medicafe.py` & `medicafe-0.240515.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink.py` & `medicafe-0.240515.1/MediLink/MediLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Add parent directory of the project to the Python path
 import sys
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediBot import MediBot_Preprocessor_lib
 load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains
+from MediBot import MediBot_Crosswalk_Library
 
 """
 Development Tasks for Backend Enhancement in MediSoft Claims Submittal (MediLink) Script:
 
 Implement dynamic configurations for multiple endpoints (Availity, Optum, PNT Data) with environmental settings support.
 Enhance file detection with detailed logging and introduce integrity checks for pre-processing validation.
 Verify file transmissions via WinSCP log analysis for successful endpoint acknowledgments and secure data transfer.
@@ -304,19 +305,21 @@
 def main_menu():
     """
     Initializes the main menu loop and handles the overall program flow,
     including loading configurations and managing user input for menu selections.
     """
     # Load configuration settings and display the initial welcome message.
     config, crosswalk = MediLink_ConfigLoader.load_configuration() 
-    # BUG (Low, Config) does this need an argument? Not sure.
     
-    # TODO (Test Mode) Add here a check in config.json for key "MediLink_Config": { "TestMode": true, ...}. If it is true,
-    # prompt the user to say that MediLink is in Test Mode and ask if the user wants to stay in test mode? 
-    # Then put placeholder text for now because I don't know what the logic should be.
+    # Check to make sure payer_id key is available in crosswalk, otherwise, go through that crosswalk initialization flow
+    MediBot_Crosswalk_Library.check_and_initialize_crosswalk(config)
+    
+    # Check if the application is in test mode
+    if config.get("MediLink_Config", {}).get("TestMode", False):
+        print("MEDILINK TEST MODE: To enable full functionality, please update the config file and set 'TestMode' to 'false'.")
     
     # Display Welcome Message
     MediLink_UI.display_welcome()
 
     # Normalize the directory path for file operations.
     directory_path = os.path.normpath(config['MediLink_Config']['inputFilePath'])
```

### Comparing `medicafe-0.240515.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240515.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240515.1/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240515.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from datetime import datetime
-import requests
-import time
 import sys
 from MediLink import MediLink_ConfigLoader
 
 # Add parent directory of the project to the Python path
 import sys
 import os
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediBot import MediBot_Preprocessor_lib
 load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains
 from MediBot import MediBot_Crosswalk_Library
-update_crosswalk_with_corrected_payer_id = MediBot_Crosswalk_Library.update_crosswalk_with_corrected_payer_id
-update_crosswalk_with_new_payer_id = MediBot_Crosswalk_Library.update_crosswalk_with_new_payer_id
+from MediLink_APIs import fetch_payer_name_from_api
 
 """
 - [ ] 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
 - [ ] 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
 - [ ] 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
 - [ ] 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
 - [ ] 5. De-persisting Intermediate Files.
@@ -256,15 +253,15 @@
                     resolved_name = fetch_payer_name_from_api(corrected_payer_id, config, primary_endpoint)
                     print("API resolved to insurance name: {}".format(resolved_name))
                     MediLink_ConfigLoader.log("API Resolved to standard insurance name: {} for corrected payer ID: {}".format(resolved_name, corrected_payer_id), config, level="INFO")
                     
                     confirmation = input("Is the standard insurance name '{}' correct? (yes/no): ".format(resolved_name)).strip().lower()
                     
                     if confirmation in ['yes', 'y']:
-                        if update_crosswalk_with_corrected_payer_id(payer_id, corrected_payer_id):
+                        if MediBot_Crosswalk_Library.update_crosswalk_with_corrected_payer_id(payer_id, corrected_payer_id):
                             return resolved_name
                         else:
                             print("Failed to update crosswalk with the corrected Payer ID.")
                             exit(1) # probably needs a different failure direction here.
                     else:
                         print("User did not confirm the standard insurance name. Manual intervention is required.")
                         MediLink_ConfigLoader.log("User did not confirm the standard insurance name. Manual intervention is required.", config, level="CRITICAL")
@@ -297,14 +294,17 @@
         insurance_name (str): Name of the insurance.
         config (dict): Configuration settings.
 
     Returns:
         str: The payer ID corresponding to the insurance name.
     """
     try:
+        # Ensure crosswalk is initialized and 'payer_id' key is available
+        MediBot_Crosswalk_Library.check_and_initialize_crosswalk(config)
+        
         # Load crosswalk configuration
         _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
         
         # Load insurance data from MAINS to get insurance ID
         insurance_to_id = load_insurance_data_from_mains(config)
         
         # Get medisoft ID corresponding to the insurance name
@@ -315,27 +315,18 @@
             raise ValueError(error_message)
         
         # Convert medisoft_id to string to match the JSON data type
         medisoft_id_str = str(medisoft_id)
         
         # Get payer ID corresponding to the medisoft ID
         payer_id = None
-        try:
-            for payer, payer_info in crosswalk['payer_id'].items():
-                if medisoft_id_str in payer_info['medisoft_id']:
-                    payer_id = payer
-                    break
-        except KeyError:
-            error_message = "The 'payer_id' key does not exist in the crosswalk configuration. " \
-                            "This could be because the crosswalk is not initialized. " \
-                            "Consider running the Crosswalk initializer."
-                            # TODO Can add an optional function call here to the initializer directly.
-                            # initialize_crosswalk_from_mapat(config, crosswalk) but with the full config.
-            MediLink_ConfigLoader.log(error_message, level="ERROR")
-            raise KeyError(error_message)
+        for payer, payer_info in crosswalk['payer_id'].items():
+            if medisoft_id_str in payer_info['medisoft_id']:
+                payer_id = payer
+                break
 
         # Handle the case where no payer ID is found
         if payer_id is None:
             error_message = "No payer ID found for Medisoft ID: {}".format(medisoft_id)
             MediLink_ConfigLoader.log(error_message, config, level="ERROR")
             print(error_message)
             payer_id = handle_missing_payer_id(insurance_name, config)
@@ -382,15 +373,15 @@
         return None
     
     # Ask for user confirmation
     confirmation = input("Is the standard insurance name '{}' correct? (yes/no): ".format(standard_insurance_name)).strip().lower() or 'yes'
     
     if confirmation in ['yes', 'y']:
         # Update the crosswalk with the new payer ID and insurance name mapping
-        update_crosswalk_with_new_payer_id(insurance_name, payer_id, config)
+        MediBot_Crosswalk_Library.update_crosswalk_with_new_payer_id(insurance_name, payer_id, config)
         return payer_id
     else:
         print("User did not confirm the standard insurance name. Manual intervention is required.")
         MediLink_ConfigLoader.log("User did not confirm the standard insurance name. Manual intervention is required.", config, level="CRITICAL")
         return None
 
 def create_nm1_payto_address_segments(config):
```

### Comparing `medicafe-0.240515.0/MediLink/MediLink_APIs.py` & `medicafe-0.240515.1/MediLink/MediLink_APIs.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 
     Raises:
         ValueError: If all endpoints are exhausted without finding the payer.
 
     Returns:
         str: The fetched payer name.
     """
+    # Reload for safety
+    config, _ = MediLink_ConfigLoader.load_configuration()
+    
     # Step 1: Retrieve endpoint configurations
-    endpoints = config['endpoints']
+    endpoints = config['MediLink_Config']['endpoints']
     tried_endpoints = []
 
     # Step 2: Check if the primary endpoint is specified and is valid
     if primary_endpoint and primary_endpoint in endpoints:
         endpoint_order = [primary_endpoint] + [endpoint for endpoint in endpoints if endpoint != primary_endpoint]
     else:
         endpoint_order = list(endpoints.keys())
@@ -34,30 +37,33 @@
     # Step 3: Iterate through available endpoints in specified order
     for endpoint_name in endpoint_order:
         endpoint_config = endpoints[endpoint_name]
         if not all(key in endpoint_config for key in ['token_url', 'client_id', 'client_secret']):
             MediLink_ConfigLoader.log("Skipping {} due to missing API keys.".format(endpoint_name), config, level="WARNING")
             continue
 
-        # Consider abstracting out the API call.
-
         # Step 4: Get access token for the endpoint
         token = get_access_token(endpoint_config)
         api_url = endpoint_config.get("api_url", "")
         headers = {'Authorization': 'Bearer {}'.format(token), 'Accept': 'application/json'}
         params = {'payerId': payer_id}
 
         try:
             # Step 5: Make API call to fetch payer name
             response = requests.get(api_url, headers=headers, params=params)
             response.raise_for_status()
             data = response.json()
             if 'payers' in data and data['payers']:
                 payer = data['payers'][0]
-                return payer.get('displayName') or payer.get('name')
+                payer_name = payer.get('displayName') or payer.get('name')
+                
+                # Log successful match
+                MediLink_ConfigLoader.log("Successfully found payer at {} for ID {}: {}".format(endpoint_name, payer_id, payer_name), config, level="INFO")
+                
+                return payer_name
             else:
                 MediLink_ConfigLoader.log("No payer found at {} for ID: {}. Trying next available endpoint.".format(endpoint_name, payer_id), config, level="INFO")
         except requests.RequestException as e:
             # Step 6: Log API call failure
             MediLink_ConfigLoader.log("API call failed at {} for Payer ID '{}': {}".format(endpoint_name, payer_id, str(e)), config, level="ERROR")
             tried_endpoints.append(endpoint_name)
```

### Comparing `medicafe-0.240515.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240515.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240515.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_Down.py` & `medicafe-0.240515.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240515.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240515.1/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240515.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_UI.py` & `medicafe-0.240515.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/MediLink_Up.py` & `medicafe-0.240515.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/MediLink/test.py` & `medicafe-0.240515.1/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/PKG-INFO` & `medicafe-0.240515.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.0
+Version: 0.240515.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.0/README.md` & `medicafe-0.240515.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240515.1/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.0
+Version: 0.240515.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240515.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.0/setup.py` & `medicafe-0.240515.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240515.0",
+    version="0.240515.1",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

