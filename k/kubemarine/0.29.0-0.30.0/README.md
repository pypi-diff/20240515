# Comparing `tmp/kubemarine-0.29.0.tar.gz` & `tmp/kubemarine-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.29.0.tar", last modified: Fri Apr 19 15:14:25 2024, max compression
+gzip compressed data, was "kubemarine-0.30.0.tar", last modified: Tue May 14 11:54:02 2024, max compression
```

## Comparing `kubemarine-0.29.0.tar` & `kubemarine-0.30.0.tar`

### file list

```diff
@@ -1,276 +1,280 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-19 15:14:01.000000 kubemarine-0.29.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-19 15:14:01.000000 kubemarine-0.29.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14049 2024-04-19 15:14:25.860358 kubemarine-0.29.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9311 2024-04-19 15:14:01.000000 kubemarine-0.29.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.792358 kubemarine-0.29.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2024-04-19 15:14:01.000000 kubemarine-0.29.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2024-04-19 15:14:01.000000 kubemarine-0.29.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.800358 kubemarine-0.29.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7973 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    28959 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     5506 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     5517 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     6228 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.804358 kubemarine-0.29.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2043 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    29983 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4292 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    30924 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     7314 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    30562 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    21097 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    38592 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    15382 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)    24931 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    16671 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2185 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    26382 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7218 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     3373 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16782 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3892 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    27748 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4619 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10637 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2993 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     2347 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    12441 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    55462 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47459 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/components.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3993 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2162 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/secrets.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5967 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)     4007 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/modprobe.py
--rw-r--r--   0 root         (0) root         (0)    30835 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.808358 kubemarine-0.29.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1371 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/boot_timeout_per_node.py
--rw-r--r--   0 root         (0) root         (0)     1045 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/software_upgrade.yaml
--rw-r--r--   0 root         (0) root         (0)     1569 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/patches/strong_cipher_suits_for_kubelet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.812358 kubemarine-0.29.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    44984 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7859 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    29039 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     7916 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     7942 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    27778 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    19641 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.820358 kubemarine-0.29.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)     5796 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5874 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)   222019 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250597 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250781 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)   258410 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15642 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15662 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16337 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.824358 kubemarine-0.29.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)     3369 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    32557 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     3553 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    73258 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    90763 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/check_paas.py
--rw-r--r--   0 root         (0) root         (0)     2747 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/config.py
--rwxr-xr-x   0 root         (0) root         (0)     5004 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    23627 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1532 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)     8057 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    21667 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2435 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/reboot.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/reconfigure.py
--rwxr-xr-x   0 root         (0) root         (0)     3928 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    14178 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13025 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/procedures/upgrade.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.824358 kubemarine-0.29.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     4939 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     6152 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     5256 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     8015 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     4101 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    32236 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    11309 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.788358 kubemarine-0.29.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.828358 kubemarine-0.29.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.832358 kubemarine-0.29.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.832358 kubemarine-0.29.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2643 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1635 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3317 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.836358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)     1429 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      686 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     3679 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     3512 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.840358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     7227 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.840358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     3129 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3472 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.844358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1948 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     3115 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     5430 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
--rw-r--r--   0 root         (0) root         (0)      938 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     2764 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     5264 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4268 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1965 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.848358 kubemarine-0.29.0/kubemarine/resources/schemas/internal/
--rw-r--r--   0 root         (0) root         (0)     1343 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/internal/connections.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)     2326 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/reconfigure.json
--rw-r--r--   0 root         (0) root         (0)      872 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.852358 kubemarine-0.29.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3646 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/etcdctl.sh
--rwxr-xr-x   0 root         (0) root         (0)  2664799 2024-04-19 15:14:20.000000 kubemarine-0.29.0/kubemarine/resources/scripts/ipip_check.gz
--rw-r--r--   0 root         (0) root         (0)     1483 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_client.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.788358 kubemarine-0.29.0/kubemarine/resources/scripts/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.852358 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.mod
--rw-r--r--   0 root         (0) root         (0)     1446 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.sum
--rw-r--r--   0 root         (0) root         (0)     5732 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
--rw-r--r--   0 root         (0) root         (0)     8497 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     4073 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26293 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.856358 kubemarine-0.29.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2431 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      996 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.856358 kubemarine-0.29.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calico-typha-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      136 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    12104 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    19586 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     5696 2024-04-19 15:14:01.000000 kubemarine-0.29.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:14:25.860358 kubemarine-0.29.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14049 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10848 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-19 15:14:25.000000 kubemarine-0.29.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5790 2024-04-19 15:14:01.000000 kubemarine-0.29.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 15:14:25.860358 kubemarine-0.29.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2024-04-19 15:14:01.000000 kubemarine-0.29.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.586145 kubemarine-0.30.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-14 11:53:34.000000 kubemarine-0.30.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2024-05-14 11:53:34.000000 kubemarine-0.30.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14048 2024-05-14 11:54:02.586145 kubemarine-0.30.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9311 2024-05-14 11:53:34.000000 kubemarine-0.30.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.518144 kubemarine-0.30.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2024-05-14 11:53:34.000000 kubemarine-0.30.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2024-05-14 11:53:34.000000 kubemarine-0.30.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.526144 kubemarine-0.30.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7973 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    28959 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     6228 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.534144 kubemarine-0.30.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    30443 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    32010 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    30562 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    21097 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    38592 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/inventory.py
+-rw-r--r--   0 root         (0) root         (0)    15417 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8324 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/proxytypes.py
+-rw-r--r--   0 root         (0) root         (0)    24840 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    18631 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    26521 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.534144 kubemarine-0.30.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     3373 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16782 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3892 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    27748 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10637 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    12441 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.534144 kubemarine-0.30.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    55762 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47429 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/components.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5967 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     6997 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/modprobe.py
+-rw-r--r--   0 root         (0) root         (0)    32515 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.538145 kubemarine-0.30.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/patches/disable_unattended_upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     5093 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/patches/preserve_compatibility_kernel.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/patches/reinstall_etcdctl_thirdparty.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.538145 kubemarine-0.30.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    45094 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    29039 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     7916 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     7942 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    27778 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    19641 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.546145 kubemarine-0.30.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5874 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   222019 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250597 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250781 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   258410 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15642 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15662 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16337 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4643 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    32557 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     3553 2024-05-14 11:53:34.000000 kubemarine-0.30.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    75312 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    92640 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/check_paas.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     5004 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    23949 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1643 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1532 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)     8057 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    21667 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2435 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/reboot.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/reconfigure.py
+-rwxr-xr-x   0 root         (0) root         (0)     3928 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    14445 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    13348 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/procedures/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     4939 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     5256 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     8015 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    32996 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    11449 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.554145 kubemarine-0.30.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.514144 kubemarine-0.30.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.558145 kubemarine-0.30.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.558145 kubemarine-0.30.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.558145 kubemarine-0.30.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.562145 kubemarine-0.30.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.566145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.566145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     3679 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     3536 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/patch.json
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.566145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     7227 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.570145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.570145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.574145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     5430 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.574145 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4268 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.574145 kubemarine-0.30.0/kubemarine/resources/schemas/internal/
+-rw-r--r--   0 root         (0) root         (0)     1343 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/internal/connections.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/reconfigure.json
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.578145 kubemarine-0.30.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     4118 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/etcdctl.sh
+-rwxr-xr-x   0 root         (0) root         (0)  2666378 2024-05-14 11:53:57.000000 kubemarine-0.30.0/kubemarine/resources/scripts/ipip_check.gz
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/simple_port_client.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/simple_port_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.518144 kubemarine-0.30.0/kubemarine/resources/scripts/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.582145 kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/go.mod
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/go.sum
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
+-rw-r--r--   0 root         (0) root         (0)     8497 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)    10323 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26409 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.582145 kubemarine-0.30.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      996 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.582145 kubemarine-0.30.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.586145 kubemarine-0.30.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calico-typha-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    12104 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    19586 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     5696 2024-05-14 11:53:35.000000 kubemarine-0.30.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:54:02.586145 kubemarine-0.30.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14048 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11013 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 11:54:02.000000 kubemarine-0.30.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5789 2024-05-14 11:53:35.000000 kubemarine-0.30.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 11:54:02.586145 kubemarine-0.30.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-05-14 11:53:35.000000 kubemarine-0.30.0/setup.py
```

### Comparing `kubemarine-0.29.0/LICENSE` & `kubemarine-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/PKG-INFO` & `kubemarine-0.30.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.29.0
+Version: 0.30.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -27,15 +27,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.*
 Requires-Dist: deepmerge==1.1.*
 Requires-Dist: fabric==3.2.*
 Requires-Dist: jinja2==3.1.*
 Requires-Dist: MarkupSafe==2.1.*
 Requires-Dist: invoke==2.2.*
-Requires-Dist: ruamel.yaml==0.17.22
+Requires-Dist: ruamel.yaml==0.18.*
 Requires-Dist: pygelf==0.4.*
 Requires-Dist: toml==0.10.*
 Requires-Dist: python-dateutil==2.8.*
 Requires-Dist: deepdiff==6.7.*
 Requires-Dist: ordered-set==4.1.*
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: paramiko==3.3.*
@@ -63,38 +63,38 @@
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -112,15 +112,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -131,15 +131,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -160,24 +160,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -206,42 +206,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/LICENSE)
```

### Comparing `kubemarine-0.29.0/README.md` & `kubemarine-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/bin/kubemarine` & `kubemarine-0.30.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/bin/kubemarine.cmd` & `kubemarine-0.30.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/__init__.py` & `kubemarine-0.30.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/__main__.py` & `kubemarine-0.30.0/kubemarine/__main__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/admission.py` & `kubemarine-0.30.0/kubemarine/admission.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/apparmor.py` & `kubemarine-0.30.0/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/apt.py` & `kubemarine-0.30.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/audit.py` & `kubemarine-0.30.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/controlplane.py` & `kubemarine-0.30.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/__init__.py` & `kubemarine-0.30.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/action.py` & `kubemarine-0.30.0/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/annotations.py` & `kubemarine-0.30.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/cluster.py` & `kubemarine-0.30.0/kubemarine/core/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 @dataclasses.dataclass(repr=False)
 class _EnrichmentProducts:
     """States of inventory and context at the particular `EnrichmentStage` of enrichment."""
     inventory: dict
     context: Optional[dict]
     procedure_inventory: Optional[dict]
 
+    nodes_inventory: Dict[str, dict] = dataclasses.field(default_factory=dict)
     nodes: Dict[str, Dict[str, NodeGroup]] = dataclasses.field(default_factory=dict)
 
     formatted_inventory: Optional[dict] = None
     raw_inventory: Optional[dict] = None
 
 
 class KubernetesCluster(Environment):
