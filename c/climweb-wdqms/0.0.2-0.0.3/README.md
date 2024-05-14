# Comparing `tmp/climweb_wdqms-0.0.2.tar.gz` & `tmp/climweb_wdqms-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climweb_wdqms-0.0.2.tar", last modified: Sun May 12 01:27:23 2024, max compression
+gzip compressed data, was "climweb_wdqms-0.0.3.tar", last modified: Tue May 14 19:51:01 2024, max compression
```

## Comparing `climweb_wdqms-0.0.2.tar` & `climweb_wdqms-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/fetch_transmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-12 01:27:23.858836 climweb_wdqms-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.536323 climweb_wdqms-0.0.3/climweb_wdqms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/climweb_wdqms/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/climweb_wdqms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/management/commands/fetch_transmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/climweb_wdqms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/climweb_wdqms/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 19:51:01.000000 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 19:51:01.000000 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:51:01.000000 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 19:51:01.000000 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 19:51:01.000000 climweb_wdqms-0.0.3/climweb_wdqms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 19:50:57.000000 climweb_wdqms-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-14 19:51:01.540323 climweb_wdqms-0.0.3/setup.cfg
```

### Comparing `climweb_wdqms-0.0.2/PKG-INFO` & `climweb_wdqms-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.2
+Version: 0.0.3
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms/management/commands/fetch_transmissions.py` & `climweb_wdqms-0.0.3/climweb_wdqms/management/commands/fetch_transmissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,160 +57,169 @@
         df_filtered = df_filtered.copy()
         df_filtered['received_rate'] = (df_filtered['#received'] / df_filtered['#expected']) * 100
          # Group by 'name' and select the row with the highest 'received rate'
         max_rate_indices = df_filtered.groupby('wigosid')['received_rate'].idxmax()
         df_filtered = df_filtered.loc[max_rate_indices]
         df_filtered.replace([np.inf, -np.inf], 0, inplace=True)
 
-        # os.remove(file_name)
+        os.remove(file_name)
         return df_filtered
 
     else:
         print("Failed to retrieve data. Status code:", response.status_code)
 
 def generate_date_range(start_date, end_date):
     dates = []
     current_date = datetime.strptime(start_date, "%Y-%m-%d")
     while current_date <= datetime.strptime(end_date, "%Y-%m-%d"):
         dates.append(current_date.strftime('%Y-%m-%d'))
         current_date += timedelta(days=1)
     return dates
 
 
-def ingest_transmission_rates(start_date, end_date,variable, periods, centers, country_code):
+def ingest_transmission_rates(start_date, end_date,variables, periods, centers, country_code):
     dates = generate_date_range(start_date, end_date)
     baseline = "OSCAR" 
 
-    for date in dates:
-        for period in periods:
-            trans_rates = download_transmission_rate_csv(date, period, variable, centers, baseline, country_code)
-
-            print(f"INGEST: Starting data ingestion for {date}-{period}")
-
-            # Create or update stations
-            stations_to_create = []
-            for _, row in trans_rates.iterrows():
-                station_data = {
-                    'wigos_id': row['wigosid'],
-                    'name': row['name'],
-                    'geom':Point(row['longitude'], row['latitude']),
-                    'in_oscar':row['in OSCAR']
-                }
-                
-                stations_to_create.append(Station(**station_data))
+    for variable in variables:
+        print(f"INGEST: Ingesting {variable.upper()}...")
+        variable = variable.lower()
+        for date in dates:
+            for period in periods:
+                trans_rates = download_transmission_rate_csv(date, period, variable, centers, baseline, country_code)
 
+                print(f"INGEST: Starting data ingestion for {date}-{period}")
 
-            # Bulk create new stations
-            Station.objects.bulk_create(stations_to_create, ignore_conflicts=True)
+                # Create or update stations
+                stations_to_create = []
+                for _, row in trans_rates.iterrows():
+                    station_data = {
+                        'wigos_id': row['wigosid'],
+                        'name': row['name'],
+                        'geom':Point(row['longitude'], row['latitude']),
+                        'in_oscar':row['in OSCAR']
+                    }
+                    
+                    stations_to_create.append(Station(**station_data))
 
-            # Create or update transmissions
-            transmissions_to_create = []
-            for _, row in trans_rates.iterrows():
 
-                if Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).exists():
-                    transmission_data = {
-                        'received_rate':row['received_rate'],
-                        'received':row['#received'],
-                        'expected':row['#expected'],
-                    }
-                    Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).update(**transmission_data)
+                # Bulk create new stations
+                Station.objects.bulk_create(stations_to_create, ignore_conflicts=True)
 
-                else:
-                    station = Station.objects.get(wigos_id=row['wigosid'])
-                    transmissions_to_create.append(Transmission(
-                        station=station,
-                        variable=row['variable'],
-                        received_rate=row['received_rate'],
-                        received=row['#received'],
-                        expected=row['#expected'],
-                        received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')
-                    ))
+                # Create or update transmissions
+                transmissions_to_create = []
+                for _, row in trans_rates.iterrows():
+
+                    if Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).exists():
+                        transmission_data = {
+                            'received_rate':row['received_rate'],
+                            'received':row['#received'],
+                            'expected':row['#expected'],
+                        }
+                        Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).update(**transmission_data)
+
+                    else:
+                        station = Station.objects.get(wigos_id=row['wigosid'])
+                        transmissions_to_create.append(Transmission(
+                            station=station,
+                            variable=row['variable'],
+                            received_rate=row['received_rate'],
+                            received=row['#received'],
+                            expected=row['#expected'],
+                            received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')
+                        ))
 
