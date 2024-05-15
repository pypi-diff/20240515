# Comparing `tmp/medicafe-0.240515.1.tar.gz` & `tmp/medicafe-0.240515.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240515.1.tar", last modified: Wed May 15 18:59:00 2024, max compression
+gzip compressed data, was "medicafe-0.240515.2.tar", last modified: Wed May 15 19:54:10 2024, max compression
```

## Comparing `medicafe-0.240515.1.tar` & `medicafe-0.240515.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.670000 medicafe-0.240515.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-15 18:58:59.621000 medicafe-0.240515.1/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14539 2024-05-15 18:56:28.000000 medicafe-0.240515.1/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8605 2024-05-15 16:21:09.000000 medicafe-0.240515.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.402000 medicafe-0.240515.1/MediLink/
--rw-rw-rw-   0        0        0    20303 2024-05-15 18:53:31.000000 medicafe-0.240515.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    41978 2024-05-15 18:52:35.000000 medicafe-0.240515.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.1/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.1/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.1/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-15 18:59:00.619000 medicafe-0.240515.1/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 18:59:00.599000 medicafe-0.240515.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 18:58:58.000000 medicafe-0.240515.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:59:00.665000 medicafe-0.240515.1/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-15 18:58:57.000000 medicafe-0.240515.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.661000 medicafe-0.240515.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:09.639000 medicafe-0.240515.2/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.2/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240515.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8965 2024-05-15 19:49:49.000000 medicafe-0.240515.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.415000 medicafe-0.240515.2/MediLink/
+-rw-rw-rw-   0        0        0    20303 2024-05-15 19:29:00.000000 medicafe-0.240515.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25315 2024-05-14 15:17:10.000000 medicafe-0.240515.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    41978 2024-05-15 18:52:35.000000 medicafe-0.240515.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.2/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.2/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19252 2024-05-15 13:35:59.000000 medicafe-0.240515.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.2/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-15 19:54:10.641000 medicafe-0.240515.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 19:54:10.620000 medicafe-0.240515.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 19:54:08.000000 medicafe-0.240515.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:54:10.656000 medicafe-0.240515.2/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-15 19:54:07.000000 medicafe-0.240515.2/setup.py
```

### Comparing `medicafe-0.240515.1/LICENSE` & `medicafe-0.240515.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot.bat` & `medicafe-0.240515.2/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot.py` & `medicafe-0.240515.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot_Charges.py` & `medicafe-0.240515.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240515.2/MediBot/MediBot_Crosswalk_Library.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,22 @@
     config, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
     
     try:
         # Attempt to access the 'payer_id' key to ensure it exists
         if 'payer_id' not in crosswalk:
             raise KeyError("Missing 'payer_id' key in crosswalk.")
     except KeyError:
-        error_message = "The 'payer_id' key does not exist in the crosswalk configuration. " \
-                        "This could be because the crosswalk is not initialized. " \
+        error_message = "The 'payer_id' key does not exist in the crosswalk configuration. \n" \
+                        "This could be because the crosswalk is not initialized. \n" \
                         "Consider running the Crosswalk initializer."
         print(error_message)
         MediLink_ConfigLoader.log(error_message, config, level="ERROR")
         
         # Prompt user to initialize crosswalk
-        initialize_choice = input("\nADVANCED OPTION: The crosswalk is not initialized. Do you want to initialize it now? (yes/no): ").strip().lower()
+        initialize_choice = input("\nADVANCED OPTION: The crosswalk may not be initialized. \nType 'yes' to initialize it now: ").strip().lower()
         if initialize_choice == 'yes':
             initialize_crosswalk_from_mapat()
             _, crosswalk = MediLink_ConfigLoader.load_configuration() # Reload crosswalk
             MediLink_ConfigLoader.log("Crosswalk reloaded successfully.", config, level="INFO")
         else:
             raise KeyError(error_message)