@@ -305,14 +306,25 @@
         The resulting inventory describing the cluster.
 
         Should be changed only during the enrichment.
         """
         return self._products.inventory
 
     @property
+    def nodes_inventory(self) -> Dict[str, dict]:
+        """
+        The resulting inventory describing specific nodes.
+        The inventory can be derived from the main `inventory` only,
+        and should not depend on other sources of information.
+
+        Should be changed only during the enrichment.
+        """
+        return self._products.nodes_inventory
+
+    @property
     def context(self) -> dict:
         """
         Context that stores an intermediate enrichment and execution result.
 
         At DEFAULT stage, the context is available only during enrichment.
         """
         context = self._products.context
```

### Comparing `kubemarine-0.29.0/kubemarine/core/connections.py` & `kubemarine-0.30.0/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/defaults.py` & `kubemarine-0.30.0/kubemarine/core/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 import re
-from typing import Optional, Dict, Any, Tuple, List, Callable, Union
+from typing import Optional, Dict, Any, Tuple, List, Callable, Union, Sequence, cast, Type
 
 import yaml
 
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.errors import KME
 from kubemarine import jinja, keepalived, haproxy, controlplane, kubernetes, thirdparties
 from kubemarine.core import utils, static, log, os
+from kubemarine.core.proxytypes import Primitive, Index, Node
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.cri.containerd import contains_old_format_properties
 
 
 supported_connection_defaults = {
     'node_defaults': 'nodes',
 }
@@ -49,16 +51,14 @@
     'address', 'internal_address', 'connect_to',
     'name',  # In context of connections, the name is used only in logging. This dependency can potentially be avoided.
     'roles'  # Required to distinguish control planes to preserve inventory.
 ]
 
 
 invalid_node_name_regex = re.compile("[^a-z-.\\d]", re.M)
-escaped_expression_regex = re.compile('({%[\\s*|]raw[\\s*|]%}.*?{%[\\s*|]endraw[\\s*|]%})', re.M)
-jinja_query_regex = re.compile("{{ .* }}", re.M)
 
 
 @enrichment(EnrichmentStage.LIGHT, procedures=['add_node'])
 def add_node_enrich_roles(cluster: KubernetesCluster) -> None:
     # At LIGHT stage, we should mark the nodes with `add_node` service role to find them after compilation.
     # This is for optimization to avoid two-staged enrichment even for connections only.
     for node in cluster.procedure_inventory['nodes']:
@@ -465,103 +465,108 @@
     base_inventory = utils.deepcopy_yaml(base)
     inventory: dict = default_merger.merge(base_inventory, cluster.inventory)
     return inventory
 
 
 @enrichment(EnrichmentStage.LIGHT)
 def compile_connections(cluster: KubernetesCluster) -> None:
-    return _compile_inventory(cluster, inject_globals=False)
+    return _compile_inventory(cluster, light=True)
 
 
 @enrichment(EnrichmentStage.FULL)
 def compile_inventory(cluster: KubernetesCluster) -> None:
-    return _compile_inventory(cluster, inject_globals=True)
+    return _compile_inventory(cluster, light=False)
 
 
-def _compile_inventory(cluster: KubernetesCluster, *, inject_globals: bool) -> None:
+def _compile_inventory(cluster: KubernetesCluster, *, light: bool) -> None:
     inventory = cluster.inventory
-    # convert references in yaml to normal values
-    iterations = 100
-    root = utils.deepcopy_yaml(inventory)
-    if inject_globals:
-        root['globals'] = static.GLOBALS
-    root['env'] = os.Environ()
-
-    while iterations > 0:
-
-        cluster.log.verbose('Inventory is not rendered yet...')
-        inventory = compile_object(cluster.log, inventory, root)
-
-        temp_dump = yaml.dump(inventory)
-
-        # remove golang specific
-        temp_dump = re.sub(escaped_expression_regex, '', temp_dump.replace('\n', ''))
-
-        # it is necessary to carry out several iterations,
-        # in case we have dynamic variables that reference each other
-        if '{{' in temp_dump or '{%' in temp_dump:
-            iterations -= 1
-        else:
-            iterations = 0
 
-    compile_object(cluster.log, inventory, root, ignore_jinja_escapes=False)
+    extra: Dict[str, Any] = {'env': os.Environ()}
+    if not light:
+        extra['globals'] = static.GLOBALS
+
+    if light:
+        # Management of primitive values is currently not necessary for LIGHT stage.
+        env = Environment(cluster.log, inventory, recursive_compile=True, recursive_extra=extra)
+        jinja.compile_node(inventory, [], env)
+    else:
+        primitives_config = _get_primitive_values_registry()
+        env = Environment(cluster.log, inventory, recursive_compile=True, recursive_extra=extra,
+                          primitives_config=primitives_config)
+        compile_node_with_primitives(inventory, [], env, primitives_config)
+
+    remove_empty_items(inventory)
+
     dump_inventory(cluster, cluster.context, "cluster_precompiled.yaml")
 
 
 def dump_inventory(cluster: KubernetesCluster, context: dict, filename: str) -> None:
     if not utils.is_dump_allowed(context, filename):
         return
 
     inventory = utils.deepcopy_yaml(cluster.inventory)
     inventory_for_dump = controlplane.controlplane_finalize_inventory(cluster, inventory)
 
     data = yaml.dump(inventory_for_dump)
     utils.dump_file(context, data, filename)
 
 
-def compile_object(logger: log.EnhancedLogger, struct: Any, root: dict, ignore_jinja_escapes: bool = True) -> Any:
+PrimitivesConfig = List[Tuple[List[str], Callable[[Any], Any]]]
+
+
+def compile_node_with_primitives(struct: Union[list, dict],
+                                 path: List[Union[str, int]],
+                                 env: jinja.Environment,
+                                 primitives_config: PrimitivesConfig) -> Union[list, dict]:
     if isinstance(struct, list):
-        new_struct = []
         for i, v in enumerate(struct):
-            struct[i] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
-            # delete empty list entries, which can appear after jinja compilation
-            if struct[i] != '':
-                new_struct.append(struct[i])
-        struct = new_struct
-    elif isinstance(struct, dict):
+            struct[i] = compile_object_with_primitives(v, path, i, env, primitives_config)
+    else:
         for k, v in struct.items():
-            struct[k] = compile_object(logger, v, root, ignore_jinja_escapes=ignore_jinja_escapes)
-    elif isinstance(struct, str) and jinja.is_template(struct):
-        struct = compile_string(logger, struct, root, ignore_jinja_escapes=ignore_jinja_escapes)
+            struct[k] = compile_object_with_primitives(v, path, k, env, primitives_config)
 
     return struct
 
 
-def compile_string(logger: log.EnhancedLogger, struct: str, root: dict,
-                   ignore_jinja_escapes: bool = True) -> str:
-    logger.verbose("Rendering \"%s\"" % struct)
-
-    def precompile(struct: str) -> str:
-        return compile_string(logger, struct, root)
-
-    if ignore_jinja_escapes:
-        iterator = escaped_expression_regex.finditer(struct)
-        struct = re.sub(escaped_expression_regex, '', struct)
-        struct = jinja.new(logger, recursive_compiler=precompile, precompile_filters={
-            'kubernetes_version': kubernetes.verify_allowed_version
-        }).from_string(struct).render(**root)
-
-        # TODO this does not work for {raw}{jinja}{raw}{jinja}
-        for match in iterator:
-            span = match.span()
-            struct = struct[:span[0]] + match.group() + struct[span[0]:]
+def compile_object_with_primitives(struct: Union[Primitive, list, dict],
+                                   path: List[Index], index: Index,
+                                   env: jinja.Environment,
+                                   primitives_config: PrimitivesConfig) -> Union[Primitive, list, dict]:
+    depth = len(path)
+    primitives_config = choose_nested_primitives_config(primitives_config, depth, index)
+
+    path.append(index)
+    if isinstance(struct, (list, dict)):
+        if primitives_config:
+            struct = compile_node_with_primitives(struct, path, env, primitives_config)
+        else:
+            struct = jinja.compile_node(struct, path, env)
     else:
-        struct = jinja.new(logger, recursive_compiler=precompile).from_string(struct).render(**root)
+        if isinstance(struct, str) and jinja.is_template(struct):
+            struct = env.compile_string(struct, jinja.Path(path))
+
+        struct = convert_primitive(struct, path, primitives_config)
+
+    path.pop()
+    return struct
+
+
+def remove_empty_items(struct: Any) -> Any:
+    if isinstance(struct, list):
+        new_struct = []
+        for v in struct:
+            v = remove_empty_items(v)
+            # delete empty list entries, which can appear after jinja compilation
+            if v != '':
+                new_struct.append(v)
+        struct = new_struct
+    elif isinstance(struct, dict):
+        for k, v in struct.items():
+            struct[k] = remove_empty_items(v)
 
-    logger.verbose("\tRendered as \"%s\"" % struct)
     return struct
 
 
 def escape_jinja_characters_for_inventory(cluster: KubernetesCluster, obj: Any) -> Any:
     if isinstance(obj, dict):
         for key, value in obj.items():
             obj[key] = escape_jinja_characters_for_inventory(cluster, value)
@@ -570,125 +575,174 @@
             obj[key] = escape_jinja_characters_for_inventory(cluster, value)
     elif isinstance(obj, str):
         obj = _escape_jinja_character(obj)
     return obj
 
 
 def _escape_jinja_character(value: str) -> str:
-    if '{{' in value and '}}' in value and re.search(jinja_query_regex, value):
-        matches = re.findall(jinja_query_regex, value)
-        for match in matches:
-            # TODO: rewrite to correct way of match replacement: now it can cause "{raw}{raw}xxx.." circular bug
-            value = value.replace(match, '{% raw %}'+match+'{% endraw %}')
+    if jinja.is_template(value):
+        value = '{{ %s }}' % (json.JSONEncoder().encode(value),)
+
     return value
 
 
-def _get_primitive_values_registry() -> List[Tuple[List[str], Callable[[Any], Any], bool]]:
+def _get_primitive_values_registry() -> PrimitivesConfig:
     return [
         (['services', 'cri', 'containerdConfig',
           'plugins."io.containerd.grpc.v1.cri".containerd.runtimes.runc.options',
-          'SystemdCgroup'], utils.strtobool, False),
-        (['services', 'modprobe', '*', '*'], str, True),
+          'SystemdCgroup'], utils.strtobool),
+        (['services', 'modprobe', '*', '*', 'install'], utils.strtobool),
+        # kernel parameters are actually not always represented as integers
+        (['services', 'sysctl', '*', 'value'], utils.strtoint),
+        (['services', 'sysctl', '*', 'install'], utils.strtobool),
         # kernel parameters are actually not always represented as integers
-        (['services', 'sysctl', '*'], utils.strtoint, True),
-        (['plugins', '*', 'install'], utils.strtobool, False),
-        (['plugins', 'calico', 'typha', 'enabled'], utils.strtobool, False),
-        (['plugins', 'calico', 'typha', 'replicas'], utils.strtoint, False),
-        (['plugins', 'nginx-ingress-controller', 'ports', '*', 'hostPort'], utils.strtoint, False),
+        (['patches', '*', 'services', 'sysctl', '*', 'value'], utils.strtoint),
+        (['patches', '*', 'services', 'sysctl', '*', 'install'], utils.strtobool),
+        (['plugins', '*', 'install'], utils.strtobool),
+        (['plugins', 'calico', 'typha', 'enabled'], utils.strtobool),
+        (['plugins', 'calico', 'typha', 'replicas'], utils.strtoint),
+        (['plugins', 'nginx-ingress-controller', 'ports', '*', 'hostPort'], utils.strtoint),
     ]
 
 
-@enrichment(EnrichmentStage.FULL)
-def manage_primitive_values(cluster: KubernetesCluster) -> None:
-    paths_func_strip = _get_primitive_values_registry()
-    for search_path, func, strip in paths_func_strip:
-        _convert_primitive_values(cluster.inventory, [], search_path, func, strip)
+def choose_nested_primitives_config(primitives_config: PrimitivesConfig, depth: int, index: Index) -> PrimitivesConfig:
+    nested_config = []
+    for search in primitives_config:
+        search_path = search[0]
+        if depth == len(search_path):
+            continue
 
+        section = search_path[depth]
+        if section in ('*', index):
+            nested_config.append(search)
 
-def finalize_primitive_values(cluster: KubernetesCluster, inventory: dict) -> dict:
-    paths_func_strip = _get_primitive_values_registry()
-    for search_path, _, strip in paths_func_strip:
-        if not strip:
-            continue
-        _set_overridden_blank_primitive_values(cluster.raw_inventory, inventory, [], search_path)
-    return inventory
+    return nested_config
 
 
-def _convert_primitive_values(struct: Union[dict, list], path: List[Union[str, int]],
-                              search_path: List[str], func: Callable[[Any], Any], strip: bool) -> None:
-    depth = len(path)
-    section = search_path[depth]
-    if section == '*':
-        if isinstance(struct, list):
-            for i in reversed(range(len(struct))):
-                _convert_primitive_value_section(struct, i, path, search_path, func, strip)
-
-        elif isinstance(struct, dict):
-            for k in list(struct):
-                _convert_primitive_value_section(struct, k, path, search_path, func, strip)
-
-    # Only dict is possible here as struct
-    elif section in struct:
-        _convert_primitive_value_section(struct, section, path, search_path, func, strip)
-
-
-def _convert_primitive_value_section(struct: Union[dict, list], section: Union[str, int],
-                                     path: List[Union[str, int]],
-                                     search_path: List[str], func: Callable[[Any], Any], strip: bool) -> None:
-    value = struct[section]  # type: ignore[index]
-    path.append(section)
-    depth = len(path)
-    if depth < len(search_path):
-        _convert_primitive_values(value, path, search_path, func, strip)
-    else:
-        if strip and isinstance(value, str):
-            value = value.strip()
-        if strip and value == '':
-            del struct[section]  # type: ignore[arg-type]
-        else:
+def convert_primitive(struct: Primitive, path: Sequence[Index], primitives_config: PrimitivesConfig) -> Primitive:
+    for search_path, func in primitives_config:
+        if len(search_path) == len(path):
             try:
-                struct[section] = func(value)  # type: ignore[index]
+                struct = func(struct)
             except ValueError as e:
-                raise ValueError(f"{str(e)} in section [{']['.join(repr(p) for p in path)}]") from None
+                raise ValueError(f"{str(e)} in section {utils.pretty_path(path)}") from None
 
-    path.pop()
+    return struct
 
 
-def _set_overridden_blank_primitive_values(raw_struct: Union[dict, list], struct: Union[dict, list],
-                                           path: List[Union[str, int]],
-                                           search_path: List[str]) -> None:
-    depth = len(path)
-    section = search_path[depth]
-    if section == '*':
-        if isinstance(raw_struct, list):
-            for i in reversed(range(len(raw_struct))):
-                _set_overridden_blank_primitive_value_section(raw_struct, struct, i, path, search_path)
-
-        elif isinstance(raw_struct, dict):
-            for k in list(raw_struct):
-                _set_overridden_blank_primitive_value_section(raw_struct, struct, k, path, search_path)
-
-    # Only dict is possible here as raw_struct / struct
-    elif section in raw_struct:
-        _set_overridden_blank_primitive_value_section(raw_struct, struct, section, path, search_path)
-
-
-def _set_overridden_blank_primitive_value_section(raw_struct: Union[dict, list], struct: Union[dict, list],
-                                                  section: Union[str, int], path: List[Union[str, int]],
-                                                  search_path: List[str]) -> None:
-    raw_value = raw_struct[section]  # type: ignore[index]
-    path.append(section)
-    depth = len(path)
-    if depth < len(search_path):
-        # Items can be deleted only in leafs, so it is safe to get nested struct by key.
-        # See _convert_primitive_value_section()
-        value = struct[section]  # type: ignore[index]
-        _set_overridden_blank_primitive_values(raw_value, value, path, search_path)
-    elif isinstance(struct, dict) and section not in struct:
-        # Leaves can be stripped and deleted during enrichment.
-        # If they were redefined in raw inventory, we should return blank string in finalized inventory.
-        # If finalized inventory is used as a source inventory, it will again redefine defaults with blank strings,
-        # that will be again deleted.
-        # See _convert_primitive_value_section()
-        struct[section] = ''
+class NodePrimitives(jinja.JinjaNode):
+    """
+    A Node that both compiles template strings and converts primitive values in the underlying `dict` or `list`.
+    """
 
-    path.pop()
+    def __init__(self, delegate: Union[dict, list], *,
+                 path: jinja.Path, env: jinja.Environment,
+                 primitives_config: PrimitivesConfig):
+        super().__init__(delegate, path=path, env=env)
+        self.primitives_config = primitives_config
+
+    def _child(self, index: Index, val: Union[list, dict]) -> jinja.Node:
+        primitives_config = self._nested_primitives_config(index)
+        return self._child_type(index)(val, path=self.path + (index,), env=self.env,
+                                       primitives_config=primitives_config)
+
+    def _child_type(self, _: Index) -> Type['NodePrimitives']:
+        return NodePrimitives
+
+    def _convert(self, index: Index, val: Primitive) -> Primitive:
+        val = super()._convert(index, val)
+
+        primitives_config = self._nested_primitives_config(index)
+        val = convert_primitive(val, self.path + (index,), primitives_config)
+
+        return val
+
+    def _nested_primitives_config(self, index: Index) -> PrimitivesConfig:
+        depth = len(self.path)
+        return choose_nested_primitives_config(self.primitives_config, depth, index)
+
+
+class NodesCustomization:
+    """
+    Customize access to the particular sections of the inventory.
+    """
+
+    # pylint: disable=no-self-argument
+
+    def __init__(nodes) -> None:
+        # The classes below should customize access to the sections of the inventory,
+        # while preserving the global behaviour of Node implementations: NodePrimitives, JinjaNode, Node.
+
+        class Kubeadm(Node):
+            def descend(self, index: Index) -> Union[Primitive, Node]:
+                child: Union[Primitive, Node] = super().descend(index)
+
+                if index == 'kubernetesVersion':
+                    kubernetes.verify_allowed_version(cast(str, child))
+
+                return child
+
+        class Services(Node):
+            def _child_type(self, index: Index) -> Type[Node]:
+                if index == 'kubeadm':
+                    return nodes.Kubeadm
+
+                return super()._child_type(index)
+
+        class Root(Node):
+            def _child_type(self, index: Index) -> Type[Node]:
+                if index == 'services':
+                    return nodes.Services
+
+                return super()._child_type(index)
+
+        nodes.Kubeadm: Type[Node] = Kubeadm
+        nodes.Services: Type[Node] = Services
+        nodes.Root: Type[Node] = Root
+
+    def derive(nodes, Base: Type[Node], delegate: dict, **kwargs: Any) -> Node:
+        nodes.Kubeadm = cast(Type[Node], type("Kubeadm", (nodes.Kubeadm, Base), {}))
+        nodes.Services = cast(Type[Node], type("Services", (nodes.Services, Base), {}))
+        nodes.Root = cast(Type[Node], type("Root", (nodes.Root, Base), {}))
+
+        return nodes.Root(delegate, **kwargs)
+
+
+class Environment(jinja.Environment):
+    """
+    Environment that supports recursive compilation and on-the-fly conversion of primitive values.
+
+    It also customizes access to the particular sections of the inventory.
+    """
+
+    def __init__(self, logger: log.EnhancedLogger, recursive_values: dict,
+                 *,
+                 recursive_compile: bool = False,
+                 recursive_extra: Dict[str, Any] = None,
+                 primitives_config: PrimitivesConfig = None):
+        """
+        Instantiate new environment and set default filters.
+
+        :param logger: EnhancedLogger
+        :param recursive_values: The render values access to which should be customized.
+                                 They may also be automatically converted and compiled if necessary.
+        :param recursive_compile: Flag that enables recursive compilation.
+        :param recursive_extra: If recursive compilation occurs, these render values are supplied to the template.
+        :param primitives_config: List of sections and convertors of primitive values.
+        """
+        self.recursive_compile = recursive_compile
+        self.primitives_config = primitives_config
+        super().__init__(logger, recursive_values, recursive_extra=recursive_extra)
+
+    def create_root(self, delegate: dict) -> Node:
+        kwargs = {}
+        Base: Type[Node]
+        if not self.recursive_compile:
+            Base = Node
+        else:
+            Base = jinja.JinjaNode
+            kwargs = {"path": jinja.Path(), "env": self}
+            if self.primitives_config is not None:
+                Base = NodePrimitives
+                kwargs = {**kwargs, "primitives_config": self.primitives_config}
+
+        return NodesCustomization().derive(Base, delegate, **kwargs)
```

### Comparing `kubemarine-0.29.0/kubemarine/core/environment.py` & `kubemarine-0.30.0/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/errors.py` & `kubemarine-0.30.0/kubemarine/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     "in cluster.yaml{previous_version_spec}, "
                     "but not present in procedure inventory{next_version_spec}. "
                     "Please, specify required 'sandbox_image' explicitly in procedure inventory."
         }
     }
 
 
-class _BaseKME(RuntimeError, ABC):
+class BaseKME(RuntimeError, ABC):
     def __init__(self, code: str):
         self.code = code
         if self.code not in get_kme_dictionary():
             raise ValueError('An error was raised with an unknown error code')
         self.kme: dict = get_kme_dictionary()[self.code]
         self.message = self._format()
         super().__init__(self.message)
@@ -101,28 +101,28 @@
     @abstractmethod
     def _format(self) -> str: ...
 
     def __str__(self) -> str:
         return self.code + ": " + self.message
 
 
-class KME(_BaseKME):
+class KME(BaseKME):
     def __init__(self, code: str, **kwargs: object):
         self.kwargs = kwargs
         super().__init__(code)
 
     def _format(self) -> str:
         if 'name' not in self.kme:
             raise ValueError('An error was raised with an unsupported error code')
 
         name: str = self.kme['name']
         return name.format_map(self.kwargs)
 
 
-class KME0006(_BaseKME):
+class KME0006(BaseKME):
     def __init__(self, offline: List[str], inaccessible: List[str]):
         self.offline = offline
         self.inaccessible = inaccessible
         self.summary = ""
         self.details = ""
         super().__init__("KME0006")
 
@@ -175,15 +175,15 @@
         error_logger(message)
 
     if reason is None:
         return
 
     reason = wrap_kme_exception(reason)
 
-    if isinstance(reason, _BaseKME):
+    if isinstance(reason, BaseKME):
         error_logger(reason)
         return
 
     if log:
         log.critical('KME0001: Unexpected exception', exc_info=reason)
     else:
         sys.stderr.write("KME0001: Unexpected exception\n")
```

### Comparing `kubemarine-0.29.0/kubemarine/core/executor.py` & `kubemarine-0.30.0/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/flow.py` & `kubemarine-0.30.0/kubemarine/core/flow.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/group.py` & `kubemarine-0.30.0/kubemarine/core/group.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/log.py` & `kubemarine-0.30.0/kubemarine/core/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,22 +192,22 @@
 
     def __init__(self,
                  target: str,
                  level: str,
                  colorize: bool = False,
                  correct_newlines: bool = False,
                  filemode: str = 'a',
-                 format_: str = DEFAULT_FORMAT,
+                 format: str = DEFAULT_FORMAT,  # pylint: disable=redefined-builtin
                  datefmt: str = None,
                  header: str = None,
                  **kwargs: Union[str, bool, int]):
 
         self._colorize = colorize
         self._correct_newlines = correct_newlines
-        self._format = format_
+        self._format = format
         self._datefmt = datefmt
         self._header = header
 
         self._formatter = LogFormatter(self._format, self._datefmt,
                                        colorize=self._colorize,
                                        correct_newlines=self._correct_newlines)
```

### Comparing `kubemarine-0.29.0/kubemarine/core/os.py` & `kubemarine-0.30.0/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/patch.py` & `kubemarine-0.30.0/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/resources.py` & `kubemarine-0.30.0/kubemarine/core/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import ruamel.yaml
 
 import kubemarine.admission
 import kubemarine.audit
 import kubemarine.controlplane
 import kubemarine.core.cluster
 import kubemarine.core.defaults
+import kubemarine.core.inventory
 import kubemarine.core.schema
 import kubemarine.cri
 import kubemarine.cri.containerd
 import kubemarine.haproxy
 import kubemarine.k8s_certs
 import kubemarine.keepalived
 import kubemarine.kubernetes
@@ -37,14 +38,15 @@
 import kubemarine.packages
 import kubemarine.plugins
 import kubemarine.plugins.builtin
 import kubemarine.plugins.calico
 import kubemarine.plugins.kubernetes_dashboard
 import kubemarine.plugins.local_path_provisioner
 import kubemarine.plugins.nginx_ingress
+import kubemarine.sysctl
 import kubemarine.system
 import kubemarine.thirdparties
 
 from kubemarine.core import cluster as c  # pylint: disable=reimported
 from kubemarine.core import utils, log, errors, static
 from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.yaml_merger import default_merger
@@ -427,18 +429,14 @@
             kubemarine.core.defaults.calculate_connect_to,
             kubemarine.core.defaults.verify_nodes,
             kubemarine.core.defaults.apply_connection_defaults,
             kubemarine.core.defaults.calculate_nodegroups,
             kubemarine.core.defaults.remove_service_roles,
             # Enrichment of inventory for LIGHT stage should be finished at this step.
 
-            # Should be just after compilation, but currently not necessary for LIGHT stage.
-            # Sections with primitive values may be potentially split in the future if necessary for LIGHT.
-            kubemarine.core.defaults.manage_primitive_values,
-
             # Validation of procedure inventory enrichment after compilation
             kubemarine.kubernetes.verify_version,
             kubemarine.admission.verify_manage_enrichment,
             kubemarine.k8s_certs.renew_verify,
             kubemarine.plugins.nginx_ingress.verify_cert_renew,
             # The functions below depend on kubemarine.kubernetes.verify_version
             kubemarine.kubernetes.verify_upgrade_inventory,
@@ -446,22 +444,26 @@
             kubemarine.packages.verify_procedure_inventory,
             kubemarine.plugins.verify_upgrade_inventory,
             kubemarine.thirdparties.verify_procedure_inventory,
             kubemarine.cri.verify_upgrade_inventory,
 
             # Remained default enrichment.
             # Many functions depend on kubemarine.core.defaults.calculate_nodegroups
+            kubemarine.core.inventory.verify_inventory_patches,
             kubemarine.core.defaults.apply_defaults,
             kubemarine.packages.enrich_inventory,
             kubemarine.core.defaults.apply_registry,
+            kubemarine.sysctl.enrich_inventory,
             kubemarine.keepalived.enrich_inventory_apply_defaults,
             kubemarine.keepalived.enrich_inventory_calculate_nodegroup,
             # Depends on kubemarine.keepalived.enrich_inventory_apply_defaults
             kubemarine.haproxy.enrich_inventory,
-            # Depends on kubemarine.core.defaults.apply_registry
+            # Depends on
+            # * kubemarine.core.defaults.apply_registry
+            # * kubemarine.sysctl.enrich_inventory
             kubemarine.kubernetes.enrich_inventory,
             kubemarine.admission.enrich_inventory,
             # Depends on kubemarine.core.defaults.apply_defaults
             kubemarine.kubernetes_accounts.enrich_inventory,
             # Depends on kubemarine.kubernetes.enrich_inventory
             kubemarine.cri.enrich_inventory,
             # Depends on kubemarine.core.defaults.apply_registry
@@ -492,15 +494,14 @@
             c.enrichment(c.EnrichmentStage.LIGHT)(kubemarine.core.cluster.KubernetesCluster.check_nodes_accessibility),
         ]
 
     def finalization_functions(self) -> List[Callable[[c.KubernetesCluster, dict], dict]]:
         return [
             kubemarine.packages.cache_package_versions,
             kubemarine.core.defaults.escape_jinja_characters_for_inventory,
-            kubemarine.core.defaults.finalize_primitive_values,
             kubemarine.controlplane.controlplane_finalize_inventory,
         ]
 
     def _choose_enrichment_functions(self, stage: c.EnrichmentStage) -> List[c.EnrichmentFunction]:
         procedure = self.context['initial_procedure']
         enrichment_fns = self.enrichment_functions()
         return [fn for fn in enrichment_fns
```

### Comparing `kubemarine-0.29.0/kubemarine/core/schema.py` & `kubemarine-0.30.0/kubemarine/core/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import pathlib
 from collections.abc import Hashable
 from textwrap import dedent
-from typing import List, Dict, Callable, Union, Sequence
+from typing import List, Dict, Callable, Union, cast
 
 import jsonschema
 from ordered_set import OrderedSet
 
 from kubemarine.core import utils, log, errors
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 
@@ -129,14 +129,15 @@
     # jsonschema might show not very friendly messages for anyOf / oneOf.
     # In case of failed type or enum validation in each subschema, we can unnest the error to the higher level.
     # Note that possible remaining subschema errors will be discarded,
     # but it is acceptable for our current schemas implementation.
     subschemas_errors = list(errors_by_subschema.values())
     _unnest_type_subschema_errors(error, subschemas_errors)
     _unnest_enum_subschema_errors(error, subschemas_errors)
+    _unnest_required_subschema_errors(error, subschemas_errors)
 
 
 def _descend_errors(error: jsonschema.ValidationError) -> List[jsonschema.ValidationError]:
     if not error.context:
         return [error]
 
     # Here can be anyOf or oneOf with all not valid subschemas.
@@ -182,15 +183,15 @@
         for child in errs:
             if _validated_by(child, "type") and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["type"]:
                 value = child.validator_value
                 expected_types.update([value] if isinstance(value, str) else value)
                 break
         else:  # not found error with "type" validation failed for root instance.
             break
-    else:  # not found subschema not containing the necessary error, i. e. all subschemas has necessary error
+    else:  # not found subschema not containing the necessary error, i.e. all subschemas have necessary error
         reprs = ", ".join(repr(type) for type in expected_types)
         for child in error.context:
             child.parent = None
         error.context = []
         error.validator = "type"  # type: ignore[assignment]
         error.validator_value = list(expected_types)
         error.schema_path[-1] = "type"
@@ -207,25 +208,67 @@
     for errs in subschemas_errors:
         for child in errs:
             if _validated_by(child, "enum") and len(child.relative_path) == 0 and list(child.schema_path)[1:] == ["enum"]:
                 expected_elems.update(child.validator_value)
                 break
         else:  # not found error with "enum" validation failed for root instance.
             break
-    else:  # not found subschema not containing the necessary error, i. e. all subschemas has necessary error
+    else:  # not found subschema not containing the necessary error, i.e. all subschemas have necessary error
         for child in error.context:
             child.parent = None
         error.context = []
         error.validator = "enum"  # type: ignore[assignment]
         error.validator_value = list(expected_elems)
         error.schema_path[-1] = "enum"
         error.message = f"{error.instance!r} is not one of {list(expected_elems)!r}"
         subschemas_errors.clear()
 
 
+def _unnest_required_subschema_errors(error: jsonschema.ValidationError,
+                                      subschemas_errors: List[List[jsonschema.ValidationError]]) -> None:
+    if not error.context:
+        return
+
+    required_sets: List[List[str]] = []
+    for errs in subschemas_errors:
+        if len(errs) > 1:
+            # Support only the case when all subschema failed with the only 'required' validation.
+            # This is a common pattern if "at least one property from the set is required" requirement
+            # is moved to the separate "allOf (anyOf (required prop1, required prop2)) subschema.
+            break
+        for child in errs:
+            if (_validated_by(child, "required") and len(child.relative_path) == 0
+                    and list(child.schema_path)[1:] == ["required"] and len(child.validator_value) > 0
+                    and child.validator_value != ['<<']):
+                if isinstance(child.validator_value[0], str):
+                    required_sets.append(child.validator_value)
+                else:
+                    required_sets.extend(child.validator_value)
+                break
+        else:  # not found error with "required" validation failed for root instance.
+            break
+    # not found subschema not containing the only necessary error,
+    # i.e. all subschemas have the only necessary error
+    else:
+        initial_validator = cast(str, error.validator)
+
+        for child in error.context:
+            child.parent = None
+
+        error.context = []
+        error.validator = "required"  # type: ignore[assignment]
+        # This breaks original typing.
+        # Access to the validator_value should always be guarded with extra isinstance() checks.
+        error.validator_value = required_sets
+        error.schema_path[-1] = "required"
+        error.message = (f"{'One' if initial_validator == 'oneOf' else 'At least one'} "
+                         f"of the following property sets is required: {', '.join(map(str, required_sets))}")
+        subschemas_errors.clear()
+
+
 def _extended_relevance() -> Callable[[jsonschema.ValidationError], tuple]:
     # The extended relevance function is intended to improve heuristic for oneOf|anyOf,
     # when it is necessary to choose the most suitable branch.
 
     def relevance(error: jsonschema.ValidationError) -> tuple:
         relevance_value: tuple = jsonschema.exceptions.relevance(error)  # type: ignore[assignment]
         if error.parent is None:
@@ -268,15 +311,15 @@
 
 
 def _apply_required_and_optional_properties_heuristic(error: jsonschema.ValidationError,
                                                       relevance_value: tuple) -> tuple:
     # Resolve oneOf|anyOf(object, object) ambiguity.
     # Currently only 'registry' section has such schema.
     # The chosen priority is:
-    # 1. If all required properties are present, than the error has lower relevance.
+    # 1. If all required properties are present, then the error has lower relevance.
     # 2. Otherwise, calculate proportion of matched properties.
 
     # By default, consider all required properties are present, and no properties are matched
     coeff: list = [False, 0]
     if len(error.relative_path) != 0 or not isinstance(error.schema, dict) or not isinstance(error.instance, dict):
         return _append_relevance_element(relevance_value, tuple(coeff))
 
@@ -297,27 +340,27 @@
     return tuple(mutate_relevance)
 
 
 def _error_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
     return dedent(
         f"""\
         {_friendly_msg(validator, error)}
