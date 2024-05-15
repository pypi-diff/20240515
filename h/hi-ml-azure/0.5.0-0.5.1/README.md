# Comparing `tmp/hi-ml-azure-0.5.0.tar.gz` & `tmp/hi-ml-azure-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-azure-0.5.0.tar", last modified: Tue Mar 19 14:00:51 2024, max compression
+gzip compressed data, was "hi-ml-azure-0.5.1.tar", last modified: Wed May 15 13:24:13 2024, max compression
```

## Comparing `hi-ml-azure-0.5.0.tar` & `hi-ml-azure-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/package_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:51.002386 hi-ml-azure-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/src/health_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/amulet.py
--rw-r--r--   0 runner    (1001) docker     (127)    20546 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/argparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    28568 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/src/health_azure/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/examples/elevate_this.py
--rw-r--r--   0 runner    (1001) docker     (127)    62278 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/himl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/himl_download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5604 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/himl_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/mlflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/package_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    91509 2024-03-19 14:00:31.000000 hi-ml-azure-0.5.0/src/health_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:51.006386 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 14:00:50.000000 hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:13.191679 hi-ml-azure-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/src/health_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/amulet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20546 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28568 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/src/health_azure/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/examples/elevate_this.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62979 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/himl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/himl_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5604 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/himl_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/mlflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91509 2024-05-15 13:24:02.000000 hi-ml-azure-0.5.1/src/health_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:13.195679 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 13:24:13.000000 hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/top_level.txt
```

### Comparing `hi-ml-azure-0.5.0/LICENSE` & `hi-ml-azure-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/PKG-INFO` & `hi-ml-azure-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.5.0
+Version: 0.5.1
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-azure-0.5.0/package_description.md` & `hi-ml-azure-0.5.1/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/setup.py` & `hi-ml-azure-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/__init__.py` & `hi-ml-azure-0.5.1/src/health_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/amulet.py` & `hi-ml-azure-0.5.1/src/health_azure/amulet.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/argparsing.py` & `hi-ml-azure-0.5.1/src/health_azure/argparsing.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/auth.py` & `hi-ml-azure-0.5.1/src/health_azure/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 logger = logging.getLogger(__name__)
 
 # Environment variables used for authentication
 ENV_SERVICE_PRINCIPAL_ID = "HIML_SERVICE_PRINCIPAL_ID"
 ENV_SERVICE_PRINCIPAL_PASSWORD = "HIML_SERVICE_PRINCIPAL_PASSWORD"
 ENV_TENANT_ID = "HIML_TENANT_ID"
 
+# This is an environment variable that is set by GitHub Actions, for checking if the code is running in GitHub
+ENV_GITHUB_ACTIONS = "GITHUB_ACTIONS"
+
+# The scope for the access tokens that are requested from Azure
+ACCESS_TOKEN_SCOPE = "https://management.azure.com/.default"
+
 
 def get_secret_from_environment(name: str, allow_missing: bool = False) -> Optional[str]:
     """
     Gets a password or key from the secrets file or environment variables.
 
     :param name: The name of the environment variable to read. It will be converted to uppercase.
     :param allow_missing: If true, the function returns None if there is no entry of the given name in any of the
@@ -65,19 +71,25 @@
             tenant_id=tenant_id,
             service_principal_id=service_principal_id,
             service_principal_password=service_principal_password,
         )
     try:
         logger.debug("Trying to authenticate using Azure CLI")
         auth = AzureCliAuthentication()
-        _ = auth.get_token()
+        _ = auth.get_token(ACCESS_TOKEN_SCOPE)
         logger.info("Successfully started AzureCLI authentication.")
         return auth
-    except AuthenticationException:
-        pass
+    except AuthenticationException as ex:
+        # If the code is running in GitHub, there is no point in even trying to authenticate interactively.
+        # Raise the exception to get some information about the authentication problem.
+        # Otherwise, try to authenticate interactively.
+        # The GITHUB_ACTIONS environment variable is meant to be used exactly for this check
+        # https://docs.github.com/en/actions/learn-github-actions/variables
+        if os.getenv(ENV_GITHUB_ACTIONS, "") == "true":
+            raise AuthenticationException("AzureCLI authentication must be set up when running in GitHub") from ex
 
     logger.info(
         "Using interactive login to Azure. To use Service Principal authentication, set the environment "
         f"variables {ENV_SERVICE_PRINCIPAL_ID}, {ENV_SERVICE_PRINCIPAL_PASSWORD}, and {ENV_TENANT_ID}. "
         "For Azure CLI authentication, log in using 'az login' and ensure that the subscription is set."
     )
     return InteractiveLoginAuthentication()
@@ -86,15 +98,15 @@
 def _validate_credential(credential: TokenCredential) -> None:
     """
     Validate credential by attempting to get token. If authentication has been successful, get_token
     will succeed. Otherwise an exception will be raised
 
     :param credential: The credential object to validate.
     """
-    credential.get_token("https://management.azure.com/.default")
+    credential.get_token(ACCESS_TOKEN_SCOPE)
 
 
 def _get_legitimate_service_principal_credential(
     tenant_id: str, service_principal_id: str, service_principal_password: str
 ) -> TokenCredential:
     """
     Create a ClientSecretCredential given a tenant id, service principal id and password
