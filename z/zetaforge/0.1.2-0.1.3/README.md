# Comparing `tmp/zetaforge-0.1.2.tar.gz` & `tmp/zetaforge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetaforge-0.1.2.tar", last modified: Thu Apr 18 21:39:05 2024, max compression
+gzip compressed data, was "zetaforge-0.1.3.tar", last modified: Mon May 13 22:28:00 2024, max compression
```

## Comparing `zetaforge-0.1.2.tar` & `zetaforge-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.144678 zetaforge-0.1.2/
--rw-r--r--   0 jon        (501) staff       (20)    34523 2024-04-08 18:07:53.000000 zetaforge-0.1.2/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-18 21:39:05.144558 zetaforge-0.1.2/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     5695 2024-04-10 16:47:21.000000 zetaforge-0.1.2/README.md
--rw-r--r--   0 jon        (501) staff       (20)      104 2024-04-08 19:29:07.000000 zetaforge-0.1.2/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2024-04-18 21:39:05.144725 zetaforge-0.1.2/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)     1844 2024-04-18 20:56:32.000000 zetaforge-0.1.2/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.142507 zetaforge-0.1.2/zetaforge/
--rw-r--r--   0 jon        (501) staff       (20)       22 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)     1657 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/check_forge_dependencies.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143305 zetaforge-0.1.2/zetaforge/executables/
--rw-r--r--   0 jon        (501) staff       (20)      122 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/executables/README.md
--rw-r--r--   0 jon        (501) staff       (20)     3389 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/forge_cli.py
--rw-r--r--   0 jon        (501) staff       (20)    13795 2024-04-18 20:56:35.000000 zetaforge-0.1.2/zetaforge/forge_runner.py
--rw-r--r--   0 jon        (501) staff       (20)    11862 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/install_forge_dependencies.py
--rw-r--r--   0 jon        (501) staff       (20)     1504 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/mixpanel_client.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143840 zetaforge-0.1.2/zetaforge/utils/
--rw-r--r--   0 jon        (501) staff       (20)     3003 2024-04-10 16:47:21.000000 zetaforge-0.1.2/zetaforge/utils/build.yaml
--rw-r--r--   0 jon        (501) staff       (20)    37294 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/utils/install.yaml
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143174 zetaforge-0.1.2/zetaforge.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      507 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       55 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/entry_points.txt
--rw-r--r--   0 jon        (501) staff       (20)      126 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       10 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/top_level.txt
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-05-13 22:28:00.709871 zetaforge-0.1.3/
+-rw-r--r--   0 jon        (501) staff       (20)    34523 2024-04-08 18:07:53.000000 zetaforge-0.1.3/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)      477 2024-05-13 22:28:00.709637 zetaforge-0.1.3/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     5695 2024-04-10 16:47:21.000000 zetaforge-0.1.3/README.md
+-rw-r--r--   0 jon        (501) staff       (20)      104 2024-04-08 19:29:07.000000 zetaforge-0.1.3/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2024-05-13 22:28:00.709918 zetaforge-0.1.3/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)     1869 2024-05-09 19:07:32.000000 zetaforge-0.1.3/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-05-13 22:28:00.707645 zetaforge-0.1.3/zetaforge/
+-rw-r--r--   0 jon        (501) staff       (20)       22 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)     2148 2024-05-09 14:53:18.000000 zetaforge-0.1.3/zetaforge/check_forge_dependencies.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-05-13 22:28:00.708480 zetaforge-0.1.3/zetaforge/executables/
+-rw-r--r--   0 jon        (501) staff       (20)      122 2024-04-08 19:29:07.000000 zetaforge-0.1.3/zetaforge/executables/README.md
+-rw-r--r--   0 jon        (501) staff       (20)     4073 2024-05-09 14:53:18.000000 zetaforge-0.1.3/zetaforge/forge_cli.py
+-rw-r--r--   0 jon        (501) staff       (20)    13965 2024-05-09 19:05:58.000000 zetaforge-0.1.3/zetaforge/forge_runner.py
+-rw-r--r--   0 jon        (501) staff       (20)    12279 2024-05-13 21:57:19.000000 zetaforge-0.1.3/zetaforge/install_forge_dependencies.py
+-rw-r--r--   0 jon        (501) staff       (20)    25173 2024-05-08 21:53:36.000000 zetaforge-0.1.3/zetaforge/mixpanel.py
+-rw-r--r--   0 jon        (501) staff       (20)     2218 2024-05-08 21:53:36.000000 zetaforge-0.1.3/zetaforge/mixpanel_client.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-05-13 22:28:00.708855 zetaforge-0.1.3/zetaforge/utils/
+-rw-r--r--   0 jon        (501) staff       (20)     3075 2024-05-09 14:53:18.000000 zetaforge-0.1.3/zetaforge/utils/build.yaml
+-rw-r--r--   0 jon        (501) staff       (20)    37294 2024-05-09 14:53:18.000000 zetaforge-0.1.3/zetaforge/utils/install.yaml
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-05-13 22:28:00.709358 zetaforge-0.1.3/zetaforge.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      477 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      529 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       55 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (501) staff       (20)      145 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       10 2024-05-13 22:28:00.000000 zetaforge-0.1.3/zetaforge.egg-info/top_level.txt
```

### Comparing `zetaforge-0.1.2/LICENSE` & `zetaforge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zetaforge-0.1.2/README.md` & `zetaforge-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `zetaforge-0.1.2/setup.py` & `zetaforge-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,10 +50,11 @@
     install_requires = [
         'setuptools==69.0.2',
         'requests==2.31.0', 
         'boto3==1.34.79', 
         'colorama==0.4.6', 
         'mixpanel==4.10.1', 
         "langchain==0.1.15", 
-        "langchain-openai==0.1.2"],
+        "langchain-openai==0.1.2",
+        "sentry-sdk===2.0.1"],
     include_package_data=True,
-    package_data={'zetaforge': ['utils/*.yaml', 'executables/*'],},)
+    package_data={'zetaforge': ['utils/*', 'executables/*'],},)
```