-        On inventory{_convert_to_indices(error.absolute_path)}
+        On inventory{utils.pretty_path(error.absolute_path)}
         """.rstrip()
     )
 
 
 def _verbose_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
-    schema_path = _convert_to_indices(list(error.absolute_schema_path)[:-1])
+    schema_path = utils.pretty_path(list(error.absolute_schema_path)[:-1])
     return dedent(
         f"""\
         {_friendly_msg(validator, error)}
         
         Failed validating {error.validator!r} in {schema_path}
-        On inventory{_convert_to_indices(error.absolute_path)}
+        On inventory{utils.pretty_path(error.absolute_path)}
         """.rstrip()
     )
 
 
 def _friendly_msg(validator: jsonschema.Draft7Validator, error: jsonschema.ValidationError) -> str:
     # pylint: disable=too-many-return-statements
 
@@ -358,13 +401,7 @@
             return f"Property name {error.instance!r} is not one of {error.validator_value!r}"
 
     return error.message
 
 
 def _validated_by(error: jsonschema.ValidationError, expected: str) -> bool:
     return error.validator == expected  # type: ignore[comparison-overlap]
-
-
-def _convert_to_indices(path: Sequence[Union[str, int]]) -> str:
-    if not path:
-        return ""
-    return f"[{']['.join(repr(p) for p in path)}]"
```

### Comparing `kubemarine-0.29.0/kubemarine/core/static.py` & `kubemarine-0.30.0/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/summary.py` & `kubemarine-0.30.0/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/core/utils.py` & `kubemarine-0.30.0/kubemarine/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,14 +460,20 @@
         with open_utf8(filepath, 'r') as stream:
             data: dict = yaml.safe_load(stream)
             return data
     except yaml.YAMLError as exc:
         do_fail(f"Failed to load {filepath}", exc)
 
 
+def pretty_path(path: Sequence[Union[str, int]]) -> str:
+    if not path:
+        return ""
+    return f"[{']['.join(map(repr, path))}]"
+
+
 def strtobool(value: Union[str, bool]) -> bool:
     """
     The method check string and boolean value
     :param value: Value that should be checked
     """
     val = str(value).lower()
     if val in ('y', 'yes', 't', 'true', 'on', '1'):
```

### Comparing `kubemarine-0.29.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.30.0/kubemarine/core/yaml_merger.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,34 +7,41 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Tuple, Optional
 
 from deepmerge import Merger  # type: ignore[import-untyped]
 
 
-def is_list_extends(nxt: list) -> bool:
-    return any({'<<': 'merge'} == v for i, v in enumerate(nxt))
+def is_list_extends(nxt: list, path: list) -> bool:
+    return get_strategy_position(nxt, path)[0] == 'merge'
 
 
-def list_merger(_: Merger, path: list, base: list, nxt: list) -> list:
+def get_strategy_position(nxt: list, path: list) -> Tuple[Optional[str], int]:
     strategy = None
     strategy_definition_position = 0
     for i, v in enumerate(nxt):
         if isinstance(v, dict) and '<<' in v:
             if strategy is not None:
                 raise Exception(f"Found more than one merge strategy definitions at path {path}.")
             strategy = v.get('<<')
             strategy_definition_position = i
             if v.keys() != {'<<'} or strategy not in ('replace', 'merge'):
                 raise Exception(f"Unexpected merge strategy definition {v} at path {path}.")
 
+    return strategy, strategy_definition_position
+
+
+def list_merger(_: Merger, path: list, base: list, nxt: list) -> list:
+    strategy, strategy_definition_position = get_strategy_position(nxt, path)
+
     if strategy is None:
         return nxt
 
     elements_after = nxt[(strategy_definition_position + 1):]
     elements_before = nxt[:strategy_definition_position]
     # do not modify source list
     nxt = []
```

### Comparing `kubemarine-0.29.0/kubemarine/coredns.py` & `kubemarine-0.30.0/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/cri/__init__.py` & `kubemarine-0.30.0/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/cri/containerd.py` & `kubemarine-0.30.0/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/cri/docker.py` & `kubemarine-0.30.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/demo.py` & `kubemarine-0.30.0/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/etcd.py` & `kubemarine-0.30.0/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/haproxy.py` & `kubemarine-0.30.0/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/k8s_certs.py` & `kubemarine-0.30.0/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/keepalived.py` & `kubemarine-0.30.0/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.30.0/kubemarine/kubernetes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import time
 from contextlib import contextmanager
 from typing import List, Dict, Iterator, Any, Optional
 
 import yaml
 from jinja2 import Template
 
-from kubemarine import system, admission, etcd, packages, jinja
+from kubemarine import system, admission, etcd, packages, jinja, sysctl
 from kubemarine.core import utils, static, summary, log, errors
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.executor import Token
 from kubemarine.core.group import NodeGroup, DeferredGroup, RunnersGroupResult, CollectorCallback
 from kubemarine.core.errors import KME
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.cri import containerd
@@ -40,14 +40,16 @@
 
 ERROR_KUBELET_PATCH_NOT_KUBERNETES_NODE = "%s patch can be uploaded only to control-plane or worker nodes"
 ERROR_CONTROL_PLANE_PATCH_NOT_CONTROL_PLANE_NODE = "%s patch can be uploaded only to control-plane nodes"
 ERROR_KUBEADM_DOES_NOT_SUPPORT_PATCHES_KUBELET = "Patches for kubelet are not supported in Kubernetes {version}"
 
 ERROR_UPGRADE_UNEXPECTED_PROPERTY='Unexpected %s properties in the procedure inventory for upgrade.'
 
+ERROR_AMBIGUOUS_CONNTRACK_MAX = "Detected ambiguous 'net.netfilter.nf_conntrack_max' value: {values}"
+
 
 @enrichment(EnrichmentStage.PROCEDURE, procedures=['upgrade'])
 def enrich_upgrade_inventory(cluster: KubernetesCluster) -> None:
     procedure_inventory = cluster.procedure_inventory
     allowed_properties = {
         'upgrade_plan', 'upgrade_nodes', 'disable-eviction', 'prepull_group_size', 'grace_period', 'drain_timeout'
     }
@@ -179,19 +181,32 @@
     # check ignorePreflightErrors value and add mandatory errors from defaults.yaml if they're absent
     default_preflight_errors = static.DEFAULTS["services"]["kubeadm_flags"]["ignorePreflightErrors"].split(",")
     preflight_errors = inventory["services"]["kubeadm_flags"]["ignorePreflightErrors"].split(",")
 
     preflight_errors.extend(default_preflight_errors)
     inventory["services"]["kubeadm_flags"]["ignorePreflightErrors"] = ",".join(set(preflight_errors))
 
+    enrich_kube_proxy(cluster)
+
+
+def enrich_kube_proxy(cluster: KubernetesCluster) -> None:
+    inventory = cluster.inventory
+
     # override kubeadm_kube-proxy.conntrack.min with sysctl.net.netfilter.nf_conntrack_max
     # since they define the same kernel variable
-    version_key = utils.version_key(inventory["services"]["kubeadm"]["kubernetesVersion"])
-    conntrack_max = inventory["services"]["sysctl"].get("net.netfilter.nf_conntrack_max")
-    if version_key >= (1, 29, 0) and conntrack_max is not None:
+    kubernetes_nodes = cluster.make_group_from_roles(['control-plane', 'worker'])
+    conntrack_max_values = {
+        sysctl.get_parameter(cluster, node, 'net.netfilter.nf_conntrack_max')
+        for node in kubernetes_nodes.get_ordered_members_list()}
+
+    if len(conntrack_max_values) > 1:
+        raise Exception(ERROR_AMBIGUOUS_CONNTRACK_MAX.format(values=conntrack_max_values))
+
+    conntrack_max = next(iter(conntrack_max_values), None)
+    if components.kube_proxy_overwrites_higher_system_values(cluster) and conntrack_max is not None:
         inventory["services"]["kubeadm_kube-proxy"]["conntrack"]["min"] = conntrack_max
     else:
         inventory["services"]["kubeadm_kube-proxy"]["conntrack"].pop("min",None)
 
 
 def reset_installation_env(group: NodeGroup) -> Optional[RunnersGroupResult]:
     log = group.cluster.log
@@ -708,18 +723,14 @@
     first_control_plane.sudo(
         f"sudo kubeadm upgrade apply {version} {flags} && "
         f"sudo kubectl uncordon {node_name} && "
         f"sudo systemctl restart kubelet", hide=False)
 
     copy_admin_config(cluster.log, first_control_plane)
 
-    # In some versions, kubeadm reverts resolvConf to the default during `upgrade apply`
-    # Remove default resolvConf from kubelet-config ConfigMap for debian OS family
-    first_control_plane.call(components.patch_kubelet_configmap)
-
     expect_kubernetes_version(cluster, version, apply_filter=node_name)
     components.wait_for_pods(first_control_plane)
     exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
 def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs: Any) -> None:
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
```

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/components.py` & `kubemarine-0.30.0/kubemarine/kubernetes/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import re
 from textwrap import dedent
-from typing import List, Optional, Dict, Callable, Sequence
+from typing import List, Optional, Dict, Callable, Sequence, Union
 
 import yaml
 from jinja2 import Template
 from ordered_set import OrderedSet
 
 from kubemarine import plugins, system
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
-from kubemarine.core.group import NodeConfig, NodeGroup, DeferredGroup, CollectorCallback, AbstractGroup, RunResult
+from kubemarine.core.group import NodeGroup, DeferredGroup, CollectorCallback, AbstractGroup, RunResult
 from kubemarine.core.yaml_merger import override_merger
 from kubemarine.kubernetes.object import KubernetesObject
 
 ERROR_WAIT_FOR_PODS_NOT_SUPPORTED = "Waiting for pods of {components} components is currently not supported"
 ERROR_RESTART_NOT_SUPPORTED = "Restart of {components} components is currently not supported"
 ERROR_RECONFIGURE_NOT_SUPPORTED = "Reconfiguration of {components} components is currently not supported"
 
@@ -1089,22 +1089,24 @@
     for component in components:
         defer.sudo(restart_pod.format(pod=component, node=node_name))
 
     defer.flush()
 
 
 # function to get dictionary of flags to be patched for a given control plane item and a given node
-def _get_patched_flags_for_section(inventory: dict, patch_section: str, node: NodeConfig) -> Dict[str, str]:
+def get_patched_flags_for_section(cluster: KubernetesCluster,
+                                  patch_section: str, group: AbstractGroup[RunResult]) -> Dict[str, Union[str, bool, int]]:
+    node = group.get_config()
     flags = {}
 
-    for n in inventory['services']['kubeadm_patches'][patch_section]:
-        if n.get('groups') is not None and list(set(node['roles']) & set(n['groups'])):
-            for arg, value in n['patch'].items():
-                flags[arg] = value
-        if n.get('nodes') is not None and node['name'] in n['nodes']:
+    for n in cluster.inventory['services']['kubeadm_patches'][patch_section]:
+        group = cluster.create_group_from_groups_nodes_names(
+            n.get('groups', []), n.get('nodes', []))
+
+        if group.has_node(node['name']):
             for arg, value in n['patch'].items():
                 flags[arg] = value
 
     # we always set binding-address to the node's internal address for apiServer
     if patch_section == 'apiServer' and 'control-plane' in node['roles']:
         flags['bind-address'] = node['internal_address']
 
@@ -1120,16 +1122,15 @@
     if backup_dir is not None:
         node.sudo(f'{component_patches} -exec cp {{}} {backup_dir}/patches \\;')
 
     if reset:
         node.sudo(f'{component_patches} -delete')
 
     # read patch content from inventory and upload patch files to a node
-    node_config = node.get_config()
-    patched_flags = _get_patched_flags_for_section(cluster.inventory, patch_constants['section'], node_config)
+    patched_flags = get_patched_flags_for_section(cluster, patch_constants['section'], node)
     if patched_flags:
         if component == 'kubelet':
             template_filename = 'templates/patches/kubelet.yaml.j2'
         else:
             template_filename = 'templates/patches/control-plane-pod.json.j2'
 
         control_plane_patch = Template(utils.read_internal(template_filename)).render(flags=patched_flags)
```

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.30.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.30.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/object.py` & `kubemarine-0.30.0/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.30.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/secrets.py` & `kubemarine-0.30.0/kubemarine/kubernetes/secrets.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.30.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.30.0/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/packages.py` & `kubemarine-0.30.0/kubemarine/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
 from typing import List, Dict, Tuple, Optional, Union, Mapping, Set
-
+from io import StringIO
 from typing_extensions import Protocol
 
 from kubemarine import yum, apt, jinja
 from kubemarine.core import errors, static, utils
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage, enrichment
 from kubemarine.core.executor import RunnersResult, Token, Callback
 from kubemarine.core.group import (
@@ -373,32 +373,47 @@
 
     if association_name in ('docker', 'containerd') \
             and association_name != inventory['services']['cri']['containerRuntime']:
         relevant_group = cluster.make_group([])
 
     relevant_group = relevant_group.intersection_group(group)
 
-    global_cache_versions = packages_section['cache_versions']
     for node in relevant_group.get_ordered_members_list():
         os_family = node.get_nodes_os()
-        package_associations = packages_section['associations'].get(os_family, {}).get(association_name, {})
-        packages = package_associations.get('package_name', [])
-
-        if isinstance(packages, str):
-            packages = [packages]
+        packages = get_association_packages(cluster, os_family, association_name)
 
-        if ensured_association_only and not (global_cache_versions and package_associations.get('cache_versions', True)):
+        if ensured_association_only and not cache_versions_enabled(cluster, os_family, association_name):
             packages = []
 
         if packages:
             hosts_to_packages[node.get_host()] = packages
 
     return hosts_to_packages
 
 
+def get_association_packages(cluster: KubernetesCluster, os_family: str, association_name: str) -> List[str]:
+    packages_section = cluster.inventory['services']['packages']
+    package_associations = packages_section['associations'].get(os_family, {}).get(association_name, {})
+    packages: Union[str, List[str]] = package_associations.get('package_name', [])
+
+    if isinstance(packages, str):
+        packages = [packages]
+
+    return packages
+
+
+def cache_versions_enabled(cluster: KubernetesCluster, os_family: str, association_name: str) -> bool:
+    packages_section = cluster.inventory['services']['packages']
+    global_cache_versions = packages_section['cache_versions']
+    specific_cache_versions: bool = packages_section['associations'] \
+        .get(os_family, {}).get(association_name, {}).get('cache_versions', True)
+
+    return global_cache_versions and specific_cache_versions
+
+
 def _cache_package_associations(group: NodeGroup, inventory: dict,
                                 detected_packages: Dict[str, Dict[str, List]], ensured_association_only: bool) -> None:
     cluster: KubernetesCluster = group.cluster
     associations = inventory['services']['packages']['associations'][cluster.get_os_family()]
     for association_name, associated_params in associations.items():
         hosts_to_packages = get_association_hosts_to_packages(
             group, inventory, association_name, ensured_association_only)
@@ -455,14 +470,32 @@
                 f"Use default package '{package}' from inventory.")
             # return default package from inventory if multiple versions detected
             return package
     else:
         return detected_package_versions[0]
 
 
+def disable_unattended_upgrade(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+    if group.get_nodes_os() != 'debian':
+        cluster.log.debug("Skipped - unattended upgrades are supported only on Ubuntu/Debian os family")
+        return
+
+    packages_per_node = get_all_managed_packages_for_group(group=group, inventory=cluster.inventory,
+                                                           ensured_association_only=True)
+
+    with group.new_executor() as exe:
+        for node in exe.group.get_ordered_members_list():
+            packages = [get_package_name(node.get_nodes_os(), package) for package in packages_per_node[node.get_host()]]
+            unattended_upgrade_config = 'Unattended-Upgrade::Package-Blacklist { %s };\n' % " ".join(
+                ['"%s";' % package for package in packages])
+            node.put(StringIO(unattended_upgrade_config), '/etc/apt/apt.conf.d/51unattended-upgrades-kubemarine',
+                     sudo=True, backup=True)
+
+
 def get_associations_os_family_keys() -> Set[str]:
     return {'debian', 'rhel', 'rhel8', 'rhel9'}
 
 
 def get_compatibility_version_key(os_family: str) -> str:
     """
     Get os-specific version key to be used in software compatibility map.
