# Comparing `tmp/fb-python-sdk-1.1.5.tar.gz` & `tmp/fb_python_sdk-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.1.5.tar", last modified: Sun Jun 25 15:58:25 2023, max compression
+gzip compressed data, was "fb_python_sdk-1.1.6.tar", last modified: Wed May 15 18:08:23 2024, max compression
```

## Comparing `fb-python-sdk-1.1.5.tar` & `fb_python_sdk-1.1.6.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 15:58:25.000000 fb-python-sdk-1.1.5/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fbclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/category.py
--rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/data_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/event_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/flag_change_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/notice_broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/status_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/update_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/fbclient/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/repeatable_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/fbclient/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.945436 fb-python-sdk-1.1.5/release/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/release/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:25.949436 fb-python-sdk-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_data_update_status_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_event_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_fbclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 15:58:15.000000 fb-python-sdk-1.1.5/tests/test_flag_change_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.527006 fb_python_sdk-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-15 18:08:23.527006 fb_python_sdk-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.527006 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-15 18:08:23.000000 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-15 18:08:23.000000 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:08:23.000000 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 18:08:23.000000 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 18:08:23.000000 fb_python_sdk-1.1.6/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.523005 fb_python_sdk-1.1.6/fbclient/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/flag_change_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/notice_broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/status_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/update_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.523005 fb_python_sdk-1.1.6/fbclient/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.523005 fb_python_sdk-1.1.6/release/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/release/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:08:23.527006 fb_python_sdk-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:23.527006 fb_python_sdk-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_data_update_status_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_fbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-15 18:08:18.000000 fb_python_sdk-1.1.6/tests/test_flag_change_notification.py
```

### Comparing `fb-python-sdk-1.1.5/LICENSE` & `fb_python_sdk-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/PKG-INFO` & `fb_python_sdk-1.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: fb-python-sdk
-Version: 1.1.5
-Summary: A Python SDK for FeatBit plateform
-Home-page: https://github.com/featbit/featbit-python-sdk
-Author: Dian SUN
-Author-email: featbit.master@gmail.com
-Project-URL: Code, https://github.com/featbit/featbit-python-sdk
-Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # FeatBit Server-Side SDK for Python
 
 ## Introduction
 
 This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
 The FeatBit Server-Side SDK for Python is designed primarily for use in multi-user systems such as web servers and applications.
@@ -52,16 +26,16 @@
 
 ### Prerequisite
 
 Before using the SDK, you need to obtain the environment secret and SDK URLs. 
 
 Follow the documentation below to retrieve these values
 
-- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
-- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+- [How to get the environment secret](https://docs.featbit.co/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/sdk/faq#how-to-get-the-sdk-urls)
   
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
@@ -187,27 +161,27 @@
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
 
 The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
 or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
 
-When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+When you track a flag change using `add_flag_value_maybe_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
 
 If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
 
 Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
 If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
 
 ```python
 if client.initialize:
     #  flag value may be changed
-    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_maybe_changed_listener(flag_key, user, flag_value_maybe_changed_callback_fn)
     #  flag value must be changed
-    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, flag_value_changed_callback_fn)
 
 ```
 `flag_key`: the key of the feature flag to track
 
 `user`: the user to evaluate the flag value
 
 `callback_fn`: the function to be called for the flag value change
@@ -257,8 +231,8 @@
 
 - If you have a specific question about using this sdk, we encourage you
   to [ask it in our slack](https://join.slack.com/t/featbit/shared_invite/zt-1ew5e2vbb-x6Apan1xZOaYMnFzqZkGNQ).
 - If you encounter a bug or would like to request a
   feature, [submit an issue](https://github.com/featbit/featbit-python-sdk/issues/new).
 
 ## See Also
-- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
+- [Connect To Python Sdk](https://docs.featbit.co/sdk/overview#python)
```