### Comparing `zetaforge-0.1.2/zetaforge/check_forge_dependencies.py` & `zetaforge-0.1.3/zetaforge/check_forge_dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,17 +24,29 @@
     for line in lines:
         parts = line.split("-")
         if parts[0] == name:
             return True
     
     return False
 
-def check_dependencies():
-    kubectl_flag = check_kubectl()
-    return kubectl_flag
+def check_kube_svc(name, namespace="default"):
+    check_kube = subprocess.run(["kubectl", f"--namespace={namespace}", "get", "svc"], capture_output=True, text=True)
+    print(check_kube)
+    lines = check_kube.stdout.strip().split("\n")[1:]  # Skip the header line
+    for line in lines:
+        print(line)
+        parts = line.split(" ")
+        if parts[0].strip() == name:
+            return True
+    
+    return False
+    
+def check_minikube():
+    check_ctl = subprocess.run(["minikube", "version"], capture_output=True, text=True)
+    return check_ctl.returncode == 0
 
 def check_docker_installed():
     docker = subprocess.run("docker", capture_output=True, text=True)
     if docker.returncode != 0:
         print("Please install docker desktop to your computer:")
         if platform.system() == 'Windows':
             print("https://docs.docker.com/desktop/install/windows-install/")
```

### Comparing `zetaforge-0.1.2/zetaforge/forge_runner.py` & `zetaforge-0.1.3/zetaforge/forge_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 import os
 import subprocess
 import platform
 import time
 import json
 from pkg_resources import resource_filename
-from .check_forge_dependencies import check_dependencies, check_running_kube, check_kube_pod
+from .check_forge_dependencies import check_minikube, check_running_kube, check_kube_pod, check_kubectl
 from .install_forge_dependencies import *
 from pathlib import Path
 from colorama import init, Fore
 from datetime import datetime
-import socket, errno
+import socket
 import json
 import shutil
-import yaml 
 import threading
