# Comparing `tmp/nextline_schedule-0.3.0.tar.gz` & `tmp/nextline_schedule-0.3.1.tar.gz`

## Comparing `nextline_schedule-0.3.0.tar` & `nextline_schedule-0.3.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/release.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/dummy.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/py.typed
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/auto_mode.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/__init__.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/factory.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/machine.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/QueuePush.gql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/AutoMode.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/QueueItems.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/Version.gql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/pubsub_queue.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/queue.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/strategies.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/mutation.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/query.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/subscription.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/mutation.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/query.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/subscription.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/types.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/__init__.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/safe.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/utc.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/datetime.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/misc.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_plugin.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_request.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_scratch.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/__init__.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/state_machine/__init__.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/state_machine/test_fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/test_pubsub_queue.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/test_queue.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/mutations/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/mutations/test_queue_push.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/test_queue_items.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/test_safe_compare.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/test_safe_min_max.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_datetimes.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_ints.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_python_scripts.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_ranges.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/README.md
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/dummy.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/py.typed
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/auto_mode.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/state_machine/factory.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/auto/state_machine/machine.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/mutations/QueuePush.gql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/queries/AutoMode.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/queries/QueueItems.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/queries/Version.gql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/queue/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/queue/pubsub_queue.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/queue/queue.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/queue/strategies.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/mutation.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/query.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/subscription.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/mutation.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/query.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/subscription.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/types.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/safe.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/utc.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/datetime.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/misc.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/test_request.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/test_scratch.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/auto/state_machine/test_fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/queue/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/queue/test_pubsub_queue.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/queue/test_queue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/mutations/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/mutations/test_queue_push.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/queries/test_queue_items.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/schema/queries/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/test_safe_compare.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/test_safe_min_max.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/strategies/test_st_datetimes.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/strategies/test_st_ints.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/strategies/test_st_python_scripts.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/tests/utils/strategies/test_st_ranges.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/README.md
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 nextline_schedule-0.3.1/PKG-INFO
```

### Comparing `nextline_schedule-0.3.0/.github/workflows/pypi.yml` & `nextline_schedule-0.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/.github/workflows/release.yml` & `nextline_schedule-0.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/.github/workflows/type-check.yml` & `nextline_schedule-0.3.1/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/.github/workflows/unit-test.yml` & `nextline_schedule-0.3.1/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/plugin.py` & `nextline_schedule-0.3.1/src/nextline_schedule/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/scheduler.py` & `nextline_schedule-0.3.1/src/nextline_schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/auto/auto_mode.py` & `nextline_schedule-0.3.1/src/nextline_schedule/auto/auto_mode.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/auto/callback.py` & `nextline_schedule-0.3.1/src/nextline_schedule/auto/callback.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/factory.py` & `nextline_schedule-0.3.1/src/nextline_schedule/auto/state_machine/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/machine.py` & `nextline_schedule-0.3.1/src/nextline_schedule/auto/state_machine/machine.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/graphql/__init__.py` & `nextline_schedule-0.3.1/src/nextline_schedule/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/queue/pubsub_queue.py` & `nextline_schedule-0.3.1/src/nextline_schedule/queue/pubsub_queue.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/queue/queue.py` & `nextline_schedule-0.3.1/src/nextline_schedule/queue/queue.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/queue/strategies.py` & `nextline_schedule-0.3.1/src/nextline_schedule/queue/strategies.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/mutation.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/subscription.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/subscription.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/mutation.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/query.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/subscription.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/auto/subscription.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/mutation.py` & `nextline_schedule-0.3.1/src/nextline_schedule/schema/queue/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/utils/safe.py` & `nextline_schedule-0.3.1/src/nextline_schedule/utils/safe.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/utils/utc.py` & `nextline_schedule-0.3.1/src/nextline_schedule/utils/utc.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/datetime.py` & `nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/datetime.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/misc.py` & `nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/misc.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/script.py` & `nextline_schedule-0.3.1/src/nextline_schedule/utils/strategies/script.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/test_plugin.py` & `nextline_schedule-0.3.1/tests/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 from collections.abc import AsyncIterator
 
 import pytest
-from async_asgi_testclient import TestClient
 from nextlinegraphql import create_app
 from nextlinegraphql.plugins.ctrl.graphql import SUBSCRIBE_STATE
