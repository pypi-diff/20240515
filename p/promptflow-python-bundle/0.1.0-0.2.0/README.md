# Comparing `tmp/promptflow_python_bundle-0.1.0-py3-none-any.whl.zip` & `tmp/promptflow_python_bundle-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 6781 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      183 b- defN 24-Apr-17 06:40 promptflow_python/__init__.py
--rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-17 06:45 promptflow_python/_version.py
--rw-rw-rw-  2.0 fat     2728 b- defN 24-Apr-17 06:40 promptflow_python/start_server.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-Apr-17 06:40 promptflow_python/package_data/runit/promptflow-python/finish
--rw-rw-rw-  2.0 fat     1457 b- defN 24-Apr-17 06:40 promptflow_python/package_data/runit/promptflow-python/run
--rw-rw-rw-  2.0 fat     2439 b- defN 24-Apr-17 06:40 promptflow_python/package_data/scripts/auto_detect_env.sh
--rw-rw-rw-  2.0 fat      410 b- defN 24-Apr-17 06:40 promptflow_python/package_data/scripts/start.sh
--rw-rw-rw-  2.0 fat     1696 b- defN 24-Apr-17 06:45 promptflow_python_bundle-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 06:45 promptflow_python_bundle-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 06:45 promptflow_python_bundle-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-17 06:45 promptflow_python_bundle-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1186 b- defN 24-Apr-17 06:45 promptflow_python_bundle-0.1.0.dist-info/RECORD
-12 files, 10717 bytes uncompressed, 4713 bytes compressed:  56.0%
+Zip file size: 9536 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      183 b- defN 24-May-15 08:46 promptflow_python/__init__.py
+-rw-rw-rw-  2.0 fat       19 b- defN 24-May-15 08:49 promptflow_python/_version.py
+-rw-rw-rw-  2.0 fat     2728 b- defN 24-May-15 08:46 promptflow_python/start_server.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-15 08:46 promptflow_python/package_data/runit/promptflow-python/finish
+-rw-rw-rw-  2.0 fat     1967 b- defN 24-May-15 08:46 promptflow_python/package_data/runit/promptflow-python/run
+-rw-rw-rw-  2.0 fat      935 b- defN 24-May-15 08:46 promptflow_python/package_data/runit/token-provider/run
+-rw-rw-rw-  2.0 fat     4262 b- defN 24-May-15 08:46 promptflow_python/package_data/runit/token-provider/token_provider.py
+-rw-rw-rw-  2.0 fat     2936 b- defN 24-May-15 08:46 promptflow_python/package_data/scripts/auto_detect_env.sh
+-rw-rw-rw-  2.0 fat      410 b- defN 24-May-15 08:46 promptflow_python/package_data/scripts/start.sh
+-rw-rw-rw-  2.0 fat     1696 b- defN 24-May-15 08:49 promptflow_python_bundle-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 08:49 promptflow_python_bundle-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-15 08:49 promptflow_python_bundle-0.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       18 b- defN 24-May-15 08:49 promptflow_python_bundle-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1423 b- defN 24-May-15 08:49 promptflow_python_bundle-0.2.0.dist-info/RECORD
+14 files, 17158 bytes uncompressed, 7068 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -9,29 +9,35 @@
 
 Filename: promptflow_python/package_data/runit/promptflow-python/finish
 Comment: 
 
 Filename: promptflow_python/package_data/runit/promptflow-python/run
 Comment: 
 
+Filename: promptflow_python/package_data/runit/token-provider/run
+Comment: 
+
+Filename: promptflow_python/package_data/runit/token-provider/token_provider.py
+Comment: 
+
 Filename: promptflow_python/package_data/scripts/auto_detect_env.sh
 Comment: 
 
 Filename: promptflow_python/package_data/scripts/start.sh
 Comment: 
 
-Filename: promptflow_python_bundle-0.1.0.dist-info/METADATA
+Filename: promptflow_python_bundle-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_python_bundle-0.1.0.dist-info/WHEEL
+Filename: promptflow_python_bundle-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_python_bundle-0.1.0.dist-info/entry_points.txt
+Filename: promptflow_python_bundle-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: promptflow_python_bundle-0.1.0.dist-info/top_level.txt
+Filename: promptflow_python_bundle-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: promptflow_python_bundle-0.1.0.dist-info/RECORD
+Filename: promptflow_python_bundle-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow_python/_version.py

```diff
@@ -1 +1 @@
-VERSION = "0.1.0"
+VERSION = "0.2.0"
```

## promptflow_python/package_data/runit/promptflow-python/run

