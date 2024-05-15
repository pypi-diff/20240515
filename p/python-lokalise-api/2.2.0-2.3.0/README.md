# Comparing `tmp/python_lokalise_api-2.2.0.tar.gz` & `tmp/python_lokalise_api-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_lokalise_api-2.2.0.tar", max compression
+gzip compressed data, was "python_lokalise_api-2.3.0.tar", max compression
```

## Comparing `python_lokalise_api-2.2.0.tar` & `python_lokalise_api-2.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1505 2023-01-11 16:49:12.730266 python_lokalise_api-2.2.0/LICENSE
--rw-r--r--   0        0        0      317 2022-10-05 17:09:24.598941 python_lokalise_api-2.2.0/lokalise/__init__.py
--rw-r--r--   0        0        0      115 2023-02-27 17:36:02.975057 python_lokalise_api-2.2.0/lokalise/_version.py
--rw-r--r--   0        0        0     1355 2022-11-30 21:18:17.855530 python_lokalise_api-2.2.0/lokalise/base_client.py
--rw-r--r--   0        0        0    63236 2023-08-09 10:51:09.428371 python_lokalise_api-2.2.0/lokalise/client.py
--rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/__init__.py
--rw-r--r--   0        0        0     3144 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/base_collection.py
--rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/branches.py
--rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/comments.py
--rw-r--r--   0        0        0      389 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/contributors.py
--rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/files.py
--rw-r--r--   0        0        0      309 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/keys.py
--rw-r--r--   0        0        0      373 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/languages.py
--rw-r--r--   0        0        0      327 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/orders.py
--rw-r--r--   0        0        0      387 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/payment_cards.py
--rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/projects.py
--rw-r--r--   0        0        0      404 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/queued_processes.py
--rw-r--r--   0        0        0      372 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/screenshots.py
--rw-r--r--   0        0        0      345 2021-12-17 13:27:20.711362 python_lokalise_api-2.2.0/lokalise/collections/segments.py
--rw-r--r--   0        0        0      354 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/snapshots.py
--rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/tasks.py
--rw-r--r--   0        0        0      406 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/team_user_groups.py
--rw-r--r--   0        0        0      360 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/team_users.py
--rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/teams.py
--rw-r--r--   0        0        0      459 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/translation_providers.py
--rw-r--r--   0        0        0      454 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/translation_statuses.py
--rw-r--r--   0        0        0      381 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/translations.py
--rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/collections/webhooks.py
--rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/__init__.py
--rw-r--r--   0        0        0     4369 2023-02-27 17:36:02.975057 python_lokalise_api-2.2.0/lokalise/endpoints/base_endpoint.py
--rw-r--r--   0        0        0      830 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/branches_endpoint.py
--rw-r--r--   0        0        0      342 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/contributors_endpoint.py
--rw-r--r--   0        0        0     1172 2022-07-27 15:15:30.268244 python_lokalise_api-2.2.0/lokalise/endpoints/files_endpoint.py
--rw-r--r--   0        0        0      270 2023-01-11 16:49:12.732277 python_lokalise_api-2.2.0/lokalise/endpoints/jwt_endpoint.py
--rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/key_comments_endpoint.py
--rw-r--r--   0        0        0      294 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/keys_endpoint.py
--rw-r--r--   0        0        0      332 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/languages_endpoint.py
--rw-r--r--   0        0        0      295 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/orders_endpoint.py
--rw-r--r--   0        0        0      317 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/payment_cards_endpoint.py
--rw-r--r--   0        0        0      336 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/project_comments_endpoint.py
--rw-r--r--   0        0        0      688 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/projects_endpoint.py
--rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/queued_processes_endpoint.py
--rw-r--r--   0        0        0      333 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/screenshots_endpoint.py
--rw-r--r--   0        0        0      331 2021-12-17 13:27:20.711362 python_lokalise_api-2.2.0/lokalise/endpoints/segments_endpoint.py
--rw-r--r--   0        0        0      316 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/snapshots_endpoint.py
--rw-r--r--   0        0        0      326 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/system_languages_endpoint.py
--rw-r--r--   0        0        0      292 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/tasks_endpoint.py
--rw-r--r--   0        0        0      384 2021-12-17 13:27:20.712362 python_lokalise_api-2.2.0/lokalise/endpoints/team_user_billing_details_endpoint.py
--rw-r--r--   0        0        0     2735 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/team_user_groups_endpoint.py
--rw-r--r--   0        0        0      313 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/team_users_endpoint.py
--rw-r--r--   0        0        0      259 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/teams_endpoint.py
--rw-r--r--   0        0        0      384 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/translation_providers_endpoint.py
--rw-r--r--   0        0        0      802 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/translation_statuses_endpoint.py
--rw-r--r--   0        0        0      334 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/translations_endpoint.py
--rw-r--r--   0        0        0      701 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/endpoints/webhooks_endpoint.py
--rw-r--r--   0        0        0     2449 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/errors.py
--rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/__init__.py
--rw-r--r--   0        0        0     2880 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/base_model.py
--rw-r--r--   0        0        0      405 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/branch.py
--rw-r--r--   0        0        0      420 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/comment.py
--rw-r--r--   0        0        0      499 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/contributor.py
--rw-r--r--   0        0        0      272 2022-10-05 17:09:24.599953 python_lokalise_api-2.2.0/lokalise/models/file.py
--rw-r--r--   0        0        0      220 2022-11-30 21:18:17.856531 python_lokalise_api-2.2.0/lokalise/models/jwt.py
--rw-r--r--   0        0        0      815 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/key.py
--rw-r--r--   0        0        0      383 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/language.py
--rw-r--r--   0        0        0      738 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/order.py
--rw-r--r--   0        0        0      387 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/payment_card.py
--rw-r--r--   0        0        0      550 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/project.py
--rw-r--r--   0        0        0      493 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/queued_process.py
--rw-r--r--   0        0        0      495 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/screenshot.py
--rw-r--r--   0        0        0      561 2021-12-17 13:27:20.712362 python_lokalise_api-2.2.0/lokalise/models/segment.py
--rw-r--r--   0        0        0      416 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/snapshot.py
--rw-r--r--   0        0        0      980 2023-02-27 17:36:02.976058 python_lokalise_api-2.2.0/lokalise/models/task.py
--rw-r--r--   0        0        0      377 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/team.py
--rw-r--r--   0        0        0      401 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/team_user.py
--rw-r--r--   0        0        0      546 2021-12-17 13:27:20.712362 python_lokalise_api-2.2.0/lokalise/models/team_user_billing_details.py
--rw-r--r--   0        0        0      471 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/team_user_group.py
--rw-r--r--   0        0        0      636 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/translation.py
--rw-r--r--   0        0        0      463 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/translation_provider.py
--rw-r--r--   0        0        0      388 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/translation_status.py
--rw-r--r--   0        0        0      362 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/models/webhook.py
--rw-r--r--   0        0        0        0 2022-03-07 13:50:09.211635 python_lokalise_api-2.2.0/lokalise/oauth2/__init__.py
--rw-r--r--   0        0        0     2771 2022-07-27 15:15:30.268244 python_lokalise_api-2.2.0/lokalise/oauth2/auth.py
--rw-r--r--   0        0        0     1430 2022-07-27 15:15:30.268244 python_lokalise_api-2.2.0/lokalise/oauth2/request.py
--rw-r--r--   0        0        0     1558 2021-10-27 12:17:46.650227 python_lokalise_api-2.2.0/lokalise/oauth_client.py
--rw-r--r--   0        0        0     4840 2024-03-13 16:54:18.758218 python_lokalise_api-2.2.0/lokalise/request.py
--rw-r--r--   0        0        0     1427 2022-07-27 15:15:30.268244 python_lokalise_api-2.2.0/lokalise/request_utils.py
--rw-r--r--   0        0        0      571 2021-08-19 13:33:19.797646 python_lokalise_api-2.2.0/lokalise/utils.py
--rw-r--r--   0        0        0     1622 2024-04-17 10:48:59.700522 python_lokalise_api-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2068 2024-04-17 10:47:55.143011 python_lokalise_api-2.2.0/README.md
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 python_lokalise_api-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-01-11 16:49:12.730266 python_lokalise_api-2.3.0/LICENSE
+-rw-r--r--   0        0        0      317 2022-10-05 17:09:24.598941 python_lokalise_api-2.3.0/lokalise/__init__.py
+-rw-r--r--   0        0        0      115 2023-02-27 17:36:02.975057 python_lokalise_api-2.3.0/lokalise/_version.py
+-rw-r--r--   0        0        0     1355 2022-11-30 21:18:17.855530 python_lokalise_api-2.3.0/lokalise/base_client.py
+-rw-r--r--   0        0        0    63236 2023-08-09 10:51:09.428371 python_lokalise_api-2.3.0/lokalise/client.py
+-rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/__init__.py
+-rw-r--r--   0        0        0     3424 2024-05-15 11:40:51.959556 python_lokalise_api-2.3.0/lokalise/collections/base_collection.py
+-rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/branches.py
+-rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/comments.py
+-rw-r--r--   0        0        0      389 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/contributors.py
+-rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/files.py
+-rw-r--r--   0        0        0      309 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/keys.py
+-rw-r--r--   0        0        0      373 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/languages.py
+-rw-r--r--   0        0        0      327 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/orders.py
+-rw-r--r--   0        0        0      387 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/payment_cards.py
+-rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/projects.py
+-rw-r--r--   0        0        0      404 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/queued_processes.py
+-rw-r--r--   0        0        0      372 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/screenshots.py
+-rw-r--r--   0        0        0      345 2021-12-17 13:27:20.711362 python_lokalise_api-2.3.0/lokalise/collections/segments.py
+-rw-r--r--   0        0        0      354 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/snapshots.py
+-rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/tasks.py
+-rw-r--r--   0        0        0      406 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/team_user_groups.py
+-rw-r--r--   0        0        0      360 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/team_users.py
+-rw-r--r--   0        0        0      318 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/teams.py
+-rw-r--r--   0        0        0      459 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/translation_providers.py
+-rw-r--r--   0        0        0      454 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/translation_statuses.py
+-rw-r--r--   0        0        0      381 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/translations.py
+-rw-r--r--   0        0        0      345 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/collections/webhooks.py
+-rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/__init__.py
+-rw-r--r--   0        0        0     4369 2023-02-27 17:36:02.975057 python_lokalise_api-2.3.0/lokalise/endpoints/base_endpoint.py
+-rw-r--r--   0        0        0      830 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/branches_endpoint.py
+-rw-r--r--   0        0        0      342 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/contributors_endpoint.py
+-rw-r--r--   0        0        0     1172 2022-07-27 15:15:30.268244 python_lokalise_api-2.3.0/lokalise/endpoints/files_endpoint.py
+-rw-r--r--   0        0        0      270 2023-01-11 16:49:12.732277 python_lokalise_api-2.3.0/lokalise/endpoints/jwt_endpoint.py
+-rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/key_comments_endpoint.py
+-rw-r--r--   0        0        0      294 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/keys_endpoint.py
+-rw-r--r--   0        0        0      332 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/languages_endpoint.py
+-rw-r--r--   0        0        0      295 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/orders_endpoint.py
+-rw-r--r--   0        0        0      317 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/payment_cards_endpoint.py
+-rw-r--r--   0        0        0      336 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/project_comments_endpoint.py
+-rw-r--r--   0        0        0      688 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/projects_endpoint.py
+-rw-r--r--   0        0        0      350 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/queued_processes_endpoint.py
+-rw-r--r--   0        0        0      333 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/screenshots_endpoint.py
+-rw-r--r--   0        0        0      331 2021-12-17 13:27:20.711362 python_lokalise_api-2.3.0/lokalise/endpoints/segments_endpoint.py
+-rw-r--r--   0        0        0      316 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/snapshots_endpoint.py
+-rw-r--r--   0        0        0      326 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/system_languages_endpoint.py
+-rw-r--r--   0        0        0      292 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/tasks_endpoint.py
+-rw-r--r--   0        0        0      384 2021-12-17 13:27:20.712362 python_lokalise_api-2.3.0/lokalise/endpoints/team_user_billing_details_endpoint.py
+-rw-r--r--   0        0        0     2735 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/team_user_groups_endpoint.py
+-rw-r--r--   0        0        0      313 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/team_users_endpoint.py
+-rw-r--r--   0        0        0      259 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/teams_endpoint.py
+-rw-r--r--   0        0        0      384 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/translation_providers_endpoint.py
+-rw-r--r--   0        0        0      802 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/translation_statuses_endpoint.py
+-rw-r--r--   0        0        0      334 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/translations_endpoint.py
+-rw-r--r--   0        0        0      701 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/endpoints/webhooks_endpoint.py
+-rw-r--r--   0        0        0     2449 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/errors.py
+-rw-r--r--   0        0        0        0 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/__init__.py
+-rw-r--r--   0        0        0     2880 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/base_model.py
+-rw-r--r--   0        0        0      405 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/branch.py
+-rw-r--r--   0        0        0      420 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/comment.py
+-rw-r--r--   0        0        0      499 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/contributor.py
+-rw-r--r--   0        0        0      272 2022-10-05 17:09:24.599953 python_lokalise_api-2.3.0/lokalise/models/file.py
+-rw-r--r--   0        0        0      220 2022-11-30 21:18:17.856531 python_lokalise_api-2.3.0/lokalise/models/jwt.py
+-rw-r--r--   0        0        0      815 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/key.py
+-rw-r--r--   0        0        0      383 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/language.py
+-rw-r--r--   0        0        0      738 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/order.py
+-rw-r--r--   0        0        0      387 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/payment_card.py
+-rw-r--r--   0        0        0      550 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/project.py
+-rw-r--r--   0        0        0      493 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/queued_process.py
+-rw-r--r--   0        0        0      495 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/screenshot.py
+-rw-r--r--   0        0        0      561 2021-12-17 13:27:20.712362 python_lokalise_api-2.3.0/lokalise/models/segment.py
+-rw-r--r--   0        0        0      416 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/snapshot.py
+-rw-r--r--   0        0        0      980 2023-02-27 17:36:02.976058 python_lokalise_api-2.3.0/lokalise/models/task.py
+-rw-r--r--   0        0        0      377 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/team.py
+-rw-r--r--   0        0        0      401 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/team_user.py
+-rw-r--r--   0        0        0      546 2021-12-17 13:27:20.712362 python_lokalise_api-2.3.0/lokalise/models/team_user_billing_details.py
+-rw-r--r--   0        0        0      471 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/team_user_group.py
+-rw-r--r--   0        0        0      636 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/translation.py
+-rw-r--r--   0        0        0      463 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/translation_provider.py
+-rw-r--r--   0        0        0      388 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/translation_status.py
+-rw-r--r--   0        0        0      362 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/models/webhook.py
+-rw-r--r--   0        0        0        0 2022-03-07 13:50:09.211635 python_lokalise_api-2.3.0/lokalise/oauth2/__init__.py
+-rw-r--r--   0        0        0     2771 2022-07-27 15:15:30.268244 python_lokalise_api-2.3.0/lokalise/oauth2/auth.py
+-rw-r--r--   0        0        0     1430 2022-07-27 15:15:30.268244 python_lokalise_api-2.3.0/lokalise/oauth2/request.py
+-rw-r--r--   0        0        0     1558 2021-10-27 12:17:46.650227 python_lokalise_api-2.3.0/lokalise/oauth_client.py
+-rw-r--r--   0        0        0     4873 2024-05-15 11:21:18.681079 python_lokalise_api-2.3.0/lokalise/request.py
+-rw-r--r--   0        0        0     1427 2022-07-27 15:15:30.268244 python_lokalise_api-2.3.0/lokalise/request_utils.py
+-rw-r--r--   0        0        0      571 2021-08-19 13:33:19.797646 python_lokalise_api-2.3.0/lokalise/utils.py
+-rw-r--r--   0        0        0     1622 2024-05-15 11:33:31.547308 python_lokalise_api-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2068 2024-04-17 10:47:55.143011 python_lokalise_api-2.3.0/README.md
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 python_lokalise_api-2.3.0/PKG-INFO
```

### Comparing `python_lokalise_api-2.2.0/LICENSE` & `python_lokalise_api-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/base_client.py` & `python_lokalise_api-2.3.0/lokalise/base_client.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/client.py` & `python_lokalise_api-2.3.0/lokalise/client.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/collections/base_collection.py` & `python_lokalise_api-2.3.0/lokalise/collections/base_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         pagination = raw_data.get("_pagination", {})
         if pagination:
             self.total_count = int(pagination.get(
                 "x-pagination-total-count", 0))
             self.page_count = int(pagination.get("x-pagination-page-count", 0))
             self.limit = int(pagination.get("x-pagination-limit", 0))
             self.current_page = int(pagination.get("x-pagination-page", 0))
