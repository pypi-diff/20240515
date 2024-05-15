# Comparing `tmp/moobius-1.2.1.tar.gz` & `tmp/moobius-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.2.1.tar", last modified: Wed May  8 03:40:28 2024, max compression
+gzip compressed data, was "moobius-1.2.2.tar", last modified: Wed May 15 17:33:41 2024, max compression
```

## Comparing `moobius-1.2.1.tar` & `moobius-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.503814 moobius-1.2.1/
--rw-rw-rw-   0        0        0     8946 2024-05-08 03:40:28.502841 moobius-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-25 06:01:03.000000 moobius-1.2.1/license.md
--rw-rw-rw-   0        0        0      647 2024-05-08 03:33:36.000000 moobius-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     8091 2024-03-26 23:06:54.000000 moobius-1.2.1/readme.md
--rw-rw-rw-   0        0        0       42 2024-05-08 03:40:28.503814 moobius-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.483356 moobius-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.486276 moobius-1.2.1/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.2.1/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.493088 moobius-1.2.1/src/moobius/core/
--rw-rw-rw-   0        0        0    57654 2024-04-24 21:24:30.000000 moobius-1.2.1/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-05-04 16:47:45.000000 moobius-1.2.1/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.496982 moobius-1.2.1/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.2.1/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4435 2024-04-26 06:18:04.000000 moobius-1.2.1/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.2.1/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.2.1/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9708 2024-04-26 06:18:04.000000 moobius-1.2.1/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.500881 moobius-1.2.1/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.2.1/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    45076 2024-04-24 18:33:19.000000 moobius-1.2.1/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25820 2024-05-04 17:20:19.000000 moobius-1.2.1/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.2.1/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-04-23 19:30:39.000000 moobius-1.2.1/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.501867 moobius-1.2.1/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8946 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.2.1/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.295771 moobius-1.2.2/
+-rw-rw-rw-   0        0        0     8946 2024-05-15 17:33:41.295771 moobius-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-25 06:01:03.000000 moobius-1.2.2/license.md
+-rw-rw-rw-   0        0        0      647 2024-05-15 17:21:00.000000 moobius-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     8091 2024-03-26 23:06:54.000000 moobius-1.2.2/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:33:41.295771 moobius-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.271069 moobius-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.273201 moobius-1.2.2/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.2.2/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.287153 moobius-1.2.2/src/moobius/core/
+-rw-rw-rw-   0        0        0    56973 2024-05-15 16:54:42.000000 moobius-1.2.2/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-05-04 16:47:45.000000 moobius-1.2.2/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.291139 moobius-1.2.2/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.2.2/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4435 2024-04-26 06:18:04.000000 moobius-1.2.2/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.2.2/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.2.2/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9708 2024-05-08 15:46:50.000000 moobius-1.2.2/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.292867 moobius-1.2.2/src/moobius/network/
+-rw-rw-rw-   0        0        0    15108 2024-05-15 04:53:42.000000 moobius-1.2.2/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    45345 2024-05-15 17:24:04.000000 moobius-1.2.2/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25817 2024-05-15 16:56:22.000000 moobius-1.2.2/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7344 2024-05-14 19:33:36.000000 moobius-1.2.2/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7852 2024-05-15 16:48:55.000000 moobius-1.2.2/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:33:41.293719 moobius-1.2.2/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8946 2024-05-15 17:33:41.000000 moobius-1.2.2/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-05-15 17:33:41.000000 moobius-1.2.2/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:33:41.000000 moobius-1.2.2/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-05-15 17:33:41.000000 moobius-1.2.2/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 17:33:41.000000 moobius-1.2.2/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.2.2/src/setup.py
```

### Comparing `moobius-1.2.1/PKG-INFO` & `moobius-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.2.1
+Version: 1.2.2
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.2.1/license.md` & `moobius-1.2.2/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/pyproject.toml` & `moobius-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.2.1/readme.md` & `moobius-1.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/core/sdk.py` & `moobius-1.2.2/src/moobius/core/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         if is_message_down:
             ids2id = self.id2ids_mdown
             id2ids = self.id2ids_mdown
         else:
             ids2id = self.id2ids_mup
             id2ids = self.id2ids_mup
         async with self.alock: # Make sure the old list is stored before the new list is created.