```diff
@@ -13,17 +13,26 @@
 RUN_MODE=${PROMPTFLOW_RUN_MODE:-"compute"}
 
 if [ "$RUN_MODE" = "serving" ]; then
     # https://docs.gunicorn.org/en/latest/settings.html#threads
     # If you try to use the sync worker type and set the threads setting to more than 1, the gthread worker type will be used instead.
     WORKER_NUM=${PROMPTFLOW_WORKER_NUM:-"8"}
     WORKER_THREADS=${PROMPTFLOW_WORKER_THREADS:-"1"}
-    gunicorn_app="promptflow.core._serving.app:create_app(extension_type='azureml')"
+    SERVING_ENGINE=${PROMPTFLOW_SERVING_ENGINE:-"flask"}
+    extra_envs=""
+    if [[ -n "${AZUREML_MODEL_DIR}" && $PROMPTFLOW_WORKER_NUM -gt 4 ]]; then
+        extra_envs="-e IDENTITY_ENDPOINT=http://localhost:8081/token -e IDENTITY_HEADER=${IDENTITY_HEADER}"
+    fi
+    gunicorn_app="promptflow.core._serving.app:create_app(extension_type='azureml',engine='${SERVING_ENGINE}')"
     echo "$(date -uIns) - Start promptflow serving with worker_num: ${WORKER_NUM}, worker_threads: ${WORKER_THREADS}, app: ${gunicorn_app}"
-    gunicorn -w ${WORKER_NUM} --threads ${WORKER_THREADS} -b "0.0.0.0:8080" --timeout 300 ${gunicorn_app}
+    if [ "$SERVING_ENGINE" = "flask" ]; then
+        gunicorn -w ${WORKER_NUM} --threads ${WORKER_THREADS} -b "0.0.0.0:8080" $extra_envs --timeout 300 ${gunicorn_app}
+    else
+        gunicorn --worker-class uvicorn.workers.UvicornWorker -w ${WORKER_NUM} -b "0.0.0.0:8080" $extra_envs --timeout 300 ${gunicorn_app}
+    fi
 else
     HOST=${HOST:-"0.0.0.0"}
     PORT=${PORT:-"8000"}
     uvicorn_app="promptflow.executor._service.app:app"
     echo "$(date -uIns) - Start promptflow python server with app: ${uvicorn_app}"
     gunicorn -k uvicorn.workers.UvicornWorker -b ${HOST}:${PORT} ${uvicorn_app}
 fi
```

## promptflow_python/package_data/scripts/auto_detect_env.sh

```diff
@@ -14,19 +14,20 @@
             export PROMPTFLOW_WORKER_NUM=$max_process
         fi
     fi
 }
 
 # check whether a model is a promptflow model
 is_pf_model() {
-    [[ -f "${1}/MLmodel" || -f "${1}/flow.dag.yaml" ]]
+    [[ -f "${1}/MLmodel" || -f "${1}/flow.dag.yaml" || -f "${1}/flow.flex.yaml" ]]
 }
 
-# auto-detect PROMPTFLOW_RUN_MODE for pf serving scenario.
+
 auto_detect_env() {
+    # auto-detect PROMPTFLOW_RUN_MODE for pf serving scenario.
     if [[ -z "${PROMPTFLOW_RUN_MODE}" ]]; then
         echo "$(date -uIns) - Detecting promptflow run mode..."
         if [[ -z "${AZUREML_MODEL_DIR}" && -z "${PROMPTFLOW_PROJECT_PATH}" ]]; then
             export PROMPTFLOW_RUN_MODE="compute"
         else
             # if PROMPTFLOW_PROJECT_PATH is set, this is a serving environment
             if [[ -z "${AZUREML_MODEL_DIR}" ]]; then
@@ -49,10 +50,21 @@
         echo "$(date -uIns) - PROMPTFLOW_RUN_MODE: ${PROMPTFLOW_RUN_MODE}"
     fi
     # only update the settings for pf serving scenario
     if [[ ${PROMPTFLOW_RUN_MODE} == "serving" ]]; then
         update_process_num
     fi
     export PROMPTFLOW_AUTO_DETECT="true"
+
+    # auto-detect AML cloud name
+    if [ -n "$AML_CloudName" ]; then
+        export AZUREML_CURRENT_CLOUD="$AML_CloudName"
+        echo "$(date -uIns) - AZUREML_CURRENT_CLOUD set to '$AZUREML_CURRENT_CLOUD'"
+    else
+        echo "$(date -uIns) - AML_CloudName is not set. Skip setting AZUREML_CURRENT_CLOUD."
+    fi
+
+    # auto-detect tracing env to prevent user from calling start_trace to start local pfs
+    export PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON="true"
 }
 
 auto_detect_env
```

