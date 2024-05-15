# Comparing `tmp/lightspark-2.7.0.zip` & `tmp/lightspark-2.7.1.zip`

## zipinfo {}

```diff
@@ -1,228 +1,228 @@
 Zip file size: 223043 bytes, number of entries: 226
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/
--rw-r--r--  2.0 unx    11352 b- defN 24-May-14 02:48 lightspark-2.7.0/LICENSE
--rwxr-xr-x  2.0 unx       87 b- defN 24-May-14 02:48 lightspark-2.7.0/setup.py
--rw-r--r--  2.0 unx     1035 b- defN 24-May-14 02:48 lightspark-2.7.0/README.md
--rw-r--r--  2.0 unx       81 b- defN 24-May-14 02:48 lightspark-2.7.0/pyproject.toml
--rw-r--r--  2.0 unx      750 b- defN 24-May-14 02:48 lightspark-2.7.0/setup.cfg
--rw-r--r--  2.0 unx     1630 b- defN 24-May-14 02:48 lightspark-2.7.0/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/
--rw-r--r--  2.0 unx        0 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/py.typed
--rw-r--r--  2.0 unx       22 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/version.py
--rw-r--r--  2.0 unx    35091 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/lightspark_client.py
--rw-r--r--  2.0 unx    12874 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/__init__.py
--rw-r--r--  2.0 unx      185 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/exceptions.py
--rw-r--r--  2.0 unx     2354 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/webhooks.py
--rw-r--r--  2.0 unx     1038 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/remote_signing.py
--rw-r--r--  2.0 unx      912 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py
--rw-r--r--  2.0 unx     6800 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py
--rw-r--r--  2.0 unx    20571 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/InvoiceData.py
--rw-r--r--  2.0 unx     3170 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
--rw-r--r--  2.0 unx      999 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionStatus.py
--rw-r--r--  2.0 unx    32826 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPayment.py
--rw-r--r--  2.0 unx      949 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py
--rw-r--r--  2.0 unx      635 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py
--rw-r--r--  2.0 unx      543 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/InvoiceType.py
--rw-r--r--  2.0 unx     2688 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
--rw-r--r--  2.0 unx     1086 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
--rw-r--r--  2.0 unx     2585 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
--rw-r--r--  2.0 unx      551 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
--rw-r--r--  2.0 unx      951 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py
--rw-r--r--  2.0 unx     1824 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RequestWithdrawalInput.py
--rw-r--r--  2.0 unx      823 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py
--rw-r--r--  2.0 unx      964 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Permission.py
--rw-r--r--  2.0 unx     1206 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py
--rw-r--r--  2.0 unx     1080 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
--rw-r--r--  2.0 unx      769 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FailHtlcsOutput.py
--rw-r--r--  2.0 unx     1519 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SendPaymentInput.py
--rw-r--r--  2.0 unx      633 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py
--rw-r--r--  2.0 unx      801 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py
--rw-r--r--  2.0 unx     5777 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Withdrawal.py
--rw-r--r--  2.0 unx     1299 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py
--rw-r--r--  2.0 unx     1833 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py
--rw-r--r--  2.0 unx     6010 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CurrencyAmount.py
--rw-r--r--  2.0 unx    48408 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Transaction.py
--rw-r--r--  2.0 unx      640 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IdAndSignature.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
--rw-r--r--  2.0 unx     2773 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
--rw-r--r--  2.0 unx     1613 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletStatus.py
--rw-r--r--  2.0 unx    10741 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Connection.py
--rw-r--r--  2.0 unx      847 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py
--rw-r--r--  2.0 unx      527 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalMode.py
--rw-r--r--  2.0 unx      659 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
--rw-r--r--  2.0 unx    27441 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Node.py
--rw-r--r--  2.0 unx     6193 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/BlockchainBalance.py
--rw-r--r--  2.0 unx     3872 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py
--rw-r--r--  2.0 unx     1563 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py
--rw-r--r--  2.0 unx     2777 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
--rw-r--r--  2.0 unx      655 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py
--rw-r--r--  2.0 unx     1138 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
--rw-r--r--  2.0 unx      497 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignablePayloadStatus.py
--rw-r--r--  2.0 unx     1591 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py
--rw-r--r--  2.0 unx    85008 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Wallet.py
--rw-r--r--  2.0 unx     3170 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
--rw-r--r--  2.0 unx      647 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RichText.py
--rw-r--r--  2.0 unx     1286 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py
--rw-r--r--  2.0 unx    18534 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py
--rw-r--r--  2.0 unx     1293 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
--rw-r--r--  2.0 unx     1119 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WebhookEventType.py
--rw-r--r--  2.0 unx     1745 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PostTransactionData.py
--rw-r--r--  2.0 unx     2635 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py
--rw-r--r--  2.0 unx      873 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignMessagesInput.py
--rw-r--r--  2.0 unx     2464 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py
--rw-r--r--  2.0 unx     1240 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py
--rw-r--r--  2.0 unx     1417 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Signable.py
--rw-r--r--  2.0 unx      577 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FundNodeOutput.py
--rw-r--r--  2.0 unx     2018 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FeeEstimate.py
--rw-r--r--  2.0 unx     5126 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/GraphNode.py
--rw-r--r--  2.0 unx     9474 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPayment.py
--rw-r--r--  2.0 unx     2518 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py
--rw-r--r--  2.0 unx      644 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py
--rw-r--r--  2.0 unx     1671 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py
--rw-r--r--  2.0 unx      470 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentDirection.py
--rw-r--r--  2.0 unx      864 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
--rw-r--r--  2.0 unx     1310 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
--rw-r--r--  2.0 unx    88288 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Entity.py
--rw-r--r--  2.0 unx      892 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py
--rw-r--r--  2.0 unx      819 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py
--rw-r--r--  2.0 unx     3242 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
--rw-r--r--  2.0 unx      849 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py
--rw-r--r--  2.0 unx     2227 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py
--rw-r--r--  2.0 unx     2893 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ApiToken.py
--rw-r--r--  2.0 unx     3618 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UmaInvitation.py
--rw-r--r--  2.0 unx   125678 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Account.py
--rw-r--r--  2.0 unx     2597 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py
--rw-r--r--  2.0 unx      812 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py
--rw-r--r--  2.0 unx     6939 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RoutingTransaction.py
--rw-r--r--  2.0 unx     5785 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py
--rw-r--r--  2.0 unx     1491 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelStatus.py
--rw-r--r--  2.0 unx     1783 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
--rw-r--r--  2.0 unx      630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py
--rw-r--r--  2.0 unx     5663 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Deposit.py
--rw-r--r--  2.0 unx     1180 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
--rw-r--r--  2.0 unx     1927 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py
--rw-r--r--  2.0 unx    14407 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/all_entities.py
--rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/__init__.py
--rw-r--r--  2.0 unx    22092 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Invoice.py
--rw-r--r--  2.0 unx      511 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequestStatus.py
--rw-r--r--  2.0 unx     1195 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py
--rw-r--r--  2.0 unx    18952 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegionCode.py
--rw-r--r--  2.0 unx      900 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py
--rw-r--r--  2.0 unx      935 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py
--rw-r--r--  2.0 unx     1392 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py
--rw-r--r--  2.0 unx     1748 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionType.py
--rw-r--r--  2.0 unx     1141 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeAddress.py
--rw-r--r--  2.0 unx     1668 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelFees.py
--rw-r--r--  2.0 unx     4273 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py
--rw-r--r--  2.0 unx     3123 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignablePayload.py
--rw-r--r--  2.0 unx      990 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
--rw-r--r--  2.0 unx      844 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FailHtlcsInput.py
--rw-r--r--  2.0 unx     2793 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
--rw-r--r--  2.0 unx      937 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py
--rw-r--r--  2.0 unx     4269 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Hop.py
--rw-r--r--  2.0 unx      904 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py
--rw-r--r--  2.0 unx    10172 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py
--rw-r--r--  2.0 unx      711 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py
--rw-r--r--  2.0 unx     2756 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
--rw-r--r--  2.0 unx      811 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncentivesStatus.py
--rw-r--r--  2.0 unx    23513 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequest.py
--rw-r--r--  2.0 unx    21264 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequestData.py
--rw-r--r--  2.0 unx     1424 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
--rw-r--r--  2.0 unx     1004 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CurrencyUnit.py
--rw-r--r--  2.0 unx     3984 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Balances.py
--rw-r--r--  2.0 unx     2619 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Secret.py
--rw-r--r--  2.0 unx     1172 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py
--rw-r--r--  2.0 unx     6589 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py
--rw-r--r--  2.0 unx     2497 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py
--rw-r--r--  2.0 unx     1807 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py
--rw-r--r--  2.0 unx      519 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeAddressType.py
--rw-r--r--  2.0 unx      969 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py
--rw-r--r--  2.0 unx     1483 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py
--rw-r--r--  2.0 unx      877 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py
--rw-r--r--  2.0 unx     2504 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AuditLogActor.py
--rw-r--r--  2.0 unx     2441 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
--rw-r--r--  2.0 unx     1410 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py
--rw-r--r--  2.0 unx      513 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py
--rw-r--r--  2.0 unx    39085 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNode.py
--rw-r--r--  2.0 unx      619 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RiskRating.py
--rw-r--r--  2.0 unx     1493 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
--rw-r--r--  2.0 unx    27341 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
--rw-r--r--  2.0 unx     6803 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py
--rw-r--r--  2.0 unx     1316 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py
--rw-r--r--  2.0 unx    24929 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
--rw-r--r--  2.0 unx     1021 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py
--rw-r--r--  2.0 unx     2980 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
--rw-r--r--  2.0 unx     1789 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
--rw-r--r--  2.0 unx      535 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py
--rw-r--r--  2.0 unx    27489 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py
--rw-r--r--  2.0 unx    15650 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Channel.py
--rw-r--r--  2.0 unx      615 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FundNodeInput.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionFailures.py
--rw-r--r--  2.0 unx     1709 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py
--rw-r--r--  2.0 unx      462 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ComplianceProvider.py
--rw-r--r--  2.0 unx     1517 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PageInfo.py
--rw-r--r--  2.0 unx      948 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py
--rw-r--r--  2.0 unx    16266 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OnChainTransaction.py
--rw-r--r--  2.0 unx      817 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py
--rw-r--r--  2.0 unx     2540 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py
--rw-r--r--  2.0 unx    35908 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningTransaction.py
--rw-r--r--  2.0 unx      569 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py
--rw-r--r--  2.0 unx      819 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py
--rw-r--r--  2.0 unx     1151 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/currency_amount.py
--rw-r--r--  2.0 unx     3848 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/crypto.py
--rw-r--r--  2.0 unx     1587 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/signing_key.py
--rw-r--r--  2.0 unx      137 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/__init__.py
--rw-r--r--  2.0 unx     1146 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/enums.py
--rw-r--r--  2.0 unx      471 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_test_mode_invoice.py
--rw-r--r--  2.0 unx      644 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/request_withdrawal.py
--rw-r--r--  2.0 unx      601 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py
--rw-r--r--  2.0 unx      582 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_payment_hash.py
--rw-r--r--  2.0 unx      630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py
--rw-r--r--  2.0 unx      365 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/recover_node_signing_key.py
--rw-r--r--  2.0 unx      266 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/delete_api_token.py
--rw-r--r--  2.0 unx      378 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/bitcoin_fee_estimate.py
--rw-r--r--  2.0 unx      367 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fetch_uma_invitation.py
--rw-r--r--  2.0 unx      582 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py
--rw-r--r--  2.0 unx      277 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_node_address.py
--rw-r--r--  2.0 unx      312 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/screen_node.py
--rw-r--r--  2.0 unx      645 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/register_payment.py
--rw-r--r--  2.0 unx      626 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
--rw-r--r--  2.0 unx      578 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py
--rw-r--r--  2.0 unx      433 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fund_node.py
--rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/__init__.py
--rw-r--r--  2.0 unx      577 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py
--rw-r--r--  2.0 unx      687 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py
--rw-r--r--  2.0 unx      475 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/decoded_payment_request.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py
--rw-r--r--  2.0 unx      391 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/cancel_invoice.py
--rw-r--r--  2.0 unx      283 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/current_account.py
--rw-r--r--  2.0 unx      306 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fail_htlcs.py
--rw-r--r--  2.0 unx      929 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py
--rw-r--r--  2.0 unx      701 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/send_payment.py
--rw-r--r--  2.0 unx      676 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/pay_invoice.py
--rw-r--r--  2.0 unx      477 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_api_token.py
--rw-r--r--  2.0 unx      576 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py
--rw-r--r--  2.0 unx      604 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_invoice.py
--rw-r--r--  2.0 unx      416 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/encoder.py
--rw-r--r--  2.0 unx     4775 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/requester.py
--rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/__init__.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     9157 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       63 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/requires.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/
+-rw-r--r--  2.0 unx    11352 b- defN 24-May-14 16:46 lightspark-2.7.1/LICENSE
+-rwxr-xr-x  2.0 unx       87 b- defN 24-May-14 16:46 lightspark-2.7.1/setup.py
+-rw-r--r--  2.0 unx     1035 b- defN 24-May-14 16:46 lightspark-2.7.1/README.md
+-rw-r--r--  2.0 unx       81 b- defN 24-May-14 16:46 lightspark-2.7.1/pyproject.toml
+-rw-r--r--  2.0 unx      750 b- defN 24-May-14 16:46 lightspark-2.7.1/setup.cfg
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-14 16:46 lightspark-2.7.1/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 16:46 lightspark-2.7.1/lightspark/requests/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/py.typed
+-rw-r--r--  2.0 unx       22 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/version.py
+-rw-r--r--  2.0 unx    35091 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/lightspark_client.py
+-rw-r--r--  2.0 unx    12874 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/__init__.py
+-rw-r--r--  2.0 unx      185 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/exceptions.py
+-rw-r--r--  2.0 unx     2354 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/webhooks.py
+-rw-r--r--  2.0 unx     1038 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/remote_signing.py
+-rw-r--r--  2.0 unx      912 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CancelInvoiceOutput.py
+-rw-r--r--  2.0 unx     6800 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelClosingTransaction.py
+-rw-r--r--  2.0 unx    20571 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/InvoiceData.py
+-rw-r--r--  2.0 unx     3170 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+-rw-r--r--  2.0 unx      999 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/TransactionStatus.py
+-rw-r--r--  2.0 unx    32826 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPayment.py
+-rw-r--r--  2.0 unx      949 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateApiTokenInput.py
+-rw-r--r--  2.0 unx      635 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CancelInvoiceInput.py
+-rw-r--r--  2.0 unx      543 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/InvoiceType.py
+-rw-r--r--  2.0 unx     2688 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WalletToWithdrawalRequestsConnection.py
+-rw-r--r--  2.0 unx     1086 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
+-rw-r--r--  2.0 unx     2585 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeToChannelsConnection.py
+-rw-r--r--  2.0 unx      551 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptStatus.py
+-rw-r--r--  2.0 unx      951 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RemoteSigningSubEventType.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RequestWithdrawalInput.py
+-rw-r--r--  2.0 unx      823 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignInvoiceOutput.py
+-rw-r--r--  2.0 unx      964 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Permission.py
+-rw-r--r--  2.0 unx     1206 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateTestModePaymentInput.py
+-rw-r--r--  2.0 unx     1080 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
+-rw-r--r--  2.0 unx      769 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/FailHtlcsOutput.py
+-rw-r--r--  2.0 unx     1519 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SendPaymentInput.py
+-rw-r--r--  2.0 unx      633 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesInput.py
+-rw-r--r--  2.0 unx      801 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateInvoiceOutput.py
+-rw-r--r--  2.0 unx     5777 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Withdrawal.py
+-rw-r--r--  2.0 unx     1299 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesOutput.py
+-rw-r--r--  2.0 unx     1833 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RegisterPaymentInput.py
+-rw-r--r--  2.0 unx     6010 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CurrencyAmount.py
+-rw-r--r--  2.0 unx    48408 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Transaction.py
+-rw-r--r--  2.0 unx      640 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IdAndSignature.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
+-rw-r--r--  2.0 unx     2773 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPaymentToAttemptsConnection.py
+-rw-r--r--  2.0 unx     1613 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WalletStatus.py
+-rw-r--r--  2.0 unx    10741 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Connection.py
+-rw-r--r--  2.0 unx      847 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ScreenNodeOutput.py
+-rw-r--r--  2.0 unx      527 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalMode.py
+-rw-r--r--  2.0 unx      659 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateUmaInvitationInput.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesOutput.py
+-rw-r--r--  2.0 unx    27441 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Node.py
+-rw-r--r--  2.0 unx     6193 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/BlockchainBalance.py
+-rw-r--r--  2.0 unx     3872 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPaymentAttempt.py
+-rw-r--r--  2.0 unx     1563 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PayInvoiceInput.py
+-rw-r--r--  2.0 unx     2777 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
+-rw-r--r--  2.0 unx      655 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RoutingTransactionFailureReason.py
+-rw-r--r--  2.0 unx     1138 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
+-rw-r--r--  2.0 unx      497 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignablePayloadStatus.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateInvoiceInput.py
+-rw-r--r--  2.0 unx    85008 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Wallet.py
+-rw-r--r--  2.0 unx     3170 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
+-rw-r--r--  2.0 unx      647 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RichText.py
+-rw-r--r--  2.0 unx     1286 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceInput.py
+-rw-r--r--  2.0 unx    18534 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalRequest.py
+-rw-r--r--  2.0 unx     1293 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
+-rw-r--r--  2.0 unx     1119 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WebhookEventType.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PostTransactionData.py
+-rw-r--r--  2.0 unx     2635 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToPaymentRequestsConnection.py
+-rw-r--r--  2.0 unx      873 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignMessagesInput.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToChannelsConnection.py
+-rw-r--r--  2.0 unx     1240 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignMessagesOutput.py
+-rw-r--r--  2.0 unx     1417 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Signable.py
+-rw-r--r--  2.0 unx      577 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightningPaymentDirection.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/FundNodeOutput.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/FeeEstimate.py
+-rw-r--r--  2.0 unx     5126 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/GraphNode.py
+-rw-r--r--  2.0 unx     9474 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPayment.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToNodesConnection.py
+-rw-r--r--  2.0 unx      644 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeStatus.py
+-rw-r--r--  2.0 unx     1671 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/MultiSigAddressValidationParameters.py
+-rw-r--r--  2.0 unx      470 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PaymentDirection.py
+-rw-r--r--  2.0 unx      864 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretOutput.py
+-rw-r--r--  2.0 unx     1310 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
+-rw-r--r--  2.0 unx    88288 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Entity.py
+-rw-r--r--  2.0 unx      892 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RequestWithdrawalOutput.py
+-rw-r--r--  2.0 unx      819 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageInput.py
+-rw-r--r--  2.0 unx     3242 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
+-rw-r--r--  2.0 unx      849 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/BitcoinNetwork.py
+-rw-r--r--  2.0 unx     2227 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/DailyLiquidityForecast.py
+-rw-r--r--  2.0 unx     2893 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ApiToken.py
+-rw-r--r--  2.0 unx     3618 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/UmaInvitation.py
+-rw-r--r--  2.0 unx   125678 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Account.py
+-rw-r--r--  2.0 unx     2597 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressOutput.py
+-rw-r--r--  2.0 unx      812 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/DeleteApiTokenOutput.py
+-rw-r--r--  2.0 unx     6939 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RoutingTransaction.py
+-rw-r--r--  2.0 unx     5785 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToTransactionsConnection.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeOwner.py
+-rw-r--r--  2.0 unx     1491 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateTestModePaymentoutput.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelStatus.py
+-rw-r--r--  2.0 unx     1783 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
+-rw-r--r--  2.0 unx      630 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalRequestStatus.py
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Deposit.py
+-rw-r--r--  2.0 unx     1180 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
+-rw-r--r--  2.0 unx     1927 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/HtlcAttemptFailureCode.py
+-rw-r--r--  2.0 unx    14407 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/all_entities.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/__init__.py
+-rw-r--r--  2.0 unx    22092 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Invoice.py
+-rw-r--r--  2.0 unx      511 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PaymentRequestStatus.py
+-rw-r--r--  2.0 unx     1195 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashInput.py
+-rw-r--r--  2.0 unx    18952 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RegionCode.py
+-rw-r--r--  2.0 unx      900 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PaymentFailureReason.py
+-rw-r--r--  2.0 unx      935 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignInvoiceInput.py
+-rw-r--r--  2.0 unx     1392 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateLnurlInvoiceInput.py
+-rw-r--r--  2.0 unx     1748 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/TransactionType.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/NodeAddress.py
+-rw-r--r--  2.0 unx     1668 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelFees.py
+-rw-r--r--  2.0 unx     4273 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelToTransactionsConnection.py
+-rw-r--r--  2.0 unx     3123 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SignablePayload.py
+-rw-r--r--  2.0 unx      990 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
+-rw-r--r--  2.0 unx      844 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/FailHtlcsInput.py
+-rw-r--r--  2.0 unx     2793 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToWithdrawalRequestsConnection.py
+-rw-r--r--  2.0 unx      937 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationInput.py
+-rw-r--r--  2.0 unx     4269 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Hop.py
+-rw-r--r--  2.0 unx      904 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationOutput.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SendPaymentOutput.py
+-rw-r--r--  2.0 unx    10172 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttempt.py
+-rw-r--r--  2.0 unx      711 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretInput.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
+-rw-r--r--  2.0 unx      811 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncentivesStatus.py
+-rw-r--r--  2.0 unx    23513 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PaymentRequest.py
+-rw-r--r--  2.0 unx    21264 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PaymentRequestData.py
+-rw-r--r--  2.0 unx     1424 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesInput.py
+-rw-r--r--  2.0 unx     1004 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateUmaInvoiceInput.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CurrencyUnit.py
+-rw-r--r--  2.0 unx     3984 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Balances.py
+-rw-r--r--  2.0 unx     2619 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WalletToPaymentRequestsConnection.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Secret.py
+-rw-r--r--  2.0 unx     1172 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PayUmaInvoiceInput.py
+-rw-r--r--  2.0 unx     6589 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelSnapshot.py
+-rw-r--r--  2.0 unx     2497 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToApiTokensConnection.py
+-rw-r--r--  2.0 unx     1807 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/NodeToAddressesConnection.py
+-rw-r--r--  2.0 unx      519 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/NodeAddressType.py
+-rw-r--r--  2.0 unx      969 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceOutput.py
+-rw-r--r--  2.0 unx     1483 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightningFeeEstimateOutput.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageOutput.py
+-rw-r--r--  2.0 unx      877 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashOutput.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AuditLogActor.py
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/AccountToWalletsConnection.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForNodeInput.py
+-rw-r--r--  2.0 unx     1410 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncentivesIneligibilityReason.py
+-rw-r--r--  2.0 unx      513 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/DeleteApiTokenInput.py
+-rw-r--r--  2.0 unx    39085 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNode.py
+-rw-r--r--  2.0 unx      619 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RiskRating.py
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateOutput.py
+-rw-r--r--  2.0 unx    27341 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeWithRemoteSigning.py
+-rw-r--r--  2.0 unx     6803 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ChannelOpeningTransaction.py
+-rw-r--r--  2.0 unx     1316 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateInput.py
+-rw-r--r--  2.0 unx    24929 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
+-rw-r--r--  2.0 unx     1021 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ScreenNodeInput.py
+-rw-r--r--  2.0 unx     2980 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
+-rw-r--r--  2.0 unx     1789 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
+-rw-r--r--  2.0 unx      535 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressInput.py
+-rw-r--r--  2.0 unx    27489 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightsparkNodeWithOSK.py
+-rw-r--r--  2.0 unx    15650 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/Channel.py
+-rw-r--r--  2.0 unx      615 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/FundNodeInput.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/TransactionFailures.py
+-rw-r--r--  2.0 unx     1709 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateApiTokenOutput.py
+-rw-r--r--  2.0 unx      462 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/ComplianceProvider.py
+-rw-r--r--  2.0 unx     1517 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PageInfo.py
+-rw-r--r--  2.0 unx      948 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/CreateUmaInvitationOutput.py
+-rw-r--r--  2.0 unx    16266 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/OnChainTransaction.py
+-rw-r--r--  2.0 unx      817 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/RegisterPaymentOutput.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/WalletToTransactionsConnection.py
+-rw-r--r--  2.0 unx    35908 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/LightningTransaction.py
+-rw-r--r--  2.0 unx      569 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/IncomingPaymentAttemptStatus.py
+-rw-r--r--  2.0 unx      819 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/objects/PayInvoiceOutput.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/currency_amount.py
+-rw-r--r--  2.0 unx     3848 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/crypto.py
+-rw-r--r--  2.0 unx     1587 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/signing_key.py
+-rw-r--r--  2.0 unx      137 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/__init__.py
+-rw-r--r--  2.0 unx     1146 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/utils/enums.py
+-rw-r--r--  2.0 unx      471 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_test_mode_invoice.py
+-rw-r--r--  2.0 unx      644 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/request_withdrawal.py
+-rw-r--r--  2.0 unx      601 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_test_mode_payment.py
+-rw-r--r--  2.0 unx      582 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_payment_hash.py
+-rw-r--r--  2.0 unx      630 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_node.py
+-rw-r--r--  2.0 unx      365 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/recover_node_signing_key.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/delete_api_token.py
+-rw-r--r--  2.0 unx      378 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/bitcoin_fee_estimate.py
+-rw-r--r--  2.0 unx      367 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/fetch_uma_invitation.py
+-rw-r--r--  2.0 unx      582 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_lnurl_invoice.py
+-rw-r--r--  2.0 unx      277 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_node_address.py
+-rw-r--r--  2.0 unx      312 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/screen_node.py
+-rw-r--r--  2.0 unx      645 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/register_payment.py
+-rw-r--r--  2.0 unx      626 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_invoice.py
+-rw-r--r--  2.0 unx      578 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/incoming_payments_for_invoice.py
+-rw-r--r--  2.0 unx      433 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/fund_node.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/__init__.py
+-rw-r--r--  2.0 unx      577 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_invoice.py
+-rw-r--r--  2.0 unx      687 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/pay_uma_invoice.py
+-rw-r--r--  2.0 unx      475 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/decoded_payment_request.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/claim_uma_invitation.py
+-rw-r--r--  2.0 unx      391 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/cancel_invoice.py
+-rw-r--r--  2.0 unx      283 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/current_account.py
+-rw-r--r--  2.0 unx      306 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/fail_htlcs.py
+-rw-r--r--  2.0 unx      929 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_uma_invitation.py
+-rw-r--r--  2.0 unx      701 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/send_payment.py
+-rw-r--r--  2.0 unx      676 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/pay_invoice.py
+-rw-r--r--  2.0 unx      477 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_api_token.py
+-rw-r--r--  2.0 unx      576 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_uma_invoice.py
+-rw-r--r--  2.0 unx      604 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/scripts/create_invoice.py
+-rw-r--r--  2.0 unx      416 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/requests/encoder.py
+-rw-r--r--  2.0 unx     4775 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/requests/requester.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark/requests/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     9157 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       63 b- defN 24-May-14 16:46 lightspark-2.7.1/lightspark.egg-info/requires.txt
 226 files, 1125728 bytes uncompressed, 180053 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -1,679 +1,679 @@
-Filename: lightspark-2.7.0/
+Filename: lightspark-2.7.1/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/
+Filename: lightspark-2.7.1/lightspark/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/
+Filename: lightspark-2.7.1/lightspark.egg-info/
 Comment: 
 
-Filename: lightspark-2.7.0/LICENSE
+Filename: lightspark-2.7.1/LICENSE
 Comment: 
 
-Filename: lightspark-2.7.0/setup.py
+Filename: lightspark-2.7.1/setup.py
 Comment: 
 
-Filename: lightspark-2.7.0/README.md
+Filename: lightspark-2.7.1/README.md
 Comment: 
 
-Filename: lightspark-2.7.0/pyproject.toml
+Filename: lightspark-2.7.1/pyproject.toml
 Comment: 
 
-Filename: lightspark-2.7.0/setup.cfg
+Filename: lightspark-2.7.1/setup.cfg
 Comment: 
 
-Filename: lightspark-2.7.0/PKG-INFO
+Filename: lightspark-2.7.1/PKG-INFO
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/
+Filename: lightspark-2.7.1/lightspark/objects/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/
+Filename: lightspark-2.7.1/lightspark/utils/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/
+Filename: lightspark-2.7.1/lightspark/scripts/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/requests/
+Filename: lightspark-2.7.1/lightspark/requests/
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/py.typed
+Filename: lightspark-2.7.1/lightspark/py.typed
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/version.py
+Filename: lightspark-2.7.1/lightspark/version.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/lightspark_client.py
+Filename: lightspark-2.7.1/lightspark/lightspark_client.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/__init__.py
+Filename: lightspark-2.7.1/lightspark/__init__.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/exceptions.py
+Filename: lightspark-2.7.1/lightspark/exceptions.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/webhooks.py
+Filename: lightspark-2.7.1/lightspark/webhooks.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/remote_signing.py
+Filename: lightspark-2.7.1/lightspark/remote_signing.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CancelInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelClosingTransaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/InvoiceData.py
+Filename: lightspark-2.7.1/lightspark/objects/InvoiceData.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/TransactionStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/TransactionStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPayment.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPayment.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateApiTokenInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CancelInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/InvoiceType.py
+Filename: lightspark-2.7.1/lightspark/objects/InvoiceType.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WalletToWithdrawalRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeToChannelsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py
+Filename: lightspark-2.7.1/lightspark/objects/RemoteSigningSubEventType.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RequestWithdrawalInput.py
+Filename: lightspark-2.7.1/lightspark/objects/RequestWithdrawalInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/SignInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Permission.py
+Filename: lightspark-2.7.1/lightspark/objects/Permission.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateTestModePaymentInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/FailHtlcsOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/FailHtlcsOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SendPaymentInput.py
+Filename: lightspark-2.7.1/lightspark/objects/SendPaymentInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py
+Filename: lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Withdrawal.py
+Filename: lightspark-2.7.1/lightspark/objects/Withdrawal.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py
+Filename: lightspark-2.7.1/lightspark/objects/RegisterPaymentInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CurrencyAmount.py
+Filename: lightspark-2.7.1/lightspark/objects/CurrencyAmount.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Transaction.py
+Filename: lightspark-2.7.1/lightspark/objects/Transaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IdAndSignature.py
+Filename: lightspark-2.7.1/lightspark/objects/IdAndSignature.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
+Filename: lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPaymentToAttemptsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WalletStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/WalletStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Connection.py
+Filename: lightspark-2.7.1/lightspark/objects/Connection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/ScreenNodeOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalMode.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalMode.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateUmaInvitationInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Node.py
+Filename: lightspark-2.7.1/lightspark/objects/Node.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/BlockchainBalance.py
+Filename: lightspark-2.7.1/lightspark/objects/BlockchainBalance.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPaymentAttempt.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/PayInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py
+Filename: lightspark-2.7.1/lightspark/objects/RoutingTransactionFailureReason.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
+Filename: lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignablePayloadStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/SignablePayloadStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Wallet.py
+Filename: lightspark-2.7.1/lightspark/objects/Wallet.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RichText.py
+Filename: lightspark-2.7.1/lightspark/objects/RichText.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalRequest.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WebhookEventType.py
+Filename: lightspark-2.7.1/lightspark/objects/WebhookEventType.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PostTransactionData.py
+Filename: lightspark-2.7.1/lightspark/objects/PostTransactionData.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToPaymentRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignMessagesInput.py
+Filename: lightspark-2.7.1/lightspark/objects/SignMessagesInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToChannelsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/SignMessagesOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Signable.py
+Filename: lightspark-2.7.1/lightspark/objects/Signable.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py
+Filename: lightspark-2.7.1/lightspark/objects/LightningPaymentDirection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/FundNodeOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/FundNodeOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/FeeEstimate.py
+Filename: lightspark-2.7.1/lightspark/objects/FeeEstimate.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/GraphNode.py
+Filename: lightspark-2.7.1/lightspark/objects/GraphNode.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPayment.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPayment.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToNodesConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py
+Filename: lightspark-2.7.1/lightspark/objects/MultiSigAddressValidationParameters.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PaymentDirection.py
+Filename: lightspark-2.7.1/lightspark/objects/PaymentDirection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Entity.py
+Filename: lightspark-2.7.1/lightspark/objects/Entity.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/RequestWithdrawalOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py
+Filename: lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py
+Filename: lightspark-2.7.1/lightspark/objects/BitcoinNetwork.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py
+Filename: lightspark-2.7.1/lightspark/objects/DailyLiquidityForecast.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ApiToken.py
+Filename: lightspark-2.7.1/lightspark/objects/ApiToken.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/UmaInvitation.py
+Filename: lightspark-2.7.1/lightspark/objects/UmaInvitation.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Account.py
+Filename: lightspark-2.7.1/lightspark/objects/Account.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/DeleteApiTokenOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RoutingTransaction.py
+Filename: lightspark-2.7.1/lightspark/objects/RoutingTransaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeOwner.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateTestModePaymentoutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
+Filename: lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalRequestStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Deposit.py
+Filename: lightspark-2.7.1/lightspark/objects/Deposit.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py
+Filename: lightspark-2.7.1/lightspark/objects/HtlcAttemptFailureCode.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/all_entities.py
+Filename: lightspark-2.7.1/lightspark/objects/all_entities.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/__init__.py
+Filename: lightspark-2.7.1/lightspark/objects/__init__.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Invoice.py
+Filename: lightspark-2.7.1/lightspark/objects/Invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PaymentRequestStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/PaymentRequestStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py
+Filename: lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RegionCode.py
+Filename: lightspark-2.7.1/lightspark/objects/RegionCode.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py
+Filename: lightspark-2.7.1/lightspark/objects/PaymentFailureReason.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/SignInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateLnurlInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/TransactionType.py
+Filename: lightspark-2.7.1/lightspark/objects/TransactionType.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/NodeAddress.py
+Filename: lightspark-2.7.1/lightspark/objects/NodeAddress.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelFees.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelFees.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SignablePayload.py
+Filename: lightspark-2.7.1/lightspark/objects/SignablePayload.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/FailHtlcsInput.py
+Filename: lightspark-2.7.1/lightspark/objects/FailHtlcsInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToWithdrawalRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py
+Filename: lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Hop.py
+Filename: lightspark-2.7.1/lightspark/objects/Hop.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/SendPaymentOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttempt.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py
+Filename: lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncentivesStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/IncentivesStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PaymentRequest.py
+Filename: lightspark-2.7.1/lightspark/objects/PaymentRequest.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PaymentRequestData.py
+Filename: lightspark-2.7.1/lightspark/objects/PaymentRequestData.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateUmaInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CurrencyUnit.py
+Filename: lightspark-2.7.1/lightspark/objects/CurrencyUnit.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Balances.py
+Filename: lightspark-2.7.1/lightspark/objects/Balances.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WalletToPaymentRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Secret.py
+Filename: lightspark-2.7.1/lightspark/objects/Secret.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py
+Filename: lightspark-2.7.1/lightspark/objects/PayUmaInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelSnapshot.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToApiTokensConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/NodeToAddressesConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/NodeAddressType.py
+Filename: lightspark-2.7.1/lightspark/objects/NodeAddressType.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/LightningFeeEstimateOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AuditLogActor.py
+Filename: lightspark-2.7.1/lightspark/objects/AuditLogActor.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/AccountToWalletsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
+Filename: lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForNodeInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py
+Filename: lightspark-2.7.1/lightspark/objects/IncentivesIneligibilityReason.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py
+Filename: lightspark-2.7.1/lightspark/objects/DeleteApiTokenInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNode.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNode.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RiskRating.py
+Filename: lightspark-2.7.1/lightspark/objects/RiskRating.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeWithRemoteSigning.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py
+Filename: lightspark-2.7.1/lightspark/objects/ChannelOpeningTransaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py
+Filename: lightspark-2.7.1/lightspark/objects/ScreenNodeInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py
+Filename: lightspark-2.7.1/lightspark/objects/LightsparkNodeWithOSK.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/Channel.py
+Filename: lightspark-2.7.1/lightspark/objects/Channel.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/FundNodeInput.py
+Filename: lightspark-2.7.1/lightspark/objects/FundNodeInput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/TransactionFailures.py
+Filename: lightspark-2.7.1/lightspark/objects/TransactionFailures.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateApiTokenOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/ComplianceProvider.py
+Filename: lightspark-2.7.1/lightspark/objects/ComplianceProvider.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PageInfo.py
+Filename: lightspark-2.7.1/lightspark/objects/PageInfo.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/CreateUmaInvitationOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/OnChainTransaction.py
+Filename: lightspark-2.7.1/lightspark/objects/OnChainTransaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/RegisterPaymentOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py
+Filename: lightspark-2.7.1/lightspark/objects/WalletToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/LightningTransaction.py
+Filename: lightspark-2.7.1/lightspark/objects/LightningTransaction.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py
+Filename: lightspark-2.7.1/lightspark/objects/IncomingPaymentAttemptStatus.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py
+Filename: lightspark-2.7.1/lightspark/objects/PayInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/currency_amount.py
+Filename: lightspark-2.7.1/lightspark/utils/currency_amount.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/crypto.py
+Filename: lightspark-2.7.1/lightspark/utils/crypto.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/signing_key.py
+Filename: lightspark-2.7.1/lightspark/utils/signing_key.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/__init__.py
+Filename: lightspark-2.7.1/lightspark/utils/__init__.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/utils/enums.py
+Filename: lightspark-2.7.1/lightspark/utils/enums.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_test_mode_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_test_mode_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/request_withdrawal.py
+Filename: lightspark-2.7.1/lightspark/scripts/request_withdrawal.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_test_mode_payment.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_payment_hash.py
+Filename: lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_payment_hash.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py
+Filename: lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_node.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/recover_node_signing_key.py
+Filename: lightspark-2.7.1/lightspark/scripts/recover_node_signing_key.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/delete_api_token.py
+Filename: lightspark-2.7.1/lightspark/scripts/delete_api_token.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/bitcoin_fee_estimate.py
+Filename: lightspark-2.7.1/lightspark/scripts/bitcoin_fee_estimate.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/fetch_uma_invitation.py
+Filename: lightspark-2.7.1/lightspark/scripts/fetch_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_lnurl_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_node_address.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_node_address.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/screen_node.py
+Filename: lightspark-2.7.1/lightspark/scripts/screen_node.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/register_payment.py
+Filename: lightspark-2.7.1/lightspark/scripts/register_payment.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/incoming_payments_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/fund_node.py
+Filename: lightspark-2.7.1/lightspark/scripts/fund_node.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/__init__.py
+Filename: lightspark-2.7.1/lightspark/scripts/__init__.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/pay_uma_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/decoded_payment_request.py
+Filename: lightspark-2.7.1/lightspark/scripts/decoded_payment_request.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py
+Filename: lightspark-2.7.1/lightspark/scripts/claim_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/cancel_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/cancel_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/current_account.py
+Filename: lightspark-2.7.1/lightspark/scripts/current_account.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/fail_htlcs.py
+Filename: lightspark-2.7.1/lightspark/scripts/fail_htlcs.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/send_payment.py
+Filename: lightspark-2.7.1/lightspark/scripts/send_payment.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/pay_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/pay_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_api_token.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_api_token.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_uma_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/scripts/create_invoice.py
+Filename: lightspark-2.7.1/lightspark/scripts/create_invoice.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/requests/encoder.py
+Filename: lightspark-2.7.1/lightspark/requests/encoder.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/requests/requester.py
+Filename: lightspark-2.7.1/lightspark/requests/requester.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark/requests/__init__.py
+Filename: lightspark-2.7.1/lightspark/requests/__init__.py
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/dependency_links.txt
+Filename: lightspark-2.7.1/lightspark.egg-info/dependency_links.txt
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/SOURCES.txt
+Filename: lightspark-2.7.1/lightspark.egg-info/SOURCES.txt
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/top_level.txt
+Filename: lightspark-2.7.1/lightspark.egg-info/top_level.txt
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/PKG-INFO
+Filename: lightspark-2.7.1/lightspark.egg-info/PKG-INFO
 Comment: 
 
-Filename: lightspark-2.7.0/lightspark.egg-info/requires.txt
+Filename: lightspark-2.7.1/lightspark.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `lightspark-2.7.0/LICENSE` & `lightspark-2.7.1/LICENSE`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/README.md` & `lightspark-2.7.1/README.md`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/setup.cfg` & `lightspark-2.7.1/setup.cfg`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/PKG-INFO` & `lightspark-2.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightspark
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python SDK for the Lightspark API
 Home-page: https://www.lightspark.com/
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.lightspark.com/lightspark-sdk/getting-started?language=Python
 Project-URL: Source Code, https://github.com/lightsparkdev/python-sdk
```

