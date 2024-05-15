# Comparing `tmp/mapchete-2024.5.0.tar.gz` & `tmp/mapchete-2024.5.1.tar.gz`

## Comparing `mapchete-2024.5.0.tar` & `mapchete-2024.5.1.tar`

### file list

```diff
@@ -1,114 +1,110 @@
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/__init__.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/enums.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/errors.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/index.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/log.py
--rw-r--r--   0        0        0    33243 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/path.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/pretty.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/protocols.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/registered.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/settings.py
--rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/stac.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/testing.py
--rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/tile.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/timer.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/types.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/main.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/mpath.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/options.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/progress_bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/__init__.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/observer.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/parser.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/contours.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/__init__.py
--rw-r--r--   0        0        0    33124 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/base.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/models.py
--rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/parse.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/process_func.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/__init__.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/base.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/concurrent_futures.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/dask.py
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/future.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/sequential.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/types.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/base.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/loaders.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/models.py
--rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22077 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    16775 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_json.py
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_misc.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_path.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/profiles.py
--rw-r--r--   0        0        0    22406 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/vector.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/__init__.py
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/array.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/convert.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/mosaic.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/open.py
--rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/read.py
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/referenced_raster.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/write.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/__init__.py
--rw-r--r--   0        0        0    29802 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/base.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/execute.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/mp.py
--rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/types.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/memory.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/requests.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/index.html
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.5.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.5.0/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.5.0/README.rst
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 mapchete-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 mapchete-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/__init__.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/enums.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/errors.py
+-rw-r--r--   0        0        0    17605 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/index.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/log.py
+-rw-r--r--   0        0        0    33227 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/path.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/pretty.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/protocols.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/registered.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/settings.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/stac.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/testing.py
+-rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/tile.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/timer.py
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/types.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/main.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/mpath.py
+-rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/options.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/progress_bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/convert.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/cp.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/execute.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/index.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/observer.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/parser.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/commands/rm.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/config/__init__.py
+-rw-r--r--   0        0        0    33609 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/config/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/config/models.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/config/parse.py
+-rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/config/process_func.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/__init__.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/base.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/concurrent_futures.py
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/dask.py
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/future.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/sequential.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/executor/types.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20399 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/base.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/protocols.py
+-rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/_path.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/profiles.py
+-rw-r--r--   0        0        0    20397 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/__init__.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/array.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/convert.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/mosaic.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/open.py
+-rw-r--r--   0        0        0    17643 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/read.py
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/referenced_raster.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/io/raster/write.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/clip.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/__init__.py
+-rw-r--r--   0        0        0    30124 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/base.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/execute.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/mp.py
+-rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/types.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/profilers/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/profilers/memory.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/profilers/requests.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/processing/profilers/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/static/index.html
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.5.1/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.5.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.5.1/README.rst
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 mapchete-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 mapchete-2024.5.1/PKG-INFO
```

### Comparing `mapchete-2024.5.0/mapchete/__init__.py` & `mapchete-2024.5.1/mapchete/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 import logging
 import os
-from typing import Optional, Union
+from typing import Union
 
 from fsspec import AbstractFileSystem
 
 from mapchete.config import MapcheteConfig
+from mapchete.errors import Empty, MapcheteNodataTile
 from mapchete.executor import Executor, MFuture
 from mapchete.formats import read_output_metadata
+from mapchete.formats.protocols import (
+    RasterInput,
+    RasterInputGroup,
+    VectorInput,
+    VectorInputGroup,
+)
 from mapchete.path import MPath, fs_from_path
 from mapchete.processing import Mapchete, MapcheteProcess
 from mapchete.tile import count_tiles
 from mapchete.timer import Timer
 from mapchete.types import MPathLike
 
 __all__ = [
     "count_tiles",
     "Mapchete",
     "MapcheteProcess",
     "Timer",
     "Executor",
+    "Empty",
+    "MapcheteNodataTile",
     "MFuture",
+    "RasterInput",
+    "RasterInputGroup",
+    "VectorInput",
+    "VectorInputGroup",
 ]
-__version__ = "2024.5.0"
+__version__ = "2024.5.1"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def open(
     some_input: Union[MPathLike, dict, MapcheteConfig],
     with_cache: bool = False,
-    fs: Optional[AbstractFileSystem] = None,
-    fs_kwargs: Optional[dict] = None,
     **kwargs,
 ) -> Mapchete:
     """
     Open a Mapchete process.
 
     Parameters
     ----------
@@ -68,32 +79,28 @@
     """
     # convert to MPath object if possible
     if isinstance(some_input, str):
         some_input = MPath.from_inp(some_input)
     # for TileDirectory inputs
     if isinstance(some_input, MPath) and some_input.suffix == "":
         logger.debug("assuming TileDirectory")
-        metadata_json = MPath.from_inp(some_input).joinpath("metadata.json")
-        fs_kwargs = fs_kwargs or {}
-        fs = fs or fs_from_path(metadata_json, **fs_kwargs)
+        metadata_json = MPath.from_inp(some_input) / "metadata.json"
         logger.debug("read metadata.json")
-        metadata = read_output_metadata(metadata_json, fs=fs)
+        metadata = read_output_metadata(metadata_json)
         config = dict(
             process=None,
             input=None,
             pyramid=metadata["pyramid"].to_dict(),
             output=dict(
                 {
                     k: v
                     for k, v in metadata["driver"].items()
                     if k not in ["delimiters", "mode"]
                 },
                 path=some_input,
-                fs=fs,
-                fs_kwargs=fs_kwargs,
                 **kwargs,
             ),
             config_dir=os.getcwd(),
             zoom_levels=kwargs.get("zoom"),
         )
         kwargs.update(mode="readonly")
         return Mapchete(MapcheteConfig(config, **kwargs))
```

### Comparing `mapchete-2024.5.0/mapchete/enums.py` & `mapchete-2024.5.1/mapchete/enums.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/errors.py` & `mapchete-2024.5.1/mapchete/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     """Generic exception raised by a driver if input tile is empty."""
 
 
 class MapcheteNodataTile(Exception):
     """Indicates an empty tile."""
 
 
+class Empty(MapcheteNodataTile):
+    """Short alias for MapcheteNodataTile."""
+
+
 class GeometryTypeError(TypeError):
     """Raised when geometry type does not fit."""
 
 
 class MapcheteIOError(IOError):
     """Raised when mapchete cannot read a file."""
```

### Comparing `mapchete-2024.5.0/mapchete/index.py` & `mapchete-2024.5.1/mapchete/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,14 @@
 
 
 class VRTFileWriter:
     """Generates GDAL-style VRT file."""
 
     def __init__(self, out_path=None, output=None, out_pyramid=None):
         # see if lxml is installed before checking all output tiles
-        from lxml.builder import ElementMaker
 
         self.path = out_path
         self._tp = out_pyramid
         self._output = output
         self.fs = fs_from_path(out_path)
         logger.debug("initialize VRT writer for %s", self.path)
         if path_exists(self.path):
```

### Comparing `mapchete-2024.5.0/mapchete/log.py` & `mapchete-2024.5.1/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/path.py` & `mapchete-2024.5.1/mapchete/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import oyaml as yaml
 import rasterio
 from fiona.session import Session as FioSession
 from fsspec import AbstractFileSystem
 from rasterio.session import Session as RioSession
 from retry import retry
 
-import mapchete
 from mapchete.executor import Executor
 from mapchete.settings import GDALHTTPOptions, IORetrySettings, mapchete_options
 from mapchete.tile import BufferedTile
 from mapchete.types import MPathLike
 
 logger = logging.getLogger(__name__)
```

### Comparing `mapchete-2024.5.0/mapchete/pretty.py` & `mapchete-2024.5.1/mapchete/pretty.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/registered.py` & `mapchete-2024.5.1/mapchete/registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/settings.py` & `mapchete-2024.5.1/mapchete/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/stac.py` & `mapchete-2024.5.1/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/testing.py` & `mapchete-2024.5.1/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/tile.py` & `mapchete-2024.5.1/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/timer.py` & `mapchete-2024.5.1/mapchete/timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/types.py` & `mapchete-2024.5.1/mapchete/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from typing import Iterable, List, Optional, Tuple, Union
 
 from affine import Affine
 from fiona.crs import CRS as FionaCRS
 from pydantic import BaseModel
 from rasterio.crs import CRS as RasterioCRS
+from rasterio.enums import Resampling
 from rasterio.transform import array_bounds, from_bounds
 from shapely.geometry import shape
 from shapely.geometry.base import BaseGeometry
 from tilematrix import Shape
 
 from mapchete.tile import BufferedTile
 
@@ -18,14 +19,17 @@
 BoundsLike = Union[List[float], Tuple[float], dict, BaseGeometry]
 ShapeLike = Union[Shape, List[int], Tuple[int, int]]
 ZoomLevelsLike = Union[List[int], int, dict]
 TileLike = Union[BufferedTile, Tuple[int, int, int]]
 CRSLike = Union[FionaCRS, RasterioCRS]
 NodataVal = Optional[float]
 NodataVals = Union[List[NodataVal], NodataVal]
+ResamplingLike = Union[Resampling, str]
+BandIndex = int
+BandIndexes = Union[BandIndex, List[BandIndex]]
 
 
 class Bounds(list):
     """
     Class to handle geographic bounds.
     """
```

### Comparing `mapchete-2024.5.0/mapchete/validate.py` & `mapchete-2024.5.1/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/mpath.py` & `mapchete-2024.5.1/mapchete/cli/mpath.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/options.py` & `mapchete-2024.5.1/mapchete/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
             zoom_levels = list(map(int, zoom.split(",")))
         except ValueError:
             raise click.BadParameter("zoom levels must be integer values")
         try:
             if len(zoom_levels) > 2:
                 raise ValueError("zooms can be maximum two items")
             return ZoomLevels.from_inp(zoom_levels)
-        except Exception as e:
-            raise click.BadParameter(e)
+        except Exception as exc:
+            raise click.BadParameter(str(exc))
 
 
 def _validate_bounds(ctx, param, bounds):
     if bounds:
         return Bounds.from_inp(bounds)
```

### Comparing `mapchete-2024.5.0/mapchete/cli/progress_bar.py` & `mapchete-2024.5.1/mapchete/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/convert.py` & `mapchete-2024.5.1/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/cp.py` & `mapchete-2024.5.1/mapchete/cli/default/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-import tqdm
 
 from mapchete import commands
 from mapchete.cli import options
 from mapchete.cli.progress_bar import PBar
 
 
 def _cb_none_concurrency(ctx, param, value):
```

### Comparing `mapchete-2024.5.0/mapchete/cli/default/create.py` & `mapchete-2024.5.1/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/execute.py` & `mapchete-2024.5.1/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/formats.py` & `mapchete-2024.5.1/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/index.py` & `mapchete-2024.5.1/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/processes.py` & `mapchete-2024.5.1/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/cli/default/rm.py` & `mapchete-2024.5.1/mapchete/cli/default/rm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 import tqdm
 
 from mapchete import commands
 from mapchete.cli import options
 from mapchete.cli.progress_bar import PBar
-from mapchete.commands._rm import existing_paths
+from mapchete.commands.rm import existing_paths
 
 
 @click.command(help="Remove tiles from TileDirectory.")
 @options.arg_tiledir
 @options.opt_zoom
 @options.opt_area
 @options.opt_area_crs
```

### Comparing `mapchete-2024.5.0/mapchete/cli/default/serve.py` & `mapchete-2024.5.1/mapchete/cli/default/serve.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,12 +173,12 @@
 
     out_data, mime_type = mp.config.output.for_web(data)
     logger.debug("create tile response %s", mime_type)
     if isinstance(out_data, MemoryFile):
         return RangeRequest(out_data).make_response()
     elif isinstance(out_data, list):
         response = make_response(jsonify(data))
-    else:
+    else:  # pragma: no cover
         response = make_response(out_data)
     response.headers["Content-Type"] = mime_type
     response.cache_control.no_write = True
     return response
```

### Comparing `mapchete-2024.5.0/mapchete/cli/default/stac.py` & `mapchete-2024.5.1/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/commands/_convert.py` & `mapchete-2024.5.1/mapchete/commands/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import os
 from contextlib import AbstractContextManager
 from multiprocessing import cpu_count
 from pprint import pformat
-from typing import List, NoReturn, Optional, Tuple, Type, Union
+from typing import List, Optional, Tuple, Type, Union
 
 import tilematrix
 from rasterio.crs import CRS
 from rasterio.enums import Resampling
 from shapely.geometry import box
 from shapely.geometry.base import BaseGeometry
 
-from mapchete.commands._execute import execute
+from mapchete.commands.execute import execute
 from mapchete.commands.observer import ObserverProtocol, Observers
 from mapchete.commands.parser import InputInfo, OutputInfo
 from mapchete.config import DaskSettings
 from mapchete.enums import Concurrency, DataType, ProcessingMode
 from mapchete.errors import JobCancelledError
 from mapchete.executor import Executor
 from mapchete.formats import available_output_formats
@@ -39,15 +39,15 @@
     point: Optional[Tuple[float, float]] = None,
     point_crs: Optional[Tuple[float, float]] = None,
     overwrite: bool = False,
     concurrency: Concurrency = Concurrency.processes,
     dask_settings: DaskSettings = DaskSettings(),
     workers: Optional[int] = None,
     clip_geometry: Optional[str] = None,
-    bidx: Optional[List[int]] = None,
+    bidx: Optional[Union[List[int], int]] = None,
     output_pyramid: Optional[Union[str, dict, MPathLike]] = None,
     output_metatiling: Optional[int] = None,
     output_format: Optional[str] = None,
     output_dtype: Optional[str] = None,
     output_geometry_type: Optional[str] = None,
     creation_options: Optional[dict] = None,
     scale_ratio: Optional[float] = None,
@@ -59,15 +59,15 @@
     src_fs_opts: Optional[dict] = None,
     dst_fs_opts: Optional[dict] = None,
     executor_getter: AbstractContextManager = Executor,
     observers: Optional[List[ObserverProtocol]] = None,
     retry_on_exception: Tuple[Type[Exception], Type[Exception]] = Exception,
     cancel_on_exception: Type[Exception] = JobCancelledError,
     retries: int = 0,
