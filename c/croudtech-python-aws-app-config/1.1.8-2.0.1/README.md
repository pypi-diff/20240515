# Comparing `tmp/croudtech-python-aws-app-config-1.1.8.tar.gz` & `tmp/croudtech_python_aws_app_config-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/croudtech-python-aws-app-config-1.1.8.tar", last modified: Tue Oct 12 12:06:06 2021, max compression
+gzip compressed data, was "croudtech_python_aws_app_config-2.0.1.tar", max compression
```

## Comparing `croudtech-python-aws-app-config-1.1.8.tar` & `croudtech_python_aws_app_config-2.0.1.tar`

### file list

```diff
@@ -1,52 +1,14 @@
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/
--rw-r--r--   0 jim       (1000) jim       (1000)      614 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.coveragerc
--rw-r--r--   0 jim       (1000) jim       (1000)      534 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.gitignore
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/.vscode/
--rw-r--r--   0 jim       (1000) jim       (1000)      115 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.vscode/settings.json
--rw-r--r--   0 jim       (1000) jim       (1000)       79 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/AUTHORS.rst
--rw-r--r--   0 jim       (1000) jim       (1000)      128 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/CHANGELOG.rst
--rw-r--r--   0 jim       (1000) jim       (1000)     1079 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/LICENSE.txt
--rw-r--r--   0 jim       (1000) jim       (1000)     7402 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)      334 2021-07-28 15:20:34.000000 croudtech-python-aws-app-config-1.1.8/Pipfile
--rw-r--r--   0 jim       (1000) jim       (1000)    21362 2021-07-28 15:20:47.000000 croudtech-python-aws-app-config-1.1.8/Pipfile.lock
--rw-r--r--   0 jim       (1000) jim       (1000)     5376 2021-07-28 10:34:33.000000 croudtech-python-aws-app-config-1.1.8/README.md
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/docs/
--rw-r--r--   0 jim       (1000) jim       (1000)     7656 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/Makefile
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/docs/_static/
--rw-r--r--   0 jim       (1000) jim       (1000)       18 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/_static/.gitignore
--rw-r--r--   0 jim       (1000) jim       (1000)       41 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/authors.rst
--rw-r--r--   0 jim       (1000) jim       (1000)       43 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/changelog.rst
--rw-r--r--   0 jim       (1000) jim       (1000)     9345 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/conf.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2325 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/index.rst
--rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/license.rst
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/nodejs/
--rw-r--r--   0 jim       (1000) jim       (1000)       20 2021-08-16 10:58:50.000000 croudtech-python-aws-app-config-1.1.8/nodejs/.gitignore
--rw-r--r--   0 jim       (1000) jim       (1000)    30752 2021-08-16 11:02:06.000000 croudtech-python-aws-app-config-1.1.8/nodejs/package-lock.json
--rw-r--r--   0 jim       (1000) jim       (1000)      886 2021-08-16 11:02:05.000000 croudtech-python-aws-app-config-1.1.8/nodejs/package.json
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/nodejs/src/
--rw-r--r--   0 jim       (1000) jim       (1000)     1933 2021-08-16 10:13:19.000000 croudtech-python-aws-app-config-1.1.8/nodejs/src/index.ts
--rw-r--r--   0 jim       (1000) jim       (1000)      226 2021-08-13 13:18:11.000000 croudtech-python-aws-app-config-1.1.8/nodejs/tsconfig.json
--rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/pytest.ini
--rw-r--r--   0 jim       (1000) jim       (1000)      332 2021-04-26 18:47:32.000000 croudtech-python-aws-app-config-1.1.8/requirements.txt
--rw-r--r--   0 jim       (1000) jim       (1000)     1297 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/setup.cfg
--rw-r--r--   0 jim       (1000) jim       (1000)      933 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/setup.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/src/
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/
--rw-r--r--   0 jim       (1000) jim       (1000)      388 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/__init__.py
--rw-r--r--   0 jim       (1000) jim       (1000)     6549 2021-10-12 12:01:52.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/cli.py
--rw-r--r--   0 jim       (1000) jim       (1000)      804 2021-08-11 11:10:04.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/metrics.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2895 2021-08-18 10:20:00.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/redis_config.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2010 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/response.py
--rw-r--r--   0 jim       (1000) jim       (1000)    13418 2021-10-12 12:04:29.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/ssm_config.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/
--rw-r--r--   0 jim       (1000) jim       (1000)        0 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/__init__.py
--rw-r--r--   0 jim       (1000) jim       (1000)      252 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/conftest.py
--rw-r--r--   0 jim       (1000) jim       (1000)      931 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/redis_config_test.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/
--rw-r--r--   0 jim       (1000) jim       (1000)     7402 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)     1256 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       82 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/entry_points.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/not-zip-safe
--rw-r--r--   0 jim       (1000) jim       (1000)      295 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/requires.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       32 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/top_level.txt
+-rw-r--r--   0        0        0       79 2021-04-22 10:05:38.190000 croudtech_python_aws_app_config-2.0.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1079 2021-04-22 10:05:38.190000 croudtech_python_aws_app_config-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     7362 2021-12-10 12:23:48.556187 croudtech_python_aws_app_config-2.0.1/README.md
+-rw-r--r--   0        0        0      581 2024-05-15 14:25:50.583326 croudtech_python_aws_app_config-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-05-15 14:17:47.683629 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/__init__.py
+-rw-r--r--   0        0        0    11062 2021-12-10 12:18:23.686189 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/cli.py
+-rw-r--r--   0        0        0      804 2021-08-11 11:10:04.410611 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/metrics.py
+-rw-r--r--   0        0        0     3382 2021-12-10 11:41:22.826198 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/redis_config.py
+-rw-r--r--   0        0        0     2010 2021-07-28 15:20:56.246621 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/response.py
+-rw-r--r--   0        0        0    14638 2024-05-15 14:18:56.333598 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/ssm_config.py
+-rw-r--r--   0        0        0        0 2021-04-22 10:05:38.350000 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/tests/__init__.py
+-rw-r--r--   0        0        0      252 2021-04-22 10:05:38.350000 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/tests/conftest.py
+-rw-r--r--   0        0        0      931 2021-07-28 15:20:56.216621 croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/tests/redis_config_test.py
+-rw-r--r--   0        0        0     8040 1970-01-01 00:00:00.000000 croudtech_python_aws_app_config-2.0.1/PKG-INFO
```

### Comparing `croudtech-python-aws-app-config-1.1.8/LICENSE.txt` & `croudtech_python_aws_app_config-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/PKG-INFO` & `croudtech_python_aws_app_config-2.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,207 +1,281 @@
 Metadata-Version: 2.1
 Name: croudtech-python-aws-app-config