-            if type(character_ids) is str:
-                character_ids = [character_ids]
-            character_ids = list(character_ids)
+            character_ids = utils.to_char_id_list(character_ids)
             if len(character_ids) == 0:
                 return None
             else: # Convert list to a single group id in this mode.
                 massive_str = '_'.join(character_ids)
                 need_new_group = massive_str not in ids2id
                 if need_new_group: # Call /service/group/create
                     character_ids = character_ids.copy()
@@ -364,32 +362,14 @@
             await self.checkin_channel(channel_id)
 
     async def checkin_channel(self, channel_id):
         """This is called on startup and on reconnect"""
         if channel_id == list(self.channels.keys())[0]:
             logger.warning('checkin_channel not overriden, occasional desyncs are possible.')
 
-    async def upload_avatar_and_create_character(self, name, image_path, description):
-        """
-        Upload an avatar image and create a character. Service function.
-
-        Parameters:
-          name: str
-            The name of the character.
-          image_path: str
-            The local path of the avatar image.
-          description: str
-            The description of the character.
-
-        Returns:
-          The created character (Character object).
-        """
-        avatar = await self.http_api.upload_file(image_path)
-        return await self.http_api.create_character(self.client_id, name, avatar, description)
-
     def limit_len(self, txt, n):
         if len(txt)>n:
             txt = txt[0:n]+'...'+str(len(txt))+' chars'
         return txt
 
     async def send_message(self, the_message, channel_id=None, sender=None, recipients=None, subtype=None, len_limit=None, file_display_name=None):
         """
@@ -605,15 +585,15 @@
     async def fetch_popular_channels(self): """Calls self.http_api.fetch_popular_channels."""; return await self.http_api.fetch_popular_channels()
     async def fetch_channel_list(self): """Calls self.http_api.fetch_channel_list."""; return await self.http_api.fetch_channel_list()
     async def fetch_real_character_ids(self, channel_id, raise_empty_list_err=True): """Calls self.http_api.fetch_real_character_ids using self.client_id."""; return await self.http_api.fetch_real_character_ids(channel_id, self.client_id, raise_empty_list_err=raise_empty_list_err)
     async def fetch_character_profile(self, character_id): """Calls self.http_api.fetch_character_profile"""; return await self.http_api.fetch_character_profile(character_id)
     async def fetch_service_id_list(self): """Calls self.http_api.fetch_service_id_list"""; return await self.http_api.fetch_service_id_list()
     async def fetch_service_characters(self): """Calls self.http_api.fetch_service_characters using self.client_id."""; return await self.http_api.fetch_service_characters(self.client_id)
     async def upload_file(self, filepath): """Calls self.http_api.upload_file."""; return await self.http_api.upload_file(filepath)
-    async def download_file(self, url, filepath, assert_no_overwrite=False): """Calls self.http_api.download_file"""; return await self.http_api.download_file(url, filepath, assert_no_overwrite=assert_no_overwrite)
+    async def download_file(self, url, filepath, assert_no_overwrite=False, headers=None): """Calls self.http_api.download_file"""; return await self.http_api.download_file(url, filepath, assert_no_overwrite=assert_no_overwrite, headers=headers)
     async def fetch_message_history(self, channel_id, limit=1024, before="null"): """Calls self.http_api.fetch_message_history."""; return await self.http_api.fetch_message_history(channel_id, limit, before)
     async def create_channel_group(self, channel_id, group_name, members): """Calls self.http_api.create_channel_group."""; return await self.http_api.create_channel_group(channel_id, group_name, members)
     async def create_service_group(self, group_id, members): """Calls self.http_api.create_service_group."""; return await self.http_api.create_service_group(group_id, members)
     async def character_ids_of_channel_group(self, sender_id, channel_id, group_id): """Calls self.http_api.character_ids_of_channel_group"""; return await self.http_api.character_ids_of_channel_group(sender_id, channel_id, group_id)
     async def character_ids_of_service_group(self, group_id): """Calls self.http_api.character_ids_of_service_group"""; return await self.http_api.character_ids_of_service_group(group_id)
     async def update_channel_group(self, channel_id, group_id, members): """Calls self.http_api.update_channel_group."""; return await self.http_api.update_channel_group(channel_id, group_id, members)
     async def update_temp_channel_group(self, channel_id, members): """Calls self.http_api.update_temp_channel_group."""; return await self.http_api.update_temp_channel_group(channel_id, members)
```

### Comparing `moobius-1.2.1/src/moobius/core/wand.py` & `moobius-1.2.2/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/database/database_interface.py` & `moobius-1.2.2/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/database/json_database.py` & `moobius-1.2.2/src/moobius/database/json_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/database/null_database.py` & `moobius-1.2.2/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/database/redis_database.py` & `moobius-1.2.2/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/database/storage.py` & `moobius-1.2.2/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.1/src/moobius/network/asserts.py` & `moobius-1.2.2/src/moobius/network/asserts.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         raise Exception(f'Error in template. Unrecognized template type: {ty}')
     if err1:
         raise PlatformAssertException(f'{err1}; {base_message}; where={path}')
     else:
         return True
 
 
-def optional_dict_template(min_keys, dtemplate):
-    """Creates a template function will not error on missing keys unless missing keys are in min_keys."""
+def min_subset_dict(min_keys, dtemplate):
+    """Creates a template function that will not error on missing keys unless missing keys are in min_keys."""
     dtemplate = dtemplate.copy() # Not sure if necessary.
     def t_fn(d, base_message, path):
         for k in min_keys:
             if k not in dtemplate:
                 raise PlatformAssertException(f'Missing key {k}; {base_message}; where={path}')
         out = True
         for k in d.keys():
@@ -136,24 +136,42 @@
 
 ######################### Specific requests ##########################
 
 def _style_check(style_element, base_message, path):
     """One element in a style vector. This is the most flexible."""
     template_dict = {'widget':'button1','display':'visible', 'text':'<h1>html_tags!</h1>', 'expand':'true', # Expand is a string?
                      'button_hook':{'button_id':'a.button', 'button_text':'A', 'arguments':[]}}
-    template = optional_dict_template([], template_dict)
+    template = min_subset_dict([], template_dict)
     return structure_assert(template, style_element, base_message, path)
+def _context_menu_item_check(cmenu_item, base_message, path):
+    if cmenu_item.get('new_window'):
+        if 'arguments' not in cmenu_item:
+            raise PlatformAssertException(f'context menu item with no arguments but a new_window specified; {base_message}; where={path}')
+        argtemplate = [min_subset_dict(['name', 'type', 'values', 'placeholder'],
+                                              {'name':'the_name', 'type':'enum', 'values':['choice1'],'placeholder':'place',
+                                               'optional':False})]
+        assert_so_far = structure_assert(argtemplate, cmenu_item['arguments'], base_message, path+['arguments'])
+    else:
+        assert_so_far = True
+
+    # Check the non-argument pard
+    cmenu_item = cmenu_item.copy()
+    for k in ['new_window', 'arguments']:
+        if k in cmenu_item:
+            del cmenu_item[k]
+    template = {'item_name':'option 1', 'item_id':'opt1','support_subtype':['txt']}
+    return assert_so_far and structure_assert(template, cmenu_item, base_message, path)
 def _socket_update_body_assert(b, base_message, path):
     """Many requests are updates with a body."""
     subty = b['subtype']
     template = {'subtype':'the_subtype', 'channel_id':'1234...', 'recipients':'1234...'}
     if subty=='update_characters':
         template['content'] = {'characters': '1234... group_id'}
     elif subty=='update_buttons':
-        button_arg_template = optional_dict_template(['name', 'type', 'placeholder', 'optional'], # Values is optional.
+        button_arg_template = min_subset_dict(['name', 'type', 'placeholder', 'optional'], # Values is optional.
                                                      {'name':'opt1', 'type':'enum', 'values':['a'], 'placeholder':'in-situ', 'optional':False})
         def _each_button(x, base_message, the_path):
             each_btn = {'button_id':'pressA', 'button_name':'pressA', 'button_text':'press this A',
                         'new_window':True, 'arguments':[button_arg_template]}
             if not x.get('new_window'):
                 if 'arguments' not in x or x.get('arguments') is None: # Falsey new_window is allowed to have None or missing arguments.
                     del each_btn['arguments']
@@ -162,37 +180,36 @@
                         del x['arguments']
             return structure_assert(each_btn, x, base_message, the_path)
         template['content'] = [_each_button]
     elif subty=='update_channel_info':
         template['content'] = {'channel_id':'123...', 'channel_name':'123...',
                                'context':{'channel_description':'a channel', 'channel_type':'ccs'}}
     elif subty=='update_canvas':
-        template['content'] = [optional_dict_template([], {'path':'url', 'text':'see this text here.'})]
+        template['content'] = [min_subset_dict([], {'path':'url', 'text':'see this text here.'})]
     elif subty=='update_style':
         template['content'] = [_style_check]
     elif subty=='update_context_menu':
-        template['content'] = [{'item_name':'option 1', 'item_id':'opt1',
-                                'support_subtype':['txt']}]
+        template['content'] = [_context_menu_item_check]
         template['context'] = {}
     elif subty=='update_characters':
         template['context'] = {}
         template['content'] = {'characters':'1234...group_id'}
     else:
         raise PlatformAssertException(f'Unrecognized subtype for an update request {subty}; {base_message}.')
     return structure_assert(template, b, base_message, path)
 def _socket_message_body_assert1(b, base_message, path, is_up):
     """Both text and image messages are supported."""
     subty = b['subtype']
     template = {'subtype':'the_subtype', 'channel_id':'1234...', 'recipients':'1234... group_id',
                 'timestamp':12334567, 'context':{}}
     if not is_up:
         template['sender'] = '1234...'
-    if 'recipients' in base_message and base_message['recipients'] is None: # Accept None type.
-        base_message = base_message.copy()
-        base_message['recipients'] = 'noooone'
+    if 'recipients' in b and b['recipients'] is None: # Accept None type.
+        b = b.copy()
+        b['recipients'] = 'noooone'
     if subty in [types.TEXT, types.IMAGE, types.AUDIO, types.FILE]:
         content = b['content'].copy()
         if not content.get('path') and subty != types.TEXT:
             raise PlatformAssertException(f'File-bearing message body has no/None path; {base_message}.')
         for k in ['text', 'path', 'filename', 'size']:
             if k in content:
                 if content[k] is None:
@@ -220,15 +237,15 @@
     template = {'button_id':'button1', 'channel_id':'1234...',
                 'arguments':[{'name':'category', 'value':'A'}],
                 'context':{}}
     return structure_assert(template, b, base_message, path)
 def _context_menuclick_body_assert(b, base_message, path):
     """Right click context menu click"""
     template = {'item_id':'item1', 'channel_id':'1234...', 'message_id':'1234...', 'message_subtype':'text/file/etc',
-                'message_content':optional_dict_template([], {'text':'text!', 'image':'url'}), 'context':{}}
+                'message_content':min_subset_dict([], {'text':'text!', 'image':'url'}), 'context':{}}
     return structure_assert(template, b, base_message, path)
 def _action_body_assert(b, base_message, path):
     """Various actions"""
     subty = b['subtype']
     template = {'subtype':'the_subtype', 'channel_id':'1234...', 'context':{}}
     if subty.startswith('fetch_') or subty=='leave_channel':
         pass
```

### Comparing `moobius-1.2.1/src/moobius/network/http_api_wrapper.py` & `moobius-1.2.2/src/moobius/network/http_api_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # aiohttp-based wrapper of the Platform's HTTP.
-import json, os
+import json, os, io
 import aiohttp
 from loguru import logger
 from dacite import from_dict
 from moobius import utils
 from moobius.types import Character, Group, UserInfo
 from moobius.network import asserts
 # TODO: refresh
@@ -209,18 +209,16 @@
         c_data['character_context'] = resp_data['character_context']
         c_data['avatar'] = resp_data['character_context']['avatar']
         c_data['description'] = resp_data['character_context']['description']
         return from_dict(data_class=Character, data=c_data)
 
     async def fetch_character_profile(self, character_id):
         """Returns a Character object (or list) given a string-valued (or list-valued) character_id."""
-        is_list = True
-        if type(character_id) is str:
-            is_list = False
-            character_id = [character_id]
+        is_list = type(character_id) not in [str, Character]
+        character_id = utils.to_char_id_list(character_id)
         for cid in character_id:
             asserts.types_assert(str, character_id_element=cid)
         response_dict = await self.checked_post(url=self.http_server_uri + "/character/fetch_profile", the_request={"character_list": character_id}, requests_kwargs={'headers':self.headers}, good_message=None, bad_message="Error fetching user profile", raise_errors=True)
         characters = [self._xtract_character(d) for d in response_dict['data']]
         return characters if is_list else characters[0]
 
     async def fetch_real_character_ids(self, channel_id, service_id, raise_empty_list_err=True):
@@ -335,19 +333,26 @@
         """
         Creates a character with given name, avatar, and description.
         The created user will be bound to the given service.
 
         Parameters:
           service_id (str): The service_id/client_id.
           name (str): The name of the user.
