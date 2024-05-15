# Comparing `tmp/dlc_run-0.0.3.tar.gz` & `tmp/dlc_run-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlc_run-0.0.3.tar", last modified: Fri May 10 09:27:26 2024, max compression
+gzip compressed data, was "dist/dlc_run-0.0.4.tar", last modified: Wed May 15 04:06:27 2024, max compression
```

## Comparing `dlc_run-0.0.3.tar` & `dlc_run-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 09:27:26.000000 dlc_run-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 09:27:20.000000 dlc_run-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/dlc_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-10 09:27:20.000000 dlc_run-0.0.3/dlc_run/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 09:27:26.000000 dlc_run-0.0.3/dlc_run.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:27:26.000000 dlc_run-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 09:27:20.000000 dlc_run-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 04:06:27.000000 dlc_run-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 04:06:25.000000 dlc_run-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/dlc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:06:27.000000 dlc_run-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-15 04:06:25.000000 dlc_run-0.0.4/setup.py
```

### Comparing `dlc_run-0.0.3/dlc_run/dlc_run.py` & `dlc_run-0.0.4/dlc_run/dlc_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import argparse
 import os
 import re
 import subprocess
 from pathlib import Path
 
-HOME = f'/cpfs01/user/{os.getenv("USER")}'
-
-
-def get_workspace_id(partition: str, config_path: str, dlc_path: str) -> str:
-    """Extract the workspace ID for the specified partition using dlc
-    command."""
-    config_path = os.path.expanduser(config_path)
-    dlc_path = os.path.expanduser(dlc_path)
-    try:
-        result = subprocess.run(
-            [dlc_path, 'get', 'workspace', '-c', config_path],
-            capture_output=True,
-            text=True,
-            check=True)
-        regex = rf'\|\s*{re.escape(partition)}\s*\|\s*([\w]+)\s*\|'
-        match = re.search(regex, result.stdout, re.MULTILINE)
-        if match:
-            return match.group(1).strip()
-    except subprocess.SubprocessError as e:
-        print(f'Error retrieving workspace ID: {e}')
-        return None
-    return None
+user_names = os.listdir('/cpfs01/user/')
+if len(user_names) == 1:
+    HOME = f'/cpfs01/user/{user_names[0]}'
+elif len(user_names) == 2:
+    if 'liukuikun' in user_names[0]:
+        HOME = f'/cpfs01/user/{user_names[1]}'
+    elif 'liukuikun' in user_names[1]:
+        HOME = f'/cpfs01/user/{user_names[0]}'
+    else:
+        HOME = None
+else:
+    HOME = None
 
 
 def get_conda_envs():
     """Function to retrieve all conda environments."""
     try:
         result = subprocess.run(['conda', 'env', 'list'],
                                 capture_output=True,
@@ -69,34 +59,45 @@
                 env_dict[key.strip()] = value.strip()
     return env_dict
 
 
 def main():
     parser = argparse.ArgumentParser(
         description='Run a job with the specified configuration using DLC.')
+    parser.add_argument('--data-sources', help='User ID')
+    parser.add_argument('--priority', type=int, default=1, help='priority')
+    parser.add_argument('--workspace-id',
+                        type=int,
+                        default=5366,
+                        help='Workspace ID')
+    parser.add_argument('--resource-id',
+                        type=str,
+                        default='quota12hhgcm8cia',
+                        help='Quota ID')
     parser.add_argument('--job-name',
                         '-J',
                         default='dlc_job',
                         help='Name of the job')
-    parser.add_argument('--partition',
-                        '-p',
-                        default='llmit',
-                        help='Partition for DLC job')
+
     parser.add_argument('--config',
                         '-c',
                         default=os.path.expanduser(f'{HOME}/.dlc/config'),
                         help='DLC configuration path')
     parser.add_argument('--dlc-path',
                         default='/cpfs01/shared/public/dlc',
                         help='DLC installation path')
     parser.add_argument('--kind',
                         type=str,
-                        choices=['TFJob', 'BatchJob', 'PyTorchJob'],
-                        default='PyTorchJob',
+                        choices=[
+                            'elasticbatchjob', 'flinkbatchjob', 'pytorchjob',
+                            'mpijob', 'tfjob', 'xgboostjob'
+                        ],
+                        default='pytorchjob',
                         help='Kind of job')
+
     parser.add_argument('--worker-count',
                         type=int,
                         default=1,
                         help='Number of workers')
     parser.add_argument('--worker-gpu',
                         type=int,
                         default=8,
@@ -104,27 +105,29 @@
     parser.add_argument('--worker-cpu',
                         type=int,
                         default=120,
                         help='CPU count for single worker')
     parser.add_argument(
         '--worker-image',
         type=str,
-        default='master0:5000/eflops/yehaochen:tears-and-blood1',
+        default=
+        'pjlab-wulan-acr-registry-vpc.cn-wulanchabu.cr.aliyuncs.com/pjlab-eflops/liukuikun:cu121-ubuntu22-lkk-0513-rc6',
         help='Docker image for the worker')
     parser.add_argument('--worker-memory',
                         type=int,
                         default=800,
                         help='Memory in GB for single worker')
     parser.add_argument('--interactive',
                         action='store_true',
                         help='Whether to print out job status or not.')
+    parser.add_argument('--home', default=HOME, help='The path for HOME')
     parser.add_argument('--shell',
                         type=str,
                         choices=['bash', 'zsh', 'none'],
-                        default='none',
+                        default='zsh',
                         help='Shell to use for command execution')
     parser.add_argument('--conda-env',
                         type=validate_conda_env,
                         default='',
                         help='Conda environment to activate')
     parser.add_argument('--proxy',
                         action='store_true',
@@ -140,20 +143,16 @@
     parser.add_argument(
         'task_cmds',
         # required=True,
         nargs=argparse.REMAINDER,
         help='Command line to execute, similar to typing in the shell.')
     args = parser.parse_args()
 
-    workspace_id = get_workspace_id(args.partition, args.config, args.dlc_path)
-    if not workspace_id:
-        print('Failed to retrieve workspace ID.')
-        exit(1)
-
-    home_cmd = f'export HOME={HOME}'
+    assert args.home is not None, 'HOME is not set.'
+    home_cmd = f'export HOME={args.home}'
     shell_cmd = (f'{args.shell} -c "source ~/.{args.shell}rc'
                  if args.shell != 'none' else '')
     conda_cmd = f'conda activate {args.conda_env}' if args.conda_env else ''
     if args.proxy:
         proxy_cmd = ('export http_proxy=http://58.34.83.134:31128 && '
                      'export https_proxy=http://58.34.83.134:31128')
     else:
@@ -165,29 +164,32 @@
     env_cmds = [
         cmd
         for cmd in [home_cmd, proxy_cmd, env_var_cmds, shell_cmd, conda_cmd]
         if cmd
     ]
     full_env_cmd = ' && '.join(env_cmds)
 
-    full_command = (
-        f'{full_env_cmd} && cd {os.getcwd()} && '
-        f"{' '.join(args.task_cmds).strip()}") + '"' if shell_cmd else ''
+    full_command = (f'{full_env_cmd} && cd {os.getcwd()} && '
+                    f"{' '.join(args.task_cmds).strip()}")
+    if shell_cmd:
+        full_command += '"'
 
     dlc_command = [
-        f'{args.dlc_path} create job',
+        f'{args.dlc_path} submit {args.kind}',
         f'--config {args.config}',
         f'--name {args.job_name}',
-        f'--kind {args.kind}',
-        f'--worker_count {args.worker_count}',
+        f'--priority {args.priority}',
+        f'--resource_id {args.resource_id}',
+        f'--data_sources {args.data_sources}',
+        f'--workspace_id {args.workspace_id}',
+        f'--workers {args.worker_count}',
         f'--worker_cpu {args.worker_cpu}',
         f'--worker_gpu {args.worker_gpu}',
-        f'--worker_memory {args.worker_memory}',
+        f'--worker_memory {args.worker_memory}Gi',
         f'--worker_image {args.worker_image}',
-        f'--workspace_id {workspace_id}',
         f'--worker_shared_memory {args.worker_memory // 2}',
         '--interactive' if args.interactive else '',
         f"--command '{full_command}'",
     ]
 
     dlc_full_command = ' '.join(filter(None, dlc_command))
     print(f'Executing command:\n{dlc_full_command}')
```

### Comparing `dlc_run-0.0.3/dlc_run/version.py` & `dlc_run-0.0.4/dlc_run/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `dlc_run-0.0.3/setup.py` & `dlc_run-0.0.4/setup.py`

 * *Files identical despite different names*

