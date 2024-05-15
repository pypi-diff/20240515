# Comparing `tmp/stellar_sdk-9.3.0.tar.gz` & `tmp/stellar_sdk-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar_sdk-9.3.0.tar", max compression
+gzip compressed data, was "stellar_sdk-9.4.0.tar", max compression
```

## Comparing `stellar_sdk-9.3.0.tar` & `stellar_sdk-9.4.0.tar`

### file list

```diff
@@ -1,572 +1,579 @@
--rw-r--r--   0        0        0    11357 2024-03-13 03:08:49.303457 stellar_sdk-9.3.0/LICENSE
--rw-r--r--   0        0        0     4635 2024-03-13 03:08:49.303457 stellar_sdk-9.3.0/README.rst
--rw-r--r--   0        0        0     3096 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/pyproject.toml
--rw-r--r--   0        0        0     1200 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/__init__.py
--rw-r--r--   0        0        0      876 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/__version__.py
--rw-r--r--   0        0        0     4736 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/account.py
--rw-r--r--   0        0        0     5223 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/address.py
--rw-r--r--   0        0        0    10156 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/asset.py
--rw-r--r--   0        0        0     6602 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/auth.py
--rw-r--r--   0        0        0    13620 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/base_server.py
--rw-r--r--   0        0        0     1931 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/base_soroban_server.py
--rw-r--r--   0        0        0     5629 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/base_transaction_envelope.py
--rw-r--r--   0        0        0        0 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/__init__.py
--rw-r--r--   0        0        0      824 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/__init__.py
--rw-r--r--   0        0        0     3349 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py
--rw-r--r--   0        0        0     1452 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_assets_call_builder.py
--rw-r--r--   0        0        0     4738 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_call_builder.py
--rw-r--r--   0        0        0     2722 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py
--rw-r--r--   0        0        0      738 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_data_call_builder.py
--rw-r--r--   0        0        0     3219 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_effects_call_builder.py
--rw-r--r--   0        0        0      537 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py
--rw-r--r--   0        0        0      959 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py
--rw-r--r--   0        0        0     2104 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py
--rw-r--r--   0        0        0     4182 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_offers_call_builder.py
--rw-r--r--   0        0        0     4563 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_operations_call_builder.py
--rw-r--r--   0        0        0     1088 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py
--rw-r--r--   0        0        0     2811 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_payments_call_builder.py
--rw-r--r--   0        0        0      378 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_root_call_builder.py
--rw-r--r--   0        0        0     2766 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2517 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     3143 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py
--rw-r--r--   0        0        0     3217 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_trades_call_builder.py
--rw-r--r--   0        0        0     3674 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py
--rw-r--r--   0        0        0      734 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/__init__.py
--rw-r--r--   0        0        0      870 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py
--rw-r--r--   0        0        0      997 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py
--rw-r--r--   0        0        0     4317 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py
--rw-r--r--   0        0        0     1077 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py
--rw-r--r--   0        0        0     1158 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py
--rw-r--r--   0        0        0      840 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py
--rw-r--r--   0        0        0     1005 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py
--rw-r--r--   0        0        0      840 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py
--rw-r--r--   0        0        0     1039 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py
--rw-r--r--   0        0        0      832 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py
--rw-r--r--   0        0        0      859 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py
--rw-r--r--   0        0        0     1081 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py
--rw-r--r--   0        0        0      859 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py
--rw-r--r--   0        0        0      874 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py
--rw-r--r--   0        0        0     2718 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2487 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     2292 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py
--rw-r--r--   0        0        0      832 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py
--rw-r--r--   0        0        0      880 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py
--rw-r--r--   0        0        0      734 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/__init__.py
--rw-r--r--   0        0        0      861 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py
--rw-r--r--   0        0        0      982 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py
--rw-r--r--   0        0        0     4119 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py
--rw-r--r--   0        0        0     1062 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py
--rw-r--r--   0        0        0     1175 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py
--rw-r--r--   0        0        0      831 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py
--rw-r--r--   0        0        0      990 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py
--rw-r--r--   0        0        0      831 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py
--rw-r--r--   0        0        0     1024 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py
--rw-r--r--   0        0        0      823 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py
--rw-r--r--   0        0        0      850 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py
--rw-r--r--   0        0        0     1072 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py
--rw-r--r--   0        0        0      850 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py
--rw-r--r--   0        0        0      859 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py
--rw-r--r--   0        0        0     2729 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2498 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     2303 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py
--rw-r--r--   0        0        0      823 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py
--rw-r--r--   0        0        0      871 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py
--rw-r--r--   0        0        0        0 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/__init__.py
--rw-r--r--   0        0        0     9952 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/aiohttp_client.py
--rw-r--r--   0        0        0     2007 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/base_async_client.py
--rw-r--r--   0        0        0     1850 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/base_sync_client.py
--rw-r--r--   0        0        0      445 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/defines.py
--rw-r--r--   0        0        0     8147 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/requests_client.py
--rw-r--r--   0        0        0     1383 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/response.py
--rw-r--r--   0        0        0     2756 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/client/simple_requests_client.py
--rw-r--r--   0        0        0     1919 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/decorated_signature.py
--rw-r--r--   0        0        0     5722 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/exceptions.py
--rw-r--r--   0        0        0     5533 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/fee_bump_transaction.py
--rw-r--r--   0        0        0     5678 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/fee_bump_transaction_envelope.py
--rw-r--r--   0        0        0     1997 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/helpers.py
--rw-r--r--   0        0        0    12145 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/keypair.py
--rw-r--r--   0        0        0     2343 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/ledger_bounds.py
--rw-r--r--   0        0        0     6056 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/liquidity_pool_asset.py
--rw-r--r--   0        0        0     2241 2024-03-13 03:08:49.307457 stellar_sdk-9.3.0/stellar_sdk/liquidity_pool_id.py
--rw-r--r--   0        0        0     9317 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/memo.py
--rw-r--r--   0        0        0     6161 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/muxed_account.py
--rw-r--r--   0        0        0     2183 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/network.py
--rw-r--r--   0        0        0      950 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/__init__.py
--rw-r--r--   0        0        0     2087 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/account_merge.py
--rw-r--r--   0        0        0     6259 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/allow_trust.py
--rw-r--r--   0        0        0     2890 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py
--rw-r--r--   0        0        0     2163 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/bump_sequence.py
--rw-r--r--   0        0        0     3157 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/change_trust.py
--rw-r--r--   0        0        0     2529 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/claim_claimable_balance.py
--rw-r--r--   0        0        0     2679 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/clawback.py
--rw-r--r--   0        0        0     2510 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/clawback_claimable_balance.py
--rw-r--r--   0        0        0     3271 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/create_account.py
--rw-r--r--   0        0        0    17123 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/create_claimable_balance.py
--rw-r--r--   0        0        0     4357 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/create_passive_sell_offer.py
--rw-r--r--   0        0        0     1737 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/end_sponsoring_future_reserves.py
--rw-r--r--   0        0        0     2228 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/extend_footprint_ttl.py
--rw-r--r--   0        0        0     1212 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/inflation.py
--rw-r--r--   0        0        0     2398 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/invoke_host_function.py
--rw-r--r--   0        0        0     4741 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/liquidity_pool_deposit.py
--rw-r--r--   0        0        0     4147 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/liquidity_pool_withdraw.py
--rw-r--r--   0        0        0     3881 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/manage_buy_offer.py
--rw-r--r--   0        0        0     3355 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/manage_data.py
--rw-r--r--   0        0        0     3892 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/manage_sell_offer.py
--rw-r--r--   0        0        0     4975 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/operation.py
--rw-r--r--   0        0        0     5013 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/path_payment_strict_receive.py
--rw-r--r--   0        0        0     4947 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/path_payment_strict_send.py
--rw-r--r--   0        0        0     2783 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/payment.py
--rw-r--r--   0        0        0     1519 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/restore_footprint.py
--rw-r--r--   0        0        0    24387 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/revoke_sponsorship.py
--rw-r--r--   0        0        0    10477 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/set_options.py
--rw-r--r--   0        0        0     4633 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/operation/set_trust_line_flags.py
--rw-r--r--   0        0        0     8741 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/preconditions.py
--rw-r--r--   0        0        0     2934 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/price.py
--rw-r--r--   0        0        0        0 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/py.typed
--rw-r--r--   0        0        0    27303 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/scval.py
--rw-r--r--   0        0        0        0 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/__init__.py
--rw-r--r--   0        0        0      827 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/ed25519_public_key_signer.py
--rw-r--r--   0        0        0     1550 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/exceptions.py
--rw-r--r--   0        0        0     9256 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/federation.py
--rw-r--r--   0        0        0     3118 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/mnemonic.py
--rw-r--r--   0        0        0     3071 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/stellar_toml.py
--rw-r--r--   0        0        0    20271 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/stellar_uri.py
--rw-r--r--   0        0        0    27857 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/stellar_web_authentication.py
--rw-r--r--   0        0        0     5328 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/toid.py
--rw-r--r--   0        0        0    71955 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/sep/txrep.py
--rw-r--r--   0        0        0    15397 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/server.py
--rw-r--r--   0        0        0    15574 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/server_async.py
--rw-r--r--   0        0        0     4148 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/signer.py
--rw-r--r--   0        0        0    11311 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/signer_key.py
--rw-r--r--   0        0        0     3954 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/soroban_data_builder.py
--rw-r--r--   0        0        0    10979 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/soroban_rpc.py
--rw-r--r--   0        0        0    16766 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/soroban_server.py
--rw-r--r--   0        0        0    16970 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/soroban_server_async.py
--rw-r--r--   0        0        0    13325 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/strkey.py
--rw-r--r--   0        0        0     2557 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/time_bounds.py
--rw-r--r--   0        0        0    12383 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/transaction.py
--rw-r--r--   0        0        0    66516 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/transaction_builder.py
--rw-r--r--   0        0        0     7388 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/transaction_envelope.py
--rw-r--r--   0        0        0     5943 2024-03-13 03:08:49.311457 stellar_sdk-9.3.0/stellar_sdk/utils.py
--rw-r--r--   0        0        0    15238 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/__init__.py
--rw-r--r--   0        0        0     6433 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry.py
--rw-r--r--   0        0        0     2338 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_ext.py
--rw-r--r--   0        0        0     2375 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v1.py
--rw-r--r--   0        0        0     2404 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     4035 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v2.py
--rw-r--r--   0        0        0     2404 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py
--rw-r--r--   0        0        0     2806 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v3.py
--rw-r--r--   0        0        0     2007 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_flags.py
--rw-r--r--   0        0        0     1529 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_id.py
--rw-r--r--   0        0        0     4475 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_merge_result.py
--rw-r--r--   0        0        0     2278 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/account_merge_result_code.py
--rw-r--r--   0        0        0     2513 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_op.py
--rw-r--r--   0        0        0     3331 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_result.py
--rw-r--r--   0        0        0     2199 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_result_code.py
--rw-r--r--   0        0        0     2081 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/alpha_num12.py
--rw-r--r--   0        0        0     2069 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/alpha_num4.py
--rw-r--r--   0        0        0     3494 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/asset.py
--rw-r--r--   0        0        0     3345 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code.py
--rw-r--r--   0        0        0     1578 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code12.py
--rw-r--r--   0        0        0     1557 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code4.py
--rw-r--r--   0        0        0     1400 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/asset_type.py
--rw-r--r--   0        0        0     1578 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/auth.py
--rw-r--r--   0        0        0     2407 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/auth_cert.py
--rw-r--r--   0        0        0     2353 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/authenticated_message.py
--rw-r--r--   0        0        0     2500 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/authenticated_message_v0.py
--rw-r--r--   0        0        0     6626 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/base.py
--rw-r--r--   0        0        0     1870 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
--rw-r--r--   0        0        0     3567 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
--rw-r--r--   0        0        0     1875 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
--rw-r--r--   0        0        0     4356 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_entry.py
--rw-r--r--   0        0        0     1561 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_entry_type.py
--rw-r--r--   0        0        0     2344 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_metadata.py
--rw-r--r--   0        0        0     1708 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_metadata_ext.py
--rw-r--r--   0        0        0     1711 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_op.py
--rw-r--r--   0        0        0     2197 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_result.py
--rw-r--r--   0        0        0     1483 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_result_code.py
--rw-r--r--   0        0        0     4470 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_asset.py
--rw-r--r--   0        0        0     2078 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_op.py
--rw-r--r--   0        0        0     3930 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_result.py
--rw-r--r--   0        0        0     2461 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_result_code.py
--rw-r--r--   0        0        0     4050 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_atom.py
--rw-r--r--   0        0        0     1359 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_atom_type.py
--rw-r--r--   0        0        0     1834 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_op.py
--rw-r--r--   0        0        0     3808 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_result.py
--rw-r--r--   0        0        0     1826 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py
--rw-r--r--   0        0        0     3491 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_liquidity_atom.py
--rw-r--r--   0        0        0     3766 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_offer_atom.py
--rw-r--r--   0        0        0     3834 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_offer_atom_v0.py
--rw-r--r--   0        0        0     7471 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_predicate.py
--rw-r--r--   0        0        0     1636 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claim_predicate_type.py
--rw-r--r--   0        0        0     4122 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry.py
--rw-r--r--   0        0        0     2438 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_ext.py
--rw-r--r--   0        0        0     2346 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
--rw-r--r--   0        0        0     1816 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     1420 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_flags.py
--rw-r--r--   0        0        0     2388 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_id.py
--rw-r--r--   0        0        0     1267 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_id_type.py
--rw-r--r--   0        0        0     2426 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimant.py
--rw-r--r--   0        0        0     1183 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimant_type.py
--rw-r--r--   0        0        0     2257 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/claimant_v0.py
--rw-r--r--   0        0        0     1855 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_op.py
--rw-r--r--   0        0        0     3412 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_result.py
--rw-r--r--   0        0        0     1815 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
--rw-r--r--   0        0        0     2337 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_op.py
--rw-r--r--   0        0        0     2765 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_result.py
--rw-r--r--   0        0        0     1630 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_result_code.py
--rw-r--r--   0        0        0     3140 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_bandwidth_v0.py
--rw-r--r--   0        0        0     3888 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_compute_v0.py
--rw-r--r--   0        0        0     2855 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_events_v0.py
--rw-r--r--   0        0        0     2050 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_execution_lanes_v0.py
--rw-r--r--   0        0        0     2003 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_historical_data_v0.py
--rw-r--r--   0        0        0    10678 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_ledger_cost_v0.py
--rw-r--r--   0        0        0    19807 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_entry.py
--rw-r--r--   0        0        0     2620 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_id.py
--rw-r--r--   0        0        0     2338 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_upgrade_set.py
--rw-r--r--   0        0        0     2177 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/config_upgrade_set_key.py
--rw-r--r--   0        0        0     1323 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/constants.py
--rw-r--r--   0        0        0     2369 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_code_entry.py
--rw-r--r--   0        0        0     2590 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_cost_param_entry.py
--rw-r--r--   0        0        0     2436 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_cost_params.py
--rw-r--r--   0        0        0     4235 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_cost_type.py
--rw-r--r--   0        0        0     1268 2024-03-13 03:08:49.315457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_data_durability.py
--rw-r--r--   0        0        0     3086 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_data_entry.py
--rw-r--r--   0        0        0     3317 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event.py
--rw-r--r--   0        0        0     2272 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_body.py
--rw-r--r--   0        0        0     1283 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_type.py
--rw-r--r--   0        0        0     2444 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_v0.py
--rw-r--r--   0        0        0     2787 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_executable.py
--rw-r--r--   0        0        0     1352 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_executable_type.py
--rw-r--r--   0        0        0     3617 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage.py
--rw-r--r--   0        0        0     2114 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage_from_address.py
--rw-r--r--   0        0        0     1366 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage_type.py
--rw-r--r--   0        0        0     2312 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_op.py
--rw-r--r--   0        0        0     2954 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_result.py
--rw-r--r--   0        0        0     1889 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_result_code.py
--rw-r--r--   0        0        0     2950 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_op.py
--rw-r--r--   0        0        0     4556 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_result.py
--rw-r--r--   0        0        0     1836 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_result_code.py
--rw-r--r--   0        0        0     2435 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_contract_args.py
--rw-r--r--   0        0        0     2775 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/create_passive_sell_offer_op.py
--rw-r--r--   0        0        0     1610 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/crypto_key_type.py
--rw-r--r--   0        0        0     1662 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/curve25519_public.py
--rw-r--r--   0        0        0     1662 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/curve25519_secret.py
--rw-r--r--   0        0        0     2990 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/data_entry.py
--rw-r--r--   0        0        0     1678 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/data_entry_ext.py
--rw-r--r--   0        0        0     1544 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/data_value.py
--rw-r--r--   0        0        0     2179 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/decorated_signature.py
--rw-r--r--   0        0        0     2357 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/diagnostic_event.py
--rw-r--r--   0        0        0     2004 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/dont_have.py
--rw-r--r--   0        0        0     1484 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/duration.py
--rw-r--r--   0        0        0     1625 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/encrypted_body.py
--rw-r--r--   0        0        0     2725 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
--rw-r--r--   0        0        0     1621 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
--rw-r--r--   0        0        0     1848 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/envelope_type.py
--rw-r--r--   0        0        0     1919 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/error.py
--rw-r--r--   0        0        0     1433 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/error_code.py
--rw-r--r--   0        0        0     2778 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/eviction_iterator.py
--rw-r--r--   0        0        0     2098 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_op.py
--rw-r--r--   0        0        0     3108 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_result.py
--rw-r--r--   0        0        0     1761 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_result_code.py
--rw-r--r--   0        0        0     1690 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/extension_point.py
--rw-r--r--   0        0        0     3122 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction.py
--rw-r--r--   0        0        0     2842 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py
--rw-r--r--   0        0        0     1732 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_ext.py
--rw-r--r--   0        0        0     2405 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
--rw-r--r--   0        0        0     1717 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/flood_advert.py
--rw-r--r--   0        0        0     1717 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/flood_demand.py
--rw-r--r--   0        0        0     2432 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/generalized_transaction_set.py
--rw-r--r--   0        0        0     1441 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash.py
--rw-r--r--   0        0        0     6002 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage.py
--rw-r--r--   0        0        0     2395 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_contract_id.py
--rw-r--r--   0        0        0     2611 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py
--rw-r--r--   0        0        0     3361 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
--rw-r--r--   0        0        0     3269 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_soroban_authorization.py
--rw-r--r--   0        0        0     4746 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hello.py
--rw-r--r--   0        0        0     1641 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hmac_sha256_key.py
--rw-r--r--   0        0        0     1641 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/hmac_sha256_mac.py
--rw-r--r--   0        0        0     4343 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/host_function.py
--rw-r--r--   0        0        0     1443 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/host_function_type.py
--rw-r--r--   0        0        0     2143 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_payout.py
--rw-r--r--   0        0        0     3169 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_result.py
--rw-r--r--   0        0        0     1418 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_result_code.py
--rw-r--r--   0        0        0     3627 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result.py
--rw-r--r--   0        0        0     1756 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_ext.py
--rw-r--r--   0        0        0     2415 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_pair.py
--rw-r--r--   0        0        0     6879 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_result.py
--rw-r--r--   0        0        0     1878 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/int128_parts.py
--rw-r--r--   0        0        0     2548 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/int256_parts.py
--rw-r--r--   0        0        0     1433 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/int32.py
--rw-r--r--   0        0        0     1429 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/int64.py
--rw-r--r--   0        0        0     3056 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_contract_args.py
--rw-r--r--   0        0        0     2806 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_op.py
--rw-r--r--   0        0        0     4216 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_result.py
--rw-r--r--   0        0        0     1945 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_result_code.py
--rw-r--r--   0        0        0     2724 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_success_pre_image.py
--rw-r--r--   0        0        0     1182 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ip_addr_type.py
--rw-r--r--   0        0        0     2130 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_bounds.py
--rw-r--r--   0        0        0     2729 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta.py
--rw-r--r--   0        0        0     5570 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta_v0.py
--rw-r--r--   0        0        0     9666 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta_v1.py
--rw-r--r--   0        0        0     2223 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_value_signature.py
--rw-r--r--   0        0        0     3616 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry.py
--rw-r--r--   0        0        0     4553 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_change.py
--rw-r--r--   0        0        0     1573 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_change_type.py
--rw-r--r--   0        0        0     2345 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_changes.py
--rw-r--r--   0        0        0     9412 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_data.py
--rw-r--r--   0        0        0     2327 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_ext.py
--rw-r--r--   0        0        0     2376 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_extension_v1.py
--rw-r--r--   0        0        0     1756 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     1610 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_type.py
--rw-r--r--   0        0        0     3074 2024-03-13 03:08:49.319457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_footprint.py
--rw-r--r--   0        0        0     8598 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header.py
--rw-r--r--   0        0        0     2338 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_ext.py
--rw-r--r--   0        0        0     2229 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_extension_v1.py
--rw-r--r--   0        0        0     1762 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
--rw-r--r--   0        0        0     1457 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_flags.py
--rw-r--r--   0        0        0     2620 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_history_entry.py
--rw-r--r--   0        0        0     1768 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py
--rw-r--r--   0        0        0    10306 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key.py
--rw-r--r--   0        0        0     1733 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_account.py
--rw-r--r--   0        0        0     1833 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_claimable_balance.py
--rw-r--r--   0        0        0     1890 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_config_setting.py
--rw-r--r--   0        0        0     1660 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_contract_code.py
--rw-r--r--   0        0        0     2549 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_contract_data.py
--rw-r--r--   0        0        0     2125 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_data.py
--rw-r--r--   0        0        0     1844 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py
--rw-r--r--   0        0        0     2090 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_offer.py
--rw-r--r--   0        0        0     2136 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_trust_line.py
--rw-r--r--   0        0        0     1736 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_ttl.py
--rw-r--r--   0        0        0     2622 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_scp_messages.py
--rw-r--r--   0        0        0     8093 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_upgrade.py
--rw-r--r--   0        0        0     1705 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_upgrade_type.py
--rw-r--r--   0        0        0     1973 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liabilities.py
--rw-r--r--   0        0        0     2562 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
--rw-r--r--   0        0        0     3513 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py
--rw-r--r--   0        0        0     4114 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py
--rw-r--r--   0        0        0     2624 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
--rw-r--r--   0        0        0     2913 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry.py
--rw-r--r--   0        0        0     3260 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry_body.py
--rw-r--r--   0        0        0     3955 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
--rw-r--r--   0        0        0     2848 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_parameters.py
--rw-r--r--   0        0        0     1243 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_type.py
--rw-r--r--   0        0        0     3112 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
--rw-r--r--   0        0        0     3751 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
--rw-r--r--   0        0        0     2288 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
--rw-r--r--   0        0        0     3246 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_op.py
--rw-r--r--   0        0        0     5642 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_result.py
--rw-r--r--   0        0        0     2960 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_result_code.py
--rw-r--r--   0        0        0     2334 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_op.py
--rw-r--r--   0        0        0     2873 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_result.py
--rw-r--r--   0        0        0     1895 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_result_code.py
--rw-r--r--   0        0        0     1355 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_effect.py
--rw-r--r--   0        0        0     3130 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_success_result.py
--rw-r--r--   0        0        0     3165 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_success_result_offer.py
--rw-r--r--   0        0        0     3162 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_op.py
--rw-r--r--   0        0        0     5719 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_result.py
--rw-r--r--   0        0        0     3062 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_result_code.py
--rw-r--r--   0        0        0     4258 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/memo.py
--rw-r--r--   0        0        0     1325 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/memo_type.py
--rw-r--r--   0        0        0     2292 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/message_type.py
--rw-r--r--   0        0        0     3228 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/muxed_account.py
--rw-r--r--   0        0        0     2018 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/muxed_account_med25519.py
--rw-r--r--   0        0        0     1475 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/node_id.py
--rw-r--r--   0        0        0     4300 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry.py
--rw-r--r--   0        0        0     1684 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry_ext.py
--rw-r--r--   0        0        0     1303 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry_flags.py
--rw-r--r--   0        0        0     5038 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation.py
--rw-r--r--   0        0        0    27280 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_body.py
--rw-r--r--   0        0        0     1726 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_meta.py
--rw-r--r--   0        0        0     6380 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result.py
--rw-r--r--   0        0        0     1874 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result_code.py
--rw-r--r--   0        0        0    31859 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result_tr.py
--rw-r--r--   0        0        0     2879 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/operation_type.py
--rw-r--r--   0        0        0     4349 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_op.py
--rw-r--r--   0        0        0     8163 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result.py
--rw-r--r--   0        0        0     3359 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
--rw-r--r--   0        0        0     2677 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
--rw-r--r--   0        0        0     4362 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_op.py
--rw-r--r--   0        0        0     7685 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result.py
--rw-r--r--   0        0        0     3249 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py
--rw-r--r--   0        0        0     2659 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py
--rw-r--r--   0        0        0     2513 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/payment_op.py
--rw-r--r--   0        0        0     3771 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/payment_result.py
--rw-r--r--   0        0        0     2348 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/payment_result_code.py
--rw-r--r--   0        0        0     2526 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/peer_address.py
--rw-r--r--   0        0        0     2894 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/peer_address_ip.py
--rw-r--r--   0        0        0     2118 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/peer_stat_list.py
--rw-r--r--   0        0        0     8363 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/peer_stats.py
--rw-r--r--   0        0        0     3163 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state.py
--rw-r--r--   0        0        0     4503 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state_v0.py
--rw-r--r--   0        0        0     3695 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state_v1.py
--rw-r--r--   0        0        0     1449 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/pool_id.py
--rw-r--r--   0        0        0     1297 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/precondition_type.py
--rw-r--r--   0        0        0     3321 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/preconditions.py
--rw-r--r--   0        0        0     6234 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/preconditions_v2.py
--rw-r--r--   0        0        0     1816 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/price.py
--rw-r--r--   0        0        0     2341 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/public_key.py
--rw-r--r--   0        0        0     1218 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/public_key_type.py
--rw-r--r--   0        0        0     1688 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_op.py
--rw-r--r--   0        0        0     2995 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_result.py
--rw-r--r--   0        0        0     1725 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_result_code.py
--rw-r--r--   0        0        0     3486 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_op.py
--rw-r--r--   0        0        0     2240 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
--rw-r--r--   0        0        0     3420 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_result.py
--rw-r--r--   0        0        0     1879 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py
--rw-r--r--   0        0        0     1344 2024-03-13 03:08:49.323457 stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_type.py
--rw-r--r--   0        0        0     3227 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_address.py
--rw-r--r--   0        0        0     1278 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_address_type.py
--rw-r--r--   0        0        0     1522 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_bytes.py
--rw-r--r--   0        0        0     2348 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_contract_instance.py
--rw-r--r--   0        0        0     2622 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_env_meta_entry.py
--rw-r--r--   0        0        0     1225 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_env_meta_kind.py
--rw-r--r--   0        0        0     5920 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error.py
--rw-r--r--   0        0        0     2258 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error_code.py
--rw-r--r--   0        0        0     2100 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error_type.py
--rw-r--r--   0        0        0     1929 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_map.py
--rw-r--r--   0        0        0     1876 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_map_entry.py
--rw-r--r--   0        0        0     2222 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_entry.py
--rw-r--r--   0        0        0     1159 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_kind.py
--rw-r--r--   0        0        0     1909 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_v0.py
--rw-r--r--   0        0        0     1604 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_nonce_key.py
--rw-r--r--   0        0        0     6096 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_entry.py
--rw-r--r--   0        0        0     1545 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_entry_kind.py
--rw-r--r--   0        0        0     2422 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_function_input_v0.py
--rw-r--r--   0        0        0     3748 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_function_v0.py
--rw-r--r--   0        0        0     2848 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type.py
--rw-r--r--   0        0        0     1607 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_bytes_n.py
--rw-r--r--   0        0        0    10391 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_def.py
--rw-r--r--   0        0        0     2117 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_map.py
--rw-r--r--   0        0        0     1761 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_option.py
--rw-r--r--   0        0        0     2125 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_result.py
--rw-r--r--   0        0        0     2267 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_tuple.py
--rw-r--r--   0        0        0     1638 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_udt.py
--rw-r--r--   0        0        0     1766 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_vec.py
--rw-r--r--   0        0        0     2383 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_enum_case_v0.py
--rw-r--r--   0        0        0     3144 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_enum_v0.py
--rw-r--r--   0        0        0     2418 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_error_enum_case_v0.py
--rw-r--r--   0        0        0     3205 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_error_enum_v0.py
--rw-r--r--   0        0        0     2429 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_struct_field_v0.py
--rw-r--r--   0        0        0     3194 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_struct_v0.py
--rw-r--r--   0        0        0     2894 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_tuple_v0.py
--rw-r--r--   0        0        0     3608 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0.py
--rw-r--r--   0        0        0     1372 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0_kind.py
--rw-r--r--   0        0        0     2077 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_void_v0.py
--rw-r--r--   0        0        0     3156 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_v0.py
--rw-r--r--   0        0        0     1514 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_string.py
--rw-r--r--   0        0        0     1557 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_symbol.py
--rw-r--r--   0        0        0    16109 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_val.py
--rw-r--r--   0        0        0     3579 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_val_type.py
--rw-r--r--   0        0        0     1903 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sc_vec.py
--rw-r--r--   0        0        0     1989 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_ballot.py
--rw-r--r--   0        0        0     2119 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_envelope.py
--rw-r--r--   0        0        0     2177 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_history_entry.py
--rw-r--r--   0        0        0     2897 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_history_entry_v0.py
--rw-r--r--   0        0        0     3384 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_nomination.py
--rw-r--r--   0        0        0     3464 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_quorum_set.py
--rw-r--r--   0        0        0     3677 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement.py
--rw-r--r--   0        0        0     3227 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_confirm.py
--rw-r--r--   0        0        0     2683 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_externalize.py
--rw-r--r--   0        0        0     5628 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_pledges.py
--rw-r--r--   0        0        0     3953 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_prepare.py
--rw-r--r--   0        0        0     1378 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_type.py
--rw-r--r--   0        0        0     1693 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/send_more.py
--rw-r--r--   0        0        0     2154 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/send_more_extended.py
--rw-r--r--   0        0        0     1598 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sequence_number.py
--rw-r--r--   0        0        0     6626 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_op.py
--rw-r--r--   0        0        0     4319 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_result.py
--rw-r--r--   0        0        0     2616 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_result_code.py
--rw-r--r--   0        0        0     2858 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_op.py
--rw-r--r--   0        0        0     3407 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_result.py
--rw-r--r--   0        0        0     2015 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py
--rw-r--r--   0        0        0     1533 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signature.py
--rw-r--r--   0        0        0     1611 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signature_hint.py
--rw-r--r--   0        0        0     2378 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signed_survey_request_message.py
--rw-r--r--   0        0        0     2416 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signed_survey_response_message.py
--rw-r--r--   0        0        0     1964 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signer.py
--rw-r--r--   0        0        0     5223 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key.py
--rw-r--r--   0        0        0     2288 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
--rw-r--r--   0        0        0     1536 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key_type.py
--rw-r--r--   0        0        0     2463 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/simple_payment_result.py
--rw-r--r--   0        0        0     3082 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_address_credentials.py
--rw-r--r--   0        0        0     2478 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorization_entry.py
--rw-r--r--   0        0        0     4111 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_function.py
--rw-r--r--   0        0        0     1480 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_function_type.py
--rw-r--r--   0        0        0     2958 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_invocation.py
--rw-r--r--   0        0        0     2852 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_credentials.py
--rw-r--r--   0        0        0     1360 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_credentials_type.py
--rw-r--r--   0        0        0     3219 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_resources.py
--rw-r--r--   0        0        0     3230 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_transaction_data.py
--rw-r--r--   0        0        0     4413 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_transaction_meta.py
--rw-r--r--   0        0        0     1974 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/sponsorship_descriptor.py
--rw-r--r--   0        0        0     6554 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/state_archival_settings.py
--rw-r--r--   0        0        0    17518 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_message.py
--rw-r--r--   0        0        0     4020 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value.py
--rw-r--r--   0        0        0     2852 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value_ext.py
--rw-r--r--   0        0        0     1280 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value_type.py
--rw-r--r--   0        0        0     2986 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stored_debug_transaction_set.py
--rw-r--r--   0        0        0     3573 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/stored_transaction_set.py
--rw-r--r--   0        0        0     1497 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/string32.py
--rw-r--r--   0        0        0     1497 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/string64.py
--rw-r--r--   0        0        0     1253 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/survey_message_command_type.py
--rw-r--r--   0        0        0     1364 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/survey_message_response_type.py
--rw-r--r--   0        0        0     3653 2024-03-13 03:08:49.327457 stellar_sdk-9.3.0/stellar_sdk/xdr/survey_request_message.py
--rw-r--r--   0        0        0     4040 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/survey_response_body.py
--rw-r--r--   0        0        0     3645 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/survey_response_message.py
--rw-r--r--   0        0        0     1382 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/threshold_indexes.py
--rw-r--r--   0        0        0     1546 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/thresholds.py
--rw-r--r--   0        0        0     2063 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/time_bounds.py
--rw-r--r--   0        0        0     1513 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/time_point.py
--rw-r--r--   0        0        0     3409 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/topology_response_body_v0.py
--rw-r--r--   0        0        0     4415 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/topology_response_body_v1.py
--rw-r--r--   0        0        0     4750 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction.py
--rw-r--r--   0        0        0     3899 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_envelope.py
--rw-r--r--   0        0        0     2507 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_ext.py
--rw-r--r--   0        0        0     2793 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_entry.py
--rw-r--r--   0        0        0     2689 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_entry_ext.py
--rw-r--r--   0        0        0     2892 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_result_entry.py
--rw-r--r--   0        0        0     1798 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py
--rw-r--r--   0        0        0     4548 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta.py
--rw-r--r--   0        0        0     2816 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v1.py
--rw-r--r--   0        0        0     3568 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v2.py
--rw-r--r--   0        0        0     4682 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v3.py
--rw-r--r--   0        0        0     2907 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_phase.py
--rw-r--r--   0        0        0     3629 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result.py
--rw-r--r--   0        0        0     3143 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_code.py
--rw-r--r--   0        0        0     1726 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_ext.py
--rw-r--r--   0        0        0     2874 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_meta.py
--rw-r--r--   0        0        0     2306 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_pair.py
--rw-r--r--   0        0        0     8349 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_result.py
--rw-r--r--   0        0        0     2264 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_set.py
--rw-r--r--   0        0        0     2691 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_set.py
--rw-r--r--   0        0        0     2753 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_set_v1.py
--rw-r--r--   0        0        0     2836 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_signature_payload.py
--rw-r--r--   0        0        0     3373 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
--rw-r--r--   0        0        0     4792 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0.py
--rw-r--r--   0        0        0     2781 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0_envelope.py
--rw-r--r--   0        0        0     1702 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0_ext.py
--rw-r--r--   0        0        0     2770 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v1_envelope.py
--rw-r--r--   0        0        0     4417 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_asset.py
--rw-r--r--   0        0        0     4137 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry.py
--rw-r--r--   0        0        0     2637 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_ext.py
--rw-r--r--   0        0        0     2506 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py
--rw-r--r--   0        0        0     1774 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
--rw-r--r--   0        0        0     2370 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_v1.py
--rw-r--r--   0        0        0     2421 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py
--rw-r--r--   0        0        0     1742 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_flags.py
--rw-r--r--   0        0        0     2284 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/ttl_entry.py
--rw-r--r--   0        0        0     2215 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/tx_advert_vector.py
--rw-r--r--   0        0        0     2215 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/tx_demand_vector.py
--rw-r--r--   0        0        0     3020 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component.py
--rw-r--r--   0        0        0     2792 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component_txs_maybe_discounted_fee.py
--rw-r--r--   0        0        0     1399 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component_type.py
--rw-r--r--   0        0        0     1863 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/u_int128_parts.py
--rw-r--r--   0        0        0     2533 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/u_int256_parts.py
--rw-r--r--   0        0        0     1495 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/uint256.py
--rw-r--r--   0        0        0     1484 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/uint32.py
--rw-r--r--   0        0        0     1480 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/uint64.py
--rw-r--r--   0        0        0     2154 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/upgrade_entry_meta.py
--rw-r--r--   0        0        0     1583 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/upgrade_type.py
--rw-r--r--   0        0        0     1475 2024-03-13 03:08:49.331457 stellar_sdk-9.3.0/stellar_sdk/xdr/value.py
--rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 stellar_sdk-9.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 01:57:38.628906 stellar_sdk-9.4.0/LICENSE
+-rw-r--r--   0        0        0     4635 2024-05-01 01:57:38.628906 stellar_sdk-9.4.0/README.rst
+-rw-r--r--   0        0        0     3097 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1200 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/__init__.py
+-rw-r--r--   0        0        0      876 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/__version__.py
+-rw-r--r--   0        0        0     4736 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/account.py
+-rw-r--r--   0        0        0     5223 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/address.py
+-rw-r--r--   0        0        0    10156 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/asset.py
+-rw-r--r--   0        0        0     6602 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/auth.py
+-rw-r--r--   0        0        0    13620 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/base_server.py
+-rw-r--r--   0        0        0     1931 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/base_soroban_server.py
+-rw-r--r--   0        0        0     5629 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/base_transaction_envelope.py
+-rw-r--r--   0        0        0        0 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/__init__.py
+-rw-r--r--   0        0        0     3349 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py
+-rw-r--r--   0        0        0     1452 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_assets_call_builder.py
+-rw-r--r--   0        0        0     4738 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_call_builder.py
+-rw-r--r--   0        0        0     2722 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py
+-rw-r--r--   0        0        0      738 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_data_call_builder.py
+-rw-r--r--   0        0        0     3219 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_effects_call_builder.py
+-rw-r--r--   0        0        0      537 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py
+-rw-r--r--   0        0        0      959 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py
+-rw-r--r--   0        0        0     2104 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py
+-rw-r--r--   0        0        0     4182 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_offers_call_builder.py
+-rw-r--r--   0        0        0     4563 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_operations_call_builder.py
+-rw-r--r--   0        0        0     1088 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py
+-rw-r--r--   0        0        0     2811 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_payments_call_builder.py
+-rw-r--r--   0        0        0      378 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_root_call_builder.py
+-rw-r--r--   0        0        0     2766 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2517 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     3143 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0     3217 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_trades_call_builder.py
+-rw-r--r--   0        0        0     3674 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py
+-rw-r--r--   0        0        0      734 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/__init__.py
+-rw-r--r--   0        0        0      870 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py
+-rw-r--r--   0        0        0      997 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py
+-rw-r--r--   0        0        0     4317 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py
+-rw-r--r--   0        0        0     1077 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py
+-rw-r--r--   0        0        0     1158 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py
+-rw-r--r--   0        0        0      840 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py
+-rw-r--r--   0        0        0     1005 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py
+-rw-r--r--   0        0        0      840 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py
+-rw-r--r--   0        0        0     1039 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py
+-rw-r--r--   0        0        0      832 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py
+-rw-r--r--   0        0        0      859 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py
+-rw-r--r--   0        0        0     1081 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py
+-rw-r--r--   0        0        0      859 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py
+-rw-r--r--   0        0        0      874 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py
+-rw-r--r--   0        0        0     2718 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2487 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     2292 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0      832 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py
+-rw-r--r--   0        0        0      880 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py
+-rw-r--r--   0        0        0      734 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py
+-rw-r--r--   0        0        0      982 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py
+-rw-r--r--   0        0        0     4119 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py
+-rw-r--r--   0        0        0     1062 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py
+-rw-r--r--   0        0        0     1175 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py
+-rw-r--r--   0        0        0      831 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py
+-rw-r--r--   0        0        0      990 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py
+-rw-r--r--   0        0        0      831 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py
+-rw-r--r--   0        0        0     1024 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py
+-rw-r--r--   0        0        0      823 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py
+-rw-r--r--   0        0        0      850 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py
+-rw-r--r--   0        0        0     1072 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py
+-rw-r--r--   0        0        0      850 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py
+-rw-r--r--   0        0        0      859 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py
+-rw-r--r--   0        0        0     2729 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2498 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     2303 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0      823 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py
+-rw-r--r--   0        0        0      871 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py
+-rw-r--r--   0        0        0        0 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/__init__.py
+-rw-r--r--   0        0        0     9952 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/aiohttp_client.py
+-rw-r--r--   0        0        0     2007 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/base_async_client.py
+-rw-r--r--   0        0        0     1850 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/base_sync_client.py
+-rw-r--r--   0        0        0      445 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/defines.py
+-rw-r--r--   0        0        0     8147 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/requests_client.py
+-rw-r--r--   0        0        0     1383 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/response.py
+-rw-r--r--   0        0        0     2756 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/client/simple_requests_client.py
+-rw-r--r--   0        0        0     1919 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/decorated_signature.py
+-rw-r--r--   0        0        0     5722 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/exceptions.py
+-rw-r--r--   0        0        0     5533 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/fee_bump_transaction.py
+-rw-r--r--   0        0        0     5678 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/fee_bump_transaction_envelope.py
+-rw-r--r--   0        0        0     1997 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/helpers.py
+-rw-r--r--   0        0        0    12145 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/keypair.py
+-rw-r--r--   0        0        0     2343 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/ledger_bounds.py
+-rw-r--r--   0        0        0     6056 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/liquidity_pool_asset.py
+-rw-r--r--   0        0        0     2241 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/liquidity_pool_id.py
+-rw-r--r--   0        0        0     9317 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/memo.py
+-rw-r--r--   0        0        0     6161 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/muxed_account.py
+-rw-r--r--   0        0        0     2183 2024-05-01 01:57:38.632906 stellar_sdk-9.4.0/stellar_sdk/network.py
+-rw-r--r--   0        0        0      950 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/__init__.py
+-rw-r--r--   0        0        0     2087 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/account_merge.py
+-rw-r--r--   0        0        0     6259 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/allow_trust.py
+-rw-r--r--   0        0        0     2890 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py
+-rw-r--r--   0        0        0     2163 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/bump_sequence.py
+-rw-r--r--   0        0        0     3157 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/change_trust.py
+-rw-r--r--   0        0        0     2529 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/claim_claimable_balance.py
+-rw-r--r--   0        0        0     2679 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/clawback.py
+-rw-r--r--   0        0        0     2510 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/clawback_claimable_balance.py
+-rw-r--r--   0        0        0     3271 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/create_account.py
+-rw-r--r--   0        0        0    17123 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/create_claimable_balance.py
+-rw-r--r--   0        0        0     4357 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/create_passive_sell_offer.py
+-rw-r--r--   0        0        0     1737 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/end_sponsoring_future_reserves.py
+-rw-r--r--   0        0        0     2225 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/extend_footprint_ttl.py
+-rw-r--r--   0        0        0     1212 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/inflation.py
+-rw-r--r--   0        0        0     2398 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/invoke_host_function.py
+-rw-r--r--   0        0        0     4741 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/liquidity_pool_deposit.py
+-rw-r--r--   0        0        0     4147 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/liquidity_pool_withdraw.py
+-rw-r--r--   0        0        0     3881 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/manage_buy_offer.py
+-rw-r--r--   0        0        0     3355 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/manage_data.py
+-rw-r--r--   0        0        0     3892 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/manage_sell_offer.py
+-rw-r--r--   0        0        0     4975 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/operation.py
+-rw-r--r--   0        0        0     5013 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/path_payment_strict_receive.py
+-rw-r--r--   0        0        0     4947 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/path_payment_strict_send.py
+-rw-r--r--   0        0        0     2783 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/payment.py
+-rw-r--r--   0        0        0     1516 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/restore_footprint.py
+-rw-r--r--   0        0        0    24387 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/revoke_sponsorship.py
+-rw-r--r--   0        0        0    10477 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/set_options.py
+-rw-r--r--   0        0        0     4633 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/operation/set_trust_line_flags.py
+-rw-r--r--   0        0        0     8741 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/preconditions.py
+-rw-r--r--   0        0        0     2934 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/price.py
+-rw-r--r--   0        0        0        0 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/py.typed
+-rw-r--r--   0        0        0    27303 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/scval.py
+-rw-r--r--   0        0        0        0 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/ed25519_public_key_signer.py
+-rw-r--r--   0        0        0     1550 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/exceptions.py
+-rw-r--r--   0        0        0     9256 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/federation.py
+-rw-r--r--   0        0        0     3118 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/mnemonic.py
+-rw-r--r--   0        0        0     3071 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/stellar_toml.py
+-rw-r--r--   0        0        0    20271 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/stellar_uri.py
+-rw-r--r--   0        0        0    27857 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/stellar_web_authentication.py
+-rw-r--r--   0        0        0     5328 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/toid.py
+-rw-r--r--   0        0        0    71955 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/sep/txrep.py
+-rw-r--r--   0        0        0    15397 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/server.py
+-rw-r--r--   0        0        0    15574 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/server_async.py
+-rw-r--r--   0        0        0     4148 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/signer.py
+-rw-r--r--   0        0        0    11311 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/signer_key.py
+-rw-r--r--   0        0        0     3954 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/soroban_data_builder.py
+-rw-r--r--   0        0        0    10979 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/soroban_rpc.py
+-rw-r--r--   0        0        0    16766 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/soroban_server.py
+-rw-r--r--   0        0        0    16970 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/soroban_server_async.py
+-rw-r--r--   0        0        0    13325 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/strkey.py
+-rw-r--r--   0        0        0     2557 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/time_bounds.py
+-rw-r--r--   0        0        0    12383 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/transaction.py
+-rw-r--r--   0        0        0    66516 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/transaction_builder.py
+-rw-r--r--   0        0        0     7388 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/transaction_envelope.py
+-rw-r--r--   0        0        0     5943 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/utils.py
+-rw-r--r--   0        0        0    15524 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/xdr/__init__.py
+-rw-r--r--   0        0        0     6433 2024-05-01 01:57:38.636906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry.py
+-rw-r--r--   0        0        0     2338 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_ext.py
+-rw-r--r--   0        0        0     2375 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v1.py
+-rw-r--r--   0        0        0     2404 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     4035 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v2.py
+-rw-r--r--   0        0        0     2404 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py
+-rw-r--r--   0        0        0     2806 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v3.py
+-rw-r--r--   0        0        0     2007 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_flags.py
+-rw-r--r--   0        0        0     1529 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_id.py
+-rw-r--r--   0        0        0     4475 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_merge_result.py
+-rw-r--r--   0        0        0     2278 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/account_merge_result_code.py
+-rw-r--r--   0        0        0     2513 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_op.py
+-rw-r--r--   0        0        0     3331 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_result.py
+-rw-r--r--   0        0        0     2199 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_result_code.py
+-rw-r--r--   0        0        0     2081 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/alpha_num12.py
+-rw-r--r--   0        0        0     2069 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/alpha_num4.py
+-rw-r--r--   0        0        0     3494 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/asset.py
+-rw-r--r--   0        0        0     3345 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code.py
+-rw-r--r--   0        0        0     1578 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code12.py
+-rw-r--r--   0        0        0     1557 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code4.py
+-rw-r--r--   0        0        0     1400 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/asset_type.py
+-rw-r--r--   0        0        0     1578 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/auth.py
+-rw-r--r--   0        0        0     2407 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/auth_cert.py
+-rw-r--r--   0        0        0     2353 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/authenticated_message.py
+-rw-r--r--   0        0        0     2500 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/authenticated_message_v0.py
+-rw-r--r--   0        0        0     6626 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/base.py
+-rw-r--r--   0        0        0     1870 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
+-rw-r--r--   0        0        0     3567 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
+-rw-r--r--   0        0        0     1875 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0        0        0     4356 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_entry.py
+-rw-r--r--   0        0        0     1561 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_entry_type.py
+-rw-r--r--   0        0        0     2344 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_metadata.py
+-rw-r--r--   0        0        0     1708 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_metadata_ext.py
+-rw-r--r--   0        0        0     1711 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_op.py
+-rw-r--r--   0        0        0     2197 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_result.py
+-rw-r--r--   0        0        0     1483 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_result_code.py
+-rw-r--r--   0        0        0     4470 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_asset.py
+-rw-r--r--   0        0        0     2078 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_op.py
+-rw-r--r--   0        0        0     3930 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_result.py
+-rw-r--r--   0        0        0     2461 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_result_code.py
+-rw-r--r--   0        0        0     4050 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_atom.py
+-rw-r--r--   0        0        0     1359 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_atom_type.py
+-rw-r--r--   0        0        0     1834 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_op.py
+-rw-r--r--   0        0        0     3808 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_result.py
+-rw-r--r--   0        0        0     1826 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     3491 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_liquidity_atom.py
+-rw-r--r--   0        0        0     3766 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_offer_atom.py
+-rw-r--r--   0        0        0     3834 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_offer_atom_v0.py
+-rw-r--r--   0        0        0     7471 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_predicate.py
+-rw-r--r--   0        0        0     1636 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claim_predicate_type.py
+-rw-r--r--   0        0        0     4122 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry.py
+-rw-r--r--   0        0        0     2438 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_ext.py
+-rw-r--r--   0        0        0     2346 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
+-rw-r--r--   0        0        0     1816 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     1420 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_flags.py
+-rw-r--r--   0        0        0     2388 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_id.py
+-rw-r--r--   0        0        0     1267 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_id_type.py
+-rw-r--r--   0        0        0     2426 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimant.py
+-rw-r--r--   0        0        0     1183 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimant_type.py
+-rw-r--r--   0        0        0     2257 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/claimant_v0.py
+-rw-r--r--   0        0        0     1855 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_op.py
+-rw-r--r--   0        0        0     3412 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_result.py
+-rw-r--r--   0        0        0     1815 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     2337 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_op.py
+-rw-r--r--   0        0        0     2765 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_result.py
+-rw-r--r--   0        0        0     1630 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_result_code.py
+-rw-r--r--   0        0        0     3140 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_bandwidth_v0.py
+-rw-r--r--   0        0        0     3888 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_compute_v0.py
+-rw-r--r--   0        0        0     2855 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_events_v0.py
+-rw-r--r--   0        0        0     2050 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_execution_lanes_v0.py
+-rw-r--r--   0        0        0     2003 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_historical_data_v0.py
+-rw-r--r--   0        0        0    10678 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_ledger_cost_v0.py
+-rw-r--r--   0        0        0    19807 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_entry.py
+-rw-r--r--   0        0        0     2620 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_id.py
+-rw-r--r--   0        0        0     2338 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_upgrade_set.py
+-rw-r--r--   0        0        0     2177 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/config_upgrade_set_key.py
+-rw-r--r--   0        0        0     1323 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/constants.py
+-rw-r--r--   0        0        0     5538 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_code_cost_inputs.py
+-rw-r--r--   0        0        0     2681 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_code_entry.py
+-rw-r--r--   0        0        0     2498 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_code_entry_ext.py
+-rw-r--r--   0        0        0     2227 2024-05-01 01:57:38.640906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_code_entry_v1.py
+-rw-r--r--   0        0        0     2590 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_cost_param_entry.py
+-rw-r--r--   0        0        0     2436 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_cost_params.py
+-rw-r--r--   0        0        0     7509 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_cost_type.py
+-rw-r--r--   0        0        0     1268 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_data_durability.py
+-rw-r--r--   0        0        0     3086 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_data_entry.py
+-rw-r--r--   0        0        0     3317 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event.py
+-rw-r--r--   0        0        0     2272 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_body.py
+-rw-r--r--   0        0        0     1283 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_type.py
+-rw-r--r--   0        0        0     2444 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_v0.py
+-rw-r--r--   0        0        0     2787 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_executable.py
+-rw-r--r--   0        0        0     1352 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_executable_type.py
+-rw-r--r--   0        0        0     3617 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage.py
+-rw-r--r--   0        0        0     2114 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage_from_address.py
+-rw-r--r--   0        0        0     1366 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage_type.py
+-rw-r--r--   0        0        0     2312 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_op.py
+-rw-r--r--   0        0        0     2954 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_result.py
+-rw-r--r--   0        0        0     1889 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_result_code.py
+-rw-r--r--   0        0        0     2950 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_op.py
+-rw-r--r--   0        0        0     4556 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_result.py
+-rw-r--r--   0        0        0     1836 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     2435 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_contract_args.py
+-rw-r--r--   0        0        0     2775 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/create_passive_sell_offer_op.py
+-rw-r--r--   0        0        0     1610 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/crypto_key_type.py
+-rw-r--r--   0        0        0     1662 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/curve25519_public.py
+-rw-r--r--   0        0        0     1662 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/curve25519_secret.py
+-rw-r--r--   0        0        0     2990 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/data_entry.py
+-rw-r--r--   0        0        0     1678 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/data_entry_ext.py
+-rw-r--r--   0        0        0     1544 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/data_value.py
+-rw-r--r--   0        0        0     2179 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/decorated_signature.py
+-rw-r--r--   0        0        0     2357 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/diagnostic_event.py
+-rw-r--r--   0        0        0     2004 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/dont_have.py
+-rw-r--r--   0        0        0     1484 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/duration.py
+-rw-r--r--   0        0        0     1625 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/encrypted_body.py
+-rw-r--r--   0        0        0     2725 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
+-rw-r--r--   0        0        0     1621 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0        0        0     1848 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/envelope_type.py
+-rw-r--r--   0        0        0     1919 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/error.py
+-rw-r--r--   0        0        0     1433 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/error_code.py
+-rw-r--r--   0        0        0     2778 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/eviction_iterator.py
+-rw-r--r--   0        0        0     2098 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_op.py
+-rw-r--r--   0        0        0     3108 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_result.py
+-rw-r--r--   0        0        0     1761 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_result_code.py
+-rw-r--r--   0        0        0     1690 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/extension_point.py
+-rw-r--r--   0        0        0     3122 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction.py
+-rw-r--r--   0        0        0     2842 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py
+-rw-r--r--   0        0        0     1732 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_ext.py
+-rw-r--r--   0        0        0     2405 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
+-rw-r--r--   0        0        0     1717 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/flood_advert.py
+-rw-r--r--   0        0        0     1717 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/flood_demand.py
+-rw-r--r--   0        0        0     2432 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/generalized_transaction_set.py
+-rw-r--r--   0        0        0     1441 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash.py
+-rw-r--r--   0        0        0     6002 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage.py
+-rw-r--r--   0        0        0     2395 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_contract_id.py
+-rw-r--r--   0        0        0     2611 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py
+-rw-r--r--   0        0        0     3361 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
+-rw-r--r--   0        0        0     3269 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_soroban_authorization.py
+-rw-r--r--   0        0        0     4746 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hello.py
+-rw-r--r--   0        0        0     1641 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hmac_sha256_key.py
+-rw-r--r--   0        0        0     1641 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/hmac_sha256_mac.py
+-rw-r--r--   0        0        0     4343 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/host_function.py
+-rw-r--r--   0        0        0     1443 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/host_function_type.py
+-rw-r--r--   0        0        0     2143 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_payout.py
+-rw-r--r--   0        0        0     3169 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_result.py
+-rw-r--r--   0        0        0     1418 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_result_code.py
+-rw-r--r--   0        0        0     3627 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result.py
+-rw-r--r--   0        0        0     1756 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_ext.py
+-rw-r--r--   0        0        0     2415 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_pair.py
+-rw-r--r--   0        0        0     6879 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_result.py
+-rw-r--r--   0        0        0     1878 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/int128_parts.py
+-rw-r--r--   0        0        0     2548 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/int256_parts.py
+-rw-r--r--   0        0        0     1433 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/int32.py
+-rw-r--r--   0        0        0     1429 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/int64.py
+-rw-r--r--   0        0        0     3056 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_contract_args.py
+-rw-r--r--   0        0        0     2806 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_op.py
+-rw-r--r--   0        0        0     4216 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_result.py
+-rw-r--r--   0        0        0     1945 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_result_code.py
+-rw-r--r--   0        0        0     2724 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_success_pre_image.py
+-rw-r--r--   0        0        0     1182 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ip_addr_type.py
+-rw-r--r--   0        0        0     2130 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_bounds.py
+-rw-r--r--   0        0        0     2729 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta.py
+-rw-r--r--   0        0        0     2338 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_ext.py
+-rw-r--r--   0        0        0     2283 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_ext_v1.py
+-rw-r--r--   0        0        0     5570 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_v0.py
+-rw-r--r--   0        0        0     9578 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_v1.py
+-rw-r--r--   0        0        0     2223 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_value_signature.py
+-rw-r--r--   0        0        0     3616 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry.py
+-rw-r--r--   0        0        0     4553 2024-05-01 01:57:38.644906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_change.py
+-rw-r--r--   0        0        0     1573 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_change_type.py
+-rw-r--r--   0        0        0     2345 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_changes.py
+-rw-r--r--   0        0        0     9412 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_data.py
+-rw-r--r--   0        0        0     2327 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_ext.py
+-rw-r--r--   0        0        0     2376 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_extension_v1.py
+-rw-r--r--   0        0        0     1756 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     1610 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_type.py
+-rw-r--r--   0        0        0     3074 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_footprint.py
+-rw-r--r--   0        0        0     8598 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header.py
+-rw-r--r--   0        0        0     2338 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_ext.py
+-rw-r--r--   0        0        0     2229 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_extension_v1.py
+-rw-r--r--   0        0        0     1762 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
+-rw-r--r--   0        0        0     1457 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_flags.py
+-rw-r--r--   0        0        0     2620 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_history_entry.py
+-rw-r--r--   0        0        0     1768 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py
+-rw-r--r--   0        0        0    10306 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key.py
+-rw-r--r--   0        0        0     1733 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_account.py
+-rw-r--r--   0        0        0     1833 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_claimable_balance.py
+-rw-r--r--   0        0        0     1890 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_config_setting.py
+-rw-r--r--   0        0        0     1660 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_contract_code.py
+-rw-r--r--   0        0        0     2549 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_contract_data.py
+-rw-r--r--   0        0        0     2125 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_data.py
+-rw-r--r--   0        0        0     1844 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py
+-rw-r--r--   0        0        0     2090 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_offer.py
+-rw-r--r--   0        0        0     2136 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_trust_line.py
+-rw-r--r--   0        0        0     1736 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_ttl.py
+-rw-r--r--   0        0        0     2622 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_scp_messages.py
+-rw-r--r--   0        0        0     8093 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_upgrade.py
+-rw-r--r--   0        0        0     1705 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_upgrade_type.py
+-rw-r--r--   0        0        0     1973 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liabilities.py
+-rw-r--r--   0        0        0     2562 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
+-rw-r--r--   0        0        0     3513 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py
+-rw-r--r--   0        0        0     4114 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py
+-rw-r--r--   0        0        0     2624 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
+-rw-r--r--   0        0        0     2913 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry.py
+-rw-r--r--   0        0        0     3260 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry_body.py
+-rw-r--r--   0        0        0     3955 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
+-rw-r--r--   0        0        0     2848 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_parameters.py
+-rw-r--r--   0        0        0     1243 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_type.py
+-rw-r--r--   0        0        0     3112 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
+-rw-r--r--   0        0        0     3751 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
+-rw-r--r--   0        0        0     2288 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
+-rw-r--r--   0        0        0     3246 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_op.py
+-rw-r--r--   0        0        0     5642 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_result.py
+-rw-r--r--   0        0        0     2960 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_result_code.py
+-rw-r--r--   0        0        0     2334 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_op.py
+-rw-r--r--   0        0        0     2873 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_result.py
+-rw-r--r--   0        0        0     1895 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_result_code.py
+-rw-r--r--   0        0        0     1355 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_effect.py
+-rw-r--r--   0        0        0     3130 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_success_result.py
+-rw-r--r--   0        0        0     3165 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_success_result_offer.py
+-rw-r--r--   0        0        0     3162 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_op.py
+-rw-r--r--   0        0        0     5719 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_result.py
+-rw-r--r--   0        0        0     3062 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_result_code.py
+-rw-r--r--   0        0        0     4258 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/memo.py
+-rw-r--r--   0        0        0     1325 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/memo_type.py
+-rw-r--r--   0        0        0     2292 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/message_type.py
+-rw-r--r--   0        0        0     3228 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/muxed_account.py
+-rw-r--r--   0        0        0     2018 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/muxed_account_med25519.py
+-rw-r--r--   0        0        0     1475 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/node_id.py
+-rw-r--r--   0        0        0     4300 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry.py
+-rw-r--r--   0        0        0     1684 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry_ext.py
+-rw-r--r--   0        0        0     1303 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry_flags.py
+-rw-r--r--   0        0        0     5038 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation.py
+-rw-r--r--   0        0        0    27280 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_body.py
+-rw-r--r--   0        0        0     1726 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_meta.py
+-rw-r--r--   0        0        0     6380 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result.py
+-rw-r--r--   0        0        0     1874 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result_code.py
+-rw-r--r--   0        0        0    31859 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result_tr.py
+-rw-r--r--   0        0        0     2879 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/operation_type.py
+-rw-r--r--   0        0        0     4349 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_op.py
+-rw-r--r--   0        0        0     8163 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result.py
+-rw-r--r--   0        0        0     3359 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
+-rw-r--r--   0        0        0     2677 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
+-rw-r--r--   0        0        0     4362 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_op.py
+-rw-r--r--   0        0        0     7685 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result.py
+-rw-r--r--   0        0        0     3249 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py
+-rw-r--r--   0        0        0     2659 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py
+-rw-r--r--   0        0        0     2513 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/payment_op.py
+-rw-r--r--   0        0        0     3771 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/payment_result.py
+-rw-r--r--   0        0        0     2348 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/payment_result_code.py
+-rw-r--r--   0        0        0     2526 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/peer_address.py
+-rw-r--r--   0        0        0     2894 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/peer_address_ip.py
+-rw-r--r--   0        0        0     2118 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/peer_stat_list.py
+-rw-r--r--   0        0        0     8363 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/peer_stats.py
+-rw-r--r--   0        0        0     3163 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state.py
+-rw-r--r--   0        0        0     4503 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state_v0.py
+-rw-r--r--   0        0        0     3695 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state_v1.py
+-rw-r--r--   0        0        0     1449 2024-05-01 01:57:38.648906 stellar_sdk-9.4.0/stellar_sdk/xdr/pool_id.py
+-rw-r--r--   0        0        0     1297 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/precondition_type.py
+-rw-r--r--   0        0        0     3321 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/preconditions.py
+-rw-r--r--   0        0        0     6234 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/preconditions_v2.py
+-rw-r--r--   0        0        0     1816 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/price.py
+-rw-r--r--   0        0        0     2341 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/public_key.py
+-rw-r--r--   0        0        0     1218 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/public_key_type.py
+-rw-r--r--   0        0        0     1688 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_op.py
+-rw-r--r--   0        0        0     2995 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_result.py
+-rw-r--r--   0        0        0     1725 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_result_code.py
+-rw-r--r--   0        0        0     3486 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_op.py
+-rw-r--r--   0        0        0     2240 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
+-rw-r--r--   0        0        0     3420 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_result.py
+-rw-r--r--   0        0        0     1879 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py
+-rw-r--r--   0        0        0     1344 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_type.py
+-rw-r--r--   0        0        0     3227 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_address.py
+-rw-r--r--   0        0        0     1278 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_address_type.py
+-rw-r--r--   0        0        0     1522 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_bytes.py
+-rw-r--r--   0        0        0     2348 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_contract_instance.py
+-rw-r--r--   0        0        0     2622 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_env_meta_entry.py
+-rw-r--r--   0        0        0     1225 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_env_meta_kind.py
+-rw-r--r--   0        0        0     5920 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error.py
+-rw-r--r--   0        0        0     2258 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error_code.py
+-rw-r--r--   0        0        0     2100 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error_type.py
+-rw-r--r--   0        0        0     1929 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_map.py
+-rw-r--r--   0        0        0     1876 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_map_entry.py
+-rw-r--r--   0        0        0     2222 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_entry.py
+-rw-r--r--   0        0        0     1159 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_kind.py
+-rw-r--r--   0        0        0     1909 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_v0.py
+-rw-r--r--   0        0        0     1604 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_nonce_key.py
+-rw-r--r--   0        0        0     6096 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_entry.py
+-rw-r--r--   0        0        0     1545 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_entry_kind.py
+-rw-r--r--   0        0        0     2422 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_function_input_v0.py
+-rw-r--r--   0        0        0     3748 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_function_v0.py
+-rw-r--r--   0        0        0     2848 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type.py
+-rw-r--r--   0        0        0     1607 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_bytes_n.py
+-rw-r--r--   0        0        0    10391 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_def.py
+-rw-r--r--   0        0        0     2117 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_map.py
+-rw-r--r--   0        0        0     1761 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_option.py
+-rw-r--r--   0        0        0     2125 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_result.py
+-rw-r--r--   0        0        0     2267 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_tuple.py
+-rw-r--r--   0        0        0     1638 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_udt.py
+-rw-r--r--   0        0        0     1766 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_vec.py
+-rw-r--r--   0        0        0     2383 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_enum_case_v0.py
+-rw-r--r--   0        0        0     3144 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_enum_v0.py
+-rw-r--r--   0        0        0     2418 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_error_enum_case_v0.py
+-rw-r--r--   0        0        0     3205 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_error_enum_v0.py
+-rw-r--r--   0        0        0     2429 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_struct_field_v0.py
+-rw-r--r--   0        0        0     3194 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_struct_v0.py
+-rw-r--r--   0        0        0     2894 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_tuple_v0.py
+-rw-r--r--   0        0        0     3608 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0.py
+-rw-r--r--   0        0        0     1372 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0_kind.py
+-rw-r--r--   0        0        0     2077 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_void_v0.py
+-rw-r--r--   0        0        0     3156 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_v0.py
+-rw-r--r--   0        0        0     1514 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_string.py
+-rw-r--r--   0        0        0     1557 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_symbol.py
+-rw-r--r--   0        0        0    16109 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_val.py
+-rw-r--r--   0        0        0     3579 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_val_type.py
+-rw-r--r--   0        0        0     1903 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sc_vec.py
+-rw-r--r--   0        0        0     1989 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_ballot.py
+-rw-r--r--   0        0        0     2119 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_envelope.py
+-rw-r--r--   0        0        0     2177 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_history_entry.py
+-rw-r--r--   0        0        0     2897 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_history_entry_v0.py
+-rw-r--r--   0        0        0     3384 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_nomination.py
+-rw-r--r--   0        0        0     3464 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_quorum_set.py
+-rw-r--r--   0        0        0     3677 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement.py
+-rw-r--r--   0        0        0     3227 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_confirm.py
+-rw-r--r--   0        0        0     2683 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_externalize.py
+-rw-r--r--   0        0        0     5628 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_pledges.py
+-rw-r--r--   0        0        0     3953 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_prepare.py
+-rw-r--r--   0        0        0     1378 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_type.py
+-rw-r--r--   0        0        0     1693 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/send_more.py
+-rw-r--r--   0        0        0     2154 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/send_more_extended.py
+-rw-r--r--   0        0        0     1598 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/sequence_number.py
+-rw-r--r--   0        0        0     6626 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_op.py
+-rw-r--r--   0        0        0     4319 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_result.py
+-rw-r--r--   0        0        0     2616 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_result_code.py
+-rw-r--r--   0        0        0     2858 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_op.py
+-rw-r--r--   0        0        0     3407 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_result.py
+-rw-r--r--   0        0        0     2015 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py
+-rw-r--r--   0        0        0     1533 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signature.py
+-rw-r--r--   0        0        0     1611 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signature_hint.py
+-rw-r--r--   0        0        0     2378 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signed_survey_request_message.py
+-rw-r--r--   0        0        0     2416 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signed_survey_response_message.py
+-rw-r--r--   0        0        0     1964 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signer.py
+-rw-r--r--   0        0        0     5223 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key.py
+-rw-r--r--   0        0        0     2288 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
+-rw-r--r--   0        0        0     1536 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key_type.py
+-rw-r--r--   0        0        0     2463 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/simple_payment_result.py
+-rw-r--r--   0        0        0     3082 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_address_credentials.py
+-rw-r--r--   0        0        0     2478 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorization_entry.py
+-rw-r--r--   0        0        0     4111 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_function.py
+-rw-r--r--   0        0        0     1480 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_function_type.py
+-rw-r--r--   0        0        0     2958 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_invocation.py
+-rw-r--r--   0        0        0     2852 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_credentials.py
+-rw-r--r--   0        0        0     1360 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_credentials_type.py
+-rw-r--r--   0        0        0     3219 2024-05-01 01:57:38.652906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_resources.py
+-rw-r--r--   0        0        0     3230 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_data.py
+-rw-r--r--   0        0        0     4470 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_meta.py
+-rw-r--r--   0        0        0     2422 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_meta_ext.py
+-rw-r--r--   0        0        0     5477 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_meta_ext_v1.py
+-rw-r--r--   0        0        0     1974 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/sponsorship_descriptor.py
+-rw-r--r--   0        0        0     7248 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/state_archival_settings.py
+-rw-r--r--   0        0        0    17518 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_message.py
+-rw-r--r--   0        0        0     4020 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value.py
+-rw-r--r--   0        0        0     2852 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value_ext.py
+-rw-r--r--   0        0        0     1280 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value_type.py
+-rw-r--r--   0        0        0     2986 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stored_debug_transaction_set.py
+-rw-r--r--   0        0        0     3573 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/stored_transaction_set.py
+-rw-r--r--   0        0        0     1497 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/string32.py
+-rw-r--r--   0        0        0     1497 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/string64.py
+-rw-r--r--   0        0        0     1253 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/survey_message_command_type.py
+-rw-r--r--   0        0        0     1364 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/survey_message_response_type.py
+-rw-r--r--   0        0        0     3653 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/survey_request_message.py
+-rw-r--r--   0        0        0     4040 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/survey_response_body.py
+-rw-r--r--   0        0        0     3645 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/survey_response_message.py
+-rw-r--r--   0        0        0     1382 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/threshold_indexes.py
+-rw-r--r--   0        0        0     1546 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/thresholds.py
+-rw-r--r--   0        0        0     2063 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/time_bounds.py
+-rw-r--r--   0        0        0     1513 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/time_point.py
+-rw-r--r--   0        0        0     3409 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/topology_response_body_v0.py
+-rw-r--r--   0        0        0     4415 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/topology_response_body_v1.py
+-rw-r--r--   0        0        0     4750 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction.py
+-rw-r--r--   0        0        0     3899 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_envelope.py
+-rw-r--r--   0        0        0     2507 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_ext.py
+-rw-r--r--   0        0        0     2793 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_entry.py
+-rw-r--r--   0        0        0     2689 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_entry_ext.py
+-rw-r--r--   0        0        0     2892 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_result_entry.py
+-rw-r--r--   0        0        0     1798 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py
+-rw-r--r--   0        0        0     4548 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta.py
+-rw-r--r--   0        0        0     2816 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v1.py
+-rw-r--r--   0        0        0     3568 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v2.py
+-rw-r--r--   0        0        0     4682 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v3.py
+-rw-r--r--   0        0        0     2907 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_phase.py
+-rw-r--r--   0        0        0     3629 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result.py
+-rw-r--r--   0        0        0     3143 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_code.py
+-rw-r--r--   0        0        0     1726 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_ext.py
+-rw-r--r--   0        0        0     2874 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_meta.py
+-rw-r--r--   0        0        0     2306 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_pair.py
+-rw-r--r--   0        0        0     8349 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_result.py
+-rw-r--r--   0        0        0     2264 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_set.py
+-rw-r--r--   0        0        0     2691 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_set.py
+-rw-r--r--   0        0        0     2753 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_set_v1.py
+-rw-r--r--   0        0        0     2836 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_signature_payload.py
+-rw-r--r--   0        0        0     3373 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
+-rw-r--r--   0        0        0     4792 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0.py
+-rw-r--r--   0        0        0     2781 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0_envelope.py
+-rw-r--r--   0        0        0     1702 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0_ext.py
+-rw-r--r--   0        0        0     2770 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v1_envelope.py
+-rw-r--r--   0        0        0     4417 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_asset.py
+-rw-r--r--   0        0        0     4137 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry.py
+-rw-r--r--   0        0        0     2637 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_ext.py
+-rw-r--r--   0        0        0     2506 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py
+-rw-r--r--   0        0        0     1774 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
+-rw-r--r--   0        0        0     2370 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_v1.py
+-rw-r--r--   0        0        0     2421 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py
+-rw-r--r--   0        0        0     1742 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_flags.py
+-rw-r--r--   0        0        0     2284 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/ttl_entry.py
+-rw-r--r--   0        0        0     2215 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/tx_advert_vector.py
+-rw-r--r--   0        0        0     2215 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/tx_demand_vector.py
+-rw-r--r--   0        0        0     3020 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component.py
+-rw-r--r--   0        0        0     2792 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component_txs_maybe_discounted_fee.py
+-rw-r--r--   0        0        0     1399 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component_type.py
+-rw-r--r--   0        0        0     1863 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/u_int128_parts.py
+-rw-r--r--   0        0        0     2533 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/u_int256_parts.py
+-rw-r--r--   0        0        0     1495 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/uint256.py
+-rw-r--r--   0        0        0     1484 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/uint32.py
+-rw-r--r--   0        0        0     1480 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/uint64.py
+-rw-r--r--   0        0        0     2154 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/upgrade_entry_meta.py
+-rw-r--r--   0        0        0     1583 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/upgrade_type.py
+-rw-r--r--   0        0        0     1475 2024-05-01 01:57:38.656906 stellar_sdk-9.4.0/stellar_sdk/xdr/value.py
+-rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 stellar_sdk-9.4.0/PKG-INFO
```

### Comparing `stellar_sdk-9.3.0/LICENSE` & `stellar_sdk-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/README.rst` & `stellar_sdk-9.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/pyproject.toml` & `stellar_sdk-9.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stellar-sdk"
-version = "9.3.0"
+version = "9.4.0"
 description = "The Python Stellar SDK library provides APIs to build transactions and connect to Horizon and Soroban-RPC server."
 authors = [
     "overcat <4catcode@gmail.com>",
     "Eno <appweb.cn@gmail.com>"
 ]
 maintainers = ["overcat <4catcode@gmail.com>"]
 readme = "README.rst"