-          avatar (str): The image URL of the user's picture/
+          avatar (str): The image URL of the user's picture OR the local file path.
           description (str): The description of the user.
 
         Returns: A Character object representing the created user, None if doesn't receive a valid response (error condition). TODO: Should these error conditions jsut raise Exceptions instead?
         """
+        if 'https://' in avatar or 'http://' in avatar or 'ftp://' in avatar or 'ftps://' in avatar:
+            pass
+        elif not os.path.exists(avatar):
+            raise Exception(f'Cannot find this local file to upload: {os.path.realpath(avatar)}')
+        else:
+            avatar = await self.upload_file(avatar)
+
         jsonr = {"service_id": service_id,
                  "context": {
                    "name": name,
                    "avatar": avatar,
                    "description": description}}
         asserts.types_assert(str, service_id=service_id, avatar=avatar, description=description, name=name)
         response_dict = await self.checked_post(url=self.http_server_uri + "/service/character/create", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message="Successfully created character", bad_message="Error creating character", raise_errors=True)
@@ -355,22 +360,24 @@
         return character
 
     async def update_character(self, service_id, character_id, avatar, description, name):
         """Updates the user info for a FAKE user, for real users use update_current_user.
 
            Parameters:
              service_id (str): Which service holds the user.
-             character_id (str): Of the user.
+             character_id (str): Of the user. Can also be a Character. Cannot be a list.
              avatar (str): Link to user's image.
              description (str): Description of user.
              name (str): The name that shows in chat.
 
            Returns:
             Data about the user as a dict.
         """
+        if type(character_id) is Character:
+            character_id = character_id.character_id
         asserts.types_assert(str, service_id=service_id, character_id=character_id, description=description, name=name, avatar=avatar)
         the_request = {"service_id": service_id, 'character_id':character_id, 'context': {'avatar':avatar, 'description':description, 'name':name}}
         response_dict = await self.checked_post(url=self.http_server_uri + f"/service/character/update", the_request=the_request, requests_kwargs={'headers':self.headers}, good_message="Successfully updated character info", bad_message="Error updating character info", raise_errors=True)
         return response_dict.get('data')
 
     ############################# Channel ############################
 
@@ -516,27 +523,38 @@
             # Exception will be raised in _do_upload_file(), no need to raise here
             full_url = await self._do_upload_file(upload_url, upload_fields, file_path)
             return full_url
         else:
             logger.error(f"Error getting upload url and upload fields! file_path: {file_path}")
             raise Exception(f"Error getting upload url and upload fields! file_path: {file_path}")
 
-    async def download_file(self, url, filename, assert_no_overwrite=False):
-        """Downloads a file from url to filename, automatically creating dirs and overwriting pre-existing files."""
-        requests_kwargs={'headers':self.headers} # Auth allows downloading form buckets we authed for.
+    async def download_file(self, url, filename=None, assert_no_overwrite=False, headers=None):
+        """Downloads a file from url to filename, automatically creating dirs and overwriting pre-existing files.
+        If filename is None will return the bytes and not save any file."""
+        if headers is None: # These buckets are public so no need to upload.
+            headers = {}
+        if headers == 'self':
+            headers={'headers':self.headers} # Auth allows downloading form buckets we authed for.
         # https://stackoverflow.com/questions/35388332/how-to-download-images-with-aiohttp
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, **requests_kwargs) as resp:
+            async with session.get(url, **headers) as resp:
                 if resp.status == 200:
-                    if os.path.exists(filename) and assert_no_overwrite:
-                        raise Exception(f'Assert no overwrite to pre-existing file: {os.path.realpath(filename)}')
-                    os.makedirs(os.path.dirname(filename), exist_ok=True)
-                    with open(filename, 'wb') as fd:
+                    if filename:
+                        os.makedirs(os.path.dirname(filename), exist_ok=True)
+                        if os.path.exists(filename) and assert_no_overwrite:
+                            raise Exception(f'Assert no overwrite to pre-existing file: {os.path.realpath(filename)}')
+                        with open(filename, 'wb') as fd:
+                            async for chunk in resp.content.iter_chunked(10):
+                                fd.write(chunk)
+                    else:
+                        buffer = io.BytesIO()
                         async for chunk in resp.content.iter_chunked(10):
-                            fd.write(chunk)
+                            buffer.write(chunk)
+                        buffer.seek(0)
+                        return buffer.getvalue()
                 else:
                     raise Exception(f'Cannot download file: {resp}')
 
     ############################# Groups ############################
 
     async def fetch_channel_group_dict(self, channel_id, service_id):
         """Like fetch_real_character_ids but returns a dict from group_id to all characters."""
@@ -557,31 +575,32 @@
         asserts.types_assert(str, channel_id=channel_id, service_id=service_id)
         params = {"channel_id": channel_id, "service_id": service_id}
         rkwargs = {'params':params, 'headers':self.headers}
 
         response_dict = await self.checked_get(url=self.http_server_uri + "/user/group/list", the_request=None, requests_kwargs=rkwargs, good_message="Successfully fetched channel group list", bad_message="Error fetching channel group list", raise_errors=True)
         return response_dict['data']
 
-    async def create_channel_group(self, channel_id, group_name, characters):
+    async def create_channel_group(self, channel_id, group_name, character_ids):
         """
         Creates a channel group.
 
         Parameters:
           channel_id (str): The id of the group leader?
           group_name (str): What to call it.
           characters (list): A list of channel_id strings that will be inside the group.
 
         Returns:
           The group id string.
         """
+        character_ids = utils.to_char_id_list(character_ids) # Should not be necessary since this function is an internal function.
         asserts.types_assert(str, channel_id=channel_id, group_name=group_name)
-        asserts.structure_assert(['the_id'], characters, 'Create channel group characters')
-        jsonr = {"channel_id": channel_id, "group_name":group_name, "characters": characters}
+        asserts.structure_assert(['the_id'], character_ids, 'Create channel group characters')
+        jsonr = {"channel_id": channel_id, "group_name":group_name, "characters": character_ids}
         response_dict = await self.checked_post(url=self.http_server_uri + "/user/group/create", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message="Successfully created channel group {group_name}!", bad_message="Error creating channel group {group_name}", raise_errors=True)
-        return from_dict(data_class=Group, data={'group_id': response_dict['data']['group_id'], 'character_ids':characters})
+        return from_dict(data_class=Group, data={'group_id': response_dict['data']['group_id'], 'character_ids':character_ids})
 
     async def character_ids_of_service_group(self, group_id):
         """
         Gets a list of character ids belonging to a service group.
         Note that the 'recipients' in 'on message up' might be None:
           This function will return an empty list given Falsey inputs or Falsey string literals.
         """
@@ -618,64 +637,59 @@
             response_dict = await self.checked_get(url=self.http_server_uri + f"/user/group", the_request=the_json, requests_kwargs={'headers':self.headers}, good_message="Successfully fetched channel group roster!", bad_message="Error fetching channel group roster", raise_errors=True)
         logger.info(f'List character IDs of channel group HTTP response: {response_dict}')
         if len(response_dict['data']) == 0:
             logger.warning(f'This group, if channel group, seems to have no character ids in it: {group_id}')
             return []
         return response_dict['data']['characters']
 
-    async def create_service_group(self, characters):
+    async def create_service_group(self, character_ids):
         """
         Create a group containing characters id list, returning a Group object.
         Sending messages down for the new .net API requires giving myGroup.group_id instead of a list of character_ids.
 
         Parameters:
           group_name (str): What to call it.