-            # Bulk create new transmissions
-            Transmission.objects.bulk_create(transmissions_to_create, ignore_conflicts=True)
-            
-            print(f"INGEST: Completed ingestion for {date}-{period}")
+                # Bulk create new transmissions
+                Transmission.objects.bulk_create(transmissions_to_create, ignore_conflicts=True)
+                
+                print(f"INGEST: Completed ingestion for {date}-{period}")
 
 
 
 class Command(BaseCommand):
     help = ('Fetch Country level transmission rate from WDQMS')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def add_arguments(self, parser):
         parser.add_argument('-s', '--start_date', type=str, help='Start date of transmission. format YYYY-MM-DD') 
         parser.add_argument('-e', '--end_date', type=str, help='End date of transmission. format YYYY-MM-DD') 
-        parser.add_argument('-var', '--variable', type=str, help='Accepted variables one of pressure,temperature, humidity, meridional_wind, zonal_wind') 
+        parser.add_argument('-var', '--variables', nargs='+', type=str, help='List of variables e.g pressure,temperature, humidity, meridional_wind, zonal_wind') 
         parser.add_argument('-p', '--periods', nargs='+', type=str, help='List of synoptic hours e.g 00, 06, 12, 18') 
         parser.add_argument('-c', '--centers', nargs='+', type=str, help='List of monitoring centers e.g DWD, ECMWF, JMA, NCEP') 
 
         # Arguments are not added here since they will be parsed manually
         return
 
     def handle(self, *args, **kwargs):
 
-        start_date = kwargs['start_date'] if kwargs['start_date'] is not None else self.stderr.write(self.style.ERROR(f"Missing start_date (-s) arguement. Accepts YYYY-MM-DD"))
-        end_date = kwargs['end_date'] if kwargs['end_date'] is not None else self.stderr.write(self.style.ERROR(f"Missing end_date (-e) arguement. Accepts YYYY-MM-DD"))
-        periods = kwargs['periods'] if kwargs['periods'] is not None else self.stderr.write(self.style.ERROR(f"Missing period (-p) arguement. Accepts 00, 06, 12, 18"))
-        centers = kwargs['centers'] if kwargs['periods'] is not None else self.stderr.write(self.style.ERROR(f"Missing centers (-c) arguement. Accepts DWD, ECMWF, JMA, NCEP"))
-        variable = kwargs['variable'].lower() if kwargs['periods'] is not None else self.stderr.write(self.style.ERROR(f"Missing centers (-var) arguement. Accepts one of  pressure,temperature, humidity, meridional_wind, zonal_wind"))
+        latest_date = Transmission.objects.values_list('received_date__date').order_by('received_date__date').last()
+        yesterday = datetime.now().date() - timedelta(days=1)
+
+        start_date = kwargs['start_date'] if kwargs['start_date'] is not None else latest_date[0].strftime("%Y-%m-%d")
+        end_date = kwargs['end_date'] if kwargs['end_date'] is not None else yesterday.strftime("%Y-%m-%d")
+        periods = kwargs['periods'] if kwargs['periods'] is not None else ["00", "06", "12", "18"]
+        centers = kwargs['centers'] if kwargs['centers'] is not None else ["DWD", "ECMWF", "JMA", "NCEP"]
+        variables = kwargs['variables'] if kwargs['variables'] is not None else ['pressure', 'temperature', 'humidity', 'meridional_wind' , 'zonal_wind']
 
         variables_ls = ['pressure', 'temperature', 'humidity', 'meridional_wind' , 'zonal_wind']
         period_ls = ["00", "06", "12", "18"]
         center_ls = ["DWD", "ECMWF", "JMA", "NCEP"]
 
         # Regular expression to match YYYY-MM-DD format
         date_pattern = re.compile(r'^\d{4}-\d{2}-\d{2}$')
 
         # Parsing the arguments manually
-        if start_date:
+        if start_date is not None:
             if not date_pattern.match(start_date):
                 self.stderr.write(self.style.ERROR(f"Invalid format for 'start_date'. Use YYYY-MM-DD format."))
                 return  # Exit the command
+        else:
+            # usually when there is no data in the database 
+            start_date = "2019-01-01" # earliest date ever on wdqms
 
-        if end_date:  
+        if end_date is not None:  
             if not date_pattern.match(end_date):
                 self.stderr.write(self.style.ERROR(f"Invalid format for 'end_date'. Use YYYY-MM-DD format."))
                 return  # Exit the command
             
         if datetime.strptime(start_date, "%Y-%m-%d") > datetime.strptime(end_date, "%Y-%m-%d"):