## Comparing `lightspark-2.7.0/lightspark/lightspark_client.py` & `lightspark-2.7.1/lightspark/lightspark_client.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/__init__.py` & `lightspark-2.7.1/lightspark/__init__.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/webhooks.py` & `lightspark-2.7.1/lightspark/webhooks.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/remote_signing.py` & `lightspark-2.7.1/lightspark/remote_signing.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py` & `lightspark-2.7.1/lightspark/objects/CancelInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py` & `lightspark-2.7.1/lightspark/objects/ChannelClosingTransaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/InvoiceData.py` & `lightspark-2.7.1/lightspark/objects/InvoiceData.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/TransactionStatus.py` & `lightspark-2.7.1/lightspark/objects/TransactionStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPayment.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPayment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py` & `lightspark-2.7.1/lightspark/objects/CreateApiTokenInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/CancelInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/InvoiceType.py` & `lightspark-2.7.1/lightspark/objects/InvoiceType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py` & `lightspark-2.7.1/lightspark/objects/WalletToWithdrawalRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py` & `lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeToChannelsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py` & `lightspark-2.7.1/lightspark/objects/RemoteSigningSubEventType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RequestWithdrawalInput.py` & `lightspark-2.7.1/lightspark/objects/RequestWithdrawalInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py` & `lightspark-2.7.1/lightspark/objects/SignInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Permission.py` & `lightspark-2.7.1/lightspark/objects/Permission.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py` & `lightspark-2.7.1/lightspark/objects/CreateTestModePaymentInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py` & `lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/FailHtlcsOutput.py` & `lightspark-2.7.1/lightspark/objects/FailHtlcsOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SendPaymentInput.py` & `lightspark-2.7.1/lightspark/objects/SendPaymentInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py` & `lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Withdrawal.py` & `lightspark-2.7.1/lightspark/objects/Withdrawal.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py` & `lightspark-2.7.1/lightspark/objects/DeclineToSignMessagesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py` & `lightspark-2.7.1/lightspark/objects/RegisterPaymentInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CurrencyAmount.py` & `lightspark-2.7.1/lightspark/objects/CurrencyAmount.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Transaction.py` & `lightspark-2.7.1/lightspark/objects/Transaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IdAndSignature.py` & `lightspark-2.7.1/lightspark/objects/IdAndSignature.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py` & `lightspark-2.7.1/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py` & `lightspark-2.7.1/lightspark/objects/IncomingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WalletStatus.py` & `lightspark-2.7.1/lightspark/objects/WalletStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Connection.py` & `lightspark-2.7.1/lightspark/objects/Connection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py` & `lightspark-2.7.1/lightspark/objects/ScreenNodeOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalMode.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalMode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py` & `lightspark-2.7.1/lightspark/objects/CreateUmaInvitationInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Node.py` & `lightspark-2.7.1/lightspark/objects/Node.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/BlockchainBalance.py` & `lightspark-2.7.1/lightspark/objects/BlockchainBalance.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py` & `lightspark-2.7.1/lightspark/objects/IncomingPaymentAttempt.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/PayInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py` & `lightspark-2.7.1/lightspark/objects/RoutingTransactionFailureReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py` & `lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/CreateInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Wallet.py` & `lightspark-2.7.1/lightspark/objects/Wallet.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RichText.py` & `lightspark-2.7.1/lightspark/objects/RichText.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalRequest.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WebhookEventType.py` & `lightspark-2.7.1/lightspark/objects/WebhookEventType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PostTransactionData.py` & `lightspark-2.7.1/lightspark/objects/PostTransactionData.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToPaymentRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SignMessagesInput.py` & `lightspark-2.7.1/lightspark/objects/SignMessagesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToChannelsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py` & `lightspark-2.7.1/lightspark/objects/SignMessagesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Signable.py` & `lightspark-2.7.1/lightspark/objects/Signable.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py` & `lightspark-2.7.1/lightspark/objects/LightningPaymentDirection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/FundNodeOutput.py` & `lightspark-2.7.1/lightspark/objects/FundNodeOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/FeeEstimate.py` & `lightspark-2.7.1/lightspark/objects/FeeEstimate.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/GraphNode.py` & `lightspark-2.7.1/lightspark/objects/GraphNode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPayment.py` & `lightspark-2.7.1/lightspark/objects/IncomingPayment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToNodesConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py` & `lightspark-2.7.1/lightspark/objects/MultiSigAddressValidationParameters.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py` & `lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Entity.py` & `lightspark-2.7.1/lightspark/objects/Entity.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py` & `lightspark-2.7.1/lightspark/objects/RequestWithdrawalOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py` & `lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py` & `lightspark-2.7.1/lightspark/objects/BitcoinNetwork.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py` & `lightspark-2.7.1/lightspark/objects/DailyLiquidityForecast.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ApiToken.py` & `lightspark-2.7.1/lightspark/objects/ApiToken.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/UmaInvitation.py` & `lightspark-2.7.1/lightspark/objects/UmaInvitation.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Account.py` & `lightspark-2.7.1/lightspark/objects/Account.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py` & `lightspark-2.7.1/lightspark/objects/DeleteApiTokenOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RoutingTransaction.py` & `lightspark-2.7.1/lightspark/objects/RoutingTransaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeOwner.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py` & `lightspark-2.7.1/lightspark/objects/CreateTestModePaymentoutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelStatus.py` & `lightspark-2.7.1/lightspark/objects/ChannelStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py` & `lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalRequestStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Deposit.py` & `lightspark-2.7.1/lightspark/objects/Deposit.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py` & `lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py` & `lightspark-2.7.1/lightspark/objects/HtlcAttemptFailureCode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/all_entities.py` & `lightspark-2.7.1/lightspark/objects/all_entities.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Invoice.py` & `lightspark-2.7.1/lightspark/objects/Invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py` & `lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RegionCode.py` & `lightspark-2.7.1/lightspark/objects/RegionCode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py` & `lightspark-2.7.1/lightspark/objects/PaymentFailureReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/SignInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/CreateLnurlInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/TransactionType.py` & `lightspark-2.7.1/lightspark/objects/TransactionType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/NodeAddress.py` & `lightspark-2.7.1/lightspark/objects/NodeAddress.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelFees.py` & `lightspark-2.7.1/lightspark/objects/ChannelFees.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py` & `lightspark-2.7.1/lightspark/objects/ChannelToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SignablePayload.py` & `lightspark-2.7.1/lightspark/objects/SignablePayload.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py` & `lightspark-2.7.1/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/FailHtlcsInput.py` & `lightspark-2.7.1/lightspark/objects/FailHtlcsInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToWithdrawalRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py` & `lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Hop.py` & `lightspark-2.7.1/lightspark/objects/Hop.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py` & `lightspark-2.7.1/lightspark/objects/ClaimUmaInvitationOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py` & `lightspark-2.7.1/lightspark/objects/SendPaymentOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentAttempt.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py` & `lightspark-2.7.1/lightspark/objects/UpdateNodeSharedSecretInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncentivesStatus.py` & `lightspark-2.7.1/lightspark/objects/IncentivesStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PaymentRequest.py` & `lightspark-2.7.1/lightspark/objects/PaymentRequest.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PaymentRequestData.py` & `lightspark-2.7.1/lightspark/objects/PaymentRequestData.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py` & `lightspark-2.7.1/lightspark/objects/CreateInvitationWithIncentivesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/CreateUmaInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CurrencyUnit.py` & `lightspark-2.7.1/lightspark/objects/CurrencyUnit.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Balances.py` & `lightspark-2.7.1/lightspark/objects/Balances.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py` & `lightspark-2.7.1/lightspark/objects/WalletToPaymentRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Secret.py` & `lightspark-2.7.1/lightspark/objects/Secret.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py` & `lightspark-2.7.1/lightspark/objects/PayUmaInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py` & `lightspark-2.7.1/lightspark/objects/ChannelSnapshot.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToApiTokensConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py` & `lightspark-2.7.1/lightspark/objects/NodeToAddressesConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/NodeAddressType.py` & `lightspark-2.7.1/lightspark/objects/NodeAddressType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateTestModeInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py` & `lightspark-2.7.1/lightspark/objects/LightningFeeEstimateOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py` & `lightspark-2.7.1/lightspark/objects/ReleasePaymentPreimageOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py` & `lightspark-2.7.1/lightspark/objects/SetInvoicePaymentHashOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AuditLogActor.py` & `lightspark-2.7.1/lightspark/objects/AuditLogActor.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py` & `lightspark-2.7.1/lightspark/objects/AccountToWalletsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py` & `lightspark-2.7.1/lightspark/objects/LightningFeeEstimateForNodeInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py` & `lightspark-2.7.1/lightspark/objects/IncentivesIneligibilityReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py` & `lightspark-2.7.1/lightspark/objects/DeleteApiTokenInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNode.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RiskRating.py` & `lightspark-2.7.1/lightspark/objects/RiskRating.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeWithRemoteSigning.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py` & `lightspark-2.7.1/lightspark/objects/ChannelOpeningTransaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalFeeEstimateInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py` & `lightspark-2.7.1/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py` & `lightspark-2.7.1/lightspark/objects/ScreenNodeInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py` & `lightspark-2.7.1/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py` & `lightspark-2.7.1/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py` & `lightspark-2.7.1/lightspark/objects/CreateNodeWalletAddressInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py` & `lightspark-2.7.1/lightspark/objects/LightsparkNodeWithOSK.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/Channel.py` & `lightspark-2.7.1/lightspark/objects/Channel.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/FundNodeInput.py` & `lightspark-2.7.1/lightspark/objects/FundNodeInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/TransactionFailures.py` & `lightspark-2.7.1/lightspark/objects/TransactionFailures.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateApiTokenOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PageInfo.py` & `lightspark-2.7.1/lightspark/objects/PageInfo.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py` & `lightspark-2.7.1/lightspark/objects/CreateUmaInvitationOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/OnChainTransaction.py` & `lightspark-2.7.1/lightspark/objects/OnChainTransaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py` & `lightspark-2.7.1/lightspark/objects/RegisterPaymentOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py` & `lightspark-2.7.1/lightspark/objects/WalletToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/LightningTransaction.py` & `lightspark-2.7.1/lightspark/objects/LightningTransaction.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py` & `lightspark-2.7.1/lightspark/objects/IncomingPaymentAttemptStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py` & `lightspark-2.7.1/lightspark/objects/PayInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/utils/currency_amount.py` & `lightspark-2.7.1/lightspark/utils/currency_amount.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/utils/crypto.py` & `lightspark-2.7.1/lightspark/utils/crypto.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/utils/signing_key.py` & `lightspark-2.7.1/lightspark/utils/signing_key.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/utils/enums.py` & `lightspark-2.7.1/lightspark/utils/enums.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/request_withdrawal.py` & `lightspark-2.7.1/lightspark/scripts/request_withdrawal.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py` & `lightspark-2.7.1/lightspark/scripts/create_test_mode_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_payment_hash.py` & `lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_payment_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from lightspark.objects.OutgoingPayment import FRAGMENT as OutgoingPaymentFragment
 
 OUTGOING_PAYMENTS_FOR_PAYMENT_HASH_QUERY = f"""
 query OutgoingPaymentsForPaymentHash(
-    $payment_hash: String!,
+    $payment_hash: Hash32!,
     $transaction_statuses: [TransactionStatus!] = null
 ) {{
     outgoing_payments_for_payment_hash(input: {{
         payment_hash: $payment_hash,
         statuses: $transaction_statuses
     }}) {{
         payments {{
```

## Comparing `lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py` & `lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_node.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py` & `lightspark-2.7.1/lightspark/scripts/create_lnurl_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/register_payment.py` & `lightspark-2.7.1/lightspark/scripts/register_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py` & `lightspark-2.7.1/lightspark/scripts/lightning_fee_estimate_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py` & `lightspark-2.7.1/lightspark/scripts/incoming_payments_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py` & `lightspark-2.7.1/lightspark/scripts/outgoing_payments_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py` & `lightspark-2.7.1/lightspark/scripts/pay_uma_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py` & `lightspark-2.7.1/lightspark/scripts/claim_uma_invitation.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py` & `lightspark-2.7.1/lightspark/scripts/create_uma_invitation.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/send_payment.py` & `lightspark-2.7.1/lightspark/scripts/send_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/pay_invoice.py` & `lightspark-2.7.1/lightspark/scripts/pay_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py` & `lightspark-2.7.1/lightspark/scripts/create_uma_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/scripts/create_invoice.py` & `lightspark-2.7.1/lightspark/scripts/create_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark/requests/requester.py` & `lightspark-2.7.1/lightspark/requests/requester.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark.egg-info/SOURCES.txt` & `lightspark-2.7.1/lightspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `lightspark-2.7.0/lightspark.egg-info/PKG-INFO` & `lightspark-2.7.1/lightspark.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightspark
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python SDK for the Lightspark API
 Home-page: https://www.lightspark.com/
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.lightspark.com/lightspark-sdk/getting-started?language=Python
 Project-URL: Source Code, https://github.com/lightsparkdev/python-sdk
```