### Comparing `fb-python-sdk-1.1.5/README.md` & `fb_python_sdk-1.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: fb-python-sdk
+Version: 1.1.6
+Summary: A Python SDK for FeatBit plateform
+Home-page: https://github.com/featbit/featbit-python-sdk
+Author: Dian SUN
+Author-email: featbit.master@gmail.com
+Project-URL: Code, https://github.com/featbit/featbit-python-sdk
+Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6, <=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: certifi>=2018.4.16
+Requires-Dist: urllib3>=1.22.0
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: websocket-client>=1.0.0
+Provides-Extra: dev
+Requires-Dist: certifi>=2018.4.16; extra == "dev"
+Requires-Dist: urllib3>=1.22.0; extra == "dev"
+Requires-Dist: websocket-client>=1.0.0; extra == "dev"
+Requires-Dist: python-dateutil>=2.8.2; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 # FeatBit Server-Side SDK for Python
 
 ## Introduction
 
 This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
 The FeatBit Server-Side SDK for Python is designed primarily for use in multi-user systems such as web servers and applications.
@@ -26,16 +67,16 @@
 
 ### Prerequisite
 
 Before using the SDK, you need to obtain the environment secret and SDK URLs. 
 
 Follow the documentation below to retrieve these values
 
-- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
-- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+- [How to get the environment secret](https://docs.featbit.co/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/sdk/faq#how-to-get-the-sdk-urls)
   
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
@@ -161,27 +202,27 @@
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
 
 The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
 or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
 
-When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+When you track a flag change using `add_flag_value_maybe_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
 
 If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
 
 Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
 If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
 
 ```python
 if client.initialize:
     #  flag value may be changed
-    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_maybe_changed_listener(flag_key, user, flag_value_maybe_changed_callback_fn)
     #  flag value must be changed
-    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, flag_value_changed_callback_fn)
 
 ```
 `flag_key`: the key of the feature flag to track
 
 `user`: the user to evaluate the flag value
 
 `callback_fn`: the function to be called for the flag value change
@@ -231,8 +272,8 @@
 
 - If you have a specific question about using this sdk, we encourage you
   to [ask it in our slack](https://join.slack.com/t/featbit/shared_invite/zt-1ew5e2vbb-x6Apan1xZOaYMnFzqZkGNQ).
 - If you encounter a bug or would like to request a
   feature, [submit an issue](https://github.com/featbit/featbit-python-sdk/issues/new).
 
 ## See Also
-- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
+- [Connect To Python Sdk](https://docs.featbit.co/sdk/overview#python)
```

### Comparing `fb-python-sdk-1.1.5/fb_python_sdk.egg-info/PKG-INFO` & `fb_python_sdk-1.1.6/fb_python_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,18 +15,33 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <=3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6, <=3.12
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: certifi>=2018.4.16
+Requires-Dist: urllib3>=1.22.0
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: websocket-client>=1.0.0
+Provides-Extra: dev
+Requires-Dist: certifi>=2018.4.16; extra == "dev"
+Requires-Dist: urllib3>=1.22.0; extra == "dev"
+Requires-Dist: websocket-client>=1.0.0; extra == "dev"
+Requires-Dist: python-dateutil>=2.8.2; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # FeatBit Server-Side SDK for Python
 
 ## Introduction
 
 This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
@@ -52,16 +67,16 @@
 
 ### Prerequisite
 
 Before using the SDK, you need to obtain the environment secret and SDK URLs. 
 
 Follow the documentation below to retrieve these values
 
-- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
-- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+- [How to get the environment secret](https://docs.featbit.co/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/sdk/faq#how-to-get-the-sdk-urls)
   
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
@@ -187,27 +202,27 @@
 `fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
 
 Note that a flag value change listener is bound to a specific user and flag key.
 
 The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
 or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
 
-When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+When you track a flag change using `add_flag_value_maybe_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
 
 If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
 
 Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
 If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
 
 ```python
 if client.initialize:
     #  flag value may be changed
-    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_maybe_changed_listener(flag_key, user, flag_value_maybe_changed_callback_fn)
     #  flag value must be changed
-    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, flag_value_changed_callback_fn)
 
 ```
 `flag_key`: the key of the feature flag to track
 
 `user`: the user to evaluate the flag value
 
 `callback_fn`: the function to be called for the flag value change
@@ -257,8 +272,8 @@
 
 - If you have a specific question about using this sdk, we encourage you
   to [ask it in our slack](https://join.slack.com/t/featbit/shared_invite/zt-1ew5e2vbb-x6Apan1xZOaYMnFzqZkGNQ).
 - If you encounter a bug or would like to request a
   feature, [submit an issue](https://github.com/featbit/featbit-python-sdk/issues/new).
 
 ## See Also
-- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
+- [Connect To Python Sdk](https://docs.featbit.co/sdk/overview#python)
```

### Comparing `fb-python-sdk-1.1.5/fb_python_sdk.egg-info/SOURCES.txt` & `fb_python_sdk-1.1.6/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 fbclient/flag_change_notification.py
 fbclient/interfaces.py
 fbclient/notice_broadcaster.py
 fbclient/status.py
 fbclient/status_types.py
 fbclient/streaming.py
 fbclient/update_processor.py
-fbclient/version.py
 fbclient/utils/__init__.py
 fbclient/utils/exponential_backoff_jitter_strategy.py
 fbclient/utils/http_client.py
 fbclient/utils/repeatable_task.py
 fbclient/utils/rwlock.py
 fbclient/utils/variation_splitting_algorithm.py
 release/package.json
```

### Comparing `fb-python-sdk-1.1.5/fbclient/__init__.py` & `fb_python_sdk-1.1.6/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/category.py` & `fb_python_sdk-1.1.6/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/client.py` & `fb_python_sdk-1.1.6/fbclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,15 @@
         Our feature flag center supports to track pageviews and clicks that are specified in the dashboard UI.
         This can be used to track custom metric.
 
         :param user: the attributes of the user
         :param event_name: the name of the event, which may correspond to a goal in A/B tests
         :param metric_value: a numeric value used by the experiment, default value is 1.0
         """
-        if not event_name or metric_value <= 0:
+        if not event_name:
             log.warning('FB Python SDK: event/metric invalid')
             return
         try:
             fb_user = FBUser.from_dict(user)
         except ValueError:
             log.warning('FB Python SDK: user invalid')
             return
@@ -371,15 +371,15 @@
             fb_user = FBUser.from_dict(user)
         except ValueError:
             log.warning('FB Python SDK: user invalid')
             return
 
         metric_event = MetricEvent(fb_user)
         for event_name, metric_value in metrics.items():
-            if event_name and metric_value > 0:
+            if event_name:
                 metric_event.add(Metric(event_name, metric_value))
         self._event_handler(metric_event)
 
     def initialize_from_external_json(self, json_str: str) -> bool:
         """SDK initialization in the offline mode, this method is mainly used for tests
 
         :param json_str: feature flags, segments...etc in the json format
```

### Comparing `fb-python-sdk-1.1.5/fbclient/common_types.py` & `fb_python_sdk-1.1.6/fbclient/common_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/config.py` & `fb_python_sdk-1.1.6/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/data_storage.py` & `fb_python_sdk-1.1.6/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/evaluator.py` & `fb_python_sdk-1.1.6/fbclient/evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/event_processor.py` & `fb_python_sdk-1.1.6/fbclient/event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/event_types.py` & `fb_python_sdk-1.1.6/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/flag_change_notification.py` & `fb_python_sdk-1.1.6/fbclient/flag_change_notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,41 +34,41 @@
 
 
 class FlagValueChangedListener(FlagChangedListener):
     def __init__(self,
                  flag_key: str,
                  user: dict,
                  evaluate_fn: Callable[[str, dict, Any], Any],
-                 flag_value_changed_fn: Callable[[str, Any], None]):
+                 flag_value_changed_fn: Callable[[str, Any, Any], None]):
         self.__flag_key = flag_key
         self.__user = user
         self.__evaluate_fn = evaluate_fn
         self.__fn = flag_value_changed_fn
         # record the flag value when the listener is created
         self.__prvious_flag_value = self.__evaluate_fn(self.__flag_key, self.__user, None)
 
     def on_flag_change(self, notice: FlagChangedNotice):
         if notice.flag_key == self.__flag_key:
             prev_flag_value = self.__prvious_flag_value
             curr_flag_value = self.__evaluate_fn(self.__flag_key, self.__user, None)
             if prev_flag_value != curr_flag_value:
-                self.__fn(self.__flag_key, curr_flag_value)
+                self.__fn(self.__flag_key, prev_flag_value, curr_flag_value)
                 self.__prvious_flag_value = curr_flag_value
 
 
-class FlagValueMayChangedListener(FlagChangedListener):
+class FlagValueMaybeChangedListener(FlagChangedListener):
     def __init__(self,
                  flag_key: str,
                  user: dict,
                  evaluate_fn: Callable[[str, dict, Any], Any],
-                 flag_value_changed_fn: Callable[[str, Any], None]):
+                 flag_value_maybe_changed_fn: Callable[[str, Any], None]):
         self.__flag_key = flag_key
         self.__user = user
         self.__evaluate_fn = evaluate_fn
-        self.__fn = flag_value_changed_fn
+        self.__fn = flag_value_maybe_changed_fn
 
     def on_flag_change(self, notice: FlagChangedNotice):
         if notice.flag_key == self.__flag_key:
             curr_flag_value = self.__evaluate_fn(self.__flag_key, self.__user, None)
             self.__fn(self.__flag_key, curr_flag_value)
 
 
@@ -91,30 +91,31 @@
         """
         self.__broadcater = flag_change_broadcaster
         self.__evaluate_fn = evaluate_fn
 
     def add_flag_value_changed_listener(self,
                                         flag_key: str,
                                         user: dict,
-                                        flag_value_changed_fn: Callable[[str, Any], None]) -> FlagValueChangedListener:
+                                        flag_value_changed_fn: Callable[[str, Any, Any], None]) -> FlagValueChangedListener:
         """
         Registers a listener to be notified of a change in a specific feature flag's value for a specific FeatBit user.
 
         The listener will be notified whenever the SDK receives any change to any feature flag's configuration,
         or to a user segment that is referenced by a feature flag.
 
         When you call this method, it first immediately evaluates the feature flag. It then uses :class:`FlagChangeListener` to start listening for feature flag configuration
         changes, and whenever the specified feature flag changes, it re-evaluates the flag for the same user. It then calls :class:`FlagValueChangeListener`
         if and only if the resulting value has changed.
 
         :param flag_key: The key of the feature flag to track
         :param user: The user to evaluate the flag value
         :param flag_value_changed_fn: The function to be called only when this flag value changes
             * the first argument is the flag key
-            * the second argument is the latest flag value, this value must be different from the previous value
+            * the second argument is the previous flag value
+            * the third argument is the current flag value
 
         :return: A listener object that can be used to remove it later on.
         """
 
         # check flag key
         if not isinstance(flag_key, str) or not flag_key:
             raise ValueError('flag_key must be a non-empty string')
@@ -124,49 +125,49 @@
         if not isinstance(flag_value_changed_fn, Callable) or not flag_value_changed_fn:
             raise ValueError('flag_value_changed_fn must be a callable function')
 
         listener = FlagValueChangedListener(flag_key, user, self.__evaluate_fn, flag_value_changed_fn)
         self.add_flag_changed_listener(listener)
         return listener
 
-    def add_flag_value_may_changed_listener(self,
-                                            flag_key: str,
-                                            user: dict,
-                                            flag_value_changed_fn: Callable[[str, Any], None]) -> FlagValueMayChangedListener:
+    def add_flag_value_maybe_changed_listener(self,
+                                              flag_key: str,
+                                              user: dict,
+                                              flag_value_maybe_changed_fn: Callable[[str, Any], None]) -> FlagValueMaybeChangedListener:
         """
         Registers a listener to be notified of a change in a specific feature flag's value for a specific FeatBit user.
 
         The listener will be notified whenever the SDK receives any change to any feature flag's configuration,
         or to a user segment that is referenced by a feature flag.
 
         Note that this does not necessarily mean the flag's value has changed for any particular flag,
         only that some part of the flag configuration was changed so that it may return a different value than it previously returned for some user.
 
         If you want to track flag value changes,use :func:`add_flag_value_changed_listener instead.
 
         :param flag_key: The key of the feature flag to track
         :param user: The user to evaluate the flag value
-        :param flag_value_changed_fn: The function to be called only if any changes to a specific flag
+        :param flag_value_maybe_changed_fn: The function to be called if any changes to a specific flag
             * the first argument is the flag key
             * the second argument is the latest flag value, this value may be same as the previous value
 
         :return: A listener object that can be used to remove it later on.
 
         """
 
         # check flag key
         if not isinstance(flag_key, str) or not flag_key:
             raise ValueError('flag_key must be a non-empty string')
         # check user
         FBUser.from_dict(user)
         # check flag_value_changed_fn
-        if not isinstance(flag_value_changed_fn, Callable) or not flag_value_changed_fn:
+        if not isinstance(flag_value_maybe_changed_fn, Callable) or not flag_value_maybe_changed_fn:
             raise ValueError('flag_value_changed_fn must be a callable function')
 
-        listener = FlagValueMayChangedListener(flag_key, user, self.__evaluate_fn, flag_value_changed_fn)
+        listener = FlagValueMaybeChangedListener(flag_key, user, self.__evaluate_fn, flag_value_maybe_changed_fn)
         self.add_flag_changed_listener(listener)
         return listener
 
     def add_flag_changed_listener(self, listener: FlagChangedListener):
         """
         Registers a listener to be notified of feature flag changes in general.
```

### Comparing `fb-python-sdk-1.1.5/fbclient/interfaces.py` & `fb_python_sdk-1.1.6/fbclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/notice_broadcaster.py` & `fb_python_sdk-1.1.6/fbclient/notice_broadcaster.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/status.py` & `fb_python_sdk-1.1.6/fbclient/status.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/status_types.py` & `fb_python_sdk-1.1.6/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/streaming.py` & `fb_python_sdk-1.1.6/fbclient/streaming.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/update_processor.py` & `fb_python_sdk-1.1.6/fbclient/update_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/__init__.py` & `fb_python_sdk-1.1.6/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb_python_sdk-1.1.6/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/http_client.py` & `fb_python_sdk-1.1.6/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/repeatable_task.py` & `fb_python_sdk-1.1.6/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/rwlock.py` & `fb_python_sdk-1.1.6/fbclient/utils/rwlock.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             self._readers += 1
 
     def release_read_lock(self):
         """ Release a read lock. """
         with self._read_ready:
             self._readers = self._readers - 1 if self._readers > 0 else 0
             if self._readers == 0:
-                self._read_ready.notifyAll()
+                self._read_ready.notify_all()
 
     def write_lock(self):
         """ Acquire a write lock. Blocks until there are no
         acquired read or write locks. """
         self._read_ready.acquire()
         while self._readers > 0:
             self._read_ready.wait()
```

### Comparing `fb-python-sdk-1.1.5/fbclient/utils/variation_splitting_algorithm.py` & `fb_python_sdk-1.1.6/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/setup.py` & `fb_python_sdk-1.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         'Topic :: Software Development :: Libraries',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     extras_require={
         "dev": dev_reqs
     },
     tests_require=dev_reqs,
-    python_requires='>=3.6, <=3.11'
+    python_requires='>=3.6, <=3.12'
 )
```

### Comparing `fb-python-sdk-1.1.5/tests/test_data_storage.py` & `fb_python_sdk-1.1.6/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/tests/test_data_update_status_provider.py` & `fb_python_sdk-1.1.6/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/tests/test_evaluator.py` & `fb_python_sdk-1.1.6/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/tests/test_event_processor.py` & `fb_python_sdk-1.1.6/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/tests/test_fbclient.py` & `fb_python_sdk-1.1.6/tests/test_fbclient.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.5/tests/test_flag_change_notification.py` & `fb_python_sdk-1.1.6/tests/test_flag_change_notification.py`

 * *Files identical despite different names*

