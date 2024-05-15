# Comparing `tmp/x10_python_trading-0.1.2.tar.gz` & `tmp/x10_python_trading-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x10_python_trading-0.1.2.tar", max compression
+gzip compressed data, was "x10_python_trading-0.1.3.tar", max compression
```

## Comparing `x10_python_trading-0.1.2.tar` & `x10_python_trading-0.1.3.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0      794 2024-04-26 19:58:17.546355 x10_python_trading-0.1.2/README.md
--rw-r--r--   0        0        0     1541 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/__init__.py
--rw-r--r--   0        0        0     3945 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/README.md
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/fast_pedersen_hash.py
--rw-r--r--   0        0        0     3627 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/math_utils.py
--rw-r--r--   0        0        0     6074 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
--rw-r--r--   0        0        0   102708 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/pedersen_params.json
--rw-r--r--   0        0        0    11728 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/signature.py
--rw-r--r--   0        0        0     3759 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/assets_precomputed.json
--rw-r--r--   0        0        0    70705 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/constant_points.json
--rw-r--r--   0        0        0     3701 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/crypto/signature/src/config/keys_precomputed.json
--rw-r--r--   0        0        0     1955 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/BUILD
--rw-r--r--   0        0        0       31 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/CMakeLists.txt
--rw-r--r--   0        0        0     1254 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/CMakeLists_common.txt
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/__init__.py
--rw-r--r--   0        0        0     1522 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/async_subprocess.py
--rw-r--r--   0        0        0     5946 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/expression_string.py
--rw-r--r--   0        0        0     1883 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/expression_string_test.py
--rw-r--r--   0        0        0     3938 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/fixed_point.py
--rw-r--r--   0        0        0      675 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/BUILD
--rw-r--r--   0        0        0      359 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/CMakeLists.txt
--rw-r--r--   0        0        0      812 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/client.py
--rw-r--r--   0        0        0      681 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/json_rpc/client_test.py
--rw-r--r--   0        0        0     8881 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/math_utils.py
--rw-r--r--   0        0        0     5102 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/math_utils_test.py
--rw-r--r--   0        0        0     1614 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/merkle_tree.py
--rw-r--r--   0        0        0     1796 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/object_utils.py
--rw-r--r--   0        0        0     1545 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/python_dependencies.py
--rw-r--r--   0        0        0     6247 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/random_test.py
--rw-r--r--   0        0        0     6247 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/random_test_utils.py
--rw-r--r--   0        0        0     3460 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/test_utils.py
--rw-r--r--   0        0        0     2783 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/test_utils_test.py
--rw-r--r--   0        0        0    19817 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils.py
--rw-r--r--   0        0        0      599 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_stub_module.py
--rw-r--r--   0        0        0     1554 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_stub_module.pyi
--rw-r--r--   0        0        0     7959 2024-04-26 19:58:17.550356 x10_python_trading-0.1.2/starkware/python/utils_test.py
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/__init__.py
--rw-r--r--   0        0        0      413 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/config.py
--rw-r--r--   0        0        0       36 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/errors.py
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/__init__.py
--rw-r--r--   0        0        0     1492 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/accounts.py
--rw-r--r--   0        0        0     1618 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/amounts.py
--rw-r--r--   0        0        0     1120 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/assets.py
--rw-r--r--   0        0        0      347 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/balances.py
--rw-r--r--   0        0        0      327 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/fees.py
--rw-r--r--   0        0        0      459 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/funding_rates.py
--rw-r--r--   0        0        0     2702 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/markets.py
--rw-r--r--   0        0        0     5141 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/order_object.py
--rw-r--r--   0        0        0      739 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/orderbooks.py
--rw-r--r--   0        0        0     2207 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/orders.py
--rw-r--r--   0        0        0     1069 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/positions.py
--rw-r--r--   0        0        0       99 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/__init__.py
--rw-r--r--   0        0        0     2974 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/perpetual_stream_connection.py
--rw-r--r--   0        0        0     2497 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/stream_client/stream_client.py
--rw-r--r--   0        0        0     1241 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trades.py
--rw-r--r--   0        0        0      102 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/__init__.py
--rw-r--r--   0        0        0     4303 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/account_module.py
--rw-r--r--   0        0        0      636 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/base_module.py
--rw-r--r--   0        0        0     1499 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/markets_information_module.py
--rw-r--r--   0        0        0     2831 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/order_management_module.py
--rw-r--r--   0        0        0     1138 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/perpetual/trading_client/trading_client.py
--rw-r--r--   0        0        0        0 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/date.py
--rw-r--r--   0        0        0     5649 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/http.py
--rw-r--r--   0        0        0       79 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/log.py
--rw-r--r--   0        0        0     2336 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/model.py
--rw-r--r--   0        0        0    14980 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/starkex.py
--rw-r--r--   0        0        0      275 2024-04-26 19:58:17.554355 x10_python_trading-0.1.2/x10/utils/string.py
--rw-r--r--   0        0        0     1748 1970-01-01 00:00:00.000000 x10_python_trading-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5537 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/README.md
+-rw-r--r--   0        0        0     1541 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/__init__.py
+-rw-r--r--   0        0        0     3945 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/fast_pedersen_hash.py
+-rw-r--r--   0        0        0     3627 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/math_utils.py
+-rw-r--r--   0        0        0     6074 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
+-rw-r--r--   0        0        0   102708 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/pedersen_params.json
+-rw-r--r--   0        0        0    11728 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/signature.py
+-rw-r--r--   0        0        0     3759 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/assets_precomputed.json
+-rw-r--r--   0        0        0    70705 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/constant_points.json
+-rw-r--r--   0        0        0     3701 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/keys_precomputed.json
+-rw-r--r--   0        0        0     1955 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/BUILD
+-rw-r--r--   0        0        0       31 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/CMakeLists.txt
+-rw-r--r--   0        0        0     1254 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/CMakeLists_common.txt
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/async_subprocess.py
+-rw-r--r--   0        0        0     5946 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/expression_string.py
+-rw-r--r--   0        0        0     1883 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/expression_string_test.py
+-rw-r--r--   0        0        0     3938 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/fixed_point.py
+-rw-r--r--   0        0        0      675 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/BUILD
+-rw-r--r--   0        0        0      359 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/CMakeLists.txt
+-rw-r--r--   0        0        0      812 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/client.py
+-rw-r--r--   0        0        0      681 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/client_test.py
+-rw-r--r--   0        0        0     8881 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/math_utils.py
+-rw-r--r--   0        0        0     5102 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/math_utils_test.py
+-rw-r--r--   0        0        0     1614 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/merkle_tree.py
+-rw-r--r--   0        0        0     1796 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/object_utils.py
+-rw-r--r--   0        0        0     1545 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/python_dependencies.py
+-rw-r--r--   0        0        0     6247 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/random_test.py
+-rw-r--r--   0        0        0     6247 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/random_test_utils.py
+-rw-r--r--   0        0        0     3460 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/test_utils.py
+-rw-r--r--   0        0        0     2783 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/test_utils_test.py
+-rw-r--r--   0        0        0    19817 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils.py
+-rw-r--r--   0        0        0      599 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_stub_module.py
+-rw-r--r--   0        0        0     1554 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_stub_module.pyi
+-rw-r--r--   0        0        0     7959 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_test.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/config.py
+-rw-r--r--   0        0        0       36 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/errors.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/__init__.py
+-rw-r--r--   0        0        0     1575 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/accounts.py
+-rw-r--r--   0        0        0     1618 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/amounts.py
+-rw-r--r--   0        0        0     1120 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/assets.py
+-rw-r--r--   0        0        0      347 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/balances.py
+-rw-r--r--   0        0        0      427 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/configuration.py
+-rw-r--r--   0        0        0      327 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/fees.py
+-rw-r--r--   0        0        0      459 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/funding_rates.py
+-rw-r--r--   0        0        0     2744 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/markets.py
+-rw-r--r--   0        0        0     4461 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/order_object.py
+-rw-r--r--   0        0        0      739 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/orderbooks.py
+-rw-r--r--   0        0        0     2207 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/orders.py
+-rw-r--r--   0        0        0     1069 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/positions.py
+-rw-r--r--   0        0        0     4227 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/simple_client/simple_trading_client.py
+-rw-r--r--   0        0        0       99 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/__init__.py
+-rw-r--r--   0        0        0     2974 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/perpetual_stream_connection.py
+-rw-r--r--   0        0        0     2497 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/stream_client.py
+-rw-r--r--   0        0        0     1241 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trades.py
+-rw-r--r--   0        0        0      102 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/__init__.py
+-rw-r--r--   0        0        0     4996 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/account_module.py
+-rw-r--r--   0        0        0      636 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/base_module.py
+-rw-r--r--   0        0        0     1499 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/markets_information_module.py
+-rw-r--r--   0        0        0     2353 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/order_management_module.py
+-rw-r--r--   0        0        0     2953 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/trading_client.py
+-rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/date.py
+-rw-r--r--   0        0        0     5981 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/http.py
+-rw-r--r--   0        0        0       79 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/log.py
+-rw-r--r--   0        0        0     2336 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/model.py
+-rw-r--r--   0        0        0    14980 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/starkex.py
+-rw-r--r--   0        0        0      275 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/string.py
+-rw-r--r--   0        0        0     6491 1970-01-01 00:00:00.000000 x10_python_trading-0.1.3/PKG-INFO
```

### Comparing `x10_python_trading-0.1.2/pyproject.toml` & `x10_python_trading-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x10-python-trading"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for X10 API"
 authors = ["X10 <tech@ex10.org>"]
 packages = [
     { include = "starkware" },
     { include = "x10" },
 ]
 readme = "README.md"