```

### Comparing `kubemarine-0.29.0/kubemarine/patches/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
-from kubemarine.patches.boot_timeout_per_node import TimeoutPerNode
-from kubemarine.patches.strong_cipher_suits_for_kubelet import UpdatekubeletCipherSuites
 
 patches: List[Patch] = [
-    TimeoutPerNode(),
-    UpdatekubeletCipherSuites(),  # Add the new patch to the list
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.29.0/kubemarine/patches/boot_timeout_per_node.py` & `kubemarine-0.30.0/kubemarine/patches/reinstall_etcdctl_thirdparty.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,44 +7,40 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from textwrap import dedent
 
 from kubemarine.core.action import Action
-from kubemarine.core.patch import InventoryOnlyPatch
+from kubemarine.core.patch import RegularPatch
 from kubemarine.core.resources import DynamicResources
+from kubemarine.thirdparties import install_thirdparty
 
 
 class TheAction(Action):
     def __init__(self) -> None:
-        super().__init__("Move globals.nodes.boot.timeout to per-node configuration")
+        super().__init__("Reinstall etcdctl thirdparty")
 
     def run(self, res: DynamicResources) -> None:
-        inventory = res.inventory()
-
-        if 'boot' in inventory.get('globals', {}).get('nodes', {}):
-            self.recreate_inventory = True
-            inventory.setdefault('node_defaults', {})['boot'] = inventory['globals']['nodes'].pop('boot')
-        else:
-            res.logger().info("Nothing has changed")
+        cluster = res.cluster()
+        cluster.log.info("Update /usr/bin/etcdctl thirdparty")
+        install_thirdparty(cluster.nodes['all'], '/usr/bin/etcdctl')
 
 
-class TimeoutPerNode(InventoryOnlyPatch):
+class ReinstallEtcdctl(RegularPatch):
     def __init__(self) -> None:
-        super().__init__("boot_timeout_per_node")
+        super().__init__("reinstall_etcdctl")
 
     @property
     def action(self) -> Action:
         return TheAction()
 
     @property
     def description(self) -> str:
         return dedent(
             f"""\
-            Move globals.nodes.boot.timeout to node_defaults.boot.timeout
+            This patch reinstalls etcdctl thirdparty.
             """.rstrip()
-        )
+        )
```

### Comparing `kubemarine-0.29.0/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.30.0/kubemarine/patches/software_upgrade.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -31,11 +31,10 @@
   keepalived:
     version_rhel: false
     version_rhel8: false
     version_rhel9: false
     version_debian: false
 plugins:
   calico: []
-  nginx-ingress-controller:
-  - v1.29.1
+  nginx-ingress-controller: []
   kubernetes-dashboard: []
   local-path-provisioner: []
```

### Comparing `kubemarine-0.29.0/kubemarine/patches/strong_cipher_suits_for_kubelet.py` & `kubemarine-0.30.0/kubemarine/patches/disable_unattended_upgrade.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,37 +7,39 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from textwrap import dedent
+
 from kubemarine.core.action import Action
 from kubemarine.core.patch import RegularPatch
 from kubemarine.core.resources import DynamicResources
-from kubemarine.kubernetes.components import reconfigure_components
+from kubemarine.packages import disable_unattended_upgrade
+
 
 class TheAction(Action):
     def __init__(self) -> None:
-        super().__init__("Update kubelet TLS cipher suites (if necessary)")
+        super().__init__("Disable unattended upgrade for important packages")
 
     def run(self, res: DynamicResources) -> None:
-        kubernetes_nodes = res.cluster().make_group_from_roles(['control-plane', 'worker'])
-        reconfigure_components(kubernetes_nodes, ['kubelet'])
+        group = res.cluster().make_group_from_roles(['all'])
+        group.call(disable_unattended_upgrade)
+
 
-class UpdatekubeletCipherSuites(RegularPatch):
+class DisableUnattendedUpgrades(RegularPatch):
     def __init__(self) -> None:
-        super().__init__("kubelet_cipher_suites")
+        super().__init__("disable_unattended_upgrades")
 
     @property
     def action(self) -> Action:
         return TheAction()
 
     @property
     def description(self) -> str:
         return dedent(
             f"""\
-            Patch to update the kubelet TLS cipher suites.
+            Disable unattended upgrades on debian nodes for important packages.
             """.rstrip()
         )
```

### Comparing `kubemarine-0.29.0/kubemarine/plugins/__init__.py` & `kubemarine-0.30.0/kubemarine/plugins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,14 +993,16 @@
 
 
 def _apply_file(cluster: KubernetesCluster, config: dict, file_type: str) -> None:
     """
         Apply yamls as is or
         renders and applies templates that match the config 'source' key.
     """
+    from kubemarine.core import defaults  # pylint: disable=cyclic-import
+
     log = cluster.log
     do_render = config.get('do_render', True)
 
     source: Union[str, io.StringIO]
     source, is_external = get_source_absolute_pattern(config)
     files = glob.glob(source)
 
@@ -1011,17 +1013,18 @@
         if do_render:
             # templates usually have '.j2' extension, which we want to remove from resulting filename
             # but we also support usual '.yaml' files without '.j2' extension, in this case we do not want to remove extension
             split_extension = os.path.splitext(source_filename)
             if split_extension[1] == ".j2":
                 source_filename = split_extension[0]
 
-            render_vars = {**cluster.inventory, 'runtime_vars': cluster.context['runtime_vars'], 'env': kos.Environ()}
+            render_vars = {'runtime_vars': cluster.context['runtime_vars'], 'env': kos.Environ()}
             with utils.open_utf8(file, 'r') as template_stream:
-                generated_data = jinja.new(log).from_string(template_stream.read()).render(**render_vars)
+                env = defaults.Environment(log, cluster.inventory)
+                generated_data = env.from_string(template_stream.read()).render(**render_vars)
 
             utils.dump_file(cluster, generated_data, source_filename)
             source = io.StringIO(generated_data)
         elif not is_external:
             with utils.open_utf8(file, 'r') as config_stream:
                 source = io.StringIO(config_stream.read())
```

### Comparing `kubemarine-0.29.0/kubemarine/plugins/builtin.py` & `kubemarine-0.30.0/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/calico.py` & `kubemarine-0.30.0/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.30.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.30.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/manifest.py` & `kubemarine-0.30.0/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.30.0/kubemarine/plugins/nginx_ingress.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml` & `kubemarine-0.30.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.6-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/__init__.py` & `kubemarine-0.30.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/add_node.py` & `kubemarine-0.30.0/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/backup.py` & `kubemarine-0.30.0/kubemarine/procedures/backup.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.30.0/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.30.0/kubemarine/procedures/check_iaas.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 import string
 from collections import OrderedDict
 import time
 from contextlib import contextmanager, nullcontext, AbstractContextManager
 from typing import List, Dict, cast, Match, Iterator, Optional, Tuple, Set, Union
 
 import yaml
+from jinja2 import Template
 from ordered_set import OrderedSet
 
 from kubemarine.core import flow, utils, static
-from kubemarine import system, packages, jinja, thirdparties
+from kubemarine import system, packages, thirdparties
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.errors import KME0006
 from kubemarine.testsuite import TestSuite, TestCase, TestFailure, TestWarn
 from kubemarine.core.group import (
     NodeConfig, NodeGroup, DeferredGroup, GroupException, GroupResultException, CollectorCallback
 )
 
@@ -975,19 +976,19 @@
 def get_stop_listener_cmd(port_listener: str) -> str:
     identify_pid = f"ps aux | grep \" {port_listener} ${{port}}$\" " \
                    f"| grep -v grep | grep -v nohup | awk '{{print $2}}'"
     return f"port=%s;pid=$({identify_pid}) " \
            "&& if [ ! -z $pid ]; then sudo kill -9 $pid; echo \"killed pid $pid for port $port\"; fi"
 
 
-def install_client(cluster: KubernetesCluster, group: DeferredGroup, proto: str, mtu: int, timeout: int) -> str:
+def install_client(group: DeferredGroup, proto: str, mtu: int, timeout: int) -> str:
     check_script = utils.read_internal('resources/scripts/simple_port_client.py')
     udp_client = utils.get_remote_tmp_path(ext='py')
     for node in group.get_ordered_members_list():
