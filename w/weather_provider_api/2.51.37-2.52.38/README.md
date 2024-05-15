# Comparing `tmp/weather_provider_api-2.51.37.tar.gz` & `tmp/weather_provider_api-2.52.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_provider_api-2.51.37.tar", max compression
+gzip compressed data, was "weather_provider_api-2.52.38.tar", max compression
```

## Comparing `weather_provider_api-2.51.37.tar` & `weather_provider_api-2.52.38.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    17098 2024-04-22 11:14:55.507030 weather_provider_api-2.51.37/LICENSE
-drwxr-xr-x   0        0        0        0 2024-04-22 11:14:55.507030 weather_provider_api-2.51.37/LICENSES/
--rw-r--r--   0        0        0    10438 2024-04-22 11:14:55.507030 weather_provider_api-2.51.37/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    12890 2024-04-22 11:14:55.507030 weather_provider_api-2.51.37/LICENSES/CC-BY-2.5.txt
--rw-r--r--   0        0        0    15199 2024-04-22 11:14:55.507030 weather_provider_api-2.51.37/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    11816 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/README.md
--rw-r--r--   0        0        0     3088 2024-04-22 11:15:17.823244 weather_provider_api-2.51.37/pyproject.toml
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/__init__.py
--rw-r--r--   0        0        0     2651 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/__main__.py
--rw-r--r--   0        0        0     1821 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/app_version.py
--rw-r--r--   0        0        0     1054 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/config/__init__.py
--rw-r--r--   0        0        0      913 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/config/config.toml
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/core/__init__.py
--rw-r--r--   0        0        0     2995 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/core/application.py
--rw-r--r--   0        0        0      478 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/core/base_model.py
--rw-r--r--   0        0        0      135 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/core/exceptions/__init__.py
--rw-r--r--   0        0        0      263 2024-04-22 11:14:55.511030 weather_provider_api-2.51.37/weather_provider_api/core/exceptions/additional_responses.py
--rw-r--r--   0        0        0      267 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/exceptions/api_models.py
--rw-r--r--   0        0        0      704 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/exceptions/exceptions.py
--rw-r--r--   0        0        0     2278 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/gunicorn_application.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/__init__.py
--rw-r--r--   0        0        0     2157 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/cors.py
--rw-r--r--   0        0        0     2006 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/exception_handling.py
--rw-r--r--   0        0        0     1310 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/headers.py
--rw-r--r--   0        0        0     5297 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/logging_handler.py
--rw-r--r--   0        0        0     1318 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/mounting.py
--rw-r--r--   0        0        0     1642 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/prometheus.py
--rw-r--r--   0        0        0      348 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/rate_limiter.py
--rw-r--r--   0        0        0     4375 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/initializers/validation.py
--rw-r--r--   0        0        0       46 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/utils/__init__.py
--rw-r--r--   0        0        0      696 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/core/utils/example_responses.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/__init__.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/__init__.py
--rw-r--r--   0        0        0     6446 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_models.py
--rw-r--r--   0        0        0     5806 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_view_v1.py
--rw-r--r--   0        0        0     9649 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_view_v2.py
--rw-r--r--   0        0        0       91 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/base_models/__init__.py
--rw-r--r--   0        0        0     5975 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/base_models/model.py
--rw-r--r--   0        0        0     1135 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/base_models/source.py
--rw-r--r--   0        0        0     6686 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/controller.py
--rw-r--r--   0        0        0      726 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/exceptions.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/repository/__init__.py
--rw-r--r--   0        0        0    14191 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/repository/repository.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/__init__.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/__init__.py
--rw-r--r--   0        0        0      681 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/cds.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/__init__.py
--rw-r--r--   0        0        0    13309 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/downloader.py
--rw-r--r--   0        0        0     6408 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
--rw-r--r--   0        0        0     6840 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
--rw-r--r--   0        0        0    15187 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
--rw-r--r--   0        0        0      591 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/factors.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/models/__init__.py
--rw-r--r--   0        0        0     8711 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/models/era5land.py
--rw-r--r--   0        0        0     7833 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/__init__.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
--rw-r--r--   0        0        0     6930 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
--rw-r--r--   0        0        0    23812 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
--rw-r--r--   0        0        0     9169 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
--rw-r--r--   0        0        0     1495 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/knmi.py
--rw-r--r--   0        0        0      421 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
--rw-r--r--   0        0        0     4963 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
--rw-r--r--   0        0        0     5320 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
--rw-r--r--   0        0        0    15117 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
--rw-r--r--   0        0        0     4781 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
--rw-r--r--   0        0        0    11062 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
--rw-r--r--   0        0        0    13403 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
--rw-r--r--   0        0        0    19917 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/stations.py
--rw-r--r--   0        0        0     7014 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/utils.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
--rw-r--r--   0        0        0     5148 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/__init__.py
--rw-r--r--   0        0        0     3048 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/date_helpers.py
--rw-r--r--   0        0        0     1397 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/file_helpers.py
--rw-r--r--   0        0        0     5742 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/geo_position.py
--rw-r--r--   0        0        0     1791 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/grid_helpers.py
--rw-r--r--   0        0        0      447 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/pandas_helpers.py
--rw-r--r--   0        0        0     5053 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/serializers.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/__init__.py
--rw-r--r--   0        0        0      393 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/erase_arome_repository.py
--rw-r--r--   0        0        0      413 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/erase_era5land_repository.py
--rw-r--r--   0        0        0      438 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/erase_era5sl_repository.py
--rw-r--r--   0        0        0      497 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/erase_waarnemingen_register.py
--rw-r--r--   0        0        0      383 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/update_arome_repository.py
--rw-r--r--   0        0        0      401 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/update_era5land_repository.py
--rw-r--r--   0        0        0      371 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/update_era5sl_repository.py
--rw-r--r--   0        0        0      462 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/scripts/update_waarnemingen_register.py
--rw-r--r--   0        0        0      140 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/versions/__init__.py
--rw-r--r--   0        0        0      796 2024-04-22 11:14:55.515030 weather_provider_api-2.51.37/weather_provider_api/versions/v1.py
--rw-r--r--   0        0        0      772 2024-04-22 11:14:55.519030 weather_provider_api-2.51.37/weather_provider_api/versions/v2.py
--rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 weather_provider_api-2.51.37/PKG-INFO
+-rw-r--r--   0        0        0    17098 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/LICENSE
+drwxr-xr-x   0        0        0        0 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/LICENSES/
+-rw-r--r--   0        0        0    10438 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    12890 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/LICENSES/CC-BY-2.5.txt
+-rw-r--r--   0        0        0    15199 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    11816 2024-05-15 08:57:39.371887 weather_provider_api-2.52.38/README.md
+-rw-r--r--   0        0        0     3088 2024-05-15 08:58:02.900003 weather_provider_api-2.52.38/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/__init__.py
+-rw-r--r--   0        0        0     2650 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/__main__.py
+-rw-r--r--   0        0        0     1820 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/app_version.py
+-rw-r--r--   0        0        0     1052 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/config/__init__.py
+-rw-r--r--   0        0        0      912 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/config/config.toml
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/__init__.py
+-rw-r--r--   0        0        0     3013 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/application.py
+-rw-r--r--   0        0        0      479 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/base_model.py
+-rw-r--r--   0        0        0      135 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/exceptions/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/exceptions/additional_responses.py
+-rw-r--r--   0        0        0      267 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/exceptions/api_models.py
+-rw-r--r--   0        0        0      704 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2278 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/gunicorn_application.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/__init__.py
+-rw-r--r--   0        0        0     2155 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/cors.py
+-rw-r--r--   0        0        0     2005 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/exception_handling.py
+-rw-r--r--   0        0        0     1310 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/headers.py
+-rw-r--r--   0        0        0     5296 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/logging_handler.py
+-rw-r--r--   0        0        0     1317 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/mounting.py
+-rw-r--r--   0        0        0     1640 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/prometheus.py
+-rw-r--r--   0        0        0      347 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/rate_limiter.py
+-rw-r--r--   0        0        0     4377 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/initializers/validation.py
+-rw-r--r--   0        0        0       46 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/utils/__init__.py
+-rw-r--r--   0        0        0      696 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/core/utils/example_responses.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/__init__.py
+-rw-r--r--   0        0        0     6446 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_models.py
+-rw-r--r--   0        0        0     5805 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_view_v1.py
+-rw-r--r--   0        0        0     9654 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_view_v2.py
+-rw-r--r--   0        0        0       91 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/base_models/__init__.py
+-rw-r--r--   0        0        0     5952 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/base_models/model.py
+-rw-r--r--   0        0        0     1135 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/base_models/source.py
+-rw-r--r--   0        0        0     6684 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/controller.py
+-rw-r--r--   0        0        0      726 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/exceptions.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/repository/__init__.py
+-rw-r--r--   0        0        0    14031 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/repository/repository.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/cds.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/__init__.py
+-rw-r--r--   0        0        0    13309 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/downloader.py
+-rw-r--r--   0        0        0     6397 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
+-rw-r--r--   0        0        0     6829 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
+-rw-r--r--   0        0        0    15179 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
+-rw-r--r--   0        0        0      602 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/factors.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/models/__init__.py
+-rw-r--r--   0        0        0     8689 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/models/era5land.py
+-rw-r--r--   0        0        0     7811 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
+-rw-r--r--   0        0        0     6928 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
+-rw-r--r--   0        0        0    23752 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
+-rw-r--r--   0        0        0     9168 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
+-rw-r--r--   0        0        0     1495 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/knmi.py
+-rw-r--r--   0        0        0      432 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
+-rw-r--r--   0        0        0     4948 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
+-rw-r--r--   0        0        0     5305 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
+-rw-r--r--   0        0        0    15073 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
+-rw-r--r--   0        0        0     4802 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
+-rw-r--r--   0        0        0    11031 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
+-rw-r--r--   0        0        0    13413 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
+-rw-r--r--   0        0        0    19911 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/stations.py
+-rw-r--r--   0        0        0     6982 2024-05-15 08:57:39.375887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/utils.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
+-rw-r--r--   0        0        0     5114 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/__init__.py
+-rw-r--r--   0        0        0     3042 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/date_helpers.py
+-rw-r--r--   0        0        0     1397 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/file_helpers.py
+-rw-r--r--   0        0        0     5742 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/geo_position.py
+-rw-r--r--   0        0        0     1791 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/grid_helpers.py
+-rw-r--r--   0        0        0      447 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/pandas_helpers.py
+-rw-r--r--   0        0        0     5053 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/serializers.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/erase_arome_repository.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/erase_era5land_repository.py
+-rw-r--r--   0        0        0      438 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/erase_era5sl_repository.py
+-rw-r--r--   0        0        0      497 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/erase_waarnemingen_register.py
+-rw-r--r--   0        0        0      394 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/update_arome_repository.py
+-rw-r--r--   0        0        0      412 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/update_era5land_repository.py
+-rw-r--r--   0        0        0      382 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/update_era5sl_repository.py
+-rw-r--r--   0        0        0      462 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/scripts/update_waarnemingen_register.py
+-rw-r--r--   0        0        0      140 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/versions/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/versions/v1.py
+-rw-r--r--   0        0        0      772 2024-05-15 08:57:39.379887 weather_provider_api-2.52.38/weather_provider_api/versions/v2.py
+-rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 weather_provider_api-2.52.38/PKG-INFO
```

### Comparing `weather_provider_api-2.51.37/LICENSE` & `weather_provider_api-2.52.38/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/LICENSES/Apache-2.0.txt` & `weather_provider_api-2.52.38/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/LICENSES/CC-BY-2.5.txt` & `weather_provider_api-2.52.38/LICENSES/CC-BY-2.5.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/LICENSES/MPL-2.0.txt` & `weather_provider_api-2.52.38/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/README.md` & `weather_provider_api-2.52.38/README.md`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/pyproject.toml` & `weather_provider_api-2.52.38/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather_provider_api"
-version = "2.51.037"
+version = "2.52.038"
 description = "Weather Provider Libraries and API"
 authors = ["Verbindingsteam", "Raoul Linnenbank <58594297+rflinnenbank@users.noreply.github.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository="https://github.com/alliander-opensource/wpla/"
 include = [
     {path = "var_maps/*.json", format = "wheel"}
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/__main__.py` & `weather_provider_api-2.52.38/weather_provider_api/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Main executable module """
+"""Main executable module."""
 
 import uvicorn
 from loguru import logger
 
 from weather_provider_api.core.initializers.logging_handler import initialize_logging
 
 # Logging is initialized before the importing of APP_CONFIG, to ensure custom logging for APP_CONFIG initialisation.
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/app_version.py` & `weather_provider_api-2.52.38/weather_provider_api/app_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Version detection module """
+"""Version detection module."""
 
 from importlib import metadata
 
 import tomli
 from loguru import logger
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/config/__init__.py` & `weather_provider_api-2.52.38/weather_provider_api/config/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Configuration folder """
+"""Configuration folder"""
 
 import os
 import tempfile
 from pathlib import Path
 
 from tomli import load
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/config/config.toml` & `weather_provider_api-2.52.38/weather_provider_api/config/config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [logging]
 log_level = "INFO"
 use_stdout_logger = true
 use_file_loggers = false
 file_logger_folder = "/tmp/wpla_logs"
 
 [components]
-prometheus = false
+prometheus = true
 cors = false
 cors_allowed_origins = ['*']
 cors_allowed_origins_regex = []
 
 [api_v1]
 implementation = "2.2.0"
 expiration_date = "2024-08-01"
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/application.py` & `weather_provider_api-2.52.38/weather_provider_api/core/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Main Application """
+"""Main Application."""
 
 from fastapi import FastAPI
 from starlette.responses import RedirectResponse
 
 from weather_provider_api.app_version import APP_VERSION
 from weather_provider_api.config import APP_CONFIG
 from weather_provider_api.core.initializers.cors import initialize_cors_middleware
-from weather_provider_api.core.initializers.exception_handling import initialize_exception_handler
+from weather_provider_api.core.initializers.exception_handling import (
+    initialize_exception_handler,
+)
 from weather_provider_api.core.initializers.headers import initialize_header_metadata
 from weather_provider_api.core.initializers.logging_handler import initialize_logging
 from weather_provider_api.core.initializers.mounting import mount_api_version
-from weather_provider_api.core.initializers.prometheus import initialize_prometheus_interface
+from weather_provider_api.core.initializers.prometheus import (
+    initialize_prometheus_interface,
+)
 from weather_provider_api.core.initializers.validation import initialize_api_validation
 from weather_provider_api.versions.v1 import app as v1
 from weather_provider_api.versions.v2 import app as v2
 
 
 def _build_api_application() -> FastAPI:
     """The main method for building a standardized FastAPI application for use with for instance Uvicorn.
@@ -61,15 +65,15 @@
     # Create and connect to end-points
     mount_api_version(application, v1)
     mount_api_version(application, v2)
 
     # Adding a redirect from the root of the application to our default view
     @application.get("/")
     def redirect_to_docs():
-        """This function redirects the visitors to the default view from the application's base URL"""
+        """This function redirects the visitors to the default view from the application's base URL."""
         return RedirectResponse(url="/api/v2/docs")
 
     application.openapi()
 
     return application
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/exceptions/exceptions.py` & `weather_provider_api-2.52.38/weather_provider_api/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/gunicorn_application.py` & `weather_provider_api-2.52.38/weather_provider_api/core/gunicorn_application.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/cors.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/cors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" CORS support """
+"""CORS support"""
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from loguru import logger
 
 from weather_provider_api.config import APP_CONFIG
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/exception_handling.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/exception_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Exception Handling
+"""Exception Handling
 
 This module holds the API's exception handler.
 """
 
 from fastapi import FastAPI
 from loguru import logger
-
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
 from weather_provider_api.config import APP_CONFIG
 
 
@@ -31,21 +30,22 @@
 
 
 def initialize_exception_handler(application: FastAPI):
     """The method that attaches the customized exception handling method to a FastAPI application.
 
     Args:
         application:    The FastAPI application to attach the custom exception handler to.
+
     Returns:
         Nothing. The FastAPI application itself is updated.
 
     Notes:
         This method assumes that the FastAPI application given has a [title] set.
 
-    TODO:
+    Todo:
         Evaluate the dependency on [title] and [root_path] parameters being set for FastAPI applications in ALL
          initializers. By either extending the base class to enforce these or improving the code to not be dependent on
          these parameters, we can eradiate code smell and chances at Exceptions caused by not having these parameters.
     """
     application.add_exception_handler(StarletteHTTPException, handler=handle_http_exception)
     logger.info(f"Attached the Exception Handler to the application ({application.title})...")
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/headers.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/headers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
 
 from fastapi import FastAPI
-
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.requests import Request
 
 from weather_provider_api.app_version import APP_VERSION
 from weather_provider_api.config import APP_CONFIG
 
 
 def initialize_header_metadata(application: FastAPI):
     """Method that attaches the customized Metadata Header method that adds extra metadata.
 
     Args:
         application: The FastAPI application to attach the custom method to.
+
     Returns:
         Nothing. The FastAPI application itself is updated.
     """
 
     async def add_metadata_headers(request: Request, call_next):
         response = await call_next(request)
         response.headers["X-App-Version"] = APP_VERSION
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/logging_handler.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/logging_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Logging Handler
+"""Logging Handler
 
 This module initializes the logging intercept handler, which intercepts other logging methods and translates them into
  the intended loguru logging format.
 """
 
 import logging
 import sys
 from pathlib import Path
 from tempfile import gettempdir
 
 from loguru import logger
 
-from weather_provider_api.config import APP_DEBUGGING, APP_CONFIG, APP_LOG_LEVEL
+from weather_provider_api.config import APP_CONFIG, APP_DEBUGGING, APP_LOG_LEVEL
 
 
 class LoggingInterceptHandler(logging.Handler):
     """A class with the purpose of intercepting all log messages, and forwarding it to our own custom logging system.
 
     Notes:
         For our custom logging, we use Loguru.
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/mounting.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/mounting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" (sub)-API Mounting
+"""(sub)-API Mounting
 
 This module handles the mounting of sub-API's onto a main API.
 """
 
 from fastapi import FastAPI
 from loguru import logger
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/prometheus.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/prometheus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" Prometheus Middleware handler """
+"""Prometheus Middleware handler"""
 
 from fastapi import FastAPI
 from loguru import logger
-
 from starlette_prometheus import PrometheusMiddleware, metrics
 
 
 def initialize_prometheus_interface(application: FastAPI, metrics_endpoint: str = "/metrics"):
     """The method that attaches the Prometheus Middleware to a FastAPI application.
 
     Args:
         application:        The FastAPI application to attach the Prometheus Middleware to.
         metrics_endpoint:   The endpoint at which the Prometheus data should become available.
+
     Returns:
         Nothing. The FastAPI application itself is updated.
 
     Notes:
         Prometheus is a metrics system that interprets requests and results and processes those into metrics. From a
          Prometheus server this data can be gathered and preprocessed, allowing for more extensive data on request
          and the handling thereof, like information on memory usage or the time taken to process certain types of
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/initializers/validation.py` & `weather_provider_api-2.52.38/weather_provider_api/core/initializers/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" API Validation checks """
+"""API Validation checks"""
 
-from datetime import datetime
 import re
+from datetime import datetime
 
 from fastapi import FastAPI
 from loguru import logger
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.requests import Request
 
 from weather_provider_api.config import APP_CONFIG
@@ -22,25 +22,27 @@
 
 
 def initialize_api_validation(application: FastAPI):
     """Method for attach the API validity checker to a FastAPI application.
 
     Args:
         application:    The FastAPI application to attach the checker to.
+
     Returns:
         Nothing. The application itself is updated.
 
     """
 
     async def check_api_for_validity(request: Request, call_next):
         """The method that validated the API validity.
 
         Args:
             request:    The request to evaluate
             call_next:  The call_next object for the request (what to do next if this step doesn't raise any exceptions)
+
         Returns:
             The next step to execute for this request. This is either the original call_next, or an
              HTTP Exception trigger for an APIExpiredException.
 
         """
         api_prefix = r"/api/v"
         api_suffix = "/weather"
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/core/utils/example_responses.py` & `weather_provider_api-2.52.38/weather_provider_api/core/utils/example_responses.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_models.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_models.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_view_v1.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_view_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-TODO:
+"""TODO:
 - Decouple weather factors from the get_weather function
 - Add the async process for e.g. CDS and Harmonie
 - Improve datetime slicing
 - Fix datetime validation in Swagger UI on IE and Safari
 - Improve output / error messages when no data is available
 """
 
@@ -22,15 +21,17 @@
     WeatherContentRequestQuery,
     WeatherFormattingRequestQuery,
     WeatherModel,
     WeatherSource,
     result_mime_types,
 )
 from weather_provider_api.routers.weather.controller import WeatherController
-from weather_provider_api.routers.weather.sources.weather_alert.weather_alert import WeatherAlert
+from weather_provider_api.routers.weather.sources.weather_alert.weather_alert import (
+    WeatherAlert,
+)
 from weather_provider_api.routers.weather.utils import serializers
 from weather_provider_api.routers.weather.utils.date_helpers import parse_datetime
 from weather_provider_api.routers.weather.utils.file_helpers import remove_file
 
 app = APIRouter()
 
 controller = WeatherController()
@@ -69,33 +70,32 @@
     source_id: str,
     model_id: str,
     cleanup_tasks: BackgroundTasks,
     ret_args: WeatherContentRequestQuery = Depends(),
     fmt_args: WeatherFormattingRequestQuery = Depends(),
     accept: str = Depends(header_accept_type),
 ):  # pragma: no cover
-    """
-        Function to gather data for a specific model using specific settings (location, period, factors, e.g.).
+    """Function to gather data for a specific model using specific settings (location, period, factors, e.g.).
         The function then formats this data into the requested output format (file-format and selected output unit) and
         returns it.
+
     Args:
         source_id:  The identifier for the chosen source
         model_id:   The identifier for the chosen model
         cleanup_tasks: Holder for background tasks, in get_sync_weather solely used for file cleanup, hence the name
         ret_args:   Contains a WeatherContentRequestQuery item with all the settings to be used for data collection
         fmt_args:   Contains a WeatherFormattingRequestQuery item with all the setting to be used for formatting the
                     output
         accept:
 
     Returns:
         Returns a file in the requested output format, containing any weather data that matched the specifications from
         the WeatherContentRequestQuery.
 
     """
-
     # TODO: Append a proper definition of the accept arg
     source_id = source_id.lower()
     model_id = model_id.lower()
     coords = controller.lat_lon_to_coords(ret_args.lat, ret_args.lon)
 
     begin = parse_datetime(ret_args.begin, raise_errors=True, loc=["query", "begin"])
     end = parse_datetime(
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/api_view_v2.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/api_view_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     WeatherContentRequestQuery,
     WeatherFormattingRequestQuery,
     WeatherModel,
     WeatherSource,
     result_mime_types,
 )
 from weather_provider_api.routers.weather.controller import WeatherController
-from weather_provider_api.routers.weather.sources.weather_alert.weather_alert import WeatherAlert
+from weather_provider_api.routers.weather.sources.weather_alert.weather_alert import (
+    WeatherAlert,
+)
 from weather_provider_api.routers.weather.utils import serializers
 from weather_provider_api.routers.weather.utils.date_helpers import parse_datetime
 from weather_provider_api.routers.weather.utils.file_helpers import remove_file
 
 v2_router = APIRouter()
 
 controller = WeatherController()
@@ -90,16 +92,15 @@
     source_id: str,
     model_id: str,
     cleanup_tasks: BackgroundTasks,
     ret_args: WeatherContentRequestQuery = Depends(),
     fmt_args: WeatherFormattingRequestQuery = Depends(),
     accept: str = Depends(header_accept_type),
 ):  # pragma: no cover
-    """
-    <B>Request weather data for a specific Model using the given settings (location, period, weather factors, e.g.). <BR>
+    """<B>Request weather data for a specific Model using the given settings (location, period, weather factors, e.g.). <BR>
     This data is then formatted as the requested output format (output unit system and file format) before returning the requested data.</B>
 
     <I>(Please note that as some models are predictive or otherwise restricted in the periods available for requests,
     that sometimes the 'begin' and 'end' values will be altered to match these restrictions.)</I>
     """
     """
         An API function that retrieves specific weather data for a specific Weather Model and returns it as the
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/base_models/model.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/base_models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from abc import ABCMeta, abstractmethod
 from typing import List, Optional
 
 import numpy as np
 import xarray as xr
 
-from weather_provider_api.core.initializers.exception_handling import NOT_IMPLEMENTED_ERROR
+from weather_provider_api.core.initializers.exception_handling import (
+    NOT_IMPLEMENTED_ERROR,
+)
 from weather_provider_api.routers.weather.api_models import OutputUnit
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class WeatherModelBase(metaclass=ABCMeta):
-    """
-    Base class for all Weather Models. All new models should use this base class!
+    """Base class for all Weather Models. All new models should use this base class!
     """
 
     def __init__(self):
         self.to_si = None
         self.to_human = None
         self.human_to_model_specific = None
 
@@ -36,16 +37,15 @@
         raise NotImplementedError(NOT_IMPLEMENTED_ERROR)
 
     @abstractmethod
     def is_async(self):  # pragma: no cover
         raise NotImplementedError(NOT_IMPLEMENTED_ERROR)
 
     def convert_names_and_units(self, weather_data: xr.Dataset, unit: OutputUnit):
-        """
-            Function to convert all names and units in a dataset according to the required translations set in the
+        """Function to convert all names and units in a dataset according to the required translations set in the
             to_xxxx values for the model itself
         Args:
             weather_data:   A Xarray Dataset containing
             unit:           The requested output unit format
 
         Returns:
             The same dataset, but with values altered to match the requested output unit format
@@ -149,16 +149,15 @@
             else:
                 return None
 
         return np.frompyfunc(dutch_wind_direction_to_degrees_single, 1, 1)(xs)
 
     @staticmethod
     def knmi_visibility_class_to_meter_estimate(xs):
-        """
-            Function to transform KNMI visibility class values to an estimate of meters visibility
+        """Function to transform KNMI visibility class values to an estimate of meters visibility
         Args:
             xs:     The visibility class value to be interpreted
 
         Returns:
             A numeric value containing an estimate of the meters of visibility matching the given visibility class value
 
         """
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/base_models/source.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/base_models/source.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/controller.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 
 import numpy as np
 import xarray as xr
 
 from weather_provider_api.routers.weather.api_models import OutputUnit
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
 from weather_provider_api.routers.weather.base_models.source import WeatherSourceBase
-from weather_provider_api.routers.weather.exceptions import UnknownModelException, UnknownSourceException
+from weather_provider_api.routers.weather.exceptions import (
+    UnknownModelException,
+    UnknownSourceException,
+)
 from weather_provider_api.routers.weather.sources.cds.cds import CDS
 from weather_provider_api.routers.weather.sources.knmi.knmi import KNMI
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class WeatherController(object):  # pragma: no cover
-    """
-    A Controller Object that can handle any request for the hooked up weather models and format it into any of the
+    """A Controller Object that can handle any request for the hooked up weather models and format it into any of the
     hooked up output formats.
     """
 
     def __init__(self):
         # Load Sources (and with it their models) and hook them up to the controller
         source_instances = [KNMI(), CDS()]
         self.sources = {source.id: source for source in source_instances}
@@ -38,17 +40,17 @@
         model_id: str,
         fetch_async: bool,
         coords: List[List[Tuple[float, float]]],
         begin: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         factors: List[str] = None,
     ):
-        """
-            Function to use the requested weather model from the requested source to get specific weather factors for a
+        """Function to use the requested weather model from the requested source to get specific weather factors for a
             specific time and specific location(s)
+
         Args:
             source_id:  The weather source that need to be queried (e.g.: knmi, cds)
             model_id:   The model identifier of the model that needs to be queried (has to be a model that exists within
                         the specific source requested through source_id
             fetch_async:    A boolean indicated if the request was made to asynchronously fetch the data or not
             coords:     A nested 3-layer list representing a list of polygons
                         in the case of points, they are treated as a one-point polygon
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/exceptions.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/repository/repository.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/repository/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,54 +13,54 @@
 from typing import List
 
 import xarray as xr
 from fastapi import HTTPException
 from loguru import logger
 
 from weather_provider_api.config import APP_STORAGE_FOLDER
-from weather_provider_api.core.initializers.exception_handling import NOT_IMPLEMENTED_ERROR
+from weather_provider_api.core.initializers.exception_handling import (
+    NOT_IMPLEMENTED_ERROR,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class RepositoryUpdateResult(Enum):
     failure = 0
     completed = 1
     timed_out = 2
 
 
 class WeatherRepositoryBase(metaclass=ABCMeta):
-    """
-    This is the base class for all weather data storage repositories. Any new repositories should implement this
+    """This is the base class for all weather data storage repositories. Any new repositories should implement this
     as their base class.
     All valid stored repository files are named as follows:
     {file_prefix}_{file_identifier}.nc
     or
     {file_prefix}_{file_identifier}_{permanent_suffix}.nc
     Any files found not matching this pattern shall be deleted as being temporary in nature.
     """
 
     def __init__(self):
-        """
-        Specification of required fields for a weather data storage repository:
-            - repository_folder:    Contains the folder where the repository will be saved. Is set inside a main
-                                    repository folder, and based on a sub-folder passed by the repository itself
-                                    through the _get_repo_subfolder() function.
-            - file_prefix:          Contains a string with the file_prefix to use for all files within the
-                                    repository. Is set from the repository itself.
-            - runtime_limit:        Contains the maximum time the update function of the repository is allowed to be
-                                    running, in seconds.
-            - first_day_of_repo:    Contains a datetime indicating the oldest moment allowed to be stored in the
-                                    repository.
-            - last_day_of_repo:     Contains a datetime indicating the newest moment allowed to be stored in the
-                                    repository.
-            - permanent_suffixes:   Contains a list of suffixes that can be added to the repository files to
-                                    indicate that the file should not be deleted. Any file not matching the prefix
-                                    or having a suffix not matching this list will be deleted upon cleanup.
-            - file_identifier_length:   This is the length in characters that the unique identifier part of the
-                                        filename takes up. Usually this is based on a datetime.
+        """Specification of required fields for a weather data storage repository:
+        - repository_folder:    Contains the folder where the repository will be saved. Is set inside a main
+                                repository folder, and based on a sub-folder passed by the repository itself
+                                through the _get_repo_subfolder() function.
+        - file_prefix:          Contains a string with the file_prefix to use for all files within the
+                                repository. Is set from the repository itself.
+        - runtime_limit:        Contains the maximum time the update function of the repository is allowed to be
+                                running, in seconds.
+        - first_day_of_repo:    Contains a datetime indicating the oldest moment allowed to be stored in the
+                                repository.
+        - last_day_of_repo:     Contains a datetime indicating the newest moment allowed to be stored in the
+                                repository.
+        - permanent_suffixes:   Contains a list of suffixes that can be added to the repository files to
+                                indicate that the file should not be deleted. Any file not matching the prefix
+                                or having a suffix not matching this list will be deleted upon cleanup.
+        - file_identifier_length:   This is the length in characters that the unique identifier part of the
+                                    filename takes up. Usually this is based on a datetime.
         """
         self.repository_folder = Path(APP_STORAGE_FOLDER).joinpath(self._get_repo_sub_folder())
         self.repository_name = None
         self.file_prefix = None
         self.runtime_limit = 60 * 60 * 2  # seconds * minutes * hours (2 hours default)
         self.permanent_suffixes = None
         self.file_identifier_length = None
@@ -75,32 +75,30 @@
 
     @staticmethod
     @abstractmethod
     def _get_repo_sub_folder():
         raise NotImplementedError(NOT_IMPLEMENTED_ERROR)
 
     def _validate_repo_folder(self):
-        """
-        This function checks whether the repository folder already exists (starting from its parent folder)
+        """This function checks whether the repository folder already exists (starting from its parent folder)
         and creates it, if it (or its parent folder) don't exist yet.
         """
         if not Path(self.repository_folder).exists():  # If the folder doesn't exist yet, create it
             logger.debug(f"Attempting to create folder[{self.repository_folder}]")
             try:
                 # If the main folder for all repositories doesn't exist yet, create it
                 if not Path(self.repository_folder).parent.exists():
                     Path(self.repository_folder).parent.mkdir()
                 Path(self.repository_folder).mkdir()
             except OSError as e:
                 logger.error(f"An error occurred creating the directory: {e}")
                 raise e
 
     def cleanup(self):
-        """
-        This is the cleanup function for any Weather Repository.
+        """This is the cleanup function for any Weather Repository.
         Any files not matching the pattern required for the Repository shall be deleted.
         """
         self._validate_repo_folder()
         logger.debug(f"Verifying existing files for {self.repository_name} in [{self.repository_folder}]")
 
         # Delete any files that aren't of a permanent type
         self._delete_non_permanent_files()
@@ -112,16 +110,15 @@
         self._delete_excess_files()
 
     @abstractmethod
     def update(self):
         raise NotImplementedError(NOT_IMPLEMENTED_ERROR)
 
     def gather_period(self, begin: datetime, end: datetime, coordinates: List[GeoPosition]) -> xr.Dataset:
-        """
-            A function that gathers the repository files associated with a requested period, and then returns the full
+        """A function that gathers the repository files associated with a requested period, and then returns the full
             weather data that matches both that period as the requested locations from those files, as a Xarray Dataset
         Args:
             begin:          A datetime holding the starting moment for the requested period to gather data for
             end:            A datetime holding the ending moment for the requested period to gather data for
             coordinates:    A list of GeoPositions holding the coordinates that the data request is for
         Returns:
             A Xarray Dataset containing all the repository data that matches both the requested period, and
@@ -155,41 +152,38 @@
                 ds = ds_temp
             else:
                 ds = ds.combine_first(ds_temp)
         return ds
 
     @staticmethod
     def load_file(file: Path) -> xr.Dataset:
-        """
-            A function that loads and returns the full data for a specific repository file as a Xarray Dataset
+        """A function that loads and returns the full data for a specific repository file as a Xarray Dataset
         Args:
             file:   The filename (in the Path format by PathLib) specifying the file to load
         Returns:
             An Xarray Dataset containing all the weather data held within the specified file.
         """
         if file.exists():
             with xr.open_dataset(file) as ds:
                 ds.load()
             return ds
 
         # Raise a FileNotFoundError if the file doesn't exist
-        logger.error(f"File [{str(file)} does not exist]")
+        logger.error(f"File [{file!s} does not exist]")
         raise FileNotFoundError
 
     def purge_repository(self):
-        """
-        Function to fully delete the repository's folder and create a new clean one. Use with care!
+        """Function to fully delete the repository's folder and create a new clean one. Use with care!
         """
         logger.warning(f"Purging the entire repository folder for {self.repository_name}!")
         shutil.rmtree(self.repository_folder, ignore_errors=True)
         self._validate_repo_folder()  # Rebuild the folder after deletion
 
     def _delete_non_permanent_files(self):
-        """
-        A function that deletes any and all files in the repository's folder that are not considered permanent in
+        """A function that deletes any and all files in the repository's folder that are not considered permanent in
         nature. Only the files matching either repository files without a suffix or those with suffix listed in the
         permanent_suffixes field are allowed.
         Every other file should be deleted from the repository immediately.
         """
         # TODO: Enhance the detection of files that do not belong in the folder.
         #       A repository folder should only have repository files..
         len_filename_until_after_date = (
@@ -204,16 +198,15 @@
                 self._safely_delete_file(file_name)
 
     @abstractmethod
     def _delete_files_outside_of_scope(self):
         pass
 
     def _delete_excess_files(self):
-        """
-        A function that selects the proper file to keep when more than one permanent file exists for a given
+        """A function that selects the proper file to keep when more than one permanent file exists for a given
         identifier. The other files are deleted.
         """
         len_filename_until_date = len(str(self.repository_folder.joinpath(self.file_prefix))) + 1
         file_list = glob.glob(str(self.repository_folder.joinpath(self.file_prefix)) + "*.*")
         identifier_list = list(
             set(
                 [
@@ -262,19 +255,20 @@
         return True
 
     @abstractmethod
     def _get_file_list_for_period(self, start: datetime, end: datetime):
         raise NotImplementedError(NOT_IMPLEMENTED_ERROR)
 
     def _filter_dataset_by_coordinates(self, coordinates: List[GeoPosition], ds: xr.Dataset) -> xr.Dataset:
-        """
-            A function that filters a given Xarray Dataset down to the values matching a given list of locations.
+        """A function that filters a given Xarray Dataset down to the values matching a given list of locations.
+
         Args:
             coordinates:    A list of GeoPositions that the data is requested for.
             ds:             An Xarray Dataset containing the data to be filtered.
+
         Returns:
             An Xarray Dataset containing only the weather data that matched the given list of coordinates.
         """
         ds_selected = xr.Dataset()
         coordinate_list = self.get_grid_coordinates(coordinates)
 
         for coordinate in coordinate_list:
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/cds.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/cds.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/downloader.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 import glob
 from datetime import datetime
 from typing import List
 
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
-from weather_provider_api.routers.weather.repository.repository import WeatherRepositoryBase
-from weather_provider_api.routers.weather.sources.cds.client.utils_era5 import era5_update
+from weather_provider_api.routers.weather.repository.repository import (
+    WeatherRepositoryBase,
+)
+from weather_provider_api.routers.weather.sources.cds.client.utils_era5 import (
+    era5_update,
+)
 from weather_provider_api.routers.weather.sources.cds.factors import era5land_factors
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
-from weather_provider_api.routers.weather.utils.grid_helpers import round_coordinates_to_wgs84_grid
+from weather_provider_api.routers.weather.utils.grid_helpers import (
+    round_coordinates_to_wgs84_grid,
+)
 
 
 class ERA5LandRepository(WeatherRepositoryBase):
-    """
-    A class that holds all functionality (excepting the downloader) for the ERA5 Single Levels Repository
+    """A class that holds all functionality (excepting the downloader) for the ERA5 Single Levels Repository
     """
 
     def __init__(self):
         super().__init__()
         self.repository_name = "CSD: ERA5-Land"
         logger.debug(f"Initializing {self.repository_name} repository")
         self.file_prefix = "ERA5LAND"
@@ -49,24 +54,23 @@
     @property
     def last_day_of_repo(self):
         last_day_of_repo = datetime.utcnow() - relativedelta(days=2)
         last_day_of_repo = last_day_of_repo.replace(hour=0, minute=0, second=0, microsecond=0)
         return last_day_of_repo
 
     def update(self):
-        """
-            The implementation of the WeatherRepository required update() function.
+        """The implementation of the WeatherRepository required update() function.
             This function handles all the required actions to update the repository completely, but taking into
             account its set runtime_limit. If based on the time of completion of other downloaded files this session
             the next file wouldn't complete within the runtime_limit, the update process halts.
             (if no other downloads were made yet, a generous rough estimate is used)
+
         Returns:
             A RepositoryUpdateResult value indicating a completion, time-out or failure of the update process
         """
-
         # Always start with a nicely cleaned repository
         self.cleanup()
 
         return era5_update(
             self.file_prefix,
             self.repository_folder,
             (self.first_day_of_repo, self.last_day_of_repo),
@@ -76,17 +80,17 @@
             (self.grid_resolution, self.grid_resolution),
             era5land_factors,
             self.runtime_limit,
             True,
         )
 
     def _delete_files_outside_of_scope(self):
-        """
-            A function that deletes all files in the repository with a date not inside the repository's scope.
+        """A function that deletes all files in the repository with a date not inside the repository's scope.
             All files labeled as either before or after the given scope will be deleted.
+
         Returns:
             Nothing. Successful means the all files outside the scope were deleted.
         """
         len_filename_until_date = len(str(self.repository_folder.joinpath(self.file_prefix))) + 1
 
         for file_name in glob.glob(str(self.repository_folder.joinpath(self.file_prefix)) + "*.nc"):
             file_year = int(file_name[len_filename_until_date : len_filename_until_date + 4])
@@ -101,19 +105,19 @@
                 logger.debug(
                     f"Deleting file [{file_name}] because it does not lie in the "
                     f"repository scope ({self.first_day_of_repo, self.last_day_of_repo})"
                 )
                 self._safely_delete_file(file_name)
 
     def _get_file_list_for_period(self, start: datetime, end: datetime):
-        """
-            A function that retrieves a list of files in the repository associated with the requested period of time
+        """A function that retrieves a list of files in the repository associated with the requested period of time
         Args:
             start:  A datetime containing the start of the requested period of time.
             end:    A datetime containing the end of the requested period of time.
+
         Returns:
             A list of files (in string format) that indicate the files containing data for the requested period.
         """
         self.cleanup()
 
         len_filename_until_date = len(str(self.repository_folder.joinpath(self.file_prefix))) + 1
         full_list_of_files = glob.glob(str(self.repository_folder.joinpath(self.file_prefix)) + "*.nc")
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 import glob
 from datetime import datetime
 from typing import List
 
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
-from weather_provider_api.routers.weather.repository.repository import WeatherRepositoryBase
-from weather_provider_api.routers.weather.sources.cds.client.utils_era5 import era5_update
+from weather_provider_api.routers.weather.repository.repository import (
+    WeatherRepositoryBase,
+)
+from weather_provider_api.routers.weather.sources.cds.client.utils_era5 import (
+    era5_update,
+)
 from weather_provider_api.routers.weather.sources.cds.factors import era5sl_factors
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
-from weather_provider_api.routers.weather.utils.grid_helpers import round_coordinates_to_wgs84_grid
+from weather_provider_api.routers.weather.utils.grid_helpers import (
+    round_coordinates_to_wgs84_grid,
+)
 
 
 class ERA5SLRepository(WeatherRepositoryBase):
-    """
-    A class that holds all functionality (excepting the downloader) for the ERA5 Single Levels Repository
+    """A class that holds all functionality (excepting the downloader) for the ERA5 Single Levels Repository
     """
 
     def __init__(self):
         super().__init__()
         self.repository_name = "CSD ERA5 Single Levels"
         logger.debug(f"Initializing {self.repository_name} repository")
         self.file_prefix = "ERA5SL"
@@ -49,24 +54,23 @@
     @property
     def last_day_of_repo(self):
         last_day_of_repo = datetime.utcnow() - relativedelta(days=5)
         last_day_of_repo = last_day_of_repo.replace(hour=0, minute=0, second=0, microsecond=0)
         return last_day_of_repo
 
     def update(self):
-        """
-            The implementation of the WeatherRepository required update() function.
+        """The implementation of the WeatherRepository required update() function.
             This function handles all the required actions to update the repository completely, but taking into
             account its set runtime_limit. If based on the time of completion of other downloaded files this session
             the next file wouldn't complete within the runtime_limit, the update process halts.
             (if no other downloads were made yet, a generous rough estimate is used)
+
         Returns:
             A RepositoryUpdateResult value indicating a completion, time-out or failure of the update process
         """
-
         # Always start with a nicely cleaned repository
         self.cleanup()
 
         logger.info(f"ERA5 Single Levels Update - Storage in: {self.repository_folder} ")
         return era5_update(
             self.file_prefix,
             self.repository_folder,
@@ -77,17 +81,17 @@
             (self.grid_resolution, self.grid_resolution),
             era5sl_factors,
             self.runtime_limit,
             True,
         )
 
     def _delete_files_outside_of_scope(self):
-        """
-            A function that deletes all files in the repository with a date not inside the repository's scope.
+        """A function that deletes all files in the repository with a date not inside the repository's scope.
             All files labeled as either before or after the given scope will be deleted.
+
         Returns:
             Nothing. Successful means the all files outside the scope were deleted.
         """
         len_filename_until_date = len(str(self.repository_folder.joinpath(self.file_prefix))) + 1
 
         for file_name in glob.glob(str(self.repository_folder.joinpath(self.file_prefix)) + "*.nc"):
             file_year = int(file_name[len_filename_until_date : len_filename_until_date + 4])
@@ -102,19 +106,19 @@
                 logger.debug(
                     f"Deleting file [{file_name}] because it does not lie in the "
                     f"repository scope ({self.first_day_of_repo, self.last_day_of_repo})"
                 )
                 self._safely_delete_file(file_name)
 
     def _get_file_list_for_period(self, start: datetime, end: datetime):
-        """
-            A function that retrieves a list of files in the repository associated with the requested period of time
+        """A function that retrieves a list of files in the repository associated with the requested period of time
         Args:
             start:  A datetime containing the start of the requested period of time.
             end:    A datetime containing the end of the requested period of time.
+
         Returns:
             A list of files (in string format) that indicate the files containing data for the requested period.
         """
         self.cleanup()
 
         len_filename_until_date = len(str(self.repository_folder.joinpath(self.file_prefix))) + 1
         logger.info(
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import xarray as xr
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
-from weather_provider_api.routers.weather.repository.repository import RepositoryUpdateResult
+from weather_provider_api.routers.weather.repository.repository import (
+    RepositoryUpdateResult,
+)
 from weather_provider_api.routers.weather.sources.cds.client import downloader
 
 _FORMATTED_SUFFIX = ".FORMATTED.nc"
 _UNFORMATTED_SUFFIX = ".UNFORMATTED.nc"
 _INCOMPLETE_SUFFIX = ".INCOMPLETE.nc"
 _TEMP_SUFFIX = ".TEMP.nc"
 
@@ -258,26 +260,27 @@
     grid_resolution,
     weather_factors,
     years,
     months,
     days,
     target_location,
 ):
-    """
-        A function that download a NetCDF file to the target location, containing the requested factors for an
+    """A function that download a NetCDF file to the target location, containing the requested factors for an
         also requested range of years, months, days and locations.
+
     Args:
         dataset:            The name of the dataset to download from
         product_type:       The type of product to download
         grid_resolution:    The grid resolution to download the results in
         weather_factors:    A list of factors to be downloaded (in string format)
         years:              A list of years to be requested (numeric)
         months:             A list of months to be requested (numeric)
         days:               A list of days to be requested (numeric)
         target_location:    The file location to which the result should be saved after downloading.
+
     Returns:
         Returns nothing, but success means a result file will exist at the given target location.
     """
     c = downloader.CDSDownloadClient(persist_request_callback=_repository_callback(), verify=True)
     try:
         c.retrieve(
             dataset,
@@ -321,29 +324,28 @@
         )
     except Exception as e:
         logger.warning(f"Could not download the requested file: {e}")
         return False
 
 
 def load_file(file: Path) -> xr.Dataset:
-    """
-        A function that loads and returns the full data for a specific repository file as a Xarray Dataset
+    """A function that loads and returns the full data for a specific repository file as a Xarray Dataset
     Args:
         file:   The filename (in the Path format by PathLib) specifying the file to load
     Returns:
         An Xarray Dataset containing all the weather data held within the specified file.
 
     """
     if file.exists():
         with xr.open_dataset(file) as ds:
             ds.load()
         return ds
 
     # Raise a FileNotFoundError if the file doesn't exist
-    logger.error(f"File [{str(file)}] does not exist")
+    logger.error(f"File [{file!s}] does not exist")
     raise FileNotFoundError
 
 
 def _safely_delete_file(file: Path):
     """Basic function to safely remove files from the repository if possible, and supply errors if not"""
     try:
         logger.debug(f"Safely deleting file [{file}]")
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/factors.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/factors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
 # factor name mapping
 
 import json
 
-from weather_provider_api.routers.weather.utils.file_helpers import get_var_map_file_location
+from weather_provider_api.routers.weather.utils.file_helpers import (
+    get_var_map_file_location,
+)
 
 file_to_use_era5sl = get_var_map_file_location("era5sl_var_map.json")
 file_to_use_era5land = get_var_map_file_location("era5land_var_map.json")
 
 with open(file_to_use_era5sl, "r") as _f:
     era5sl_factors = json.load(_f)
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/models/era5land.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/models/era5land.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-    CDS - ERA5 Single Levels Weatherdata Model
+"""CDS - ERA5 Single Levels Weatherdata Model
 """
 import copy
 from datetime import datetime
 from typing import List, Optional
 
 import xarray
 import xarray as xr
 from loguru import logger
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
-from weather_provider_api.routers.weather.sources.cds.client.era5land_repository import ERA5LandRepository
+from weather_provider_api.routers.weather.sources.cds.client.era5land_repository import (
+    ERA5LandRepository,
+)
 from weather_provider_api.routers.weather.sources.cds.factors import era5sl_factors
-from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
+from weather_provider_api.routers.weather.utils.date_helpers import (
+    validate_begin_and_end,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class ERA5LandModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
+    """A Weather Model that incorporates the:
         ERA5 hourly data on single levels from 1979 to present
     dataset into the Weather Provider API
     """
 
     def __init__(self):
         super().__init__()
         self.id = "era5land"
@@ -78,26 +80,26 @@
     def get_weather(
         self,
         coords: List[GeoPosition],
         begin: datetime,
         end: datetime,
         weather_factors: List[str] = None,
     ) -> xr.Dataset:
-        """
-            The function that gathers and processes the requested ERA5 Single Levels weather data from the repository
+        """The function that gathers and processes the requested ERA5 Single Levels weather data from the repository
             and returns it as a Xarray Dataset.
+
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
         """
-
         # Test and account for invalid datetime timeframes or input
         begin, end = validate_begin_and_end(
             begin,
             end,
             self.repository.first_day_of_repo,
             self.repository.last_day_of_repo,
         )
@@ -106,20 +108,21 @@
         validated_factors = self._validate_weather_factors(weather_factors)
 
         ds = self._fill_dataset_with_data(coords, begin, end, validated_factors)
         return ds
 
     @staticmethod
     def _validate_weather_factors(weather_factors: List[str]) -> List[str]:
-        """
-            A function that validates a list of weather factors to that of the dataset in the repository.
+        """A function that validates a list of weather factors to that of the dataset in the repository.
             Existing factors will be kept, non-existing removed, and if the list is empty the full set for the dataset
             will be used.
+
         Args:
             weather_factors:    A list of weather factors to validate (in string format)
+
         Returns:
             A list of weather factors (in string format) only factors that match those of the ERA5SL dataset.
         """
         if weather_factors is None:
             weather_factors = [era5sl_factors[x] for x in list(era5sl_factors.keys())]
 
         # Lookup using the generic long name
@@ -151,22 +154,23 @@
     def _fill_dataset_with_data(
         self,
         era5sl_coordinates: List[GeoPosition],
         begin: datetime,
         end: datetime,
         validated_factors: List[str],
     ) -> xr.Dataset:
-        """
-            A function that fills a dataset with ERA5SL weather data from the repository, based on the requested
+        """A function that fills a dataset with ERA5SL weather data from the repository, based on the requested
             coordinates and period, and removes any not-requested weather factors from the output.
+
         Args:
             era5sl_coordinates:     A list of GeoPositions containing the locations to be gathered from the repository.
             begin:                  A datetime containing the starting moment for the period to gather.
             end:                    A datetime containing the end moment for the period to gather.
             validated_factors:      A list of valid ERA5SL factors wanted for the result.
+
         Returns:
             An Xarray Dataset containing the weather data requested.
         """
         # Gather a dataset with the proper period and coordinates
         ds = self.repository.gather_period(begin, end, era5sl_coordinates)
         ds = ds.sel(time=slice(begin, end))  # Slice of any overflowing time-range
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/cds/models/era5sl.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/cds/models/era5sl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-    CDS - ERA5 Single Levels Weather data Model
+"""CDS - ERA5 Single Levels Weather data Model
 """
 import copy
 from datetime import datetime
 from typing import List, Optional
 
 import numpy as np
 import xarray as xr
 from loguru import logger
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
-from weather_provider_api.routers.weather.sources.cds.client.era5sl_repository import ERA5SLRepository
+from weather_provider_api.routers.weather.sources.cds.client.era5sl_repository import (
+    ERA5SLRepository,
+)
 from weather_provider_api.routers.weather.sources.cds.factors import era5sl_factors
-from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
+from weather_provider_api.routers.weather.utils.date_helpers import (
+    validate_begin_and_end,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class ERA5SLModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
+    """A Weather Model that incorporates the:
         ERA5 hourly data on single levels from 1979 to present
     dataset into the Weather Provider API
     """
 
     def __init__(self):
         super().__init__()
         self.id = "era5sl"
@@ -74,26 +76,26 @@
     def get_weather(
         self,
         coords: List[GeoPosition],
         begin: datetime,
         end: datetime,
         weather_factors: List[str] = None,
     ) -> xr.Dataset:
-        """
-            The function that gathers and processes the requested ERA5 Single Levels weather data from the repository
+        """The function that gathers and processes the requested ERA5 Single Levels weather data from the repository
             and returns it as a Xarray Dataset.
+
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
         """
-
         # Test and account for invalid datetime timeframes or input
         begin, end = validate_begin_and_end(
             begin,
             end,
             self.repository.first_day_of_repo,
             self.repository.last_day_of_repo,
         )
@@ -102,20 +104,21 @@
         validated_factors = self._validate_weather_factors(weather_factors)
 
         ds = self._fill_dataset_with_data(coords, begin, end, validated_factors)
         return ds
 
     @staticmethod
     def _validate_weather_factors(weather_factors: List[str]) -> List[str]:
-        """
-            A function that validates a list of weather factors to that of the dataset in the repository.
+        """A function that validates a list of weather factors to that of the dataset in the repository.
             Existing factors will be kept, non-existing removed, and if the list is empty the full set for the dataset
             will be used.
+
         Args:
             weather_factors:    A list of weather factors to validate (in string format)
+
         Returns:
             A list of weather factors (in string format) only factors that match those of the ERA5SL dataset.
         """
         if weather_factors is None:
             weather_factors = [era5sl_factors[x] for x in list(era5sl_factors.keys())]
 
         # Lookup using the generic long name
@@ -140,22 +143,23 @@
     def _fill_dataset_with_data(
         self,
         era5sl_coordinates: List[GeoPosition],
         begin: datetime,
         end: datetime,
         validated_factors: List[str],
     ) -> xr.Dataset:
-        """
-            A function that fills a dataset with ERA5SL weather data from the repository, based on the requested
+        """A function that fills a dataset with ERA5SL weather data from the repository, based on the requested
             coordinates and period, and removes any not-requested weather factors from the output.
+
         Args:
             era5sl_coordinates:     A list of GeoPositions containing the locations to be gathered from the repository.
             begin:                  A datetime containing the starting moment for the period to gather.
             end:                    A datetime containing the end moment for the period to gather.
             validated_factors:      A list of valid ERA5SL factors wanted for the result.
+
         Returns:
             An Xarray Dataset containing the weather data requested.
         """
         # Gather a dataset with the proper period and coordinates
         ds = self.repository.gather_period(begin, end, era5sl_coordinates)
 
         ds = ds.sel(time=slice(np.datetime64(begin), np.datetime64(end)))
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" This module houses the repository class for the Actuele Waarnemingen Register. """
+"""This module houses the repository class for the Actuele Waarnemingen Register."""
 from datetime import datetime
 from typing import List
 
 import xarray as xr
 from dateutil import tz
 from dateutil.relativedelta import relativedelta
 from loguru import logger
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.dataset_name = "harmonie_arome_cy40_p1"
         self.dataset_version = "0.2"
         self.file_identifier_length = 13
         self.time_encoding = "hours since 2018-01-01"  # Used to keep values usable for at least the upcoming decennium
 
         # Verify if cfgrib is properly installed
         try:
-            import cfgrib
+            pass
         except RuntimeError as e:
             logger.warning(f"CFGRIB could not properly be initialized: {e}")
             logger.warning(
                 "Due to problems with CFGRIB, this repository will only be able to access existing "
                 "data. The repository will not be able to update"
             )
 
@@ -197,15 +197,14 @@
         except Exception as e:
             logger.error(f"The tarfile [{file_name}] could not be unpacked!")
             raise e
 
     def _convert_unpacked_data_to_netcdf4_files(self, download_folder: Path, prediction_time: datetime):
         """This function converts any unpacked data files into NetCDF4 files"""
         try:
-            import cfgrib
 
             logger.debug("Import of cfgrib was successful")
         except RuntimeError as e:
             logger.error("CFGRIB was not properly installed. Cannot access GRIB files.")
             raise e
 
         grib_files_available = glob.glob(
@@ -261,17 +260,15 @@
 
     def _process_grib_message_to_message_dataset(
         self,
         grib_message: cfgrib.Message,
         prediction_moment: datetime,
         predicted_hour: int,
     ) -> (str, xr.Dataset):
-        """
-
-        Args:
+        """Args:
             grib_message (grib.Message):    A GRIB message holding the data to process
             prediction_moment (datetime):   The datetime moment the data was generated
             predicted_hour (int):           The hour it is predicting
 
         Returns:
             (str, xarray.Dataset): A string holding the parameter name and a Xarray Dataset holding the data that was
             converted a dataset.
@@ -336,17 +333,15 @@
 
         time_cet -= relativedelta(hours=knmi_lag_time)  # Subtract the KNMI lag
         rounded_hour = (time_cet.hour // 6) * 6  # Get the nearest preceding hours divisible by six
         time_cet = time_cet.replace(hour=rounded_hour, minute=0, second=0)
         return time_cet
 
     def _fuse_hourly_netcdf4_files(self, download_folder: Path, prediction_moment: datetime):
-        """
-
-        Args:
+        """Args:
             download_folder:
             prediction_moment:
 
         Returns:
 
         """
         logger.info(f"Starting merge of all files for: {prediction_moment}")
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
-""" Module that holds the KNMI Downloader class
+"""Module that holds the KNMI Downloader class
 """
 
 import os
 import re
 import shutil
 import tempfile
 from pathlib import Path
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/knmi.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/knmi.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" KNMI current weather data fetcher.
+"""KNMI current weather data fetcher.
 """
 import copy
 from typing import List, Optional
 
 import numpy as np
 import xarray as xr
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
 from weather_provider_api.routers.weather.sources.knmi.stations import (
     stations_actual,
 )
 from weather_provider_api.routers.weather.sources.knmi.utils import (
-    find_closest_stn_list,
     download_actuele_waarnemingen_weather,
+    find_closest_stn_list,
 )
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class ActueleWaarnemingenModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
-    "KNMI Actuele Waarnemingen" dataset into the Weather Provider API
+    """A Weather Model that incorporates the "KNMI Actuele Waarnemingen"
+    dataset into the Weather Provider API.
     """
 
     def __init__(self):
         super().__init__()
         self.id = "waarnemingen"
         self.name = "KNMI Actuele Waarnemingen"
         self.version = ""
@@ -62,30 +61,29 @@
     def get_weather(
         self,
         coords: List[GeoPosition],
         begin: Optional[np.datetime64],
         end: Optional[np.datetime64],
         weather_factors: List[str] = None,
     ) -> xr.Dataset:
-        """
-        The function that gathers and processes the requested Actuele Waarnemingen weather data from the KNMI site
+        """The function that gathers and processes the requested Actuele Waarnemingen weather data from the KNMI site
         and returns it as a Xarray Dataset.
         (This model interprets directly from an HTML page, but the information is also available from the data
         platform. Due to it being rather impractically handled, we stick to the site for now.)
 
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
 
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
 
-        NOTES:
+        Notes:
             As this model only return the current weather data the 'begin' and 'end' values are not actually used.
         """
         updated_weather_factors = self._request_weather_factors(weather_factors)
 
         # Download the current weather data
         raw_ds = download_actuele_waarnemingen_weather()
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" KNMI current weather data aggregate fetcher.
+"""KNMI current weather data aggregate fetcher.
 """
 import copy
 from datetime import datetime
 from typing import List, Optional
 
 import numpy as np
 import xarray as xr
@@ -23,16 +23,15 @@
     find_closest_stn_list,
 )
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class ActueleWaarnemingenRegisterModel(WeatherModelBase):
-    """
-    A Weather model aimed at accessing a 24-hour register for the "KNMi Actuele Waarnemingen" dataset.
+    """A Weather model aimed at accessing a 24-hour register for the "KNMi Actuele Waarnemingen" dataset.
     """
 
     def is_async(self):
         return self.async_model
 
     def __init__(self):
         super().__init__()
@@ -67,30 +66,29 @@
     def get_weather(
         self,
         coords: List[GeoPosition],
         begin: Optional[np.datetime64],
         end: Optional[np.datetime64],
         weather_factors: List[str] = None,
     ) -> xr.Dataset:
-        """
-        The function that gathers and processes the requested Actuele Waarnemingen Register weather data from the
+        """The function that gathers and processes the requested Actuele Waarnemingen Register weather data from the
         48-hour register and returns it as a Xarray Dataset.
         (The register for this model interprets directly from an HTML page, but the information is also available from
         the data platform. Due to it being rather impractically handled, we stick to the site for now.)
 
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
 
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
 
-        NOTES:
+        Notes:
             As this model only return the current weather data the 'begin' and 'end' values are not actually used.
         """
         updated_weather_factors = self._request_weather_factors(weather_factors)
         coords_stn, _, _ = find_closest_stn_list(stations_actual, coords)
 
         now = datetime.utcnow()
         if now - relativedelta(days=1) > begin:
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-    KNMI day models data fetcher.
+"""KNMI day models data fetcher.
 """
 
 import copy
 import json
 from datetime import datetime
 from typing import List, Optional
 
@@ -29,16 +28,15 @@
     validate_begin_and_end,
 )
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class DagGegevensModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
+    """A Weather Model that incorporates the:
         KNMI Daggegevens
     dataset into the Weather Provider API
     """
 
     def __init__(self):
         super().__init__()
         self.id = "daggegevens"
@@ -182,25 +180,26 @@
             self,
             coords: List[GeoPosition],
             begin: datetime,
             end: datetime,
             inseason=False,
             weather_factors: List[str] = None,
     ) -> xr.Dataset:
-        """
-            The function that gathers and processes the requested Daggegevens weather data from the KNMI site
+        """The function that gathers and processes the requested Daggegevens weather data from the KNMI site
             and returns it as a Xarray Dataset.
             (Though this model downloads from a specific download url, the question remains whether this source is also
             listed on the new KNMI Data Platform)
+
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             inseason:           A boolean representing the "inseason" parameter
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
         """
         # Test and account for invalid datetime timeframes or input
         begin, end = validate_begin_and_end(begin, end, None, datetime.utcnow() - relativedelta(days=1))
         # Get a list of the relevant STNs and choose the closest STN for each coordinate
         station_id, stns, _ = find_closest_stn_list(stations_history, coords)
@@ -232,22 +231,22 @@
             self,
             stations: List[int],
             start: datetime,
             end: datetime,
             inseason=False,
             weather_factors: List[str] = None,
     ):
-        """
-            A function that downloads the weather from the KNMI download location and returns it as a text
+        """A function that downloads the weather from the KNMI download location and returns it as a text
         Args:
             stations:           A list containing the requested stations
             start:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             inseason:           A boolean representing the "inseason" parameter
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             A field containing the full response of the made download-request (text-based)
         """
         # fetch data
         params = self._create_request_params(start, end, inseason, stations, weather_factors)
         r = requests.post(url=self.download_url, data=params)
 
@@ -257,22 +256,23 @@
                 r.status_code,
                 self.download_url,
                 params,
             )
         return r.text
 
     def _create_request_params(self, start, end, inseason, stations, weather_factors):
-        """
-            A Function that transforms the request settings into parameters usable for the KMNI download request.
+        """A Function that transforms the request settings into parameters usable for the KMNI download request.
+
         Args:
             start:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             inseason:           A boolean representing the "inseason" parameter
             stations:           A list containing the requested stations
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             A params field (string) containing the matching settings for a KNMI Daggegevens download request.
         """
         params = {
             "fmt": "json",
             "stns": ":".join(str(station) for station in stations),
             "start": start.strftime("%Y%m%d"),
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-""" -- MODULE --
+"""-- MODULE --
 
 """
 import copy
 from datetime import datetime, time, timedelta
 from typing import List, Union
 
 import xarray as xr
 from loguru import logger
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
-from weather_provider_api.routers.weather.sources.knmi.client.arome_repository import HarmonieAromeRepository
+from weather_provider_api.routers.weather.sources.knmi.client.arome_repository import (
+    HarmonieAromeRepository,
+)
 from weather_provider_api.routers.weather.sources.knmi.knmi_factors import arome_factors
-from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
+from weather_provider_api.routers.weather.utils.date_helpers import (
+    validate_begin_and_end,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 class HarmonieAromeModel(WeatherModelBase):
     """A weather model that incorporates the 'KNMI - Harmonie Arome' weather dataset into the Weather Provider
      Libraries and API.
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/pluim.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/pluim.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 import numpy as np
 import requests
 import xarray as xr
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
-from weather_provider_api.routers.weather.sources.knmi.stations import stations_prediction
-from weather_provider_api.routers.weather.sources.knmi.utils import find_closest_stn_list
-from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
+from weather_provider_api.routers.weather.sources.knmi.stations import (
+    stations_prediction,
+)
+from weather_provider_api.routers.weather.sources.knmi.utils import (
+    find_closest_stn_list,
+)
+from weather_provider_api.routers.weather.utils.date_helpers import (
+    validate_begin_and_end,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class PluimModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
+    """A Weather Model that incorporates the:
         KNMI Pluim
     dataset into the Weather Provider API
     """
 
     def __init__(self):
         super().__init__()
         self.id = "pluim"
@@ -98,28 +103,28 @@
         self,
         coords: List[GeoPosition],
         begin: datetime,
         end: datetime,
         weather_factors: List[str] = None,
         **_kwargs,
     ) -> xr.Dataset:
-        """
-            The function that gathers and processes the requested Daggegevens weather data from the KNMI site
+        """The function that gathers and processes the requested Daggegevens weather data from the KNMI site
             and returns it as a Xarray Dataset.
             (Though this model downloads from a specific download url, the question remains whether this source is also
             listed on the new KNMI Data Platform)
+
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
         """
-
         # Test and account for invalid datetime timeframes or input
         begin, end = validate_begin_and_end(begin, end, datetime.utcnow(), datetime.utcnow() + relativedelta(days=15))
 
         # get list of relevant STNs, choose closest STN
         _, stns, coords_stn_ind = find_closest_stn_list(stations_prediction, coords)
 
         # load default weather factors if unspecified
@@ -132,20 +137,21 @@
         ds = self._select_weather_from_given_period(ds, begin, end)
         ds = ds.dropna("time", "all")  # Dropping any times that only carry NaN values
 
         return ds
 
     @staticmethod
     def _select_weather_from_given_period(ds: xr.Dataset, begin: datetime, end: datetime):
-        """
-            A function that filters the given Xarray Dataset to only the requested period.
+        """A function that filters the given Xarray Dataset to only the requested period.
+
         Args:
             ds:     An Xarray Dataset to be filtered
             begin:  A datetime containing the start of the period to filter.
             end:    A datetime containing the end of the period to filter.
+
         Returns:
             An Xarray Dataset containing all the data from the original dataset that matches the given period.
         """
         begin, end = validate_begin_and_end(
             begin,
             end,
             datetime.today().replace(hour=0, minute=0, second=0),
@@ -160,21 +166,22 @@
     def _download_weather(
         self,
         coordinates: List[GeoPosition],
         coords_stn_ind,
         stns,
         weather_factors: List[str],
     ):
-        """
-            A function that downloads the requested weather data, factor by factor.
+        """A function that downloads the requested weather data, factor by factor.
+
         Args:
             coordinates:        A list of GeoPositions containing the coordinates to request data for.
             coords_stn_ind:     A list of station coordinates in order
             stns:               A list of stations by ID in the same order
             weather_factors:    A list of weather factors to request the data for (string based)
+
         Returns:
             An Xarray Dataset containing the requested factors for the requested period and location(s).
         """
         arr_dict = {}
         ds = xr.Dataset()
         for weather_factor in weather_factors:
             try:
@@ -196,16 +203,15 @@
             )
             ds = xr.merge(arr_dict.values(), join="outer")
         ds = ds.unstack("coord")
         return ds
 
     @staticmethod
     def _download_single_stn_factor(stn: int, factor: int):
-        """
-            A function to download a single factor for a single station
+        """A function to download a single factor for a single station
         Args:
             stn:    The station (ID) to download the factor for
             factor: The weather factor to download
         Returns:
             A list of datetime64 items holding the times for the factors, and a matching list of values holding
             values belonging to the requested factor during those times.
         """
@@ -234,19 +240,19 @@
             timeline = np.array([x[0] for x in prediction_data]).astype("datetime64[ms]")
             # get value
             value = np.array([x[1] for x in prediction_data], dtype=np.float64)
 
         return timeline, value
 
     def _download_single_factor(self, stns: list, factor: int):
-        """
-            A function that downloads a single factor for all the given stations
+        """A function that downloads a single factor for all the given stations
         Args:
             stns:   A list of stations to download the factor for.
             factor: The weather factor to download.
+
         Returns:
             A list holding a timeline in datetime64 items as returned from the download requests, matching the request,
             and a list holding the values for the requested factor for all the stations in the order:
                 Station, Timeline
         """
         values = []
         timeline = []
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 import requests
 import xarray as xr
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 
 from weather_provider_api.routers.weather.base_models.model import WeatherModelBase
 from weather_provider_api.routers.weather.sources.knmi.stations import stations_history
-from weather_provider_api.routers.weather.sources.knmi.utils import find_closest_stn_list
-from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
+from weather_provider_api.routers.weather.sources.knmi.utils import (
+    find_closest_stn_list,
+)
+from weather_provider_api.routers.weather.utils.date_helpers import (
+    validate_begin_and_end,
+)
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class UurgegevensModel(WeatherModelBase):
     """A Weather Model that incorporates the: KNMI Uurgegevens dataset into the Weather Provider API."""
 
@@ -181,21 +185,21 @@
     def _download_weather(
         self,
         stations: List[int],
         start: datetime,
         end: datetime,
         weather_factors: List[str] | None = None,
     ):
-        """
-            A function that downloads the weather from the KNMI download location and returns it as a text
+        """A function that downloads the weather from the KNMI download location and returns it as a text
         Args:
             stations:           A list containing the requested stations
             start:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             A field containing the full response of the made download-request (text-based)
         """
         # fetch data
         params = self._create_request_params(start, end, stations, weather_factors)
         r = requests.post(url=self.download_url, data=params, timeout=60)
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/stations.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/stations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-    The list of stations used in various KNMI datasets.
+"""The list of stations used in various KNMI datasets.
 """
 
 from collections import namedtuple
 
 import numpy as np
 import pandas as pd
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/knmi/utils.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/knmi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,36 +24,35 @@
 )
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 
 
 def find_closest_stn_list(
         stn_stations: pd.DataFrame, coords: List[GeoPosition]
 ) -> tuple[list[np.int64], list[np.int64], list[int]]:
-    """
-            A function that finds the closest stations to the locations in the given list of GeoPositions
+    """A function that finds the closest stations to the locations in the given list of GeoPositions
     Args:
             stn_stations:   A Pandas Dataframe containing all the station data for the KNMI stations
             coords:         A list of GeoPositions with locations to find the nearest stations to.
-        Returns:
+
+    Returns:
             A list of coordinates for found stations
             A list of found stations in the same order
             A list of index numbers for the found in the same order
     """
     _stn_stations = stn_stations.copy(deep=True)
 
     # get list of relevant STNs, choose closest STN
     coords_stn = [_find_closest_stn_single(_stn_stations, coord) for coord in coords]
     stns = list(set(coords_stn))
     coords_stn_ind = [stns.index(x) for x in coords_stn]
     return coords_stn, stns, coords_stn_ind
 
 
 def _find_closest_stn_single(stn_stations: pd.DataFrame, coord: GeoPosition) -> np.int64:
-    """
-        A function that finds the closest station to a single GeoPosition
+    """A function that finds the closest station to a single GeoPosition
     Args:
         stn_stations:   A Pandas Dataframe containing all the station data for the KNMI stations
         coord:          A GeoPosition to find the nearest station for
     Returns:
         A station number indicating its index in the supplied dataframe.
     """
     stn_stations["distance"] = stn_stations.apply(
@@ -126,16 +125,15 @@
     except (requests.exceptions.BaseHTTPError, IndexError) as expected_error:
         logger.exception(str(expected_error))
 
     return raw_ds
 
 
 def _retrieve_observation_moment(html_body: str) -> datetime:
-    """
-    A function that extracts the observation date from the supplied html body of the Actuele Waarnemingen site.
+    """A function that extracts the observation date from the supplied html body of the Actuele Waarnemingen site.
 
     Args:
         html_body:  The text from the body downloaded from the Actuele Waarnemingen Site.
 
     Returns:
         Either the matching datetime if it can be extracted, or the current datetime if it cannot.
     """
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""
-    Class to retrieve the current Weather Alert status according to the KNMI site
+"""Class to retrieve the current Weather Alert status according to the KNMI site
 """
 
 from enum import Enum
 
 import requests
 from bs4 import BeautifulSoup
 from requests.adapters import HTTPAdapter
@@ -22,16 +21,15 @@
     green = "green"
     yellow = "yellow"
     orange = "orange"
     red = "red"
 
 
 class WeatherAlert:
-    """
-    A class (not a Weather Model!) that parses the Weather Alert status from the KNMI site (Weeralarm)
+    """A class (not a Weather Model!) that parses the Weather Alert status from the KNMI site (Weeralarm)
     """
 
     def __init__(self):
         self.id = "weatheralert"
         self.name = "KNMI Weather Alert"
         self.version = "0.8"
         self.url = "https://www.knmi.nl/nederland-nu/weer/waarschuwingen/"
@@ -48,17 +46,17 @@
             "overijssel",
             "utrecht",
             "zeeland",
             "zuid-holland",
         )  # The Dutch Provinces. Every province has its own page.
 
     def get_alarm(self):
-        """
-            A function that retrieves the current weather alarm stage for each of the Dutch provinces and puts those
+        """A function that retrieves the current weather alarm stage for each of the Dutch provinces and puts those
             together into a formatted list of results (string-based).
+
         Returns:
             A list of strings holding all the provinces and their retrieved current alarm stages according to KNMI
         """
         alarm_list = []
         for province in self.provinces:
             # Every province is available from a different page, so we have to request all of them separately
             page_text = ""
@@ -75,20 +73,21 @@
 
             append_string = self.process_page(page_text, status_code, province)
             alarm_list.append(append_string)
         return alarm_list
 
     @staticmethod
     def process_page(page_text: str, status_code, province):
-        """
-            A function that parses the weather alert page for a province and retrieves its current alarm stage.
+        """A function that parses the weather alert page for a province and retrieves its current alarm stage.
+
         Args:
             page_text:      The response content retrieved while trying to download the page
             status_code:    The status code retrieved while trying to download the page.
             province:       The province associated with the url, status code and alarm stage.
+
         Returns:
             A tuple holding the province and a result-string for that province.
             A result-string usually hold the alarm stage for that province, but can also hold exceptions when
             downloading did not succeed as intended.
         """
         if status_code == 200 and page_text is not None:
             # A page was found and loaded
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/date_helpers.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/date_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         return True
     return False
 
 
 def validate_begin_and_end(
     start: datetime, end: datetime, data_start: Union[datetime, None] = None, data_end: Union[datetime, None] = None
 ):
-    """
-    Checks the given date parameters and replaces them with default values if they aren't valid.
+    """Checks the given date parameters and replaces them with default values if they aren't valid.
     The resulting values are then returned.
     """
     if data_end is None:
         # Assuming predictions fill in this value, the most recent value for the past is before "now".
         data_end = datetime.utcnow()
 
     if data_start is not None and data_start > start:
```

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/file_helpers.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/geo_position.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/geo_position.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/grid_helpers.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/routers/weather/utils/serializers.py` & `weather_provider_api-2.52.38/weather_provider_api/routers/weather/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/versions/v1.py` & `weather_provider_api-2.52.38/weather_provider_api/versions/v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/weather_provider_api/versions/v2.py` & `weather_provider_api-2.52.38/weather_provider_api/versions/v2.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.51.37/PKG-INFO` & `weather_provider_api-2.52.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_provider_api
-Version: 2.51.37
+Version: 2.52.38
 Summary: Weather Provider Libraries and API
 Home-page: https://github.com/alliander-opensource/wpla/
 License: MPL-2.0
 Author: Verbindingsteam
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