```

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/README.md` & `x10_python_trading-0.1.3/starkware/crypto/signature/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/fast_pedersen_hash.py` & `x10_python_trading-0.1.3/starkware/crypto/signature/fast_pedersen_hash.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/math_utils.py` & `x10_python_trading-0.1.3/starkware/crypto/signature/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/nothing_up_my_sleeve_gen.py` & `x10_python_trading-0.1.3/starkware/crypto/signature/nothing_up_my_sleeve_gen.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/pedersen_params.json` & `x10_python_trading-0.1.3/starkware/crypto/signature/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/signature.py` & `x10_python_trading-0.1.3/starkware/crypto/signature/signature.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/assets_precomputed.json` & `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/assets_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/constant_points.json` & `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/constant_points.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/crypto/signature/src/config/keys_precomputed.json` & `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/keys_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/BUILD` & `x10_python_trading-0.1.3/starkware/python/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/CMakeLists_common.txt` & `x10_python_trading-0.1.3/starkware/python/CMakeLists_common.txt`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/async_subprocess.py` & `x10_python_trading-0.1.3/starkware/python/async_subprocess.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/expression_string.py` & `x10_python_trading-0.1.3/starkware/python/expression_string.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/expression_string_test.py` & `x10_python_trading-0.1.3/starkware/python/expression_string_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/fixed_point.py` & `x10_python_trading-0.1.3/starkware/python/fixed_point.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/json_rpc/BUILD` & `x10_python_trading-0.1.3/starkware/python/json_rpc/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/json_rpc/client.py` & `x10_python_trading-0.1.3/starkware/python/json_rpc/client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/json_rpc/client_test.py` & `x10_python_trading-0.1.3/starkware/python/json_rpc/client_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/math_utils.py` & `x10_python_trading-0.1.3/starkware/python/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/math_utils_test.py` & `x10_python_trading-0.1.3/starkware/python/math_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/merkle_tree.py` & `x10_python_trading-0.1.3/starkware/python/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/object_utils.py` & `x10_python_trading-0.1.3/starkware/python/object_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/python_dependencies.py` & `x10_python_trading-0.1.3/starkware/python/python_dependencies.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/random_test.py` & `x10_python_trading-0.1.3/starkware/python/random_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/random_test_utils.py` & `x10_python_trading-0.1.3/starkware/python/random_test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/test_utils.py` & `x10_python_trading-0.1.3/starkware/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/test_utils_test.py` & `x10_python_trading-0.1.3/starkware/python/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/utils.py` & `x10_python_trading-0.1.3/starkware/python/utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/utils_stub_module.py` & `x10_python_trading-0.1.3/starkware/python/utils_stub_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/utils_stub_module.pyi` & `x10_python_trading-0.1.3/starkware/python/utils_stub_module.pyi`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/starkware/python/utils_test.py` & `x10_python_trading-0.1.3/starkware/python/utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/accounts.py` & `x10_python_trading-0.1.3/x10/perpetual/accounts.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,33 +12,37 @@
 
 class StarkPerpetualAccount:
     __vault: int
     __private_key: int
     __public_key: int
     __trading_fee: Dict[str, TradingFeeModel]
 
-    def __init__(self, *, vault: int, private_key: str, public_key: str):
-        assert vault > 10000
+    def __init__(self, vault: int, private_key: str, public_key: str, api_key: str):
         assert is_hex_string(private_key)
         assert is_hex_string(public_key)
 
         self.__vault = vault
         self.__private_key = int(private_key, base=16)
         self.__public_key = int(public_key, base=16)
+        self.__api_key = api_key
         self.__trading_fee = {}
 
     @property
     def vault(self):
         return self.__vault
 
     @property
     def public_key(self):
         return self.__public_key
 
     @property
+    def api_key(self):
+        return self.__api_key
+
+    @property
     def trading_fee(self):
         return self.__trading_fee
 
     def sign(self, msg_hash: int) -> Tuple[int, int]:
         return sign(private_key=self.__private_key, msg_hash=msg_hash)
```