+            self.next_cursor = pagination.get("x-pagination-next-cursor", None)
 
     def is_last_page(self) -> bool:
         """Checks whether the current collection set is the last page.
 
         :rtype: bool
         """
         return not self.has_next_page()
@@ -81,14 +82,21 @@
     def has_prev_page(self) -> bool:
         """Checks whether the current collection set has the previous page.
 
         :rtype: bool
         """
         return self.current_page > 1
 
+    def has_next_cursor(self) -> bool:
+        """Checks whether the current collection set has the next cursor.
+
+        :rtype: bool
+        """
+        return self.next_cursor is not None
+
     def __extract_common_attrs(self, raw_data: Dict) -> None:
         """Fetches common data from the response and sets the
         corresponding attributes.
         """
         for attr in self.COMMON_ATTRS:
             if attr in raw_data:
                 setattr(self, attr, raw_data[attr])
```

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/base_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/branches_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/branches_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/files_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/files_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/projects_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/projects_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/team_user_groups_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/team_user_groups_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/translation_statuses_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/translation_statuses_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/endpoints/webhooks_endpoint.py` & `python_lokalise_api-2.3.0/lokalise/endpoints/webhooks_endpoint.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/errors.py` & `python_lokalise_api-2.3.0/lokalise/errors.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/base_model.py` & `python_lokalise_api-2.3.0/lokalise/models/base_model.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/key.py` & `python_lokalise_api-2.3.0/lokalise/models/key.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/order.py` & `python_lokalise_api-2.3.0/lokalise/models/order.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/project.py` & `python_lokalise_api-2.3.0/lokalise/models/project.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/segment.py` & `python_lokalise_api-2.3.0/lokalise/models/segment.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/task.py` & `python_lokalise_api-2.3.0/lokalise/models/task.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/team_user_billing_details.py` & `python_lokalise_api-2.3.0/lokalise/models/team_user_billing_details.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/models/translation.py` & `python_lokalise_api-2.3.0/lokalise/models/translation.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/oauth2/auth.py` & `python_lokalise_api-2.3.0/lokalise/oauth2/auth.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/oauth2/request.py` & `python_lokalise_api-2.3.0/lokalise/oauth2/request.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/oauth_client.py` & `python_lokalise_api-2.3.0/lokalise/oauth_client.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/request.py` & `python_lokalise_api-2.3.0/lokalise/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 
 BASE_URL = "https://api.lokalise.com/api2/"
 PAGINATION_HEADERS = [
     "x-pagination-total-count",
     "x-pagination-page-count",
     "x-pagination-limit",
-    "x-pagination-page"
+    "x-pagination-page",
+    "x-pagination-next-cursor"
 ]
 
 
 def get(client: lokalise.client.Client, path: str,
         params: Optional[Dict] = None) -> Dict:
     """Performs GET requests
```

### Comparing `python_lokalise_api-2.2.0/lokalise/request_utils.py` & `python_lokalise_api-2.3.0/lokalise/request_utils.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/lokalise/utils.py` & `python_lokalise_api-2.3.0/lokalise/utils.py`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/pyproject.toml` & `python_lokalise_api-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-lokalise-api"
-version = "2.2.0"
+version = "2.3.0"
 description = "Official Python interface for the Lokalise API v2"
 authors = ["Ilya Krukowski <golosizpru@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/lokalise/python-lokalise-api"
 documentation = "https://python-lokalise-api.readthedocs.io/"
 keywords = ["lokalise", "api", "client"]
```

### Comparing `python_lokalise_api-2.2.0/README.md` & `python_lokalise_api-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python_lokalise_api-2.2.0/PKG-INFO` & `python_lokalise_api-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lokalise-api
-Version: 2.2.0
+Version: 2.3.0
 Summary: Official Python interface for the Lokalise API v2
 Home-page: https://github.com/lokalise/python-lokalise-api
 License: BSD-3-Clause
 Keywords: lokalise,api,client
 Author: Ilya Krukowski
 Author-email: golosizpru@gmail.com
 Requires-Python: >=3.8,<4.0
```

