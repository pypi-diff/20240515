# Comparing `tmp/sparecores_runner-0.0.2.tar.gz` & `tmp/sparecores_runner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_runner-0.0.2.tar", last modified: Fri May 10 20:32:02 2024, max compression
+gzip compressed data, was "sparecores_runner-0.0.3.tar", last modified: Wed May 15 20:43:57 2024, max compression
```

## Comparing `sparecores_runner-0.0.2.tar` & `sparecores_runner-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/sc_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.337211 sparecores_runner-0.0.2/src/sc_runner/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-10 20:31:58.000000 sparecores_runner-0.0.2/src/sc_runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:32:02.341211 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 20:32:02.000000 sparecores_runner-0.0.2/src/sparecores_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:57.062899 sparecores_runner-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 20:43:57.062899 sparecores_runner-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:43:57.062899 sparecores_runner-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:57.058899 sparecores_runner-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:57.058899 sparecores_runner-0.0.3/src/sc_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:57.062899 sparecores_runner-0.0.3/src/sc_runner/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/resources/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-15 20:43:50.000000 sparecores_runner-0.0.3/src/sc_runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:43:57.062899 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 20:43:57.000000 sparecores_runner-0.0.3/src/sparecores_runner.egg-info/top_level.txt
```

### Comparing `sparecores_runner-0.0.2/LICENSE` & `sparecores_runner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.2/PKG-INFO` & `sparecores_runner-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-runner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Start cloud instances.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-runner
 Project-URL: issues, https://github.com/SpareCores/sc-runner/issues
 Project-URL: documentation, https://sparecores.github.io/sc-runner/
 Project-URL: homepage, https://sparecores.com
```

### Comparing `sparecores_runner-0.0.2/pyproject.toml` & `sparecores_runner-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-runner"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">= 3.9"
 dependencies = [
     "click",
     "pulumi",
     "pulumi-aws",
     "sparecores-crawler",
     "sparecores-data",
```

### Comparing `sparecores_runner-0.0.2/src/sc_runner/cli.py` & `sparecores_runner-0.0.3/src/sc_runner/cli.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.2/src/sc_runner/data.py` & `sparecores_runner-0.0.3/src/sc_runner/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,7 +33,11 @@
 def servers_vendors(vendor: str, region: str | None = None, zone: str | None = None):
     stmt = select(ServerPrice.vendor_id, ServerPrice.datacenter_id, Zone.name, ServerPrice.server_id).join(Zone).where(ServerPrice.vendor_id == vendor)
     if region:
         stmt = stmt.where(ServerPrice.datacenter_id == region)
     if zone:
         stmt = stmt.where(ServerPrice.zone_id == zone)
     return session.exec(stmt.distinct()).all()
+
+
+def server_cpu_architecture(vendor: str, server: str) -> str:
+    return session.exec(select(Server.cpu_architecture).where(Server.vendor_id == vendor).where(Server.api_reference == server)).one().value
```

### Comparing `sparecores_runner-0.0.2/src/sc_runner/resources/aws.py` & `sparecores_runner-0.0.3/src/sc_runner/resources/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 
 
 def resources_aws(
         region: Annotated[str, DefaultOpt(["--region"], type=click.Choice(data.regions("aws")), help="Region"), StackName()] = os.environ.get("AWS_DEFAULT_REGION", "us-east-1"),
         zone: Annotated[str, DefaultOpt(["--zone"], type=click.Choice(data.zones("aws")), help="Availability zone"), StackName()] = os.environ.get("AWS_ZONE", None),
         assume_role_arn: Annotated[str, DefaultOpt(["--assume-role-arn"], type=str, help="Role to be assumed")] = os.environ.get("AWS_ASSUME_ROLE_ARN", ""),
         ami_owner: Annotated[str, DefaultOpt(["--ami-owner"], type=str, help="AMI owner")] = os.environ.get("AWS_AMI_OWNER", "099720109477"),
-        ami_name: Annotated[str, DefaultOpt(["--ami-name"], type=str, help="AWS name filter")] = os.environ.get("AWS_AMI_NAME", "ubuntu/images/hvm-ssd/ubuntu-jammy-22.04-amd64-server-20240301"),
+        # to get the available image names:
+        # aws ec2 describe-images --region us-east-1 --owners 099720109477 | jq '.Images[].Name'
+        ami_name: Annotated[str, DefaultOpt(["--ami-name"], type=str, help="AWS name filter")] = os.environ.get("AWS_AMI_NAME", "ubuntu/images/hvm-ssd-gp3/ubuntu-noble-24.04-*-server-20240423"),
         instance: Annotated[str, DefaultOpt(["--instance"], type=click.Choice(data.servers("aws")), help="Instance type"), StackName()] = os.environ.get("AWS_TYPE", "t3.micro"),
         public_key: Annotated[str, DefaultOpt(["--public-key"], type=str, help="SSH public key")] = os.environ.get("SSH_PUBLIC_KEY", ""),
         tags: Annotated[str, DefaultOpt(["--tags"], type=JSON, default=defaults(DEFAULTS, "tags"), help="Tags for created resources")] = default(DEFAULTS, "tags"),
         instance_opts: Annotated[str, DefaultOpt(["--instance-opts"], type=JSON, default=defaults(DEFAULTS, "instance_opts"), help="Pulumi aws.ec2.Instance options")] = default(DEFAULTS, "instance_opts"),
         vpc_opts: Annotated[str, DefaultOpt(["--vpc-opts"], type=JSON, default=defaults(DEFAULTS, "vpc_opts"), help="Pulumi aws.ec2.Vpc options")] = default(DEFAULTS, "vpc_opts"),
         subnet_opts: Annotated[str, DefaultOpt(["--subnet-opts"], type=JSON, default=defaults(DEFAULTS, "subnet_opts"), help="Pulumi aws.ec2.Subnet options")] = default(DEFAULTS, "subnet_opts"),
         sg_opts: Annotated[str, DefaultOpt(["--sg-opts"], type=JSON, default=defaults(DEFAULTS, "sg_opts"), help="Pulumi aws.ec2.SecurityGroup options")] = default(DEFAULTS, "sg_opts"),
@@ -67,14 +69,15 @@
         )
         instance_opts["key_name"] = pubkey.id
 
     if "ami" not in instance_opts:
         ami = aws.ec2.get_ami(
             most_recent=True,  # in case of a filter is given as the name
             filters=[
+                aws.ec2.GetAmiFilterArgs(name="architecture", values=[data.server_cpu_architecture("aws", instance)]),
                 aws.ec2.GetAmiFilterArgs(name="name", values=[ami_name]),
                 aws.ec2.GetAmiFilterArgs(name="virtualization-type", values=["hvm"]),
             ],
             owners=[ami_owner],
             opts=pulumi.InvokeOptions(provider=provider),
         )
         instance_opts["ami"] = ami.id
```

### Comparing `sparecores_runner-0.0.2/src/sc_runner/resources/base.py` & `sparecores_runner-0.0.3/src/sc_runner/resources/base.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.2/src/sc_runner/runner.py` & `sparecores_runner-0.0.3/src/sc_runner/runner.py`

 * *Files identical despite different names*

### Comparing `sparecores_runner-0.0.2/src/sparecores_runner.egg-info/PKG-INFO` & `sparecores_runner-0.0.3/src/sparecores_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-runner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Start cloud instances.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-runner
 Project-URL: issues, https://github.com/SpareCores/sc-runner/issues
 Project-URL: documentation, https://sparecores.github.io/sc-runner/
 Project-URL: homepage, https://sparecores.com
```