```

### Comparing `hi-ml-azure-0.5.0/src/health_azure/datasets.py` & `hi-ml-azure-0.5.1/src/health_azure/datasets.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/examples/elevate_this.py` & `hi-ml-azure-0.5.1/src/health_azure/examples/elevate_this.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/himl.py` & `hi-ml-azure-0.5.1/src/health_azure/himl.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,15 @@
     wait_for_completion: bool = False,
     identity_based_auth: bool = False,
     hyperparam_args: Optional[Dict[str, Any]] = None,
     num_nodes: int = 1,
     pytorch_processes_per_node: Optional[int] = None,
     use_mpi_run_for_single_node_jobs: bool = True,
     display_name: Optional[str] = None,
+    hyperdrive_argument_prefix: str = "--",
 ) -> Job:
     """
     Starts a v2 AML Job on a given workspace by submitting a command
 
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
     :param environment: An AML v2 Environment object.
     :param entry_script: The Python script that should be run in AzureML. If None, the current main Python file will be
@@ -448,14 +449,17 @@
     :param pytorch_processes_per_node: For plain PyTorch multi-GPU processing: The number of processes per node.
         If supplied, it will run a command job with the "pytorch" framework (rather than "Python"), and using "nccl"
         as the communication backend.
     :param use_mpi_run_for_single_node_jobs: If True, even single node jobs will be run as distributed MPI jobs.
         This is required for Kubernetes compute. If False, single node jobs will not be run as distributed jobs.
     :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
         display name will be generated by AzureML.
+    :param: hyperdrive_argument_prefix: Prefix to add to hyperparameter arguments. Some examples might be "--", "-"
+        or "". For example, if "+" is used, a hyperparameter "learning_rate" with value 0.01 will be passed as
+        `+learning_rate=0.01`.
     :return: An AzureML Run object.
     """
     root_dir = sanitize_snapshoot_directory(snapshot_root_directory)
     script_params = script_params or []
     script_param_str = create_v2_job_command_line_args_from_params(script_params)
     if entry_command is None:
         entry_script_relative = sanitize_entry_script(entry_script, root_dir)
@@ -508,15 +512,15 @@
         param_sampling = hyperparam_args[PARAM_SAMPLING_ARG]
 
         if input_datasets_v2 is None:
             input_datasets_v2 = {}
 
         for sample_param, choices in param_sampling.items():
             input_datasets_v2[sample_param] = choices.values[0]
