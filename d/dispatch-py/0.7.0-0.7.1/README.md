# Comparing `tmp/dispatch_py-0.7.0.tar.gz` & `tmp/dispatch_py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispatch_py-0.7.0.tar", last modified: Fri May  3 23:10:30 2024, max compression
+gzip compressed data, was "dispatch_py-0.7.1.tar", last modified: Tue May 14 22:50:39 2024, max compression
```

## Comparing `dispatch_py-0.7.0.tar` & `dispatch_py-0.7.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.261509 dispatch_py-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-03 23:10:30.261509 dispatch_py-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:10:30.261509 dispatch_py-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.245509 dispatch_py-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.245509 dispatch_py-0.7.0/src/buf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.249508 dispatch_py-0.7.0/src/buf/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/expression_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/expression_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.249508 dispatch_py-0.7.0/src/buf/validate/priv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/priv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/priv/private_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/priv/private_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/validate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.249508 dispatch_py-0.7.0/src/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.249508 dispatch_py-0.7.0/src/dispatch/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.253508 dispatch_py-0.7.0/src/dispatch/experimental/durable/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame308.h
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame309.h
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame310.h
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame311.h
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame312.h
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/frame313.h
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/function.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/durable/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/experimental/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14421 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.253508 dispatch_py-0.7.0/src/dispatch/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/integrations/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    15043 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.253508 dispatch_py-0.7.0/src/dispatch/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.257509 dispatch_py-0.7.0/src/dispatch/sdk/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/call_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/call_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/call_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/exit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/exit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/exit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/poll_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/poll_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/poll_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/sdk/v1/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.257509 dispatch_py-0.7.0/src/dispatch/signature/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/signature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/signature/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/signature/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/signature/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.257509 dispatch_py-0.7.0/src/dispatch/test/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14109 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/src/dispatch/test/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.257509 dispatch_py-0.7.0/src/dispatch_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-03 23:10:30.000000 dispatch_py-0.7.0/src/dispatch_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-03 23:10:30.000000 dispatch_py-0.7.0/src/dispatch_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:10:30.000000 dispatch_py-0.7.0/src/dispatch_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-03 23:10:30.000000 dispatch_py-0.7.0/src/dispatch_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 23:10:30.000000 dispatch_py-0.7.0/src/dispatch_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:30.257509 dispatch_py-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-03 23:10:23.000000 dispatch_py-0.7.0/tests/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.372649 dispatch_py-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-14 22:50:39.372649 dispatch_py-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 22:50:39.372649 dispatch_py-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.356649 dispatch_py-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.356649 dispatch_py-0.7.1/src/buf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.360648 dispatch_py-0.7.1/src/buf/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/expression_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/expression_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.360648 dispatch_py-0.7.1/src/buf/validate/priv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/priv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/priv/private_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/validate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.360648 dispatch_py-0.7.1/src/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.360648 dispatch_py-0.7.1/src/dispatch/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.364649 dispatch_py-0.7.1/src/dispatch/experimental/durable/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame308.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame309.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame310.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame311.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame312.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/frame313.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/durable/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/experimental/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14421 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.364649 dispatch_py-0.7.1/src/dispatch/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/integrations/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15043 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.364649 dispatch_py-0.7.1/src/dispatch/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.368649 dispatch_py-0.7.1/src/dispatch/sdk/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/call_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/call_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/call_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/exit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/exit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/exit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/poll_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/poll_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/poll_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/sdk/v1/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.368649 dispatch_py-0.7.1/src/dispatch/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/signature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/signature/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/signature/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/signature/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.368649 dispatch_py-0.7.1/src/dispatch/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14109 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/src/dispatch/test/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.372649 dispatch_py-0.7.1/src/dispatch_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-14 22:50:39.000000 dispatch_py-0.7.1/src/dispatch_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-14 22:50:39.000000 dispatch_py-0.7.1/src/dispatch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:50:39.000000 dispatch_py-0.7.1/src/dispatch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 22:50:39.000000 dispatch_py-0.7.1/src/dispatch_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 22:50:39.000000 dispatch_py-0.7.1/src/dispatch_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:50:39.372649 dispatch_py-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-14 22:50:32.000000 dispatch_py-0.7.1/tests/test_http.py
```

### Comparing `dispatch_py-0.7.0/CONTRIBUTING.md` & `dispatch_py-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/LICENSE` & `dispatch_py-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/Makefile` & `dispatch_py-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/PKG-INFO` & `dispatch_py-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
@@ -39,25 +39,25 @@
 
 <p align="center">
 <img src="https://github.com/dispatchrun/.github/blob/main/profile/dispatch_logo_light.png?raw=true" height="64"/>
 </p>
 
 # dispatch-py
 