-          characters (list): A list of character_id strings that will be inside the group.
+          character_ids (list): A list of character_id strings or Characters that will be inside the group.
 
         Returns:
           A Group object."""
-        if type(characters) is not list:
-            raise Exception('Create service group expects a list of strings.')
-        asserts.structure_assert(['the_id'], characters, 'Create service group characters')
-        jsonr = {"group_id": "", "characters": characters}
+        character_ids = utils.to_char_id_list(character_ids) # Should not be necessary since this function is an internal function.
+        asserts.structure_assert(['the_id'], character_ids, 'Create service group characters')
+        jsonr = {"group_id": "", "characters": character_ids}
         response_dict = await self.checked_post(url=self.http_server_uri + "/service/group/create", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message="Successfully created service group!", bad_message="Error creating service group", raise_errors=True)
         group_id = response_dict['data']
         if type(group_id) is not str:
             raise Exception('The group id returned was not a string.')
-        group = from_dict(data_class=Group, data={'group_id': group_id, 'character_ids':characters})
+        group = from_dict(data_class=Group, data={'group_id': group_id, 'character_ids':character_ids})
         return group
 
     async def update_channel_group(self, channel_id, group_id, members):
         """
         Updates a channel group.
 
         Parameters:
           channel_id (str): The id of the group leader?
           group_name (str): What to call it.