### Comparing `x10_python_trading-0.1.2/x10/perpetual/amounts.py` & `x10_python_trading-0.1.3/x10/perpetual/amounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/assets.py` & `x10_python_trading-0.1.3/x10/perpetual/assets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/markets.py` & `x10_python_trading-0.1.3/x10/perpetual/markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,19 @@
     max_position_value: Decimal
     max_leverage: Decimal
     max_num_orders: int
     limit_price_cap: Decimal
     limit_price_floor: Decimal
     risk_factor_config: List[RiskFactorConfig]
 
+    @cached_property
     def price_precision(self) -> int:
         return abs(int(self.min_price_change.log10().to_integral_exact(ROUND_CEILING)))
 
+    @cached_property
     def quantity_precision(self) -> int:
         return abs(int(self.min_order_size_change.log10().to_integral_exact(ROUND_CEILING)))
 
 
 class L2ConfigModel(X10BaseModel):
     type: str
     collateral_id: str
```

### Comparing `x10_python_trading-0.1.2/x10/perpetual/order_object.py` & `x10_python_trading-0.1.3/x10/perpetual/order_object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import asyncio
-from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from decimal import Decimal
 from typing import Callable, Tuple
 
 from x10.perpetual.accounts import StarkPerpetualAccount
 from x10.perpetual.amounts import (
     ROUNDING_BUY_CONTEXT,
@@ -22,83 +20,58 @@
     StarkDebuggingOrderAmountsModel,
     StarkSettlementModel,
     TimeInForce,
 )
 from x10.utils.date import to_epoch_millis, utc_now
 from x10.utils.starkex import generate_nonce, hash_order
 