-            cmd += f" --{sample_param}=" + "${{inputs." + sample_param + "}}"
+            cmd += f" {hyperdrive_argument_prefix}{sample_param}=" + "${{inputs." + sample_param + "}}"
 
         command_job = create_command_job(cmd)
 
         del hyperparam_args[PARAM_SAMPLING_ARG]
         # override command with parameter expressions
         command_job = command_job(
             **param_sampling,
@@ -740,14 +744,15 @@
     hyperparam_args: Optional[Dict[str, Any]] = None,
     strictly_aml_v1: bool = False,
     identity_based_auth: bool = False,
     pytorch_processes_per_node_v2: Optional[int] = None,
     use_mpi_run_for_single_node_jobs: bool = False,
     display_name: Optional[str] = None,
     entry_command: Optional[PathOrString] = None,
+    hyperdrive_argument_prefix: str = "--",
 ) -> AzureRunInfo:  # pragma: no cover
     """
     Submit a folder to Azure, if needed and run it.
     Use the commandline flag --azureml to submit to AzureML, and leave it out to run locally.
 
     :param after_submission: A function that will be called directly after submitting the job to AzureML.
         Use this to, for example, add additional tags or print information about the run.
@@ -815,14 +820,17 @@
         is only supported with AML SDK v2, and ignored in v1. If supplied, the job will be submitted as using the
         "pytorch" framework (rather than "Python"), and using "nccl" as the communication backend.
     :param use_mpi_run_for_single_node_jobs: If True, even single node jobs will be run as distributed MPI
         jobs. If False, single node jobs will not be run as distributed jobs.
         Setting this flag to True is required Kubernetes compute.
     :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
         display name will be generated by AzureML.
+    :param: hyperdrive_argument_prefix: Prefix to add to hyperparameter arguments. Some examples might be "--", "-"
+        or "". For example, if "+" is used, a hyperparameter "learning_rate" with value 0.01 will be passed as
+        `+learning_rate=0.01`.
     :return: If the script is submitted to AzureML then we terminate python as the script should be executed in AzureML,
         otherwise we return a AzureRunInfo object.
     """
     health_azure_package_setup()
     workspace_config_path = _str_to_path(workspace_config_file)
     snapshot_root_directory = _str_to_path(snapshot_root_directory)
     cleaned_input_datasets = _replace_string_datasets(input_datasets or [], default_datastore_name=default_datastore)
@@ -982,14 +990,15 @@
                 docker_shm_size=docker_shm_size,
                 wait_for_completion=wait_for_completion,
                 identity_based_auth=identity_based_auth,
                 hyperparam_args=hyperparam_args,
                 num_nodes=num_nodes,
                 pytorch_processes_per_node=pytorch_processes_per_node_v2,
                 use_mpi_run_for_single_node_jobs=use_mpi_run_for_single_node_jobs,
+                hyperdrive_argument_prefix=hyperdrive_argument_prefix,
             )
 
             if after_submission is not None:
                 after_submission(job, ml_client)  # type: ignore
 
     exit(0)
```

### Comparing `hi-ml-azure-0.5.0/src/health_azure/himl_download.py` & `hi-ml-azure-0.5.1/src/health_azure/himl_download.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/himl_tensorboard.py` & `hi-ml-azure-0.5.1/src/health_azure/himl_tensorboard.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/logging.py` & `hi-ml-azure-0.5.1/src/health_azure/logging.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/mlflow_utils.py` & `hi-ml-azure-0.5.1/src/health_azure/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/package_setup.py` & `hi-ml-azure-0.5.1/src/health_azure/package_setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/paths.py` & `hi-ml-azure-0.5.1/src/health_azure/paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/traverse.py` & `hi-ml-azure-0.5.1/src/health_azure/traverse.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/health_azure/utils.py` & `hi-ml-azure-0.5.1/src/health_azure/utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/PKG-INFO` & `hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.5.0
+Version: 0.5.1
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-azure-0.5.0/src/hi_ml_azure.egg-info/SOURCES.txt` & `hi-ml-azure-0.5.1/src/hi_ml_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