-) -> NoReturn:
+) -> None:
     """
     Convert mapchete outputs or other geodata.
 
     This is a wrapper around the mapchete.processes.convert process which helps generating tiled
     outputs for raster and vector data or single COGs from TileDirectory raster inputs.
 
     It also supports clipping of the input by a vector dataset.
@@ -117,17 +117,19 @@
                 pixelbuffer=(
                     input_info.output_pyramid.pixelbuffer
                     if input_info.output_pyramid
                     else 0
                 ),
             )
             if output_pyramid
-            else input_info.output_pyramid.to_dict()
-            if input_info.output_pyramid
-            else None
+            else (
+                input_info.output_pyramid.to_dict()
+                if input_info.output_pyramid
+                else None
+            )
         ),
         output=dict(
             {
                 k: v
                 for k, v in input_info.output_params.items()
                 if k not in ["delimiters", "bounds", "mode"]
             },
@@ -135,17 +137,19 @@
             format=(
                 output_format
                 or output_info.driver
                 or input_info.output_params["format"]
             ),
             dtype=output_dtype or input_info.output_params.get("dtype"),
             **creation_options,
-            **dict(overviews=True, overviews_resampling=overviews_resampling_method)
-            if overviews
-            else dict(),
+            **(
+                dict(overviews=True, overviews_resampling=overviews_resampling_method)
+                if overviews
+                else dict()
+            ),
         ),
         config_dir=os.getcwd(),
         zoom_levels=zoom or input_info.zoom_levels,
         process_parameters=dict(
             scale_ratio=scale_ratio,
             scale_offset=scale_offset,
             resampling=resampling_method,
@@ -181,15 +185,17 @@
     elif input_info.data_type != output_type:
         raise ValueError(
             f"Output format type ({output_type}) is incompatible with input format ({input_info.data_type})."
         )
     if output_metatiling:
         mapchete_config["pyramid"].update(metatiling=output_metatiling)
         mapchete_config["output"].update(metatiling=output_metatiling)
-    if input_info.output_params.get("schema") and output_geometry_type:
+    if (
+        input_info.output_params.get("schema") and output_geometry_type
+    ):  # pragma: no cover
         mapchete_config["output"]["schema"].update(geometry=output_geometry_type)
 
     # determine process bounds
     out_pyramid = BufferedTilePyramid.from_dict(mapchete_config["pyramid"])
     inp_bounds = (
         bounds
         or reproject_geometry(
```

### Comparing `mapchete-2024.5.0/mapchete/commands/_cp.py` & `mapchete-2024.5.1/mapchete/commands/cp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,92 @@
 """Copy tiles between Tile Directories."""
 
 import logging
-from contextlib import AbstractContextManager
 from multiprocessing import cpu_count
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Type, Union
 
-from rasterio.crs import CRS
+from distributed import Client
 from shapely.geometry import Point
 from shapely.geometry.base import BaseGeometry
 
 import mapchete
 from mapchete.commands.observer import ObserverProtocol, Observers
+from mapchete.enums import Concurrency
 from mapchete.executor import Executor
 from mapchete.io import MPath, copy, tiles_exist
 from mapchete.io.vector import reproject_geometry
-from mapchete.types import Progress
+from mapchete.types import BoundsLike, CRSLike, Progress, ZoomLevelsLike
 
 logger = logging.getLogger(__name__)
 
 
 def cp(
     src_tiledir: Union[str, MPath],
     dst_tiledir: Union[str, MPath],
-    zoom: Union[int, List[int]] = None,
-    area: Union[BaseGeometry, str, dict] = None,
-    area_crs: Union[CRS, str] = None,
-    bounds: Tuple[float] = None,
-    bounds_crs: Union[CRS, str] = None,
-    point: Tuple[float, float] = None,
-    point_crs: Tuple[float, float] = None,
+    zoom: ZoomLevelsLike,
+    area: Optional[Union[BaseGeometry, str, dict]] = None,
+    area_crs: Optional[CRSLike] = None,
+    bounds: Optional[BoundsLike] = None,
+    bounds_crs: Optional[CRSLike] = None,
+    point: Optional[Tuple[float, float]] = None,
+    point_crs: Optional[CRSLike] = None,
     overwrite: bool = False,
-    workers: Union[int, None] = None,
-    multi: Union[int, None] = None,
-    concurrency: Union[str, None] = None,
-    dask_scheduler: Union[str, None] = None,
-    dask_client=None,
+    workers: Optional[int] = None,
+    concurrency: Concurrency = Concurrency.threads,
+    dask_scheduler: Optional[str] = None,
+    dask_client: Optional[Client] = None,
     src_fs_opts: Union[dict, None] = None,
     dst_fs_opts: Union[dict, None] = None,
-    executor_getter: AbstractContextManager = Executor,
+    executor_getter: Type[Executor] = Executor,
     observers: Optional[List[ObserverProtocol]] = None,
 ):
     """
     Copy TileDirectory from source to destination.
-
-    Parameters
-    ----------
-    src_tiledir : str
-        Source TileDirectory or mapchete file.
-    dst_tiledir : str
-        Destination TileDirectory.
-    zoom : integer or list of integers
-        Single zoom, minimum and maximum zoom or a list of zoom levels.
-    area : str, dict, BaseGeometry
-        Geometry to override bounds or area provided in process configuration. Can be either a
-        WKT string, a GeoJSON mapping, a shapely geometry or a path to a Fiona-readable file.
-    area_crs : CRS or str
-        CRS of area (default: process CRS).
-    bounds : tuple
-        Override bounds or area provided in process configuration.
-    bounds_crs : CRS or str
-        CRS of area (default: process CRS).
-    point : iterable
-        X and y coordinates of point whose corresponding output tile bounds will be used.
-    point_crs : str or CRS
-        CRS of point (defaults to process pyramid CRS).
-    overwrite : bool
-        Overwrite existing output.
-    workers : int
-        Number of threads used to check whether tiles exist.
-    concurrency : str
-        Concurrency to be used. Could either be "processes", "threads" or "dask".
-    dask_scheduler : str
-        URL to dask scheduler if required.
-    dask_client : dask.distributed.Client
-        Reusable Client instance if required. Otherwise a new client will be created.
-    src_fs_opts : dict
-        Configuration options for source fsspec filesystem.
-    dst_fs_opts : dict
-        Configuration options for destination fsspec filesystem.
     """
 
     workers = workers or cpu_count()
     src_fs_opts = src_fs_opts or {}
     dst_fs_opts = dst_fs_opts or {}
-    if zoom is None:  # pragma: no cover
-        raise ValueError("zoom level(s) required")
 
     src_tiledir = MPath.from_inp(src_tiledir, storage_options=src_fs_opts)
     dst_tiledir = MPath.from_inp(dst_tiledir, storage_options=dst_fs_opts)
-    src_fs = src_tiledir.fs
-    dst_fs = dst_tiledir.fs
     all_observers = Observers(observers)
 
     # open source tile directory
     with mapchete.open(
         src_tiledir,
         zoom=zoom,
         area=area,
         area_crs=area_crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
-        fs=src_fs,
-        fs_kwargs=src_fs_opts,
         mode="readonly",
     ) as src_mp:
         tp = src_mp.config.output_pyramid
 
         # copy metadata to destination if necessary
         src_metadata = src_tiledir / "metadata.json"
         dst_metadata = dst_tiledir / "metadata.json"
-        if not dst_fs.exists(dst_metadata):
+        if not dst_tiledir.fs.exists(dst_metadata):
             msg = f"copy {src_metadata} to {dst_metadata}"
             logger.debug(msg)
             all_observers.notify(message=msg)
             copy(
                 src_metadata,
                 dst_metadata,
-                src_fs=src_fs,
-                dst_fs=dst_fs,
                 overwrite=overwrite,
             )
 
         with mapchete.open(
             dst_tiledir,
             zoom=zoom,
             area=area,
             area_crs=area_crs,
             bounds=bounds,
             bounds_crs=bounds_crs,
-            fs=dst_fs,
-            fs_kwargs=dst_fs_opts,
             mode="readonly",
         ) as dst_mp:
             with executor_getter(
                 concurrency=concurrency,
                 max_workers=workers,
                 dask_scheduler=dask_scheduler,
                 dask_client=dask_client,
@@ -181,16 +134,16 @@
                             _copy_tile,
                             tiles,
                             fargs=(
                                 src_mp,
                                 dst_mp,
                                 src_tiles_exist,
                                 dst_tiles_exist,
-                                src_fs,
-                                dst_fs,
+                                src_tiledir.fs,
+                                dst_tiledir.fs,
                                 overwrite,
                             ),
                         ),
                         1,
                     ):
                         copied, message = future.result()
                         total_copied += copied
```

### Comparing `mapchete-2024.5.0/mapchete/commands/_execute.py` & `mapchete-2024.5.1/mapchete/commands/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/commands/_index.py` & `mapchete-2024.5.1/mapchete/commands/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import mapchete
 from mapchete.commands.observer import ObserverProtocol, Observers
 from mapchete.commands.parser import InputInfo
 from mapchete.config import MapcheteConfig
 from mapchete.config.parse import bounds_from_opts, raw_conf
 from mapchete.enums import InputType
 from mapchete.index import zoom_index_gen
-from mapchete.path import MPath
 from mapchete.types import MPathLike, Progress
 
 logger = logging.getLogger(__name__)
 
 
 def index(
     some_input: Union[MPathLike, dict, MapcheteConfig],
```

### Comparing `mapchete-2024.5.0/mapchete/commands/_rm.py` & `mapchete-2024.5.1/mapchete/commands/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/commands/parser.py` & `mapchete-2024.5.1/mapchete/commands/parser.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/commons/hillshade.py` & `mapchete-2024.5.1/mapchete/processes/hillshade.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,23 +29,86 @@
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
+import logging
 import math
 import warnings
 from itertools import product
+from typing import Optional, Tuple
 
 import numpy as np
 import numpy.ma as ma
+from affine import Affine
+
+from mapchete import Empty, RasterInput, VectorInput
+from mapchete.io import MatchingMethod
+from mapchete.types import ResamplingLike
+
+logger = logging.getLogger(__name__)
+
+
+def execute(
+    dem: RasterInput,
+    clip: Optional[VectorInput] = None,
+    resampling: ResamplingLike = "nearest",
+    azimuth: float = 315.0,
+    altitude: float = 45.0,
+    z: float = 1.0,
+    scale: float = 1.0,
+    td_matching_method: MatchingMethod = MatchingMethod.gdal,
+    td_matching_max_zoom: Optional[int] = None,
+    td_matching_precision: int = 8,
+    td_fallback_to_higher_zoom: bool = False,
+) -> ma.MaskedArray:
+    """
+    Calculate hillshade from elevation.
+    """
+    # read clip geometry
+    if clip is None:
+        clip_geom = []
+    else:
+        clip_geom = clip.read()
+        if not clip_geom:
+            logger.debug("no clip data over tile")
+            raise Empty
+
+    if dem.is_empty():
+        raise Empty
+
+    logger.debug("reading input raster")
+    elevation_data = dem.read(
+        resampling=resampling,
+        matching_method=td_matching_method,
+        matching_max_zoom=td_matching_max_zoom,
+        matching_precision=td_matching_precision,
+        fallback_to_higher_zoom=td_fallback_to_higher_zoom,
+    )
+
+    if elevation_data.mask.all():  # pragma: no cover
+        raise Empty
+
+    logger.debug("calculate hillshade")
+    return hillshade(
+        elevation_data,
+        dem.tile.affine,
+        azimuth=azimuth,
+        altitude=altitude,
+        z=z,
+        scale=scale,
+    )
 
 
-def calculate_slope_aspect(elevation, xres, yres, z=1.0, scale=1.0):
+def calculate_slope_aspect(
+    elevation: np.ndarray, xres: float, yres: float, z: float = 1.0, scale: float = 1.0
+) -> Tuple[np.ndarray, np.ndarray]:
     """
     Calculate slope and aspect map.
 
     Return a pair of arrays 2 pixels smaller than the input elevation array.
 
     Slope is returned in radians, from 0 for sheer face to pi/2 for
     flat ground. Aspect is returned in radians, counterclockwise from -pi
@@ -92,21 +155,21 @@
         slope = math.pi / 2 - np.arctan(np.sqrt(x * x + y * y))
         # in radians counterclockwise, from -pi at north back to pi
         aspect = np.arctan2(x, y)
         return slope, aspect
 
 
 def hillshade(
-    elevation,
-    tile,
-    azimuth=315.0,
-    altitude=45.0,
-    z=1.0,
-    scale=1.0,
-):
+    elevation: ma.MaskedArray,
+    affine: Affine,
+    azimuth: float = 315.0,
+    altitude: float = 45.0,
+    z: float = 1.0,
+    scale: float = 1.0,
+) -> ma.MaskedArray:
     """
     Return hillshaded numpy array.
 
     Parameters
     ----------
     elevation : array
         Input elevation data.
@@ -123,20 +186,20 @@
         when having elevation values in meters in a geodetic projection).
     """
     elevation = elevation[0] if elevation.ndim == 3 else elevation
     azimuth = float(azimuth)
     altitude = float(altitude)
     z = float(z)
     scale = float(scale)
-    xres = tile.pixel_x_size
-    yres = -tile.pixel_y_size
+    xres = affine[0]
+    yres = affine[4]
     slope, aspect = calculate_slope_aspect(elevation, xres, yres, z=z, scale=scale)
     deg2rad = math.pi / 180.0
     # shaded has values between -1.0 and +1.0
     shaded = np.sin(altitude * deg2rad) * np.sin(slope) + np.cos(
         altitude * deg2rad
     ) * np.cos(slope) * np.cos((azimuth - 90.0) * deg2rad - aspect)
     # stretch to 0 - 255 and add one pixel padding using the edge values
     return ma.masked_array(
-        data=np.pad(np.clip(shaded * 255.0, 1, 255).astype("uint8"), 1, mode="edge"),
+        data=np.pad(np.clip(shaded * 255.0, 1, 255).astype(np.uint8), 1, mode="edge"),
         mask=elevation.mask,
     )
```

### Comparing `mapchete-2024.5.0/mapchete/config/base.py` & `mapchete-2024.5.1/mapchete/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 import logging
 import warnings
 from collections import OrderedDict
 from copy import deepcopy
 from functools import cached_property
 from typing import Any, Iterator, Optional, Tuple, Union