-from nextlinegraphql.plugins.graphql.test import gql_request, gql_subscribe
+from nextlinegraphql.plugins.graphql.test import TestClient, gql_request, gql_subscribe
 from pytest_httpx import HTTPXMock
 
 from nextline_schedule.graphql import (
     MUTATE_AUTO_MODE_TURN_OFF,
     MUTATE_AUTO_MODE_TURN_ON,
     QUERY_AUTO_MODE,
     QUERY_SCHEDULER,
@@ -45,23 +44,23 @@
     expected = {'schedule': {'autoMode': {'state': 'off'}}}
     assert data == expected
 
     data = await gql_request(client, MUTATE_AUTO_MODE_TURN_ON)
 
     n_runs = 0
     async for data in gql_subscribe(client, SUBSCRIBE_STATE):
-        if data['state'] == 'running':
+        if data['ctrlState'] == 'running':
             turned_on.set()
             n_runs += 1
         if n_runs >= 3:
             data = await gql_request(client, MUTATE_AUTO_MODE_TURN_OFF)
             break
 
     async for data in gql_subscribe(client, SUBSCRIBE_STATE):
-        if data['state'] == 'finished':
+        if data['ctrlState'] == 'finished':
             break
 
     await task
 
 
 async def subscribe_auto_mode_state(client: TestClient, turned_on: asyncio.Event):
     await turned_on.wait()
```

### Comparing `nextline_schedule-0.3.0/tests/test_request.py` & `nextline_schedule-0.3.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/test_scratch.py` & `nextline_schedule-0.3.1/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/auto/test_auto.py` & `nextline_schedule-0.3.1/tests/auto/test_auto.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/auto/test_auto_on_raised.py` & `nextline_schedule-0.3.1/tests/auto/test_auto_on_raised.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/auto/test_auto_turn_off.py` & `nextline_schedule-0.3.1/tests/auto/test_auto_turn_off.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/auto/state_machine/test_fsm.py` & `nextline_schedule-0.3.1/tests/auto/state_machine/test_fsm.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/queue/test_pubsub_queue.py` & `nextline_schedule-0.3.1/tests/queue/test_pubsub_queue.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/queue/test_queue.py` & `nextline_schedule-0.3.1/tests/queue/test_queue.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/schema/mutations/test_queue_push.py` & `nextline_schedule-0.3.1/tests/schema/mutations/test_queue_push.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/schema/queries/test_queue_items.py` & `nextline_schedule-0.3.1/tests/schema/queries/test_queue_items.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/utils/test_safe_compare.py` & `nextline_schedule-0.3.1/tests/utils/test_safe_compare.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/utils/test_safe_min_max.py` & `nextline_schedule-0.3.1/tests/utils/test_safe_min_max.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/utils/strategies/test_st_ints.py` & `nextline_schedule-0.3.1/tests/utils/strategies/test_st_ints.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/tests/utils/strategies/test_st_ranges.py` & `nextline_schedule-0.3.1/tests/utils/strategies/test_st_ranges.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/.gitignore` & `nextline_schedule-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/LICENSE.txt` & `nextline_schedule-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/README.md` & `nextline_schedule-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.0/pyproject.toml` & `nextline_schedule-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,24 @@
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
+  "nextline-graphql>=0.7.8",
   "transitions>=0.9",
   "httpx>=0.23",
   "hypothesis>=6.65",
   "black>=23.10",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-host = ["nextline-graphql>=0.7.7"]
 tests = [
-  "async-asgi-testclient>=1.4",
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
   "pytest-httpx>=0.21",
 ]
```

### Comparing `nextline_schedule-0.3.0/PKG-INFO` & `nextline_schedule-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-schedule
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin of nextline-graphql. An interface to the SO scheduler.
 Project-URL: Documentation, https://github.com/simonsobs/nextline-schedule#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-schedule/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-schedule
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,19 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: black>=23.10
 Requires-Dist: httpx>=0.23
 Requires-Dist: hypothesis>=6.65
+Requires-Dist: nextline-graphql>=0.7.8
 Requires-Dist: transitions>=0.9
-Provides-Extra: host
-Requires-Dist: nextline-graphql>=0.7.7; extra == 'host'
 Provides-Extra: tests
-Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-httpx>=0.21; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
 Description-Content-Type: text/markdown
```