-from .mixpanel_client import MixpanelClient
+from .mixpanel_client import mixpanel_client
+import sentry_sdk
 
 
-mixpanel_client = MixpanelClient('4c09914a48f08de1dbe3dc4dd2dcf90d')
-
+run_env = mixpanel_client.is_dev
+env = "production"
+if run_env:
+    env = "development"
+sentry_sdk.init(
+    dsn="https://7fb18e8e487455a950298625457264f3@o1096443.ingest.us.sentry.io/4507031960223744",
+
+    # Enable performance monitoring
+    enable_tracing=True,
+    environment=env
+)
 
 BUILD_YAML = resource_filename("zetaforge", os.path.join('utils', 'build.yaml'))
 INSTALL_YAML = resource_filename("zetaforge", os.path.join('utils', 'install.yaml'))
 
 EXECUTABLES_PATH = os.path.join(Path(__file__).parent, 'executables')
 FRONT_END = os.path.join(EXECUTABLES_PATH, "frontend")
 
-def write_json(server_version, client_version, context, registry_port):
-    _, server_path = get_launch_paths(server_version, client_version)
-    config = create_config_json(os.path.dirname(server_path), context, registry_port)
+def write_json(server_version, client_version, context, driver, is_dev, s2_path=None):
+    if s2_path:
+        server_path = s2_path
+    else:
+        _, server_path = get_launch_paths(server_version, client_version)
+    config = create_config_json(os.path.dirname(server_path), context, driver, is_dev)
     return config
+#changes the ZetaforgeIsDev in config.json, it's implemented to prevent certain edge cases.
+def change_env_config(server_version, client_version, env):
+    _, server_path = get_launch_paths(server_version, client_version)
+    config = dict()
+    config_path = os.path.join(os.path.dirname(server_path), "config.json")
+    with open(config_path, "r") as f:
+        config = json.load(f)
+    config['ZetaforgeIsDev'] = env
+    with open(config_path, "w") as outfile:
+        json.dump(config, outfile)
+    return outfile
+
+
 
 
 def check_for_container(name):
     ls_cmd = subprocess.run(["docker", "container", "ls", '--format', 'json'], capture_output=True, text=True)
     container_id = None
 
     if ls_cmd.returncode == 0:
@@ -65,27 +90,14 @@
                 s.close()  # Close the socket to release the port
                 print(f"Port {port} is open, setting this for the registry")
                 return port
             except OSError:
                 pass
     return None
 
-def update_yaml(port):
-    d = None
-    yaml_doc = None
-    with open(BUILD_YAML) as f:
-        yaml_doc = list(yaml.safe_load_all(f))
-        d = yaml_doc[-1]
-
-    d['spec']['ports'][0]['port'] = port
-    yaml_doc[-1] = d
-
-    with open(BUILD_YAML, "w") as f:
-        yaml.dump_all(yaml_doc, f, default_flow_style=False)
-
 def get_kubectl_contexts():
     # Get the list of kubectl contexts
     result = subprocess.run(["kubectl", "config", "get-contexts"], capture_output=True, text=True)
     lines = result.stdout.strip().split("\n")[1:]  # Skip the header line
 
     contexts = []
     for line in lines:
@@ -127,112 +139,78 @@
     confirmation = input(f"You have selected the context: {selected_context}. Is this correct? (y/n): ")
     if confirmation.lower() != "y":
         print("Context selection canceled.")
         return None
 
     return selected_context
 
-def setup(server_version, client_version, build_flag = True, install_flag = True):
+def setup(server_version, client_version, driver, build_flag = True, install_flag = True, is_dev=False, server_path=None):
     print("Platform: ", platform.machine())
     print("CWD: ", os.path.abspath(os.getcwd()))
-    context = select_kubectl_context()
+    mixpanel_client.track_event('Setup Initiated')
 