@@ -58,27 +58,27 @@
 xdrlib3 = "^0.1.1"
 requests-sse = "^0.3.0"
 
 [tool.poetry.extras]
 aiohttp = ["aiohttp", "aiohttp-sse-client"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.1.1"
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
 pytest-timeout = "^2.3.1"
-pytest-asyncio = "^0.23.5"
+pytest-asyncio = "^0.23.6"
 pytest-httpserver = "^1.0.10"
 # currently, mypy cannot run in pypy https://github.com/python/typed_ast/issues/111
-mypy = {version = "^1.9", markers = "platform_python_implementation == 'CPython'"}
+mypy = {version = "^1.10", markers = "platform_python_implementation == 'CPython'"}
 types-toml = {version = "^0.10.8", markers = "platform_python_implementation == 'CPython'"}
 types-requests = {version = "^2.31.0", markers = "platform_python_implementation == 'CPython'"}
 autoflake = "^2.3"
 isort = "^5.13.2"
-black = "^24.2.0"
-requests-mock = "^1.11.0"
+black = "^24.4.2"
+requests-mock = "^1.12.1"
 aioresponses = {git = "https://github.com/pnuckowski/aioresponses.git"}
 
 [tool.mypy]
 show_error_codes = true
 ignore_missing_imports = true
 warn_unused_configs = true
 no_implicit_optional = false
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/__version__.py` & `stellar_sdk-9.4.0/stellar_sdk/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
  |_____/   |_|  |______|______|______/_/    \_\_|  \_\    |_____/|_____/|_|\_\
 """
 
 __title__ = "stellar-sdk"
 __description__ = "The Python Stellar SDK library provides APIs to build transactions and connect to Horizon and Soroban-RPC server."
 __url__ = "https://github.com/StellarCN/py-stellar-base"
 __issues__ = f"{__url__}/issues"
-__version__ = "9.3.0"
+__version__ = "9.4.0"
 __author__ = "Eno, overcat"
 __author_email__ = "appweb.cn@gmail.com, 4catcode@gmail.com"
 __license__ = "Apache License 2.0"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/account.py` & `stellar_sdk-9.4.0/stellar_sdk/account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/address.py` & `stellar_sdk-9.4.0/stellar_sdk/address.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/asset.py` & `stellar_sdk-9.4.0/stellar_sdk/asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/auth.py` & `stellar_sdk-9.4.0/stellar_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/base_server.py` & `stellar_sdk-9.4.0/stellar_sdk/base_server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/base_soroban_server.py` & `stellar_sdk-9.4.0/stellar_sdk/base_soroban_server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/base_transaction_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/base_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_assets_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_data_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_effects_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_offers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_operations_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_payments_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_trades_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/aiohttp_client.py` & `stellar_sdk-9.4.0/stellar_sdk/client/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/base_async_client.py` & `stellar_sdk-9.4.0/stellar_sdk/client/base_async_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/base_sync_client.py` & `stellar_sdk-9.4.0/stellar_sdk/client/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/requests_client.py` & `stellar_sdk-9.4.0/stellar_sdk/client/requests_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/response.py` & `stellar_sdk-9.4.0/stellar_sdk/client/response.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/client/simple_requests_client.py` & `stellar_sdk-9.4.0/stellar_sdk/client/simple_requests_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/decorated_signature.py` & `stellar_sdk-9.4.0/stellar_sdk/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/exceptions.py` & `stellar_sdk-9.4.0/stellar_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/fee_bump_transaction.py` & `stellar_sdk-9.4.0/stellar_sdk/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/fee_bump_transaction_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/helpers.py` & `stellar_sdk-9.4.0/stellar_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/keypair.py` & `stellar_sdk-9.4.0/stellar_sdk/keypair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/ledger_bounds.py` & `stellar_sdk-9.4.0/stellar_sdk/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/liquidity_pool_asset.py` & `stellar_sdk-9.4.0/stellar_sdk/liquidity_pool_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/liquidity_pool_id.py` & `stellar_sdk-9.4.0/stellar_sdk/liquidity_pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/memo.py` & `stellar_sdk-9.4.0/stellar_sdk/memo.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/muxed_account.py` & `stellar_sdk-9.4.0/stellar_sdk/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/network.py` & `stellar_sdk-9.4.0/stellar_sdk/network.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/account_merge.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/account_merge.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/allow_trust.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/allow_trust.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/bump_sequence.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/bump_sequence.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/change_trust.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/change_trust.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/claim_claimable_balance.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/claim_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/clawback.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/clawback.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/clawback_claimable_balance.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/clawback_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/create_account.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/create_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/create_claimable_balance.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/create_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/create_passive_sell_offer.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/create_passive_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/end_sponsoring_future_reserves.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/end_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/extend_footprint_ttl.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/extend_footprint_ttl.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __all__ = ["ExtendFootprintTTL"]
 
 
 class ExtendFootprintTTL(Operation):
     """The :class:`ExtendFootprintTTL` object, which represents a ExtendFootprintTTL
     operation on Stellar's network.
 
-    Threshold: Medium
+    Threshold: Low
 
     See `ExtendFootprintTTLOp <https://soroban.stellar.org/docs/fundamentals-and-concepts/state-expiration#ExtendFootprintTTLop>`_.
 
     :param extend_to: The number of ledgers past the LCL (last closed ledger)
         by which to extend the validity of the ledger keys in this transaction.
     :param source: The source account for the operation. Defaults to the transaction's source account.
     """
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/inflation.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/inflation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/invoke_host_function.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/invoke_host_function.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/liquidity_pool_deposit.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/liquidity_pool_deposit.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/liquidity_pool_withdraw.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/liquidity_pool_withdraw.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/manage_buy_offer.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/manage_buy_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/manage_data.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/manage_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/manage_sell_offer.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/manage_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/operation.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/operation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/path_payment_strict_receive.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/path_payment_strict_receive.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/path_payment_strict_send.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/path_payment_strict_send.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/payment.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/payment.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/restore_footprint.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/restore_footprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __all__ = ["RestoreFootprint"]
 
 
 class RestoreFootprint(Operation):
     """The :class:`RestoreFootprint` object, which represents a RestoreFootprint
     operation on Stellar's network.
 
-    Threshold: Medium
+    Threshold: Low
 
     See `RestoreFootprintOp <https://soroban.stellar.org/docs/fundamentals-and-concepts/state-expiration#restorefootprintop>`_.
 
     :param source: The source account for the operation. Defaults to the transaction's source account.
     """
 
     _XDR_OPERATION_TYPE: stellar_xdr.OperationType = (
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/revoke_sponsorship.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/revoke_sponsorship.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/set_options.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/set_options.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/operation/set_trust_line_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/operation/set_trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/preconditions.py` & `stellar_sdk-9.4.0/stellar_sdk/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/price.py` & `stellar_sdk-9.4.0/stellar_sdk/price.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/scval.py` & `stellar_sdk-9.4.0/stellar_sdk/scval.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/ed25519_public_key_signer.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/ed25519_public_key_signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/exceptions.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/exceptions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/federation.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/federation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/mnemonic.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/mnemonic.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/stellar_toml.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/stellar_toml.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/stellar_uri.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/stellar_uri.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/stellar_web_authentication.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/stellar_web_authentication.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/toid.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/toid.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/sep/txrep.py` & `stellar_sdk-9.4.0/stellar_sdk/sep/txrep.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/server.py` & `stellar_sdk-9.4.0/stellar_sdk/server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/server_async.py` & `stellar_sdk-9.4.0/stellar_sdk/server_async.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/signer.py` & `stellar_sdk-9.4.0/stellar_sdk/signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/signer_key.py` & `stellar_sdk-9.4.0/stellar_sdk/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/soroban_data_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/soroban_data_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/soroban_rpc.py` & `stellar_sdk-9.4.0/stellar_sdk/soroban_rpc.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/soroban_server.py` & `stellar_sdk-9.4.0/stellar_sdk/soroban_server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/soroban_server_async.py` & `stellar_sdk-9.4.0/stellar_sdk/soroban_server_async.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/strkey.py` & `stellar_sdk-9.4.0/stellar_sdk/strkey.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/time_bounds.py` & `stellar_sdk-9.4.0/stellar_sdk/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/transaction.py` & `stellar_sdk-9.4.0/stellar_sdk/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/transaction_builder.py` & `stellar_sdk-9.4.0/stellar_sdk/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/transaction_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/utils.py` & `stellar_sdk-9.4.0/stellar_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/__init__.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,18 @@
 from .config_setting_contract_historical_data_v0 import *
 from .config_setting_contract_ledger_cost_v0 import *
 from .config_setting_entry import *
 from .config_setting_id import *
 from .config_upgrade_set import *
 from .config_upgrade_set_key import *
 from .constants import *
+from .contract_code_cost_inputs import *
 from .contract_code_entry import *
+from .contract_code_entry_ext import *
+from .contract_code_entry_v1 import *
 from .contract_cost_param_entry import *
 from .contract_cost_params import *
 from .contract_cost_type import *
 from .contract_data_durability import *
 from .contract_data_entry import *
 from .contract_event import *
 from .contract_event_body import *
@@ -154,14 +157,16 @@
 from .invoke_host_function_op import *
 from .invoke_host_function_result import *
 from .invoke_host_function_result_code import *
 from .invoke_host_function_success_pre_image import *
 from .ip_addr_type import *
 from .ledger_bounds import *
 from .ledger_close_meta import *
+from .ledger_close_meta_ext import *
+from .ledger_close_meta_ext_v1 import *
 from .ledger_close_meta_v0 import *
 from .ledger_close_meta_v1 import *
 from .ledger_close_value_signature import *
 from .ledger_entry import *
 from .ledger_entry_change import *
 from .ledger_entry_change_type import *
 from .ledger_entry_changes import *
@@ -346,14 +351,16 @@
 from .soroban_authorized_function_type import *
 from .soroban_authorized_invocation import *
 from .soroban_credentials import *
 from .soroban_credentials_type import *
 from .soroban_resources import *
 from .soroban_transaction_data import *
 from .soroban_transaction_meta import *
+from .soroban_transaction_meta_ext import *
+from .soroban_transaction_meta_ext_v1 import *
 from .sponsorship_descriptor import *
 from .state_archival_settings import *
 from .stellar_message import *
 from .stellar_value import *
 from .stellar_value_ext import *
 from .stellar_value_type import *
 from .stored_debug_transaction_set import *
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v2.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_entry_extension_v3.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_entry_extension_v3.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_merge_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_merge_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/account_merge_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/account_merge_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/allow_trust_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/allow_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/alpha_num12.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/alpha_num12.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/alpha_num4.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/alpha_num4.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/asset.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code12.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code12.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/asset_code4.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/asset_code4.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/asset_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/asset_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/auth.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/auth.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/auth_cert.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/auth_cert.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/authenticated_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/authenticated_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/authenticated_message_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/authenticated_message_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/base.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/base.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_entry_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_metadata.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_metadata.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bucket_metadata_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bucket_metadata_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/bump_sequence_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/bump_sequence_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_asset.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/change_trust_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/change_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_atom.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_atom_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_atom_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_liquidity_atom.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_liquidity_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_offer_atom.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_offer_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_offer_atom_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_offer_atom_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_predicate.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_predicate.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claim_predicate_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claim_predicate_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimable_balance_id_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimable_balance_id_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimant.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimant.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimant_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimant_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/claimant_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/claimant_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/clawback_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/clawback_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_bandwidth_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_bandwidth_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_compute_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_compute_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_events_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_events_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_execution_lanes_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_execution_lanes_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_historical_data_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_historical_data_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_contract_ledger_cost_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_contract_ledger_cost_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_setting_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_setting_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_upgrade_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_upgrade_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/config_upgrade_set_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/config_upgrade_set_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/constants.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/constants.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_code_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/int128_parts.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,96 +2,82 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .base import Opaque
-from .extension_point import ExtensionPoint
-from .hash import Hash
+from .int64 import Int64
+from .uint64 import Uint64
 
-__all__ = ["ContractCodeEntry"]
+__all__ = ["Int128Parts"]
 
 
-class ContractCodeEntry:
+class Int128Parts:
     """
     XDR Source Code::
 
-        struct ContractCodeEntry {
-            ExtensionPoint ext;
-
-            Hash hash;
-            opaque code<>;
+        struct Int128Parts {
+            int64 hi;
+            uint64 lo;
         };
     """
 
     def __init__(
         self,
-        ext: ExtensionPoint,
-        hash: Hash,
-        code: bytes,
+        hi: Int64,
+        lo: Uint64,
     ) -> None:
-        self.ext = ext
-        self.hash = hash
-        self.code = code
+        self.hi = hi
+        self.lo = lo
 
     def pack(self, packer: Packer) -> None:
-        self.ext.pack(packer)
-        self.hash.pack(packer)
-        Opaque(self.code, 4294967295, False).pack(packer)
+        self.hi.pack(packer)
+        self.lo.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> ContractCodeEntry:
-        ext = ExtensionPoint.unpack(unpacker)
-        hash = Hash.unpack(unpacker)
-        code = Opaque.unpack(unpacker, 4294967295, False)
+    def unpack(cls, unpacker: Unpacker) -> Int128Parts:
+        hi = Int64.unpack(unpacker)
+        lo = Uint64.unpack(unpacker)
         return cls(
-            ext=ext,
-            hash=hash,
-            code=code,
+            hi=hi,
+            lo=lo,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> ContractCodeEntry:
+    def from_xdr_bytes(cls, xdr: bytes) -> Int128Parts:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> ContractCodeEntry:
+    def from_xdr(cls, xdr: str) -> Int128Parts:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
         return hash(
             (
-                self.ext,
-                self.hash,
-                self.code,
+                self.hi,
+                self.lo,
             )
         )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return (
-            self.ext == other.ext
-            and self.hash == other.hash
-            and self.code == other.code
-        )
+        return self.hi == other.hi and self.lo == other.lo
 
     def __str__(self):
         out = [
-            f"ext={self.ext}",
-            f"hash={self.hash}",
-            f"code={self.code}",
+            f"hi={self.hi}",
+            f"lo={self.lo}",
         ]
-        return f"<ContractCodeEntry [{', '.join(out)}]>"
+        return f"<Int128Parts [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_cost_param_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_cost_param_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_cost_params.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_cost_params.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_data_durability.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_data_durability.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_data_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_data_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_body.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_event_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_event_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_executable.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_executable.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_executable_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_executable_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage_from_address.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage_from_address.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/contract_id_preimage_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_id_preimage_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_account_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_account_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_claimable_balance_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_contract_args.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_contract_args.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/create_passive_sell_offer_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/create_passive_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/crypto_key_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/crypto_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/curve25519_public.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/curve25519_public.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/curve25519_secret.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/curve25519_secret.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/data_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/data_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/data_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/data_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/data_value.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/data_value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/decorated_signature.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/diagnostic_event.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/diagnostic_event.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/dont_have.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/dont_have.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/duration.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/duration.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/encrypted_body.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/encrypted_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/envelope_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/envelope_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/error.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/error.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/error_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/error_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/eviction_iterator.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/eviction_iterator.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/extend_footprint_ttl_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/extend_footprint_ttl_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/extension_point.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/extension_point.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/flood_advert.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/flood_advert.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/flood_demand.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/flood_demand.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/generalized_transaction_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/generalized_transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_contract_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_contract_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hash_id_preimage_soroban_authorization.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hash_id_preimage_soroban_authorization.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hello.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hello.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hmac_sha256_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hmac_sha256_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/hmac_sha256_mac.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/hmac_sha256_mac.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/host_function.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/host_function.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/host_function_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/host_function_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_payout.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_payout.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inflation_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inflation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_pair.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/inner_transaction_result_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/inner_transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/int128_parts.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/price.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,82 +2,82 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .int64 import Int64
-from .uint64 import Uint64
+from .int32 import Int32
 
-__all__ = ["Int128Parts"]
+__all__ = ["Price"]
 
 
-class Int128Parts:
+class Price:
     """
     XDR Source Code::
 
-        struct Int128Parts {
-            int64 hi;
-            uint64 lo;
+        struct Price
+        {
+            int32 n; // numerator
+            int32 d; // denominator
         };
     """
 
     def __init__(
         self,
-        hi: Int64,
-        lo: Uint64,
+        n: Int32,
+        d: Int32,
     ) -> None:
-        self.hi = hi
-        self.lo = lo
+        self.n = n
+        self.d = d
 
     def pack(self, packer: Packer) -> None:
-        self.hi.pack(packer)
-        self.lo.pack(packer)
+        self.n.pack(packer)
+        self.d.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> Int128Parts:
-        hi = Int64.unpack(unpacker)
-        lo = Uint64.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> Price:
+        n = Int32.unpack(unpacker)
+        d = Int32.unpack(unpacker)
         return cls(
-            hi=hi,
-            lo=lo,
+            n=n,
+            d=d,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> Int128Parts:
+    def from_xdr_bytes(cls, xdr: bytes) -> Price:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> Int128Parts:
+    def from_xdr(cls, xdr: str) -> Price:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
         return hash(
             (
-                self.hi,
-                self.lo,
+                self.n,
+                self.d,
             )
         )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.hi == other.hi and self.lo == other.lo
+        return self.n == other.n and self.d == other.d
 
     def __str__(self):
         out = [
-            f"hi={self.hi}",
-            f"lo={self.lo}",
+            f"n={self.n}",
+            f"d={self.d}",
         ]
-        return f"<Int128Parts [{', '.join(out)}]>"
+        return f"<Price [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/int256_parts.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/int256_parts.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/int32.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/int32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/int64.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/int64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_contract_args.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_contract_args.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/invoke_host_function_success_pre_image.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/invoke_host_function_success_pre_image.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ip_addr_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ip_addr_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_bounds.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_meta_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_meta_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 
 import base64
 from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
-from .extension_point import ExtensionPoint
 from .generalized_transaction_set import GeneralizedTransactionSet
+from .ledger_close_meta_ext import LedgerCloseMetaExt
 from .ledger_entry import LedgerEntry
 from .ledger_header_history_entry import LedgerHeaderHistoryEntry
 from .ledger_key import LedgerKey
 from .scp_history_entry import SCPHistoryEntry
 from .transaction_result_meta import TransactionResultMeta
 from .uint64 import Uint64
 from .upgrade_entry_meta import UpgradeEntryMeta
@@ -22,17 +22,15 @@
 
 class LedgerCloseMetaV1:
     """
     XDR Source Code::
 
         struct LedgerCloseMetaV1
         {
-            // We forgot to add an ExtensionPoint in v0 but at least
-            // we can add one now in v1.
-            ExtensionPoint ext;
+            LedgerCloseMetaExt ext;
 
             LedgerHeaderHistoryEntry ledgerHeader;
 
             GeneralizedTransactionSet txSet;
 
             // NB: transactions are sorted in apply order here
             // fees for all transactions are processed first
@@ -56,15 +54,15 @@
             // evicted at this ledger.
             LedgerEntry evictedPersistentLedgerEntries<>;
         };
     """
 
     def __init__(
         self,
-        ext: ExtensionPoint,
+        ext: LedgerCloseMetaExt,
         ledger_header: LedgerHeaderHistoryEntry,
         tx_set: GeneralizedTransactionSet,
         tx_processing: List[TransactionResultMeta],
         upgrades_processing: List[UpgradeEntryMeta],
         scp_info: List[SCPHistoryEntry],
         total_byte_size_of_bucket_list: Uint64,
         evicted_temporary_ledger_keys: List[LedgerKey],
@@ -132,15 +130,15 @@
         for (
             evicted_persistent_ledger_entries_item
         ) in self.evicted_persistent_ledger_entries:
             evicted_persistent_ledger_entries_item.pack(packer)
 
     @classmethod
     def unpack(cls, unpacker: Unpacker) -> LedgerCloseMetaV1:
-        ext = ExtensionPoint.unpack(unpacker)
+        ext = LedgerCloseMetaExt.unpack(unpacker)
         ledger_header = LedgerHeaderHistoryEntry.unpack(unpacker)
         tx_set = GeneralizedTransactionSet.unpack(unpacker)
         length = unpacker.unpack_uint()
         tx_processing = []
         for _ in range(length):
             tx_processing.append(TransactionResultMeta.unpack(unpacker))
         length = unpacker.unpack_uint()
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_close_value_signature.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_close_value_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_change.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_change.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_change_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_change_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_changes.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_changes.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_data.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_extension_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_entry_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_footprint.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_footprint.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_extension_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_history_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_account.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_claimable_balance.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_config_setting.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_config_setting.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_contract_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_contract_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_contract_data.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_contract_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_data.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_offer.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_trust_line.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_trust_line.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_key_ttl.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_key_ttl.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_scp_messages.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_scp_messages.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_upgrade.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_upgrade.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ledger_upgrade_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ledger_upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liabilities.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liabilities.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry_body.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_parameters.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_buy_offer_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_buy_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_data_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_data_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_effect.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_effect.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_success_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_success_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_offer_success_result_offer.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_offer_success_result_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/manage_sell_offer_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/manage_sell_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/memo.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/memo.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/memo_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/memo_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/message_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/message_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/muxed_account.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/muxed_account_med25519.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/muxed_account_med25519.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/node_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/node_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/offer_entry_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/offer_entry_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_body.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_result_tr.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_result_tr.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/operation_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/operation_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/payment_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/payment_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/payment_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/payment_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/payment_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/peer_address.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/peer_address.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/peer_address_ip.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/peer_address_ip.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/peer_stat_list.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/peer_stat_list.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/peer_stats.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/peer_stats.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/persisted_scp_state_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/persisted_scp_state_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/pool_id.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/precondition_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/precondition_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/preconditions.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/preconditions_v2.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/preconditions_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/price.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_bytes_n.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,82 +2,70 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .int32 import Int32
+from .uint32 import Uint32
 
-__all__ = ["Price"]
+__all__ = ["SCSpecTypeBytesN"]
 
 
-class Price:
+class SCSpecTypeBytesN:
     """
     XDR Source Code::
 
-        struct Price
+        struct SCSpecTypeBytesN
         {
-            int32 n; // numerator
-            int32 d; // denominator
+            uint32 n;
         };
     """
 
     def __init__(
         self,
-        n: Int32,
-        d: Int32,
+        n: Uint32,
     ) -> None:
         self.n = n
-        self.d = d
 
     def pack(self, packer: Packer) -> None:
         self.n.pack(packer)
-        self.d.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> Price:
-        n = Int32.unpack(unpacker)
-        d = Int32.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeBytesN:
+        n = Uint32.unpack(unpacker)
         return cls(
             n=n,
-            d=d,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> Price:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeBytesN:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> Price:
+    def from_xdr(cls, xdr: str) -> SCSpecTypeBytesN:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash(
-            (
-                self.n,
-                self.d,
-            )
-        )
+        return hash((self.n,))
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.n == other.n and self.d == other.d
+        return self.n == other.n
 
     def __str__(self):
         out = [
             f"n={self.n}",
-            f"d={self.d}",
         ]
-        return f"<Price [{', '.join(out)}]>"
+        return f"<SCSpecTypeBytesN [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/public_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/public_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/public_key_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/public_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/restore_footprint_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/restore_footprint_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/revoke_sponsorship_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/revoke_sponsorship_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_address.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_address.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_address_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_address_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_bytes.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_bytes.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_contract_instance.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_contract_instance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_env_meta_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_env_meta_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_env_meta_kind.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_env_meta_kind.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_error_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_error_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_map.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_map.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_map_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_map_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_kind.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_kind.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_meta_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_meta_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_nonce_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_nonce_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_entry_kind.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_entry_kind.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_function_input_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_function_input_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_function_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_function_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_bytes_n.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_option.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,70 +2,70 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .uint32 import Uint32
+from .sc_spec_type_def import SCSpecTypeDef
 
-__all__ = ["SCSpecTypeBytesN"]
+__all__ = ["SCSpecTypeOption"]
 
 
-class SCSpecTypeBytesN:
+class SCSpecTypeOption:
     """
     XDR Source Code::
 
-        struct SCSpecTypeBytesN
+        struct SCSpecTypeOption
         {
-            uint32 n;
+            SCSpecTypeDef valueType;
         };
     """
 
     def __init__(
         self,
-        n: Uint32,
+        value_type: SCSpecTypeDef,
     ) -> None:
-        self.n = n
+        self.value_type = value_type
 
     def pack(self, packer: Packer) -> None:
-        self.n.pack(packer)
+        self.value_type.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeBytesN:
-        n = Uint32.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeOption:
+        value_type = SCSpecTypeDef.unpack(unpacker)
         return cls(
-            n=n,
+            value_type=value_type,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeBytesN:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeOption:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecTypeBytesN:
+    def from_xdr(cls, xdr: str) -> SCSpecTypeOption:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash((self.n,))
+        return hash((self.value_type,))
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.n == other.n
+        return self.value_type == other.value_type
 
     def __str__(self):
         out = [
-            f"n={self.n}",
+            f"value_type={self.value_type}",
         ]
-        return f"<SCSpecTypeBytesN [{', '.join(out)}]>"
+        return f"<SCSpecTypeOption [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_def.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_def.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_map.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_map.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_option.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_udt.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,70 +2,70 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .sc_spec_type_def import SCSpecTypeDef
+from .base import String
 
-__all__ = ["SCSpecTypeOption"]
+__all__ = ["SCSpecTypeUDT"]
 
 
-class SCSpecTypeOption:
+class SCSpecTypeUDT:
     """
     XDR Source Code::
 
-        struct SCSpecTypeOption
+        struct SCSpecTypeUDT
         {
-            SCSpecTypeDef valueType;
+            string name<60>;
         };
     """
 
     def __init__(
         self,
-        value_type: SCSpecTypeDef,
+        name: bytes,
     ) -> None:
-        self.value_type = value_type
+        self.name = name
 
     def pack(self, packer: Packer) -> None:
-        self.value_type.pack(packer)
+        String(self.name, 60).pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeOption:
-        value_type = SCSpecTypeDef.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeUDT:
+        name = String.unpack(unpacker)
         return cls(
-            value_type=value_type,
+            name=name,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeOption:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeUDT:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecTypeOption:
+    def from_xdr(cls, xdr: str) -> SCSpecTypeUDT:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash((self.value_type,))
+        return hash((self.name,))
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.value_type == other.value_type
+        return self.name == other.name
 
     def __str__(self):
         out = [
-            f"value_type={self.value_type}",
+            f"name={self.name}",
         ]
-        return f"<SCSpecTypeOption [{', '.join(out)}]>"
+        return f"<SCSpecTypeUDT [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_tuple.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_tuple.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_udt.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_struct_field_v0.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,69 +3,95 @@
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
 from .base import String
+from .constants import *
+from .sc_spec_type_def import SCSpecTypeDef
 
-__all__ = ["SCSpecTypeUDT"]
+__all__ = ["SCSpecUDTStructFieldV0"]
 
 
-class SCSpecTypeUDT:
+class SCSpecUDTStructFieldV0:
     """
     XDR Source Code::
 
-        struct SCSpecTypeUDT
+        struct SCSpecUDTStructFieldV0
         {
-            string name<60>;
+            string doc<SC_SPEC_DOC_LIMIT>;
+            string name<30>;
+            SCSpecTypeDef type;
         };
     """
 
     def __init__(
         self,
+        doc: bytes,
         name: bytes,
+        type: SCSpecTypeDef,
     ) -> None:
+        self.doc = doc
         self.name = name
+        self.type = type
 
     def pack(self, packer: Packer) -> None:
-        String(self.name, 60).pack(packer)
+        String(self.doc, SC_SPEC_DOC_LIMIT).pack(packer)
+        String(self.name, 30).pack(packer)
+        self.type.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecTypeUDT:
+    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTStructFieldV0:
+        doc = String.unpack(unpacker)
         name = String.unpack(unpacker)
+        type = SCSpecTypeDef.unpack(unpacker)
         return cls(
+            doc=doc,
             name=name,
+            type=type,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecTypeUDT:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTStructFieldV0:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecTypeUDT:
+    def from_xdr(cls, xdr: str) -> SCSpecUDTStructFieldV0:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash((self.name,))
+        return hash(
+            (
+                self.doc,
+                self.name,
+                self.type,
+            )
+        )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.name == other.name
+        return (
+            self.doc == other.doc
+            and self.name == other.name
+            and self.type == other.type
+        )
 
     def __str__(self):
         out = [
+            f"doc={self.doc}",
             f"name={self.name}",
+            f"type={self.type}",
         ]
-        return f"<SCSpecTypeUDT [{', '.join(out)}]>"
+        return f"<SCSpecUDTStructFieldV0 [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_type_vec.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_type_vec.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_enum_case_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_enum_case_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_enum_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_enum_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_error_enum_case_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_error_enum_case_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_error_enum_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_error_enum_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_struct_field_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_tuple_v0.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,87 @@
 # This is an automatically generated file.
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
+from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
 from .base import String
 from .constants import *
 from .sc_spec_type_def import SCSpecTypeDef
 
-__all__ = ["SCSpecUDTStructFieldV0"]
+__all__ = ["SCSpecUDTUnionCaseTupleV0"]
 
 
-class SCSpecUDTStructFieldV0:
+class SCSpecUDTUnionCaseTupleV0:
     """
     XDR Source Code::
 
-        struct SCSpecUDTStructFieldV0
+        struct SCSpecUDTUnionCaseTupleV0
         {
             string doc<SC_SPEC_DOC_LIMIT>;
-            string name<30>;
-            SCSpecTypeDef type;
+            string name<60>;
+            SCSpecTypeDef type<12>;
         };
     """
 
     def __init__(
         self,
         doc: bytes,
         name: bytes,
-        type: SCSpecTypeDef,
+        type: List[SCSpecTypeDef],
     ) -> None:
+        _expect_max_length = 12
+        if type and len(type) > _expect_max_length:
+            raise ValueError(
+                f"The maximum length of `type` should be {_expect_max_length}, but got {len(type)}."
+            )
         self.doc = doc
         self.name = name
         self.type = type
 
     def pack(self, packer: Packer) -> None:
         String(self.doc, SC_SPEC_DOC_LIMIT).pack(packer)
-        String(self.name, 30).pack(packer)
-        self.type.pack(packer)
+        String(self.name, 60).pack(packer)
+        packer.pack_uint(len(self.type))
+        for type_item in self.type:
+            type_item.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTStructFieldV0:
+    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTUnionCaseTupleV0:
         doc = String.unpack(unpacker)
         name = String.unpack(unpacker)
-        type = SCSpecTypeDef.unpack(unpacker)
+        length = unpacker.unpack_uint()
+        type = []
+        for _ in range(length):
+            type.append(SCSpecTypeDef.unpack(unpacker))
         return cls(
             doc=doc,
             name=name,
             type=type,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTStructFieldV0:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTUnionCaseTupleV0:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecUDTStructFieldV0:
+    def from_xdr(cls, xdr: str) -> SCSpecUDTUnionCaseTupleV0:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
         return hash(
             (
                 self.doc,
@@ -90,8 +101,8 @@
 
     def __str__(self):
         out = [
             f"doc={self.doc}",
             f"name={self.name}",
             f"type={self.type}",
         ]
-        return f"<SCSpecUDTStructFieldV0 [{', '.join(out)}]>"
+        return f"<SCSpecUDTUnionCaseTupleV0 [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_struct_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_struct_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_tuple_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_v0.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,104 +5,113 @@
 import base64
 from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
 from .base import String
 from .constants import *
-from .sc_spec_type_def import SCSpecTypeDef
+from .sc_spec_udt_union_case_v0 import SCSpecUDTUnionCaseV0
 
-__all__ = ["SCSpecUDTUnionCaseTupleV0"]
+__all__ = ["SCSpecUDTUnionV0"]
 
 
-class SCSpecUDTUnionCaseTupleV0:
+class SCSpecUDTUnionV0:
     """
     XDR Source Code::
 
-        struct SCSpecUDTUnionCaseTupleV0
+        struct SCSpecUDTUnionV0
         {
             string doc<SC_SPEC_DOC_LIMIT>;
+            string lib<80>;
             string name<60>;
-            SCSpecTypeDef type<12>;
+            SCSpecUDTUnionCaseV0 cases<50>;
         };
     """
 
     def __init__(
         self,
         doc: bytes,
+        lib: bytes,
         name: bytes,
-        type: List[SCSpecTypeDef],
+        cases: List[SCSpecUDTUnionCaseV0],
     ) -> None:
-        _expect_max_length = 12
-        if type and len(type) > _expect_max_length:
+        _expect_max_length = 50
+        if cases and len(cases) > _expect_max_length:
             raise ValueError(
-                f"The maximum length of `type` should be {_expect_max_length}, but got {len(type)}."
+                f"The maximum length of `cases` should be {_expect_max_length}, but got {len(cases)}."
             )
         self.doc = doc
+        self.lib = lib
         self.name = name
-        self.type = type
+        self.cases = cases
 
     def pack(self, packer: Packer) -> None:
         String(self.doc, SC_SPEC_DOC_LIMIT).pack(packer)
+        String(self.lib, 80).pack(packer)
         String(self.name, 60).pack(packer)
-        packer.pack_uint(len(self.type))
-        for type_item in self.type:
-            type_item.pack(packer)
+        packer.pack_uint(len(self.cases))
+        for cases_item in self.cases:
+            cases_item.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTUnionCaseTupleV0:
+    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTUnionV0:
         doc = String.unpack(unpacker)
+        lib = String.unpack(unpacker)
         name = String.unpack(unpacker)
         length = unpacker.unpack_uint()
-        type = []
+        cases = []
         for _ in range(length):
-            type.append(SCSpecTypeDef.unpack(unpacker))
+            cases.append(SCSpecUDTUnionCaseV0.unpack(unpacker))
         return cls(
             doc=doc,
+            lib=lib,
             name=name,
-            type=type,
+            cases=cases,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTUnionCaseTupleV0:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTUnionV0:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecUDTUnionCaseTupleV0:
+    def from_xdr(cls, xdr: str) -> SCSpecUDTUnionV0:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
         return hash(
             (
                 self.doc,
+                self.lib,
                 self.name,
-                self.type,
+                self.cases,
             )
         )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
         return (
             self.doc == other.doc
+            and self.lib == other.lib
             and self.name == other.name
-            and self.type == other.type
+            and self.cases == other.cases
         )
 
     def __str__(self):
         out = [
             f"doc={self.doc}",
+            f"lib={self.lib}",
             f"name={self.name}",
-            f"type={self.type}",
+            f"cases={self.cases}",
         ]
-        return f"<SCSpecUDTUnionCaseTupleV0 [{', '.join(out)}]>"
+        return f"<SCSpecUDTUnionV0 [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0_kind.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_v0_kind.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_case_void_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_spec_udt_union_case_void_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_spec_udt_union_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_vec.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,115 +3,69 @@
 from __future__ import annotations
 
 import base64
 from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
-from .base import String
-from .constants import *
-from .sc_spec_udt_union_case_v0 import SCSpecUDTUnionCaseV0
+from .sc_val import SCVal
 
-__all__ = ["SCSpecUDTUnionV0"]
+__all__ = ["SCVec"]
 
 
-class SCSpecUDTUnionV0:
+class SCVec:
     """
     XDR Source Code::
 
-        struct SCSpecUDTUnionV0
-        {
-            string doc<SC_SPEC_DOC_LIMIT>;
-            string lib<80>;
-            string name<60>;
-            SCSpecUDTUnionCaseV0 cases<50>;
-        };
+        typedef SCVal SCVec<>;
     """
 
-    def __init__(
-        self,
-        doc: bytes,
-        lib: bytes,
-        name: bytes,
-        cases: List[SCSpecUDTUnionCaseV0],
-    ) -> None:
-        _expect_max_length = 50
-        if cases and len(cases) > _expect_max_length:
+    def __init__(self, sc_vec: List[SCVal]) -> None:
+        _expect_max_length = 4294967295
+        if sc_vec and len(sc_vec) > _expect_max_length:
             raise ValueError(
-                f"The maximum length of `cases` should be {_expect_max_length}, but got {len(cases)}."
+                f"The maximum length of `sc_vec` should be {_expect_max_length}, but got {len(sc_vec)}."
             )
-        self.doc = doc
-        self.lib = lib
-        self.name = name
-        self.cases = cases
+        self.sc_vec = sc_vec
 
     def pack(self, packer: Packer) -> None:
-        String(self.doc, SC_SPEC_DOC_LIMIT).pack(packer)
-        String(self.lib, 80).pack(packer)
-        String(self.name, 60).pack(packer)
-        packer.pack_uint(len(self.cases))
-        for cases_item in self.cases:
-            cases_item.pack(packer)
+        packer.pack_uint(len(self.sc_vec))
+        for sc_vec_item in self.sc_vec:
+            sc_vec_item.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCSpecUDTUnionV0:
-        doc = String.unpack(unpacker)
-        lib = String.unpack(unpacker)
-        name = String.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> SCVec:
         length = unpacker.unpack_uint()
-        cases = []
+        sc_vec = []
         for _ in range(length):
-            cases.append(SCSpecUDTUnionCaseV0.unpack(unpacker))
-        return cls(
-            doc=doc,
-            lib=lib,
-            name=name,
-            cases=cases,
-        )
+            sc_vec.append(SCVal.unpack(unpacker))
+        return cls(sc_vec)
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCSpecUDTUnionV0:
+    def from_xdr_bytes(cls, xdr: bytes) -> SCVec:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCSpecUDTUnionV0:
+    def from_xdr(cls, xdr: str) -> SCVec:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash(
-            (
-                self.doc,
-                self.lib,
-                self.name,
-                self.cases,
-            )
-        )
+        return hash(self.sc_vec)
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return (
-            self.doc == other.doc
-            and self.lib == other.lib
-            and self.name == other.name
-            and self.cases == other.cases
-        )
+        return self.sc_vec == other.sc_vec
 
     def __str__(self):
-        out = [
-            f"doc={self.doc}",
-            f"lib={self.lib}",
-            f"name={self.name}",
-            f"cases={self.cases}",
-        ]
-        return f"<SCSpecUDTUnionV0 [{', '.join(out)}]>"
+        return f"<SCVec [sc_vec={self.sc_vec}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_string.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_string.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_symbol.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_symbol.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_val.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_val.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_val_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sc_val_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sc_vec.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/u_int128_parts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 # This is an automatically generated file.
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
-from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
-from .sc_val import SCVal
+from .uint64 import Uint64
 
-__all__ = ["SCVec"]
+__all__ = ["UInt128Parts"]
 
 
-class SCVec:
+class UInt128Parts:
     """
     XDR Source Code::
 
-        typedef SCVal SCVec<>;
+        struct UInt128Parts {
+            uint64 hi;
+            uint64 lo;
+        };
     """
 
-    def __init__(self, sc_vec: List[SCVal]) -> None:
-        _expect_max_length = 4294967295
-        if sc_vec and len(sc_vec) > _expect_max_length:
-            raise ValueError(
-                f"The maximum length of `sc_vec` should be {_expect_max_length}, but got {len(sc_vec)}."
-            )
-        self.sc_vec = sc_vec
+    def __init__(
+        self,
+        hi: Uint64,
+        lo: Uint64,
+    ) -> None:
+        self.hi = hi
+        self.lo = lo
 
     def pack(self, packer: Packer) -> None:
-        packer.pack_uint(len(self.sc_vec))
-        for sc_vec_item in self.sc_vec:
-            sc_vec_item.pack(packer)
+        self.hi.pack(packer)
+        self.lo.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> SCVec:
-        length = unpacker.unpack_uint()
-        sc_vec = []
-        for _ in range(length):
-            sc_vec.append(SCVal.unpack(unpacker))
-        return cls(sc_vec)
+    def unpack(cls, unpacker: Unpacker) -> UInt128Parts:
+        hi = Uint64.unpack(unpacker)
+        lo = Uint64.unpack(unpacker)
+        return cls(
+            hi=hi,
+            lo=lo,
+        )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> SCVec:
+    def from_xdr_bytes(cls, xdr: bytes) -> UInt128Parts:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> SCVec:
+    def from_xdr(cls, xdr: str) -> UInt128Parts:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
-        return hash(self.sc_vec)
+        return hash(
+            (
+                self.hi,
+                self.lo,
+            )
+        )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.sc_vec == other.sc_vec
+        return self.hi == other.hi and self.lo == other.lo
 
     def __str__(self):
-        return f"<SCVec [sc_vec={self.sc_vec}]>"
+        out = [
+            f"hi={self.hi}",
+            f"lo={self.lo}",
+        ]
+        return f"<UInt128Parts [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_ballot.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_ballot.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_history_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_history_entry_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_history_entry_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_nomination.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_nomination.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_quorum_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_quorum_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_confirm.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_confirm.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_externalize.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_externalize.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_pledges.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_pledges.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_prepare.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_prepare.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/scp_statement_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/scp_statement_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/send_more.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/send_more.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/send_more_extended.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/send_more_extended.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sequence_number.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sequence_number.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_options_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_options_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_op.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signature.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signature_hint.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signature_hint.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signed_survey_request_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signed_survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signed_survey_response_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signed_survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signer.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/signer_key_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/signer_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/simple_payment_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/simple_payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_address_credentials.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_address_credentials.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorization_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorization_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_function.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_function.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_function_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_function_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_authorized_invocation.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_authorized_invocation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_credentials.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_credentials.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_credentials_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_credentials_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_resources.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_resources.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_transaction_data.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/soroban_transaction_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/soroban_transaction_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 import base64
 from typing import List
 
 from xdrlib3 import Packer, Unpacker
 
 from .contract_event import ContractEvent
 from .diagnostic_event import DiagnosticEvent
-from .extension_point import ExtensionPoint
 from .sc_val import SCVal
+from .soroban_transaction_meta_ext import SorobanTransactionMetaExt
 
 __all__ = ["SorobanTransactionMeta"]
 
 
 class SorobanTransactionMeta:
     """
     XDR Source Code::
 
         struct SorobanTransactionMeta
         {
-            ExtensionPoint ext;
+            SorobanTransactionMetaExt ext;
 
             ContractEvent events<>;             // custom events populated by the
                                                 // contracts themselves.
             SCVal returnValue;                  // return value of the host fn invocation
 
             // Diagnostics events that are not hashed.
             // This will contain all contract and diagnostic events. Even ones
             // that were emitted in a failed contract call.
             DiagnosticEvent diagnosticEvents<>;
         };
     """
 
     def __init__(
         self,
-        ext: ExtensionPoint,
+        ext: SorobanTransactionMetaExt,
         events: List[ContractEvent],
         return_value: SCVal,
         diagnostic_events: List[DiagnosticEvent],
     ) -> None:
         _expect_max_length = 4294967295
         if events and len(events) > _expect_max_length:
             raise ValueError(
@@ -64,15 +64,15 @@
         self.return_value.pack(packer)
         packer.pack_uint(len(self.diagnostic_events))
         for diagnostic_events_item in self.diagnostic_events:
             diagnostic_events_item.pack(packer)
 
     @classmethod
     def unpack(cls, unpacker: Unpacker) -> SorobanTransactionMeta:
-        ext = ExtensionPoint.unpack(unpacker)
+        ext = SorobanTransactionMetaExt.unpack(unpacker)
         length = unpacker.unpack_uint()
         events = []
         for _ in range(length):
             events.append(ContractEvent.unpack(unpacker))
         return_value = SCVal.unpack(unpacker)
         length = unpacker.unpack_uint()
         diagnostic_events = []
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/sponsorship_descriptor.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/sponsorship_descriptor.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/state_archival_settings.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/state_archival_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
 from .int64 import Int64
 from .uint32 import Uint32
-from .uint64 import Uint64
 
 __all__ = ["StateArchivalSettings"]
 
 
 class StateArchivalSettings:
     """
     XDR Source Code::
@@ -28,16 +27,19 @@
 
             // max number of entries that emit archival meta in a single ledger
             uint32 maxEntriesToArchive;
 
             // Number of snapshots to use when calculating average BucketList size
             uint32 bucketListSizeWindowSampleSize;
 
+            // How often to sample the BucketList size for the average, in ledgers
+            uint32 bucketListWindowSamplePeriod;
+
             // Maximum number of bytes that we scan for eviction per ledger
-            uint64 evictionScanSize;
+            uint32 evictionScanSize;
 
             // Lowest BucketList level to be scanned to evict entries
             uint32 startingEvictionScanLevel;
         };
     """
 
     def __init__(
@@ -45,57 +47,62 @@
         max_entry_ttl: Uint32,
         min_temporary_ttl: Uint32,
         min_persistent_ttl: Uint32,
         persistent_rent_rate_denominator: Int64,
         temp_rent_rate_denominator: Int64,
         max_entries_to_archive: Uint32,
         bucket_list_size_window_sample_size: Uint32,
-        eviction_scan_size: Uint64,
+        bucket_list_window_sample_period: Uint32,
+        eviction_scan_size: Uint32,
         starting_eviction_scan_level: Uint32,
     ) -> None:
         self.max_entry_ttl = max_entry_ttl
         self.min_temporary_ttl = min_temporary_ttl
         self.min_persistent_ttl = min_persistent_ttl
         self.persistent_rent_rate_denominator = persistent_rent_rate_denominator
         self.temp_rent_rate_denominator = temp_rent_rate_denominator
         self.max_entries_to_archive = max_entries_to_archive
         self.bucket_list_size_window_sample_size = bucket_list_size_window_sample_size
+        self.bucket_list_window_sample_period = bucket_list_window_sample_period
         self.eviction_scan_size = eviction_scan_size
         self.starting_eviction_scan_level = starting_eviction_scan_level
 
     def pack(self, packer: Packer) -> None:
         self.max_entry_ttl.pack(packer)
         self.min_temporary_ttl.pack(packer)
         self.min_persistent_ttl.pack(packer)
         self.persistent_rent_rate_denominator.pack(packer)
         self.temp_rent_rate_denominator.pack(packer)
         self.max_entries_to_archive.pack(packer)
         self.bucket_list_size_window_sample_size.pack(packer)
+        self.bucket_list_window_sample_period.pack(packer)
         self.eviction_scan_size.pack(packer)
         self.starting_eviction_scan_level.pack(packer)
 
     @classmethod
     def unpack(cls, unpacker: Unpacker) -> StateArchivalSettings:
         max_entry_ttl = Uint32.unpack(unpacker)
         min_temporary_ttl = Uint32.unpack(unpacker)
         min_persistent_ttl = Uint32.unpack(unpacker)
         persistent_rent_rate_denominator = Int64.unpack(unpacker)
         temp_rent_rate_denominator = Int64.unpack(unpacker)
         max_entries_to_archive = Uint32.unpack(unpacker)
         bucket_list_size_window_sample_size = Uint32.unpack(unpacker)
-        eviction_scan_size = Uint64.unpack(unpacker)
+        bucket_list_window_sample_period = Uint32.unpack(unpacker)
+        eviction_scan_size = Uint32.unpack(unpacker)
         starting_eviction_scan_level = Uint32.unpack(unpacker)
         return cls(
             max_entry_ttl=max_entry_ttl,
             min_temporary_ttl=min_temporary_ttl,
             min_persistent_ttl=min_persistent_ttl,
             persistent_rent_rate_denominator=persistent_rent_rate_denominator,
             temp_rent_rate_denominator=temp_rent_rate_denominator,
             max_entries_to_archive=max_entries_to_archive,
             bucket_list_size_window_sample_size=bucket_list_size_window_sample_size,
+            bucket_list_window_sample_period=bucket_list_window_sample_period,
             eviction_scan_size=eviction_scan_size,
             starting_eviction_scan_level=starting_eviction_scan_level,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
@@ -121,14 +128,15 @@
                 self.max_entry_ttl,
                 self.min_temporary_ttl,
                 self.min_persistent_ttl,
                 self.persistent_rent_rate_denominator,
                 self.temp_rent_rate_denominator,
                 self.max_entries_to_archive,
                 self.bucket_list_size_window_sample_size,
+                self.bucket_list_window_sample_period,
                 self.eviction_scan_size,
                 self.starting_eviction_scan_level,
             )
         )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
@@ -139,24 +147,27 @@
             and self.min_persistent_ttl == other.min_persistent_ttl
             and self.persistent_rent_rate_denominator
             == other.persistent_rent_rate_denominator
             and self.temp_rent_rate_denominator == other.temp_rent_rate_denominator
             and self.max_entries_to_archive == other.max_entries_to_archive
             and self.bucket_list_size_window_sample_size
             == other.bucket_list_size_window_sample_size
+            and self.bucket_list_window_sample_period
+            == other.bucket_list_window_sample_period
             and self.eviction_scan_size == other.eviction_scan_size
             and self.starting_eviction_scan_level == other.starting_eviction_scan_level
         )
 
     def __str__(self):
         out = [
             f"max_entry_ttl={self.max_entry_ttl}",
             f"min_temporary_ttl={self.min_temporary_ttl}",
             f"min_persistent_ttl={self.min_persistent_ttl}",
             f"persistent_rent_rate_denominator={self.persistent_rent_rate_denominator}",
             f"temp_rent_rate_denominator={self.temp_rent_rate_denominator}",
             f"max_entries_to_archive={self.max_entries_to_archive}",
             f"bucket_list_size_window_sample_size={self.bucket_list_size_window_sample_size}",
+            f"bucket_list_window_sample_period={self.bucket_list_window_sample_period}",
             f"eviction_scan_size={self.eviction_scan_size}",
             f"starting_eviction_scan_level={self.starting_eviction_scan_level}",
         ]
         return f"<StateArchivalSettings [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stellar_value_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stellar_value_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stored_debug_transaction_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stored_debug_transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/stored_transaction_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/stored_transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/string32.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/string32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/string64.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/string64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/survey_message_command_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/survey_message_command_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/survey_message_response_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/survey_message_response_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/survey_request_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/survey_response_body.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/survey_response_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/survey_response_message.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/threshold_indexes.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/threshold_indexes.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/thresholds.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/thresholds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/time_bounds.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/time_point.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/time_point.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/topology_response_body_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/topology_response_body_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/topology_response_body_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/topology_response_body_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_result_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_result_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v2.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_meta_v3.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_meta_v3.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_phase.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_phase.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_code.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_pair.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_result.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_result_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_result_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_set.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_set_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_set_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_signature_payload.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_signature_payload.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v0_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v0_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/transaction_v1_envelope.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/transaction_v1_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_asset.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_v1.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/trust_line_flags.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/ttl_entry.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/ttl_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/tx_advert_vector.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/tx_advert_vector.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/tx_demand_vector.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/tx_demand_vector.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component_txs_maybe_discounted_fee.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component_txs_maybe_discounted_fee.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/tx_set_component_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/tx_set_component_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/u_int128_parts.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/contract_code_entry_v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,81 +2,83 @@
 # DO NOT EDIT or your changes may be overwritten
 from __future__ import annotations
 
 import base64
 
 from xdrlib3 import Packer, Unpacker
 
-from .uint64 import Uint64
+from .contract_code_cost_inputs import ContractCodeCostInputs
+from .extension_point import ExtensionPoint
 
-__all__ = ["UInt128Parts"]
+__all__ = ["ContractCodeEntryV1"]
 
 
-class UInt128Parts:
+class ContractCodeEntryV1:
     """
     XDR Source Code::
 
-        struct UInt128Parts {
-            uint64 hi;
-            uint64 lo;
-        };
+        struct
+                    {
+                        ExtensionPoint ext;
+                        ContractCodeCostInputs costInputs;
+                    }
     """
 
     def __init__(
         self,
-        hi: Uint64,
-        lo: Uint64,
+        ext: ExtensionPoint,
+        cost_inputs: ContractCodeCostInputs,
     ) -> None:
-        self.hi = hi
-        self.lo = lo
+        self.ext = ext
+        self.cost_inputs = cost_inputs
 
     def pack(self, packer: Packer) -> None:
-        self.hi.pack(packer)
-        self.lo.pack(packer)
+        self.ext.pack(packer)
+        self.cost_inputs.pack(packer)
 
     @classmethod
-    def unpack(cls, unpacker: Unpacker) -> UInt128Parts:
-        hi = Uint64.unpack(unpacker)
-        lo = Uint64.unpack(unpacker)
+    def unpack(cls, unpacker: Unpacker) -> ContractCodeEntryV1:
+        ext = ExtensionPoint.unpack(unpacker)
+        cost_inputs = ContractCodeCostInputs.unpack(unpacker)
         return cls(
-            hi=hi,
-            lo=lo,
+            ext=ext,
+            cost_inputs=cost_inputs,
         )
 
     def to_xdr_bytes(self) -> bytes:
         packer = Packer()
         self.pack(packer)
         return packer.get_buffer()
 
     @classmethod
-    def from_xdr_bytes(cls, xdr: bytes) -> UInt128Parts:
+    def from_xdr_bytes(cls, xdr: bytes) -> ContractCodeEntryV1:
         unpacker = Unpacker(xdr)
         return cls.unpack(unpacker)
 
     def to_xdr(self) -> str:
         xdr_bytes = self.to_xdr_bytes()
         return base64.b64encode(xdr_bytes).decode()
 
     @classmethod
-    def from_xdr(cls, xdr: str) -> UInt128Parts:
+    def from_xdr(cls, xdr: str) -> ContractCodeEntryV1:
         xdr_bytes = base64.b64decode(xdr.encode())
         return cls.from_xdr_bytes(xdr_bytes)
 
     def __hash__(self):
         return hash(
             (
-                self.hi,
-                self.lo,
+                self.ext,
+                self.cost_inputs,
             )
         )
 
     def __eq__(self, other: object):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.hi == other.hi and self.lo == other.lo
+        return self.ext == other.ext and self.cost_inputs == other.cost_inputs
 
     def __str__(self):
         out = [
-            f"hi={self.hi}",
-            f"lo={self.lo}",
+            f"ext={self.ext}",
+            f"cost_inputs={self.cost_inputs}",
         ]
-        return f"<UInt128Parts [{', '.join(out)}]>"
+        return f"<ContractCodeEntryV1 [{', '.join(out)}]>"
```

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/u_int256_parts.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/u_int256_parts.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/uint256.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/uint256.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/uint32.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/uint32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/uint64.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/uint64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/upgrade_entry_meta.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/upgrade_entry_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/upgrade_type.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/stellar_sdk/xdr/value.py` & `stellar_sdk-9.4.0/stellar_sdk/xdr/value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-9.3.0/PKG-INFO` & `stellar_sdk-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-sdk
-Version: 9.3.0
+Version: 9.4.0
 Summary: The Python Stellar SDK library provides APIs to build transactions and connect to Horizon and Soroban-RPC server.
 Home-page: https://github.com/StellarCN/py-stellar-base
 License: Apache-2.0
 Keywords: stellar-sdk,stellar,stellar.org,lumens,xlm,blockchain,distributed exchange,cryptocurrency,dex,horizon,soroban,sdex,trading,soroban,soroban-rpc
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
```