@@ -13,14 +15,15 @@
 
 from mapchete.config.models import ProcessConfig
 from mapchete.config.parse import (
     get_zoom_levels,
     guess_geometry,
     parse_config,
     raw_conf_at_zoom,
+    zoom_parameters,
 )
 from mapchete.config.process_func import ProcessFunc
 from mapchete.enums import ProcessingMode
 from mapchete.errors import MapcheteConfigError, MapcheteDriverError
 from mapchete.formats import (
     available_output_formats,
     load_input_reader,
@@ -136,15 +139,15 @@
             self.mode = ProcessingMode(mode)
         except Exception as exc:
             raise MapcheteConfigError from exc
         self.preprocessing_tasks_finished = False
 
         # (2) check user process
         self.config_dir = self.parsed_config.config_dir
-        if self.mode != "readonly":
+        if self.mode != ProcessingMode.READONLY:
             if self.parsed_config.process is None:
                 raise MapcheteConfigError(
                     f"process must be provided on {self.mode} mode"
                 )
             logger.debug("validating process code")
             self.process = ProcessFunc(
                 self.parsed_config.process, config_dir=self.config_dir
@@ -201,14 +204,23 @@
 
         # (5) prepare process parameters per zoom level without initializing
         # input and output classes
         logger.debug("preparing process parameters")
         self._params_at_zoom = raw_conf_at_zoom(
             self.parsed_config, self.init_zoom_levels
         )
+        # TODO: check execute function parameters and provide warnings in case parameters
+        # have been omitted, are not defined in the config, or have the wrong type
+        if self.process:
+            self.process.analyze_parameters(
+                {
+                    zoom: zoom_parameters(self.parsed_config, zoom)
+                    for zoom in self.init_zoom_levels
+                }
+            )
 
         # (6) determine process area and process boundaries both from config as well
         # as from initialization.
         # First, the area and bounds parameters from the configuration are checked. If
         # both are provided, the intersection will be taken into account. If none are,
         # the process pyramid area is assumed.
         # Second, they can be overrided by the area and bounds kwargs when constructing
@@ -935,17 +947,17 @@
         path = key.split("/")
         # we are at the end of a branch
         if len(path) == 1:
             tree[key] = value
         # there are more branches
         else:
             # create new dict
-            if not path[0] in tree:
+            if path[0] not in tree:
                 tree[path[0]] = _unflatten_tree({"/".join(path[1:]): value})
             # add keys to existing dict
             else:
                 branch = _unflatten_tree({"/".join(path[1:]): value})
-                if not path[1] in tree[path[0]]:
+                if path[1] not in tree[path[0]]:
                     tree[path[0]][path[1]] = branch[path[1]]
                 else:
                     tree[path[0]][path[1]].update(branch[path[1]])
     return tree
```

### Comparing `mapchete-2024.5.0/mapchete/config/models.py` & `mapchete-2024.5.1/mapchete/config/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from collections import OrderedDict
 from typing import List, Optional, Type, Union
 
 from distributed import Client
-from pydantic import BaseModel, ConfigDict, Field, NonNegativeInt, field_validator
+from pydantic import BaseModel, Field, NonNegativeInt, field_validator
 from shapely.geometry.base import BaseGeometry
 
 from mapchete.types import Bounds, BoundsLike, MPathLike, ZoomLevels, ZoomLevelsLike
 
 
 class OutputConfigBase(BaseModel):
     format: str
@@ -49,14 +50,22 @@
     scheduler_cores: int = 1
     scheduler_cores_limit: float = 1.0
     scheduler_memory: float = 1.0
     image: Optional[str] = None
     adapt_options: DaskAdaptOptions = DaskAdaptOptions()
 
 
+class DaskSettings(BaseModel):
+    process_graph: bool = True
+    max_submitted_tasks: int = 500
+    chunksize: int = 100
+    scheduler: Optional[str] = None
+    client: Optional[Type[Client]] = None
+
+
 class ProcessConfig(BaseModel, arbitrary_types_allowed=True):
     pyramid: PyramidConfig
     output: dict
     zoom_levels: Union[ZoomLevels, ZoomLevelsLike]
     process: Optional[Union[MPathLike, List[str]]] = None
     baselevels: Optional[dict] = None
     input: Optional[dict] = None
@@ -66,13 +75,10 @@
     area_crs: Optional[Union[dict, str]] = None
     bounds: Optional[Union[Bounds, BoundsLike]] = None
     bounds_crs: Optional[Union[dict, str]] = None
     process_parameters: dict = Field(default_factory=dict)
     dask_specs: Optional[DaskSpecs] = None
 
 
-class DaskSettings(BaseModel):
-    process_graph: bool = True
-    max_submitted_tasks: int = 500
-    chunksize: int = 100
-    scheduler: Optional[str] = None
-    client: Optional[Type[Client]] = None
+class ZoomParameters(BaseModel):
+    input: OrderedDict = Field(default_factory=OrderedDict)
+    process_parameters: OrderedDict = Field(default_factory=OrderedDict)
```

### Comparing `mapchete-2024.5.0/mapchete/config/parse.py` & `mapchete-2024.5.1/mapchete/config/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from rasterio.crs import CRS
 from shapely import wkt
 from shapely.geometry import Point, box, shape
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 
-from mapchete.config.models import ProcessConfig
+from mapchete.config.models import ProcessConfig, ZoomParameters
 from mapchete.errors import GeometryTypeError, MapcheteConfigError
 from mapchete.io.vector import clean_geometry_type, fiona_open, reproject_geometry
 from mapchete.path import MPath
 from mapchete.tile import BufferedTilePyramid
 from mapchete.types import Bounds, MPathLike, ZoomLevels, ZoomLevelsLike
 from mapchete.validate import validate_values
 
@@ -142,14 +142,24 @@
             out_element = element_at_zoom(name, element, zoom)
             if out_element is not None:
                 params[name] = out_element
         params_per_zoom[zoom] = params
     return OrderedDict(params_per_zoom)
 
 
+def zoom_parameters(config: ProcessConfig, zoom: int) -> ZoomParameters:
+    """Return parameter dictionary per zoom level."""
+    params = dict()
+    for name, element in config.model_dump().items():
+        out_element = element_at_zoom(name, element, zoom)
+        if out_element is not None:
+            params[name] = out_element
+    return ZoomParameters(**params)
+
+
 def element_at_zoom(name: str, element: Any, zoom: int) -> Any:
     """
     Return the element filtered by zoom level.
 
     - An input integer or float gets returned as is.
     - An input string is checked whether it starts with "zoom". Then, the
       provided zoom level gets parsed and compared with the actual zoom
```

### Comparing `mapchete-2024.5.0/mapchete/executor/__init__.py` & `mapchete-2024.5.1/mapchete/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/executor/base.py` & `mapchete-2024.5.1/mapchete/executor/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/executor/concurrent_futures.py` & `mapchete-2024.5.1/mapchete/executor/concurrent_futures.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/executor/dask.py` & `mapchete-2024.5.1/mapchete/executor/dask.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from dask.distributed import Client, LocalCluster, as_completed, wait
 
 from mapchete.errors import JobCancelledError
 from mapchete.executor.base import ExecutorBase
 from mapchete.executor.future import MFuture
 from mapchete.executor.types import Result
 from mapchete.pretty import pretty_bytes
-from mapchete.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 
 class DaskExecutor(ExecutorBase):
     """Execute tasks using dask cluster."""
```

### Comparing `mapchete-2024.5.0/mapchete/executor/future.py` & `mapchete-2024.5.1/mapchete/executor/future.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/executor/sequential.py` & `mapchete-2024.5.1/mapchete/executor/sequential.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/__init__.py` & `mapchete-2024.5.1/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/base.py` & `mapchete-2024.5.1/mapchete/formats/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,40 +5,81 @@
 respective interfaces.
 """
 
 import logging
 import types
 import warnings
 from itertools import chain
+from typing import Any, List, Optional, Tuple
 
 import numpy as np
 import numpy.ma as ma
+from pydantic import NonNegativeInt
 from shapely.geometry import shape
 
 from mapchete.config import get_hash
 from mapchete.errors import MapcheteNodataTile, MapcheteProcessOutputError
 from mapchete.formats import write_output_metadata
-from mapchete.io import fs_from_path, path_exists
+
+# from mapchete.formats.models import BaseInputParams
+from mapchete.formats.protocols import InputDataProtocol, InputTileProtocol
 from mapchete.io.raster import (
     create_mosaic,
     extract_from_array,
     prepare_array,
     read_raster_window,
 )
 from mapchete.io.vector import read_vector_window
+from mapchete.path import MPath
 from mapchete.processing.tasks import Task
-from mapchete.tile import BufferedTilePyramid
+from mapchete.tile import BufferedTile, BufferedTilePyramid
+from mapchete.types import CRSLike
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_TILE_PATH_SCHEMA = "{zoom}/{row}/{col}.{extension}"
 
 
-class InputData(object):
+class InputTile(InputTileProtocol):
+    """
+    Target Tile representation of input data.
+
+    Parameters
+    ----------
+    tile : ``Tile``
+    kwargs : keyword arguments
+        driver specific parameters
+    """
+
+    preprocessing_tasks_results: dict
+    input_key: str
+    tile: BufferedTile
+
+    def __init__(self, tile: BufferedTile, input_key: str, **kwargs):
+        """Initialize."""
+        self.tile = tile
+        self.input_key = input_key
+        self.preprocessing_tasks_results = {}
+
+    def set_preprocessing_task_result(self, task_key: str, result: Any = None) -> None:
+        """
+        Adds a preprocessing task result.
+        """
+        self.preprocessing_tasks_results[task_key] = result
+
+    def __enter__(self):
+        """Required for 'with' statement."""
+        return self
+
+    def __exit__(self, t, v, tb):
+        """Clean up."""
+
+
+class InputData(InputDataProtocol):
     """
     Template class handling geographic input data.
 
     Parameters
     ----------
     input_params : dictionary
         driver specific parameters
@@ -49,72 +90,37 @@
         buffer around output tiles
     pyramid : ``tilematrix.TilePyramid``
         output ``TilePyramid``
     crs : ``rasterio.crs.CRS``
         object describing the process coordinate reference system
     """
 
+    input_key: str
+    pyramid: BufferedTilePyramid
+    pixelbuffer: int
+    crs: CRSLike
+    preprocessing_tasks: dict
+    preprocessing_tasks_results: dict
     METADATA = {"driver_name": None, "data_type": None, "mode": "r"}
 
-    def __init__(self, input_params, input_key=None, **kwargs):
+    def __init__(self, input_params: dict, input_key: Optional[str] = None, **kwargs):
         """Initialize relevant input information."""
-        self.input_key = input_key
+        self.input_key = input_key or get_hash(input_params)
         self.pyramid = input_params.get("pyramid")
         self.pixelbuffer = input_params.get("pixelbuffer")
         self.crs = self.pyramid.crs if self.pyramid else None
         # collect preprocessing tasks to be run by the Executor
         self.preprocessing_tasks = {}
         # storage location of all preprocessing tasks
         self.preprocessing_tasks_results = {}
         self.storage_options = input_params.get("abstract", {}).get(
             "storage_options", {}
         )
 
-    def open(self, tile, **kwargs):
-        """
-        Return InputTile object.
-
-        Parameters
-        ----------
-        tile : ``Tile``
-
-        Returns
-        -------
-        input tile : ``InputTile``
-            tile view of input data
-        """
-        raise NotImplementedError
-
-    def bbox(self, out_crs=None):
-        """
-        Return data bounding box.
-
-        Parameters
-        ----------
-        out_crs : ``rasterio.crs.CRS``
-            rasterio CRS object (default: CRS of process pyramid)
-
-        Returns
-        -------
-        bounding box : geometry
-            Shapely geometry object
-        """
-        raise NotImplementedError
-
-    def exists(self):
-        """
-        Check if data or file even exists.
-
-        Returns
-        -------
-        file exists : bool
-        """
-        raise NotImplementedError
-
-    def cleanup(self):
+    def cleanup(self) -> None:
         """Optional cleanup function called when Mapchete exits."""
 
     def add_preprocessing_task(
         self, func, fargs=None, fkwargs=None, key=None, geometry=None, bounds=None
     ):
         """
         Add longer running preprocessing function to be called right before processing.
@@ -177,70 +183,21 @@
         if self.input_key and not task_key.startswith(f"{self.input_key}:"):
             task_key = f"{self.input_key}:{task_key}"
         if task_key not in self.preprocessing_tasks:  # pragma: no cover
             raise KeyError(f"task {task_key} is not a task for current input")
         return task_key in self.preprocessing_tasks_results
 
 
-class InputTile(object):
-    """
-    Target Tile representation of input data.
-
-    Parameters
-    ----------
-    tile : ``Tile``
-    kwargs : keyword arguments
-        driver specific parameters
-    """
-
-    preprocessing_tasks_results = {}
-    input_key = None
-
-    def __init__(self, tile, **kwargs):
-        """Initialize."""
-
-    def read(self, **kwargs):
-        """
-        Read reprojected & resampled input data.
-
-        Returns
-        -------
-        data : array or list
-            NumPy array for raster data or feature list for vector data
-        """
-        raise NotImplementedError
-
-    def is_empty(self):
-        """
-        Check if there is data within this tile.
-
-        Returns
-        -------
-        is empty : bool
-        """
-        raise NotImplementedError
-
-    def set_preprocessing_task_result(self, task_key=None, result=None):
-        """
-        Adds a preprocessing task result.
-        """
-        self.preprocessing_tasks_results[task_key] = result
-
-    def __enter__(self):
-        """Required for 'with' statement."""
-        return self
-
-    def __exit__(self, t, v, tb):
-        """Clean up."""
-
-
-class OutputDataBaseFunctions:
+class OutputDataBase:
     write_in_parent_process = False
+    pixelbuffer: NonNegativeInt
+    pyramid: BufferedTilePyramid
+    crs: CRSLike
 
-    def __init__(self, output_params, readonly=False, **kwargs):
+    def __init__(self, output_params: dict, readonly: bool = False, **kwargs):
         """Initialize."""
         self.pixelbuffer = output_params["pixelbuffer"]
         if "type" in output_params:  # pragma: no cover
             warnings.warn(
                 DeprecationWarning("'type' is deprecated and should be 'grid'")
             )
             if "grid" not in output_params:
@@ -248,62 +205,17 @@
         self.pyramid = BufferedTilePyramid(
             grid=output_params["grid"],
             metatiling=output_params["metatiling"],
             pixelbuffer=output_params["pixelbuffer"],
         )
         self.crs = self.pyramid.crs
         self.storage_options = output_params.get("storage_options")
-        self.fs = self._fs = output_params.get(
-            "fs", fs_from_path(output_params.get("path", ""))
-        )
-        self.fs_kwargs = self._fs_kwargs = output_params.get("fs_kwargs") or {}
-        self.tile_path_schema = output_params.get(
-            "tile_path_schema", DEFAULT_TILE_PATH_SCHEMA
-        )
-
-    @property
-    def stac_path(self):
-        """Return path to STAC JSON file."""
-        return self.path.joinpath(f"{self.stac_item_id}.json")
-
-    @property
-    def stac_item_id(self):
-        """
-        Return STAC item ID according to configuration.
-
-        Defaults to path basename.
-        """
-        return self.output_params.get("stac", {}).get("id") or self.path.stem
-
-    @property
-    def stac_item_metadata(self):
-        """Custom STAC metadata."""
-        return self.output_params.get("stac", {})
-
-    @property
-    def stac_asset_type(self):  # pragma: no cover
-        """Asset MIME type."""
-        raise ValueError("no MIME type set for this output")
 
-    def is_valid_with_config(self, config):
-        """
-        Check if output format is valid with other process parameters.
-
-        Parameters
-        ----------
-        config : dictionary
-            output configuration parameters
-
-        Returns
-        -------
-        is_valid : bool
-        """
-        raise NotImplementedError()
-
-    def get_path(self, tile):
+    # TODO: move to path based output
+    def get_path(self, tile: BufferedTile) -> MPath:
         """
         Determine target file path.
 
         Parameters
         ----------
         tile : ``BufferedTile``
             must be member of output ``TilePyramid``
@@ -315,15 +227,18 @@
         return self.path / self.tile_path_schema.format(
             zoom=str(tile.zoom),
             row=str(tile.row),
             col=str(tile.col),
             extension=self.file_extension.lstrip("."),
         )
 
-    def extract_subset(self, input_data_tiles=None, out_tile=None):
+    # TODO: split up into vector and raster based output (mixin classes)
+    def extract_subset(
+        self, input_data_tiles: List[Tuple[BufferedTile, Any]], out_tile: BufferedTile
+    ) -> Any:
         """
         Extract subset from multiple tiles.
         input_data_tiles : list of (``Tile``, process data) tuples
         out_tile : ``Tile``
         Returns
         -------
         NumPy array or list of features.
@@ -348,31 +263,62 @@
                 if shape(feature["geometry"]).intersects(out_tile.bbox)
             ]
 
     def prepare(self, **kwargs):
         pass
 
 
-class OutputDataReader(OutputDataBaseFunctions):
-    def read(self, output_tile):
+class OutputSTACMixin:
+    """Adds STAC related features."""
+
+    path: MPath
+    output_params: dict
+
+    @property
+    def stac_path(self) -> MPath:
+        """Return path to STAC JSON file."""
+        return self.path / f"{self.stac_item_id}.json"
+
+    @property
+    def stac_item_id(self) -> str:
+        """
+        Return STAC item ID according to configuration.
+
+        Defaults to path basename.
+        """
+        return self.output_params.get("stac", {}).get("id") or self.path.stem
+
+    @property
+    def stac_item_metadata(self):
+        """Custom STAC metadata."""
+        return self.output_params.get("stac", {})
+
+    @property
+    def stac_asset_type(self):  # pragma: no cover
+        """Asset MIME type."""
+        raise ValueError("no MIME type set for this output")
+
+
+class OutputDataReader(OutputDataBase):
+    def read(self, output_tile):  # pragma: no cover
         """
         Read existing process output.
 
         Parameters
         ----------
         output_tile : ``BufferedTile``
             must be member of output ``TilePyramid``
 
         Returns
         -------
         process output : array or list
         """
         raise NotImplementedError()
 
-    def empty(self, process_tile):
+    def empty(self, process_tile):  # pragma: no cover
         """
         Return empty data.
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
             must be member of process ``TilePyramid``
@@ -381,26 +327,26 @@
         -------
         empty data : array or list
             empty array with correct data type for raster data or empty list
             for vector data
         """
         raise NotImplementedError()
 
-    def open(self, tile, process):
+    def open(self, tile, process):  # pragma: no cover
         """
         Open process output as input for other process.
 
         Parameters
         ----------
         tile : ``Tile``
         process : ``MapcheteProcess``
         """
         raise NotImplementedError
 
-    def for_web(self, data):
+    def for_web(self, data):  # pragma: no cover
         """
         Convert data to web output (raster only).
 
         Parameters
         ----------
         data : array
 
@@ -429,15 +375,15 @@
     crs : ``rasterio.crs.CRS``
         object describing the process coordinate reference system
     """
 
     METADATA = {"driver_name": None, "data_type": None, "mode": "w"}
     use_stac = False
 
-    def write(self, process_tile, data):
+    def write(self, process_tile, data):  # pragma: no cover
         """
         Write data from one or more process tiles.
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
             must be member of process ``TilePyramid``
@@ -512,18 +458,23 @@
                 "invalid output type: %s" % type(process_data)
             )
 
     def close(self, exc_type=None, exc_value=None, exc_traceback=None):
         """Gets called if process is closed."""
 
 
-class TileDirectoryOutputReader(OutputDataReader):
+class TileDirectoryOutputReader(OutputDataReader, OutputSTACMixin):
+    tile_path_schema: str = DEFAULT_TILE_PATH_SCHEMA
+
     def __init__(self, output_params, readonly=False):
         """Initialize."""
         super().__init__(output_params, readonly=readonly)
+        self.tile_path_schema = output_params.get(
+            "tile_path_schema", DEFAULT_TILE_PATH_SCHEMA
+        )
         if not readonly:
             write_output_metadata(
                 {k: v for k, v in output_params.items() if k not in ["stac"]}
             )
 
     def tiles_exist(self, process_tile=None, output_tile=None):
         """
@@ -539,20 +490,21 @@
         Returns
         -------
         exists : bool
         """
         if process_tile and output_tile:  # pragma: no cover
             raise ValueError("just one of 'process_tile' and 'output_tile' allowed")
         if process_tile:
-            return any(
-                path_exists(self.get_path(tile), fs=self._fs)
-                for tile in self.pyramid.intersecting(process_tile)
-            )
+            for tile in self.pyramid.intersecting(process_tile):
+                if self.get_path(tile).exists():
+                    return True
+            else:
+                return False
         if output_tile:
-            return path_exists(self.get_path(output_tile), fs=self._fs)
+            return self.get_path(output_tile).exists()
 
     def _read_as_tiledir(
         self,
         out_tile=None,
         td_crs=None,
         tiles_paths=None,
         profile=None,
@@ -598,20 +550,20 @@
         )
 
 
 class TileDirectoryOutputWriter(OutputDataWriter, TileDirectoryOutputReader):
     pass
 
 
-class SingleFileOutputReader(OutputDataReader):
+class SingleFileOutputReader(OutputDataReader, OutputSTACMixin):
     def __init__(self, output_params, readonly=False):
         """Initialize."""
         super().__init__(output_params, readonly=readonly)
 
-    def tiles_exist(self, process_tile=None, output_tile=None):
+    def tiles_exist(self, process_tile=None, output_tile=None):  # pragma: no cover
         """
         Check whether output tiles of a tile (either process or output) exists.
 
         Parameters
         ----------
         process_tile : ``BufferedTile``
             must be member of process ``TilePyramid``
@@ -619,23 +571,23 @@
             must be member of output ``TilePyramid``
 
         Returns
         -------
         exists : bool
         """
         # TODO
-        raise NotImplementedError  # pragma: no cover
+        raise NotImplementedError
 
 
 class SingleFileOutputWriter(OutputDataWriter, SingleFileOutputReader):
     pass
 
 
 def is_numpy_or_masked_array(data):
-    return isinstance(data, (np.ndarray, ma.core.MaskedArray))
+    return isinstance(data, (np.ndarray, ma.MaskedArray))
 
 
 def is_numpy_or_masked_array_with_tags(data):
     return (
         isinstance(data, tuple)
         and len(data) == 2
         and is_numpy_or_masked_array(data[0])
```

### Comparing `mapchete-2024.5.0/mapchete/formats/loaders.py` & `mapchete-2024.5.1/mapchete/formats/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import logging
-from typing import Dict, Optional
+from typing import Optional
 
 from mapchete.errors import MapcheteDriverError
+from mapchete.formats.protocols import (
+    InputDataProtocol,
+    OutputDataReaderProtocol,
+    OutputDataWriterProtocol,
+)
 from mapchete.formats.tools import driver_from_file
 from mapchete.registered import drivers
 
 logger = logging.getLogger(__name__)
 
 
-def load_output_reader(output_params: Dict) -> "OutputDataReader":
+def load_output_reader(output_params: dict) -> OutputDataReaderProtocol:
     """
     Return OutputReader class of driver.
 
     Parameters
     ----------
     output_params : dict
         Output parameters as given in mapchete configuration.
@@ -31,16 +36,16 @@
             [hasattr(_driver, attr) for attr in ["OutputDataReader", "METADATA"]]
         ) and (_driver.METADATA["driver_name"] == driver_name):
             return _driver.OutputDataReader(output_params, readonly=True)
     raise MapcheteDriverError("no loader for driver '%s' could be found." % driver_name)
 
 
 def load_output_writer(
-    output_params: Dict, readonly: bool = False
-) -> "OutputDataWriter":
+    output_params: dict, readonly: bool = False
+) -> OutputDataWriterProtocol:
     """
     Return output class of driver.
 
     Parameters
     ----------
     output_params : dict
         Output parameters as given in mapchete configuration.
@@ -61,16 +66,16 @@
             [hasattr(_driver, attr) for attr in ["OutputDataWriter", "METADATA"]]
         ) and (_driver.METADATA["driver_name"] == driver_name):
             return _driver.OutputDataWriter(output_params, readonly=readonly)
     raise MapcheteDriverError("no loader for driver '%s' could be found." % driver_name)
 
 
 def load_input_reader(
-    input_params: Dict, readonly: bool = False, input_key: Optional[str] = None
-) -> "InputData":
+    input_params: dict, readonly: bool = False, input_key: Optional[str] = None
+) -> InputDataProtocol:
     """
     Return input class of driver.
 
     Parameters
     ----------
     input_params : dict
         Input parameters as given in mapchete configuration.
```

### Comparing `mapchete-2024.5.0/mapchete/formats/tools.py` & `mapchete-2024.5.1/mapchete/formats/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Dict
 
 import dateutil.parser
 from rasterio.crs import CRS
 from shapely.geometry.base import BaseGeometry
 
 from mapchete.errors import MapcheteConfigError, MapcheteDriverError
-from mapchete.formats.models import DriverMetadata
 from mapchete.io import MPath, fiona_open, rasterio_open
 from mapchete.registered import drivers
 from mapchete.tile import BufferedTilePyramid
 from mapchete.types import MPathLike
 
 logger = logging.getLogger(__name__)
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/_fiona_base.py` & `mapchete-2024.5.1/mapchete/formats/default/_fiona_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Baseclasses for all drivers using fiona for reading and writing data.
 """
 
 import logging
 import types
 
 from mapchete.formats import base