-    kubectl_flag = check_dependencies()        
-
-    registry_port = 5000
-    print(f"Setting registry port: {registry_port}")
-    update_yaml(int(registry_port))
-        
-    switch_context = None
-    if kubectl_flag:
-        switch_context = subprocess.run(["kubectl", "config", "use-context", f"{context}"], capture_output=True, text=True)
+    if driver == "minikube":
+        context = "zetaforge"
+        if not check_minikube():
+            mixpanel_client.track_event("Setup Failure - Minikube Not Found")
+            time.sleep(0.5)
+            print("Minikube not found. Please install minikube.")
+            raise Exception("Minikube not found!")
+        minikube = subprocess.run(["minikube", "-p", "zetaforge", "start"], capture_output=True, text=True)
+        if minikube.returncode != 0:
+            mixpanel_client.track_event("Setup Failure - Cannot Start Minikube")
+            time.sleep(0.5)
+            print(minikube.stderr)
+            raise Exception("Error while starting minikube")
+        mixpanel_client.track_event("Setup - Minikube Started")
     else:
-        print("Kubectl not found. Please install docker-desktop and enable kubernetes, or ensure that kubectl installed and is able to connect to a working kubernetes cluster.")
-        raise EnvironmentError("Kubectl not found!")
-        #install_kubectl()
-        #switch_context = subprocess.run(f"./kubectl config use-context {context}", shell=True, cwd=EXECUTABLES_PATH)
+        context = select_kubectl_context()
+        kubectl_flag = check_kubectl()
 
