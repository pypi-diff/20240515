# Comparing `tmp/types-docker-7.0.0.20240513.tar.gz` & `tmp/types-docker-7.0.0.20240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240513.tar", last modified: Mon May 13 02:23:39 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240515.tar", last modified: Wed May 15 02:24:49 2024, max compression
```

## Comparing `types-docker-7.0.0.20240513.tar` & `types-docker-7.0.0.20240515.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.514142 types-docker-7.0.0.20240513/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.514142 types-docker-7.0.0.20240513/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.546112 types-docker-7.0.0.20240515/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.538112 types-docker-7.0.0.20240515/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.538112 types-docker-7.0.0.20240515/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.538112 types-docker-7.0.0.20240515/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.538112 types-docker-7.0.0.20240515/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 02:24:30.000000 types-docker-7.0.0.20240515/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:24:49.546112 types-docker-7.0.0.20240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:49.542112 types-docker-7.0.0.20240515/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 02:24:49.000000 types-docker-7.0.0.20240515/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240513/CHANGELOG.md` & `types-docker-7.0.0.20240515/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 7.0.0.20240515 (2024-05-15)
+
+Add a number of types to docker.models.containers (#11912)
+
 ## 7.0.0.20240513 (2024-05-13)
 
 Add many types to docker.api.container (#11911)
 
 Add types to all "container" parameters in docker.api.container (#11908)
 
 Add remaining parameter types to docker.api.container logs (#11907)
```

### Comparing `types-docker-7.0.0.20240513/PKG-INFO` & `types-docker-7.0.0.20240515/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240513
+Version: 7.0.0.20240515
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240515/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240515/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/client.pyi` & `types-docker-7.0.0.20240515/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240515/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240515/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240515/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240515/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/containers.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from docker.types.daemon import CancellableStream
 
 from .images import Image
 from .resource import Collection, Model
 
 class Container(Model):
     @property
-    def name(self): ...
+    def name(self) -> str | None: ...
     @property
-    def image(self): ...
+    def image(self) -> Image | None: ...
     @property
     def labels(self): ...
     @property
-    def status(self): ...
+    def status(self) -> str: ...
     @property
-    def health(self): ...
+    def health(self) -> str: ...
     @property
-    def ports(self): ...
+    def ports(self) -> dict[Incomplete, Incomplete]: ...
     def attach(self, **kwargs): ...
     def attach_socket(self, **kwargs): ...
     def commit(self, repository: str | None = None, tag: str | None = None, **kwargs): ...
     def diff(self): ...
     def exec_run(
         self,
         cmd,
@@ -34,24 +34,26 @@
         user: str = "",
         detach: bool = False,
         stream: bool = False,
         socket: bool = False,
         environment: Incomplete | None = None,
         workdir: Incomplete | None = None,
         demux: bool = False,
-    ): ...
-    def export(self, chunk_size=2097152): ...
-    def get_archive(self, path, chunk_size=2097152, encode_stream: bool = False): ...
+    ) -> ExecResult: ...
+    def export(self, chunk_size: int | None = 2097152) -> str: ...
+    def get_archive(
+        self, path, chunk_size: int | None = 2097152, encode_stream: bool = False
+    ) -> tuple[Incomplete, Incomplete]: ...
     def kill(self, signal: Incomplete | None = None): ...
     def logs(self, **kwargs) -> CancellableStream | bytes: ...
     def pause(self): ...
-    def put_archive(self, path, data): ...
+    def put_archive(self, path: str, data) -> bool: ...
     def remove(self, **kwargs) -> None: ...
-    def rename(self, name): ...
-    def resize(self, height, width): ...
+    def rename(self, name: str): ...
+    def resize(self, height: int, width: int): ...
     def restart(self, **kwargs): ...
     def start(self, **kwargs) -> None: ...
     def stats(self, **kwargs): ...
     def stop(self, **kwargs) -> None: ...
     def top(self, **kwargs): ...
     def unpause(self): ...
     def update(self, **kwargs): ...
@@ -64,27 +66,27 @@
         image: str | Image,
         command: str | list[str] | None = None,
         stdout: bool = True,
         stderr: bool = False,
         remove: bool = False,
         **kwargs,
     ): ...
-    def create(self, image: str, command: str | list[str] | None = None, **kwargs): ...  # type:ignore[override]
-    def get(self, container_id: str): ...
+    def create(self, image: str, command: str | list[str] | None = None, **kwargs) -> Container: ...  # type:ignore[override]
+    def get(self, container_id: str) -> Container: ...
     def list(
         self,
         all: bool = False,
-        before: Incomplete | None = None,
+        before: str | None = None,
         filters: Incomplete | None = None,
         limit: int = -1,
-        since: Incomplete | None = None,
+        since: str | None = None,
         sparse: bool = False,
         ignore_removed: bool = False,
     ): ...
     def prune(self, filters: Incomplete | None = None): ...
 
-RUN_CREATE_KWARGS: Incomplete
-RUN_HOST_CONFIG_KWARGS: Incomplete
+RUN_CREATE_KWARGS: list[str]
+RUN_HOST_CONFIG_KWARGS: list[str]
 
 class ExecResult(NamedTuple):
     exit_code: Incomplete
     output: Incomplete
```

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/images.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/networks.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/resource.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/models/volumes.pyi` & `types-docker-7.0.0.20240515/docker-stubs/models/volumes.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240515/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240515/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/transport/sshconn.pyi` & `types-docker-7.0.0.20240515/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240515/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/networks.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/services.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240515/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240515/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240515/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240515/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240515/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240515/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240513/setup.py` & `types-docker-7.0.0.20240515/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240513",
+      version="7.0.0.20240515",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240513/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240515/types_docker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240513
+Version: 7.0.0.20240515
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240513/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240515/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