+from mapchete.formats.protocols import VectorInput
 from mapchete.io import MPath, fiona_open
 from mapchete.io.vector import write_vector_window
 from mapchete.tile import BufferedTile
 from mapchete.validate import validate_values
 
 logger = logging.getLogger(__name__)
 
@@ -164,15 +165,15 @@
                     out_path=out_path,
                     allow_multipart_geometries=(
                         self.output_params["schema"]["geometry"].startswith("Multi")
                     ),
                 )
 
 
-class InputTile(base.InputTile):
+class InputTile(base.InputTile, VectorInput):
     """
     Target Tile representation of input data.
 
     Parameters
     ----------
     tile : ``Tile``
     process : ``MapcheteProcess``
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/flatgeobuf.py` & `mapchete-2024.5.1/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/default/geobuf.py` & `mapchete-2024.5.1/mapchete/processing/mp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,170 @@
-"""
-Handles writing process output into a pyramid of Geobuf files.
+import numpy.ma as ma
 
-output configuration parameters
--------------------------------
+from mapchete.formats.protocols import InputTileProtocol
+from mapchete.validate import deprecated_kwargs
 
-output type has to be ``geodetic``
 
-mandatory
-~~~~~~~~~
-
-path: string
-    output directory
-schema: key-value pairs
-    the schema is passed on to fiona
-    - properties: key-value pairs (fields and field types, like "id: int" etc.)
-    - geometry: output geometry type (Geometry, Point, MultiPoint, Line, MultiLine,
-    Polygon, MultiPolygon)
-"""
-
-import logging
-
-from shapely.geometry import mapping, shape
-
-from mapchete.formats.default import geojson
-from mapchete.io import MPath, fs_from_path
-from mapchete.io._geometry_operations import _repair, reproject_geometry
-from mapchete.validate import validate_values
-
-logger = logging.getLogger(__name__)
-METADATA = {"driver_name": "Geobuf", "data_type": "vector", "mode": "rw"}
-
-
-class OutputDataReader(geojson.OutputDataReader):
+class MapcheteProcess(object):
     """
-    Output reader class for Geobuf Tile Directory.
+    Process class inherited by user process script.
+
+    Its attributes and methods can be accessed via "self" from within a
+    Mapchete process Python file.
 
     Parameters
     ----------
-    output_params : dictionary
-        output parameters from Mapchete file
+    tile : BufferedTile
+        Tile process should be run on
+    config : MapcheteConfig
+        process configuration
+    params : dictionary
+        process parameters
 
     Attributes
     ----------
-    path : string
-        path to output directory
-    file_extension : string
-        file extension for output files (.geobuf)
-    output_params : dictionary
-        output parameters from Mapchete file
-    pixelbuffer : integer
-        buffer around output tiles
-    pyramid : ``tilematrix.TilePyramid``
-        output ``TilePyramid``
-    crs : ``rasterio.crs.CRS``
-        object describing the process coordinate reference system
-    srid : string
-        spatial reference ID of CRS (e.g. "{'init': 'epsg:4326'}")
-    """
+    identifier : string
+        process identifier
+    title : string
+        process title
+    version : string
+        process version string
+    abstract : string
+        short text describing process purpose
+    tile : BufferedTile
+        Tile process should be run on
+    tile_pyramid : BufferedTilePyramid
+        process tile pyramid
+    output_pyramid : BufferedTilePyramid
+        output tile pyramid
+    params : dictionary
+        process parameters
+    """
+
+    def __init__(
+        self, tile=None, params=None, input=None, output_params=None, config=None
+    ):
+        """Initialize Mapchete process."""
+        self.identifier = ""
+        self.title = ""
+        self.version = ""
+        self.abstract = ""
+
+        self.tile = tile
+        self.tile_pyramid = tile.tile_pyramid
+        if config is not None:
+            input = config.get_inputs_for_tile(tile)
+            params = config.params_at_zoom(tile.zoom)
+        self.params = dict(params, input=input)
+        self.input = input
+        self.output_params = output_params
 
-    METADATA = METADATA
+    def write(self, data, **kwargs):
+        """Deprecated."""
+        raise DeprecationWarning(
+            "Please return process output data instead of using self.write()."
+        )
 
-    def __init__(self, output_params, **kwargs):
-        """Initialize."""
-        super().__init__(output_params)
-        self.path = output_params["path"]
-        self.file_extension = ".pbf"
-        self.output_params = output_params
-        self._bucket = None
+    def read(self, **kwargs):
+        """
+        Read existing output data from a previous run.
+
+        Returns
+        -------
+        process output : NumPy array (raster) or feature iterator (vector)
+        """
+        raise DeprecationWarning(
+            "Read existing output from within a process is deprecated"
+        )
 
-    def read(self, output_tile, **kwargs):
+    @deprecated_kwargs
+    def open(self, input_id, **kwargs) -> InputTileProtocol:
         """
-        Read existing process output.
+        Open input data.
 
         Parameters
         ----------
-        output_tile : ``BufferedTile``
-            must be member of output ``TilePyramid``
+        input_id : string
+            input identifier from configuration file or file path
+        kwargs : driver specific parameters (e.g. resampling)
 
         Returns
         -------
-        process output : list
+        tiled input data : InputTile
+            reprojected input data within tile
         """
-        import geobuf
-
-        path = self.get_path(output_tile)
-        try:
-            with fs_from_path(path).open(path, "rb") as src:
-                return geobuf.decode(src.read()).get("features", [])
-        except FileNotFoundError:
-            return self.empty(output_tile)
+        if input_id not in self.input:
+            raise ValueError("%s not found in config as input" % input_id)
+        return self.input[input_id]
 
-    def is_valid_with_config(self, config):
+    def hillshade(self, *_, **__) -> ma.MaskedArray:  # pragma: no cover
         """
-        Check if output format is valid with other process parameters.
+        Calculate hillshading from elevation data.
 
         Parameters
         ----------
-        config : dictionary
-            output configuration parameters
+        elevation : array
+            input elevation data
+        azimuth : float
+            horizontal angle of light source (315: North-West)
+        altitude : float
+            vertical angle of light source (90 would result in slope shading)
+        z : float
+            vertical exaggeration factor
+        scale : float
+            scale factor of pixel size units versus height units (insert 112000
+            when having elevation values in meters in a geodetic projection)
 
         Returns
         -------
-        is_valid : bool
+        hillshade : array
         """
-        validate_values(config, [("schema", dict), ("path", (str, MPath))])
-        validate_values(config["schema"], [("properties", dict), ("geometry", str)])
-        if config["schema"]["geometry"] not in [
-            "Geometry",
-            "Point",
-            "MultiPoint",
-            "Line",
-            "MultiLine",
-            "Polygon",
-            "MultiPolygon",
-        ]:  # pragma: no cover
-            raise TypeError("invalid geometry type")
-        return True
+        raise DeprecationWarning(
+            "Run hillshade via mp is deprecated. Call the hillshade method from mapchete.processes.hillshade."
+        )
 
-    def for_web(self, data):
+    def contours(self, *_, **__) -> ma.MaskedArray:  # pragma: no cover
         """
-        Convert data to web output (raster only).
+        Extract contour lines from elevation data.
 
         Parameters
         ----------
-        data : array
+        elevation : array
+            input elevation data
+        interval : integer
+            elevation value interval when drawing contour lines
+        field : string
+            output field name containing elevation value
+        base : integer
+            elevation base value the intervals are computed from
 
         Returns
         -------
-        web data : array
+        contours : iterable
+            contours as GeoJSON-like pairs of properties and geometry
         """