-    in_context = (switch_context.returncode == 0)
-        
-    if not in_context:
-        print(f"Cannot find the context {context} for kubernetes. Please double check that you have entered the correct context.")        
-        subprocess.run(["kubectl", "config", "get-contexts"], capture_output=True, text=True)
-        raise Exception("Exception while setting the context")
-    
-    running_kube = check_running_kube(context)
-    if not running_kube:
-        raise Exception("Kubernetes is not running, please start kubernetes and ensure that you are able to connect to the kube context.")
-
-        
-    build = subprocess.run(["kubectl", "apply", "-f", f"{BUILD_YAML}"], capture_output=True, text=True)
-    install = subprocess.run(["kubectl", "apply", "-f", f"{INSTALL_YAML}"], capture_output=True, text=True)
-
-    if build.returncode != 0 or install.returncode != 0:
-        raise Exception("Error while building")
-        
-    time.sleep(3)
-    name = "k8s_registry"
-    container_id = check_for_container(name)
-
-    if not container_id:
-        print("Registry is not running, please verify that docker and kubernetes are running and re-run the setup process.")
-        raise Exception("Error detecting container registry")
-        
-    if context == "docker-desktop":
-        ins_cmd = subprocess.run(["docker", "inspect", str(container_id)], capture_output=True, text=True)
-
-        json_data = json.loads(ins_cmd.stdout)[0]
-        volumename = ""
-        for item in json_data.get("Mounts", []):
-            volumetype = item.get("Type", "")
-            if volumetype == 'volume':
-                volumename = item.get("Name", "")
-        print("Volume: ", volumename)
-            
-        print("Binding k8s registry to registry pod")
-        regcmd = subprocess.Popen(["docker", "run", "--rm", "--name", "registry", "-p", f"{registry_port}:5000", "-v", f"{volumename}:/var/lib/registry", "registry:2"],  stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-        while True:
-            checkcmd = subprocess.run(["docker", "inspect", "registry"], capture_output=True)  
-            
-            if checkcmd.stdout:
-                break
-            
-            time.sleep(1)
+        switch_context = None
+        if kubectl_flag:
+            switch_context = subprocess.run(["kubectl", "config", "use-context", f"{context}"], capture_output=True, text=True)
+            mixpanel_client.track_event("Setup - Kubectl Found")
+        else:
+            print("Kubectl not found. Please install docker-desktop, orbstack, or minikube and enable kubernetes, or ensure that kubectl installed and is able to connect to a working kubernetes cluster.")
+            mixpanel_client.track_event("Setup Failure - Kubectl Not Found")
+            time.sleep(0.5)
+            raise EnvironmentError("Kubectl not found!")
+
+        in_context = (switch_context.returncode == 0)
+
+        if not in_context:
+            print(f"Cannot find the context {context} for kubernetes. Please double check that you have entered the correct context.")        
+            subprocess.run(["kubectl", "config", "get-contexts"], capture_output=True, text=True)
+            mixpanel_client.track_event("Setup Failure - Context Switch Error")
+            raise Exception("Exception while setting the context")
+
+        mixpanel_client.track_event("Setup - Context changed")
+
+        running_kube = check_running_kube(context)
+        if not running_kube:
+            raise Exception("Kubernetes is not running, please start kubernetes and ensure that you are able to connect to the kube context.")
 
-        regcmd.terminate()
-        print("Completed binding pods")
-    
     install_frontend_dependencies(client_version=client_version)
 
-    config_path = write_json(server_version, client_version, context, registry_port)
+    config_path = write_json(server_version, client_version, context, driver, is_dev, s2_path=server_path)
 
     print(f"Setup complete, wrote config to {config_path}.")
-        
+    mixpanel_client.track_event("Setup Successful")
     return config_path
 
 
 #dev version is only passed, when a developer wants to pass a local version(for e.g. dev_path=./s2-v2.3.5-amd64)
-def run_forge(server_version=None, client_version=None, server_path=None, client_path=None):
+def run_forge(server_version=None, client_version=None, server_path=None, client_path=None, is_dev=False):
     global time_start
     time_start = datetime.now()
-
+    mixpanel_client.track_event('Launch Initiated')
+    change_env_config(server_version, client_version, is_dev)
     #init is called for collarama library, better logging.
-    init()   
-
-    reg = check_kube_pod("registry")
-    if not reg:
-        print("Registry container not found, restarting..")
-        setup(server_version, client_version)
-        raise Exception("Container registry is not running, please ensure kubernetes is running or re-run `zetaforge setup`.")
-    weed = check_kube_pod("weed")
-    if not weed:
-        raise Exception("SeaweedFS is not running, please ensure kubernetes is running or re-run `zetaforge setup`.")
-
-    mixpanel_client.track_event('Initial Launch')
+    init()
 
     if server_path is None:
         _, server_path = get_launch_paths(server_version, client_version)
 
     if client_path is None:
         client_path, _ = get_launch_paths(server_version, client_version)
 
@@ -242,27 +220,42 @@
         print(f"Launching execution server {server_path}..")
         server_executable = os.path.basename(server_path)
         if platform.system() != 'Windows':
             server_executable = f"./{server_executable}"
         else:
             server_executable = server_path
         
-        server = subprocess.Popen([server_executable],stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(server_path))
-
+        try:
+            server = subprocess.Popen([server_executable],stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(server_path))
+        except:
+            mixpanel_client.track_event("Launch Failure - Anvil Launch Failed")
+            raise Exception(f"Error occured while launching the server executable: {server_executable}")
+        
+        mixpanel_client.track_event('Launch - Anvil Launched')
+        
         print(f"Launching client {client_path}..")
         client_executable = os.path.basename(client_path)
         if platform.system() == 'Darwin':
             client_executable = [f"./{client_executable}"]
         elif platform.system() == 'Windows':
             client_executable = [client_path, '--no-sandbox']
         else: 
             client_executable = [f"./{client_executable}"]
+        
+        #handles the situation where user launches pip launcher with is_dev, for the client executable.
+        if is_dev:
+            client_executable.append("--is_dev")
 
-        client = subprocess.Popen(client_executable, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(client_path))
-
+        try:
+            client = subprocess.Popen(client_executable, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(client_path))
+        except:
+            mixpanel_client.track_event("Launch Failure - Client Launch Failed")
+            raise Exception(f"Error occured while launching the client executable: {client_executable}")
+            
+        mixpanel_client.track_event('Launch - Client Launched')
         def read_output(process, name):
             for line in process.stdout:
                 print(f"{name}: {line.decode('utf-8')}", end='')
 
         def read_error(process, name):
             for line in process.stderr:
                 print(f"{name} (stderr): {line.decode('utf-8')}", end='')
@@ -281,53 +274,51 @@
 
         # Wait for the threads to finish
         server_stdout_thread.join()
         server_stderr_thread.join()
         client_stdout_thread.join()
         client_stderr_thread.join()
 
+        mixpanel_client.track_event('Launch Successful')
+
     except KeyboardInterrupt: 
         print("Terminating servers..")
 
     finally:
         total_time = (datetime.now() - time_start).total_seconds()
-       
 
         try:
-            mixpanel_client.track_event('Full Launch', props={'Duration(seconds)': total_time})
+            mixpanel_client.track_event('Launch End', props={'Duration(seconds)': total_time})
             time.sleep(2) # mixpanel instance is asynch, so making sure that it completes the call before tear down
         except:
             print("Mixpanel cannot track")
 
-        server.kill()
         client.kill()
 
 
 #purge executables, and upload them from the scratch
 def purge():
     shutil.rmtree(EXECUTABLES_PATH)
     os.makedirs(EXECUTABLES_PATH)
 
-def teardown():
-    contexts = get_kubectl_contexts()
-    default = None
-    for i, context in enumerate(contexts, start=1):
-        if context.startswith("*"):
-            default = context[1:]
-    
-    print("Tearing down services..")
-    if default and default == "docker-desktop":
-        stop = subprocess.run(["kubectl", "stop", "registry"], capture_output=True, text=True)
-        print(stop.stdout)
+def teardown(driver):
+    if driver == "minikube":
+        minikube = subprocess.run(["minikube", "-p", "zetaforge", "stop"], capture_output=True, text=True)
+        if minikube.returncode != 0:
+            print(minikube.stderr)
+            raise Exception("Error while starting minikube")
 
+    print("Completed teardown!")
+
+def uninstall():
     install = subprocess.run(["kubectl", "delete", "-f", INSTALL_YAML], capture_output=True, text=True)
     print ("Removing install: ", {install.stdout})
     build = subprocess.run(["kubectl", "delete", "-f", BUILD_YAML], capture_output=True, text=True)
     print("Removing build: ", {build.stdout})
-    print("Completed teardown!")
+
 
 def check_expected_services(config):
     is_local = config["IsLocal"]
     print(config)
     if is_local:
         local = config["Local"]
         ports = [local["RegistryPort"]]
@@ -344,31 +335,34 @@
                 if e.errno == errno.EADDRINUSE:
                     print(f"Service running at port {port}")
             finally:
                 sock.close()
     
     return True 
 
-def create_config_json(s2_path, context, registry_port=5000):
+def create_config_json(s2_path, context, driver, is_dev):
     config = {
         "IsLocal":True,
-        "ServerPort":"8080",
+        "ServerPort": 8080,
         "KanikoImage":"gcr.io/kaniko-project/executor:latest",
         "WorkDir":"/app",
         "FileDir":"/files",
         "ComputationFile":"computations.py",
         "EntrypointFile":"entrypoint.py",
         "ServiceAccount":"executor",
         "Bucket":"forge-bucket",
         "Database":"./zetaforge.db",
         "KubeContext": context,
         "Local": {
-            "BucketPort":"8333",
-            "RegistryPort": str(registry_port)
-        }
+            "BucketPort": 8333,
+            "Driver": driver
+        },
+        "ZetaforgeIsDev": is_dev
     } 
 
     file_path = os.path.join(s2_path, "config.json")
     with open(file_path, "w") as outfile: 
         json.dump(config, outfile)
 