-        rendered_script = jinja.new(cluster.log).from_string(check_script).render({
+        rendered_script = Template(check_script).render({
             'proto': proto,
             'timeout': timeout,
             'mtu': mtu,
         })
         node.put(io.StringIO(rendered_script), udp_client)
 
     group.flush()
@@ -1002,15 +1003,15 @@
         return {}
 
     logger = cluster.log
     logger.debug(f"Checking {proto.upper()} connectivity between nodes...")
 
     group = get_python_group(cluster, True).get_accessible_nodes().new_defer()
     timeout = static.GLOBALS['connection']['defaults']['timeout']
-    port_client = install_client(cluster, group, proto, mtu, timeout)
+    port_client = install_client(group, proto, mtu, timeout)
 
     connectivity_ports = get_ports_connectivity(cluster, proto).get(subnet_type, {}).get('output', {})
 
     # Check connectivity from all nodes to each listened port of each specified host.
     connectivity_payloads: Dict[str, OrderedSet[Tuple[str, str, bool]]] = {}
 
     def remove_payload(host: str, payload: Tuple[str, str, bool]) -> None:
@@ -1132,15 +1133,15 @@
         collector = CollectorCallback(cluster)
         with group.new_executor() as exe:
             # Run processes that listen TCP or UDP ports
             for node in exe.group.get_ordered_members_list():
                 host = node.get_host()
                 bind_address = host_to_ip[host]
                 ip_version = ipaddress.ip_address(bind_address).version
-                rendered_script = jinja.new(logger).from_string(check_script).render({
+                rendered_script = Template(check_script).render({
                     'proto': proto,
                     'address': bind_address,
                     'ip_version': ip_version,
                     'mtu': mtu,
                 })
                 node.put(io.StringIO(rendered_script), port_listener)
 
@@ -1321,84 +1322,115 @@
                 raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
             failed_nodes = check_ipip_tunnel(group)
         else:
             skipped_msgs.append("Encapsulation IPIP is disabled")
             raise TestWarn("Check cannot be completed", hint='\n'.join(skipped_msgs))
 
         if failed_nodes:
-            raise TestFailure(f"Check firewall settings, IP in IP traffic is not allowed between nodes.",
-                              hint='\n'.join(failed_nodes))
+            raise TestFailure(f"Check firewall settings for all nodes in the cluster, "
+                              "IP in IP traffic is not allowed between nodes.", hint='\n'.join(failed_nodes))
 
+        if group.nodes_amount() == 2:
+            skipped_msgs.append("Change nodes order in 'cluster.yaml' and run the check "
+                                "10 minutes later")
+            raise TestWarn("Check has been succeded for the second node but cannot be completed for "
+                           "the first node", hint='\n'.join(skipped_msgs))
 
 def check_ipip_tunnel(group: NodeGroup) -> Set[str]:
 
     group_to_rollback = group
     cluster = group.cluster
 
     # Copy binaries to the nodes
-    random_port = str(random.randint(50000, 65535))
+    random_sport = str(random.randint(50000, 65535))
+    random_dport = str(random.randint(50000, 65535))
     failed_nodes: Set[str] = set()
     recv_cmd: Dict[str, str] = {}
     trns_cmd: Dict[str, str] = {}
 
     binary_check_path = utils.get_internal_resource_path('./resources/scripts/ipip_check.gz')
     ipip_check = utils.get_remote_tmp_path()
     # Random message
     random.seed()
     msg = ''.join(random.choices(string.ascii_letters + string.digits, k=15))
     # Random IP from class E
     int_ip = random.randint(4026531841, 4294967294)
     fake_addr = str(ipaddress.IPv4Address(int_ip))
     # That is used as number of packets for transmitter
     timeout = int(cluster.inventory['globals']['timeout_download'])
-    for node in group.get_ordered_members_configs_list():
-        host = node['internal_address']
-        # Transmitter start command
-        # Transmitter starts first and sends IPIP packets every 1 second until the timeout comes or
-        # the process is killed by terminating command
-        trns_item_cmd: List[str] = []
-        for node_item in group.get_ordered_members_configs_list():
-            if node_item['internal_address'] != host:
-                trns_item_cmd.append(f"nohup {ipip_check} -mode client -src {host} -int {fake_addr} "
-                                     f"-ext {node_item['internal_address']} -dport {random_port} "
-                                     f"-msg {msg} -timeout {timeout} > /dev/null 2>&1 & echo $! >> {ipip_check}.pid")
-        trns_cmd[host] = '& sudo '.join(trns_item_cmd)
-        # Receiver start command
-        # Receiver starts after the transmitter and try to get IPIP packets within 3 seconds from eache node
-        recv_cmd[host] = f"{ipip_check} -mode server -ext {host} -int {fake_addr} -dport {random_port} " \
-                         f"-msg {msg} -timeout 3 2> /dev/null"
+    nodes_list = group.get_ordered_members_configs_list()
+    # The ring circuit is used for the procedure. Each node in the ring transmit IPIP packets to the next node in the ring
+    # and receive IPIP packets from the previous node of the ring.
+    # That makes check more robast to some IP filters implementation.
+    recv_neighbor_node: Dict[str, str] = {}
+    trns_neighbor_host = ""
+    if len(nodes_list) > 2:
+        node_number = 0
+        for node in nodes_list:
+            host = node['internal_address']
+            if node_number < len(nodes_list) - 1:
+                recv_neighbor_node[nodes_list[node_number + 1]['name']] = node['name']
+                trns_neighbor_host = nodes_list[node_number + 1]['internal_address']
+            else:
+                recv_neighbor_node[nodes_list[0]['name']] = node['name']
+                trns_neighbor_host = nodes_list[0]['internal_address']
+            # Transmitter start command
+            # Transmitter starts first and sends IPIP packets every 1 second until the timeout comes or
+            # the process is killed by terminating command
+            trns_cmd[host] = f"nohup {ipip_check} -mode client -src {host} -int {fake_addr} " \
+                             f"-ext {trns_neighbor_host} -sport {random_sport} -dport {random_dport} " \
+                             f"-msg {msg} -timeout {timeout} > /dev/null 2>&1 & echo $! >> {ipip_check}.pid"
+            # Receiver start command
+            # Receiver starts after the transmitter and try to get IPIP packets within 3 seconds from neighbor node
+            recv_cmd[host] = f"{ipip_check} -mode server -ext {host} -int {fake_addr} -sport {random_sport}" \
+                             f" -dport {random_dport} -msg {msg} -timeout 3 2> /dev/null"
+            node_number += 1
+    else:
+        # Two nodes have only one transmitter and only one receiver
+        host = nodes_list[0]['internal_address']
+        recv_neighbor_node[nodes_list[1]['name']] = nodes_list[0]['name']
+        trns_neighbor_host = nodes_list[1]['internal_address']
+        trns_cmd[host] = f"nohup {ipip_check} -mode client -src {host} -int {fake_addr} " \
+                         f"-ext {trns_neighbor_host} -sport {random_sport} -dport {random_dport} " \
+                         f"-msg {msg} -timeout {timeout} > /dev/null 2>&1 & echo $! >> {ipip_check}.pid"
+        host = nodes_list[1]['internal_address']
+        recv_cmd[host] = f"{ipip_check} -mode server -ext {host} -int {fake_addr} -sport {random_sport} " \
+                         f"-dport {random_dport} -msg {msg} -timeout 3 2> /dev/null"
 
     try:
         collector = CollectorCallback(group.cluster)
         cluster.log.debug("Copy binaries to the nodes")
         group.put(binary_check_path, f"{ipip_check}.gz")
         group.sudo(f"gzip -d {ipip_check}.gz")
         group.sudo(f"sudo chmod +x {ipip_check}")
-        # Run transmitters
+        # Run transmitters if it's applicable for node
         cluster.log.debug("Run transmitters")
         with group.new_executor() as exe:
             for node_exe in exe.group.get_ordered_members_list():
                 host_int = node_exe.get_config()['internal_address']
-                node_exe.sudo(f"{trns_cmd[host_int]}")
-        # Run receivers and get results
+                if trns_cmd.get(host_int, ""):
+                    node_exe.sudo(f"{trns_cmd[host_int]}")
+        # Run receivers and get results if it's applicable for node
         cluster.log.debug("Run receivers")
         with group.new_executor() as exe:
             for node_exe in exe.group.get_ordered_members_list():
                 host_int = node_exe.get_config()['internal_address']
-                node_exe.sudo(f"{recv_cmd[host_int]}", warn=True, callback=collector)
+                if recv_cmd.get(host_int, ""):
+                    node_exe.sudo(f"{recv_cmd[host_int]}", warn=True, callback=collector)
 
         for host, item in collector.result.items():
             node_name = cluster.get_node_name(host)
             item_list: Set[str] = set()
             if len(item.stdout) > 0:
                 for log_item in item.stdout.split("\n")[:-1]:
                     item_list.add(log_item)
-            for node in group.get_ordered_members_configs_list():
-                if node['internal_address'] not in item_list and node['connect_to'] != host:
-                    failed_nodes.add(f"{node['name']} -> {node_name}")
+            # Check if the neighbor IP is in logs
+            trns_node = group.get_member_by_name(recv_neighbor_node[node_name]).get_config()
+            if trns_node['internal_address'] not in item_list:
+                failed_nodes.add(f"{trns_node['name']} -> {node_name}")
 
         return failed_nodes
     finally:
         # Delete binaries ang logs
         cluster.log.debug("Delete binaries")
         with group_to_rollback.new_executor() as exe:
             for node_exe in exe.group.get_ordered_members_list():
```

### Comparing `kubemarine-0.29.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.30.0/kubemarine/procedures/check_paas.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import io
 import ipaddress
 import sys
 import time
 from collections import OrderedDict
 import re
 from textwrap import dedent
-from typing import List, Dict, Optional, Union
+from typing import List, Dict, Optional, Union, cast, Iterable
 
 import yaml
 import ruamel.yaml
 from deepdiff import DeepDiff  # type: ignore[import-untyped]
 
 from ordered_set import OrderedSet
 
@@ -165,15 +165,21 @@
     :param pckg_alias: system package alias to retrieve "package_name" association.
     """
     with TestCase(cluster, '205', "Services", f"{pckg_alias} version") as tc:
         _check_same_os(cluster)
         hosts_to_packages = pckgs.get_association_hosts_to_packages(cluster.nodes['all'], cluster.inventory, pckg_alias)
         if not hosts_to_packages:
             raise TestWarn(f"No nodes to check {pckg_alias!r} version")
-        check_packages_versions(cluster, tc, hosts_to_packages, raise_successful=False)
+
+        os_family = cluster.get_os_family()
+        require_same_version = []
+        if pckgs.cache_versions_enabled(cluster, os_family, pckg_alias):
+            require_same_version = pckgs.get_association_packages(cluster, os_family, pckg_alias)
+
+        check_packages_versions(cluster, tc, hosts_to_packages, require_same_version, raise_successful=False)
 
         if pckg_alias in ["haproxy", "keepalived", "containerd", "docker"]:
             recommended_system_package_versions(cluster, pckg_alias)
         tc.success("all packages have correct versions")
 
 
 def mandatory_packages_versions(cluster: KubernetesCluster) -> None:
@@ -182,76 +188,93 @@
     Failure is shown if check is not successful.
     :param cluster: main cluster object.
     """
     with TestCase(cluster, '205', "Services", "Mandatory package versions") as tc:
         _check_same_os(cluster)
         hosts_to_packages: Dict[str, List[str]] = {}
         group = cluster.nodes['all']
+        os_family = cluster.get_os_family()
+        require_same_version = OrderedSet[str]()
         for package in cluster.inventory["services"]["packages"]['mandatory'].keys():
             packages = pckgs.get_association_hosts_to_packages(group, cluster.inventory, package)
 
             for host, packages_list in packages.items():
                 hosts_to_packages.setdefault(host, []).extend(packages_list)
 
+            if pckgs.cache_versions_enabled(cluster, os_family, package):
+                require_same_version.update(pckgs.get_association_packages(cluster, os_family, package))
+
         if not hosts_to_packages:
             raise TestWarn(f"No mandatory packages to check")
 
-        return check_packages_versions(cluster, tc, hosts_to_packages)
+        return check_packages_versions(cluster, tc, hosts_to_packages, require_same_version)
 
 
 def generic_packages_versions(cluster: KubernetesCluster) -> None:
     """
     Verifies that user-provided packages are installed on required nodes and have equal versions.
     Warning is shown if check is not successful.
     """
     with TestCase(cluster, '206', "Services", f"Generic packages version") as tc:
         _check_same_os(cluster)
         packages = cluster.inventory['services']['packages'].get('install', {}).get('include', [])
         hosts_to_packages = {host: packages for host in cluster.nodes['all'].get_hosts()}
-        return check_packages_versions(cluster, tc, hosts_to_packages, warn_on_bad_result=True)
+        return check_packages_versions(cluster, tc, hosts_to_packages, packages, warn_on_bad_result=True)
 
 
 def check_packages_versions(cluster: KubernetesCluster, tc: TestCase, hosts_to_packages: Dict[str, List[str]],
+                            packages_require_same_version: Iterable[str],
                             warn_on_bad_result: bool = False, raise_successful: bool = True) -> None:
     """
     Verifies that all packages are installed on required nodes and have equal versions
     :param cluster: main cluster object
     :param tc: current test case object
     :param hosts_to_packages: hosts where to check packages
-    :param warn_on_bad_result: if true then uses Warning instead of Failure. Default False.
+    :param packages_require_same_version: Fail or Warn for the specified set of packages
+                                          if different versions are detected.
+    :param warn_on_bad_result: if true then bad results raises Warning instead of Failure. Default False.
+    :param raise_successful: if true, successful test result will be risen. Default True.
     """
-    bad_results = []
+    bad_results = OrderedSet[str]()
+    warn_results = OrderedSet[str]()
     good_results = []
 
     packages_map = pckgs.detect_installed_packages_version_hosts(cluster, hosts_to_packages)
     for package, version_map in packages_map.items():
-        if len(version_map) != 1:
+        installed_versions = [version for version in version_map if "not installed" not in version]
+        if len(installed_versions) != 1:
             cluster.log.debug(f"Package {package} has different versions:")
-            cluster.log.debug(version_map)
-            bad_results.append(package)
-
-        version = list(version_map.keys())[0]
-        if "not installed" in version:
-            cluster.log.debug(f"Package {package} is not installed on some nodes:")
-            cluster.log.debug(version_map[version])
-            bad_results.append(package)
-        else:
-            package_name = package.replace("*", "")
-            if version.startswith(package_name):
-                good_results.append(version)
+            cluster.log.debug(installed_versions)
+            if package in packages_require_same_version:
+                bad_results.append(package)
             else:
-                bad_results.append(f"Actual version: {version} doesn't match expected package version: {package}")
+                warn_results.append(package)
 
+        for version in version_map.keys():
+            if "not installed" in version:
+                cluster.log.debug(f"Package {package} is not installed on some nodes:")
+                cluster.log.debug(version_map[version])
+                bad_results.append(package)
+            else:
+                package_name = package.replace("*", "")
+                if version.startswith(package_name):
+                    good_results.append(version)
+                else:
+                    cluster.log.debug(f"Actual version: {version} doesn't match expected package version: {package} on "
+                                      f"nodes: {version_map[version]}")
+                    bad_results.append(version)
 
-    if bad_results:
+    if bad_results and not warn_on_bad_result:
         hint_message = f'Check the presence and correctness of the version of the following packages on the ' \
-                       f'system: {bad_results}\n'
-        if warn_on_bad_result:
-            raise TestWarn("detected incorrect packages versions", hint=hint_message)
+                       f'system: {list(bad_results)}\n'
         raise TestFailure("detected incorrect packages versions", hint=hint_message)
+    if warn_results or (warn_on_bad_result and bad_results):
+        hint_message = f'Check the presence and correctness of the version of the following packages on the ' \
+                       f'system: {list(bad_results | warn_results)}\n'
+        raise TestWarn("detected incorrect packages versions", hint=hint_message)
     cluster.log.debug(f"installed packages: {good_results}")
     if raise_successful:
         tc.success("all packages have correct versions")
 
 
 def get_nodes_description(cluster: KubernetesCluster) -> dict:
     return kubernetes.get_nodes_description(cluster)
@@ -599,15 +622,15 @@
                                    "the node.")
 
         tc.success(results="%s" % ', '.join(positive_conditions))
 
 
 def get_not_running_pods(cluster: KubernetesCluster) -> str:
     # Completed pods should be excluded from the list as well
-    get_pods_cmd = ('kubectl get pods -A --field-selector status.phase!=Running '
+    get_pods_cmd = ('kubectl get pods -A | grep -v Running '
                     '| awk \'{ print $1" "$2" "$4 }\' | grep -vw Completed || true')
     result = cluster.nodes['control-plane'].get_any_member().sudo(get_pods_cmd)
     cluster.log.verbose(result)
     return list(result.values())[0].stdout.strip()
 
 
 def kubernetes_pods_condition(cluster: KubernetesCluster) -> None:
@@ -769,14 +792,15 @@
 
 
 def nodes_pid_max(cluster: KubernetesCluster) -> None:
     with TestCase(cluster, '202', "Nodes", "Nodes pid_max correctly installed") as tc:
         control_plane = cluster.nodes['control-plane'].get_any_member()
         yaml = ruamel.yaml.YAML()
         nodes_failed_pid_max_check = {}
+        nodes_warned_pid_max_check = {}
         for node in cluster.make_group_from_roles(['control-plane', 'worker']).get_ordered_members_list():
             node_name = node.get_node_name()
 
             node_info = control_plane.sudo("kubectl get node %s -o yaml" % node_name).get_simple_out()
             config = yaml.load(node_info)
             max_pods = int(config['status']['capacity']['pods'])
 
@@ -791,39 +815,46 @@
                 # we need limited podPidsLimit to avoid PIDs exhaustion
                 if pod_pids_limit != -1: 
                     required_pid_max = max_pods * pod_pids_limit + 2048
                     cluster.log.debug("Current values:\n maxPods = %s \n podPidsLimit = %s \n pid_max = %s"
                                   % (max_pods, pod_pids_limit, pid_max))
                     cluster.log.debug("Required pid_max for current kubelet configuration is %s for node '%s'"
                                   % (required_pid_max, node_name))
-                    if cluster.inventory['services']['sysctl'].get("kernel.pid_max"):
-                        inventory_pid_max = cluster.inventory['services']['sysctl'].get("kernel.pid_max")
-                        if pid_max != inventory_pid_max:
-                            raise TestWarn("The 'kernel.pid_max' value defined in system = %s, "
-                                       "but 'kernel.pid_max', which defined in cluster.yaml = %s"
-                                       % (pid_max, inventory_pid_max))
+                    inventory_pid_max = cast(int, sysctl.get_parameter(cluster, node, 'kernel.pid_max'))
+                    if pid_max != inventory_pid_max:
+                        nodes_warned_pid_max_check[node_name] = [pid_max, inventory_pid_max]
                     if pid_max < required_pid_max:
                         nodes_failed_pid_max_check[node_name] = [pid_max, required_pid_max]
                 else:
                     cluster.log.error("podPidsLimit is set to unlimited in the /var/lib/kubelet/config.yaml "
                                       f"for node '{node_name}'")
                     nodes_failed_pid_max_check[node_name] = [pid_max, -1]
             else:
                 cluster.log.error("No podPidsLimit set in the /var/lib/kubelet/config.yaml for node '%s'" % node_name)
                 nodes_failed_pid_max_check[node_name] = [pid_max, -1]
 
         if nodes_failed_pid_max_check:
             output = "The requirement for the 'pid_max' value is not met for nodes:\n"
-            for node_name, pid_max_check in nodes_failed_pid_max_check.items():
-                if pid_max_check[1] == -1:
-                    output += ("For node %s podPidsLimit is unlimited" % node_name)
+            for node_name, (pid_max, required_pid_max) in nodes_failed_pid_max_check.items():
+                if required_pid_max == -1:
+                    output += ("For node %s podPidsLimit is unlimited\n" % node_name)
                 else:
                     output += ("For node %s pid_max value = '%s', but it should be >= then '%s'\n"
-                               % (node_name, pid_max_check[0], pid_max_check[1]))
-            raise TestFailure(output)
+                               % (node_name, pid_max, required_pid_max))
+            raise TestFailure('invalid', hint=output)
+
+        if nodes_warned_pid_max_check:
+            output = ''
+            for node_name, (pid_max, inventory_pid_max) in nodes_warned_pid_max_check.items():
+                output += ("For node %s the 'kernel.pid_max' value defined in system = %s, "
+                           "but 'kernel.pid_max', which defined in cluster.yaml = %s\n"
+                           % (node_name, pid_max, inventory_pid_max))
+
+            raise TestWarn('found warnings', hint=output)
+
         tc.success(results="pid_max correctly installed on all nodes")
 
 
 def verify_selinux_status(cluster: KubernetesCluster) -> None:
     """
     This method is a test, which checks the status of Selinux. It must be `enforcing`. It may be `permissive`, but must
     be explicitly specified in the inventory. Otherwise, the test will fail. This test is applicable only for systems of
```

### Comparing `kubemarine-0.29.0/kubemarine/procedures/config.py` & `kubemarine-0.30.0/kubemarine/procedures/config.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/do.py` & `kubemarine-0.30.0/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/install.py` & `kubemarine-0.30.0/kubemarine/procedures/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     if sysctl.is_valid(group):
         cluster.log.debug("Skipped - all necessary kernel parameters are presented")
         return
 
     group.call_batch([
         sysctl.configure,
         sysctl.reload,
+        system.verify_sysctl,
     ])
 
     cluster.schedule_cumulative_point(system.reboot_nodes)
     cluster.schedule_cumulative_point(system.verify_system)
 
 
 @_applicable_for_new_nodes_with_roles('all')
@@ -249,14 +250,19 @@
     group.call(packages.add_repo, repo_data=repositories)
 
     cluster.log.debug("Nodes contain the following repositories:")
     cluster.log.debug(packages.ls_repofiles(group))
 
 
 @_applicable_for_new_nodes_with_roles('all')
+def system_prepare_package_manager_disable_unattended_upgrades(group: NodeGroup) -> None:
+    group.call(packages.disable_unattended_upgrade)
+
+
+@_applicable_for_new_nodes_with_roles('all')
 def system_prepare_package_manager_manage_packages(group: NodeGroup) -> None:
     group.call_batch([
         manage_mandatory_packages,
         manage_custom_packages
     ])
 
 
@@ -507,14 +513,15 @@
         "dns": {
             "hostname": system_prepare_dns_hostname,
             "etc_hosts": system_prepare_dns_etc_hosts,
             "resolv_conf": system_prepare_dns_resolv_conf
         },
         "package_manager": {
             "configure": system_prepare_package_manager_configure,
+            "disable_unattended_upgrades": system_prepare_package_manager_disable_unattended_upgrades,
             "manage_packages": system_prepare_package_manager_manage_packages
         },
         "ntp": {
             "chrony": system_prepare_system_chrony,
             "timesyncd": system_prepare_system_timesyncd
         },
         "system": {
```

### Comparing `kubemarine-0.29.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.30.0/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.30.0/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.30.0/kubemarine/procedures/migrate_cri.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.30.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/reboot.py` & `kubemarine-0.30.0/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/reconfigure.py` & `kubemarine-0.30.0/kubemarine/procedures/reconfigure.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.30.0/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/procedures/restore.py` & `kubemarine-0.30.0/kubemarine/procedures/restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     snap_name = '/var/lib/etcd/etcd-snapshot%s.db' % int(round(time.time() * 1000))
     cluster.nodes['control-plane'].put(os.path.join(cluster.context['backup_tmpdir'], 'etcd.db'), snap_name, sudo=True)
 
     initial_cluster_list = []
     initial_cluster_list_without_names = []
     for control_plane in cluster.nodes['control-plane'].get_ordered_members_configs_list():
         initial_cluster_list.append(control_plane['name'] + '=https://' + control_plane["internal_address"] + ":2380")
-        initial_cluster_list_without_names.append(control_plane["internal_address"] + ":2379")
+        initial_cluster_list_without_names.append('https://' + control_plane["internal_address"] + ":2379")
     initial_cluster = ','.join(initial_cluster_list)
 
     if "docker" == cluster.inventory['services']['cri']['containerRuntime']:
         cont_runtime = "docker"
     else:
         cont_runtime = "ctr"
     container_name = f'etcd-{uuid.uuid4().hex}'
@@ -197,15 +197,20 @@
     etcd_instances = 0
     for control_plane in cluster.nodes['control-plane'].get_ordered_members_configs_list():
         cluster.log.debug('Restoring ETCD member ' + control_plane['name'])
         control_plane_conn = cluster.make_group([control_plane['connect_to']])
         control_plane_conn.sudo(
             f'chmod 777 {snap_name} && '
             f'sudo ls -la {snap_name} && '
-            f'sudo etcdctl snapshot restore {snap_name} '
+            f'sudo ETCD_IMAGE="{etcd_image}" ETCD_MOUNTS="{mount_options}" etcdctl '
+            f'--cert={etcd_cert} '
+            f'--key={etcd_key} '
+            f'--cacert={etcd_cacert} '
+            f'--endpoints={",".join(initial_cluster_list_without_names)} '
+            f'snapshot restore {snap_name} '
             f'--name={control_plane["name"]} '
             f'--data-dir=/var/lib/etcd/snapshot '
             f'--initial-cluster={initial_cluster} '
             f'--initial-advertise-peer-urls=https://{control_plane["internal_address"]}:2380',
             hide=False)
 
         _ = control_plane_conn.sudo(
```

### Comparing `kubemarine-0.29.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.30.0/kubemarine/procedures/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import List, Callable, Dict
 
 from kubemarine import kubernetes, plugins, admission, jinja
 from kubemarine.core import flow, log, resources as res
 from kubemarine.core import utils
 from kubemarine.core.cluster import KubernetesCluster, EnrichmentStage
 from kubemarine.core.resources import DynamicResources
+from kubemarine.kubernetes import components
 from kubemarine.procedures import install
 
 
 def cleanup_tmp_dir(cluster: KubernetesCluster) -> None:
     # Clean up kubernetes tmp dir, where backup files from previous upgrades are located
     nodes = cluster.make_group_from_roles(roles=["control-plane", "worker"])
     nodes.sudo("rm -rf $(sudo find /etc/kubernetes/tmp -mindepth 1 -maxdepth 1)")
@@ -73,15 +74,15 @@
         preconfigure_components.append('kube-apiserver')
         preconfigure_functions['kubeadm-config'] = reconfigure_feature_gates
 
     if (kubernetes.components.kube_proxy_overwrites_higher_system_values(cluster)
             and utils.version_key(initial_kubernetes_version)[0:2] < utils.minor_version_key("v1.29")):
 
         # Defaults of KubeProxyConfiguration have changed.
-        # See services.kubeadm_kube-proxy.conntrack.min section of defaults.yaml
+        # See kubernetes.enrich_kube_proxy()
         def edit_kube_proxy_conntrack_min(kube_proxy_cm: dict) -> dict:
             expected_conntrack: dict = cluster.inventory['services']['kubeadm_kube-proxy']['conntrack']
             if 'min' not in expected_conntrack:
                 return kube_proxy_cm
 
             actual_conntrack = kube_proxy_cm['conntrack']
             if expected_conntrack['min'] != actual_conntrack.get('min'):
@@ -100,19 +101,24 @@
     grace_period = cluster.procedure_inventory.get('grace_period')
     disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
     drain_kwargs = {
         'disable_eviction': disable_eviction, 'drain_timeout': drain_timeout, 'grace_period': grace_period
     }
 
     kubernetes.upgrade_first_control_plane(upgrade_group, cluster, **drain_kwargs)
+    first_control_plane = cluster.nodes['control-plane'].get_first_member()
 
     # After first control-plane upgrade is finished we may loose our CoreDNS changes.
     # Thus, we need to re-apply our CoreDNS changes immediately after first control-plane upgrade.
     install.deploy_coredns(cluster)
 
+    # In some versions, kubeadm reverts resolvConf to the default during `upgrade apply`
+    # Remove default resolvConf from kubelet-config ConfigMap for debian OS family
+    first_control_plane.call(components.patch_kubelet_configmap)
+
     kubernetes.upgrade_other_control_planes(upgrade_group, cluster, **drain_kwargs)
 
     if cluster.nodes.get('worker', []):
         kubernetes.upgrade_workers(upgrade_group, cluster, **drain_kwargs)
 
     kubernetes_cleanup_nodes_versions(cluster)
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -147,54 +147,92 @@
         - native.cgroupdriver=systemd
       icc: False
       live-restore: True
       userland-proxy: False
 
   modprobe:
     rhel:
-      - br_netfilter
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_conntrack_ipv6{% else %}nf_conntrack{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat_masquerade_ipv6{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
-    rhel8:
-      - br_netfilter
-      - nf_conntrack
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
-    rhel9:
-      - br_netfilter
-      - nf_conntrack
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
-    debian:
-      - br_netfilter
-      - nf_conntrack
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
-      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
+      - modulename: br_netfilter
+        groups: [control-plane, worker]
+      - modulename: nf_conntrack
+        groups: [control-plane, worker]
+        install: '{{ nodes[0]["internal_address"] | isipv4 }}'
+      - modulename: nf_conntrack_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: ip6table_filter
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_nat_masquerade_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_reject_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_defrag_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+    rhel8: &modprobe-default-modules
+      - modulename: br_netfilter
+        groups: [control-plane, worker]
+      - modulename: nf_conntrack
+        groups: [control-plane, worker]
+      - modulename: ip6table_filter
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_nat
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_reject_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+      - modulename: nf_defrag_ipv6
+        install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+    rhel9: *modprobe-default-modules
+    debian: *modprobe-default-modules
 
   sysctl:
-    net.bridge.bridge-nf-call-iptables: 1
-    net.ipv4.ip_forward: 1
-    net.ipv4.ip_nonlocal_bind: 1
-    net.ipv4.conf.all.route_localnet: 1
-    net.bridge.bridge-nf-call-ip6tables: '{% if not nodes[0]["internal_address"]|isipv4 %}1{% endif %}'
-    net.ipv6.conf.all.forwarding: '{% if not nodes[0]["internal_address"]|isipv4 %}1{% endif %}'
-    net.ipv6.ip_nonlocal_bind: '{% if not nodes[0]["internal_address"]|isipv4 %}1{% endif %}'
-    net.netfilter.nf_conntrack_max: 1000000
-    kernel.panic: 10
-    vm.overcommit_memory: 1
-    kernel.panic_on_oops: 1
+    net.ipv4.ip_nonlocal_bind:
+      value: 1
+      # actually, need to be enabled only if balancer is combined with other roles
+      groups: [balancer]
+    net.ipv6.ip_nonlocal_bind:
+      value: 1
+      # actually, need to be enabled only if balancer is combined with other roles
+      groups: [balancer]
+      install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+    net.bridge.bridge-nf-call-iptables:
+      value: 1
+      groups: [control-plane, worker]
+    net.bridge.bridge-nf-call-ip6tables:
+      value: 1
+      groups: [control-plane, worker]
+      install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+    net.ipv4.ip_forward:
+      value: 1
+      groups: [control-plane, worker]
+    net.ipv4.conf.all.route_localnet:
+      # backward compatibility
+      # https://github.com/kubernetes/kubernetes/blob/master/CHANGELOG/CHANGELOG-1.21.md#no-really-you-must-read-this-before-you-upgrade-6
+      value: 1
+      groups: [control-plane, worker]
+    net.ipv6.conf.all.forwarding:
+      value: 1
+      groups: [control-plane, worker]
+      install: '{{ nodes[0]["internal_address"] | isipv6 }}'
+    net.netfilter.nf_conntrack_max:
+      value: 1000000
+      groups: [control-plane, worker]
+    kernel.panic:
+      value: 10
+      groups: [control-plane, worker]
+      install: '{{ services.kubeadm_kubelet.protectKernelDefaults }}'
+    vm.overcommit_memory:
+      value: 1
+      groups: [control-plane, worker]
+      install: '{{ services.kubeadm_kubelet.protectKernelDefaults }}'
+    kernel.panic_on_oops:
+      value: 1
+      groups: [control-plane, worker]
+      install: '{{ services.kubeadm_kubelet.protectKernelDefaults }}'
+    kernel.pid_max:
+      # default value is set in sysctl.enrich_inventory
+      groups: [control-plane, worker]
 
   etc_hosts:
     127.0.0.1:
       - localhost
       - localhost.localdomain
     '::1':
       - '{% if not nodes[0]["internal_address"]|isipv4 %}localhost{% endif %}'
@@ -404,22 +442,22 @@
             default:
               priority: 1
               class: IN
               type: A
               zone: '{{ cluster_name }}'
               data:
                 match: '^(.*\.)?{{ cluster_name }}\.$'
-                answer: '{% raw %}{{ .Name }}{% endraw %} 3600 IN A {{ control_plain["internal"] }}'
+                answer: '{{ "{{ .Name }}" }} 3600 IN A {{ control_plain["internal"] }}'
             reject-aaaa:
               enabled: '{{ nodes[0]["internal_address"]|isipv4 }}'
               priority: 1
               class: IN
               type: AAAA
               data:
-                authority: '{% raw %}{{ .Name }}{% endraw %} 3600 IN SOA coredns.kube-system.svc.cluster.local. hostmaster.coredns.kube-system.svc.cluster.local. (3600 3600 3600 3600 3600)'
+                authority: '{{ "{{ .Name }}" }} 3600 IN SOA coredns.kube-system.svc.cluster.local. hostmaster.coredns.kube-system.svc.cluster.local. (3600 3600 3600 3600 3600)'
           forward:
             - .
             - /etc/resolv.conf
       Hosts: |
         127.0.0.1 localhost localhost.localdomain
         {% if not nodes[0]["internal_address"]|isipv4 %}::1 localhost localhost.localdomain{% endif %}
 
@@ -515,15 +553,15 @@
 
 plugin_defaults:
   installation: {}
 
 plugins:
 
   calico:
-    version: '{{ globals.compatibility_map.software["calico"][services.kubeadm.kubernetesVersion|kubernetes_version].version }}'
+    version: '{{ globals.compatibility_map.software["calico"][services.kubeadm.kubernetesVersion].version }}'
     install: true
     installation:
       priority: 0
       procedures:
         - python:
             module: plugins/builtin.py
             method: apply_yaml
@@ -531,20 +569,20 @@
               plugin_name: calico
         - &plugins-calico-expect
           expect:
             daemonsets:
               - calico-node
             deployments:
               - calico-kube-controllers
-              - '{% if plugins.calico.typha.enabled | is_true %}calico-typha{% endif %}'
+              - '{% if plugins.calico.typha.enabled %}calico-typha{% endif %}'
             pods:
               - coredns
               - calico-kube-controllers
               - calico-node
-              - '{% if plugins.calico.typha.enabled | is_true %}calico-typha{% endif %}'
+              - '{% if plugins.calico.typha.enabled %}calico-typha{% endif %}'
         - thirdparty: /usr/bin/calicoctl
         - template:
             source: templates/plugins/calicoctl.cfg.j2
             destination: /etc/calico/calicoctl.cfg
             apply_required: false
         - template:
             source: templates/plugins/calico-ippool.yaml.j2
@@ -659,15 +697,15 @@
           timeout: 5
           # Sometimes the container fails the liveness probe the first time for unknown reason, and restarted.
           # The total expect timeout is set with respect to initialDelaySeconds of the livenessProbe,
           # and current `renew_apiserver_certificate` implementation details.
           retries: 40
 
   nginx-ingress-controller:
-    version: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|kubernetes_version].version }}'
+    version: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion].version }}'
     install: true
     installation:
       registry: registry.k8s.io
       priority: 1
       procedures:
         - python:
             module: plugins/nginx_ingress.py
@@ -687,15 +725,15 @@
             pods:
               - ingress-nginx-controller
     config_map:
       use-proxy-protocol: '{% if nodes | select("has_role", "balancer") | first %}true{% else %}false{% endif %}'
       # redefine default value for controller >= v1.9.0 because we need to use snippet annotations for dashboard
       allow-snippet-annotations: "true"
     webhook:
-      image: 'ingress-nginx/kube-webhook-certgen:{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|kubernetes_version]["webhook-version"] }}'
+      image: 'ingress-nginx/kube-webhook-certgen:{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion]["webhook-version"] }}'
       # resources values are based on https://github.com/kubernetes/ingress-nginx/blob/helm-chart-4.7.1/charts/ingress-nginx/values.yaml#L598
       resources:
         requests:
           cpu: 10m
           memory: 20Mi
         limits:
           cpu: 20m
@@ -727,15 +765,15 @@
         containerPort: 10254
         protocol: TCP
       - name: webhook
         containerPort: 8443
         protocol: TCP
 
   kubernetes-dashboard:
-    version: '{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion|kubernetes_version].version }}'
+    version: '{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion].version }}'
     install: false
     installation:
       priority: 2
       procedures:
         - python:
             module: plugins/builtin.py
             method: apply_yaml
@@ -764,15 +802,15 @@
         requests:
           cpu: 100m
           memory: 200Mi
         limits:
           cpu: 1
           memory: 200Mi
     metrics-scraper:
-      image: 'kubernetesui/metrics-scraper:{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion|kubernetes_version]["metrics-scraper-version"] }}'
+      image: 'kubernetesui/metrics-scraper:{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion]["metrics-scraper-version"] }}'
       nodeSelector:
         kubernetes.io/os: linux
       resources:
         requests:
           cpu: 50m
           memory: 90Mi
         limits:
@@ -804,15 +842,15 @@
                   backend:
                     service:
                       name: kubernetes-dashboard
                       port:
                         number: 443
 
   local-path-provisioner:
-    version: '{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion|kubernetes_version].version }}'
+    version: '{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion].version }}'
     install: false
     installation:
       priority: 2
       procedures:
       - python:
           module: plugins/builtin.py
           method: apply_yaml
@@ -822,15 +860,15 @@
           pods:
             - local-path-provisioner
     storage-class:
       name: local-path
       is-default: "false"
     volume-dir: /opt/local-path-provisioner
     image: 'rancher/local-path-provisioner:{{ plugins["local-path-provisioner"].version }}'
-    helper-pod-image: 'library/busybox:{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion|kubernetes_version]["busybox-version"] }}'
+    helper-pod-image: 'library/busybox:{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion]["busybox-version"] }}'
     # resources values are based on https://github.com/rancher/local-path-provisioner/blob/v0.0.24/deploy/chart/local-path-provisioner/values.yaml#L69
     resources:
       requests:
         cpu: 100m
         memory: 128Mi
       limits:
         cpu: 200m
@@ -882,7 +920,8 @@
       runtimeClasses: []
       namespaces: ["kube-system"]
 
 procedure_history:
   archive_threshold: 5
   delete_threshold: 10
 
+patches: []
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.30.0/kubemarine/resources/configurations/globals.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -255,26 +255,31 @@
         - worker
     iptables:
       package_name: 'iptables'
       groups:
         - control-plane
         - worker
     openssl:
+      cache_versions: false
       package_name: 'openssl'
       groups: [ control-plane, worker, balancer ]
     curl:
+      cache_versions: false
       package_name: 'curl'
       groups: [ control-plane, worker, balancer ]
     unzip:
+      cache_versions: false
       package_name: 'unzip'
       groups: []
     kmod:
+      cache_versions: false
       package_name: 'kmod'
       groups: [ control-plane, worker, balancer ]
     semanage:
+      cache_versions: false
       groups: [ control-plane, worker, balancer ]
 
 compatibility_map:
   # This section is filled automatically during Kubemarine work from the following resources:
   # - kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
   # - kubemarine/resources/configurations/compatibility/internal/packages.yaml
   # - kubemarine/resources/configurations/compatibility/internal/plugins.yaml
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.30.0/kubemarine/patches/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
+from kubemarine.patches.preserve_compatibility_kernel import PreserveCompatibilityKernel
+from kubemarine.patches.reinstall_etcdctl_thirdparty import ReinstallEtcdctl
 
+from kubemarine.patches.disable_unattended_upgrade import DisableUnattendedUpgrades
 patches: List[Patch] = [
+    PreserveCompatibilityKernel(),
+    ReinstallEtcdctl(),
+    DisableUnattendedUpgrades()  # Add the new patch to the list
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.30.0/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.30.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.30.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.30.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.30.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.30.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/cluster.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'properties'": "{'patches': OrderedDict([('type', 'array'), ('description', 'Override the "*

 * *                 'resulting configuration for specific nodes. The patches in the list are merged '*

 * *                 'with the global configuration one by one. Thus, the same settings have '*

 * *                 "precedence in the last patch if overridden few times for the same node.'), "*

 * *                 "('items', OrderedDict([('$ref', 'definitions/patch.json')]))])}"}*

```diff
@@ -60,14 +60,21 @@
             "description": "Describe each node of the cluster.",
             "items": {
                 "$ref": "definitions/node.json"
             },
             "minItems": 1,
             "type": "array"
         },
+        "patches": {
+            "description": "Override the resulting configuration for specific nodes. The patches in the list are merged with the global configuration one by one. Thus, the same settings have precedence in the last patch if overridden few times for the same node.",
+            "items": {
+                "$ref": "definitions/patch.json"
+            },
+            "type": "array"
+        },
         "plugin_defaults": {
             "$ref": "definitions/plugin_defaults.json"
         },
         "plugins": {
             "$ref": "definitions/plugins.json"
         },
         "procedure_history": {
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('ArrayOfStrings', OrderedDict([('type', 'array'), "*

 * *                  "('items', OrderedDict([('type', 'string')]))])), ('NonEmptyArrayOfStrings', "*

 * *                  "OrderedDict([('type', 'array'), ('items', OrderedDict([('type', 'string')])), "*

 * *                  "('minItems', 1)])), ('SetOfStrings', OrderedDict([('type', 'array'), ('items', "*

 * *                  "OrderedDict([('type', 'string')])), ('uniqueItems', True)])), "*

 * *                  "('NonEmptySetOfStri […]*

```diff
@@ -1,85 +1,100 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
-        "ControlPlane": {
-            "enum": [
-                "control-plane"
-            ]
+        "ArrayOfObjects": {
+            "items": {
+                "type": "object"
+            },
+            "type": "array"
         },
-        "ControlPlanes": {
+        "ArrayOfStrings": {
             "items": {
-                "$ref": "#/definitions/ControlPlane"
+                "type": "string"
             },
-            "minItems": 1,
-            "type": "array",
-            "uniqueItems": true
+            "type": "array"
         },
-        "Kubernetes": {
+        "ListMergingDefinition": {
+            "default": "replace",
+            "description": "Specify '<<' instead of <<. List merging strategy.",
             "enum": [
-                "worker",
-                "control-plane"
+                "replace",
+                "merge"
             ]
         },
-        "KubernetesRoles": {
+        "ListMergingSymbol": {
+            "additionalProperties": false,
+            "properties": {
+                "<<": {
+                    "$ref": "#/definitions/ListMergingDefinition"
+                }
+            },
+            "required": [
+                "<<"
+            ],
+            "type": "object"
+        },
+        "MergeableArrayOfObjects": {
             "items": {
-                "$ref": "#/definitions/Kubernetes"
+                "oneOf": [
+                    {
+                        "propertyNames": {
+                            "not": {
+                                "enum": [
+                                    "<<"
+                                ]
+                            }
+                        },
+                        "type": "object"
+                    },
+                    {
+                        "$ref": "#/definitions/ListMergingSymbol"
+                    }
+                ]
+            },
+            "type": "array"
+        },
+        "MergeableSetOfStrings": {
+            "items": {
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "$ref": "../common/utils.json#/definitions/ListMergingSymbol"
+                    }
+                ]
             },
-            "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
-        "Name": {
-            "type": "string"
+        "NonEmptyArrayOfObjects": {
+            "items": {
+                "type": "object"
+            },
+            "minItems": 1,
+            "type": "array"
+        },
+        "NonEmptyArrayOfStrings": {
+            "items": {
+                "type": "string"
+            },
+            "minItems": 1,
+            "type": "array"
         },
-        "Names": {
+        "NonEmptySetOfStrings": {
             "items": {
-                "$ref": "#/definitions/Name"
+                "type": "string"
             },
             "minItems": 1,
             "type": "array",
             "uniqueItems": true
         },
-        "OneOfNodesGroupsSpec": {
-            "oneOf": [
-                {
-                    "properties": {
-                        "groups": {
-                            "type": "array"
-                        }
-                    },
-                    "required": [
-                        "groups"
-                    ],
-                    "type": "object"
-                },
-                {
-                    "properties": {
-                        "nodes": {
-                            "type": "array"
-                        }
-                    },
-                    "required": [
-                        "nodes"
-                    ],
-                    "type": "object"
-                }
-            ]
-        },
-        "Role": {
-            "enum": [
-                "worker",
-                "control-plane",
-                "master",
-                "balancer"
-            ]
-        },
-        "Roles": {
+        "SetOfStrings": {
             "items": {
-                "$ref": "#/definitions/Role"
+                "type": "string"
             },
-            "minItems": 1,
             "type": "array",
             "uniqueItems": true
         }
     }
 }
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('OSFamilyModules', OrderedDict([('type', 'array'), "*

 * *                  "('description', 'Manage Linux Kernel modules to be loaded in the host operating "*

 * *                  'system. Each item can be either a module name, or dictionary with the module '*

 * *                  "name and additional parameters.'), ('items', OrderedDict([('anyOf', "*

 * *                  "[OrderedDict([('type', 'string'), ('enum', ['br_netfilter', 'ip6table_filter', "*

 * *                  "'nf_connt […]*

```diff
@@ -1,100 +1,101 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
-        "ArrayOfObjects": {
-            "items": {
-                "type": "object"
-            },
-            "type": "array"
-        },
-        "ArrayOfStrings": {
-            "items": {
-                "type": "string"
-            },
-            "type": "array"
-        },
-        "ListMergingDefinition": {
-            "default": "replace",
-            "description": "Specify '<<' instead of <<. List merging strategy.",
-            "enum": [
-                "replace",
-                "merge"
-            ]
-        },
-        "ListMergingSymbol": {
+        "FilteredModule": {
             "additionalProperties": false,
             "properties": {
-                "<<": {
-                    "$ref": "#/definitions/ListMergingDefinition"
+                "groups": {
+                    "$ref": "../common/node_ref.json#/definitions/Roles",
+                    "default": [
+                        "worker",
+                        "control-plane",
+                        "balancer"
+                    ],
+                    "description": "The list of group names in whose hosts the module should be loaded"
+                },
+                "install": {
+                    "default": "true",
+                    "description": "Whether the module is managed (installed, checked) by Kubemarine",
+                    "type": [
+                        "string",
+                        "boolean"
+                    ]
+                },
+                "modulename": {
+                    "description": "Module name in extended format",
+                    "type": "string"
+                },
+                "nodes": {
+                    "$ref": "../common/node_ref.json#/definitions/Names",
+                    "description": "The list of node names where the module should be loaded"
                 }
             },
             "required": [
-                "<<"
+                "modulename"
             ],
             "type": "object"
         },
-        "MergeableArrayOfObjects": {
+        "OSFamilyModules": {
+            "description": "Manage Linux Kernel modules to be loaded in the host operating system. Each item can be either a module name, or dictionary with the module name and additional parameters.",
             "items": {
-                "oneOf": [
+                "anyOf": [
                     {
-                        "propertyNames": {
-                            "not": {
-                                "enum": [
-                                    "<<"
-                                ]
-                            }
-                        },
-                        "type": "object"
+                        "enum": [
+                            "br_netfilter",
+                            "ip6table_filter",
+                            "nf_conntrack_ipv6",
+                            "nf_nat_masquerade_ipv6",
+                            "nf_reject_ipv6",
+                            "nf_defrag_ipv6",
+                            "nf_nat",
+                            "nf_conntrack"
+                        ],
+                        "type": "string"
                     },
                     {
-                        "$ref": "#/definitions/ListMergingSymbol"
-                    }
-                ]
-            },
-            "type": "array"
-        },
-        "MergeableSetOfStrings": {
-            "items": {
-                "oneOf": [
-                    {
                         "type": "string"
                     },
                     {
-                        "$ref": "../common/utils.json#/definitions/ListMergingSymbol"
+                        "oneOf": [
+                            {
+                                "$ref": "#/definitions/FilteredModule"
+                            },
+                            {
+                                "$ref": "../common/utils.json#/definitions/ListMergingSymbol"
+                            }
+                        ]
                     }
                 ]
             },
             "type": "array",
             "uniqueItems": true
+        }
+    },
+    "properties": {
+        "debian": {
+            "$ref": "#/definitions/OSFamilyModules"
         },
-        "NonEmptyArrayOfObjects": {
-            "items": {
-                "type": "object"
-            },
-            "minItems": 1,
-            "type": "array"
+        "rhel": {
+            "$ref": "#/definitions/OSFamilyModules"
         },
-        "NonEmptyArrayOfStrings": {
-            "items": {
-                "type": "string"
-            },
-            "minItems": 1,
-            "type": "array"
+        "rhel8": {
+            "$ref": "#/definitions/OSFamilyModules"
         },
-        "NonEmptySetOfStrings": {
-            "items": {
-                "type": "string"
-            },
-            "minItems": 1,
-            "type": "array",
-            "uniqueItems": true
-        },
-        "SetOfStrings": {
-            "items": {
-                "type": "string"
-            },
-            "type": "array",
-            "uniqueItems": true
+        "rhel9": {
+            "$ref": "#/definitions/OSFamilyModules"
         }
-    }
+    },
+    "propertyNames": {
+        "anyOf": [
+            {
+                "enum": [
+                    "debian",
+                    "rhel",
+                    "rhel8",
+                    "rhel9"
+                ]
+            }
+        ]
+    },
+    "type": "object"
 }
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'definitions'": "{'Properties': {'properties': {'roles': {'$ref': "*

 * *                  "'common/node_ref.json#/definitions/DeprecatedRoles'}}}}"}*

```diff
@@ -54,15 +54,15 @@
             "properties": {
                 "control_endpoint": {
                     "default": false,
                     "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
                     "type": "boolean"
                 },
                 "roles": {
-                    "$ref": "common/node_ref.json#/definitions/Roles",
+                    "$ref": "common/node_ref.json#/definitions/DeprecatedRoles",
                     "description": "Cluster member roles"
                 }
             }
         },
         "PropertyNames": {
             "anyOf": [
                 {
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238096%*

 * *Differences: {"'definitions'": "{'OneOfKeyfilePasswordSpec': {'type': 'object'}}"}*

```diff
@@ -102,15 +102,16 @@
                         }
                     },
                     "required": [
                         "password"
                     ],
                     "type": "object"
                 }
-            ]
+            ],
+            "type": "object"
         },
         "SSHAccessCommonProperties": {
             "properties": {
                 "connection_port": {
                     "default": 22,
                     "description": "Port for SSH-connection to remote machine(s)",
                     "maximum": 65535,
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333332%*

 * *Differences: {"'oneOf'": "{1: {'properties': {'groups': {'$ref': "*

 * *            "'../../common/node_ref.json#/definitions/DeprecatedRoles'}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "properties": {
                 "become": {
                     "default": false,
                     "description": "Privilege escalation switch. Enables -b argument.",
                     "type": "boolean"
                 },
                 "groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "$ref": "../../common/node_ref.json#/definitions/DeprecatedRoles",
                     "description": "Targeted list of groups, passed to Ansible as --limit argument"
                 },
                 "nodes": {
                     "$ref": "../../common/node_ref.json#/definitions/Names",
                     "description": "Targeted list of nodes, passed to Ansible as --limit argument"
                 },
                 "playbook": {
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999782986111111%*

 * *Differences: {"'oneOf'": "{1: {'properties': {'groups': {'$ref': "*

 * *            "'../../common/node_ref.json#/definitions/DeprecatedRoles'}}}}"}*

```diff
@@ -23,15 +23,15 @@
                             },
                             "minItems": 1,
                             "type": "array"
                         }
                     ]
                 },
                 "groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "$ref": "../../common/node_ref.json#/definitions/DeprecatedRoles",
                     "description": "List of groups on which the shell command should be executed"
                 },
                 "in_vars": {
                     "description": "List of ENV variables to import before command execution",
                     "items": {
                         "additionalProperties": false,
                         "properties": {
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'definitions'": "{'Properties': {'properties': {'destination_groups': {'$ref': "*

 * *                  "'../../common/node_ref.json#/definitions/DeprecatedRoles'}, 'apply_groups': "*

 * *                  "{'$ref': '../../common/node_ref.json#/definitions/DeprecatedRoles'}}}}"}*

```diff
@@ -4,15 +4,15 @@
         "Properties": {
             "properties": {
                 "apply_command": {
                     "description": "The command to apply the template on remote hosts after uploading it. It is called only if the switch apply_required is on.",
                     "type": "string"
                 },
                 "apply_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "$ref": "../../common/node_ref.json#/definitions/DeprecatedRoles",
                     "description": "List of groups on which the template apply command needs to be executed"
                 },
                 "apply_nodes": {
                     "$ref": "../../common/node_ref.json#/definitions/Names",
                     "description": "List of nodes on which the template apply command needs to be executed"
                 },
                 "apply_required": {
@@ -21,15 +21,15 @@
                     "type": "boolean"
                 },
                 "destination": {
                     "description": "The absolute path on the hosts where the compiled template needs to be uploaded",
                     "type": "string"
                 },
                 "destination_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "$ref": "../../common/node_ref.json#/definitions/DeprecatedRoles",
                     "description": "List of groups on which the compiled template needs to be uploaded"
                 },
                 "destination_nodes": {
                     "$ref": "../../common/node_ref.json#/definitions/Names",
                     "description": "List of nodes on which the compiled template needs to be uploaded"
                 },
                 "source": {
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9388888888888889%*

 * *Differences: {"'definitions'": "{'PodPidsLimit': OrderedDict([('type', 'integer'), ('default', 4096)]), "*

 * *                  "'MaxPods': OrderedDict([('type', 'integer'), ('default', 110)])}",*

 * * "'properties'": "{'podPidsLimit': {replace: OrderedDict([('$ref', "*

 * *                 "'#/definitions/PodPidsLimit')])}, 'maxPods': {replace: OrderedDict([('$ref', "*

 * *                 "'#/definitions/MaxPods')])}}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
+        "MaxPods": {
+            "default": 110,
+            "type": "integer"
+        },
+        "PodPidsLimit": {
+            "default": 4096,
+            "type": "integer"
+        },
         "ProtectKernelDefaults": {
             "default": true,
             "type": "boolean"
         },
         "SerializeImagePulls": {
             "default": false,
             "type": "boolean"
@@ -29,20 +37,18 @@
         "kind": {
             "default": "KubeletConfiguration",
             "enum": [
                 "KubeletConfiguration"
             ]
         },
         "maxPods": {
-            "default": 110,
-            "type": "integer"
+            "$ref": "#/definitions/MaxPods"
         },
         "podPidsLimit": {
-            "default": 4096,
-            "type": "integer"
+            "$ref": "#/definitions/PodPidsLimit"
         },
         "protectKernelDefaults": {
             "$ref": "#/definitions/ProtectKernelDefaults"
         },
         "readOnlyPort": {
             "default": 0,
             "type": "integer"
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999977394386574%*

 * *Differences: {"'definitions'": "{'kubelet-patch': {'items': {'oneOf': {0: {'allOf': {1: {'properties': "*

 * *                  "{'patch': {replace: OrderedDict([('allOf', [OrderedDict([('$ref', "*

 * *                  "'#/definitions/patch')])]), ('properties', OrderedDict([('podPidsLimit', "*

 * *                  "OrderedDict([('$ref', 'kubeadm_kubelet.json#/definitions/PodPidsLimit')])), "*

 * *                  "('maxPods', OrderedDict([('$ref', "*

 * *                  "'kubeadm_kubelet.json#/definitions/MaxPods')]))]))])}}}}}}}}}"}*

```diff
@@ -54,15 +54,27 @@
                                     "groups": {
                                         "$ref": "../common/node_ref.json#/definitions/KubernetesRoles"
                                     },
                                     "nodes": {
                                         "$ref": "../common/node_ref.json#/definitions/Names"
                                     },
                                     "patch": {
-                                        "$ref": "#/definitions/patch"
+                                        "allOf": [
+                                            {
+                                                "$ref": "#/definitions/patch"
+                                            }
+                                        ],
+                                        "properties": {
+                                            "maxPods": {
+                                                "$ref": "kubeadm_kubelet.json#/definitions/MaxPods"
+                                            },
+                                            "podPidsLimit": {
+                                                "$ref": "kubeadm_kubelet.json#/definitions/PodPidsLimit"
+                                            }
+                                        }
                                     }
                                 },
                                 "required": [
                                     "patch"
                                 ],
                                 "type": "object"
                             }
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999937996031747%*

 * *Differences: {"'definitions'": "{'ThirdParty': {'oneOf': {1: {'properties': {'group': {'$ref': "*

 * *                  "'../common/node_ref.json#/definitions/DeprecatedRole'}, 'groups': {'$ref': "*

 * *                  "'../common/node_ref.json#/definitions/DeprecatedRoles'}}}}}}"}*

```diff
@@ -32,19 +32,19 @@
                     "allOf": [
                         {
                             "$ref": "#/definitions/MinimalThirdPartyProperties"
                         }
                     ],
                     "properties": {
                         "group": {
-                            "$ref": "../common/node_ref.json#/definitions/Role",
+                            "$ref": "../common/node_ref.json#/definitions/DeprecatedRole",
                             "description": "The name of the group to whose hosts the file should be uploaded"
                         },
                         "groups": {
-                            "$ref": "../common/node_ref.json#/definitions/Roles",
+                            "$ref": "../common/node_ref.json#/definitions/DeprecatedRoles",
                             "description": "The list of group names to whose hosts the file should be uploaded"
                         },
                         "mode": {
                             "default": "700",
                             "description": "The mode which needs to be assigned to the file after downloading it",
                             "type": [
                                 "string",
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/internal/connections.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/internal/connections.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/reconfigure.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/reconfigure.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.30.0/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.30.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.30.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.30.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files 21% similar despite different names*

```diff
@@ -28,60 +28,89 @@
     echo "Unable to find etcd configuration neither in kubernetes nor on host, exiting with error..."
     exit 1
   fi
 fi
 
 # If any pod configuration detected
 if [ -n "${ETCD_POD_CONFIG}" ]; then
-  ETCD_IMAGE=$(echo "${ETCD_POD_CONFIG}" | grep ' image:' | awk '{print $2; exit}')
-  ETCD_MOUNTS=""
-  ETCD_MOUNTS_RAW=$(echo "${ETCD_POD_CONFIG}" | grep ' mountPath: ')
   ETCD_CERT=$(echo "${ETCD_POD_CONFIG}" | grep '\- --cert-file' | sed s/=/\\n/g | sed -n 2p)
   ETCD_KEY=$(echo "${ETCD_POD_CONFIG}" | grep '\- --key-file' | sed s/=/\\n/g | sed -n 2p)
   ETCD_CA=$(echo "${ETCD_POD_CONFIG}" | grep '\- --trusted-ca-file' | sed s/=/\\n/g | sed -n 2p)
   ETCD_ENDPOINTS=$(echo "${ETCD_POD_CONFIG}" | grep '\- --initial-cluster=' | sed -e 's/\s*- --initial-cluster=//g' -e "s/[a-zA-Z0-9\.-]*=//g" -e "s/2380/2379/g")
-  while IFS= read -r line; do
-      volume=$(echo "${line}" | awk '{print $3; exit}')
-      if [ "$CONT_RUNTIME" == "ctr" ]; then
-        ETCD_MOUNTS="${ETCD_MOUNTS} -mount type=bind,src=${volume},dst=${volume},options=rbind:rw"
-      else
-        ETCD_MOUNTS="${ETCD_MOUNTS} -v ${volume}:${volume}"
-      fi
-  done <<< "${ETCD_MOUNTS_RAW}"
+  if [ -z "${ETCD_IMAGE}" ];then
+    ETCD_IMAGE=$(echo "${ETCD_POD_CONFIG}" | grep ' image:' | awk '{print $2; exit}')
+  fi
+  if [ -z "${ETCD_MOUNTS}" ];then
+    ETCD_MOUNTS=""
+    ETCD_MOUNTS_RAW=$(echo "${ETCD_POD_CONFIG}" | grep ' mountPath: ')
+    while IFS= read -r line; do
+        volume=$(echo "${line}" | awk '{print $3; exit}')
+        if [ "$CONT_RUNTIME" == "ctr" ]; then
+          ETCD_MOUNTS="${ETCD_MOUNTS} -mount type=bind,src=${volume},dst=${volume},options=rbind:rw"
+        else
+          ETCD_MOUNTS="${ETCD_MOUNTS} -v ${volume}:${volume}"
+        fi
+    done <<< "${ETCD_MOUNTS_RAW}"
+  fi
 
   # User can override some of our "default" etcdctl args (see cases).
   # If user passed his own arg, then our "default" arg will be NULLed.
   USER_ARGS=("$@")
-  opts=$(getopt --quiet --longoptions "endpoints:," -- "$@")
+  opts=$(getopt --quiet --longoptions "cert:,key:,cacert:,endpoints:" -o '' -- "$@")
   eval set --$opts
   while [[ $# -gt 0 ]]; do
     case "$1" in
+      --cert)
+        ETCD_CERT=""
+        shift 2
+        ;;
+      --key)
+        ETCD_KEY=""
+        shift 2
+        ;;
+      --cacert)
+        ETCD_CA=""
+        shift 2
+        ;;
       --endpoints)
         ETCD_ENDPOINTS=""
         shift 2
         ;;
+      --)
+        # skip remained options
+        break
+        ;;
       *)
         # skip unknown options
         shift 1
         ;;
     esac
   done
   # If our default arg is not NULLed, then user did not provided his own flag and we should append our default.
   # Otherwise arg is already provided by user and thus our default arg should not be appended.
+  if [ -n "$ETCD_CERT" ]; then
+    USER_ARGS+=("--cert=$ETCD_CERT")
+  fi
+  if [ -n "$ETCD_KEY" ]; then
+    USER_ARGS+=("--key=$ETCD_KEY")
+  fi
+  if [ -n "$ETCD_CA" ]; then
+    USER_ARGS+=("--cacert=$ETCD_CA")
+  fi
   if [ -n "$ETCD_ENDPOINTS" ]; then
     USER_ARGS+=("--endpoints=$ETCD_ENDPOINTS")
   fi
 
   if [ "$CONT_RUNTIME" == "ctr" ]; then
     ETCD_REGISTRY=$(echo ${ETCD_IMAGE} | cut -d "/" -f1)
     ctr_default_pull_opts=$(cat /etc/ctr/kubemarine_ctr_flags.conf |  grep "^*=" | sed "s/^*=//;")
     ctr_pull_opts=$(cat /etc/ctr/kubemarine_ctr_flags.conf |  grep "^${ETCD_REGISTRY}=" | sed "s/^${ETCD_REGISTRY}=//;")
     container_name="etcdctl-$(cat /proc/sys/kernel/random/uuid | sed 's/[-]//g' | head -c 20; echo;)"
     ctr image pull ${ctr_default_pull_opts} ${ctr_pull_opts} ${ETCD_IMAGE} > /dev/null 2&>1
     ctr run --net-host --rm ${ETCD_MOUNTS} --env ETCDCTL_API=3 ${ETCD_IMAGE} $container_name \
-	    etcdctl --cert=${ETCD_CERT} --key=${ETCD_KEY} --cacert=${ETCD_CA} "${USER_ARGS[@]}"
+	    etcdctl "${USER_ARGS[@]}"
   else
     docker run --rm ${ETCD_MOUNTS} -e ETCDCTL_API=3 ${ETCD_IMAGE} \
-	    etcdctl --cert=${ETCD_CERT} --key=${ETCD_KEY} --cacert=${ETCD_CA} "${USER_ARGS[@]}"
+	    etcdctl "${USER_ARGS[@]}"
   fi
   exit $?
 fi
```

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_client.py` & `kubemarine-0.30.0/kubemarine/resources/scripts/simple_port_client.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/simple_port_listener.py` & `kubemarine-0.30.0/kubemarine/resources/scripts/simple_port_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/go.sum` & `kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/go.sum`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go` & `kubemarine-0.30.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go`

 * *Files 10% similar despite different names*

```diff
@@ -29,39 +29,41 @@
 	"github.com/google/gopacket"
 	"github.com/google/gopacket/layers"
 )
 
 var (
 	mode, msg, src, dstExt, dstInt string
 	srcIP, dstExtIP, dstIntIP net.IP
-	dport, timeout uint
+	sport, dport, timeout uint
 )
 
 func customUsage() {
 	fmt.Printf("Usage of %s:\n", os.Args[0])
-	fmt.Printf("%s -mode client -src 192.168.0.1 -ext 192.168.0.2 -int 240.0.0.1 -dport 54545 -msg Message -timeout 10\n",
+	fmt.Printf("%s -mode client -src 192.168.0.1 -ext 192.168.0.2 -int 240.0.0.1 -sport 45455 -dport 54545 -msg Message -timeout 10\n",
 	      os.Args[0])
-	fmt.Printf("%s -mode server -ext 192.168.0.2 -int 240.0.0.1 -dport 54545 -msg Message -timeout 3\n",
+	fmt.Printf("%s -mode server -ext 192.168.0.2 -int 240.0.0.1 -sport 45455 -dport 54545 -msg Message -timeout 3\n",
 	      os.Args[0])
 	fmt.Println("Where:")
 	flag.PrintDefaults()
+	fmt.Println("Note: Pay attention to the fact that some implementations of packet filters might includes rule that allows 'related' traffic (eg.: Security Groups implementation in OpenStack). That means the mode changing on the same host might lead to incorrect results of the check.")
 }
 
 func parseParam() error {
 	flag.Usage = customUsage
 	// Server or client mode. Server gets and parses IPIP pakets, and client sends IPIP pakets
 	flag.StringVar(&mode, "mode", "", "Server or client mode")
 	// External source IP (Src IP)
 	flag.StringVar(&src, "src", "", "External source IP address")
 	// External destination IP (DstExt IP)
 	flag.StringVar(&dstExt, "ext", "", "External destination IP address")
 	// Internal destination IP (DstInt IP)
 	flag.StringVar(&dstInt, "int", "", "Internal destination IP address")
 	// UDP port number (UDP Dst Port)
 	flag.UintVar(&dport, "dport", 65000, "Destination UDP port")
+	flag.UintVar(&sport, "sport", 53, "Source UDP port")
 	flag.UintVar(&timeout, "timeout", 0, "Operation timeout")
 	flag.StringVar(&msg, "msg", "", "Message as UDP payload")
 	flag.Parse()
 	if mode != "server" && mode != "client" {
 		return errors.New("Unknown mode. It might be 'server' or 'client'")
 	}
 	srcIP = net.ParseIP(src)
@@ -72,28 +74,32 @@
 	if dstExtIP == nil {
 		return errors.New("External destination address is invalid")
 	}
 	dstIntIP = net.ParseIP(dstInt)
 	if dstIntIP == nil {
 		return errors.New("Internal destination address is invalid")
 	}
+	if sport > 65535 {
+		return errors.New("Source UDP port out of range")
+	}
 	if dport > 65535 {
 		return errors.New("Destination UDP port out of range")
 	}
 	if len(msg) > 1000 {
 		return errors.New("Message is too long")
 	}
 	return nil
 }
 
 func runSrv() {
 
 	dstExtIPaddr := net.IPAddr{
 		IP: dstExtIP,
 	}
+	srcUDPPort := layers.UDPPort(sport)
 	dstUDPPort := layers.UDPPort(dport)
 	// Listen on the external IP address. The payload protocol is IPIP
 	ipConn, err := net.ListenIP("ip4:4", &dstExtIPaddr)
 	if err != nil {
                 fmt.Println(err)
 		os.Exit(1)
 	}
@@ -127,15 +133,16 @@
 			dstIntIP := fmt.Sprintf("%s", ipIntPacket.DstIP)
 			// Check if destination IP matches with 'Interal IP' parameter
 			if  dstInt == dstIntIP {
 				// Check UDP port
 				if packet.Layers()[1].LayerType() == layers.LayerTypeUDP {
 					udpLayer := packet.Layers()[1]
 					udpPacket := udpLayer.(*layers.UDP)
-					if udpPacket.DstPort == dstUDPPort {
+					if udpPacket.DstPort == dstUDPPort &&
+					   udpPacket.SrcPort == srcUDPPort {
 						payload := fmt.Sprintf("%s", packet.Layers()[1].LayerPayload())
 						// Check UDP paylaod
 						if payload == msg {
 							fmt.Println(srcIntIP)
 						}
 					}
 				}
@@ -158,15 +165,15 @@
 		DstIP:    dstIntIP,
 		Version:  4,
 		IHL:      5,
 		Protocol: layers.IPProtocolUDP,
 	}
 	// Describe UDP packet
 	udpLayer := layers.UDP{
-		SrcPort: layers.UDPPort(53),
+		SrcPort: layers.UDPPort(uint16(sport)),
 		DstPort: layers.UDPPort(uint16(dport)),
 	}
 	udpLayer.SetNetworkLayerForChecksum(&ipLayer2)
 	buf := gopacket.NewSerializeBuffer()
 	opts := gopacket.SerializeOptions{
 		ComputeChecksums: true,
 		FixLengths:       true,
```

### Comparing `kubemarine-0.29.0/kubemarine/selinux.py` & `kubemarine-0.30.0/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/system.py` & `kubemarine-0.30.0/kubemarine/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,24 +527,30 @@
         log.debug(modprobe_result)
         if not modprobe_valid:
             raise Exception("Required kernel modules are not presented")
     else:
         log.debug('Modprobe verification skipped - origin setup task was not completed')
 
     if cluster.is_task_completed('prepare.system.sysctl'):
-        log.debug("Verifying kernel parameters...")
-        sysctl_valid = sysctl.is_valid(group)
-        if not sysctl_valid:
-            raise Exception("Required kernel parameters are not presented")
-        else:
-            log.debug("Required kernel parameters are presented")
+        verify_sysctl(group)
     else:
         log.debug('Kernel parameters verification skipped - origin setup task was not completed')
 
 
+def verify_sysctl(group: NodeGroup) -> None:
+    cluster: KubernetesCluster = group.cluster
+
+    cluster.log.debug("Verifying kernel parameters...")
+    sysctl_valid = sysctl.is_valid(group)
+    if not sysctl_valid:
+        raise Exception("Required kernel parameters are not presented")
+    else:
+        cluster.log.debug("Required kernel parameters are presented")
+
+
 def detect_active_interface(cluster: KubernetesCluster) -> None:
     group = cluster.make_group(cluster.nodes_context).get_accessible_nodes()
     collector = CollectorCallback(cluster)
     with group.new_executor() as exe:
         for node in exe.group.get_ordered_members_list():
             detect_interface_by_address(node, node.get_config()['internal_address'], collector=collector)
```

### Comparing `kubemarine-0.29.0/kubemarine/templates/__init__.py` & `kubemarine-0.30.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.30.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.30.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.30.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.30.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.30.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/testsuite.py` & `kubemarine-0.30.0/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/thirdparties.py` & `kubemarine-0.30.0/kubemarine/thirdparties.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine/yum.py` & `kubemarine-0.30.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.29.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.30.0/kubemarine.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.29.0
+Version: 0.30.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -27,15 +27,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.*
 Requires-Dist: deepmerge==1.1.*
 Requires-Dist: fabric==3.2.*
 Requires-Dist: jinja2==3.1.*
 Requires-Dist: MarkupSafe==2.1.*
 Requires-Dist: invoke==2.2.*
-Requires-Dist: ruamel.yaml==0.17.22
+Requires-Dist: ruamel.yaml==0.18.*
 Requires-Dist: pygelf==0.4.*
 Requires-Dist: toml==0.10.*
 Requires-Dist: python-dateutil==2.8.*
 Requires-Dist: deepdiff==6.7.*
 Requires-Dist: ordered-set==4.1.*
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: paramiko==3.3.*
@@ -63,38 +63,38 @@
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -112,15 +112,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -131,15 +131,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -160,24 +160,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -206,42 +206,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.29.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.30.0/LICENSE)
```

### Comparing `kubemarine-0.29.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.30.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,19 @@
 kubemarine/core/connections.py
 kubemarine/core/defaults.py
 kubemarine/core/environment.py
 kubemarine/core/errors.py
 kubemarine/core/executor.py
 kubemarine/core/flow.py
 kubemarine/core/group.py
+kubemarine/core/inventory.py
 kubemarine/core/log.py
 kubemarine/core/os.py
 kubemarine/core/patch.py
+kubemarine/core/proxytypes.py
 kubemarine/core/resources.py
 kubemarine/core/schema.py
 kubemarine/core/static.py
 kubemarine/core/summary.py
 kubemarine/core/utils.py
 kubemarine/core/yaml_merger.py
 kubemarine/cri/__init__.py
@@ -64,17 +66,18 @@
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/secrets.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
-kubemarine/patches/boot_timeout_per_node.py
+kubemarine/patches/disable_unattended_upgrade.py
+kubemarine/patches/preserve_compatibility_kernel.py
+kubemarine/patches/reinstall_etcdctl_thirdparty.py
 kubemarine/patches/software_upgrade.yaml
-kubemarine/patches/strong_cipher_suits_for_kubelet.py
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
@@ -157,14 +160,15 @@
 kubemarine/resources/schemas/remove_node.json
 kubemarine/resources/schemas/restore.json
 kubemarine/resources/schemas/upgrade.json
 kubemarine/resources/schemas/definitions/gateway_node.json
 kubemarine/resources/schemas/definitions/globals.json
 kubemarine/resources/schemas/definitions/node.json
 kubemarine/resources/schemas/definitions/node_defaults.json
+kubemarine/resources/schemas/definitions/patch.json
 kubemarine/resources/schemas/definitions/plugin_defaults.json
 kubemarine/resources/schemas/definitions/plugins.json
 kubemarine/resources/schemas/definitions/procedures.json
 kubemarine/resources/schemas/definitions/rbac.json
 kubemarine/resources/schemas/definitions/registry.json
 kubemarine/resources/schemas/definitions/services.json
 kubemarine/resources/schemas/definitions/vrrp_ip.json
```

### Comparing `kubemarine-0.29.0/kubemarine.egg-info/requires.txt` & `kubemarine-0.30.0/kubemarine.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 PyYAML==6.0.*
 deepmerge==1.1.*
 fabric==3.2.*
 jinja2==3.1.*
 MarkupSafe==2.1.*
 invoke==2.2.*
-ruamel.yaml==0.17.22
+ruamel.yaml==0.18.*
 pygelf==0.4.*
 toml==0.10.*
 python-dateutil==2.8.*
 deepdiff==6.7.*
 ordered-set==4.1.*
 cryptography==42.0.4
 paramiko==3.3.*
```

### Comparing `kubemarine-0.29.0/pyproject.toml` & `kubemarine-0.30.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 dependencies = [
     "PyYAML==6.0.*",
     "deepmerge==1.1.*",
     "fabric==3.2.*",
     "jinja2==3.1.*",
     "MarkupSafe==2.1.*",
     "invoke==2.2.*",
-    "ruamel.yaml==0.17.22",
+    "ruamel.yaml==0.18.*",
     "pygelf==0.4.*",
     "toml==0.10.*",
     "python-dateutil==2.8.*",
     "deepdiff==6.7.*",
     "ordered-set==4.1.*",
     # Each time cryptography version is updated, need to regenerate scripts/ci/custom-hooks/hook-cryptography.py
     "cryptography==42.0.4",
@@ -79,15 +79,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "v0.29.0"
+current_version = "v0.30.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.29.0/setup.py` & `kubemarine-0.30.0/setup.py`

 * *Files identical despite different names*