-        import geobuf
-
-        return (
-            geobuf.encode(
-                dict(
-                    type="FeatureCollection",
-                    features=[
-                        dict(
-                            f,
-                            geometry=mapping(_repair(shape(f["geometry"]))),
-                            type="Feature",
-                        )
-                        for f in data
-                    ],
-                )
-            ),
-            "application/octet-stream",
+        raise DeprecationWarning(
+            "MapcheteProcess.contours() is deprecated. Call the contours method from mapchete.processes.contours."
         )
 
-    def _read_as_tiledir(self, out_tile=None, tiles_paths=None, **kwargs):
-        return [
-            dict(
-                feature,
-                geometry=mapping(
-                    reproject_geometry(
-                        shape(feature["geometry"]),
-                        src_crs=tile.crs,
-                        dst_crs=out_tile.crs,
-                    ).intersection(out_tile.bbox)
-                ),
-            )
-            for tile, _ in tiles_paths
-            for feature in self.read(tile)
-        ]  # pragma: no cover
-        # --> this part is covered by the CLI tests but somehow gets omitted
-
-
-class OutputDataWriter(geojson.OutputDataWriter, OutputDataReader):
-    """
-    Output writer class.
-    """
-
-    METADATA = METADATA
-
-
-class InputTile(geojson.InputTile):
-    """
-    Target Tile representation of input data.
+    def clip(self, *_, **__) -> ma.MaskedArray:  # pragma: no cover
+        """
+        Clip array by geometry.
 
-    Parameters
-    ----------
-    tile : ``Tile``
-    process : ``MapcheteProcess``
+        Parameters
+        ----------
+        array : array
+            raster data to be clipped
+        geometries : iterable
+            geometries used to clip source array
+        inverted : bool
+            invert clipping (default: False)
+        clip_buffer : int
+            buffer (in pixels) geometries before applying clip
 
-    Attributes
-    ----------
-    tile : ``Tile``
-    process : ``MapcheteProcess``
-    """
+        Returns
+        -------
+        clipped array : array
+        """
+        raise DeprecationWarning(
+            "MapcheteProcess.clip() is deprecated. Call the clip method from mapchete.io.raster.array.clip_array_with_vector()."
+        )
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/geojson.py` & `mapchete-2024.5.1/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/default/gtiff.py` & `mapchete-2024.5.1/mapchete/formats/default/gtiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     internal tile height (default: 256)
 nodata: integer or float
     nodata value used for writing
 compress: string
     compression method (default: lzw): lzw, jpeg, packbits, deflate, CCITTRLE,
     CCITTFAX3, CCITTFAX4, lzma
 """
+from __future__ import annotations
 
 import logging
 import math
 import os
 import warnings
 from contextlib import ExitStack
 
@@ -44,14 +45,15 @@
 from rasterio.windows import from_bounds
 from shapely.geometry import box
 from tilematrix import Bounds
 
 from mapchete.config.base import _OUTPUT_PARAMETERS, snap_bounds
 from mapchete.errors import MapcheteConfigError
 from mapchete.formats import base
+from mapchete.formats.protocols import RasterInput
 from mapchete.io import MPath, path_exists, path_is_remote
 from mapchete.io.profiles import DEFAULT_PROFILES
 from mapchete.io.raster import (
     extract_from_array,
     memory_file,
     prepare_array,
     rasterio_write,
@@ -193,15 +195,15 @@
                 ),
                 self.profile(),
             ),
             "image/tiff",
         )
 
     @deprecated_kwargs
-    def open(self, tile, process, **kwargs):
+    def open(self, tile, process, **kwargs) -> InputTile:
         """
         Open process output as input for other process.
 
         Parameters
         ----------
         tile : ``Tile``
         process : ``MapcheteProcess``
@@ -369,15 +371,14 @@
                 write_raster_window(
                     in_grid=process_tile,
                     in_data=data,
                     out_profile=self.profile(out_tile),
                     out_grid=out_tile,
                     out_path=out_path,
                     tags=tags,
-                    fs=self.fs,
                 )
 
     @property
     def stac_asset_type(self):
         """GeoTIFF media type."""
         return "image/tiff; application=geotiff"
 
@@ -645,15 +646,15 @@
             window.col_off >= 0,
             window.row_off + window.height <= rio_file.height,
             window.col_off + window.width <= rio_file.width,
         ]
     )
 
 
-class InputTile(base.InputTile):
+class InputTile(base.InputTile, RasterInput):
     """
     Target Tile representation of input data.
 
     Parameters
     ----------
     tile : ``Tile``
     process : ``MapcheteProcess``
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/mapchete_input.py` & `mapchete-2024.5.1/mapchete/formats/default/mapchete_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Use another Mapchete process as input."""
 
 from mapchete import Mapchete
 from mapchete.config import MapcheteConfig
 from mapchete.formats import base