-    return file_path
+    return file_path
+
+
```

### Comparing `zetaforge-0.1.2/zetaforge/install_forge_dependencies.py` & `zetaforge-0.1.3/zetaforge/install_forge_dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 from pathlib import Path
 import ssl
 import os
 import platform
 import sys
 from zipfile import ZipFile
 import tarfile
+from .check_forge_dependencies import check_kube_svc
+from pkg_resources import resource_filename
 
 # BACKEND = resource_filename("")
 EXECUTABLES_PATH = os.path.join(Path(__file__).parent, 'executables')
 ssl._create_default_https_context = ssl._create_unverified_context
 
+BUILD_YAML = resource_filename("zetaforge", os.path.join('utils', 'build.yaml'))
+INSTALL_YAML = resource_filename("zetaforge", os.path.join('utils', 'install.yaml'))
+
 s3 = boto3.client('s3', config=Config(signature_version=UNSIGNED), region_name='us-east-2')
 
 def install_kubectl():
     try:
         stable_release_url = "https://dl.k8s.io/release/stable.txt"
         response = requests.get(stable_release_url)
         stable_release = None
@@ -188,40 +193,45 @@
     for filename in os.listdir(directory):
         file_parts = filename.split('-')
         if len(file_parts) >= 2:
             file_version = file_parts[1]
             if file_version == version:
                 print(f"Found an existing install of version {version}")
             else:
+                print(f"Found a previous version of forge, uninstalling..")
+
+
                 file_path = os.path.join(directory, filename)
                 if os.path.isfile(file_path):
                     os.remove(file_path)
                     print(f"Removed file: {filename}")
                 elif os.path.isdir(file_path):
                     shutil.rmtree(file_path)
                     print(f"Removed directory: {filename}")
         
-        if filename == 'ZetaForge.app':
-            _, server_path = get_launch_paths(version, version)
-            if os.path.exists(server_path):
-                print(f"Found existing version {version}")
-            else:
-                # did not find the correct version, reinstall it
-                print(f"Found ZetaForge.app but did not find version {version}, removing previous app")
-                shutil.rmtree(os.path.join(EXECUTABLES_PATH, "ZetaForge.app"))
-
-        if filename == 'zetaforge.app':
+        if filename == 'ZetaForge.app' or filename == 'zetaforge.app':
             _, server_path = get_launch_paths(version, version)
             if os.path.exists(server_path):
                 print(f"Found existing version {version}")
             else:
                 # did not find the correct version, reinstall it
                 print(f"Found ZetaForge.app but did not find version {version}, removing previous app")
-                shutil.rmtree(os.path.join(EXECUTABLES_PATH, "zetaforge.app"))
+                shutil.rmtree(os.path.join(EXECUTABLES_PATH, filename))
 
+def remove_running_services():
+    print(f"Checking for existing kube services to remove..")
+    registry = check_kube_svc("registry")
+    argo = check_kube_svc("argo-server", "argo")
+    if registry:
+        build = subprocess.run(["kubectl", "delete", "-f", BUILD_YAML], capture_output=True, text=True)
+        print("Removing build: ", {build.stdout})
+
+    if argo:
+        build = subprocess.run(["kubectl", "delete", "-f", INSTALL_YAML], capture_output=True, text=True)
+        print("Removing build: ", {build.stdout})
 
 def check_version(server_version, client_version):
     check_and_clean_files(EXECUTABLES_PATH, client_version)
     check_and_clean_files(EXECUTABLES_PATH, server_version)
 
 def get_app_dir(client_version):
     if platform.system() == 'Darwin':
```

### Comparing `zetaforge-0.1.2/zetaforge/utils/build.yaml` & `zetaforge-0.1.3/zetaforge/utils/build.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,21 @@
   name: executor
 ---
 apiVersion: rbac.authorization.k8s.io/v1
 kind: Role
 metadata:
   name: executor
 rules:
-- apiGroups:
-  - argoproj.io
-  resources:
-  - workflowtaskresults
-  verbs:
-  - create
-  - patch
+  - apiGroups:
+      - argoproj.io
+    resources:
+      - workflowtaskresults
+    verbs:
+      - create
+      - patch
 ---
 apiVersion: rbac.authorization.k8s.io/v1
 kind: RoleBinding
 metadata:
   name: executor-binding
 roleRef:
   apiGroup: rbac.authorization.k8s.io
@@ -26,116 +26,141 @@
   name: executor
 subjects:
 - kind: ServiceAccount
   name: executor
 ---
 apiVersion: v1
 kind: Secret
-metadata:
+metadata: 
   name: ninja-secret
 stringData:
   accessKey: AKIAIOSFODNN7EXAMPLE
   secretKey: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
 ---
 apiVersion: v1
-data:
-  default: "s3:\n  bucket: zetaforge\n  endpoint: weed:8333\n  region: us-east-1\n\
-    \  insecure: true\n  accessKeySecret:\n    name: ninja-secret\n    key: accessKey\n\
-    \  secretKeySecret:\n    name: ninja-secret\n    key: secretKey\n"
 kind: ConfigMap
 metadata:
   name: forge-bucket