-          members (list): A list of channel_id strings that will be inside the group.
+          members (list): A list of character_id strings that will be inside the group.
 
         No return value.
         """
-        raise Exception('Group functions are not yet fully supported in the platform. Once supported remove this and all other group-not-supported exceptions in http_api_wrapper.py')
-        jsonr = {"channel_id": channel_id, "group_id":group_id, "members": members}
-        await self.checked_post(url=self.http_server_uri + "/user/group/update", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message="Successfully updated channel group {group_name}!", bad_message="Error updating channel group {group_name}", raise_errors=True)
+        raise Exception('Unknown if this function is needed.')
 
     async def update_temp_channel_group(self, channel_id, members):
         """
         Updates a channel TEMP group.
 
         Parameters:
           channel_id (str): The id of the group leader?
-          members (list): A list of channel_id strings that will be inside the group.
+          members (list): A list of character_id strings that will be inside the group.
 
         No return value.
         """
-        raise Exception('Group functions are not yet fully supported in the platform. Once supported remove this and all other group-not-supported exceptions in http_api_wrapper.py')
-        jsonr = {"channel_id": channel_id, "members": members}
-        await self.checked_post(url=self.http_server_uri + "/user/group/temp", the_request=jsonr, requests_kwargs={'headers':self.headers}, good_message="Successfully updated channel group {group_name}!", bad_message="Error updating channel group {group_name}", raise_errors=True)
+        raise Exception('Unknown if this function is needed.')
 
     async def fetch_channel_temp_group(self, channel_id, service_id):
         """Like fetch_channel_group_list but for Temp groups."""
         asserts.types_assert(str, channel_id=channel_id, service_id=service_id)
         params = {"channel_id": channel_id, "service_id": service_id}
         rkwargs = {'params':params, 'headers':self.headers}
```

### Comparing `moobius-1.2.1/src/moobius/network/ws_client.py` & `moobius-1.2.2/src/moobius/network/ws_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,22 +225,22 @@
             }
         }
         if not dry_run:
             await self.send(message)
         return message
 
     #################################### Updating ########################################
-    async def update_character_list(self, service_id, channel_id, character_list, recipients, *, dry_run=False):
+    async def update_character_list(self, service_id, channel_id, characters, recipients, *, dry_run=False):
         """
         Constructs and sends the update message for user list.
 
         Parameters:
           service_id (str): As always.
           channel_id (str): The channel id.