## Comparing `promptflow_python_bundle-0.1.0.dist-info/METADATA` & `promptflow_python_bundle-0.2.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: promptflow-python-bundle
-Version: 0.1.0
+Version: 0.2.0
 Summary: Allow you to create your own promptflow python base images
 Author: Microsoft Corporation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: gunicorn <22.0.0,>=21.2.0
+Requires-Dist: gunicorn <23.0.0,>=22.0.0
 Requires-Dist: uvicorn <1.0.0,>=0.27.0
 Requires-Dist: promptflow-core[azureml-serving,executor-service] >=1.8.0
 
 # Promptflow python image bundle
 
 This bundle package provides a way to use your own base images to build and run promptflow-python,
 and build high-quality LLM apps with [prompt flow package](https://pypi.org/project/promptflow).
```

## Comparing `promptflow_python_bundle-0.1.0.dist-info/RECORD` & `promptflow_python_bundle-0.2.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 promptflow_python/__init__.py,sha256=JlCCObuOLZyNhIZlsoL51KtFxiY4xKIIzIRDBcdeu6Y,183
-promptflow_python/_version.py,sha256=dbv-4tfn_XlCnpA7Nq-JhvR7eXZ-8_H8Iu83qgxuVmk,19
+promptflow_python/_version.py,sha256=6q8x6xD9-0EMjrcKl3pP9jwBgEKo-lNsT4WxYOlETh4,19
 promptflow_python/start_server.py,sha256=nNvvBVAl72RmkuXY5_AzQEoEXyRJzmbcbnW8AY5bZZo,2728
 promptflow_python/package_data/runit/promptflow-python/finish,sha256=ISRFCIR8VmB3N8bODI0A_Pqy0VBRGnU241Rma3_JTxU,427
-promptflow_python/package_data/runit/promptflow-python/run,sha256=lNhAwBKQFAiATrWAA4dnQGCJ8BmuD00mOxN6PytmZ0Y,1457
-promptflow_python/package_data/scripts/auto_detect_env.sh,sha256=-jQsqpGhA4QVHDIp2JZoyOEGv1bKpQ9px7FgepT-s1A,2439
+promptflow_python/package_data/runit/promptflow-python/run,sha256=VdIjfbeEjsaQR4bRm2DiPoAcGvVlmr-eO9llfDhUSsE,1967
+promptflow_python/package_data/runit/token-provider/run,sha256=ep-Lhuh7U3s6dsRIwZNhutZ7p5fM_iX01vifDQu_F7w,935
+promptflow_python/package_data/runit/token-provider/token_provider.py,sha256=nsrt4mP4sNdw2jL7sLSYa0R83rq4Wj68m3uYV17WGcw,4262
+promptflow_python/package_data/scripts/auto_detect_env.sh,sha256=MyrCRTP4NqSnXJPfkSUKPHmxYCwGZESLbsVLx3dqny0,2936
 promptflow_python/package_data/scripts/start.sh,sha256=qB1ey7AoH6HT_Kzekc86zh8wVNV9-IJp6-UOzbMZD-c,410
-promptflow_python_bundle-0.1.0.dist-info/METADATA,sha256=P-VnYO_CkSsmlUvkK3QYi7pum3niTzK2TGHnBIGCb1E,1696
-promptflow_python_bundle-0.1.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-promptflow_python_bundle-0.1.0.dist-info/entry_points.txt,sha256=qhOktSrkr7fWPkLqezq-QrBrnJLx_-b3I9kRTEPW98Q,62
-promptflow_python_bundle-0.1.0.dist-info/top_level.txt,sha256=A7eQZn71QGS0WR12ThxwMXaYR3WV-u8zBmGwwQLuaF4,18
-promptflow_python_bundle-0.1.0.dist-info/RECORD,,
+promptflow_python_bundle-0.2.0.dist-info/METADATA,sha256=aWRTO0bJQYTh0BoLXh1pZiluZLmc4pGhDsNEiOm5W4k,1696
+promptflow_python_bundle-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+promptflow_python_bundle-0.2.0.dist-info/entry_points.txt,sha256=qhOktSrkr7fWPkLqezq-QrBrnJLx_-b3I9kRTEPW98Q,62
+promptflow_python_bundle-0.2.0.dist-info/top_level.txt,sha256=A7eQZn71QGS0WR12ThxwMXaYR3WV-u8zBmGwwQLuaF4,18
+promptflow_python_bundle-0.2.0.dist-info/RECORD,,
```