+data:
+  default: |
+    s3:
+      bucket: zetaforge
+      endpoint: weed:8333
+      region: us-east-1
+      insecure: true
+      accessKeySecret:
+        name: ninja-secret
+        key: accessKey
+      secretKeySecret:
+        name: ninja-secret
+        key: secretKey
 ---
 apiVersion: v1
-data:
-  config.json: "{\n  \"identities\": [\n    {\n      \"name\": \"main\",\n      \"\
-    credentials\": [\n        {\n          \"accessKey\": \"AKIAIOSFODNN7EXAMPLE\"\
-    ,\n          \"secretKey\": \"wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY\"\n   \
-    \     }\n      ],\n      \"actions\": [\n        \"Read\",\n        \"List\",\n\
-    \        \"Write\"\n      ]\n    },\n    {\n      \"name\": \"anonymous\",\n \
-    \     \"actions\": [\n        \"Read\",\n        \"List\"\n      ]\n    }\n\n\
-    \  ]\n}"
 kind: ConfigMap
 metadata:
   name: seaweed-config
+data:
+  config.json: |-
+    {
+      "identities": [
+        {
+          "name": "main",
+          "credentials": [
+            {
+              "accessKey": "AKIAIOSFODNN7EXAMPLE",
+              "secretKey": "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY"
+            }
+          ],
+          "actions": [
+            "Admin",
+            "Read",
+            "List",
+            "Write"
+          ]
+        },
+        {
+          "name": "anonymous",
+          "actions": [
+            "Read",
+            "List"
+          ]
+        }
+      ]
+    }
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
+  name: weed
   labels:
     app.kubernetes.io/name: weed
-  name: weed
 spec:
   replicas: 1
   selector:
     matchLabels:
       app.kubernetes.io/name: weed
   template:
     metadata:
       labels:
         app.kubernetes.io/name: weed
     spec:
       containers:
-      - command:
-        - weed
-        - server
-        - -s3.config=/home/config.json
-        - -s3
-        image: chrislusf/seaweedfs
-        name: weed
-        ports:
-        - containerPort: 8333
-        volumeMounts:
-        - mountPath: /home
-          name: config
+        - name: weed
+          image: chrislusf/seaweedfs
+          command: ["weed", "server", "-s3.config=/home/config.json", "-s3"]
+          ports:
+            - containerPort: 8333
+          volumeMounts:
+            - name: config
+              mountPath: /home
       volumes:
-      - configMap:
-          name: seaweed-config
-        name: config
+        - name: config
+          configMap:
+            name: seaweed-config
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: weed
 spec:
-  loadBalancerIP: null
-  ports:
-  - port: 8333
-    targetPort: 8333
+  type: LoadBalancer
+  loadBalancerIP: ~
   selector:
     app.kubernetes.io/name: weed
-  type: LoadBalancer
+  ports:
+    - port: 8333
+      targetPort: 8333
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
+  name: registry
   labels:
     app.kubernetes.io/name: registry
-  name: registry
 spec:
   replicas: 1
   selector:
     matchLabels:
       app.kubernetes.io/name: registry
   template:
     metadata:
       labels:
         app.kubernetes.io/name: registry
     spec:
       containers:
-      - image: registry:2
-        name: registry
-        ports:
-        - containerPort: 5000
+        - name: registry
+          image: registry:2
+          ports:
+            - containerPort: 5000
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: registry
 spec:
-  loadBalancerIP: null
+  type: LoadBalancer
+  loadBalancerIP: ~
+  selector:
+    app.kubernetes.io/name: registry
   ports:
   - port: 5000
     targetPort: 5000
-  selector:
-    app.kubernetes.io/name: registry
-  type: LoadBalancer
```

### Comparing `zetaforge-0.1.2/zetaforge/utils/install.yaml` & `zetaforge-0.1.3/zetaforge/utils/install.yaml`

 * *Files identical despite different names*