-Version: 1.1.8
-Summary: Applicaton config via AWS SSM
-Home-page: https://github.com/CroudTech/croudtech-python-aws-app-config
+Version: 2.0.1
+Summary: 
 Author: Jim Robinson
-Author-email: jscrobinson@gmail.com
-License: mit
-Description: # croudtech-python-aws-app-config
-        
-        croudtech-python-aws-app-config us a utility to help manage application config using the AWS SSM Parameter Store
-        
-        There is a cli tool to help set the values and a utility to use the SSM parameters within you application.
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install croudtech-python-aws-app-config.
-        
-        ```bash
-        pip install croudtech-python-aws-app-config
-        ```
-        
-        ## Command Line Usage
-        
-        ```
-        Usage: cli.py [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --debug / --no-debug
-          --endpoint-url TEXT
-          --help                Show this message and exit.
-        
-        Commands:
-          delete-parameters
-          get-arns
-          get-parameters
-          put-parameters
-          put-parameters-recursive
-        ```
-        
-        --endpoint-url specified the AWS API endpoint URL used. This should be used if using localstack or a similar aws mock service. You can also set the `AWS_ENDPOINT_URL` env var to enable this feature.
-        
-        ### Sub Commands
-        
-        #### delete-parameters
-        
-        Delete parameters from SSM for a specified app and environment
-        
-        ```
-        Usage: cli.py delete-parameters [OPTIONS]
-        
-        Options:
-          --environment-name TEXT  The environment name  [required]
-          --app-name TEXT          The app name  [required]
-          --ssm-prefix TEXT        The ssm path prefix
-          --region TEXT            The AWS region
-          --help                   Show this message and exit.
-        ```
-        
-        #### get-arns
-        
-        Get ARNs for published parameters
-        
-        ```
-        Usage: cli.py get-arns [OPTIONS]
-        
-        Options:
-          --environment-name TEXT         The environment name  [required]
-          --app-name TEXT                 The app name  [required]
-          --ssm-prefix TEXT               The ssm path prefix
-          --region TEXT                   The AWS region
-          --include-common / --ignore-common
-                                          Include shared variables
-          --output-format [ecs]
-          --help                          Show this message and exit.
-        ```
-        
-        #### get-parameters
-        
-        Get parameters for a specific app and environment
-        
-        ```
-        Usage: cli.py get-parameters [OPTIONS]
-        
-        Options:
-          --environment-name TEXT         The environment name  [required]
-          --app-name TEXT                 The app name  [required]
-          --ssm-prefix TEXT               The ssm path prefix
-          --region TEXT                   The AWS region
-          --include-common / --ignore-common
-                                          Include shared variables
-          --output-format [json|yaml|environment|environment-export]
-          --help                          Show this message and exit.
-        ```
-        
-        You can export the variables to your local shell by using
-        
-        ```
-        eval $(croudtech-app-config get-parameters --app-name myapp --environment-name myenv --output-format environment-export)
-        ```
-        #### put-parameters
-        
-        INPUT should be the path to a yaml or json file
-        
-        ```
-        Usage: cli.py put-parameters [OPTIONS] INPUT
-        
-        Options:
-          --environment-name TEXT  The environment name  [required]
-          --app-name TEXT          The app name  [required]
-          --ssm-prefix TEXT        The ssm path prefix
-          --region TEXT            The AWS region
-          --encrypted TEXT         Do you want these parameters to be encrypted?
-          --delete-first           Delete the values in this path before pushing
-                                   (useful for cleanup)
-        
-          --help                   Show this message and exit.
-        ```
-        
-        #### put-parameters-recursive
-        
-        Recursively put parameters from a directory with the following structure
-        
-        ```
-        ├── EnvironmentName1
-        │   ├── AppName1.yaml
-        │   ├── AppName1.secret.yaml
-        │   ├── AppName2.yaml
-        │   └──AppName2.secret.yaml
-        └── EnvironmentName2
-            ├── AppName1.yaml
-            ├── AppName1.secret.yaml
-            ├── AppName2.yaml
-            └──AppName2.secret.yaml
-        ```
-        
-        Files with a *secret.yaml* or *secret.json* suffix will have the parameters encrypted in SSM.
-        
-        ```
-        Usage: cli.py put-parameters-recursive [OPTIONS] VALUES_PATH
-        
-        Options:
-          --ssm-prefix TEXT  The ssm path prefix
-          --region TEXT      The AWS region
-          --delete-first     Delete the values in this path before pushing (useful for
-                             cleanup)
-        
-          --help             Show this message and exit.
-        ```
-        
-        ## Nested file structure and environment variables
-        
-        Nested values will have their keys flattened when being converted to environment variables. This allows for a simpler structure than just adding all your env vars separately.
-        
-        For example:
-        
-        ```
-        SOME_VARIABLE: test
-        ANOTHER_VAR: 123
-        SOME_OTHER_VAR: foo
-        CONNECTIONS:
-          POSTGRESS:
-            HOST: somehost
-            PORT: 1234
-            USERNAME: someuser
-            PASSWORD: somepass
-        ```
-        
-        Would translate into the following environment variables:
-        
-        ```
-        SOME_VARIABLE="test"
-        ANOTHER_VAR="123"
-        SOME_OTHER_VAR="foo"
-        CONNECTIONS_POSTGRESS_HOST="somehost"
-        CONNECTIONS_POSTGRESS_PORT="1234"
-        CONNECTIONS_POSTGRESS_USERNAME="someuser"
-        CONNECTIONS_POSTGRESS_PASSWORD="somepass"
-        ```
-        
-        ## Usage in application code
-        
-        In the top of your application bootstrap file (or settings.py in django) add:
-        
-        ```
-        from croudtech_python_aws_app_config.ssm_config import SsmConfig
-        
-        ssm_config = SsmConfig(
-            environment_name=os.environ.get("ENVIRONMENT_NAME"), app_name=os.environ.get("APP_NAME")
-        )
-        ssm_config.params_to_env()
-        ```
-        
-        Make sure your ENVIRONMENT_NAME and APP_NAME env vars are set.
-        
-        This will pull values from SSM and inject them into your application environment variables.
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        
-        
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown; charset=UTF-8
+Author-email: jim.robinson@croud.com
+Requires-Python: >=3.12,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: boto3 (>=1.34.105,<2.0.0)
+Requires-Dist: bson (>=0.5.10,<0.6.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: http-status-codes (>=1.0.3,<2.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: pyaml (>=24.4.0,<25.0.0)
+Requires-Dist: redis (>=5.0.4,<6.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Description-Content-Type: text/markdown
+
+# croudtech-python-aws-app-config
+
+croudtech-python-aws-app-config us a utility to help manage application config using the AWS SSM Parameter Store
+
+There is a cli tool to help set the values and a utility to use the SSM parameters within you application.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install croudtech-python-aws-app-config.
+
+```bash
+pip install croudtech-python-aws-app-config
+```
+
+## Command Line Usage
+
+```
+Usage: cli.py [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --debug / --no-debug
+  --endpoint-url TEXT
+  --help                Show this message and exit.
+
+Commands:
+  delete-parameters
+  get-arns
+  get-parameters
+  put-parameters
+  put-parameters-recursive
+  manage-redis
+```
+
+--endpoint-url specified the AWS API endpoint URL used. This should be used if using localstack or a similar aws mock service. You can also set the `AWS_ENDPOINT_URL` env var to enable this feature.
+
+### Sub Commands
+
+#### delete-parameters
+
+Delete parameters from SSM for a specified app and environment
+
+```
+Usage: cli.py delete-parameters [OPTIONS]
+
+Options:
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The app name  [required]
+  --ssm-prefix TEXT        The ssm path prefix
+  --region TEXT            The AWS region
+  --help                   Show this message and exit.
+```
+
+#### get-arns
+
+Get ARNs for published parameters
+
+```
+Usage: cli.py get-arns [OPTIONS]
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --output-format [ecs]
+  --help                          Show this message and exit.
+```
+
+#### get-parameters
+
+Get parameters for a specific app and environment
+
+```
+Usage: cli.py get-parameters [OPTIONS]
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --output-format [json|yaml|environment|environment-export]
+  --help                          Show this message and exit.
+```
+
+You can export the variables to your local shell by using
+
+```
+eval $(croudtech-app-config get-parameters --app-name myapp --environment-name myenv --output-format environment-export)
+```
+#### put-parameters
+
+INPUT should be the path to a yaml or json file
+
+```
+Usage: cli.py put-parameters [OPTIONS] INPUT
+
+Options:
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The app name  [required]
+  --ssm-prefix TEXT        The ssm path prefix
+  --region TEXT            The AWS region
+  --encrypted TEXT         Do you want these parameters to be encrypted?
+  --delete-first           Delete the values in this path before pushing
+                           (useful for cleanup)
+
+  --help                   Show this message and exit.
+```
+
+#### put-parameters-recursive
+
+Recursively put parameters from a directory with the following structure
+
+```
+├── EnvironmentName1
+│   ├── AppName1.yaml
+│   ├── AppName1.secret.yaml
+│   ├── AppName2.yaml
+│   └──AppName2.secret.yaml
+└── EnvironmentName2
+    ├── AppName1.yaml
+    ├── AppName1.secret.yaml
+    ├── AppName2.yaml
+    └──AppName2.secret.yaml
+```
+
+Files with a *secret.yaml* or *secret.json* suffix will have the parameters encrypted in SSM.
+
+```
+Usage: cli.py put-parameters-recursive [OPTIONS] VALUES_PATH
+
+Options:
+  --ssm-prefix TEXT  The ssm path prefix
+  --region TEXT      The AWS region
+  --delete-first     Delete the values in this path before pushing (useful for
+                     cleanup)
+
+  --help             Show this message and exit.
+```
+
+## Managing Redis DB Allocation
+
+Manage redis DB allocation
+
+### Sub commands
+
+#### allocate-db
+
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis allocate-db
+           [OPTIONS]
+
+  Allocate a Redis database for a specified application and environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+
+#### deallocate-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis deallocate-db
+           [OPTIONS]
+
+  Remove Redis database allocation for the specified application and
+  environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+#### show-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-db
+           [OPTIONS]
+
+  Show Allocated Redis Database for a specified application
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --help                          Show this message and exit.
+```
+#### show-dbs
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-dbs
+           [OPTIONS]
+
+  Show all allocated Redis databases
+
+Options:
+  --redis-host TEXT     The redis host  [required]
+  --redis-port INTEGER  The redis port  [required]
+  --help                Show this message and exit.
+```
+
+## Nested file structure and environment variables
+
+Nested values will have their keys flattened when being converted to environment variables. This allows for a simpler structure than just adding all your env vars separately.
+
+For example:
+
+```
+SOME_VARIABLE: test
+ANOTHER_VAR: 123
+SOME_OTHER_VAR: foo
+CONNECTIONS:
+  POSTGRESS:
+    HOST: somehost
+    PORT: 1234
+    USERNAME: someuser
+    PASSWORD: somepass
+```
+
+Would translate into the following environment variables:
+
+```
+SOME_VARIABLE="test"
+ANOTHER_VAR="123"
+SOME_OTHER_VAR="foo"
+CONNECTIONS_POSTGRESS_HOST="somehost"
+CONNECTIONS_POSTGRESS_PORT="1234"
+CONNECTIONS_POSTGRESS_USERNAME="someuser"
+CONNECTIONS_POSTGRESS_PASSWORD="somepass"
+```
+
+## Usage in application code
+
+In the top of your application bootstrap file (or settings.py in django) add:
+
+```
+from croudtech_python_aws_app_config.ssm_config import SsmConfig
+
+ssm_config = SsmConfig(
+    environment_name=os.environ.get("ENVIRONMENT_NAME"), app_name=os.environ.get("APP_NAME")
+)
+ssm_config.params_to_env()
+```
+
+Make sure your ENVIRONMENT_NAME and APP_NAME env vars are set.
+
+This will pull values from SSM and inject them into your application environment variables.
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+
+
```

### Comparing `croudtech-python-aws-app-config-1.1.8/README.md` & `croudtech_python_aws_app_config-2.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 Commands:
   delete-parameters
   get-arns
   get-parameters
   put-parameters
   put-parameters-recursive
+  manage-redis
 ```
 
 --endpoint-url specified the AWS API endpoint URL used. This should be used if using localstack or a similar aws mock service. You can also set the `AWS_ENDPOINT_URL` env var to enable this feature.
 
 ### Sub Commands
 
 #### delete-parameters
@@ -136,14 +137,80 @@
   --region TEXT      The AWS region
   --delete-first     Delete the values in this path before pushing (useful for
                      cleanup)
 
   --help             Show this message and exit.
 ```
 
+## Managing Redis DB Allocation
+
+Manage redis DB allocation
+
+### Sub commands
+
+#### allocate-db
+
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis allocate-db
+           [OPTIONS]
+
+  Allocate a Redis database for a specified application and environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+
+#### deallocate-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis deallocate-db
+           [OPTIONS]
+
+  Remove Redis database allocation for the specified application and
+  environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+#### show-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-db
+           [OPTIONS]
+
+  Show Allocated Redis Database for a specified application
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --help                          Show this message and exit.
+```
+#### show-dbs
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-dbs
+           [OPTIONS]
+
+  Show all allocated Redis databases
+
+Options:
+  --redis-host TEXT     The redis host  [required]
+  --redis-port INTEGER  The redis port  [required]
+  --help                Show this message and exit.
+```
+
 ## Nested file structure and environment variables
 
 Nested values will have their keys flattened when being converted to environment variables. This allows for a simpler structure than just adding all your env vars separately.
 
 For example:
 
 ```
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/metrics.py` & `croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/metrics.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/redis_config.py` & `croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/redis_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,20 +41,22 @@
     def redis_db_allocations(self):
         return json.loads(self.redis_config.get(self._allocated_dbs_key))
 
     @property
     def db_key(self):
         return "%s_%s" % (self._environment, self._app_name)
 
-    def get_redis_database(self):
+    def get_redis_database(self, allocate=False):
         allocated_dbs = self.redis_db_allocations
-        if self.db_key not in allocated_dbs:
+        if self.db_key not in allocated_dbs and allocate:
             allocated_db = self.allocate_db()
-        else:
+        elif self.db_key in allocated_dbs:
             allocated_db = allocated_dbs[self.db_key]
+        else:
+            allocated_db = None
         if self.put_metrics:
             self.metrics.put_redis_db_metric(
                 app_key=self.db_key,
                 redis_db=allocated_db,
                 redis_host=self._redis_host,
                 environment_name=self._environment,
             )
@@ -65,14 +67,25 @@
         db = unused_dbs[0]
         db_config = self.redis_db_allocations
         db_config[self.db_key] = db
         self._redis_config.set(self._allocated_dbs_key, json.dumps(db_config))
 
         return db
 
+    def deallocate_db(self):
+        unused_dbs = self.get_unused_dbs()        
+        db_config = self.redis_db_allocations
+        if self.db_key in db_config:
+            db = db_config[self.db_key]
+            del(db_config[self.db_key])
+            self._redis_config.set(self._allocated_dbs_key, json.dumps(db_config))
+
+            return True, db
+        return False, None
+
     def get_redis_allocated_db(self, db):
         if db not in self._redis_dbs:
             self._redis_dbs[db] = redis.Redis(
                 host=self._redis_host, port=self._redis_port, db=db
             )
         return self._redis_dbs[db]
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/response.py` & `croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/response.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/ssm_config.py` & `croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/ssm_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import boto3
 import json
 import os
 from botocore import endpoint
 import yaml
-from collections import MutableMapping
+from collections.abc import MutableMapping
 import logging
 import re
 from click._compat import open_stream
 import click
 import botocore
 import sys
 from .redis_config import RedisConfig
@@ -91,44 +91,56 @@
     def get_parameters(self):
         if self.include_common:
             parameters = self.fetch_parameters(self.common_ssm_path)
         else:
             parameters = {}
 
         parameters = {**parameters, **self.fetch_parameters(self.ssm_path)}
-        try:
-            parameters = self.parse_parameters(parameters)
-        except:
-            pass
+        parameters = self.parse_parameters(parameters)
         return parameters
 
     def parse_parameters(self, parameters):
-        if self.parse_redis and ("/REDIS_DB" not in parameters or parameters["/REDIS_DB"] == "auto"):
+        if self.parse_redis:
+            redis_db, redis_host, redis_port = self.find_redis_config(parameters, allocate=True)
+            if redis_db:
+                parameters["/REDIS_DB"] = redis_db
+                parameters["/REDIS_URL"] = "redis://%s:%s/%s" % (
+                    redis_host,
+                    redis_port,
+                    redis_db,
+                )
+            else:
+                raise Exception("Couldn't allocate Redis Database")
+        return parameters
+
+    def get_redis_db(self):
+        parameters = self.get_parameters()
+        redis_db, redis_host, redis_port = self.find_redis_config(parameters)
+        return redis_db, redis_host, redis_port
+
+    def find_redis_config(self, parameters, allocate=False):
+        if "/REDIS_DB" not in parameters or parameters["/REDIS_DB"] == "auto":
             redis_host = (
                 parameters["/REDIS_HOST"] if "/REDIS_HOST" in parameters else False
             )
             redis_port = (
                 parameters["/REDIS_PORT"] if "/REDIS_PORT" in parameters else 6379
             )
+
             if redis_host:
                 redis_config_instance = RedisConfig(
                     redis_host=redis_host,
                     redis_port=redis_port,
                     app_name=self.app_name,
                     environment=self.environment_name,
                     put_metrics=self.put_metrics,
                 )
-                redis_db = redis_config_instance.get_redis_database()
-                parameters["/REDIS_DB"] = redis_db
-                parameters["/REDIS_URL"] = "redis://%s:%s/%s" % (
-                    redis_host,
-                    redis_port,
-                    redis_db,
-                )
-        return parameters
+                redis_db = redis_config_instance.get_redis_database(allocate)
+                return redis_db, redis_host, redis_port
+        return None, None, None
 
     @property
     def current_parameters(self):
         if not hasattr(self, "_current_parameters"):
             self._current_parameters = self.fetch_parameters(
                 path=self.ssm_path, absolute_path=True
             )
@@ -200,23 +212,39 @@
     def parse_value(self, value):
         try:
             parsed_value = json.dumps(json.loads(value))
         except:
             parsed_value = value
         return str(parsed_value).strip()
 
+    def parse_fetched_parameter(self, parameter):
+        value = parameter['Value']
+        if value.startswith('ssm:'):
+            valueParameterName = value.replace('ssm:', '')
+            encrypted = False
+            if valueParameterName.startswith('encrypted:'):
+                valueParameterName = valueParameterName.replace('encrypted:')
+                encrypted = True
+            parameterresponse = self.ssm_client.get_parameter(
+                Name = valueParameterName,
+                WithDecryption = encrypted
+            )
+            value = parameterresponse['Parameter']['Value']
+        return value
+
     def fetch_parameters(self, path, absolute_path=False):
         try:
             parameters = {}
             for parameter in self.fetch_paginated_parameters(path):
                 if absolute_path:
                     parameter_name = parameter["Name"]
                 else:
                     parameter_name = parameter["Name"].replace(path, "")
-                parameters[parameter_name] = parameter["Value"]            
+                parameter_value = self.parse_fetched_parameter(parameter)
+                parameters[parameter_name] = parameter_value
         except botocore.exceptions.ClientError as err:
             logger.debug("Failed to fetch parameters. Invalid token")
             return {}
         except botocore.exceptions.NoCredentialsError as err:
             logger.debug("Failed to fetch parameters. Could not find AWS credentials")
             return {}
         return parameters
@@ -225,19 +253,19 @@
         if not hasattr(self, "fetched_parameters"):
             self.fetched_parameters = {}
         if path not in self.fetched_parameters:
             paginator = self.ssm_client.get_paginator('get_parameters_by_path')
             parameters = paginator.paginate(
                 Path=path,
                 Recursive=True,
-                WithDecryption=True,    
+                WithDecryption=True,
             )
-            
+
             self.fetched_parameters["path"] = parameters.build_full_result()["Parameters"]
-            
+
             for item in self.fetched_parameters["path"]:
                 logger.debug("Found Parameter %s." % item["Name"])
             logger.debug("Fetched parameters from AWS SSM for path %s." % path)
         return self.fetched_parameters["path"]
 
     def parameter_name_to_underscore(self, name):
         return name[1 : len(name)].replace("/", "_")
@@ -317,14 +345,15 @@
         elif file_extension == ".json":
             data = json.loads(contents)
         else:
             raise Exception("File format is not valid")
 
         flattened = convert_flatten(data, sep="/", parent_key=self.ssm_path)
         if delete_first:
+            self.parse_redis = False
             self.delete_existing()
 
         for key, value in flattened.items():
             self.put_parameter(
                 path=key, is_abs_path=True, value=value, encrypted=encrypted
             )
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/redis_config_test.py` & `croudtech_python_aws_app_config-2.0.1/src/croudtech_python_aws_app_config/tests/redis_config_test.py`

 * *Files identical despite different names*