-[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
-[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
-[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
+[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
+[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
+[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[pypi]:    https://pypi.org/project/dispatch-py/
-[signup]:  https://console.dispatch.run/
+[pypi]: https://pypi.org/project/dispatch-py/
+[signup]: https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
   - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
   - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
   - [Writing Dispatch Applications](#writing-dispatch-applications)
@@ -87,22 +87,23 @@
 brew tap dispatchrun/dispatch
 brew install dispatch
 ```
 
 Alternatively, you can download the latest `dispatch` binary from the
 [Releases](https://github.com/dispatchrun/dispatch/releases) page.
 
-*Note that this step is optional, applications that use Dispatch can run without
+_Note that this step is optional, applications that use Dispatch can run without
 the CLI, passing configuration through environment variables or directly in the
 code. However, the CLI automates the onboarding flow and simplifies the
-configuration, so we recommend starting with it.*
+configuration, so we recommend starting with it._
 
 ### Installing the Dispatch SDK
 
 The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+
 ```console
 pip install dispatch-py
 ```
 
 ## Usage
 
 ### Writing Dispatch Applications
@@ -128,27 +129,29 @@
 Obviously, this is just an example, a real application would perform much more
 interesting work, but it's a good start to get a sense of how to use Dispatch.
 
 ### Running Dispatch Applications
 
 The simplest way to run a Dispatch application is to use the Dispatch CLI, first
 we need to login:
+
 ```console
 dispatch login
 ```
 
 Then we are ready to run the example program we wrote above:
+
 ```console
 dispatch run -- python3 main.py
 ```
 
 ### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
-(a.k.a. *async* functions), in which case each `await` point becomes a
+(a.k.a. _async_ functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
 ```python
 @dispatch.function
 async def pipeline(msg):
@@ -188,18 +191,18 @@
     return await gather(*concurrent_calls)
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
-Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
+Dispatch converts Python coroutines to _Distributed Coroutines_, which can be
 suspended and resumed on any instance of a service across a fleet. For a deep
 dive on these concepts, read our blog post on
-[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://dispatch.run/blog/distributed-coroutines-in-python).
+[_Distributed Coroutines with a Native Python Extension and Dispatch_](https://dispatch.run/blog/distributed-coroutines-in-python).
 
 ### Integration with FastAPI
 
 Many web applications written in Python are developed using [FastAPI][fastapi].
 Dispatch can integrate with these applications by instantiating a
 `dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
 declared by the program can be invoked remotely over the same HTTP interface
```

### Comparing `dispatch_py-0.7.0/README.md` & `dispatch_py-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <p align="center">
 <img src="https://github.com/dispatchrun/.github/blob/main/profile/dispatch_logo_light.png?raw=true" height="64"/>
 </p>
 
 # dispatch-py
 
-[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
-[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
-[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
+[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
+[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
+[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[pypi]:    https://pypi.org/project/dispatch-py/
-[signup]:  https://console.dispatch.run/
+[pypi]: https://pypi.org/project/dispatch-py/
+[signup]: https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
   - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
   - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
   - [Writing Dispatch Applications](#writing-dispatch-applications)
@@ -48,22 +48,23 @@
 brew tap dispatchrun/dispatch
 brew install dispatch
 ```
 
 Alternatively, you can download the latest `dispatch` binary from the
 [Releases](https://github.com/dispatchrun/dispatch/releases) page.
 
-*Note that this step is optional, applications that use Dispatch can run without
+_Note that this step is optional, applications that use Dispatch can run without
 the CLI, passing configuration through environment variables or directly in the
 code. However, the CLI automates the onboarding flow and simplifies the
-configuration, so we recommend starting with it.*
+configuration, so we recommend starting with it._
 
 ### Installing the Dispatch SDK
 
 The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+
 ```console
 pip install dispatch-py
 ```
 
 ## Usage
 
 ### Writing Dispatch Applications
@@ -89,27 +90,29 @@
 Obviously, this is just an example, a real application would perform much more
 interesting work, but it's a good start to get a sense of how to use Dispatch.
 
 ### Running Dispatch Applications
 
 The simplest way to run a Dispatch application is to use the Dispatch CLI, first
 we need to login:
+
 ```console
 dispatch login
 ```
 
 Then we are ready to run the example program we wrote above:
+
 ```console
 dispatch run -- python3 main.py
 ```
 
 ### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
-(a.k.a. *async* functions), in which case each `await` point becomes a
+(a.k.a. _async_ functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
 ```python
 @dispatch.function
 async def pipeline(msg):
@@ -149,18 +152,18 @@
     return await gather(*concurrent_calls)
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
-Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
+Dispatch converts Python coroutines to _Distributed Coroutines_, which can be
 suspended and resumed on any instance of a service across a fleet. For a deep
 dive on these concepts, read our blog post on
-[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://dispatch.run/blog/distributed-coroutines-in-python).
+[_Distributed Coroutines with a Native Python Extension and Dispatch_](https://dispatch.run/blog/distributed-coroutines-in-python).
 
 ### Integration with FastAPI
 
 Many web applications written in Python are developed using [FastAPI][fastapi].
 Dispatch can integrate with these applications by instantiating a
 `dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
 declared by the program can be invoked remotely over the same HTTP interface
```

### Comparing `dispatch_py-0.7.0/mkdocs.yml` & `dispatch_py-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/pyproject.toml` & `dispatch_py-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/expression_pb2.py` & `dispatch_py-0.7.1/src/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/expression_pb2.pyi` & `dispatch_py-0.7.1/src/buf/validate/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/priv/private_pb2.py` & `dispatch_py-0.7.1/src/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/priv/private_pb2.pyi` & `dispatch_py-0.7.1/src/buf/validate/priv/private_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/validate_pb2.py` & `dispatch_py-0.7.1/src/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/buf/validate/validate_pb2.pyi` & `dispatch_py-0.7.1/src/buf/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/__init__.py` & `dispatch_py-0.7.1/src/dispatch/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Callable, Coroutine, Optional, TypeVar, overload
 from urllib.parse import urlsplit
 
 from typing_extensions import ParamSpec, TypeAlias
 
 import dispatch.integrations
 from dispatch.coroutine import all, any, call, gather, race
-from dispatch.function import DEFAULT_API_URL, Client, Function, Registry, Reset
+from dispatch.function import DEFAULT_API_URL, Batch, Client, Function, Registry, Reset
 from dispatch.http import Dispatch
 from dispatch.id import DispatchID
 from dispatch.proto import Call, Error, Input, Output
 from dispatch.status import Status
 
 __all__ = [
     "Call",
@@ -92,7 +92,12 @@
     try:
         if init is not None:
             init(*args, **kwargs)
         server.serve_forever()
     finally:
         server.shutdown()
         server.server_close()
+
+
+def batch() -> Batch:
+    """Create a new batch object."""
+    return default_registry().batch()
```

### Comparing `dispatch_py-0.7.0/src/dispatch/coroutine.py` & `dispatch_py-0.7.1/src/dispatch/coroutine.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/error.py` & `dispatch_py-0.7.1/src/dispatch/error.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/__init__.py` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame.c` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame.c`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame.pyi` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame308.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame308.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame309.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame309.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame310.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame310.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame311.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame311.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame312.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame312.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/frame313.h` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/frame313.h`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/function.py` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/function.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/durable/registry.py` & `dispatch_py-0.7.1/src/dispatch/experimental/durable/registry.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/experimental/lambda_handler.py` & `dispatch_py-0.7.1/src/dispatch/experimental/lambda_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 
             api_url: The URL of the Dispatch API to use. Uses the value of the
                 DISPATCH_API_URL environment variable if set, otherwise
                 defaults to the public Dispatch API (DEFAULT_API_URL).
 
         """
 
-        super().__init__(endpoint="not configured", api_key=api_key, api_url=api_url)
+        # We use a fake endpoint to initialize the base class. The actual endpoint (the Lambda ARN)
+        # is only known when the handler is invoked.
+        super().__init__(endpoint="http://lambda", api_key=api_key, api_url=api_url)
 
     def handle(
         self, event: str, context: LambdaContext, entrypoint: Optional[str] = None
     ):
         # The ARN is not none until the first invocation of the Lambda function.
         # We override the endpoint of all registered functions before any execution.
         if context.invoked_function_arn:
```

### Comparing `dispatch_py-0.7.0/src/dispatch/fastapi.py` & `dispatch_py-0.7.1/src/dispatch/fastapi.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/function.py` & `dispatch_py-0.7.1/src/dispatch/function.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/http.py` & `dispatch_py-0.7.1/src/dispatch/http.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/integrations/http.py` & `dispatch_py-0.7.1/src/dispatch/integrations/http.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/integrations/httpx.py` & `dispatch_py-0.7.1/src/dispatch/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/integrations/openai.py` & `dispatch_py-0.7.1/src/dispatch/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/integrations/requests.py` & `dispatch_py-0.7.1/src/dispatch/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/integrations/slack.py` & `dispatch_py-0.7.1/src/dispatch/integrations/slack.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/proto.py` & `dispatch_py-0.7.1/src/dispatch/proto.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/scheduler.py` & `dispatch_py-0.7.1/src/dispatch/scheduler.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/call_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/call_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/call_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/call_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/dispatch_pb2_grpc.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/error_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/error_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/error_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/exit_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/exit_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/exit_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/exit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/function_pb2_grpc.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/function_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/poll_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/poll_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/poll_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/poll_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/status_pb2.py` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/status_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/sdk/v1/status_pb2.pyi` & `dispatch_py-0.7.1/src/dispatch/sdk/v1/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/signature/__init__.py` & `dispatch_py-0.7.1/src/dispatch/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/signature/digest.py` & `dispatch_py-0.7.1/src/dispatch/signature/digest.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/signature/key.py` & `dispatch_py-0.7.1/src/dispatch/signature/key.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/status.py` & `dispatch_py-0.7.1/src/dispatch/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import enum
-from typing import Any, Callable, Dict, Type
+from typing import Any, Callable, Dict, Type, Union
 
 from dispatch.sdk.v1 import status_pb2 as status_pb
 
 
 @enum.unique
 class Status(int, enum.Enum):
     """Enumeration of the possible values that can be used in the return status
@@ -74,24 +74,26 @@
 Status.UNAUTHENTICATED.__doc__ = "An operation was performed without authentication"
 Status.UNAUTHENTICATED._proto = status_pb.STATUS_UNAUTHENTICATED
 Status.PERMISSION_DENIED.__doc__ = "An operation was performed without permission"
 Status.PERMISSION_DENIED._proto = status_pb.STATUS_PERMISSION_DENIED
 Status.NOT_FOUND.__doc__ = "An operation was performed on a non-existent resource"
 Status.NOT_FOUND._proto = status_pb.STATUS_NOT_FOUND
 
-_ERROR_TYPES: Dict[Type[Exception], Callable[[Exception], Status]] = {}
-_OUTPUT_TYPES: Dict[Type[Any], Callable[[Any], Status]] = {}
+_ERROR_TYPES: Dict[Type[Exception], Union[Status, Callable[[Exception], Status]]] = {}
+_OUTPUT_TYPES: Dict[Type[Any], Union[Status, Callable[[Any], Status]]] = {}
 
 
 def status_for_error(error: BaseException) -> Status:
     """Returns a Status that corresponds to the specified error."""
     # See if the error matches one of the registered types.
-    handler = _find_handler(error, _ERROR_TYPES)
-    if handler is not None:
-        return handler(error)
+    status_or_handler = _find_status_or_handler(error, _ERROR_TYPES)
+    if status_or_handler is not None:
+        if isinstance(status_or_handler, Status):
+            return status_or_handler
+        return status_or_handler(error)
     # If not, resort to standard error categorization.
     #
     # See https://docs.python.org/3/library/exceptions.html
     if isinstance(error, TimeoutError):
         return Status.TIMEOUT
     elif isinstance(error, TypeError) or isinstance(error, ValueError):
         return Status.INVALID_ARGUMENT
@@ -116,36 +118,51 @@
         return Status.TEMPORARY_ERROR
     return Status.PERMANENT_ERROR
 
 
 def status_for_output(output: Any) -> Status:
     """Returns a Status that corresponds to the specified output value."""
     # See if the output value matches one of the registered types.
-    handler = _find_handler(output, _OUTPUT_TYPES)
-    if handler is not None:
-        return handler(output)
+    status_or_handler = _find_status_or_handler(output, _OUTPUT_TYPES)
+    if status_or_handler is not None:
+        if isinstance(status_or_handler, Status):
+            return status_or_handler
+        return status_or_handler(output)
 
     return Status.OK
 
 
 def register_error_type(
-    error_type: Type[Exception], handler: Callable[[Exception], Status]
+    error_type: Type[Exception],
+    status_or_handler: Union[Status, Callable[[Exception], Status]],
 ):
-    """Register an error type, and a handler which derives a Status from
-    errors of this type."""
-    _ERROR_TYPES[error_type] = handler
+    """Register an error type to Status mapping.
+
+    The caller can either register a base exception and a handler, which
+    derives a Status from errors of this type. Or, if there's only one
+    exception to Status mapping to register, the caller can simply pass
+    the exception class and the associated Status.
+    """
+    _ERROR_TYPES[error_type] = status_or_handler
 
 
-def register_output_type(output_type: Type[Any], handler: Callable[[Any], Status]):
-    """Register an output type, and a handler which derives a Status from
-    outputs of this type."""
-    _OUTPUT_TYPES[output_type] = handler
+def register_output_type(
+    output_type: Type[Any], status_or_handler: Union[Status, Callable[[Any], Status]]
+):
+    """Register an output type to Status mapping.
+
+    The caller can either register a base class and a handler, which
+    derives a Status from other classes of this type. Or, if there's
+    only one output class to Status mapping to register, the caller can
+    simply pass the class and the associated Status.
+    """
+    _OUTPUT_TYPES[output_type] = status_or_handler
 
 
-def _find_handler(obj, types):
+def _find_status_or_handler(obj, types):
     for cls in type(obj).__mro__:
         try:
             return types[cls]
         except KeyError:
             pass
 
     return None  # not found
```

### Comparing `dispatch_py-0.7.0/src/dispatch/test/client.py` & `dispatch_py-0.7.1/src/dispatch/test/client.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/test/server.py` & `dispatch_py-0.7.1/src/dispatch/test/server.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch/test/service.py` & `dispatch_py-0.7.1/src/dispatch/test/service.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch_py.egg-info/PKG-INFO` & `dispatch_py-0.7.1/src/dispatch_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
@@ -39,25 +39,25 @@
 
 <p align="center">
 <img src="https://github.com/dispatchrun/.github/blob/main/profile/dispatch_logo_light.png?raw=true" height="64"/>
 </p>
 
 # dispatch-py
 
-[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
-[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
-[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
+[![Docs](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/docs.yml)
+[![PyPI](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/pypi.yml)
+[![Test](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/dispatchrun/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[pypi]:    https://pypi.org/project/dispatch-py/
-[signup]:  https://console.dispatch.run/
+[pypi]: https://pypi.org/project/dispatch-py/
+[signup]: https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
   - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
   - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
   - [Writing Dispatch Applications](#writing-dispatch-applications)
@@ -87,22 +87,23 @@
 brew tap dispatchrun/dispatch
 brew install dispatch
 ```
 
 Alternatively, you can download the latest `dispatch` binary from the
 [Releases](https://github.com/dispatchrun/dispatch/releases) page.
 
-*Note that this step is optional, applications that use Dispatch can run without
+_Note that this step is optional, applications that use Dispatch can run without
 the CLI, passing configuration through environment variables or directly in the
 code. However, the CLI automates the onboarding flow and simplifies the
-configuration, so we recommend starting with it.*
+configuration, so we recommend starting with it._
 
 ### Installing the Dispatch SDK
 
 The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+
 ```console
 pip install dispatch-py
 ```
 
 ## Usage
 
 ### Writing Dispatch Applications
@@ -128,27 +129,29 @@
 Obviously, this is just an example, a real application would perform much more
 interesting work, but it's a good start to get a sense of how to use Dispatch.
 
 ### Running Dispatch Applications
 
 The simplest way to run a Dispatch application is to use the Dispatch CLI, first
 we need to login:
+
 ```console
 dispatch login
 ```
 
 Then we are ready to run the example program we wrote above:
+
 ```console
 dispatch run -- python3 main.py
 ```
 
 ### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
-(a.k.a. *async* functions), in which case each `await` point becomes a
+(a.k.a. _async_ functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
 ```python
 @dispatch.function
 async def pipeline(msg):
@@ -188,18 +191,18 @@
     return await gather(*concurrent_calls)
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
-Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
+Dispatch converts Python coroutines to _Distributed Coroutines_, which can be
 suspended and resumed on any instance of a service across a fleet. For a deep
 dive on these concepts, read our blog post on
-[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://dispatch.run/blog/distributed-coroutines-in-python).
+[_Distributed Coroutines with a Native Python Extension and Dispatch_](https://dispatch.run/blog/distributed-coroutines-in-python).
 
 ### Integration with FastAPI
 
 Many web applications written in Python are developed using [FastAPI][fastapi].
 Dispatch can integrate with these applications by instantiating a
 `dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
 declared by the program can be invoked remotely over the same HTTP interface
```

### Comparing `dispatch_py-0.7.0/src/dispatch_py.egg-info/SOURCES.txt` & `dispatch_py-0.7.1/src/dispatch_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/src/dispatch_py.egg-info/requires.txt` & `dispatch_py-0.7.1/src/dispatch_py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/tests/test_client.py` & `dispatch_py-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/tests/test_fastapi.py` & `dispatch_py-0.7.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `dispatch_py-0.7.0/tests/test_http.py` & `dispatch_py-0.7.1/tests/test_http.py`

 * *Files identical despite different names*

