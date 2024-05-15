# Comparing `tmp/real_estate_realtor_com_imp_local-0.0.7.tar.gz` & `tmp/real_estate_realtor_com_imp_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real_estate_realtor_com_imp_local-0.0.7.tar", last modified: Tue May 14 17:55:18 2024, max compression
+gzip compressed data, was "real_estate_realtor_com_imp_local-0.0.8.tar", last modified: Wed May 15 00:44:09 2024, max compression
```

## Comparing `real_estate_realtor_com_imp_local-0.0.7.tar` & `real_estate_realtor_com_imp_local-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:18.469488 real_estate_realtor_com_imp_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-14 17:55:18.469488 real_estate_realtor_com_imp_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 17:54:45.000000 real_estate_realtor_com_imp_local-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 17:54:45.000000 real_estate_realtor_com_imp_local-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:18.465488 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:18.465488 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:54:45.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-05-14 17:54:45.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local/src/realtor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:55:18.465488 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-14 17:55:18.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 17:55:18.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:55:18.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 17:55:18.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 17:55:18.000000 real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:55:18.469488 real_estate_realtor_com_imp_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 17:54:45.000000 real_estate_realtor_com_imp_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.362881 real_estate_realtor_com_imp_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/realtor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:44:09.362881 real_estate_realtor_com_imp_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/setup.py
```

### Comparing `real_estate_realtor_com_imp_local-0.0.7/PKG-INFO` & `real_estate_realtor_com_imp_local-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: real-estate-realtor-com-imp-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Real estate python package
 Home-page: https://github.com/circles-zone/real-estate-realtor-com-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: importer-local>=0.0.33
 Requires-Dist: logger-local>=0.0.55
 Requires-Dist: database-mysql-local>=0.0.290
 Requires-Dist: location-local>=0.0.23
 Requires-Dist: entity-type-local>=0.0.12
 Requires-Dist: selenium
-Requires-Dist: pandas
 
 This is a package for sharing common realtor functions used in different repositories
```

### Comparing `real_estate_realtor_com_imp_local-0.0.7/pyproject.toml` & `real_estate_realtor_com_imp_local-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local/src/realtor.py` & `real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/realtor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,349 +1,251 @@
+import os
 import json
 import re
-import time
 
 import mysql.connector
-import pandas as pd
-from database_mysql_local.connector import Connector
-from entity_type_local.entities_type import EntitiesType
+from database_mysql_local.generic_crud import GenericCRUD
+# from data_source_local.data_source_enum import DataSource
+# from entity_type_local.entities_type import EntitiesType
+# from entity_type_local.entity_enum import EntityTypeId
 from importer_local.ImportersLocal import ImportersLocal
 from location_local.country import Country
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from logger_local.LoggerLocal import Logger
 from selenium import webdriver
+from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import NoSuchElementException
-from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
+from python_sdk_remote.utilities import our_get_env
+
+# TODO: move to const
+BASE_URL = "https://www.realtor.com/international/"
+PAGE_LIMIT = 5
+LISTINGS_LIMIT_PER_PAGE = 6  # TODO: Why?
+REALTOR_COM_USER_EXTERNAL_ID = 1
+REAL_ESTATE_ENTITY_ID = 1
+REAL_ESTATE_ENTITY_TYPE_ID = 79
+REAL_ESTATE_DATA_SOURCE_ID = 15
 
 REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_ID = 146
 REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME = 'real-estate-realtor_com-selenium-imp-local-python-package'
 GET_LISTING_LINKS_FROM_LOCATION_FUNCTION_NAME = 'real-estate-realtor_com-selenium-imp-local-python-package/realtor.py get_listing_links_from_location()'
-BASE_URL = "https://www.realtor.com/international/"
-PAGE_LIMIT = 5
-LISTINGS_LIMIT_PER_PAGE = 6
-df = pd.DataFrame(columns=['listing_id', 'agent_name', 'agent_office_phone', 'price', 'property_type', 'land_size',
-                           'building_size', 'num_of_bedrooms', 'num_of_bathrooms'])
 
 logger_code_init = {
     'component_id': REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_ID,
     'component_name': REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'tal@circlez.ai'
 }
 # TODO: meta logger
 logger = Logger.create_logger(object=logger_code_init)
 
 importers_local = ImportersLocal()
 
 