-          character_list (list): The list of character_id strings to be updated.
+          characters (str): The group id to represent the characters who are updated.
           recipients (str): The group id to send to.
           dry_run=False: if True don't acually send the message (messages are sent in thier JSON-strin format).
 
         Returns:
           The message as a dict.
         """
         if not recipients:
@@ -249,15 +249,15 @@
             "type": "update",
             "request_id": str(uuid.uuid4()),
             "service_id": service_id,
             "body": {
                 "subtype": "update_characters",
                 "channel_id": channel_id,
                 "recipients": recipients,
-                "content":{"characters": character_list}
+                "content":{"characters": characters}
             }
         }
         if not dry_run:
             await self.send(message)
         return message
 
     async def update_buttons(self, service_id, channel_id, buttons, recipients, *, dry_run=False):
```

### Comparing `moobius-1.2.1/src/moobius/types.py` & `moobius-1.2.2/src/moobius/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,39 +96,42 @@
 
 @dataclass
 @add_str_method
 class ContextMenuElement: # A single item in a context menu. This will likely be expanded upon with more features.
     item_name: str # How it appears.
     item_id: str # An id choosen by the CCS app to identify which choice was selected.
     support_subtype: list[str] # What message types will open the context menu. ["text","file", etc].
-
+    new_window: Optional[bool] = False
+    arguments: Optional[list[ButtonArgument]] = None
 
 @dataclass
 @add_str_method
 class MessageContent:
     text: Optional[str] = None # Used for text messages.
     path: Optional[str] = None # Used for every kind of non-text message.
     size: Optional[int] = None # Used for downloadable files only.
     filename: Optional[str] = None # Used for downloadable files only (the display filename).
     link: Optional[str] = None # For "card" messages
     title: Optional[str] = None # For "card" messages
     button: Optional[str] = None # For "card" messages
     text: Optional[str] = None # For "card" messages
 
+
 @dataclass
 @add_str_method
 class MenuClick: # Right-click context menu.
     item_id: str
     message_id: str
     message_subtype: str # 'text', 'image', 'audio', or 'file'
     message_content: MessageContent
     channel_id: str
     sender: str
     recipients: list[str]
     context: dict # Rarely used by CCS apps.
+    arguments: Optional[list[ButtonClickArgument]] = None # If the context menu has itself menus.
 
 
 @dataclass
 @add_str_method
 class CanvasElement: # Updates to the Canvas are lists of CanvasElements.
     text: Optional[str] = None
     path: Optional[str] = None
```

### Comparing `moobius-1.2.1/src/moobius/utils.py` & `moobius-1.2.2/src/moobius/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # MISC functions TODO: Just move these to a better place, having a MISC category isn't clean code.
 import sys, os, re, json, threading, asyncio, dataclasses
+from moobius import types
 from loguru import logger
 
 
 class EnhancedJSONEncoder(json.JSONEncoder):
     """Json Encoder but with automatic conversion of dataclasses to dict."""
     def default(self, o):
         if dataclasses.is_dataclass(o):
@@ -149,7 +150,18 @@
                     if field=='channels': # Allow inputing multible channels.
                         args['channels'] = list(args['channels'].split(' '))
                 template[field] = args[field]
 
             os.makedirs(os.path.split(fname)[0], exist_ok=True)
             with open(fname,'w', encoding='utf-8') as f:
                 f.write(json.dumps(template, indent=4, ensure_ascii=False))
+
+
+def to_char_id_list(c):
+    """Converts c to a list of character_ids.
+    x can be a string, a list of strings (idempotent), a list of Character, a Character.
+    lists can actually be tuples or generators etc."""
+    if type(c) is str or type(c) is types.Character:
+        c = [c]
+    c = list(c)
+    c = [ch.character_id if type(ch) is types.Character else ch for ch in c] # Convert Character objects to IDs.
+    return c
```

### Comparing `moobius-1.2.1/src/moobius.egg-info/PKG-INFO` & `moobius-1.2.2/src/moobius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.2.1
+Version: 1.2.2
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.2.1/src/moobius.egg-info/SOURCES.txt` & `moobius-1.2.2/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