```

### Comparing `medicafe-0.240515.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240515.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240515.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot_UI.py` & `medicafe-0.240515.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240515.2/MediBot/MediBot_dataformat_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,38 +71,45 @@
 
 def enforce_significant_length(output):
     # Replace spaces with a placeholder that counts as one significant digit
     temp_output = output.replace(' ', '{Space}')
     
     # Check if the number of significant digits exceeds 30
     if len(temp_output) > 30:
+        MediLink_ConfigLoader.log("Address significant length policy enforced...")
         # First line of defense: Replace ' APT ' with ' #' if the original length is longer than 30 characters.
         temp_output = temp_output.replace(' APT ', ' #')
 
-        # Remove spaces from right to left until we reach 30 significant digits or run out of spaces
-        while len(temp_output) > 30 and ' ' in temp_output:
-            temp_output = temp_output.rstrip(' ')
-        
+        # Remove spaces in a controlled manner if still too long
+        while len(temp_output) > 30:
+            # Find the last space
+            last_space_index = temp_output.rfind('{Space}')
+            if last_space_index == -1:
+                break
+            # Remove the last space
+            temp_output = temp_output[:last_space_index] + temp_output[last_space_index+7:]
+
         # If still greater than 30, truncate to 30 characters
         if len(temp_output) > 30:
             temp_output = temp_output[:30]
-    
+
     # Replace placeholder back with actual space for final return
     return temp_output.replace('{Space}', ' ')
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
     # Temporarily disable script pause status
     app_control.set_pause_status(False)
     
-    # Remove period characters and the abbreviation "APT" surrounded by spaces from the input
+    # Remove period characters.
     value = value.replace('.', '')
     
     # Proceed only if there's a comma, indicating a likely full address
     if ',' in value:
         try:
+            MediLink_ConfigLoader.log("Attempting to resolve address via regex...")
             # Retrieve common city names from configuration and prepare a regex pattern
             common_cities = config.get('cities', [])
             city_pattern = '|'.join(re.escape(city) for city in common_cities)
             city_regex_pattern = r'(?P<City>{})'.format(city_pattern)
             city_regex = re.compile(city_regex_pattern, re.IGNORECASE)
 
             # Search for a common city in the address
@@ -143,15 +150,17 @@
             app_control.set_pause_status(True)
             open_csv_for_editing(CSV_FILE_PATH)
             manage_script_pause(csv_data, e, reverse_mapping)
             # Return original value with spaces formatted, enforcing significant length
             return enforce_significant_length(value.replace(' ', '{Space}'))
     else:
         # If no comma is present, treat the input as a simple street name
-        return enforce_significant_length(value.replace(' ', '{Space}'))
+        formatted_value = value.replace(' ', '{Space}')
+        enforced_format = enforce_significant_length(formatted_value)
+        return enforced_format
 
     # Fallback return in case no address components are matched even though a comma was present
     return enforce_significant_length(value.replace(' ', '{Space}')) 
 
 def format_zip(value):
     # Ensure the value is a string, in case it's provided as an integer
     value_str = str(value)
```

### Comparing `medicafe-0.240515.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240515.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/update_json.py` & `medicafe-0.240515.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediBot/update_medicafe.py` & `medicafe-0.240515.2/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink.py` & `medicafe-0.240515.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240515.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240515.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240515.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_APIs.py` & `medicafe-0.240515.2/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240515.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240515.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_Down.py` & `medicafe-0.240515.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240515.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240515.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240515.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_UI.py` & `medicafe-0.240515.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/MediLink_Up.py` & `medicafe-0.240515.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/MediLink/test.py` & `medicafe-0.240515.2/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/PKG-INFO` & `medicafe-0.240515.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.1
+Version: 0.240515.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.1/README.md` & `medicafe-0.240515.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240515.2/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.1
+Version: 0.240515.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240515.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.1/setup.py` & `medicafe-0.240515.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240515.1",
+    version="0.240515.2",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