+from mapchete.formats.protocols import InputTileProtocol
 from mapchete.io.vector import reproject_geometry
 
 METADATA = {
     "driver_name": "Mapchete",
     "data_type": None,
     "mode": "r",
     "file_extensions": ["mapchete"],
@@ -45,15 +46,15 @@
 
     def __init__(self, input_params, **kwargs):
         """Initialize."""
         super().__init__(input_params, **kwargs)
         self.path = input_params["path"]
         self.process = Mapchete(MapcheteConfig(self.path, mode="readonly"))
 
-    def open(self, tile, **kwargs):
+    def open(self, tile, **kwargs) -> InputTileProtocol:
         """
         Return InputTile object.
 
         Parameters
         ----------
         tile : ``Tile``
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/png.py` & `mapchete-2024.5.1/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/default/png_hillshade.py` & `mapchete-2024.5.1/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/formats/default/raster_file.py` & `mapchete-2024.5.1/mapchete/formats/default/raster_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import numpy.ma as ma
 from rasterio.crs import CRS
 from rasterio.vrt import WarpedVRT
 from shapely.geometry import box
 
 from mapchete import io
 from mapchete.formats import base
+from mapchete.formats.protocols import RasterInput
 from mapchete.io.raster import (
     convert_raster,
     rasterio_open,
     read_raster,
     read_raster_window,
     resample_from_array,
 )
@@ -212,15 +213,15 @@
     def cleanup(self):
         """Cleanup when mapchete closes."""
         if self._cached_path and not self._cache_keep:  # pragma: no cover
             logger.debug("remove cached file %s", self._cached_path)
             self._cached_path.rm(ignore_errors=True)
 
 
-class InputTile(base.InputTile):
+class InputTile(base.InputTile, RasterInput):
     """
     Target Tile representation of input data.
 
     Parameters
     ----------
     tile : ``Tile``
     kwargs : keyword arguments
@@ -238,19 +239,18 @@
     _memory_cache_active = False
     _in_memory_raster = None
 
     def __init__(
         self, tile, input_data, in_memory_raster=None, cache_task_key=None, **kwargs
     ):
         """Initialize."""
-        self.tile = tile
+        super().__init__(tile, input_key=input_data.input_key, **kwargs)
         self.bbox = input_data.bbox(out_crs=self.tile.crs)
         self.profile = input_data.profile
         self.cache_task_key = cache_task_key
-        self.input_key = input_data.input_key
         if input_data._memory_cache_active:
             self._memory_cache_active = True
             self._in_memory_raster = in_memory_raster
         else:
             self.path = input_data._cached_path or input_data.path
             self.gdal_opts = {}
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/tile_directory.py` & `mapchete-2024.5.1/mapchete/formats/default/tile_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from mapchete.formats import (
     base,
     data_type_from_extension,
     driver_metadata,
     load_output_writer,
     read_output_metadata,
 )
+from mapchete.formats.protocols import RasterInput
 from mapchete.io import MPath, tile_to_zoom_level
 from mapchete.io.vector import reproject_geometry
 from mapchete.tile import BufferedTilePyramid
 from mapchete.validate import validate_values
 
 logger = logging.getLogger(__name__)
 METADATA = {
@@ -48,15 +49,15 @@
         object describing the process coordinate reference system
     srid : string
         spatial reference ID of CRS (e.g. "{'init': 'epsg:4326'}")
     """
 
     METADATA = METADATA
 
-    def __init__(self, input_params, **kwargs):
+    def __init__(self, input_params: dict, **kwargs):
         """Initialize."""
         super().__init__(input_params, **kwargs)
         self._read_as_tiledir_func = None
         logger.debug("InputData params: %s", input_params)
         # populate internal parameters initially depending on whether this input was
         # defined as simple or abstract input
         self._params = input_params.get("abstract") or dict(path=input_params["path"])
@@ -223,15 +224,15 @@
             (t, basepath.joinpath(str(t.zoom), str(t.row), str(t.col)).with_suffix(ext))
             for t in pyramid.tiles_from_bounds(bounds, zoom)
         ]
         if not exists_check or (exists_check and _path.exists())
     ]
 
 
-class InputTile(base.InputTile):
+class InputTile(base.InputTile, RasterInput):
     """
     Target Tile representation of input data.
 
     Parameters
     ----------
     tile : ``Tile``
     kwargs : keyword arguments
```

### Comparing `mapchete-2024.5.0/mapchete/formats/default/vector_file.py` & `mapchete-2024.5.1/mapchete/formats/default/vector_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 from functools import cached_property
 
 from rasterio.crs import CRS
 from shapely.geometry import Point, box
 
 from mapchete.formats import base
+from mapchete.formats.protocols import VectorInput
 from mapchete.io import fiona_open
 from mapchete.io.vector import (
     IndexedFeatures,
     convert_vector,
     read_vector,
     read_vector_window,
     reproject_geometry,
@@ -192,15 +193,15 @@
     def cleanup(self):
         """Cleanup when mapchete closes."""
         if self._cached_path and not self._cache_keep:  # pragma: no cover
             logger.debug("remove cached file %s", self._cached_path)
             self._cached_path.rm(ignore_errors=True)
 
 
-class InputTile(base.InputTile):
+class InputTile(base.InputTile, VectorInput):
     """
     Target Tile representation of input data.
 
     Parameters
     ----------
     tile : ``Tile``
     kwargs : keyword arguments
@@ -216,19 +217,18 @@
     _memory_cache_active = False
     _in_memory_features = None
 
     def __init__(
         self, tile, input_data, in_memory_features=None, cache_task_key=None, **kwargs
     ):
         """Initialize."""
-        self.tile = tile
+        super().__init__(tile, input_key=input_data.input_key, **kwargs)
         self._cache = {}
         self.bbox = input_data.bbox(out_crs=self.tile.crs)
         self.cache_task_key = cache_task_key
-        self.input_key = input_data.input_key
         if input_data._memory_cache_active:
             self._memory_cache_active = True
             self._in_memory_features = in_memory_features
         else:
             self.path = input_data._cached_path or input_data.path
 
     def __repr__(self):  # pragma: no cover
```

### Comparing `mapchete-2024.5.0/mapchete/io/__init__.py` & `mapchete-2024.5.1/mapchete/io/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions for reading and writing data."""
 
 from mapchete.io._json import read_json, write_json
 from mapchete.io._misc import (
+    MatchingMethod,
     copy,
     get_best_zoom_level,
     get_boto3_bucket,
     get_segmentize_value,
     tile_to_zoom_level,
 )
 from mapchete.io.raster import rasterio_open
@@ -25,14 +26,15 @@
 __all__ = [
     "copy",
     "fs_from_path",
     "GDALHTTPOptions",
     "get_best_zoom_level",
     "get_segmentize_value",
     "tile_to_zoom_level",
+    "MatchingMethod",
     "path_is_remote",
     "path_exists",
     "tiles_exist",
     "absolute_path",
     "relative_path",
     "makedirs",
     "Path",
```

### Comparing `mapchete-2024.5.0/mapchete/io/_geometry_operations.py` & `mapchete-2024.5.1/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/io/_misc.py` & `mapchete-2024.5.1/mapchete/io/_misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
+from enum import Enum
 
 import rasterio
 from rasterio.warp import calculate_default_transform
 from shapely.errors import TopologicalError
 from shapely.geometry import box
 
 from mapchete.io._geometry_operations import reproject_geometry, segmentize_geometry
 from mapchete.path import MPath
-from mapchete.tile import BufferedTilePyramid
+from mapchete.tile import BufferedTile, BufferedTilePyramid
 
 logger = logging.getLogger(__name__)
 
 
 def get_best_zoom_level(input_file, tile_pyramid_type):
     """
     Determine the best base zoom level for a raster.
@@ -71,23 +72,33 @@
         length suggested of line segmentation to reproject file bounds
     """
     with rasterio.open(input_file, "r") as input_raster:
         pixelsize = input_raster.transform[0]
     return pixelsize * tile_pyramid.tile_size
 
 
-def tile_to_zoom_level(tile, dst_pyramid=None, matching_method="gdal", precision=8):
+class MatchingMethod(str, Enum):
+    gdal = "gdal"
+    min = "min"
+
+
+def tile_to_zoom_level(
+    tile: BufferedTile,
+    dst_pyramid: BufferedTilePyramid,
+    matching_method: MatchingMethod = MatchingMethod.gdal,
+    precision: int = 8,
+):
     """
     Determine the best zoom level in target TilePyramid from given Tile.
 
     Parameters
     ----------
     tile : BufferedTile
     dst_pyramid : BufferedTilePyramid
-    matching_method : str ('gdal' or 'min')
+    matching_method : MatchingMethod ('gdal' or 'min')
         gdal: Uses GDAL's standard method. Here, the target resolution is calculated by
             averaging the extent's pixel sizes over both x and y axes. This approach
             returns a zoom level which may not have the best quality but will speed up
             reading significantly.
         min: Returns the zoom level which matches the minimum resolution of the extent's
             four corner pixels. This approach returns the zoom level with the best
             possible quality but with low performance. If the tile extent is outside of
@@ -116,25 +127,25 @@
         except ValueError:  # pragma: no cover
             raise TopologicalError("bounds cannot be translated into target CRS")
         return r - l, t - b
 
     if tile.tp.crs == dst_pyramid.crs:
         return tile.zoom
     else:
-        if matching_method == "gdal":
+        if matching_method == MatchingMethod.gdal:
             # use rasterio/GDAL method to calculate default warp target properties
             # enabling CHECK_WITH_INVERT_PROJ fixes #269, otherwise this function would
             # return a non-optimal zoom level for reprojection
             with rasterio.Env(CHECK_WITH_INVERT_PROJ=True):
                 transform, width, height = calculate_default_transform(
                     tile.tp.crs, dst_pyramid.crs, tile.width, tile.height, *tile.bounds
                 )
                 # this is the resolution the tile would have in destination CRS
                 tile_resolution = round(transform[0], precision)
-        elif matching_method == "min":
+        elif matching_method == MatchingMethod.min:
             # calculate the minimum pixel size from the four tile corner pixels
             l, b, r, t = tile.bounds
             x = tile.pixel_x_size
             y = tile.pixel_y_size
             res = []
             for bounds in [
                 (l, t - y, l + x, t),  # left top
```

### Comparing `mapchete-2024.5.0/mapchete/io/profiles.py` & `mapchete-2024.5.1/mapchete/io/profiles.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/io/vector.py` & `mapchete-2024.5.1/mapchete/io/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 from contextlib import ExitStack, contextmanager
 from itertools import chain
 from tempfile import NamedTemporaryFile
 from typing import Any, Union
 
 import fiona
-from fiona.errors import DriverError, FionaError, FionaValueError
+from fiona.errors import DriverError
 from fiona.io import MemoryFile
 from rasterio.crs import CRS
 from retry import retry
 from shapely.errors import TopologicalError
 from shapely.geometry import base, box, mapping, shape
 from tilematrix import clip_geometry_to_srs_bounds
 
@@ -22,15 +22,15 @@
     _repair,
     clean_geometry_type,
     multipart_to_singleparts,
     reproject_geometry,
     segmentize_geometry,
     to_shape,
 )
-from mapchete.path import MPath, fs_from_path, path_exists
+from mapchete.path import MPath, fs_from_path
 from mapchete.settings import IORetrySettings
 from mapchete.types import Bounds
 from mapchete.validate import validate_bounds
 
 __all__ = [
     "reproject_geometry",
     "segmentize_geometry",
@@ -217,17 +217,14 @@
     out_path=None,
     allow_multipart_geometries=True,
     **kwargs,
 ):
     """
     Write features to file.
 
-    When the output driver is 'Geobuf', the geobuf library will be used otherwise the
-    driver will be passed on to Fiona.
-
     Parameters
     ----------
     in_data : features
     out_driver : string
     out_schema : dictionary
         output schema for fiona
     out_tile : ``BufferedTile``
@@ -260,82 +257,31 @@
         except Exception as e:
             logger.warning("failed to prepare geometry for writing: %s", e)
             continue
 
     # write if there are output features
     if out_features:
         try:
-            if out_driver.lower() in ["geobuf"]:
-                # write data to remote file
-                with VectorWindowMemoryFile(
-                    tile=out_tile,
-                    features=out_features,
-                    schema=out_schema,
-                    driver=out_driver,
-                ) as memfile:
-                    logger.debug((out_tile.id, "write tile", out_path))
-                    with out_path.open("wb") as dst:
-                        dst.write(memfile)
-            else:  # pragma: no cover
-                with fiona_open(
-                    out_path,
-                    "w",
-                    schema=out_schema,
-                    driver=out_driver,
-                    crs=out_tile.crs.to_dict(),
-                ) as dst:
-                    logger.debug((out_tile.id, "write tile", out_path))
-                    dst.writerecords(out_features)
+            with fiona_open(
+                out_path,
+                "w",
+                schema=out_schema,
+                driver=out_driver,
+                crs=out_tile.crs.to_dict(),
+            ) as dst:
+                logger.debug((out_tile.id, "write tile", out_path))
+                dst.writerecords(out_features)
         except Exception as e:
             logger.error("error while writing file %s: %s", out_path, e)
             raise
 
     else:
         logger.debug((out_tile.id, "nothing to write", out_path))
 
 
-class VectorWindowMemoryFile:
-    """Context manager around fiona.io.MemoryFile."""
-
-    def __init__(self, tile=None, features=None, schema=None, driver=None):
-        """Prepare data & profile."""
-        self.tile = tile
-        self.schema = schema
-        self.driver = driver
-        self.features = features
-
-    def __enter__(self):
-        """Open MemoryFile, write data and return."""
-        if self.driver.lower() == "geobuf":
-            import geobuf
-
-            return geobuf.encode(
-                dict(
-                    type="FeatureCollection",
-                    features=[dict(f, type="Feature") for f in self.features],
-                )
-            )
-        else:  # pragma: no cover
-            # this part is excluded now for tests as we try to let fiona write directly
-            # to S3
-            self.fio_memfile = MemoryFile()
-            with self.fio_memfile.open(
-                schema=self.schema, driver=self.driver, crs=self.tile.crs
-            ) as dst:
-                dst.writerecords(self.features)
-            return self.fio_memfile.getbuffer()
-
-    def __exit__(self, *args):
-        """Make sure MemoryFile is closed."""
-        try:
-            self.fio_memfile.close()
-        except AttributeError:
-            pass
-
-
 @retry(
     logger=logger,
     **dict(IORetrySettings()),
 )
 def _get_reprojected_features(
     inp=None,
     dst_bounds=None,
```

### Comparing `mapchete-2024.5.0/mapchete/io/raster/__init__.py` & `mapchete-2024.5.1/mapchete/io/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/io/raster/array.py` & `mapchete-2024.5.1/mapchete/io/raster/array.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import itertools
 import logging
 import warnings
-from typing import Iterable, Optional, Tuple, Union
+from typing import Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.ma as ma
 from affine import Affine
 from numpy.typing import DTypeLike
 from rasterio.enums import Resampling
+from rasterio.features import geometry_mask
 from rasterio.warp import reproject
 from rasterio.windows import from_bounds
+from shapely.ops import unary_union
 
+from mapchete.io.vector import to_shape
 from mapchete.protocols import GridProtocol
-from mapchete.types import BoundsLike, CRSLike, NodataVal
+from mapchete.types import BoundsLike, CRSLike, Grid, NodataVal
 
 logger = logging.getLogger(__name__)
 
 
 def extract_from_array(
     array: Union[np.ndarray, ma.MaskedArray, GridProtocol],
     array_transform: Optional[Affine] = None,
@@ -43,44 +46,48 @@
             )
         )
         array_transform = array_transform or in_affine
 
     if out_grid is None:  # pragma: no cover
         raise ValueError("grid must be defined")
 
-    if hasattr(array, "affine") and hasattr(array, "data"):  # pragma: no cover
-        array_transform, array = array.affine, array.data
-    elif hasattr(array, "transform") and hasattr(array, "data"):  # pragma: no cover
-        array_transform, array = array.transform, array.data
-    elif array_transform is None:  # pragma: no cover
-        raise ValueError("an Affine object is required")
+    from mapchete.io.raster.referenced_raster import ReferencedRaster
+
+    raster = ReferencedRaster.from_array_like(
+        array, transform=array_transform, crs=out_grid.crs
+    )
+
+    if raster.crs != out_grid.crs:  # pragma: no cover
+        raise ValueError(
+            f"source CRS {raster.crs} and destination CRS {out_grid.crs} do not match!"
+        )
 
     # get range within array
     minrow, maxrow, mincol, maxcol = bounds_to_ranges(
-        bounds=out_grid.bounds, transform=array_transform
+        bounds=out_grid.bounds, transform=raster.transform
     )
     # if output window is within input window
     if (
         minrow >= 0
         and mincol >= 0
         and maxrow <= array.shape[-2]
         and maxcol <= array.shape[-1]
     ):
-        return array[..., minrow:maxrow, mincol:maxcol]
+        return raster.array[..., minrow:maxrow, mincol:maxcol]
     # raise error if output is not fully within input
     else:
         raise ValueError("extraction fails if output shape is not within input")
 
 
 def resample_from_array(
     array: Union[np.ndarray, ma.MaskedArray, GridProtocol],
     array_transform: Optional[Affine] = None,
-    out_grid: Optional[GridProtocol] = None,
+    out_grid: Optional[Union[Grid, GridProtocol]] = None,
     in_affine: Optional[Affine] = None,
-    out_tile: Optional[GridProtocol] = None,
+    out_tile: Optional[Union[Grid, GridProtocol]] = None,
     in_crs: Optional[CRSLike] = None,
     resampling: Union[Resampling, str] = Resampling.nearest,
     nodataval: Optional[NodataVal] = None,
     nodata: Optional[NodataVal] = 0,
     keep_2d: bool = False,
 ) -> ma.MaskedArray:
     """
@@ -114,29 +121,31 @@
         nodata = nodata or nodataval
 
     if isinstance(array, ma.MaskedArray):
         pass
     elif isinstance(array, np.ndarray):
         array = ma.MaskedArray(array, mask=array == nodata)
     elif hasattr(array, "affine") and hasattr(array, "data"):  # pragma: no cover
-        array_transform = array.affine
+        array_transform = getattr(array, "affine")
         in_crs = array.crs
         array = array.data
     elif hasattr(array, "transform") and hasattr(array, "data"):  # pragma: no cover
         array_transform = array.transform
         in_crs = array.crs
         array = array.data
     elif isinstance(array, tuple):
         array = ma.MaskedArray(
             data=np.stack(array),
             mask=np.stack(
                 [
-                    band.mask
-                    if isinstance(band, ma.masked_array)
-                    else np.where(band == nodata, True, False)
+                    (
+                        band.mask
+                        if isinstance(band, ma.masked_array)
+                        else np.where(band == nodata, True, False)
+                    )
                     for band in array
                 ]
             ),
             fill_value=nodata,
         )
     else:
         raise TypeError("wrong input data type: %s" % type(array))
@@ -281,7 +290,78 @@
     dtype: Optional[DTypeLike] = None,
 ) -> Union[np.ndarray, ma.MaskedArray]:
     dtype = dtype or data.dtype
     if masked:
         return ma.masked_values(data.astype(dtype, copy=False), nodata, copy=False)
     else:
         return ma.filled(data.astype(dtype, copy=False), nodata)
+
+
+def clip_array_with_vector(
+    array: np.ndarray,
+    array_affine: Affine,
+    geometries: List[dict],
+    inverted: bool = False,
+    clip_buffer: float = 0,
+) -> ma.MaskedArray:
+    """
+    Clip input array with a vector list.
+
+    Parameters
+    ----------
+    array : array
+        input raster data
+    array_affine : Affine
+        Affine object describing the raster's geolocation
+    geometries : iterable
+        iterable of dictionaries, where every entry has a 'geometry' and
+        'properties' key.
+    inverted : bool
+        invert clip (default: False)
+    clip_buffer : integer
+        buffer (in pixels) geometries before clipping
+
+    Returns
+    -------
+    clipped array : array
+    """
+    # buffer input geometries and clean up
+    buffered_geometries = []
+    for feature in geometries:
+        feature_geom = to_shape(feature["geometry"])
+        if feature_geom.is_empty:
+            continue
+        if feature_geom.geom_type == "GeometryCollection":
+            # for GeometryCollections apply buffer to every subgeometry
+            # and make union
+            buffered_geom = unary_union(
+                [g.buffer(clip_buffer) for g in feature_geom.geoms]
+            )
+        else:
+            buffered_geom = feature_geom.buffer(clip_buffer)
+        if not buffered_geom.is_empty:
+            buffered_geometries.append(buffered_geom)
+
+    # mask raster by buffered geometries
+    if buffered_geometries:
+        if array.ndim == 2:
+            return ma.masked_array(
+                array,
+                geometry_mask(
+                    buffered_geometries, array.shape, array_affine, invert=inverted
+                ),
+            )
+        elif array.ndim == 3:
+            mask = geometry_mask(
+                buffered_geometries,
+                (array.shape[1], array.shape[2]),
+                array_affine,
+                invert=inverted,
+            )
+            return ma.masked_array(array, mask=np.stack([mask for band in array]))
+        else:  # pragma: no cover
+            raise ValueError("array has to be 2D or 3D")
+
+    # if no geometries, return unmasked array
+    else:
+        fill = False if inverted else True
+        return ma.masked_array(array, mask=np.full(array.shape, fill, dtype=bool))
```

### Comparing `mapchete-2024.5.0/mapchete/io/raster/convert.py` & `mapchete-2024.5.1/mapchete/io/raster/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
 
 from mapchete.io import copy
 from mapchete.io.raster.open import rasterio_open
-from mapchete.io.raster.read import read_raster_window
-from mapchete.io.raster.referenced_raster import ReferencedRaster
 from mapchete.path import MPath
 
 logger = logging.getLogger(__name__)
 
 
 def convert_raster(inp, out, overwrite=False, exists_ok=True, **kwargs):
     """
```

### Comparing `mapchete-2024.5.0/mapchete/io/raster/mosaic.py` & `mapchete-2024.5.1/mapchete/io/raster/mosaic.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/io/raster/open.py` & `mapchete-2024.5.1/mapchete/io/raster/open.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/io/raster/read.py` & `mapchete-2024.5.1/mapchete/io/raster/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Wrapper functions around rasterio and useful raster functions."""
+
 from __future__ import annotations
 
 import logging
 import warnings
 from contextlib import contextmanager
-from typing import Iterable, List, Optional, Tuple, Union
+from typing import Generator, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.ma as ma
 import rasterio
 from affine import Affine
 from numpy.typing import DTypeLike
 from rasterio.enums import Resampling
@@ -33,15 +34,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
 def rasterio_read(
     path: MPathLike, mode: str = "r", **kwargs
-) -> Union[DatasetReader, DatasetWriter]:
+) -> Generator[Union[DatasetReader, DatasetWriter], None, None]:
     """
     Wrapper around rasterio.open but rasterio.Env is set according to path properties.
     """
     path = MPath.from_inp(path)
     with path.rio_env() as env:
         try:
             logger.debug("reading %s with GDAL options %s", str(path), env.options)
@@ -49,15 +50,15 @@
                 yield src
         except RasterioIOError as rio_exc:
             _extract_filenotfound_exception(rio_exc, path)
 
 
 def read_raster_window(
     input_files: Union[MPathLike, List[MPathLike]],
-    grid: GridProtocol,
+    grid: Union[Grid, GridProtocol],
     indexes: Optional[Union[int, List[int]]] = None,
     resampling: Union[Resampling, str] = Resampling.nearest,
     src_nodata: NodataVal = None,
     dst_nodata: NodataVal = None,
     dst_dtype: Optional[DTypeLike] = None,
     gdal_opts: Optional[dict] = None,
     skip_missing_files: bool = False,
@@ -69,41 +70,41 @@
     raster. If tile boundaries cross the antimeridian, data on the other side
     of the antimeridian will be read and concatenated to the numpy array
     accordingly.
     """
     resampling = (
         resampling if isinstance(resampling, Resampling) else Resampling[resampling]
     )
-    input_files = [
+    input_paths: List[MPath] = [
         MPath.from_inp(input_file)
         for input_file in (
             input_files if isinstance(input_files, list) else [input_files]
         )
     ]
-    if len(input_files) == 0:  # pragma: no cover
+    if len(input_paths) == 0:  # pragma: no cover
         raise ValueError("no input given")
 
-    with input_files[0].rio_env(gdal_opts) as env:
+    with input_paths[0].rio_env(gdal_opts) as env:
         logger.debug(
-            "reading %s file(s) with GDAL options %s", len(input_files), env.options
+            "reading %s file(s) with GDAL options %s", len(input_paths), env.options
         )
         return _read_raster_window(
-            input_files,
+            input_paths,
             grid,
             indexes=indexes,
             resampling=resampling,
             src_nodata=src_nodata,
             dst_nodata=dst_nodata,
             dst_dtype=dst_dtype,
             skip_missing_files=skip_missing_files,
         )
 
 
 def _read_raster_window(
-    input_files: Union[MPathLike, List[MPathLike]],
+    input_files: List[MPath],
     grid: GridProtocol,
     indexes: Optional[Union[int, List[int]]] = None,
     resampling: Resampling = Resampling.nearest,
     src_nodata: NodataVal = None,
     dst_nodata: NodataVal = None,
     dst_dtype: Optional[DTypeLike] = None,
     skip_missing_files: bool = False,
```

### Comparing `mapchete-2024.5.0/mapchete/io/raster/referenced_raster.py` & `mapchete-2024.5.1/mapchete/io/raster/referenced_raster.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,53 @@
+from __future__ import annotations
+
 import logging
-import warnings
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 import numpy as np
 import numpy.ma as ma
 from affine import Affine
-from shapely.geometry import box, mapping
+from rasterio.transform import array_bounds
+from retry import retry
+from shapely.geometry import mapping, shape
 
 from mapchete.io.raster.array import resample_from_array
 from mapchete.io.raster.open import rasterio_open
 from mapchete.io.raster.read import read_raster_window
 from mapchete.path import MPath
 from mapchete.protocols import GridProtocol
-from mapchete.tile import BufferedTile
-from mapchete.types import Bounds, CRSLike, MPathLike, NodataVal
+from mapchete.settings import IORetrySettings
+from mapchete.types import Bounds, BoundsLike, CRSLike, Grid, MPathLike, NodataVal
 
 logger = logging.getLogger(__name__)
 
 
 class ReferencedRaster:
     """
     A loose in-memory representation of a rasterio dataset.
 
     Useful to ship cached raster files between dask worker nodes.
     """
 
     data: Union[np.ndarray, ma.masked_array]
+    array: Union[np.ndarray, ma.masked_array]
     transform: Affine
-    bounds: Union[List[float], Tuple[float], Bounds]
+    bounds: Bounds
     crs: CRSLike
     nodata: Optional[NodataVal] = None
     driver: Optional[str] = None
 
     def __init__(
         self,
         data: Union[np.ndarray, ma.masked_array],
         transform: Affine,
-        bounds: Union[List[float], Tuple[float], Bounds],
         crs: CRSLike,
+        bounds: Optional[BoundsLike] = None,
         nodata: Optional[NodataVal] = None,
-        driver: Optional[str] = None,
+        driver: Optional[str] = "COG",
         **kwargs,
     ):
         if data.ndim == 1:  # pragma: no cover
             raise TypeError("input array must have at least 2 dimensions")
         elif data.ndim == 2:
             self.count = 1
             self.height, self.width = data.shape
@@ -53,22 +57,24 @@
             # for arrays with more dimensions, the first axis is assumed to be
             # the bands and the last two the width and height
             self.count = data.shape[0]
             self.height, self.width = data.shape[-2:]
         transform = transform or kwargs.get("affine")
         if transform is None:  # pragma: no cover
             raise ValueError("georeference given")
-        self.data = data
+        self.data = self.array = data
         self.driver = driver
         self.dtype = self.data.dtype
         self.nodata = nodata
         self.crs = crs
         self.transform = self.affine = transform
-        self.bounds = bounds
-        self.__geo_interface__ = mapping(box(*self.bounds))
+        self.bounds = Bounds.from_inp(
+            bounds or array_bounds(self.height, self.width, self.transform)
+        )
+        self.__geo_interface__ = mapping(shape(self.bounds))
 
     @property
     def meta(self) -> dict:
         return {
             "driver": self.driver,
             "dtype": self.dtype,
             "nodata": self.nodata,
@@ -77,121 +83,140 @@
             "count": self.count,
             "crs": self.crs,
             "transform": self.transform,
         }
 
     def read(
         self,
-        indexes: Union[int, List[int]] = None,
-        tile: Optional[BufferedTile] = None,
-        grid: Optional[GridProtocol] = None,
+        indexes: Optional[Union[int, List[int]]] = None,
+        grid: Optional[Union[Grid, GridProtocol]] = None,
         resampling: str = "nearest",
     ) -> np.ndarray:
         """Either read full array or resampled to grid."""
-        if tile:  # pragma: no cover
-            warnings.warn(
-                DeprecationWarning("'tile' is deprecated and should be 'grid'")
-            )
-            grid = grid or tile
         # select bands using band indexes
         if indexes is None or self.data.ndim == 2:
             band_selection = self.data
         else:
             band_selection = self._stack(
-                [self.data[i - 1] for i in self._get_band_indexes(indexes)]
+                [self.data[i - 1] for i in self.get_band_indexes(indexes)]
             )
 
         # return either full array or a window resampled to grid
         if grid is None:
             return band_selection
         else:
             return resample_from_array(
                 array=band_selection,
                 in_affine=self.transform,
                 in_crs=self.crs,
                 nodataval=self.nodata,
                 nodata=self.nodata,
-                out_grid=grid,
+                out_grid=Grid.from_obj(grid),
                 resampling=resampling,
             )
 
-    def _get_band_indexes(self, indexes: Union[List[int], int] = None) -> List[int]:
+    def get_band_indexes(
+        self, indexes: Optional[Union[List[int], int]] = None
+    ) -> List[int]:
         """Return valid band indexes."""
         if isinstance(indexes, int):
             return [indexes]
-        else:
+        elif isinstance(indexes, list):
             return indexes
+        else:
+            return list(range(1, self.count + 1))
 
     def _stack(self, *args) -> np.ndarray:
         """return stack of numpy or numpy.masked depending on array type"""
         return (
             ma.stack(*args)
             if isinstance(self.data, ma.masked_array)
             else np.stack(*args)
         )
 
     def to_file(
         self,
         path: MPath,
-        indexes: Union[int, List[int]] = None,
-        tile: Optional[BufferedTile] = None,
-        grid: Optional[GridProtocol] = None,
+        indexes: Optional[Union[int, List[int]]] = None,
+        grid: Optional[Union[Grid, GridProtocol]] = None,
         resampling: str = "nearest",
         **kwargs,
     ) -> MPath:
         """Write raster to output."""
-        if tile:  # pragma: no cover
-            warnings.warn(
-                DeprecationWarning("'tile' is deprecated and should be 'grid'")
-            )
-            grid = grid or tile
+        grid = Grid.from_obj(grid) if grid else None
         with rasterio_open(path, "w", **dict(self.meta, **kwargs)) as dst:
             src_array = self.read(indexes=indexes, grid=grid, resampling=resampling)
             if src_array.ndim == 2:
                 index = 1
             elif src_array.ndim == 3:
                 index = None
             else:  # pragma: no cover
                 raise TypeError(
                     "dumping to file is only possible with 2 or 3-dimensional arrays"
                 )
             dst.write(src_array, index)
         return path
 
     @staticmethod
-    def from_rasterio(src, masked: bool = True) -> "ReferencedRaster":
+    def from_rasterio(
+        src,
+        masked: bool = True,
+    ) -> ReferencedRaster:
         return ReferencedRaster(
             data=src.read(masked=masked).copy(),
             transform=src.transform,
             bounds=src.bounds,
             crs=src.crs,
         )
 
     @staticmethod
-    def from_file(path, masked: bool = True) -> "ReferencedRaster":
-        with rasterio_open(path) as src:
-            return ReferencedRaster.from_rasterio(src, masked=masked)
+    def from_file(
+        path: MPathLike,
+        grid: Optional[Union[Grid, GridProtocol]] = None,
+        masked: bool = True,
+        **kwargs,
+    ) -> ReferencedRaster:
+        path = MPath.from_inp(path)
+
+        logger.debug(f"reading {str(path)} into memory")
+        if grid:
+            grid = Grid.from_obj(grid)
+            data = read_raster_window(path, grid=grid, **kwargs)
+            return ReferencedRaster(
+                data=data if masked else data.filled(),
+                transform=grid.transform,
+                bounds=grid.bounds,
+                crs=grid.crs,
+            )
+
+        @retry(logger=logger, **dict(IORetrySettings()))
+        def _read_raster():
+            with rasterio_open(path, "r") as src:
+                return ReferencedRaster.from_rasterio(
+                    src,
+                    masked=masked,
+                )
+
+        return _read_raster()
+
+    @staticmethod
+    def from_array_like(
+        array_like: Union[np.ndarray, ma.MaskedArray, GridProtocol, ReferencedRaster],
+        transform: Optional[Affine] = None,
+        crs: Optional[CRSLike] = None,
+    ) -> ReferencedRaster:
+        if isinstance(array_like, ReferencedRaster):
+            return array_like
+        elif isinstance(array_like, np.ndarray):
+            if transform is None or crs is None:
+                raise ValueError("array transform and CRS must be provided")
+            return ReferencedRaster(data=array_like, transform=transform, crs=crs)
+        raise TypeError(f"cannot convert {array_like} to ReferencedRaster")
 
 
 def read_raster(
-    inp: MPathLike, grid: Optional[GridProtocol] = None, **kwargs
+    inp: MPathLike,
+    grid: Optional[Union[Grid, GridProtocol]] = None,
+    masked: bool = True,
+    **kwargs,
 ) -> ReferencedRaster:
-    if kwargs.get("tile"):  # pragma: no cover
-        warnings.warn(DeprecationWarning("'tile' is deprecated and should be 'grid'"))
-        grid = grid or kwargs.get("tile")
-        kwargs.pop("tile")
-    inp = MPath.from_inp(inp)
-    logger.debug(f"reading {str(inp)} into memory")
-    if grid:
-        return ReferencedRaster(
-            data=read_raster_window(inp, grid=grid, **kwargs),
-            transform=grid.transform,
-            bounds=grid.bounds,
-            crs=grid.crs,
-        )
-    with rasterio_open(inp, "r") as src:
-        return ReferencedRaster(
-            data=src.read(masked=True),
-            transform=src.transform,
-            bounds=src.bounds,
-            crs=src.crs,
-        )
+    return ReferencedRaster.from_file(inp, grid=grid, masked=masked, **kwargs)
```

### Comparing `mapchete-2024.5.0/mapchete/io/raster/write.py` & `mapchete-2024.5.1/mapchete/io/raster/write.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processes/__init__.py` & `mapchete-2024.5.1/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processes/contours.py` & `mapchete-2024.5.1/mapchete/processes/contours.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+"""Contour line extraction using matplotlib."""
+
 import logging
+from typing import Generator, List, Optional
 
-from shapely.geometry import mapping, shape
+import numpy as np
+from shapely.geometry import LineString, mapping, shape
 from shapely.ops import unary_union
 
+from mapchete import Empty, RasterInput, VectorInput
+from mapchete.io import MatchingMethod
+from mapchete.tile import BufferedTile
+from mapchete.types import ResamplingLike
+
 logger = logging.getLogger(__name__)
 
 
 def execute(
-    mp,
-    resampling="nearest",
-    interval=100,
-    field="elev",
-    base=0,
-    td_matching_method="gdal",
-    td_matching_max_zoom=None,
-    td_matching_precision=8,
-    td_fallback_to_higher_zoom=False,
+    dem: RasterInput,
+    clip: Optional[VectorInput] = None,
+    resampling: ResamplingLike = "nearest",
+    interval: float = 100,
+    field: str = "elev",
+    base: float = 0,
+    td_matching_method: MatchingMethod = MatchingMethod.gdal,
+    td_matching_max_zoom: Optional[int] = None,
+    td_matching_precision: int = 8,
+    td_fallback_to_higher_zoom: bool = False,
     clip_pixelbuffer=0,
-    **kwargs
-):
+) -> List[dict]:
     """
     Generate hillshade from DEM.
 
     Inputs
     ------
     dem
         Input DEM.
@@ -61,60 +70,109 @@
         Use pixelbuffer when clipping output by geometry. (default: 0)
 
     Output
     ------
     list of GeoJSON-like features
     """
     # read clip geometry
-    if "clip" in mp.params["input"]:
-        clip_geom = mp.open("clip").read()
+    if clip:
+        clip_geom = clip.read()
         if not clip_geom:
             logger.debug("no clip data over tile")
-            return "empty"
+            raise Empty("no clip data over tile")
     else:
         clip_geom = []
 
-    with mp.open(
-        "dem",
-    ) as dem:
-        logger.debug("reading input raster")
-        dem_data = dem.read(
-            1,
-            resampling=resampling,
-            matching_method=td_matching_method,
-            matching_max_zoom=td_matching_max_zoom,
-            matching_precision=td_matching_precision,
-            fallback_to_higher_zoom=td_fallback_to_higher_zoom,
-        )
-        if dem_data.mask.all():
-            logger.debug("raster empty")
-            return "empty"
+    if dem.is_empty():
+        raise Empty("no DEM data over tile")
+
+    logger.debug("reading input raster")
+    dem_data = dem.read(
+        1,
+        resampling=resampling,
+        matching_method=td_matching_method,
+        matching_max_zoom=td_matching_max_zoom,
+        matching_precision=td_matching_precision,
+        fallback_to_higher_zoom=td_fallback_to_higher_zoom,
+    )
+    if dem_data.mask.all():  # pragma: no cover
+        logger.debug("DEM data empty over tile")
+        raise Empty("DEM data empty over tile")
 
     logger.debug("calculate hillshade")
-    contours = mp.contours(
-        dem_data,
-        interval=interval,
-        field=field,
-        base=base,
+    contour_lines = list(
+        generate_contours(
+            dem_data,
+            dem.tile,
+            interval=interval,
+            field=field,
+            base=base,
+        )
     )
 
-    if clip_geom:
+    if clip:
         logger.debug("clipping output with geometry")
         # use inverted clip geometry to extract contours
-        clip_geom = mp.tile.bbox.difference(
+        clip_geom = dem.tile.bbox.difference(
             unary_union([shape(i["geometry"]) for i in clip_geom]).buffer(
-                clip_pixelbuffer * mp.tile.pixel_x_size
+                clip_pixelbuffer * dem.tile.pixel_x_size
             )
         )
         out_contours = []
-        for contour in contours:
+        for contour in contour_lines:
             out_geom = shape(contour["geometry"]).intersection(clip_geom)
             if not out_geom.is_empty:
                 out_contours.append(
                     dict(
                         contour,
                         geometry=mapping(out_geom),
                     )
                 )
         return out_contours
     else:
-        return contours
+        return contour_lines
+
+
+def generate_contours(
+    array: np.ndarray,
+    tile: BufferedTile,
+    interval: float = 100,
+    field: str = "elev",
+    base: float = 0,
+) -> Generator[dict, None, None]:
+    import matplotlib.pyplot as plt
+
+    elevations = (
+        get_contour_values(array.min(), array.max(), interval=interval, base=base) or []
+    )
+    for elevation, contours in zip(
+        elevations, plt.contour(array, elevations).collections
+    ):
+        for path in contours.get_paths():
+            out_coords = [
+                (
+                    tile.left + (y * tile.pixel_x_size),
+                    tile.top - (x * tile.pixel_y_size),
+                )
+                for x, y in np.asarray(path.vertices)
+            ]
+            if len(out_coords) >= 2:
+                yield dict(
+                    properties={field: elevation},
+                    geometry=mapping(LineString(out_coords)),
+                )
+
+
+def get_contour_values(
+    min_val: float, max_val: float, base: float = 0, interval: float = 100
+) -> List[float]:
+    """Return a list of values between min and max within an interval."""
+    i = base
+    out = []
+    if min_val < base:
+        while i >= min_val:
+            i -= interval
+    while i <= max_val:
+        if i >= min_val:
+            out.append(i)
+        i += interval
+    return out
```

### Comparing `mapchete-2024.5.0/mapchete/processes/convert.py` & `mapchete-2024.5.1/mapchete/processes/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import logging
-import warnings
+from typing import List, Optional, Union
 
 import numpy as np
 from rasterio.dtypes import dtype_ranges
 
+from mapchete import Empty, RasterInput, VectorInput
+from mapchete.io import MatchingMethod
+from mapchete.io.raster.array import clip_array_with_vector
+from mapchete.types import BandIndexes, ResamplingLike
+
 logger = logging.getLogger(__name__)
 
 
 def execute(
-    mp,
-    resampling="nearest",
-    band_indexes=None,
-    td_matching_method="gdal",
-    td_matching_max_zoom=None,
-    td_matching_precision=8,
-    td_fallback_to_higher_zoom=False,
-    clip_pixelbuffer=0,
-    scale_ratio=1.0,
-    scale_offset=0.0,
-    clip_to_output_dtype=None,
+    inp: Union[RasterInput, VectorInput],
+    clip: Optional[VectorInput] = None,
+    resampling: ResamplingLike = "nearest",
+    band_indexes: Optional[BandIndexes] = None,
+    td_matching_method: MatchingMethod = MatchingMethod.gdal,
+    td_matching_max_zoom: Optional[int] = None,
+    td_matching_precision: int = 8,
+    td_fallback_to_higher_zoom: bool = False,
+    clip_pixelbuffer: int = 0,
+    scale_ratio: float = 1.0,
+    scale_offset: float = 0.0,
+    clip_to_output_dtype: Optional[str] = None,
     **kwargs,
-):
+) -> Union[np.ndarray, List[dict]]:
     """
     Convert and optionally clip input raster or vector data.
 
     Inputs
     ------
     inp
         Raster or vector input.
@@ -65,72 +71,62 @@
         Clip output values to range of given dtype. (default: None)
 
     Output
     ------
     np.ndarray
     """
     # read clip geometry
-    if "clip" in mp.params["input"]:
-        clip_geom = mp.open("clip").read()
+    if clip is None:
+        clip_geom = []
+    else:
+        clip_geom = clip.read()
         if not clip_geom:
             logger.debug("no clip data over tile")
-            return "empty"
-    else:
-        clip_geom = []
+            raise Empty
 
-    if "raster" in mp.input:  # pragma: no cover
-        warnings.warn(
-            UserWarning(
-                "'raster' input name in the mapchete configuration is deprecated and has to be named 'inp'"
-            )
-        )
-        inp_key = "raster"
-    else:
-        inp_key = "inp"
-    with mp.open(inp_key) as inp:
-        if inp.is_empty():
-            return "empty"
-        logger.debug("reading input data")
+    if inp.is_empty():
+        raise Empty
+
+    logger.debug("reading input data")
+    if isinstance(inp, RasterInput):
         input_data = inp.read(
             indexes=band_indexes,
             resampling=resampling,
             matching_method=td_matching_method,
             matching_max_zoom=td_matching_max_zoom,
             matching_precision=td_matching_precision,
             fallback_to_higher_zoom=td_fallback_to_higher_zoom,
         )
-        if isinstance(input_data, np.ndarray):
-            input_type = "raster"
-        elif isinstance(input_data, list):
-            input_type = "vector"
-        else:  # pragma: no cover
-            raise TypeError(
-                "input data type for this process has to either be a raster or a vector "
-                "dataset"
-            )
-
-    if input_type == "raster":
         if scale_offset != 0.0:
             logger.debug("apply scale offset %s", scale_offset)
             input_data = input_data.astype("float64", copy=False) + scale_offset
         if scale_ratio != 1.0:
             logger.debug("apply scale ratio %s", scale_ratio)
             input_data = input_data.astype("float64", copy=False) * scale_ratio
         if (
-            scale_offset != 0.0 or scale_ratio != 1.0
-        ) and clip_to_output_dtype in dtype_ranges:
+            clip_to_output_dtype
+            and (scale_offset != 0.0 or scale_ratio != 1.0)
+            and clip_to_output_dtype in dtype_ranges
+        ):
             logger.debug("clip to output dtype ranges")
             input_data.clip(*dtype_ranges[clip_to_output_dtype], out=input_data)
 
         if clip_geom:
             logger.debug("clipping output with geometry")
             # apply original nodata mask and clip
-            return mp.clip(input_data, clip_geom, clip_buffer=clip_pixelbuffer)
+            return clip_array_with_vector(
+                input_data, inp.tile.affine, clip_geom, clip_buffer=clip_pixelbuffer
+            )
         else:
             return input_data
 
-    elif input_type == "vector":
+    elif isinstance(inp, VectorInput):
+        input_data = inp.read()
         if clip_geom:  # pragma: no cover
             raise NotImplementedError("clipping vector data is not yet implemented")
         else:
             logger.debug(f"writing {len(input_data)} features")
             return input_data
+    else:  # pragma: no cover
+        raise TypeError(
+            f"inp must either be of type RasterInput or VectorInput, not {type(inp)}"
+        )
```

### Comparing `mapchete-2024.5.0/mapchete/processes/examples/example_process.py` & `mapchete-2024.5.1/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/base.py` & `mapchete-2024.5.1/mapchete/processing/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 """Main module managing processes."""
 
 import json
 import logging
 import os
 import threading
 from contextlib import ExitStack
-from typing import Any, Iterator, List, Optional, Tuple, Union
+from typing import Any, Generator, Iterator, List, Optional, Tuple, Union
 
 from cachetools import LRUCache
 from shapely.geometry import Polygon, base
 from shapely.ops import unary_union
 
 from mapchete.config import DaskSettings, MapcheteConfig
 from mapchete.enums import Concurrency, ProcessingMode
 from mapchete.errors import MapcheteNodataTile, ReprojectionFailed
-from mapchete.executor import (
-    MULTIPROCESSING_DEFAULT_START_METHOD,
-    DaskExecutor,
-    Executor,
-    ExecutorBase,
-    MFuture,
-)
-from mapchete.executor.base import func_partial
+from mapchete.executor import Executor, ExecutorBase, MFuture
 from mapchete.executor.types import Profiler
 from mapchete.path import batch_sort_property, tiles_exist
 from mapchete.processing.execute import batches, dask_graph, single_batch
 from mapchete.processing.tasks import (
     TaskBatch,
     TaskInfo,
     Tasks,
@@ -88,15 +81,15 @@
             self.process_tile_cache = LRUCache(maxsize=512)
             self.current_processes = {}
             self.process_lock = threading.Lock()
         self._count_tiles_cache = {}
 
     def get_process_tiles(
         self, zoom: Optional[int] = None, batch_by: Optional[str] = None
-    ) -> Iterator[BufferedTile]:
+    ) -> Generator[BufferedTile, None, None]:
         """
         Yield process tiles.
 
         Tiles intersecting with the input data bounding boxes as well as
         process bounds, if provided, are considered process tiles. This is to
         avoid iterating through empty tiles.
 
@@ -109,14 +102,16 @@
             if not None, tiles can be yielded in batches either by "row" or "column".
 
         yields
         ------
         BufferedTile objects
         """
         logger.debug("get process tiles...")
+        # if batch_by is None and hasattr(self.config.output_reader, "tile_path_schema"):
+        #     batch_by = batch_sort_property(self.config.output_reader.tile_path_schema)
         if zoom or zoom == 0:
             for tile in self.config.process_pyramid.tiles_from_geom(
                 self.config.area_at_zoom(zoom),
                 zoom=zoom,
                 batch_by=batch_by,
                 exact=True,
             ):
@@ -126,16 +121,16 @@
                 for tile in self.config.process_pyramid.tiles_from_geom(
                     self.config.area_at_zoom(i), zoom=i, batch_by=batch_by, exact=True
                 ):
                     yield tile
 
     def skip_tiles(
         self,
-        tiles: Iterator[BufferedTile] = None,
-        tiles_batches: Iterator[Iterator[BufferedTile]] = None,
+        tiles: Optional[Iterator[BufferedTile]] = None,
+        tiles_batches: Optional[Iterator[Iterator[BufferedTile]]] = None,
     ) -> Iterator[Tuple[BufferedTile, bool]]:
         """
         Quickly determine whether tiles can be skipped for processing.
 
         The skip value is True if process mode is 'continue' and process output already
         exists. In all other cases, skip is False.
 
@@ -157,17 +152,19 @@
             )
         # otherwise don't skip tiles
         else:
             if tiles_batches:  # pragma: no cover
                 for batch in tiles_batches:
                     for tile in batch:
                         yield (tile, False)
-            else:
+            elif tiles:
                 for tile in tiles:
                     yield (tile, False)
+            else:  # pragma: no cover
+                raise TypeError("either tiles or tiles_batches required")
 
     def tasks(
         self,
         zoom: Optional[ZoomLevelsLike] = None,
         tile: Optional[TileLike] = None,
         profilers: Optional[List[Profiler]] = None,
     ) -> Tasks:
@@ -200,15 +197,15 @@
     def execute(
         self,
         tasks: Optional[Tasks] = None,
         zoom: Optional[ZoomLevelsLike] = None,
         tile: Optional[TileLike] = None,
         executor: Optional[ExecutorBase] = None,
         concurrency: Concurrency = Concurrency.none,
-        workers: int = os.cpu_count(),
+        workers: Optional[int] = os.cpu_count(),
         propagate_results: bool = False,
         dask_settings: DaskSettings = DaskSettings(),
         remember_preprocessing_results: bool = False,
     ) -> Iterator[TaskInfo]:
         """
         Execute all tasks on given executor and yield TaskInfo as they finish.
         """
@@ -518,15 +515,14 @@
         # get output_tiles that intersect with current tile
         if tile.pixelbuffer > self.config.output.pixelbuffer:
             output_tiles = list(
                 self.config.output_pyramid.tiles_from_bounds(tile.bounds, tile.zoom)
             )
         else:
             output_tiles = self.config.output_pyramid.intersecting(tile)
-
         if self.config.mode == ProcessingMode.READONLY or _baselevel_readonly:
             if self.config.output.tiles_exist(process_tile):
                 return self._read_existing_output(tile, output_tiles)
             else:
                 return self.config.output.empty(tile)
         elif self.config.mode == ProcessingMode.CONTINUE and not _baselevel_readonly:
             if self.config.output.tiles_exist(process_tile):
@@ -768,23 +764,23 @@
                 else ZoomLevels.from_inp(zoom)
             )
             # here we store the parents of tiles about to be processed so we can update overviews
             # also in "continue" mode in case there were updates at the baselevel
             overview_parents = set()
             for i, zoom in enumerate(zoom_levels.descending()):
                 tile_tasks = []
-
+                if hasattr(process.config.output_reader, "tile_path_schema"):
+                    batch_by = batch_sort_property(
+                        process.config.output_reader.tile_path_schema
+                    )
+                else:
+                    batch_by = "row"
                 for tile in _filter_skipable(
                     process=process,
-                    tiles_batches=process.get_process_tiles(
-                        zoom,
-                        batch_by=batch_sort_property(
-                            process.config.output_reader.tile_path_schema
-                        ),
-                    ),
+                    tiles_batches=process.get_process_tiles(zoom, batch_by=batch_by),
                     overview_tiles=(
                         overview_parents if process.config.baselevels and i else None
                     ),
                 ):
                     # we don't need the current tile anymore
                     overview_parents.discard(tile)
```

### Comparing `mapchete-2024.5.0/mapchete/processing/execute.py` & `mapchete-2024.5.1/mapchete/processing/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/tasks.py` & `mapchete-2024.5.1/mapchete/processing/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from mapchete.io._geometry_operations import to_shape
 from mapchete.io.vector import IndexedFeatures
 from mapchete.path import MPath
 from mapchete.processing.mp import MapcheteProcess
 from mapchete.processing.types import TaskInfo, default_tile_task_id
 from mapchete.tile import BufferedTile
 from mapchete.timer import Timer
-from mapchete.types import Bounds, BoundsLike, TileLike, ZoomLevels, ZoomLevelsLike
+from mapchete.types import Bounds, BoundsLike, TileLike, ZoomLevels
 from mapchete.validate import validate_bounds
 
 logger = logging.getLogger(__name__)
 
 
 class Task(ABC):
     """Generic processing task.
@@ -48,34 +48,34 @@
     Can optionally have spatial properties attached which helps building up dependencies
     between tasks.
     """
 
     id: str
     func: Callable
     fargs: Tuple
-    fkwargs: Tuple
+    fkwargs: dict
     dependencies: Dict[str, TaskInfo]
     result_key_name: str
     geometry: Optional[Union[base.BaseGeometry, dict]] = None
     bounds: Optional[Bounds] = None
     tile: Optional[BufferedTile] = None
 
     def __init__(
         self,
+        func: Callable,
         id: Optional[str] = None,
-        func: Optional[Callable] = None,
         fargs: Optional[Tuple] = None,
-        fkwargs: Optional[Tuple] = None,
+        fkwargs: Optional[dict] = None,
         dependencies: Optional[Dict[str, TaskInfo]] = None,
         result_key_name: Optional[str] = None,
         geometry: Optional[Union[base.BaseGeometry, dict]] = None,
         bounds: Optional[BoundsLike] = None,
     ):
-        self.id = id or uuid4().hex
         self.func = func
+        self.id = id or uuid4().hex
         self.fargs = fargs or ()
         self.fkwargs = fkwargs or {}
         self.dependencies = dependencies or {}
         self.result_key_name = result_key_name or f"{self.id}_result"
         if geometry and bounds:
             raise ValueError("only provide one of either 'geometry' or 'bounds'")
         elif geometry:
@@ -244,15 +244,15 @@
         else:
             self.input = config.get_inputs_for_tile(tile)
             self.process_func_params = config.get_process_func_params(tile.zoom)
             self.output_params = config.output_reader.output_params
         self.mode = config.mode
         self.output_reader = config.output_reader if config.baselevels else None
         self._dependencies = dict()
-        super().__init__(id=self.id, geometry=tile.bbox)
+        super().__init__(self.func, id=self.id, geometry=tile.bbox)
 
     def __repr__(self):  # pragma: no cover
         return f"TileTask(id={self.id}, tile={self.tile}, bounds={self.bounds})"
 
     def add_dependency(self, task_key: str, result: Any, raise_error: bool = True):
         """Append preprocessing task result to input."""
         # if dependency has geo information, only add if it intersects with task!
@@ -344,22 +344,28 @@
                                 raise KeyError(f"malformed task key: {inp_key}")
                             for inp in self.input.values():
                                 if inp.input_key == inp_key:
                                     inp.set_preprocessing_task_result(
                                         task_key=task_key, result=task_result
                                     )
                 # Actually run process.
+                mp = MapcheteProcess(
+                    tile=self.tile,
+                    params=self.process_func_params,
+                    input=self.input,
+                    output_params=self.output_params,
+                )
+                # this contains key: params mapping, where under param.annotation we can inspect for target type
+                extended_kwargs = dict(
+                    self.process_func_params,
+                    mp=mp,
+                    **{k: v for k, v in self.input.items()},
+                )
                 process_data = self.process(
-                    MapcheteProcess(
-                        tile=self.tile,
-                        params=self.process_func_params,
-                        input=self.input,
-                        output_params=self.output_params,
-                    ),
-                    **self.process_func_params,
+                    **extended_kwargs,
                 )
         except MapcheteNodataTile:
             raise
         except Exception as e:
             # Log process time and tile
             logger.error((self.tile.id, "exception in user process", e, str(duration)))
             raise
```

### Comparing `mapchete-2024.5.0/mapchete/processing/types.py` & `mapchete-2024.5.1/mapchete/processing/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/profilers/__init__.py` & `mapchete-2024.5.1/mapchete/processing/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/profilers/memory.py` & `mapchete-2024.5.1/mapchete/processing/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/profilers/requests.py` & `mapchete-2024.5.1/mapchete/processing/profilers/requests.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/processing/profilers/time.py` & `mapchete-2024.5.1/mapchete/processing/profilers/time.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/static/index.html` & `mapchete-2024.5.1/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/mapchete/static/process_template.py` & `mapchete-2024.5.1/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/LICENSE` & `mapchete-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/README.rst` & `mapchete-2024.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2024.5.0/pyproject.toml` & `mapchete-2024.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,33 +51,28 @@
     "aiobotocore>=1.1.2",
     "boto3>=1.14.44",
     "dask",
     "distributed",
     "Flask<3.0.0",
     "Flask-RangeRequest",
     "fsspec[http,s3]>=2023.12.0",
-    "geobuf",
     "lxml",
     "matplotlib",
     "memray",
     "protobuf<=3.20.1",
     "pystac[urllib3]<=1.7.3",
     "requests",
     "rtree",
     "s3fs!=2023.9.0",
     "tilebench",
     "werkzeug>=0.15",
 ]
 contours = [
     "matplotlib",
 ]
-geobuf = [
-    "geobuf",
-    "protobuf<=3.20.1",
-]
 http = [
     "aiohttp",
     "fsspec[http]",
     "requests",
 ]
 profiling = [
     "memray",
@@ -119,15 +114,14 @@
 processes = "mapchete.cli.default.processes:processes"
 rm = "mapchete.cli.default.rm:rm"
 serve = "mapchete.cli.default.serve:serve"
 stac = "mapchete.cli.default.stac:stac"
 
 [project.entry-points."mapchete.formats.drivers"]
 flatgeobuf = "mapchete.formats.default.flatgeobuf"
-geobuf = "mapchete.formats.default.geobuf"
 geojson = "mapchete.formats.default.geojson"
 gtiff = "mapchete.formats.default.gtiff"
 mapchete_input = "mapchete.formats.default.mapchete_input"
 png = "mapchete.formats.default.png"
 png_hillshade = "mapchete.formats.default.png_hillshade"
 raster_file = "mapchete.formats.default.raster_file"
 tile_directory = "mapchete.formats.default.tile_directory"
```

### Comparing `mapchete-2024.5.0/PKG-INFO` & `mapchete-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mapchete
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -40,30 +40,26 @@
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: boto3>=1.14.44; extra == 'complete'
 Requires-Dist: dask; extra == 'complete'
 Requires-Dist: distributed; extra == 'complete'
 Requires-Dist: flask-rangerequest; extra == 'complete'
 Requires-Dist: flask<3.0.0; extra == 'complete'
 Requires-Dist: fsspec[http,s3]>=2023.12.0; extra == 'complete'
-Requires-Dist: geobuf; extra == 'complete'
 Requires-Dist: lxml; extra == 'complete'
 Requires-Dist: matplotlib; extra == 'complete'
 Requires-Dist: memray; extra == 'complete'
 Requires-Dist: protobuf<=3.20.1; extra == 'complete'
 Requires-Dist: pystac[urllib3]<=1.7.3; extra == 'complete'
 Requires-Dist: requests; extra == 'complete'
 Requires-Dist: rtree; extra == 'complete'
 Requires-Dist: s3fs!=2023.9.0; extra == 'complete'
 Requires-Dist: tilebench; extra == 'complete'
 Requires-Dist: werkzeug>=0.15; extra == 'complete'
 Provides-Extra: contours
 Requires-Dist: matplotlib; extra == 'contours'
-Provides-Extra: geobuf
-Requires-Dist: geobuf; extra == 'geobuf'
-Requires-Dist: protobuf<=3.20.1; extra == 'geobuf'
 Provides-Extra: http
 Requires-Dist: aiohttp; extra == 'http'
 Requires-Dist: fsspec[http]; extra == 'http'
 Requires-Dist: requests; extra == 'http'
 Provides-Extra: profiling
 Requires-Dist: memray; extra == 'profiling'
 Requires-Dist: tilebench; extra == 'profiling'
```