-# TODO: use class
-def get_listing_links_from_location(driver, location):  # TODO: add typing everywhere
-    object_start = {
-        'driver': driver,
-        'location': location
-    }
-    logger.start(GET_LISTING_LINKS_FROM_LOCATION_FUNCTION_NAME, object=object_start)
-    listings = []
-    location_base_url = get_link_from_location(location)
-    for page_num in range(1, PAGE_LIMIT + 1):
-
-        url = location_base_url + f"/p{page_num}"
-        driver.get(url)
-        # Wait for the page to load
-        time.sleep(6)  # TODO: use selenium wait
-        logger.info("get_listing_links_from_location()", object={'url': url})
-        listings += extract_listings_from_listings_page(driver)
-
-        page_num += 1
-    logger.end(GET_LISTING_LINKS_FROM_LOCATION_FUNCTION_NAME,
-               object={'listings': listings})
-    return listings
-
-
-def extract_listings_from_listings_page(driver):
-    object_start = {
-        'driver': driver
-    }
-    logger.start(object=object_start)
-    links = []
-    ul_elements = driver.find_elements(By.CLASS_NAME, "tier-one-listing-table")
-    # ul_next_page_elements = driver.find_elements(By.CLASS_NAME, "pagination-box")
-    for x in ul_elements:
-        li_element = x.find_elements(By.CLASS_NAME, "listing")
-        for i in range(len(li_element)):
-            link = li_element[i].find_element(By.TAG_NAME, "a").get_attribute('href')
-            links.append(link)
-            logger.info("link", object={link: link})
+class Realtor(GenericCRUD):
+    def __init__(self, is_test_data: bool = False) -> None:
+        super().__init__(default_schema_name='marketplace_goods_real_estate',
+                         default_table_name='real_estate_listing_table',
+                         default_view_table_name='real_estate_listing_view',
+                         default_column_name='real_estate_listing_id',
+                         is_test_data=is_test_data)
+        self.country = Country()
+
+        # create a new ChromeDriver instance
+        options = webdriver.ChromeOptions()
+        if not our_get_env('DISABLE_HEADLESS_MODE', raise_if_not_found=False):
+            options.add_argument("--headless")
+        self.driver = webdriver.Chrome(options=options)
+
+    def get_listing_links_from_location(self, location: str) -> list[str]:
+
+        location_base_url = self.get_link_from_location(location)
+        listings = [self.extract_listings_from_listings_page(f"{location_base_url}/p{page_num}")
+                    for page_num in range(1, PAGE_LIMIT + 1)]
+        listings = [item for sublist in listings for item in sublist]
+        return listings
+
+
+    def extract_listings_from_listings_page(self, url: str) -> list[str]:
+        self.driver.get(url)
+        WebDriverWait(self.driver, 5).until(
+            lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-split-view-wrapper"))
+        ul_elements = self.driver.find_elements(By.CLASS_NAME, "listing-split-view-wrapper")
+        links = [elem.find_element(By.TAG_NAME, "a").get_attribute('href')
+                 for elem in ul_elements]
+        # ul_next_page_elements = driver.find_elements(By.CLASS_NAME, "pagination-box")
         # li_next_page_element = ul_next_page_elements.find_element(By.TAG_NAME,"a").get_attribute('href')
-    logger.end(
-        object={'links[:LISTINGS_LIMIT_PER_PAGE]': links[:LISTINGS_LIMIT_PER_PAGE]})
-    return links[:LISTINGS_LIMIT_PER_PAGE]
-
-
-def insert_to_table(connection, cursor, line, location):
-    object_start = {
-        'connection': connection,
-        'cursor': cursor,
-        'line': line,
-        'location': location
-    }
-    logger.start(object=object_start)
-    entity_type_id = EntitiesType.get_entity_type_id_by_name("Real Estate")
-    if not entity_type_id:
-        EntitiesType.insert_entity_type_id_by_name("Real Estate", 1)
-        entity_type_id = EntitiesType.get_entity_type_id_by_name("Real Estate")
-        country_name = Country().get_country_name(location)
-    else:
-        return
-    # TODO replace with a call to location Class location-local-python-package
-    query = """Select location_id from `location`.`location_table` join `location`.`country_table` on `country_table.country_id`=location_id Where iso=%s"""
-    cursor.execute(query, (country_name,))
-    location_id = cursor.fetchone()[0]
-    importers_local.insert(data_source_id=15, location_id=location_id, entity_type_id=entity_type_id,
-                           url=BASE_URL, entity_id=1, user_external_id=1)
-    # Specify the table name
-    # table_name = 'listings'
-    # Create a new record
-    try:
-        dict_values = line.to_dict()
-        if dict_values['agent_office_phone'] == -1:
-            logger.end(object={})
-            return
-        sql = "INSERT INTO listings (listing_id, agent_name, agent_office_phone, price, property_type, land_size,building_size,num_of_bedrooms,num_of_bathrooms) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s)"
-        # Execute the query
-        cursor.execute(sql, tuple(line.to_dict().values()))
-        # the connection is not autocommited by default. So we must commit to save our changes.
-        connection.commit()
-    except Exception as e:
-        if mysql.connector.errors.IntegrityError:
-            logger.error("Duplicate key has detected")
-        logger.exception(object=e)
-        raise e
-
-    # TODO
-    # # Specify the table name
-    # table_name = 'listings'
-    # # Insert the row into the table
-    # line.to_sql(name=table_name, con=engine, if_exists='replace', index=False)
-    # engine.dispose()
-    # with engine.connect() as conn:
-    #     conn.execute(text("SELECT * FROM users")
-
-    # new_row = {'listing_id': listing_id_int, 'agent_name': agent_name, 'agent_office_phone': phone_int,
-    #            'price': price_int, 'property_type': property_type, 'land_size': land_int,
-    #            'building_size': building_size_int, 'num_of_bedrooms': num_bedrooms,
-    #            'num_of_bathrooms': num_bathrooms}
-
-
-def wrapper_extract_data(driver, links):
-    object_start = {
-        'driver': driver,
-        'links': links
-    }
-    logger.start(object=object_start)
-    combined_df = pd.DataFrame()
-    for x in links:
-        logger.info(object={'x': x})
-        driver.get(str(x))
-        title = driver.title
-        # print(title)
-        new_df = extract_data(driver, title)
-        time.sleep(5)
-        pd.set_option('display.max_columns', None)
-        pd.set_option('display.max_rows', None)
-        combined_df = pd.concat([combined_df, new_df], ignore_index=True)
-        # print(combined_df)
-    logger.end(object={'combined_df': combined_df})
-    return combined_df
-
-
-def extract_data(driver, title):
-    object_start = {
-        'driver': str(driver),
-        'title': title
-    }
-    logger.start(object=object_start)
-    try:
-        address = re.findall(r'(\w+(?:-\w+)? (?:\w+,? )+\d+)', title)
-        if address:
-            address = address[0]
-            logger.info(object={'address': address})
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No address id found on page {title}")
-    try:
-        listing_id_element = driver.find_element(By.CLASS_NAME, "listing-id")
-        listing_id = listing_id_element.text
-        listing_id_int = int(listing_id)
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No listing id found on page {title}")
-        listing_id = "N/A"
-        listing_id_int = -1
-    try:
-        agent_name_element = driver.find_element(By.CLASS_NAME, "agent-name")
-        agent_name = agent_name_element.text
-        # print(agent_name)
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No agent name found on page {title}")
-        agent_name = "N/A"
-    try:
-        agent_office_phone_element = driver.find_element(
-            By.CLASS_NAME, "agent-officephone")
-        agent_office_phone = agent_office_phone_element.get_attribute('href')
-        # print(agent_office_phone)
-        office_phone_num_list = re.findall(r'\d+', agent_office_phone)
-        phone_str = ''.join(office_phone_num_list)
-        phone_int = int(phone_str)
-        logger.info(object={'phone_int': phone_int})
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No agent office phone found on page {title}")
-        agent_office_phone = "N/A"
-        phone_int = -1
-    try:
-        price_element = driver.find_element(By.CLASS_NAME, "property-price")
-        price = price_element.text
-        price_list = re.findall(r'\d+', price)
-        price_str = ''.join(price_list)
-        price_int = int(price_str)
-        logger.info(object={'price_int': price_int})
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No property price found on page {title}")
-        price = "N/A"
-        price_int = -1
-    try:
-        property_type_element = driver.find_element(
-            by='css selector', value=".propertyTypes .basicInfoValue")
-        property_type = property_type_element.text
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No property type found on page {title}")
-        property_type = "N/A"
-    try:  # TODO: use selenium.By
-        land_size_element = driver.find_element(
-            by='css selector', value=".landSize .basicInfoValue span")
-        land_size = land_size_element.text
-        building_size_until_point = re.search(
-            r'\d[\d,.]*(?=\.)', land_size).group(0)
-        land_list = re.findall(r'\d+', building_size_until_point)
-        land_str = ''.join(land_list)
-        land_int = int(land_str)
-        logger.info(object={'land_int': land_int})
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No land size found on page {title}")
-        land_size = "N/A"
-        land_int = -1
-    try:
-        building_size_element = driver.find_element(by='xpath',
-                                                    value="//div[text()='Building Size']/following-sibling::div/span")
-        building_size = building_size_element.text
-        building_size_until_point = re.search(
-            r'\d[\d,.]*(?=\.)', building_size).group(0)
-        building_size_list = re.findall(r'\d+', building_size_until_point)
-        building_size_str = ''.join(building_size_list)
-        building_size_int = int(building_size_str)
-        logger.info(object={'building_size_int': building_size_int})
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No building size found on page {title}")
-        building_size = "N/A"
-        building_size_int = -1
-    try:
-        rooms_element = driver.find_element(
-            by='css selector', value=".rooms .basicInfoValue")
-        rooms = rooms_element.text
-        rooms_list = rooms.split(',')
-        num_bedrooms = num_bathrooms = 0
-        for room in rooms_list:
-            room_type = re.findall(r'[a-z]+', room)[0]
-            if room_type.startswith('bath'):
-                num_bathrooms = int(re.findall(r'\d+', room)[0])
-            elif room_type.startswith('bed'):
-                num_bedrooms = int(re.findall(r'\d+', room)[0])
+        return links[:LISTINGS_LIMIT_PER_PAGE]
+
+
+    def insert_to_table(self, curr_location_listings: list[dict], location: str) -> None:
+        country_name = self.country.get_country_name(location)
+        # TODO replace with a call to location Class location-local-python-package
+        query = """
+        SELECT location_id
+        FROM `location`.`location_table` AS location
+                 JOIN `location`.`country_table` AS country ON country.country_id = location.country_id
+        WHERE nicename = %s
+        LIMIT 1"""
+        self.cursor.execute(query, (country_name,))
+        location_id = self.cursor.fetchone()[0]
+        # TODO use data_source and entity_id packages const / enum
+        importers_local.insert(data_source_id=REAL_ESTATE_DATA_SOURCE_ID, location_id=location_id,
+                               entity_type_id=REAL_ESTATE_ENTITY_TYPE_ID, url=BASE_URL, entity_id=REAL_ESTATE_ENTITY_ID,
+                               user_external_id=REALTOR_COM_USER_EXTERNAL_ID)
+
+        try:
+            # remove all rows with agent_office_phone missing values
+            # curr_location_listings = curr_location_listings.dropna(subset=['agent_office_phone'])
+            self.insert_many_dicts(data_dicts=curr_location_listings)
+        except Exception as exception:
+            if mysql.connector.errors.IntegrityError:
+                logger.error("Duplicate key has detected", object=exception)
             else:
-                logger.error("you didn't prepared well")
-                raise Exception("you didn't prepared well")
-    except Exception as e:
-        logger.exception(object=e)
-        if NoSuchElementException:
-            logger.error(f"No rooms found on page {title}")
-        num_bedrooms = -1
-        num_bathrooms = -1
-    logger.info(
-        f"{listing_id = }\n{agent_name = }\n{agent_office_phone = }\n{price = }\n{property_type = }\n{land_size = }\n{building_size = }\n The listing includes:{num_bedrooms = },{num_bathrooms = }")
-    new_row = {'listing_id': listing_id_int, 'agent_name': agent_name, 'agent_office_phone': phone_int,
-               'price': price_int, 'property_type': property_type, 'land_size': land_int,
-               'building_size': building_size_int, 'num_of_bedrooms': num_bedrooms,
-               'num_of_bathrooms': num_bathrooms}
-    # create a new dataframe from the new_row dictionary
-    new_df = pd.DataFrame([new_row])
-    # concatenate the new dataframe to the original dataframe
-    logger.end(object={'new_df': str(new_df)})
-    return new_df
-
-
-def read_locations_from_json():
-    logger.start(object={})
-    with open('locations.json') as f:
-        locations = json.load(f)
-    logger.end(object={'locations["locations"]': locations["locations"]})
-    return locations["locations"]
-
-
-def get_link_from_location(location):
-    object_start = {
-        'location': location
-    }
-    logger.start(object=object_start)
-    link = BASE_URL + location
-    logger.end(object={'link': link})
-    return link
-
-
-def main():
-    logger.start(object={})
-
-    # connect to the database
-    # TODO: use generic crud
-    connection = Connector.connect("marketplace_goods_realestate")
-    # read locations from JSON configuration file
-    locations = read_locations_from_json()
-    cursor = connection.cursor()
-    # create a new ChromeDriver instance
-    # r"C:\Program Files (x86)\WebDriver\chromedriver.exe"
-    service = Service(executable_path='./chromedriver.exe')
-    options = webdriver.ChromeOptions()
-    driver = webdriver.Chrome(service=service, options=options)
-    all_df = pd.DataFrame()
-    try:
+                logger.exception(object=exception)
+                raise exception
+
+        # TODO
+        # # Specify the table name
+        # table_name = 'listings'
+        # # Insert the row into the table
+        # line.to_sql(name=table_name, con=engine, if_exists='replace', index=False)
+        # engine.dispose()
+        # with engine.connect() as conn:
+        #     conn.execute(text("SELECT * FROM users")
+
+        # new_row = {'real_estate_listing_id': real_estate_listing_id_int, 'agent_name': agent_name, 'agent_office_phone': phone_int,
+        #            'price': price_int, 'property_type': property_type, 'land_size': land_int,
+        #            'building_size': building_size_int, 'num_of_bedrooms': num_bedrooms,
+        #            'num_of_bathrooms': num_bathrooms}
+
+
+    def wrapper_extract_data(self, links: list[str]) -> list[dict]:
+        data = [self.extract_data(link) for link in links]            
+        return data
+
+
+    def extract_data(self, link: str) -> dict:
+        # TODO: break to multiple functions
+        agent_office_phone = None
+        price = None
+        property_type = None
+        land_size = None
+        building_size = None
+        num_of_bedrooms = None
+        num_of_bathrooms = None
+        real_estate_listing_id = None
+        agent_name = None
+
+        self.driver.get(link)
+        WebDriverWait(self.driver, 5).until(
+            lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-id"))
+        title = self.driver.title
+        url = self.driver.current_url
+        try:
+            address = re.search(r'(\w+(?:-\w+)? (?:\w+,? )+\d+)', title)
+            if address:
+                address = address.group(0)
+                logger.info(object={'address': address})
+        except NoSuchElementException:
+            logger.warning("No address id found", object={"title": title, "url": url})
+        try:
+            listing_id_element = self.driver.find_element(By.CLASS_NAME, "listing-id")
+            real_estate_listing_id = int(listing_id_element.text)
+        except NoSuchElementException:
+            logger.warning("No listing id found", object={"title": title, "url": url})
+        try:
+            agent_name_element = self.driver.find_element(By.CLASS_NAME, "agent-name")
+            agent_name = agent_name_element.text
+            # print(agent_name)
+        except NoSuchElementException:
+            logger.warning("No agent name found", object={"title": title, "url": url})
+        try:
+            agent_office_phone_element = self.driver.find_element(By.CLASS_NAME, "agent-officephone")
+            agent_office_phone = agent_office_phone_element.get_attribute('href')
+            agent_office_phone = int(''.join(re.findall(r'\d+', agent_office_phone)))
+            logger.info(object={'agent_office_phone': agent_office_phone})
+        except NoSuchElementException:
+            logger.warning("No agent office phone found", object={"title": title, "url": url})
+        try:
+            price_element = self.driver.find_element(By.CLASS_NAME, "property-price")
+            price = int(''.join(re.findall(r'\d+', price_element.text)))
+            logger.info(object={'price': price})
+        except NoSuchElementException:
+            logger.warning("No property price found", object={"title": title, "url": url})
+        try:
+            property_type_element = self.driver.find_element(
+                by='css selector', value=".propertyTypes .basicInfoValue")
+            property_type = property_type_element.text
+        except NoSuchElementException:
+            logger.warning("No property type found", object={"title": title, "url": url})
+        try:  # TODO: use selenium.By
+            land_size_element = self.driver.find_element(
+                by='css selector', value=".landSize .basicInfoValue span")
+            building_size_until_point = re.search(r'\d[\d,.]*(?=\.)', land_size_element.text).group(0)
+            land_size = int(''.join(re.findall(r'\d+', building_size_until_point)))
+            logger.info(object={'land_size': land_size})
+        except NoSuchElementException:
+            logger.warning("No land size found", object={"title": title, "url": url})
+        try:
+            building_size_element = self.driver.find_element(by='xpath',
+                                                        value="//div[text()='Building Size']/following-sibling::div/span")
+            building_size_until_point = re.search(r'\d[\d,.]*(?=\.)', building_size_element.text).group(0)
+            building_size = int(''.join(re.findall(r'\d+', building_size_until_point)))
+            logger.info(object={'building_size': building_size})
+        except NoSuchElementException:
+            logger.warning("No building size found", object={"title": title, "url": url})
+        try:
+            rooms_element = self.driver.find_element(
+                by='css selector', value=".rooms .basicInfoValue")
+            rooms = rooms_element.text
+            rooms_list = rooms.split(',')
+            num_of_bedrooms = num_of_bathrooms = 0
+            for room in rooms_list:
+                room_type = re.findall(r'[a-z]+', room)[0]
+                if room_type.startswith('bath'):
+                    num_of_bathrooms = int(re.findall(r'\d+', room)[0])
+                elif room_type.startswith('bed'):
+                    num_of_bedrooms = int(re.findall(r'\d+', room)[0])
+                else:
+                    logger.error("you didn't prepared well")
+                    raise Exception("you didn't prepared well")
+        except NoSuchElementException:
+            logger.warning("No rooms found", object={"title": title, "url": url})
+        logger.info(
+            f"{real_estate_listing_id = }\n{agent_name = }\n{agent_office_phone = }\n{price = }\n{property_type = }\n{land_size = }\n{building_size = }\n The listing includes:{num_of_bedrooms = },{num_of_bathrooms = }")
+        new_row = {'real_estate_listing_id': real_estate_listing_id, 'agent_name': agent_name,
+                   'agent_office_phone': agent_office_phone, 'price': price, 'property_type': property_type,
+                   'land_size': land_size, 'building_size': building_size, 'num_of_bedrooms': num_of_bedrooms,
+                   'num_of_bathrooms': num_of_bathrooms}
+        return new_row
+
+
+    @staticmethod
+    def read_locations_from_json():
+        suffix = 'locations.json'
+        locations_file = os.path.join(os.path.dirname(__file__), suffix)
+        with open(locations_file) as f:
+            locations = json.load(f)
+        return locations["locations"]
+
+
+    @staticmethod
+    def get_link_from_location(location: str) -> str:
+        link = BASE_URL + location
+        return link
+
+
+    def main_function(self, locations: list[str] = None) -> None:
+        # read locations from JSON configuration file
+        if not locations:
+            locations = self.read_locations_from_json()
         for location in locations:
             # Get the links of all the listings
-            listing_links = get_listing_links_from_location(driver, location)
-            # for listing_link in listing_links:
-            #   extract_listing_data(driver, listing_link)
-            curr_location_listings = wrapper_extract_data(driver, listing_links)
-            for line in curr_location_listings.iterrows():
-                insert_to_table(connection, cursor, line, location)
-            all_df = pd.concat([all_df, curr_location_listings], ignore_index=True)
-            logger.info(object={'all_df': all_df})
-    except Exception as error:
-        logger.exception(object=error)
-    finally:
-        driver.quit()
-        logger.end(object={})
+            listing_links = self.get_listing_links_from_location(location)
+            curr_location_listings = self.wrapper_extract_data(listing_links)
+            self.insert_to_table(curr_location_listings, location)
 
 
-if __name__ == "__main__":
-    main()
+    def __del__(self):
+        self.driver.quit()
```

### Comparing `real_estate_realtor_com_imp_local-0.0.7/real_estate_realtor_com_imp_local.egg-info/PKG-INFO` & `real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: real-estate-realtor-com-imp-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Real estate python package
 Home-page: https://github.com/circles-zone/real-estate-realtor-com-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: importer-local>=0.0.33
 Requires-Dist: logger-local>=0.0.55
 Requires-Dist: database-mysql-local>=0.0.290
 Requires-Dist: location-local>=0.0.23
 Requires-Dist: entity-type-local>=0.0.12
 Requires-Dist: selenium
-Requires-Dist: pandas
 
 This is a package for sharing common realtor functions used in different repositories
```

### Comparing `real_estate_realtor_com_imp_local-0.0.7/setup.py` & `real_estate_realtor_com_imp_local-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 PACKAGE_NAME = "real-estate-realtor-com-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  
-    version='0.0.7', # https://pypi.org/project/real-estate-realtor-com-imp-local/
+    version='0.0.8', # https://pypi.org/project/real-estate-realtor-com-imp-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Real estate python package",
     long_description="This is a package for sharing common realtor functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
@@ -22,10 +22,9 @@
     install_requires=[
         'importer-local>=0.0.33',
         'logger-local>=0.0.55',
         'database-mysql-local>=0.0.290',
         'location-local>=0.0.23',
         'entity-type-local>=0.0.12',
         'selenium',
-        'pandas'
     ],
 )
```