-order_executor = ThreadPoolExecutor(thread_name_prefix="order_builder")
 
-
-async def create_order_object(
-    account: StarkPerpetualAccount,
-    market: MarketModel,
-    amount_of_synthetic: Decimal,
-    price: Decimal,
-    side: OrderSide,
-) -> PerpetualOrderModel:
-    """
-    Creates an order object to be placed on the exchange using the `place_order` method.
-    """
-    expire_time = utc_now() + timedelta(days=7)
-    fees = account.trading_fee.get(market.name, DEFAULT_FEES)
-    pool = asyncio.get_event_loop()
-    return await pool.run_in_executor(
-        order_executor,
-        __create_order_object,
-        market,
-        amount_of_synthetic,
-        price,
-        side,
-        account.vault,
-        fees,
-        account.sign,
-        account.public_key,
-        False,
-        expire_time,
-    )
-
-
-def create_order_object_sync(
+def create_order_object(
     account: StarkPerpetualAccount,
     market: MarketModel,
     amount_of_synthetic: Decimal,
     price: Decimal,
     side: OrderSide,
+    post_only: bool = False,
+    previous_order_id=None,
+    expire_time=utc_now() + timedelta(hours=8),
 ) -> PerpetualOrderModel:
     """
     Creates an order object to be placed on the exchange using the `place_order` method.
     """
-    expire_time = utc_now() + timedelta(days=7)
     fees = account.trading_fee.get(market.name, DEFAULT_FEES)
     return __create_order_object(
         market,
         amount_of_synthetic,
         price,
         side,
         account.vault,
         fees,
         account.sign,
         account.public_key,
         False,
         expire_time,
+        post_only=post_only,
+        previous_order_id=previous_order_id,
     )
 
 
 def __create_order_object(
     market: MarketModel,
     synthetic_amount: Decimal,
     price: Decimal,
     side: OrderSide,
     collateral_position_id: int,
     fees: TradingFeeModel,
     signer: Callable[[int], Tuple[int, int]],
     public_key: int,
     exact_only: bool = False,
-    expire_time: datetime = utc_now() + timedelta(days=7),
+    expire_time: datetime = utc_now() + timedelta(hours=8),
+    post_only: bool = False,
+    previous_order_id=None,
 ) -> PerpetualOrderModel:
     if exact_only:
         raise NotImplementedError("`exact_only` option is not supported yet")
 
     nonce = generate_nonce()
     is_buying_synthetic = side == OrderSide.BUY
     rounding_context = ROUNDING_BUY_CONTEXT if is_buying_synthetic else ROUNDING_SELL_CONTEXT
@@ -133,27 +106,27 @@
         id=str(order_hash),
         market=market.name,
         type=OrderType.LIMIT,
         side=side,
         qty=synthetic_amount_human.value,
         price=price,
         reduce_only=False,
-        post_only=False,
+        post_only=post_only,
         time_in_force=TimeInForce.GTT,
         fee=amounts.fee_rate,
         expiry_epoch_millis=to_epoch_millis(expire_time),
         settlement=StarkSettlementModel(
             signature=SignatureModel(r=order_signature_r, s=order_signature_s),
             stark_key=public_key,
             collateral_position=Decimal(collateral_position_id),
         ),
         nonce=Decimal(nonce),
         take_profit_signature=None,
         stop_loss_signature=None,
-        cancel_id=None,
+        cancel_id=previous_order_id,
         trigger_price=None,
         take_profit_price=None,
         take_profit_limit_price=None,
         stop_loss_price=None,
         stop_loss_limit_price=None,
         debugging_amounts=StarkDebuggingOrderAmountsModel(
             collateral_amount=Decimal(
```

### Comparing `x10_python_trading-0.1.2/x10/perpetual/orderbooks.py` & `x10_python_trading-0.1.3/x10/perpetual/orderbooks.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/orders.py` & `x10_python_trading-0.1.3/x10/perpetual/orders.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/positions.py` & `x10_python_trading-0.1.3/x10/perpetual/positions.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/stream_client/perpetual_stream_connection.py` & `x10_python_trading-0.1.3/x10/perpetual/stream_client/perpetual_stream_connection.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/stream_client/stream_client.py` & `x10_python_trading-0.1.3/x10/perpetual/stream_client/stream_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/trades.py` & `x10_python_trading-0.1.3/x10/perpetual/trades.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/trading_client/account_module.py` & `x10_python_trading-0.1.3/x10/perpetual/trading_client/account_module.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,105 +4,123 @@
 from x10.perpetual.accounts import AccountLeverage
 from x10.perpetual.balances import BalanceModel
 from x10.perpetual.fees import TradingFeeModel
 from x10.perpetual.orders import OpenOrderModel, OrderSide, OrderType
 from x10.perpetual.positions import PositionHistoryModel, PositionModel, PositionSide
 from x10.perpetual.trades import AccountTradeModel, TradeType
 from x10.perpetual.trading_client.base_module import BaseModule
-from x10.utils.http import send_get_request, send_patch_request
+from x10.utils.http import WrappedApiResponse, send_get_request, send_patch_request
 from x10.utils.model import EmptyModel
 
 
 class AccountModule(BaseModule):
-    def get_balance(self):
+    async def get_balance(self) -> WrappedApiResponse[BalanceModel]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-balance
         """
 
         url = self._get_url("/user/balance")
-        return send_get_request(url, BalanceModel, api_key=self._get_api_key())
+        return await send_get_request(url, BalanceModel, api_key=self._get_api_key())
 
-    def get_positions(self, *, market_names: Optional[List[str]] = None, position_side: Optional[PositionSide] = None):
+    async def get_positions(
+        self, *, market_names: Optional[List[str]] = None, position_side: Optional[PositionSide] = None
+    ) -> WrappedApiResponse[List[PositionModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-positions
         """
 
         url = self._get_url("/user/positions", query={"market": market_names, "side": position_side})
-        return send_get_request(url, List[PositionModel], api_key=self._get_api_key())
+        return await send_get_request(url, List[PositionModel], api_key=self._get_api_key())
 
-    def get_positions_history(
-        self, *, market_names: Optional[List[str]] = None, position_side: Optional[PositionSide] = None
-    ):
+    async def get_positions_history(
+        self,
+        market_names: Optional[List[str]] = None,
+        position_side: Optional[PositionSide] = None,
+    ) -> WrappedApiResponse[List[PositionHistoryModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-positions-history
         """
 
-        url = self._get_url("/user/positions/history", query={"market": market_names, "side": position_side})
-        return send_get_request(url, List[PositionHistoryModel], api_key=self._get_api_key())
+        url = self._get_url(
+            "/user/positions/history",
+            query={"market": market_names, "side": position_side},
+        )
+        return await send_get_request(url, List[PositionHistoryModel], api_key=self._get_api_key())
 
-    def get_open_orders(
+    async def get_open_orders(
         self,
-        *,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
         order_side: Optional[OrderSide] = None,
-    ):
+    ) -> WrappedApiResponse[List[OpenOrderModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-open-orders
         """
 
-        url = self._get_url("/user/orders", query={"market": market_names, "type": order_type, "side": order_side})
-        return send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
+        url = self._get_url(
+            "/user/orders",
+            query={"market": market_names, "type": order_type, "side": order_side},
+        )
+        return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
 
-    def get_orders_history(
+    async def get_orders_history(
         self,
-        *,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
         order_side: Optional[OrderSide] = None,
-    ):
+    ) -> WrappedApiResponse[List[OpenOrderModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-orders-history
         """
 
         url = self._get_url(
-            "/user/orders/history", query={"market": market_names, "type": order_type, "side": order_side}
+            "/user/orders/history",
+            query={"market": market_names, "type": order_type, "side": order_side},
         )
-        return send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
+        return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
 
-    def get_trades(
-        self, *, market_names: List[str], trade_side: Optional[OrderSide] = None, trade_type: Optional[TradeType] = None
-    ):
+    async def get_trades(
+        self,
+        market_names: List[str],
+        trade_side: Optional[OrderSide] = None,
+        trade_type: Optional[TradeType] = None,
+    ) -> WrappedApiResponse[List[AccountTradeModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-trades
         """
 
-        url = self._get_url("/user/trades", query={"market": market_names, "side": trade_side, "type": trade_type})
+        url = self._get_url(
+            "/user/trades",
+            query={"market": market_names, "side": trade_side, "type": trade_type},
+        )
 
-        return send_get_request(url, List[AccountTradeModel], api_key=self._get_api_key())
+        return await send_get_request(url, List[AccountTradeModel], api_key=self._get_api_key())
 
-    def get_fees(self, *, market_names: List[str]):
+    async def get_fees(self, *, market_names: List[str]) -> WrappedApiResponse[List[TradingFeeModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-fees
         """
 
         url = self._get_url("/user/fees", query={"market": market_names})
-        return send_get_request(url, List[TradingFeeModel], api_key=self._get_api_key())
+        return await send_get_request(url, List[TradingFeeModel], api_key=self._get_api_key())
 
-    def get_leverage(self, *, market_names: List[str]):
+    async def get_leverage(self, market_names: List[str]) -> WrappedApiResponse[List[AccountLeverage]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-current-leverage
         """
 
         url = self._get_url("/user/leverage", query={"market": market_names})
-        return send_get_request(url, List[AccountLeverage], api_key=self._get_api_key())
+        return await send_get_request(url, List[AccountLeverage], api_key=self._get_api_key())
 
-    def update_leverage(self, *, market_name: str, leverage: Decimal):
+    async def update_leverage(self, market_name: str, leverage: Decimal) -> WrappedApiResponse[EmptyModel]:
         """
         https://x101.docs.apiary.io/#reference/0/account/update-leverage
         """
 
         url = self._get_url("/user/leverage")
         request_model = AccountLeverage(market=market_name, leverage=leverage)
-        return send_patch_request(
-            url, EmptyModel, json=request_model.to_api_request_json(), api_key=self._get_api_key()
+        return await send_patch_request(
+            url,
+            EmptyModel,
+            json=request_model.to_api_request_json(),
+            api_key=self._get_api_key(),
         )
```

### Comparing `x10_python_trading-0.1.2/x10/perpetual/trading_client/base_module.py` & `x10_python_trading-0.1.3/x10/perpetual/trading_client/base_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/trading_client/markets_information_module.py` & `x10_python_trading-0.1.3/x10/perpetual/trading_client/markets_information_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/perpetual/trading_client/order_management_module.py` & `x10_python_trading-0.1.3/x10/perpetual/trading_client/order_management_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from decimal import Decimal
 from typing import Optional
 
-from x10.perpetual.accounts import StarkPerpetualAccount
-from x10.perpetual.markets import MarketModel
-from x10.perpetual.order_object import create_order_object
-from x10.perpetual.orders import OrderSide, PerpetualOrderModel, PlacedOrderModel
+from x10.perpetual.orders import PerpetualOrderModel, PlacedOrderModel
 from x10.perpetual.trading_client.base_module import BaseModule
 from x10.utils.http import send_delete_request, send_post_request
 from x10.utils.log import get_logger
 from x10.utils.model import EmptyModel, X10BaseModel
 
 LOGGER = get_logger(__name__)
 
@@ -17,53 +13,42 @@
     order_ids: Optional[list[int]]
     external_order_ids: Optional[list[str]]
     market_ids: Optional[list[int]]
     cancel_all: Optional[bool]
 
 
 class OrderManagementModule(BaseModule):
-    @staticmethod
-    async def create_order_object(
-        *,
-        account: StarkPerpetualAccount,
-        market: MarketModel,
-        amount_of_synthetic: Decimal,
-        price: Decimal,
-        side: OrderSide,
-    ):
-        return await create_order_object(
-            account=account,
-            market=market,
-            amount_of_synthetic=amount_of_synthetic,
-            price=price,
-            side=side,
-        )
-
-    def place_order(self, order: PerpetualOrderModel):
+    async def place_order(self, order: PerpetualOrderModel):
         """
         Placed new order on the exchange.
 
         :param order: Order object created by `create_order_object` method.
 
         https://x101.docs.apiary.io/#reference/0/order-managment/create-order
         """
         LOGGER.debug("Placing an order: id=%s", order.id)
 
         url = self._get_url("/user/order")
-        return send_post_request(url, PlacedOrderModel, json=order.to_api_request_json(), api_key=self._get_api_key())
+        response = await send_post_request(
+            url,
+            PlacedOrderModel,
+            json=order.to_api_request_json(),
+            api_key=self._get_api_key(),
+        )
+        return response
 
-    def cancel_order(self, order_id: int):
+    async def cancel_order(self, order_id: int):
         """
         https://x101.docs.apiary.io/#reference/0/order-managment/cancel-order
         """
 
         url = self._get_url("/user/order/<order_id>", order_id=order_id)
-        return send_delete_request(url, EmptyModel, api_key=self._get_api_key(), idempotent=True, retry=True)
+        return await send_delete_request(url, EmptyModel, api_key=self._get_api_key(), idempotent=True, retry=True)
 
-    def mass_cancel(
+    async def mass_cancel(
         self,
         *,
         order_ids: Optional[list[int]] = None,
         external_order_ids: Optional[list[str]] = None,
         market_ids: Optional[list[int]] = None,
         cancel_all: Optional[bool] = False,
     ):
@@ -74,10 +59,13 @@
         url = self._get_url("/user/order/massCancel")
         request_model = _MassCancelRequestModel(
             order_ids=order_ids,
             external_order_ids=external_order_ids,
             market_ids=market_ids,
             cancel_all=cancel_all,
         )
-        return send_post_request(
-            url, EmptyModel, json=request_model.to_api_request_json(exclude_none=True), api_key=self._get_api_key()
+        return await send_post_request(
+            url,
+            EmptyModel,
+            json=request_model.to_api_request_json(exclude_none=True),
+            api_key=self._get_api_key(),
         )
```

### Comparing `x10_python_trading-0.1.2/x10/utils/http.py` & `x10_python_trading-0.1.3/x10/utils/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -118,15 +118,19 @@
     headers = __get_headers(api_key=api_key)
 
     LOGGER.debug("Sending POST %s, headers=%s, data=%s", url, headers, {})
 
     async with aiohttp.ClientSession(timeout=CLIENT_TIMEOUT) as session:
         async with session.post(url, json=json, headers=headers) as response:
             response_text = await response.text()
-            return parse_response_to_model(response_text, model_class)
+            response_model = parse_response_to_model(response_text, model_class)
+            if (response_model.status != ResponseStatus.OK.value) or (response_model.error is not None):
+                LOGGER.error("Error response from POST %s: %s", url, response_model.error)
+                raise ValueError(f"Error response from POST {url}: {response_model.error}")
+            return response_model
 
 
 async def send_patch_request(
     url: str, model_class: Type[ApiResponseType], *, json: Any = None, api_key: Optional[str] = None
 ) -> WrappedApiResponse[ApiResponseType]:
     headers = __get_headers(api_key=api_key)
```

### Comparing `x10_python_trading-0.1.2/x10/utils/model.py` & `x10_python_trading-0.1.3/x10/utils/model.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.2/x10/utils/starkex.py` & `x10_python_trading-0.1.3/x10/utils/starkex.py`

 * *Files identical despite different names*