-            self.stderr.write(self.style.ERROR(f"'Start date' cannot come earlier than 'End date'"))
+            self.stderr.write(self.style.ERROR(f"'End date' cannot come earlier than 'Start date'"))
             return  # Exit the command
 
 
-        if variable:
-            if variable not in variables_ls:
-                self.stderr.write(self.style.ERROR(f"Allowed variables include pressure,temperature, humidity, meridional_wind, zonal_wind"))
-                return  # Exit the command
+        if variables is not None:
+            for variable in variables:
+                if variable not in variables_ls:
+                    self.stderr.write(self.style.ERROR(f"Allowed variables include pressure,temperature, humidity, meridional_wind, zonal_wind"))
+                    return  # Exit the command
 
             # Split the value by comma and append to list_arg
-        if periods:
+        if periods is not None:
             for period in periods:
                 if period not in period_ls:
                     self.stderr.write(self.style.ERROR(f"'{period}' is not a valid option. Choices are 00 06 12 18"))
                     return  # Exit the command
             
-        if centers:
+        if centers is not None:
             for center in centers:
                 if center.upper() not in center_ls:
                     self.stderr.write(self.style.ERROR(f"'{center}' is not a valid option. Choices are DWD ECMWF JMA NCEP"))
                     return  # Exit the command
                 
             
 
-
-        if start_date and end_date and variable and centers and periods:
+        if start_date is not None and end_date is not None and variables is not None and centers is not None and periods is not None:
             for country in Country.objects.all():
                 if Country.objects.count() > 0:
                     # loop through all countries in boundary manager for data fetching and ingestion
                     self.stdout.write(f"FETCH: Requesting data for {country.country.name}")
 
-                    ingest_transmission_rates(start_date, end_date, variable, periods, centers, country.country.alpha3)
+                    ingest_transmission_rates(start_date, end_date, variables, periods, centers, country.country.alpha3)
                 else:
                     self.stderr.write(self.style.ERROR(f"Please select atleast one country in admin boundary settings first"))
```

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms/migrations/0001_initial.py` & `climweb_wdqms-0.0.3/climweb_wdqms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms/models.py` & `climweb_wdqms-0.0.3/climweb_wdqms/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from django.contrib.gis.db import models
 from django.utils.translation import gettext_lazy as _
+from django.urls import reverse
+from django.utils.functional import cached_property
 
 class Station(models.Model):
 
     wigos_id = models.CharField(_("Wigos ID"), max_length=50, primary_key=True)
     name = models.CharField(_("Station name"), max_length=255)
     geom = models.PointField(_("Geometry"),)
     in_oscar = models.BooleanField(_("In Oscar?"),)
@@ -11,29 +13,31 @@
     class Meta:
         verbose_name = _("Station")
         verbose_name_plural = _("Stations")
 
     def __str__(self):
         return f'{self.name}-{self.wigos_id}'
     
-    
+    @cached_property
+    def stations_api(self):
+        return reverse("stations_api")
+
         
 # Create your models here.
 class Transmission(models.Model):
 
     station = models.ForeignKey("Station", on_delete=models.CASCADE)
     variable = models.CharField(_("Transmission Variable"), max_length=50 )
     received = models.IntegerField(_("Transmissions received"), null=True)
     expected = models.IntegerField(_("Transmissions expected"), null=True)
     received_rate = models.DecimalField(_("Transmission Rate"), max_digits=5, decimal_places=2)
     received_date = models.DateTimeField(_("Date Time Received"), auto_now=False, auto_now_add=False)
 
-
-        
     class Meta:
         verbose_name = _("Transmission")
         verbose_name_plural = _("Transmissions")
 
     def __str__(self):
         return f'{self.station} - {self.variable} - {self.received_date}'
+
```

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms/urls.py` & `climweb_wdqms-0.0.3/climweb_wdqms/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from django.urls import path
 
 from .views import (
     StationListView,
     SynopTransmissionView,
     MonthlyTransmissionView,
-    YearlyTransmissionView
+    YearlyTransmissionView,
+    AverageMonthlyReceivedRateGeom
 )
 
 urlpatterns = [
     path('api/synop-transmission-rate/', SynopTransmissionView.as_view(), name='synop-transmission-rate'),
     path('api/monthly-transmission-rate/', MonthlyTransmissionView.as_view(), name='monthly-transmission-rate'),
     path('api/yearly-transmission-rate/', YearlyTransmissionView.as_view(), name='yearly-transmission-rate'),
+    path('api/monthly-geom-transmission-rate/', AverageMonthlyReceivedRateGeom.as_view(), name='monthly-geom-transmission-rate'),
     path('api/stations/', StationListView.as_view(), name='station-list'),
 ]
```

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms.egg-info/PKG-INFO` & `climweb_wdqms-0.0.3/climweb_wdqms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.2
+Version: 0.0.3
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.2/climweb_wdqms.egg-info/SOURCES.txt` & `climweb_wdqms-0.0.3/climweb_wdqms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.2/setup.cfg` & `climweb_wdqms-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climweb-wdqms
-version = 0.0.2
+version = 0.0.3
 description = National level WDQMS Summary tool
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/climweb-wdqms
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

