# Comparing `tmp/smol_k8s_lab-4.0.2.tar.gz` & `tmp/smol_k8s_lab-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-4.0.2.tar", max compression
+gzip compressed data, was "smol_k8s_lab-5.0.0.tar", max compression
```

## Comparing `smol_k8s_lab-4.0.2.tar` & `smol_k8s_lab-5.0.0.tar`

### file list

```diff
@@ -1,109 +1,117 @@
--rw-r--r--   0        0        0    34260 2024-04-09 07:42:46.143312 smol_k8s_lab-4.0.2/LICENSE
--rw-r--r--   0        0        0    27169 2024-04-09 07:42:46.143312 smol_k8s_lab-4.0.2/README.md
--rw-r--r--   0        0        0     2264 2024-04-09 07:42:46.391313 smol_k8s_lab-4.0.2/pyproject.toml
--rwxr-xr-x   0        0        0    15143 2024-04-09 07:42:46.391313 smol_k8s_lab-4.0.2/smol_k8s_lab/__init__.py
--rwxr-xr-x   0        0        0    12779 2024-04-09 07:42:46.391313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-04-09 07:42:46.391313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    64187 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5675 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rwxr-xr-x   0        0        0     2318 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9486 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6716 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0    10293 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    14554 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20412 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3370 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1860 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1761 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    11178 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2543 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0      591 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/k8up_operater.py
--rw-r--r--   0        0        0      573 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/longhorn.py
--rw-r--r--   0        0        0    16270 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     4471 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0      520 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/prometheus.py
--rw-r--r--   0        0        0     4590 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2671 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3889 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     5089 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0     4974 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    15769 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1702 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    12253 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    13293 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     4129 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     6497 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3751 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     7779 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4817 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     5548 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/argocd_util.py
--rwxr-xr-x   0        0        0     8032 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    10312 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0      219 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/k9s.py
--rw-r--r--   0        0        0     1358 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    10866 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     7501 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0     6827 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     3533 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6904 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3763 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    10680 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    21507 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0     6151 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/base_cluster_modal.py
--rwxr-xr-x   0        0        0     8373 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0      925 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     6076 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1561 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6386 2024-04-09 07:42:46.395313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1116 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      867 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      855 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     1940 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1720 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1247 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3096 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2683 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10237 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    11500 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    13289 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4509 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4210 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     3733 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0     7714 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0    10049 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9388 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0     1184 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4624 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/rich_cli/help_text.py
--rwxr-xr-x   0        0        0     7215 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/subproc.py
--rw-r--r--   0        0        0      315 2024-04-09 07:42:46.399313 smol_k8s_lab-4.0.2/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    28815 1970-01-01 00:00:00.000000 smol_k8s_lab-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-15 10:15:14.083655 smol_k8s_lab-5.0.0/LICENSE
+-rw-r--r--   0        0        0    27183 2024-05-15 10:15:14.083655 smol_k8s_lab-5.0.0/README.md
+-rw-r--r--   0        0        0     3300 2024-05-15 10:15:14.343655 smol_k8s_lab-5.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0    16188 2024-05-15 10:15:14.343655 smol_k8s_lab-5.0.0/smol_k8s_lab/__init__.py
+-rw-r--r--   0        0        0  5853144 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/audio/audio-en.tar.gz
+-rwxr-xr-x   0        0        0    12759 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    17031 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/en.yml
+-rw-r--r--   0        0        0     2364 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/nl.yml
+-rw-r--r--   0        0        0    76932 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5666 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rw-r--r--   0        0        0      831 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
+-rwxr-xr-x   0        0        0     3008 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9821 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     7789 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6581 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0     9763 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    19076 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20511 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3372 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1285 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    10977 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2383 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0     8381 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     3617 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0     4286 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3759 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     4805 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0    11623 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    21465 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1706 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    18842 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    20726 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     6182 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     8034 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3755 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     8481 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4821 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/argocd_util.py
+-rw-r--r--   0        0        0     8689 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/backup.py
+-rwxr-xr-x   0        0        0     8607 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    14252 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0    22222 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/restores.py
+-rw-r--r--   0        0        0     1358 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    14333 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     9712 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0    18578 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
+-rw-r--r--   0        0        0    14373 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     4002 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6970 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3697 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    17623 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    12695 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0    32748 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
+-rw-r--r--   0        0        0     7189 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
+-rw-r--r--   0        0        0     3384 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
+-rwxr-xr-x   0        0        0     8873 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0     1546 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     7174 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1184 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6681 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1371 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      867 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      984 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     2198 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1901 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1259 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3433 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2554 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10434 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    17221 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    14337 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4359 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4138 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     4020 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0    11190 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0     8826 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9872 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0    16300 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/minio_lib.py
+-rw-r--r--   0        0        0     1184 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4720 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/help_text.py
+-rw-r--r--   0        0        0     2610 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/final_cmd.py
+-rwxr-xr-x   0        0        0     7483 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/subproc.py
+-rw-r--r--   0        0        0     2837 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/value_from.py
+-rw-r--r--   0        0        0      315 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    28869 1970-01-01 00:00:00.000000 smol_k8s_lab-5.0.0/PKG-INFO
```

### Comparing `smol_k8s_lab-4.0.2/LICENSE` & `smol_k8s_lab-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/README.md` & `smol_k8s_lab-5.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
 # Installation
-B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` or `brew`.
+B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon).
 
 ## pipx
 `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https://small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able to:
 
 ```bash
 # install the CLI
 pipx install smol-k8s-lab
```

#### html2text {}

```diff
@@ -17,27 +17,27 @@
 (#supported-k8s-distributions) - Specializes in using Bitwarden (though not
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
 hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - Lots o' [docs](https://
 small-hack.github.io/smol-k8s-lab) # Installation B sure to check out our full
 [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
-but the gist of it is `smol-k8s-lab` can be installed via `pipx` or `brew`. ##
-pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
-pipx)). If you've already got both and [other pre-reqs](https://small-
-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
-to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
-before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
-the future preferred installation method for macOS/Debian/Ubuntu, as this will
-also install any non-python prerequisites you need, so you don't need to worry
-about them. This method is new, so please [let us know if anything isn't
-working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
-tap the special homebrew repo for our formula and install it brew install
-small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
-and cli options with: ```bash smol-k8s-lab --help ```
+but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
+coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
+github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
+/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
+able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
+menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
+[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
+as this will also install any non-python prerequisites you need, so you don't
+need to worry about them. This method is new, so please [let us know if
+anything isn't working for you](https://github.com/small-hack/homebrew-tap/
+issues). ```bash # tap the special homebrew repo for our formula and install it
+brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
+the version and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/__init__.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3.11
 """
            NAME: smol-k8s-lab
     DESCRIPTION: package, cli, and tui for setting up k8s on metal with
                  k3s, KinD, and k3d, as well as installing our or your own
                  Argo CD Apps, ApplicationSets, and Projects.
+                 And now we support restores too!
 
          AUTHOR: jessebot(AT)linux(d0t)com
         LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE
 """
 
 from click import option, command
 import logging
@@ -23,31 +24,30 @@
 from .constants import KUBECONFIG, VERSION
 from .k8s_apps import (setup_oidc_provider, setup_base_apps,
                        setup_k8s_secrets_management, setup_federated_apps)
 from .k8s_apps.networking.netmaker import configure_netmaker
 from .k8s_apps.operators import setup_operators
 from .k8s_apps.operators.minio import configure_minio_tenant
 from .k8s_distros import create_k8s_distro, delete_cluster
-from .k8s_tools.argocd_util import install_with_argocd, check_if_argocd_app_exists
 from .tui import launch_config_tui
 from .utils.rich_cli.console_logging import CONSOLE, sub_header, header
 from .utils.rich_cli.help_text import RichCommand, options_help
+from .utils.run.final_cmd import run_final_cmd
 
 
 HELP = options_help()
 HELP_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def process_log_config(log_dict: dict = {"level": "warn", "file": ""}):
     """
     Sets up rich logger for the entire project.
     Returns logging.getLogger("rich")
 
     TODO: change this to always add file logger
-
     """
 
     # determine logging level and default to warning level
     level = log_dict.get("level", "warn")
     log_level = getattr(logging, level.upper(), None)
 
     # these are params to be passed into logging.basicConfig
@@ -104,19 +104,24 @@
         help=HELP['delete'])
 @option("--interactive", "-i",
         is_flag=True,
         help=HELP['interactive'])
 @option("--version", "-v",
         is_flag=True,
         help=HELP['version'])
+@option("--final_cmd", "-f",
+        type=str,
+        default="",
+        help=HELP['command'])
 def main(config: str = "",
          delete: bool = False,
          log_file: str = "",
          version: bool = False,
-         interactive: bool = False):
+         interactive: bool = False,
+         final_cmd: str = ""):
     """
     Quickly install a k8s distro for a homelab setup. Installs k3s
     with metallb, ingess-nginx, cert-manager, and argocd
     """
     # only return the version if --version was passed in
     if version:
         print(f"\n🎉 v{VERSION}\n")
@@ -202,35 +207,43 @@
             selected_distro = distro
             break
 
     # install the actual KIND, k3s, or k3d cluster
     k8s_obj = create_k8s_distro(cluster_name, selected_distro, metadata,
                                 metallb_enabled, cilium_enabled)
 
+    # run the final command immediately after k8s is up, if it's running in a
+    # new tab, window, or pane
+    window_behavior = USR_CFG['smol_k8s_lab']['run_command']['window_behavior']
+    terminal = USR_CFG['smol_k8s_lab']['run_command']['terminal']
+    if not final_cmd:
+        final_cmd = USR_CFG['smol_k8s_lab']['run_command']['command']
+
+    if final_cmd and window_behavior != "same window":
+        run_final_cmd(final_cmd, terminal, window_behavior)
+
     # check if argo is enabled
     argo_enabled = apps['argo_cd']['enabled']
-    # check if zitadel is enabled
-    zitadel_enabled = apps['zitadel']['enabled']
 
     # installs all the base apps: metallb/cilium, ingess-nginx, cert-manager, and argocd
-    setup_base_apps(k8s_obj,
-                    distro,
-                    apps.get('cilium', {}),
-                    apps['metallb'],
-                    apps.pop('ingress_nginx', {}),
-                    apps['cert_manager'],
-                    argo_enabled,
-                    apps['argo_cd']['argo']['directory_recursion'],
-                    SECRETS,
-                    bw)
+    argocd = setup_base_apps(k8s_obj,
+                             distro,
+                             apps.get('cilium', {}),
+                             apps['metallb'],
+                             apps.pop('ingress_nginx', {}),
+                             apps.pop('cert_manager', {}),
+                             apps.get('cnpg_operator', {}),
+                             apps['argo_cd'],
+                             SECRETS,
+                             bw)
 
     # 🦑 Install Argo CD: continuous deployment app for k8s
     if argo_enabled:
         # setup k8s secrets management and secret stores
-        setup_k8s_secrets_management(k8s_obj,
+        setup_k8s_secrets_management(argocd,
                                      distro,
                                      apps.pop('external_secrets_operator', {}),
                                      SECRETS['global_external_secrets'],
                                      apps.pop('infisical', {}),
                                      apps.pop('vault', {}),
                                      bw)
 
@@ -239,81 +252,85 @@
         if 'staging' in SECRETS['global_cluster_issuer']:
             api_tls_verify = False
         else:
             api_tls_verify = True
 
         # Setup minio, our local s3 provider, is essential for creating buckets
         # and cnpg operator, our postgresql operator for creating postgres clusters
-        setup_operators(k8s_obj,
+        setup_operators(argocd,
                         apps.pop('prometheus_crds', {}),
                         apps.pop('longhorn', {}),
                         apps.pop('k8up', {}),
                         apps.pop('minio_operator', {}),
                         apps.pop('seaweedfs', {}),
                         apps.pop('cnpg_operator', {}),
                         apps.pop('postgres_operator', {}),
                         bw)
 
+        # global pvc storage class
+        pvc_storage_class = SECRETS.get('global_pvc_storage_class', 'local-path')
+
+        # check if zitadel is enabled
+        zitadel_enabled = apps['zitadel']['enabled']
+
         # setup OIDC for securing all endpoints with SSO
-        oidc_obj = setup_oidc_provider(
-                k8s_obj,
-                api_tls_verify,
-                apps.pop('zitadel', {}),
-                apps.pop('vouch', {}),
-                bw,
-                SECRETS['argo_cd_hostname']
-                )
+        oidc_obj = setup_oidc_provider(argocd,
+                                       api_tls_verify,
+                                       apps.pop('zitadel', {}),
+                                       apps.pop('vouch', {}),
+                                       pvc_storage_class,
+                                       bw,
+                                       SECRETS['argo_cd_hostname'])
 
         # we need this for all the oidc apps we need to create
         zitadel_hostname = SECRETS.get('zitadel_hostname', "")
 
         # setup netmaker, a wireguard vpn management web interface
         netmaker_dict = apps.pop('netmaker', {'enabled': False})
         # only do this if the user has smol-k8s-lab init enabled
         if netmaker_dict['enabled']:
-            configure_netmaker(k8s_obj,
+            configure_netmaker(argocd,
                                netmaker_dict,
                                'zitadel',
                                zitadel_hostname,
                                bw,
                                oidc_obj)
 
         setup_federated_apps(
-                k8s_obj,
+                argocd,
                 api_tls_verify,
                 apps.pop('home_assistant', {}),
                 apps.pop('nextcloud', {}),
                 apps.pop('mastodon', {}),
                 apps.pop('matrix', {}),
+                pvc_storage_class,
                 zitadel_hostname,
                 oidc_obj,
                 bw
                 )
 
         # we support creating a default minio tenant with oidc enabled
         # we set it up here in case other apps rely on it
         minio_tenant_config = apps.pop('minio_tenant', {})
         if minio_tenant_config and minio_tenant_config.get('enabled', False):
-            configure_minio_tenant(k8s_obj,
+            configure_minio_tenant(argocd,
                                    minio_tenant_config,
                                    api_tls_verify,
                                    zitadel_hostname,
                                    oidc_obj,
                                    bw)
 
         # after argocd, zitadel, bweso, and vouch are up, we install all apps
         # as Argo CD Applications
         header("Installing the rest of the Argo CD apps")
         for app_key, app_meta in apps.items():
             if app_meta['enabled']:
-                app_installed = check_if_argocd_app_exists(app_key)
-                if not app_installed:
-                    argo_app = app_key.replace('_', '-')
-                    sub_header(f"Installing app: {argo_app}")
-                    install_with_argocd(k8s_obj, argo_app, app_meta['argo'])
+                argo_app = app_key.replace('_', '-')
+                sub_header(f"Installing app: {argo_app}")
+                argocd.install_app(argo_app, app_meta['argo'])
 
         # lock the bitwarden vault on the way out, to be polite :3
         if bw:
             bw.lock()
 
     # we're done :D
     print("")
@@ -348,17 +365,17 @@
                           f"[blue][link]https://{nextcloud_hostname}[/][/]\n")
 
         mastodon_hostname = SECRETS.get('mastodon_hostname', "")
         if mastodon_hostname:
             final_msg += ("\n🐘 Mastodon, for your social media:\n"
                           f"[blue][link]https://{mastodon_hostname}[/][/]\n")
 
-        matrix_hostname = SECRETS.get('matrix_hostname', "")
+        matrix_hostname = SECRETS.get('matrix_element_hostname', "")
         if matrix_hostname:
-            final_msg += ("\n💬 Matrix, for your chat:\n"
+            final_msg += ("\n💬 Matrix (with Element frontend), for your chat:\n"
                           f"[blue][link]https://{matrix_hostname}[/][/]\n")
 
         home_assistant_hostname = SECRETS.get('home_assistant_hostname', "")
         if home_assistant_hostname:
             final_msg += ("\n🏠 Home Assistant, for managing your IoT needs:\n"
                           f"[blue][link]https://{home_assistant_hostname}[/][/]\n")
 
@@ -369,10 +386,14 @@
 
     CONSOLE.print(Panel(final_msg,
                         title='[green]◝(ᵔᵕᵔ)◜ Success!',
                         subtitle='♥ [cyan]Have a nice day[/] ♥',
                         border_style="cornflower_blue"))
     print("")
 
+    # run final command after it all ends
+    if final_cmd and window_behavior == "same-window":
+        run_final_cmd(final_cmd, terminal, window_behavior)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import base64
 import json
 import logging as log
 from rich.prompt import Prompt
 from shutil import which
 from sys import exit
 from os import environ as env
-from ..utils.subproc import subproc
+from ..utils.run.subproc import subproc
 from .tui.bitwarden_existing_item_app import AskUserForDuplicateStrategy
 
 
 def create_custom_field(custom_field_name: str, value: str) -> dict:
    """
    creates a custom field dict for a bitwarden login item
    """
@@ -54,20 +54,20 @@
                       "Try [green]brew install bw")
             exit()
 
         # if we clean up the session when we're done or not
         self.delete_session = True
 
         # this is used for bweso and logins
-        self.host = env.get("BW_HOST", default="https://bitwarden.com")
+        self.host = env.get("BW_HOST", "https://bitwarden.com")
         log.debug(f"Using {self.host} as $BW_HOST")
 
 
         # make sure there's not a session token in the env vars already
-        self.env = {"BW_SESSION": env.get("BW_SESSION", default=None),
+        self.env = {"BW_SESSION": env.get("BW_SESSION", ""),
                     "PATH": env.get("PATH"),
                     "HOME": env.get("HOME"),
                     "NODE_OPTIONS": "--no-deprecation"}
 
         self.password = password
         self.client_id = client_id
         self.client_secret = client_secret
@@ -88,47 +88,50 @@
         return Prompt.ask(cred_prompt, password=True)
 
     def status(self) -> str:
         """
         generate a new password. Takes special_characters bool.
         """
         log.info('Checking if you are logged in...')
-        return json.loads(subproc(["bw status"]))['status']
+        return json.loads(subproc(["bw status"], env=self.env))['status']
 
     def unlock(self) -> None:
         """
         unlocks the local bitwarden vault, and returns session token
         """
         if self.env['BW_SESSION']:
             log.info('Using session token from $BW_SESSION env variable')
             self.delete_session = False
 
         status = self.status()
-
-        if status == "unauthenticated" or status == "locked":
-            # verify we're even logged in :)
-            if status == "unauthenticated":
-                log.info('Logging into the Bitwarden vault...')
-                # set command to login if we're unauthenticated
-                cmd = (f"{self.bw_path} login --passwordenv BW_PASSWORD "
-                       "--apikey --raw")
-            else:
-                log.info('Unlocking the Bitwarden vault...')
-                # set command to unlock if status is locked
-                cmd = f"{self.bw_path} unlock --passwordenv BW_PASSWORD --raw"
+        if status == "locked" or status == "unauthenticated":
+            env = {"BW_PASSWORD": self.password,
+                   "BW_CLIENTID": self.client_id,
+                   "BW_CLIENTSECRET": self.client_secret,
+                   "BW_HOST": self.host,
+                   "PATH": self.env['PATH'],
+                   "HOME": self.env['HOME'],
+                   "NODE_OPTIONS": "--no-deprecation"}
+
+        # login if we need to
+        if status == "unauthenticated":
+            log.info('Logging into the Bitwarden vault...')
+            # set command to login if we're unauthenticated
+            cmd = f"{self.bw_path} login --passwordenv BW_PASSWORD --apikey --raw"
+            subproc([cmd], quiet=True, env=env)
+
+        # we still need to unlock, even if we logged in already
+        if status == "locked" or status == "unauthenticated":
+            log.info('Unlocking the Bitwarden vault...')
+            # set command to unlock if status is locked
+            cmd = f"{self.bw_path} unlock --passwordenv BW_PASSWORD --raw"
 
             # run either bw login or bw unlock depending on bw status
-            self.env['BW_SESSION'] = subproc([cmd], quiet=True,
-                                             env={"BW_PASSWORD": self.password,
-                                                  "BW_CLIENTID": self.client_id,
-                                                  "BW_CLIENTSECRET": self.client_secret,
-                                                  "BW_HOST": self.host,
-                                                  "PATH": self.env['PATH'],
-                                                  "HOME": self.env['HOME']})
-            # log.debug(f"session is {self.session}")
+            self.env['BW_SESSION'] = subproc([cmd], quiet=True, env=env)
+            log.debug(f"bw unlock session is {self.env['BW_SESSION']}")
             log.info('Unlocked the Bitwarden vault.')
         else:
             log.info(f"[green]bw status[/] returned '{status}', so we won't "
                      "unlock the Bitwarden vault before starting.")
 
     def lock(self) -> None:
         """
@@ -201,15 +204,15 @@
             action = user_response[0]
             always_do_action = user_response[1]
             item = user_response[2]
 
             # if they always want to do this, then set self.duplicate_strategy
             if always_do_action:
                 # NOTE: we still always ask if there's more than 1 entry returned
-                self.duplicate_strategy = action 
+                self.duplicate_strategy = action
 
             return item, action
         else:
             return response['data'], self.duplicate_strategy
 
     def create_login(self,
                      name: str = "",
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 $blue_gray: rgb(86,95,137);
 $dark_gray: rgb(58,58,58);
 $navy: rgb(35,35,54);
 
 /* base container for the whole screen */
 #bitwarden-modal-container {
     width: 90%;
-    height: 50%;
+    height: 60%;
     align: center middle;
     background: $navy 50%;
 }
 
 /* box with border and inputs and button */
 #credentials-box {
     align: center middle;
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-5.0.0/smol_k8s_lab/config/default_config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -12,34 +12,44 @@
     accessibility:
       bell:
         # ring the built in terminal bell on focus to new elements on the screen
         on_focus: true
         # ring the built in terminal bell when something is wrong
         on_error: true
       text_to_speech:
-        # use a specific program for text to speech - needs to be a full path
-        # macOS default: say
-        speech_program: say
-        # read aloud the screen title and description
+        # currently only english (en) and nederlands (nl) are available, but if you know
+        # other languages, please help us translate (open an issue or discussion
+        # on github 💙)
+        language: "en"
+        # use a specific cli program for text to speech - needs to be a full path
+        # if it isn't in your default path. default is "" which means we'll use
+        # pre-recorded audio files
+        speech_program: ""
+        # read aloud the screen title
         screen_titles: true
+        # read aloud the screen description
+        screen_descriptions: true
         # read aloud the element id, value, and tooltip each time you switch focus
         on_focus: false
         # press f5 to read the element id and selected row of DataTables
         on_key_press: true
 
-    # enable text to speech
-    # k9s is a terminal UI dashboard and interface for interacting with Kubernetes
-    k9s:
-      # when set to true, if smol-k8s-lab is in interactive mode, it runs k9s
-      # immediately after the cluster is up and enabled apps have been installed
-      enabled: false
-      # default command to run when k9s launches. Defaults to application.argoproj.io
-      # so that you can view the status of all of your argo apps immediately. This
-      # default results in running: k9s --command applications.argoproj.io
-      command: applications.argoproj.io
+  run_command:
+    # command to run after smol-k8s-lab is completed
+    command: "k9s --command applications.argoproj.io"
+    # tell me which terminal you use if you'd like to use split or tab features
+    # options: wezterm, zellij (if you want other terminals, please submit a
+    # feature request and/or PR with the commands for your favorite terminal, or
+    # as a work around, let this to "none" and set full command above
+    terminal: "wezterm"
+    # where to run the command, options: same window, new window, new tab,
+    # split left, split right, split top, split bottom
+    # if set to "same window", we just run it in the same window after we're
+    # done the entire smol-k8s-lab cli run
+    window_behavior: "same window"
 
   # logging config for the smol-k8s-lab CLI
   log:
     # path of file to log to if console logging is NOT desired
     file: ""
     # logging level, Options: debug, info, warn, error
     level: info
@@ -71,25 +81,28 @@
     # automatically pass in flannel-backend: none and disable-network-policy: true
     k3s_yaml:
       # if you enable MetalLB, we automatically add servicelb to the disable list
       # enables encryption at rest for Kubernetes secrets
       secrets-encryption: true
       # disables traefik so we can enable ingress-nginx, remove if you're using traefik
       disable:
-      - "traefik"
+      - traefik
+      - servicelb
       node-label:
       - "ingress-ready=true"
       kubelet-arg:
       - "max-pods=150"
     # list of nodes to SSH to and join to cluster. example:
     # nodes:
     #   # name can be a hostname or ip address
     #   serverfriend1.lan:
     #     # change ssh_key to the name of a local private key to use
     #     ssh_key: id_rsa
+    #     # change ssh port for the remote node
+    #     ssh_port: 22
     #     # must be node type of "worker" or "control_plane"
     #     node_type: worker
     #     # labels are optional, but may be useful for pod node affinity
     #     node_labels:
     #       - iot=true
     #     # taints are optional, but may be useful for pod tolerations
     #     node_taints:
@@ -140,16 +153,23 @@
 # anything here gets set for all apps if you're using our default repos
 apps_global_config:
   # setting this changes all the below domains to use the following cluster_issuer
   # change to letsencrypt-prod when you're ready to go live with your infra
   cluster_issuer: "letsencrypt-staging"
   # change to your tz: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List
   time_zone: "Europe/Amsterdam"
-  # always deploy external secrets. *Must be a string of "" (don't use external secrets) or "bitwarden" to use bitwarden for external secrets*
+  # always deploy extnernal secrets. *Must be a string of either:
+  # ""           - don't use external secrets
+  # "bitwarden"  - use bitwarden for external secrets
+  # "openbao"    - (coming soon!) use openbao (a fork of vault) for external secrets
   external_secrets: "bitwarden"
+  # the default storage class you want to use for the creation of all Persistent Volume claims
+  # it defaults to local-path, but you can set it to longhorn or whatever you'd like :)
+  # for storage classes see:
+  pvc_storage_class: "local-path"
 
 # ---------------------------------------------------------------------------
 # Argo CD deployed and maintained Applications to run on Kubernetes
 # ---------------------------------------------------------------------------
 apps:
   argo_cd:
     # Set to false if you you just want a bare cluster with only the above apps"
@@ -174,14 +194,16 @@
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       # change to argocd/argocd to not use app of apps with secret plugin
       path: "argocd/app_of_apps/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "argocd"
       # recurse directories in the provided git repo, if true, we also deploy the appset secret plugin
       directory_recursion: true
       # source repos for Argo CD argo-cd Project (in addition to argo_cd.argo.repo)
       project:
         name: argo-cd
@@ -231,14 +253,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "cert-manager/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "cert-manager"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for cert-manager CD App Project (in addition to argo.repo)
       project:
         name: cert-manager
@@ -263,14 +287,16 @@
         hostname: ""
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "demo/cilium/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "cilium"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD cilium Project
       project:
         name: cilium
@@ -291,14 +317,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: postgres/operators/cloud-native-postgres/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: cnpg-system
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: cnpg-operator
@@ -331,14 +359,16 @@
       # change to external-secrets-operator/external-secrets-operator/ to deploy
       # ONLY the external-secrets-operator, so this will not use app of apps and
       # therefore we will not deploy the Bitwarden ESO provider. Use if you want to use
       # a different provider
       path: external-secrets-operator/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: external-secrets
       # recurse directories in the provided git repo
       directory_recursion: false
       # secret keys to provide for the Argo CD Appset secret plugin, none by default
       secret_keys: {}
       # source repos for Argo CD App Project (in addition to app.argo.repo)
@@ -368,14 +398,16 @@
         # change this to the image repo you want to deploy
         image_repo: "nginx"
         # change this the image tag you want to deploy
         image_tag: "latest"
       repo: https://github.com/small-hack/argocd-apps
       path: generic-app/
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # you can change this your app's name
       namespace: generic-app
       directory_recursion: false
       project:
         # you can change this your app's name
         name: generic-app
         source_repos:
@@ -390,14 +422,16 @@
     description: |
       This installs the [link=https://github.com/squat/generic-device-plugin/tree/main]squat/generic-device-plugin[/link], which is recommended for exposing generic devices such as USB devices to your k8s pods. This can useful if you have an IoT coordinator device such as the conbee 2 that you are using with deconz or home assistant. You can read more about device plugins in the [link=https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/device-plugins/]Kubernetes docs[/link].
     argo:
       secret_keys: {}
       repo: https://github.com/small-hack/argocd-apps
       path: generic-device-plugin/
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       namespace: kube-system
       directory_recursion: false
       project:
         name: generic-device-plugin
         source_repos:
           - https://github.com/squat/generic-device-plugin
         destination:
@@ -416,17 +450,17 @@
       This app takes one sensitive value, password for the initial owner user. You can also pass it in as an enviornment variable called $HOME_ASSISTANT_PASSWORD.
     # Initialization of the app through smol-k8s-lab
     init:
       # enable the creation of an initial owner user
       enabled: true
       values:
         # -- owner user's name
-        name: "admin"
+        admin_name: "admin"
         # -- owner user's username
-        user_name: "admin"
+        admin_user: "admin"
         # -- owner user's language, default is english
         language: "en"
       sensitive_values:
         - PASSWORD
     argo:
       secret_keys:
         hostname: ""
@@ -461,14 +495,16 @@
         # these are for passing in a bluetooth device
         bluetooth_device_path: /run/dbus
         bluetooth_device_mount_path: /run/dbus
         bluetooth_device_index: '2'
       repo: https://github.com/small-hack/argocd-apps
       path: home-assistant/toleration_and_affinity/
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       namespace: home-assistant
       directory_recursion: false
       project:
         name: home-assistant
         source_repos:
           - https://small-hack.github.io/home-assistant-chart
         destination:
@@ -491,14 +527,16 @@
         hostname: ""
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "demo/infisical/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "infisical"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to app.argo.repo)
       project:
         name: infisical
@@ -520,14 +558,16 @@
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       # change to "ingress/ingress-nginx/" to not use app of apps
       path: "ingress-nginx/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "ingress-nginx"
       # recurse directories in the provided git repo
       directory_recursion: false
       # secret keys to provide for the Argo CD Appset secret plugin, none by default
       secret_keys: {}
       # source repos for Argo CD App Project (in addition to argo.repo)
@@ -553,14 +593,16 @@
       secret_keys: []
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "k8tz/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "k8tz"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to app.argo.repo)
       project:
         name: k8tz
@@ -582,14 +624,16 @@
       secret_keys: []
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "k8up/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "k8up"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to app.argo.repo)
       project:
         name: k8up
@@ -612,14 +656,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "demo/kepler/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "kepler"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: kepler
@@ -641,14 +687,16 @@
         webui_hostname: subdomain.domain.tld
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: kubevirt/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: kubevirt
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: kubevirt
@@ -675,14 +723,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "kyverno/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "kyvero"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: kyverno
@@ -700,14 +750,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: demo/longhorn/helm/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: longhorn-system
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: longhorn
@@ -731,54 +783,77 @@
          - MASTODON_SMTP_PASSWORD
          - MASTODON_S3_BACKUP_ACCESS_ID
          - MASTODON_S3_BACKUP_SECRET_KEY
          - MASTODON_RESTIC_REPO_PASSWORD
     enabled: false
     init:
       enabled: true
+      restore:
+        enabled: true
+        cnpg_restore: true
+        restic_snapshot_ids:
+          seaweedfs_volume: latest
+          seaweedfs_filer: latest
+          seaweedfs_master: latest
       values:
         # admin user
         admin_user: "tootadmin"
         # admin user's email
         admin_email: ""
         # mail server to send verification and notification emails
         smtp_host: "change@me-to-enable.mail"
         # mail user for smtp host
         smtp_user: "change me to enable mail"
-      sensitive_values:
-        # these can be passed in as env vars if you pre-pend MASTODON_ to each one
-        - SMTP_PASSWORD
-        - S3_BACKUP_ACCESS_ID
-        - S3_BACKUP_SECRET_KEY
-        - RESTIC_REPO_PASSWORD
+        smtp_password:
+          value_from:
+            env: MASTODON_SMTP_PASSWORD
+    backups:
+      # cronjob syntax schedule to run mastodon pvc backups
+      pvc_schedule: 10 0 * * *
+      # cronjob syntax (with SECONDS field) for mastodon postgres backups
+      # must happen at least 10 minutes before pvc backups, to avoid corruption
+      # due to missing files. This is because the backup shows as completed before
+      # it actually is
+      postgres_schedule: 0 0 0 * * *
+      s3:
+        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
+        endpoint: ""
+        bucket: ""
+        region: ""
+        secret_access_key:
+          value_from:
+            env: MASTODON_S3_BACKUP_SECRET_KEY
+        access_key_id:
+          value_from:
+            env: MASTODON_S3_BACKUP_ACCESS_ID
+        restic_repo_password:
+          value_from:
+            env: MASTODON_RESTIC_REPO_PASSWORD
     argo:
       # secrets keys to make available to Argo CD ApplicationSets
       secret_keys:
         admin_user: tootadmin
         # hostname that users go to in the browser
         hostname: ""
         # set the local s3 provider for mastodon's public data in one bucket
         # and private database backups in another. can be minio or seaweedfs
         s3_provider: seaweedfs
         # how large the backing pvc's capacity should be for minio or seaweedfs
         s3_pvc_capacity: 120Gi
         # local s3 endpoint for postgresql backups, backed up constantly
         s3_endpoint: ""
         s3_region: eu-west-1
-        # Remote S3 configuration, for pushing remote backups of your local postgresql backups
-        # these are done only nightly right now, for speed and cost optimization
-        s3_backup_endpoint: ""
-        s3_backup_region: ""
-        s3_backup_bucket: ""
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: mastodon/small-hack/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: mastodon
       # recurse directories in the git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: mastodon
@@ -808,54 +883,107 @@
         - MATRIX_SMTP_PASSWORD
         - MATRIX_S3_BACKUP_ACCESS_ID
         - MATRIX_S3_BACKUP_SECRET_KEY
         - MATRIX_RESTIC_REPO_PASSWORD
     enabled: false
     init:
       enabled: true
+      restore:
+        # set to true to run a restic restore via a k8up job for your
+        # seaweedfs PVCs, matrix signing key PVC, synapse config PVC, media PVC
+        # and restoring your postgresql database
+        enabled: true
+        # for Cloudnative postgres operator cluster restores only
+        cnpg_restore: true
+        # the restic snapshot IDs of the PVC snapshots you want to restore
+        restic_snapshot_ids:
+          # seaweedFS volume pvc snapshot id. if not given, we use the latest
+          seaweedfs_volume: ""
+          # seaweedFS filer pvc snapshot id. if not given, we use the latest
+          seaweedfs_filer: ""
+          # seaweedFS master pvc snapshot id. if not given, we use the latest
+          seaweedfs_master: ""
+          # signing key snapshot id. if not given, we use the latest
+          signing_key: ""
+          # media snapshot id. if not given, we use the latest
+          media: ""
+          # synapse config snapshot id. if not given, we use the latest
+          synapse_config: ""
       values:
         smtp_user: "change me to enable mail"
         smtp_host: "change@me-to-enable.mail"
-      sensitive_values:
-        - SMTP_PASSWORD
-        - S3_BACKUP_ACCESS_ID
-        - S3_BACKUP_SECRET_KEY
-        - RESTIC_REPO_PASSWORD
+    backups:
+      # cronjob syntax schedule to run matrix pvc backups
+      pvc_schedule: 10 0 * * *
+      # cronjob syntax (with SECONDS field) for matrix postgres backups
+      # must happen at least 10 minutes before pvc backups, to avoid corruption
+      # due to missing files. This is because the backup shows as completed before
+      # it actually is
+      postgres_schedule: 0 0 0 * * *
+      s3:
+        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
+        endpoint: ""
+        bucket: ""
+        region: ""
+        secret_access_key:
+          value_from:
+            env: MATRIX_S3_BACKUP_SECRET_KEY
+        access_key_id:
+          value_from:
+            env: MATRIX_S3_BACKUP_ACCESS_ID
+      restic_repo_password:
+        value_from:
+          env: MATRIX_RESTIC_REPO_PASSWORD
     argo:
       # secrets keys to make available to Argo CD ApplicationSets
       secret_keys:
         # hostname of the synapse matrix server
         hostname: ""
         # the hostname of the element web interface
         element_hostname: ""
         # hostname for federation, that others can see you on the fediverse
         federation_hostname: ""
         # email for of the admin user
         admin_email: ""
+        # enable persistent volume claim for matrix media storage
+        media_pvc_enabled: "true"
+        # size of media pvc storage
+        media_storage: "20Gi"
+        media_access_mode: "ReadWriteOnce"
+        # enable persistent volume claim for matrix synapse config storage
+        synapse_config_pvc_enabled: "true"
+        # size of synapse config pvc storage
+        synapse_config_storage: "2Mi"
+        synapse_config_access_mode: "ReadWriteOnce"
+        # enable persistent volume claim for matrix signing key storage
+        signing_key_pvc_enabled: "true"
+        # size of signing key pvc storage
+        signing_key_storage: "1Mi"
+        signing_key_access_mode: "ReadWriteOnce"
+        # cronjob syntax schedule to run matrix backups, defaults to 1:10AM
+        backup_schedule: "10 1 * * *"
         # choose S3 as the local primary object store from either: seaweedfs, or minio
         # SeaweedFS - deploy SeaweedFS filer/s3 gateway
         # MinIO     - deploy MinIO vanilla helm chart
         s3_provider: seaweedfs
         # local s3 provider bucket name
         s3_bucket: matrix
         # the endpoint you'd like to use for your minio or SeaweedFS instance
         s3_endpoint: ""
         # how large the backing pvc's capacity should be for minio or seaweedfs
         s3_pvc_capacity: 100Gi
         s3_region: eu-west-1
-        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
-        s3_backup_endpoint: ""
-        s3_backup_bucket: ""
-        s3_backup_region: ""
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: matrix/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: matrix
       # recurse directories in the git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: matrix
@@ -889,14 +1017,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "metallb/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "metallb-system"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD metallb Project (in addition to metallb.argo.repo)
       project:
         name: metallb
@@ -920,14 +1050,16 @@
         admin_console_hostname: ""
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "minio/operator/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "minio"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: minio
@@ -960,14 +1092,16 @@
         s3_backup_bucket: "set me to your bucket name"
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "minio/tenant/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "minio"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: minio
@@ -996,14 +1130,16 @@
         auth_provider: oidc
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: netmaker/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: netmaker
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         source_repos:
@@ -1026,47 +1162,98 @@
         - NEXTCLOUD_S3_BACKUP_ACCESS_ID
         - NEXTCLOUD_RESTIC_REPO_PASSWORD
 
       Note: smol-k8s-lab is not affiliated with Nextcloud GmbH. This is a community-supported-only install method.
     # initialize the app by setting up new k8s secrets and/or bitwarden items
     init:
       enabled: true
+      restore:
+        # set to true to run a restic restore via a k8up job for:
+        # seaweedfs pvcs and nextcloud files pvc
+        enabled: false
+        # for Cloudnative Postgres operator "cluster" CRD type resources
+        cnpg_restore: true
+        # restic snapshot ID for each PVC
+        restic_snapshot_ids:
+          # seaweedFS volume pvc snapshot id
+          seaweedfs_volume: "latest"
+          # seaweedFS filer pvc snapshot id
+          seaweedfs_filer: "latest"
+          # seaweedFS master pvc snapshot id
+          seaweedfs_master: "latest"
+          # nextcloud-files pvc snapshot id
+          nextcloud_files: "latest"
+          # nextcloud-config pvc snapshot id - if you enabled config pvc, you can uncomment this
+          # nextcloud_config: "latest"
       values:
         # change the name of your admin user to whatever you like. This is used in an admin credentials k8s secret
         admin_user: "nextcloud_admin"
         smtp_user: "change me to enable mail"
         smtp_host: "change-me-to-real-email@to-enable.mail"
-      sensitive_values:
-        - SMTP_PASSWORD
-        - S3_BACKUP_ACCESS_KEY
-        - S3_BACKUP_ACCESS_ID
-        - RESTIC_REPO_PASSWORD
+        smtp_password:
+          value_from:
+            env: NEXTCLOUD_SMTP_PASSWORD
+    backups:
+      # cronjob syntax schedule to run nextcloud pvc backups
+      pvc_schedule: 10 0 * * *
+      # cronjob syntax (with SECONDS field) for nextcloud postgres backups
+      # must happen at least 10 minutes before pvc backups, to avoid corruption
+      # due to missing files. This is because the cnpg backup shows as completed
+      # before it actually is, due to the wal archive it lists as it's end not
+      # being in the backup yet
+      postgres_schedule: 0 0 0 * * *
+      s3:
+        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
+        endpoint: ""
+        bucket: ""
+        region: ""
+        secret_access_key:
+          value_from:
+            env: NEXTCLOUD_S3_BACKUP_SECRET_KEY
+        access_key_id:
+          value_from:
+            env: NEXTCLOUD_S3_BACKUP_ACCESS_ID
+      restic_repo_password:
+        value_from:
+          env: NEXTCLOUD_RESTIC_REPO_PASSWORD
     argo:
       # secrets keys to make available to Argo CD ApplicationSets
       secret_keys:
         hostname: ""
+        # create a pvc for nextcloud files
+        files_pvc_enabled: "true"
+        # size of the pvc for nextcloud files
+        files_storage: "20Gi"
+        files_access_mode: "ReadWriteOnce"
+        # create a pvc for nextcloud config
+        config_pvc_enabled: "true"
+        # size of the pvc for nextcloud config
+        config_storage: "2Gi"
+        config_access_mode: "ReadWriteOnce"
         # choose S3 as the local primary object store from either: seaweedfs, or minio
         # SeaweedFS - deploy SeaweedFS filer/s3 gateway
         # MinIO     - deploy MinIO vanilla helm chart
         s3_provider: seaweedfs
         # the endpoint you'd like to use for your minio or SeaweedFS instance
         s3_endpoint: ""
         # how large the backing pvc's capacity should be for minio or seaweedfs
         s3_pvc_capacity: 100Gi
         s3_region: eu-west-1
-        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
-        s3_backup_endpoint: ""
-        s3_backup_bucket: ""
-        s3_backup_region: ""
+        # cronjob schedule to turn on nextcloud maintenance mode for backups
+        maintenance_mode_on_schedule: "0 1 * * *"
+        # cronjob schedule to turn off nextcloud maintenance mode after backups
+        maintenance_mode_off_schedule: "30 1 * * *"
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: nextcloud/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: nextcloud
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: nextcloud
@@ -1111,14 +1298,16 @@
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important! This
       # is an app of apps. Change to "monitoring/kube-prometheus-stack/" to
       # only install kube-prometheus-stack (foregoing loki and push gateway)
       path: postgres/operators/zalando/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: postgres-operator
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: postgres-operator
@@ -1142,14 +1331,16 @@
       secret_keys: {}
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: prometheus/crds/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: prometheus
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: prometheus
@@ -1183,14 +1374,16 @@
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important! This
       # is an app of apps. Change to "monitoring/kube-prometheus-stack/" to
       # only install kube-prometheus-stack (foregoing loki and push gateway)
       path: prometheus/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "prometheus"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: prometheus
@@ -1199,14 +1392,48 @@
           - "https://github.com/prometheus-community/helm-charts.git"
           - "https://prometheus-community.github.io/helm-charts"
         destination:
           # automatically includes the app's namespace and argocd's namespace
           namespaces:
             - kube-system
 
+  renovate:
+    description: |
+      [magenta]DEMO - UNTESTED[/magenta]
+
+      [link=https://docs.renovatebot.com/]Renovate[/link] is a tool for automated dependency updates. It's Multi-platform and multi-language. This is a simple helm chart for running a self-hosted RenovateBot.
+
+    enabled: false
+    argo:
+      # secrets keys to make available to Argo CD ApplicationSets
+      secret_keys: {}
+      # git repo to install the Argo CD app from
+      repo: https://github.com/small-hack/argocd-apps
+      # path in the argo repo to point to. Trailing slash very important! This
+      # is an app of apps. Change to "monitoring/kube-prometheus-stack/" to
+      # only install kube-prometheus-stack (foregoing loki and push gateway)
+      path: demo/renovate/
+      # either the branch or tag to point at in the argo repo above
+      revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
+      # namespace to install the k8s app in
+      namespace: "renovate"
+      # recurse directories in the provided git repo
+      directory_recursion: false
+      # source repos for Argo CD App Project (in addition to argo.repo)
+      project:
+        name: renovate
+        source_repos:
+          - "https://docs.renovatebot.com/helm-charts"
+        destination:
+          # automatically includes the app's namespace and argocd's namespace
+          namespaces:
+            - renovate
+
   seaweedfs:
     enabled: false
     description: |
       [link=https://github.com/seaweedfs/seaweedfs]seaweedfs[/link] is a filesystem with an exposable S3 endpoint.
 
       This is mostly meant to be for testing, but have at it :D
 
@@ -1223,14 +1450,16 @@
         s3_region: eu-west-1
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: seaweedfs/app_of_apps/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: seaweedfs
       # recurse directories in the provided git repo
       # if set to false, we will not deploy the CSI driver
       directory_recursion: true
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
@@ -1255,14 +1484,16 @@
       secret_keys: []
       # git repo to install the Argo CD app from
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: demo/seaweedfs/app_of_apps/csi_driver/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: seaweedfs
       # recurse directories in the provided git repo
       # if set to false, we will not deploy the CSI driver
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
@@ -1288,14 +1519,16 @@
         # name of the cluster that vault is associated with, can be any unique name
         cluster_name: my-cool-cluster
       repo: https://github.com/small-hack/argocd-apps
       # path in the argo repo to point to. Trailing slash very important!
       path: demo/vault/
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: vault
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: vault
@@ -1329,14 +1562,16 @@
       # repo to install the Argo CD app from
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       path: "vouch-proxy/app_of_apps/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "vouch"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: vouch
@@ -1366,59 +1601,86 @@
         - ZITADEL_S3_BACKUP_ACCESS_ID
         - ZITADEL_S3_BACKUP_SECRET_KEY
         - ZITADEL_RESTIC_REPO_PASSWORD
     init:
       # Switch to false if you don't want to create intial secrets or use the
       # API via a service acocunt to create the above described resources
       enabled: true
+      restore:
+        # set to true to run a restic restore via a k8up job for seaweedfs PVCs,
+        # and restoring your postgresql database
+        enabled: true
+        # for Cloudnative postgres operator cluster restores only
+        cnpg_restore: true
+        # the restic snapshot IDs of the PVC snapshots you want to restore
+        restic_snapshot_ids:
+          # seaweedFS volume pvc snapshot id. if not given, we use the latest
+          seaweedfs_volume: ""
+          # seaweedFS filer pvc snapshot id. if not given, we use the latest
+          seaweedfs_filer: ""
+          # seaweedFS master pvc snapshot id. if not given, we use the latest
+          seaweedfs_master: ""
       values:
         # initial human user's usename
-        username: ""
+        admin_user: ""
         # initial human user's email
         email: ""
         # initial human's first name
         first_name: ""
         # initial human's last name
         last_name: ""
         # options: GENDER_UNSPECIFIED, GENDER_MALE, GENDER_FEMALE, GENDER_DIVERSE
         # more coming soon, see: https://github.com/zitadel/zitadel/issues/6355
         gender: GENDER_UNSPECIFIED
         # name of the default project to create OIDC applications in
         project: core
-      sensitive_values:
-      # sensitive values to provide via environment variables or via the TUI
-      - S3_BACKUP_ACCESS_ID
-      - S3_BACKUP_SECRET_KEY
-      - RESTIC_REPO_PASSWORD
-      # coming soon after we refactor a bit
-      # - SMTP_PASSWORD
+    backups:
+      # cronjob syntax schedule to run zitadel seaweedfs pvc backups
+      pvc_schedule: 10 0 * * *
+      # cronjob syntax (with SECONDS field) for zitadel postgres backups
+      # must happen at least 10 minutes before pvc backups, to avoid corruption
+      # due to missing files. This is because the cnpg backup shows as completed
+      # before it actually is, due to the wal archive it lists as it's end not
+      # being in the backup yet
+      postgres_schedule: 0 0 0 * * *
+      s3:
+        # these are for pushing remote backups of your local s3 storage, for speed and cost optimization
+        endpoint: ""
+        bucket: ""
+        region: ""
+        secret_access_key:
+          value_from:
+            env: ZITADEL_S3_BACKUP_SECRET_KEY
+        access_key_id:
+          value_from:
+            env: ZITADEL_S3_BACKUP_ACCESS_ID
+      restic_repo_password:
+        value_from:
+          env: ZITADEL_RESTIC_REPO_PASSWORD
     argo:
       # secrets keys to make available to Argo CD ApplicationSets
       secret_keys:
         # FQDN to use for zitadel
         hostname: ""
         # set the local s3 provider for zitadel's database backups. can be minio or seaweedfs
         s3_provider: seaweedfs
         # local s3 endpoint for postgresql backups, backed up constantly
         s3_endpoint: ""
         # capacity for the PVC backing your local s3 instance
         s3_pvc_capacity: 2Gi
-        # Remote S3 configuration, for pushing remote backups of your local postgresql backups
-        # these are done only nightly right now, for speed and cost optimization
-        s3_backup_endpoint: ""
-        s3_backup_region: ""
-        s3_backup_bucket: ""
       # repo to install the Argo CD app from
       # git repo to install the Argo CD app from
       repo: "https://github.com/small-hack/argocd-apps"
       # path in the argo repo to point to. Trailing slash very important!
       # if you want to use cockroachdb, change to zitadel/zitadel_and_cockroachdb
       path: "zitadel/app_of_apps/"
       # either the branch or tag to point at in the argo repo above
       revision: main
+      # kubernetes cluster to install the k8s app into, defaults to Argo CD default
+      cluster: https://kubernetes.default.svc
       # namespace to install the k8s app in
       namespace: "zitadel"
       # recurse directories in the provided git repo
       directory_recursion: false
       # source repos for Argo CD App Project (in addition to argo.repo)
       project:
         name: zitadel
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-5.0.0/smol_k8s_lab/config/keycloak_config.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962962962962963%*

 * *Differences: {"'clients'": "{1: {'rootUrl': 'https://vouch.example.org', 'adminUrl': "*

 * *              "'https://vouch.example.org/', 'redirectUris': {insert: [(1, "*

 * *              "'https://vouch.example.org/auth')], delete: [1]}}}"}*

```diff
@@ -101,15 +101,15 @@
         },
         {
             "access": {
                 "configure": true,
                 "manage": true,
                 "view": true
             },
-            "adminUrl": "https://vouch.vleermuis.tech/",
+            "adminUrl": "https://vouch.example.org/",
             "alwaysDisplayInConsole": false,
             "attributes": {
                 "acr.loa.map": "{}",
                 "backchannel.logout.revoke.offline.tokens": "false",
                 "backchannel.logout.session.required": "true",
                 "client.secret.creation.time": "1688805167",
                 "client_credentials.use_refresh_token": "false",
@@ -151,17 +151,17 @@
                 "offline_access",
                 "microprofile-jwt"
             ],
             "protocol": "openid-connect",
             "publicClient": false,
             "redirectUris": [
                 "https://oidcdebugger.com/debug",
-                "https://vouch.vleermuis.tech/auth"
+                "https://vouch.example.org/auth"
             ],
-            "rootUrl": "https://vouch.vleermuis.tech",
+            "rootUrl": "https://vouch.example.org",
             "secret": "8m0c9DhS9jNWskIEgF2CGTsUQGhkmpte",
             "serviceAccountsEnabled": false,
             "standardFlowEnabled": true,
             "surrogateAuthRequired": false,
             "webOrigins": [
                 "+"
             ]
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/constants.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 """
 NAME: constants.py
 DESC: everything to do with initial configuration of a new environment
 """
 
 from getpass import getuser
 from importlib.metadata import version as get_version
-from os import environ, path, uname
+from os import environ, path, uname, makedirs
 from pathlib import Path
 from ruamel.yaml import YAML
 from shutil import copyfile
+import tarfile
 from xdg_base_dirs import xdg_cache_home, xdg_config_home
 
 # env
 SYSINFO = uname()
 # this will be something like ('Darwin', 'x86_64')
 OS = (SYSINFO.sysname, SYSINFO.machine)
 
+# don't show pygame hello message
+environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
+
 HOME_DIR = environ["HOME"]
 USER = getuser()
 
 # pathing
 PWD = path.dirname(__file__)
 
 # for smol-k8s-lab configs and cache
@@ -39,15 +43,14 @@
 Path(KUBE_DIR).mkdir(exist_ok=True)
 
 # version of smol-k8s-lab
 VERSION = get_version('smol-k8s-lab')
 # grabs the default packaged config file from default dot files
 DEFAULT_CONFIG_FILE = path.join(PWD, 'config/default_config.yaml')
 
-
 def load_yaml(yaml_config_file=XDG_CONFIG_FILE):
     """
     load config yaml files for smol-k8s-lab and return as dicts
     """
     # create default pathing and config file if it doesn't exist
     if not path.exists(yaml_config_file):
         Path(XDG_CONFIG_DIR).mkdir(parents=True, exist_ok=True)
@@ -58,14 +61,31 @@
     with open(yaml_config_file, 'r') as yaml_file:
         return yaml.load(yaml_file)
 
 
 DEFAULT_CONFIG = load_yaml(DEFAULT_CONFIG_FILE)
 INITIAL_USR_CONFIG = load_yaml()
 
+# sets the default speech files and loads them for each language
+# if you don't see your language, please submit a PR :)
+SPEECH_TEXT = path.join(PWD, 'config/audio')
+
+# we default save all generated speech files to your XDG_DATA_HOME env var
+SPEECH_MP3_DIR = path.join(PWD, 'audio')
+en_dir = path.join(SPEECH_MP3_DIR, 'en')
+if not path.exists(en_dir):
+    # create the dirs
+    makedirs(en_dir, exist_ok=True)
+    # open file
+    file = tarfile.open(path.join(SPEECH_MP3_DIR, "audio-en.tar.gz"))
+    # extract files
+    file.extractall(SPEECH_MP3_DIR)
+    # close file
+    file.close()
+
 DEFAULT_DISTRO_OPTIONS = DEFAULT_CONFIG['k8s_distros']
 
 if 'Darwin' in OS[0]:
     # macOS can't run k3s yet
     DEFAULT_DISTRO_OPTIONS.pop('k3s')
     DEFAULT_DISTRO = 'kind'
 else:
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/env_config.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from .networking.cilium import configure_cilium
 from .secrets_management.external_secrets_operator import configure_external_secrets
 from .secrets_management.infisical import configure_infisical
 from .secrets_management.vault import configure_vault
 from .social.matrix import configure_matrix
 from .social.mastodon import configure_mastodon
 from .social.nextcloud import configure_nextcloud
-from .social.home_assistant import configure_home_assistant
 
 
 def setup_k8s_secrets_management(k8s_obj: K8s,
                                  k8s_distro: str,
                                  eso_dict: dict = {},
                                  eso_provider: str = "",
                                  infisical_dict: dict = {},
@@ -41,31 +40,31 @@
     """
     sets up k8s secrets management tooling
     """
     # secrets management section
     header_msg = "Setting up K8s secret management with [green]"
 
     # setup external secrets operator and bitwarden external secrets
-    if eso_dict.get('enabled', False):
+    if eso_dict['enabled']:
         header_msg += f'External Secrets Operator[/] and [blue]{eso_provider}[/] as the Provider'
         header(header_msg, '🤫')
         configure_external_secrets(k8s_obj,
                                    eso_dict,
                                    eso_provider,
                                    k8s_distro,
                                    bitwarden)
 
     # setup infisical - an secrets manager and operator for k8s that replaces eso
-    elif infisical_dict.get('enabled', False):
+    elif infisical_dict['enabled']:
         header_msg += 'Infisical Secrets Operator[/]'
         header(header_msg, '🤫')
         configure_infisical(k8s_obj, infisical_dict)
 
     # setup hashicorp's vault, a secret key management system that works with eso
-    if vault_dict.get('enabled', False):
+    if vault_dict['enabled']:
         configure_vault(k8s_obj, vault_dict)
 
 
 def setup_oidc_provider(k8s_obj: K8s,
                         api_tls_verify: bool = False,
                         zitadel_dict: dict = {},
                         vouch_dict: dict = {},
@@ -75,19 +74,19 @@
     sets up oidc provider. only zitadel is supported right now
     if we choose to add keycloak back, we'll be adding the following arg
     keycloak_dict: dict = {}
     """
     header("Setting up [green]OIDC[/]/[green]Oauth[/] Applications")
 
     # keycloak_enabled = keycloak_dict['enabled']
-    zitadel_enabled = zitadel_dict.get('enabled', False)
+    zitadel_enabled = zitadel_dict['enabled']
 
     vouch_enabled = False
     if vouch_dict:
-        vouch_enabled = vouch_dict.get('enabled', False)
+        vouch_enabled = vouch_dict['enabled']
 
     # setup keycloak if we're using that for OIDC
     # if keycloak_enabled:
     #     log.debug("Setting up keycloak")
     #     configure_keycloak(k8s_obj, keycloak_dict, bw)
     #     realm = keycloak_dict['argo']['secret_keys']['default_realm']
     #     user = keycloak_dict['init']['values']['username']
@@ -143,35 +142,37 @@
                     metallb_dict: dict = {},
                     ingress_dict: dict = {},
                     cert_manager_dict: dict = {},
                     argo_enabled: bool = False,
                     argo_secrets_plugin_enabled: bool = False,
                     plugin_secrets: dict = {},
                     bw: BwCLI = None) -> None:
-    """
+    """ 
     Uses Helm to install all base apps that need to be running being argo cd:
         cilium, metallb, ingess-nginx, cert-manager, argo cd, argocd secrets plugin
     All Needed for getting Argo CD up and running.
     """
-    metallb_enabled = metallb_dict.get('enabled', False)
-    cilium_enabled = cilium_dict.get('enabled', False)
-    ingress_nginx_enabled = ingress_dict.get('enabled', False)
+    metallb_enabled = metallb_dict['enabled']
+    cilium_enabled = cilium_dict['enabled']
+    ingress_nginx_enabled = ingress_dict["enabled"]
     # make sure helm is installed and the repos are up to date
     prepare_helm(k8s_distro, argo_enabled, metallb_enabled, cilium_enabled,
                  argo_secrets_plugin_enabled)
 
     # needed for network policy editor and hubble UI
     if cilium_enabled:
-        header("Installing [green]cilium[/green] so we have networking tools", '🛜')
+        header("Installing [green]cilium[/green] so we have networking tools",
+               '🛜')
         if cilium_dict['init']['enabled']:
             configure_cilium(cilium_dict)
 
     # needed for metal (non-cloud provider) installs
     if metallb_enabled:
-        header("Installing [green]metallb[/green] so we have an IP address pool.", '🛜')
+        header("Installing [green]metallb[/green] so we have an IP address pool",
+               '🛜')
         if metallb_dict['init']['enabled']:
             cidr = metallb_dict['init']['values']['address_pool']
             if not cidr:
                 m = "[green]Please enter a comma seperated list of IPs or CIDRs"
                 cidr = Prompt.ask(m).split(',')
 
             configure_metallb(k8s_obj, cidr)
@@ -181,44 +182,40 @@
         # nginx just because that's most supported, treafik support may be added later
         header("Installing [green]ingress-nginx-controller[/green] to access web"
                " apps outside the cluster", "🌐")
         configure_ingress_nginx(k8s_obj, k8s_distro)
 
     # manager SSL/TLS certificates via lets-encrypt
     header("Installing [green]cert-manager[/green] for TLS certificates...", '📜')
-    if cert_manager_dict.get('enabled', False):
+    if cert_manager_dict["enabled"]:
         configure_cert_manager(k8s_obj, cert_manager_dict['init'])
 
     # then we install argo cd if it's enabled
     if argo_enabled:
         configure_argocd(k8s_obj,
-                         bw,
+                         bw, 
                          argo_secrets_plugin_enabled,
                          plugin_secrets)
 
     if ingress_nginx_enabled and argo_enabled:
         install_ingress_nginx_argocd_app(k8s_obj, ingress_dict)
 
 
 def setup_federated_apps(k8s_obj: K8s,
                          api_tls_verify: bool = False,
-                         home_assistant_dict: dict = {},
                          nextcloud_dict: dict = {},
                          mastodon_dict: dict = {},
                          matrix_dict: dict = {},
                          zitadel_hostname: str = "",
                          zitadel_obj: Zitadel = None,
                          bw: BwCLI = None) -> None:
     """
     Setup any federated apps with initialization supported
     """
-    if home_assistant_dict.get('enabled', False):
-        configure_home_assistant(k8s_obj, home_assistant_dict, api_tls_verify, bw)
-
-    if nextcloud_dict.get('enabled', False):
+    if nextcloud_dict['enabled']:
         configure_nextcloud(k8s_obj, nextcloud_dict, bw, zitadel_obj)
 
-    if mastodon_dict.get('enabled', False):
+    if mastodon_dict['enabled']:
         configure_mastodon(k8s_obj, mastodon_dict, bw)
 
-    if matrix_dict.get('enabled', False):
+    if matrix_dict['enabled']:
         configure_matrix(k8s_obj, matrix_dict, zitadel_obj, bw)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,44 +6,44 @@
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 import bcrypt
 import logging as log
 from os import path
 import yaml
 from ..constants import XDG_CACHE_DIR
-from ..k8s_tools.argocd_util import check_if_argocd_app_exists
+from ..k8s_tools.argocd_util import ArgoCD
 from ..k8s_tools.helm import Helm
 from ..k8s_tools.k8s_lib import K8s
 from ..bitwarden.bw_cli import BwCLI
-from ..utils.subproc import subproc
 from ..utils.passwords import create_password
 from ..utils.rich_cli.console_logging import header, sub_header
 
 
 def configure_argocd(k8s_obj: K8s,
-                     bitwarden: BwCLI = None,
-                     plugin_secret_creation: bool = False,
-                     secret_dict: dict = {}) -> None:
+                     argocd_config_dict: dict = {},
+                     secret_dict: dict = {},
+                     bitwarden: BwCLI = None) -> ArgoCD:
     """
     Installs argocd with ingress enabled by default and puts admin pass in a
     password manager, currently only bitwarden is supported
     arg:
       k8s_obj:                K8s() object with the kubernetes context
       bitwarden:              BwCLI() object, defaults to None
       plugin_secret_creation: boolean for creating the plugin secret generator
       secret_dict:            set of secrets to create for secret plugin
     """
     header("Installing [green]Argo CD[/green] for managing your Kubernetes apps",
            "🦑")
 
+    namespace = argocd_config_dict['argo']['namespace']
     # this is needed for helm but also setting argo to use the current k8s context
     argo_cd_domain = secret_dict['argo_cd_hostname']
 
     # immediately start building helm object to check if helm release exists
-    release_dict = {"release_name": "argo-cd", "namespace": "argocd"}
+    release_dict = {"release_name": "argo-cd", "namespace": namespace}
     release = Helm.chart(**release_dict)
 
     if not release.check_existing():
         # this is the base python dict for the values.yaml that is created below
         val = {"fullnameOverride": "argo-cd",
                "dex": {"enabled": False},
                "configs": {
@@ -93,51 +93,90 @@
         with open(values_file_name, 'w') as values_file:
             yaml.dump(val, values_file)
 
         release_dict['values_file'] = values_file_name
         release_dict['chart_name'] = 'argo-cd/argo-cd'
 
         release = Helm.chart(**release_dict)
-        release.install(True)
+        release.install(wait=True)
 
-    if plugin_secret_creation:
-        configure_secret_plugin_generator(k8s_obj, secret_dict)
+    argocd = ArgoCD(namespace, argo_cd_domain, k8s_obj)
 
-    # setup Argo CD to talk directly to k8s
-    log.debug("setting namespace to argocd and configuring argocd to use k8s for auth")
-    subproc(['kubectl config set-context --current --namespace=argocd',
-             f'argocd login {argo_cd_domain} --core'])
-
-
-def configure_secret_plugin_generator(k8s_obj: K8s, secret_dict: dict):
+    # install the appset secret plugin generator if we're using that
+    if "github.com/small-hack/argocd-apps" in argocd_config_dict['argo']['repo']:
+        if argocd_config_dict['argo']['directory_recursion']:
+            configure_secret_plugin_generator(argocd,
+                                              argocd_config_dict,
+                                              secret_dict)
+    return argocd
+
+
+def configure_secret_plugin_generator(argocd: ArgoCD,
+                                      argocd_config: dict,
+                                      secret_dict: dict) -> None:
     """
     configures the applicationset secret plugin generator
 
     (._. ) <-- who are they?
     """
-    # creates the secret vars secret with all the key/values for each appset
-    k8s_obj.create_secret('appset-secret-vars', 'argocd', secret_dict,
-                          'secret_vars.yaml')
+    if not argocd.check_if_app_exists('appset-secrets-plugin'):
+        # creates the secret vars secret with all the key/values for each appset
+        argocd.k8s.create_secret('appset-secret-vars', 'argocd', secret_dict,
+                                 'secret_vars.yaml')
 
-    if not check_if_argocd_app_exists('appset-secrets-plugin'):
         msg = "🔌 Installing the ApplicationSet Secret Plugin Generator for Argo CD..."
         sub_header(msg)
 
         # creates only the token for authentication
         token = create_password()
-        k8s_obj.create_secret('appset-secret-token', 'argocd', {'token': token})
+        argocd.k8s.create_secret('appset-secret-token', 'argocd', {'token': token})
 
         # this creates a values.yaml from this dict
         set_opts = {'secretVars.existingSecret': 'appset-secret-vars',
                     'token.existingSecret': 'appset-secret-token'}
 
         # install the helm chart :)
         release = Helm.chart(
                 release_name='appset-secret-plugin',
                 chart_name='appset-secret-plugin/appset-secret-plugin',
                 namespace='argocd',
                 set_options=set_opts
                 )
-        release.install(True)
+        release.install(wait=True)
+
+        # gotta make sure the project already exists
+        log.info("Creating argocd project if it does not exist...")
+
+        # get project namespaces
+        proj_ns = argocd_config['argo']['project']['destination']['namespaces']
+        if argocd.namespace not in proj_ns:
+            proj_ns.append(argocd.namespace)
+
+        # create argocd project
+        argocd.create_project(argocd_config['argo']['project']['name'],
+                              "Argo CD",
+                              proj_ns,
+                              argocd_config['argo']['cluster'],
+                              set(argocd_config['argo']['project']['source_repos']))
+
+        # immediately install the argocd appset plugin
+        log.info("Immediately installing the appset secret plugin via Argo CD")
+        repo_url = argocd_config['argo']['repo'].replace("https://","").replace("http://","")
+        url_sections = repo_url.replace("github.com/", "").split('/')
+        owner = url_sections[0]
+        repo_name = url_sections[1].replace(".git", "")
+        ref = argocd_config['argo']['revision']
+        path = argocd_config['argo']['path']
+        if not path.endswith("/"):
+            path += "/"
+
+        appset_secrets_yaml = (
+                f"https://raw.githubusercontent.com/{owner}/{repo_name}/"
+                f"{ref}/{path}appset_secret_plugin/"
+                "appset_secret_plugin_generator_argocd_app.yaml"
+                )
+
+        log.info(f"applying {appset_secrets_yaml}")
+        argocd.k8s.apply_manifests(appset_secrets_yaml, argocd.namespace)
     else:
         log.info("Reloading deployment for Argo CD Appset Secret Plugin")
-        k8s_obj.reload_deployment('appset-secret-plugin', 'argocd')
+        argocd.update_appset_secret(secret_dict)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging as log
 import json
 from rich.prompt import Prompt
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
-from smol_k8s_lab.k8s_tools.argocd_util import install_with_argocd
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
+from smol_k8s_lab.utils.run.subproc import subproc
 from smol_k8s_lab.utils.passwords import create_password
 from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
 
 
 class Keycloak():
     """
     Python Wrapper for the keycloak cli
@@ -21,15 +20,15 @@
         self.realm = realm
         self.exec_path = ("kubectl exec -n keycloak keycloak-web-app-0 -- "
                           "/opt/bitnami/keycloak/bin/kcadm.sh ")
         self.cfg = (f" -o --no-config --server http://localhost:8080/ --realm {realm}"
                     "--user KEYCLOAK_ADMIN --password $KEYCLOAK_ADMIN_PASSWORD")
 
     def create_user(self, username: str, first_name: str, last_name: str) -> None:
-        """ 
+        """
         creates a user via the keycloak cli
         """
         log.info(f"Creating a new user for {username}")
         # create a new user
         cmd = (f"create users -r {self.realm} -s username={username} -s enabled=true "
                f"-s firstName={first_name} -s lastName={last_name}")
         subproc([self.exec_path + cmd + self.cfg])
@@ -43,24 +42,23 @@
         subproc([self.exec_path + cmd + self.cfg])
 
         # get client and return the client secret
         cmd = f"get clients -r {self.realm} --fields clientId,secret --query {clientId}"
         return json.loads(subproc([self.exec_path + cmd + self.cfg]))['secret']
 
 
-def configure_keycloak(k8s_obj: K8s,
+def configure_keycloak(argocd: ArgoCD,
                        config_dict: dict,
                        bitwarden: BwCLI = None) -> True:
     """
     Installs Keycloak as an Argo CD Application. If config_dict['init']['enabled']
     is True, it also configures Argo CD as OIDC Client.
 
     Required Arguments:
-        K8s: K8s() class instance so we can create secrets and install with
-             argo using a direct connection to the cluster
+        argocd:      ArgoCD obj for making argo cd calls
         config_dict: dict, Argo CD parameters for keycloak
 
     Optional Arguments:
         bitwarden:         BwCLI obj, [optional] contains bitwarden session
 
     Returns True if successful.
     """
@@ -85,42 +83,42 @@
                                    user='keycloak',
                                    password=postgres_password)
 
         # if we're not using bitwarden, create the k8s secrets directly
         else:
             sub_header("Creating secrets in k8s")
             admin_password = create_password()
-            k8s_obj.create_secret('keycloak-admin-credentials', 'keycloak',
-                                  {'password': admin_password})
+            argocd.k8s.create_secret('keycloak-admin-credentials', 'keycloak',
+                                     {'password': admin_password})
             postgres_password = create_password()
-            k8s_obj.create_secret('keycloak-postgres-credentials', 'keycloak',
-                                  {'password': postgres_password,
-                                   'postgres-password': postgres_password})
+            argocd.k8s.create_secret('keycloak-postgres-credentials', 'keycloak',
+                                     {'password': postgres_password,
+                                      'postgres-password': postgres_password})
 
-    install_with_argocd(k8s_obj, 'keycloak', config_dict['argo'])
+    argocd.install_app('keycloak', config_dict['argo'])
 
     # only continue through the rest of the function if we're initializes a
     # user and argocd client in keycloak
     if config_dict['init']['enabled']:
         realm = secrets['default_realm']
-        initialize_keycloak(k8s_obj, realm, config_dict['init']['values'], bitwarden)
+        initialize_keycloak(realm, config_dict['init']['values'], bitwarden)
     # always return True
     return True
 
 
-def initialize_keycloak(k8s_obj: K8s,
+def initialize_keycloak(argocd: ArgoCD,
                         realm: str,
                         initial_user_dict: dict = {"username": "",
                                                    "first_name": "",
                                                    "last_name": ""},
                         bitwarden=None) -> True:
     """
     Sets up initial Keycloak user, Argo CD client.
     Arguments:
-      k8s_obj:           K8s object to use for creating initial secrets
+      argocd:            ArgoCD obj for making argo cd calls
       realm:             name of the keycloak realm to use
       initial_user_dict: initial user dict with username, first_name, last_name
       bitwarden:         BwCLI obj, [optional] session to use for bitwarden
     """
     sub_header("Configuring Keycloak as your OIDC SSO for Argo CD")
     username = initial_user_dict['username']
     if not username:
@@ -134,23 +132,23 @@
 
     # create keycloak object
     keycloak = Keycloak(realm)
 
     # create initial user
     keycloak.create_user(username, first_name, last_name)
 
-    # create intial client for 
+    # create intial client for
     argocd_client_secret = keycloak.create_client("argocd")
 
 
     if bitwarden:
         sub_header("Creating OIDC secret for Argo CD OIDC in Bitwarden")
         bitwarden.create_login(name='argocd-external-oidc',
                                user='argocd',
                                password=argocd_client_secret)
     else:
         # the argocd secret needs labels.app.kubernetes.io/part-of: "argocd"
-        k8s_obj.create_secret('argocd-external-oidc', 'argocd',
-                              {'user': 'argocd',
-                               'password': argocd_client_secret}, False,
-                              {'app.kubernetes.io/part-of': 'argocd'})
+        argocd.k8s.create_secret('argocd-external-oidc', 'argocd',
+                                 {'user': 'argocd',
+                                  'password': argocd_client_secret}, False,
+                                 {'app.kubernetes.io/part-of': 'argocd'})
     return True
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 import logging as log
 from rich.prompt import Prompt
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
 from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                check_if_argocd_app_exists,
-                                                update_argocd_appset_secret)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.rich_cli.console_logging import header
 from smol_k8s_lab.utils.passwords import create_password
-from .keycloak import Keycloak
+# from .keycloak import Keycloak
 
 
-def configure_vouch(k8s_obj: K8s,
-                    vouch_config_dict: dict,
-                    oidc_provider_name: str = "",
+def configure_vouch(argocd: ArgoCD,
+                    cfg: dict,
                     oidc_provider_hostname: str = "",
                     bitwarden: BwCLI = None,
-                    users: list = [],
-                    realm: str = "",
                     zitadel: Zitadel = None) -> None:
     """
     Installs vouch-proxy as an Argo CD application on Kubernetes
 
     Required Args:
-      k8s_obj:                K8s(), for the authenticated k8s client
-      vouch_config_dict:      Argo CD parameters
+      argocd:         ArgoCD object for argo-cd operations
+      cfg:            Full smol_k8s_lab app dict for vouch
 
     Optional Args:
-      oidc_provider_name:     OIDC provider name. options: keycloak, zitadel
       oidc_provider_hostname: OIDC provider hostname e.g. zitadel.example.com
       bitwarden:              BwCLI, to store k8s secrets in bitwarden
-      users:                  list of user to give access to vouch app
-      realm:                  str keycloak realm to use
-      zitadel:                Zitadel api object 
-    """
-    header("Setting up [green]Vouch[/] to use Oauth for insecure frontends", "🗝️")
+      zitadel:                Zitadel api object
 
+    Disabled Args because we're not supporting keycloak right now:
+      oidc_provider_name:     OIDC provider name. options: keycloak, zitadel, disabled
+      realm:                  str keycloak realm to use, not functional right now
+    """
     # make sure vouch isn't already installed
-    app_installed = check_if_argocd_app_exists("vouch")
+    app_installed = argocd.check_if_app_exists("vouch")
+
+    if app_installed:
+        header_start = "Syncing"
+    else:
+        header_start = "Setting up"
+
+    header(f"{header_start} [green]Vouch[/] to use OAuth for insecure frontends",
+           "🗝️")
+
     # this handles the vouch-oauth-config secret data
-    secrets = vouch_config_dict['argo']['secret_keys']
+    secrets = cfg['argo']['secret_keys']
     if secrets:
         vouch_hostname = secrets['hostname']
 
-    if vouch_config_dict['init']['enabled'] and not app_installed:
-        auth_dict = create_vouch_app(provider=oidc_provider_name,
-                                     provider_hostname=oidc_provider_hostname,
+    init_enabled = cfg['init']['enabled']
+
+    if init_enabled and not app_installed:
+        auth_dict = create_vouch_app(provider_hostname=oidc_provider_hostname,
                                      vouch_hostname=vouch_hostname,
-                                     users=users,
-                                     zitadel=zitadel,
-                                     realm=realm)
+                                     zitadel=zitadel)
         vouch_callback_url = f'https://{vouch_hostname}/auth'
         # trying to create a string of ""
         preferred_domain = '\"\"'
 
         # this is handling the vouch-config secret
-        emails = vouch_config_dict['init']['values']['emails']
+        emails = cfg['init']['values']['emails']
         if not emails:
             m = ("[green]Please enter a comma seperated list of [yellow]emails[/]"
                  " that are allowed to access domains behind Vouch")
             emails = Prompt.ask(m)
         else:
             emails = ','.join(emails)
         log.debug(f"Allowing vouch to be accessed by emails: {emails}")
 
-        domains = vouch_config_dict['init']['values']['domains']
+        domains = cfg['init']['values']['domains']
         if not domains:
             m = ("[green]Please enter a comma seperated list of [yellow]domains[/]"
                  " that are allowed to use Vouch")
             domains = Prompt.ask(m)
         else:
             domains = ','.join(domains)
         log.debug(f"Allowing vouch to be used by these domains: {domains}")
@@ -111,123 +112,125 @@
                     user='vouch',
                     item_url=vouch_hostname,
                     password='none',
                     fields=[domains_obj, emails_obj, jwt_secret_obj]
                     )
 
             # update the vouch values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'vouch_oauth_config_bitwarden_id': oauth_id,
                      'vouch_config_bitwarden_id': vouch_id}
                     )
 
             # reload the bitwarden ESO provider
             try:
-                k8s_obj.reload_deployment('bitwarden-eso-provider', 'external-secrets')
+                argocd.k8s.reload_deployment('bitwarden-eso-provider',
+                                             'external-secrets')
             except Exception as e:
                 log.error(
                         "Couldn't scale down the [magenta]bitwarden-eso-provider[/]"
                         "deployment in [green]external-secrets[/] namespace. Recieved: "
                         f"{e}"
                         )
 
         # create vouch k8s secrets if we're not using bitwarden
         else:
             # create oauth OIDC k8s secret
-            k8s_obj.create_secret('vouch-oauth-config',
-                                  'vouch',
-                                  {'user': auth_dict['client_id'],
-                                   'password': auth_dict['client_secret'],
-                                   'authUrl': auth_dict['auth_url'],
-                                   'tokenUrl': auth_dict['token_url'],
-                                   'userInfoUrl': auth_dict['user_info_url'],
-                                   'endSessionEndpoint': auth_dict['end_session_url'],
-                                   'callbackUrls': vouch_callback_url,
-                                   'preferredDomain': preferred_domain})
+            argocd.k8s.create_secret(
+                    'vouch-oauth-config',
+                    'vouch',
+                    {'user': auth_dict['client_id'],
+                     'password': auth_dict['client_secret'],
+                     'authUrl': auth_dict['auth_url'],
+                     'tokenUrl': auth_dict['token_url'],
+                     'userInfoUrl': auth_dict['user_info_url'],
+                     'endSessionEndpoint': auth_dict['end_session_url'],
+                     'callbackUrls': vouch_callback_url,
+                     'preferredDomain': preferred_domain})
 
             # create vouch config k8s secret
-            k8s_obj.create_secret('vouch-config', 'vouch',
-                                  {'domains': domains,
-                                   'allowList': emails,
-                                   'jwtSecret': jwt_secret})
+            argocd.k8s.create_secret('vouch-config',
+                                     'vouch',
+                                     {'domains': domains,
+                                      'allowList': emails,
+                                      'jwtSecret': jwt_secret})
 
     if not app_installed:
-        install_with_argocd(k8s_obj, 'vouch', vouch_config_dict['argo'])
+        argocd.install_app('vouch', cfg['argo'])
     else:
         log.info("vouch-proxy already installed 🎉")
 
         # we need to still update the bitwarden IDs if bitwarden and init is enabled
-        if vouch_config_dict['init']['enabled'] and bitwarden:
+        if init_enabled and bitwarden:
             log.debug("Updating vouch bitwarden IDs in the appset secret")
             oauth_id = bitwarden.get_item(
                     f"vouch-oauth-config-{vouch_hostname}"
                     )[0]['id']
 
             vouch_id = bitwarden.get_item(
                     f"vouch-config-{vouch_hostname}", False
                     )[0]['id']
 
             # update the vouch values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'vouch_oauth_config_bitwarden_id': oauth_id,
                      'vouch_config_bitwarden_id': vouch_id}
                    )
 
 
-def create_vouch_app(provider: str,
-                     provider_hostname: str,
+def create_vouch_app(provider_hostname: str,
                      vouch_hostname: str = "",
-                     users: list = [],
-                     zitadel: Zitadel = None,
-                     realm: str = "default") -> list:
+                     zitadel: Zitadel = None) -> list:
     """
     Creates an OIDC application, for vouch-proxy, in either Keycloak or Zitadel
 
     Arguments:
-      provider          - either 'keycloak' or 'vouch'
       provider_hostname - hostname of keycloak or vouch
       vouch_hostname    - hostname of vouch
-      zitadel           - Zitadel api object 
-      realm             - realm to use for keycloak if using keycloak
+      zitadel           - Zitadel api object
+
+
+    Disabled Arguments because we don't supprot keycloak right now:
+      provider          - either 'keycloak' or 'zitadel'
+      realm             - realm to use for keycloak if using keycloak,
+                          default is 'default'
 
     returns [url, client_id, client_secret]
     """
     # create Vouch OIDC Application
-    if provider == 'zitadel':
-        log.info("Creating an OIDC application for Vouch via Zitadel...")
-        vouch_dict = zitadel.create_application(
-                "vouch", 
-                f"https://{vouch_hostname}/auth",
-                [f"https://{vouch_hostname}"]
-                )
-        zitadel.create_role("vouch_users", "Vouch Users", "vouch_users")
-        zitadel.update_user_grant(['vouch_users'])
-
-        client_id = vouch_dict['client_id']
-        client_secret = vouch_dict['client_secret']
-        auth_url = f'https://{provider_hostname}/oauth/v2/authorize'
-        token_url = f'https://{provider_hostname}/oauth/v2/token'
-        user_info_url = f'https://{provider_hostname}/oidc/v1/userinfo'
-        end_session_url = f'https://{provider_hostname}/oidc/v1/end_session'
-
-    elif provider == 'keycloak':
-        keycloak = Keycloak()
-        # create a vouch client
-        client_secret = keycloak.create_client('vouch')
-        client_id = 'vouch'
-        url = f"https://{provider_hostname}/realms/{realm}/protocol/openid-connect"
-        auth_url = f'{url}/auth'
-        token_url = f'{url}/token'
-        user_info_url = f'{url}/userinfo'
-        end_session_url = f'{url}/end_session'
-    else:
-        log.error("niether zitadel nor keycloak was passed into create_vouch_app,"
-                  f" got {provider} instead.")
+    # if provider == 'zitadel':
+    log.info("Creating an OIDC application for Vouch via Zitadel...")
+    vouch_dict = zitadel.create_application(
+            "vouch",
+            f"https://{vouch_hostname}/auth",
+            [f"https://{vouch_hostname}"]
+            )
+    zitadel.create_role("vouch_users", "Vouch Users", "vouch_users")
+    zitadel.update_user_grant(['vouch_users'])
+
+    client_id = vouch_dict['client_id']
+    client_secret = vouch_dict['client_secret']
+    auth_url = f'https://{provider_hostname}/oauth/v2/authorize'
+    token_url = f'https://{provider_hostname}/oauth/v2/token'
+    user_info_url = f'https://{provider_hostname}/oidc/v1/userinfo'
+    end_session_url = f'https://{provider_hostname}/oidc/v1/end_session'
+
+    # elif provider == 'keycloak':
+    #     keycloak = Keycloak()
+    #     # create a vouch client
+    #     client_secret = keycloak.create_client('vouch')
+    #     client_id = 'vouch'
+    #     url = f"https://{provider_hostname}/realms/{realm}/protocol/openid-connect"
+    #     auth_url = f'{url}/auth'
+    #     token_url = f'{url}/token'
+    #     user_info_url = f'{url}/userinfo'
+    #     end_session_url = f'{url}/end_session'
+    # else:
+    #     log.error("niether zitadel nor keycloak was passed into create_vouch_app,"
+    #               f" got {provider} instead.")
 
     auth_dict = {"auth_url": auth_url,
                  "token_url": token_url,
                  "user_info_url": user_info_url,
                  "end_session_url": end_session_url,
                  "client_id": client_id,
                  "client_secret": client_secret}
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,270 +1,201 @@
 from base64 import standard_b64decode as b64dec
 from json import loads
 import logging as log
-from .zitadel_api import Zitadel
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                wait_for_argocd_app,
-                                                check_if_argocd_app_exists,
-                                                update_argocd_appset_secret)
+from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
+from smol_k8s_lab.k8s_apps.operators.minio import create_minio_alias
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
+from smol_k8s_lab.k8s_tools.restores import restore_seaweedfs, restore_cnpg_cluster
+from smol_k8s_lab.utils.value_from import process_backup_vals
 from smol_k8s_lab.utils.passwords import create_password
 from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
 
 
-def configure_zitadel(k8s_obj: K8s,
-                      config_dict: dict,
+def configure_zitadel(argocd: ArgoCD,
+                      cfg: dict,
+                      pvc_storage_class: str = "",
                       api_tls_verify: bool = False,
-                      argocd_hostname: str = "",
                       bitwarden: BwCLI = None) -> dict | None:
     """
-    Installs zitadel as a Argo CD Applications. If config_dict['init']['enabled']
+    Installs zitadel as a Argo CD Applications. If cfg['init']['enabled']
     is True, it also configures Argo CD as OIDC Clients.
 
     Required Arguments:
-        k8s_obj:      K8s(), kubrenetes client for creating secrets
-        config_dict:  dict, Argo CD parameters for zitadel
+        argocd:             ArgoCD obj for doing Argo operations
+        cfg:                dict, Argo CD parameters for zitadel
+        pvc_storage_class:  str, storage class of PVC
 
     Optional Arguments:
-        argocd_hostname:  str, the hostname of Argo CD
-        bitwarden:        BwCLI obj, [optional] contains bitwarden session
+        api_tls_verify:    bool, enable https verification for zitadel api
+        bitwarden:         BwCLI obj, [optional] contains bitwarden session
 
     If no init: Returns True if successful.
     If init AND vouch_hostname, returns vouch credentials
     """
-    header("Setting up [green]Zitadel[/], our identity management solution", "👥")
+    # check to make sure the app instead already installed with Argo CD
+    app_installed = argocd.check_if_app_exists('zitadel')
+
+    # declare the init dict
+    init_dict = cfg.get('init', {'enabled': False, 'restore': {'enabled': False}})
+    init_enabled = init_dict['enabled']
 
     # immediately load in all the secret keys
-    secrets = config_dict['argo']['secret_keys']
+    secrets = cfg['argo']['secret_keys']
     if secrets:
         zitadel_hostname = secrets['hostname']
 
-    # check to make sure the app instead already installed with Argo CD
-    app_installed = check_if_argocd_app_exists('zitadel')
+    restore_dict = cfg['init'].get('restore', {"enabled": False})
+    restore_enabled = restore_dict['enabled']
+    if restore_enabled:
+        prefix = "Restoring"
+    else:
+        if app_installed:
+            prefix = "Syncing"
+        else:
+            prefix = "Setting up"
 
-    # declare the init dict
-    init_dict = config_dict['init']
+    header(f"{prefix} [green]Zitadel[/], for your self hosted identity management",
+           "👥")
 
-    if init_dict['enabled'] and not app_installed:
+    if init_enabled and not app_installed:
         # process init and secret values
         init_values = init_dict['values']
 
-        # configure backup s3 credentials
-        s3_backup_access_id = init_values.get('s3_backup_access_id', 'zitadel')
-        s3_backup_access_key = init_values.get('s3_backup_secret_key', '')
-        restic_repo_pass = init_values.get('restic_repo_password', '')
-
-        # first we make sure the namespace exists
-        namespace = config_dict['argo']['namespace']
-        k8s_obj.create_namespace(namespace)
 
-        if bitwarden:
-            restic_repo_obj = create_custom_field('resticRepoPassword', restic_repo_pass)
-            s3_backup_id = bitwarden.create_login(
-                    name='zitadel-backups-s3-credentials',
-                    item_url=zitadel_hostname,
-                    user=s3_backup_access_id,
-                    password=s3_backup_access_key,
-                    fields=[restic_repo_obj]
-                    )
+        s3_endpoint = secrets.get('s3_endpoint', "")
+        if s3_endpoint and not restore_enabled:
+            s3_access_key = create_password()
+            # create a local alias to check and make sure nextcloud is functional
+            create_minio_alias(minio_alias="zitadel",
+                               minio_hostname=s3_endpoint,
+                               access_key="zitadel",
+                               secret_key=s3_access_key)
 
-            # S3 credentials
-            db_access_key = create_password()
-            s3_id = bitwarden.create_login(
-                    name='zitadel-postgres-s3-credentials',
-                    item_url=zitadel_hostname,
-                    user="zitadel-postgres",
-                    password=db_access_key
-                    )
-
-            admin_s3_key = create_password()
-            s3_admin_id = bitwarden.create_login(
-                    name='zitadel-admin-s3-credentials',
-                    item_url=zitadel_hostname,
-                    user="zitadel-root",
-                    password=admin_s3_key
-                    )
+        # configure backup s3 credentials
+        backup_vals = process_backup_vals(cfg.get('backups', ''), 'zitadel', argocd)
 
-            # create zitadel core key
-            new_key = bitwarden.generate()
-            core_id = bitwarden.create_login(name="zitadel-core-key",
-                                             user="admin-service-account",
-                                             item_url=zitadel_hostname,
-                                             password=new_key)
-
-            # create db credentials password dict
-            db_id = bitwarden.create_login(
-                    name="zitadel-db-credentials",
-                    user="zitadel",
-                    item_url=zitadel_hostname,
-                    password="using-tls-now-so-we-do-not-need-a-password"
-                    )
+        # first we make sure the namespace exists
+        namespace = cfg['argo']['namespace']
+        argocd.k8s.create_namespace(namespace)
 
-            # update the zitadel values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {'zitadel_core_bitwarden_id': core_id,
-                     'zitadel_db_bitwarden_id': db_id,
-                     'zitadel_s3_postgres_credentials_bitwarden_id': s3_id,
-                     'zitadel_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                     'zitadel_s3_backups_credentials_bitwarden_id': s3_backup_id}
-                    )
+        if bitwarden and not restore_enabled:
+            setup_bitwarden_items(argocd,
+                                  zitadel_hostname,
+                                  s3_endpoint,
+                                  s3_access_key,
+                                  backup_vals['s3_user'],
+                                  backup_vals['s3_password'],
+                                  backup_vals['restic_repo_pass'],
+                                  bitwarden)
 
-            # reload the bitwarden ESO provider
-            try:
-                k8s_obj.reload_deployment('bitwarden-eso-provider', 'external-secrets')
-            except Exception as e:
-                log.error(
-                        "Couldn't scale down the [magenta]bitwarden-eso-provider[/]"
-                        "deployment in [green]external-secrets[/] namespace. Recieved: "
-                        f"{e}"
-                        )
-        else:
+        elif not bitwarden and not restore_enabled:
             # create the zitadel core key
             secret_dict = {'masterkey': create_password()}
-            k8s_obj.create_secret(name="zitadel-core-key",
-                                  namespace=namespace,
-                                  str_data=secret_dict)
+            argocd.k8s.create_secret(name="zitadel-core-key",
+                                     namespace=namespace,
+                                     str_data=secret_dict)
 
             # this is just for the db username
-            k8s_obj.create_secret(name="zitadel-db-credentials",
-                                  namespace=namespace,
-                                  str_data={'username': 'zitadel'})
+            argocd.k8s.create_secret(name="zitadel-db-credentials",
+                                     namespace=namespace,
+                                     str_data={'username': 'zitadel'})
+
+    if not app_installed and restore_enabled:
+        restore_zitadel(argocd,
+                        zitadel_hostname,
+                        namespace,
+                        cfg['argo'],
+                        secrets,
+                        restore_dict,
+                        backup_vals,
+                        pvc_storage_class,
+                        'zitadel-postgres',
+                        bitwarden)
 
     # install Zitadel using ArgoCD
-    if not app_installed:
-        install_with_argocd(k8s_obj, 'zitadel', config_dict['argo'])
-
-        # only continue through the rest of the function if we're initializes a
-        # user and argocd client in zitadel
-        if init_dict['enabled']:
-            initial_user_dict = init_values
-            # we pop these off of the dictionary, because they're only needed
-            # for creating the backups s3 credentials in bitwarden
-            initial_user_dict.pop('s3_backup_access_id')
-            initial_user_dict.pop('s3_backup_secret_key')
-            initial_user_dict.pop('restic_repo_password')
-            # also don't need the smtp password past this point
-            try:
-                initial_user_dict.pop('smtp_password')
-            except Exception as e:
-                log.debug(e)
-                pass
+    argocd.install_app('zitadel', cfg['argo'])
 
-            # Before initialization, we need to wait for zitadel's API to be up
-            wait_for_argocd_app('zitadel', retry=True)
-            wait_for_argocd_app('zitadel-web-app', retry=True)
-            vouch_dict = initialize_zitadel(k8s_obj=k8s_obj,
-                                            zitadel_hostname=zitadel_hostname,
-                                            api_tls_verify=api_tls_verify,
-                                            user_dict=initial_user_dict,
-                                            argocd_hostname=argocd_hostname,
-                                            bitwarden=bitwarden)
-            return vouch_dict
+    # only continue through the rest of the function if we're initializes a
+    # user and argocd client in zitadel
+    if not app_installed and init_enabled and not restore_enabled:
+        initial_user_dict = init_values
+        # don't need the smtp password past this point
+        try:
+            initial_user_dict.pop('smtp_password')
+        except Exception as e:
+            log.debug(e)
+            pass
+
+        # Before initialization, we need to wait for zitadel's API to be up
+        argocd.wait_for_app('zitadel', retry=True)
+        argocd.wait_for_app('zitadel-web-app', retry=True)
+        vouch_dict = initialize_zitadel(argocd,
+                                        zitadel_hostname=zitadel_hostname,
+                                        api_tls_verify=api_tls_verify,
+                                        user_dict=initial_user_dict,
+                                        bitwarden=bitwarden)
+        return vouch_dict
     else:
         log.info("Zitadel is already installed 🎉")
 
-        if bitwarden and config_dict['init']['enabled']:
+        if bitwarden and init_enabled:
             # get the zitadel service account private key json for generating a jwt
-            adm_secret_file = k8s_obj.get_secret(
+            adm_secret_file = argocd.k8s.get_secret(
                     'zitadel-admin-sa',
                     'zitadel'
                     )['data']['zitadel-admin-sa.json']
 
             # setup and return the zitadel python api wrapper
             zitadel = Zitadel(
                     zitadel_hostname,
                     loads(b64dec(str.encode(adm_secret_file)).decode('utf8')),
                     api_tls_verify
                     )
             try:
                 zitadel.set_user_by_login_name(
-                        config_dict['init']['values']['username']
+                        cfg['init']['values']['admin_user']
                         )
             except Exception as e:
                 log.error(e)
 
             try:
                 zitadel.set_project_by_name(
-                        config_dict['init']['values']['project']
+                        cfg['init']['values']['project']
                         )
             except Exception as e:
                 log.error(e)
                 raise Exception(e)
 
-            # makes sure we update the appset secret with bitwarden IDs regardless
-            db_id = bitwarden.get_item(
-                    f"zitadel-db-credentials-{zitadel_hostname}"
-                    )[0]['id']
-
-            s3_backup_id = bitwarden.get_item(
-                    f"zitadel-backups-s3-credentials-{zitadel_hostname}", False
-                    )[0]['id']
-
-            s3_admin_id = bitwarden.get_item(
-                    f"zitadel-admin-s3-credentials-{zitadel_hostname}", False
-                    )[0]['id']
-
-            s3_id = bitwarden.get_item(
-                    f"zitadel-postgres-s3-credentials-{zitadel_hostname}", False
-                    )[0]['id']
-
-            core_id = bitwarden.get_item(
-                    f"zitadel-core-key-{zitadel_hostname}", False
-                    )[0]['id']
-
-            argo_oidc_item = bitwarden.get_item(
-                    f"argocd-oidc-credentials-{argocd_hostname}", False
-                    )[0]
-
-            argo_client_id = argo_oidc_item['login']['username']
-
-            # update the zitadel values for the argocd appset
-
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {
-                    'zitadel_core_bitwarden_id': core_id,
-                    'zitadel_db_bitwarden_id': db_id,
-                    'zitadel_s3_postgres_credentials_bitwarden_id': s3_id,
-                    'zitadel_s3_backups_credentials_bitwarden_id': s3_backup_id,
-                    'zitadel_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                    'argo_cd_oidc_issuer': f"https://{zitadel_hostname}",
-                    'argo_cd_oidc_client_id': argo_client_id,
-                    'argo_cd_oidc_logout_url': f"https://{zitadel_hostname}/oidc/v1/end_session",
-                    'argo_cd_oidc_bitwarden_id': argo_oidc_item['id']
-                    }
-                    )
+            refresh_bitwarden(argocd, zitadel_hostname, bitwarden)
 
-            # sync_argocd_app('zitadel')
-            # sync_argocd_app('argo-cd')
+            # argocd.sync_app('argo-cd')
 
             return zitadel
 
 
-def initialize_zitadel(k8s_obj: K8s,
+def initialize_zitadel(argocd: ArgoCD,
                        zitadel_hostname: str,
                        api_tls_verify: bool = False,
                        user_dict: dict = {},
-                       argocd_hostname: str = "",
                        bitwarden: BwCLI = None) -> dict | None:
     """
     Sets up initial zitadel user, Argo CD client
     Arguments:
-      k8s_obj:           K8s(), kubrenetes client for creating secrets
       zitadel_hostname:  str, the hostname of Zitadel
       api_tls_verify:    bool, whether or not to verify the TLS cert on request to api
-      user_dict:         dict of initial username, email, first name, last name
+      user_dict:         dict of initial admin_user, email, first name, last name
                          gender, and project to create
       argocd_hostname:   str, the hostname of Argo CD for oidc app
       bitwarden:         BwCLI obj, [optional] session to use for bitwarden
 
     returns Zitadel() with admin user/admin service account created with session token
     """
+    k8s_obj = argocd.k8s
+    argocd_hostname = argocd.hostname
 
     sub_header("Configuring zitadel as your OIDC SSO for Argo CD")
 
     # get the zitadel service account private key json for generating a jwt
     adm_secret = k8s_obj.get_secret('zitadel-admin-sa', 'zitadel')
     adm_secret_file = adm_secret['data']['zitadel-admin-sa.json']
     private_key_obj = loads(b64dec(str.encode(adm_secret_file)).decode('utf8'))
@@ -313,22 +244,226 @@
                               {'user': argocd_client['client_id'],
                                'password': argocd_client['client_secret']},
                               labels={'app.kubernetes.io/part-of': 'argocd'})
 
     # create zitadel admin user that the project is setup
     header("Creating a Zitadel user...")
     user_id = zitadel.create_user(bitwarden=bitwarden, **user_dict)
-    zitadel.set_user_by_login_name(user_dict['username'])
+    zitadel.set_user_by_login_name(user_dict['admin_user'])
     try:
         zitadel.create_user_grant(['argocd_administrators'])
     except Exception as e:
         log.error(e)
         zitadel.update_user_grant(['argocd_administrators'])
 
     # grant admin access to first user
     sub_header("creating user IAM membership with IAM_OWNER")
     zitadel.create_iam_membership(user_id, 'IAM_OWNER')
 
     # update appset-secret-vars secret with issuer, client_id, logout_url
-    update_argocd_appset_secret(k8s_obj, fields)
+    argocd.update_appset_secret(fields)
 
     return zitadel
+
+
+def setup_bitwarden_items(argocd: ArgoCD,
+                          zitadel_hostname: str,
+                          s3_endpoint: str,
+                          s3_access_key: str,
+                          backups_s3_user: str,
+                          backups_s3_password: str,
+                          restic_repo_pass: str,
+                          bitwarden: BwCLI) -> None:
+    """
+    setup all zitadel related bitwarden items and refresh the appset secret plugin
+    """
+    restic_repo_obj = create_custom_field('resticRepoPassword', restic_repo_pass)
+    s3_backup_id = bitwarden.create_login(
+            name='zitadel-backups-s3-credentials',
+            item_url=zitadel_hostname,
+            user=backups_s3_user,
+            password=backups_s3_password,
+            fields=[restic_repo_obj]
+            )
+
+    # S3 credentials
+    db_access_key = create_password()
+    s3_id = bitwarden.create_login(
+            name='zitadel-postgres-s3-credentials',
+            item_url=zitadel_hostname,
+            user="zitadel-postgres",
+            password=db_access_key
+            )
+
+    admin_s3_key = create_password()
+    s3_admin_id = bitwarden.create_login(
+            name='zitadel-admin-s3-credentials',
+            item_url=zitadel_hostname,
+            user="zitadel-root",
+            password=admin_s3_key
+            )
+
+    # create zitadel core key
+    new_key = bitwarden.generate()
+    core_id = bitwarden.create_login(name="zitadel-core-key",
+                                     user="admin-service-account",
+                                     item_url=zitadel_hostname,
+                                     password=new_key)
+
+    # create db credentials password dict
+    db_id = bitwarden.create_login(
+            name="zitadel-db-credentials",
+            user="zitadel",
+            item_url=zitadel_hostname,
+            password="using-tls-now-so-we-do-not-need-a-password"
+            )
+
+    # update the zitadel values for the argocd appset
+    argocd.update_appset_secret(
+            {'zitadel_core_bitwarden_id': core_id,
+             'zitadel_db_bitwarden_id': db_id,
+             'zitadel_s3_postgres_credentials_bitwarden_id': s3_id,
+             'zitadel_s3_admin_credentials_bitwarden_id': s3_admin_id,
+             'zitadel_s3_backups_credentials_bitwarden_id': s3_backup_id}
+            )
+
+    # reload the bitwarden ESO provider
+    try:
+        argocd.k8s.reload_deployment('bitwarden-eso-provider', 'external-secrets')
+    except Exception as e:
+        log.error(
+                "Couldn't scale down the [magenta]bitwarden-eso-provider[/]"
+                "deployment in [green]external-secrets[/] namespace. Recieved: "
+                f"{e}"
+                )
+
+
+def refresh_bitwarden(argocd: ArgoCD,
+                      zitadel_hostname: str,
+                      bitwarden: BwCLI) -> None:
+    """
+    makes sure we update the appset secret with bitwarden IDs regardless
+    """
+    db_id = bitwarden.get_item(
+            f"zitadel-db-credentials-{zitadel_hostname}"
+            )[0]['id']
+
+    s3_backup_id = bitwarden.get_item(
+            f"zitadel-backups-s3-credentials-{zitadel_hostname}", False
+            )[0]['id']
+
+    s3_admin_id = bitwarden.get_item(
+            f"zitadel-admin-s3-credentials-{zitadel_hostname}", False
+            )[0]['id']
+
+    s3_id = bitwarden.get_item(
+            f"zitadel-postgres-s3-credentials-{zitadel_hostname}", False
+            )[0]['id']
+
+    core_id = bitwarden.get_item(
+            f"zitadel-core-key-{zitadel_hostname}", False
+            )[0]['id']
+
+    argo_oidc_item = bitwarden.get_item(
+            f"argocd-oidc-credentials-{argocd.hostname}", False
+            )[0]
+
+    argo_client_id = argo_oidc_item['login']['username']
+
+    # update the zitadel values for the argocd appset
+
+    argocd.update_appset_secret(
+            {
+            'zitadel_core_bitwarden_id': core_id,
+            'zitadel_db_bitwarden_id': db_id,
+            'zitadel_s3_postgres_credentials_bitwarden_id': s3_id,
+            'zitadel_s3_backups_credentials_bitwarden_id': s3_backup_id,
+            'zitadel_s3_admin_credentials_bitwarden_id': s3_admin_id,
+            'argo_cd_oidc_issuer': f"https://{zitadel_hostname}",
+            'argo_cd_oidc_client_id': argo_client_id,
+            'argo_cd_oidc_logout_url': f"https://{zitadel_hostname}/oidc/v1/end_session",
+            'argo_cd_oidc_bitwarden_id': argo_oidc_item['id']
+            }
+            )
+
+
+def restore_zitadel(argocd: ArgoCD,
+                    zitadel_hostname: str,
+                    zitadel_namespace: str,
+                    argo_dict: dict,
+                    secrets: dict,
+                    restore_dict: dict,
+                    backup_dict: dict,
+                    pvc_storage_class: str,
+                    pgsql_cluster_name: str,
+                    bitwarden: BwCLI) -> None:
+    """
+    restore zitadel seaweedfs PVCs, zitadel files and/or config PVC(s),
+    and CNPG postgresql cluster
+    """
+    # this is the info for the REMOTE backups
+    s3_backup_endpoint = backup_dict['endpoint']
+    s3_backup_bucket = backup_dict['bucket']
+    access_key_id = backup_dict["s3_user"]
+    secret_access_key = backup_dict["s3_password"]
+    restic_repo_password = backup_dict['restic_repo_pass']
+    cnpg_backup_schedule = backup_dict['postgres_schedule']
+
+    # first we grab existing bitwarden items if they exist
+    if bitwarden:
+        refresh_bitwarden(argocd, zitadel_hostname, bitwarden)
+
+        # apply the external secrets so we can immediately use them for restores
+        # ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️
+        # WARNING: change this back to main when done testing
+        # ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️
+        ref = "add-pvc-helm-chart-for-zitadel"
+        external_secrets_yaml = (
+                "https://raw.githubusercontent.com/small-hack/argocd-apps/"
+                f"{ref}/zitadel/app_of_apps/external_secrets_argocd_appset.yaml"
+                )
+        argocd.k8s.apply_manifests(external_secrets_yaml, argocd.namespace)
+
+        # postgresql s3 ID
+        s3_db_creds = bitwarden.get_item(
+                f"zitadel-postgres-s3-credentials-{zitadel_hostname}", False
+                )[0]['login']
+
+        pg_access_key_id = s3_db_creds["username"]
+        pg_secret_access_key = s3_db_creds["password"]
+
+    # these are the remote backups for seaweedfs
+    s3_pvc_capacity = secrets['s3_pvc_capacity']
+
+    # then we create all the seaweedfs pvcs we lost and restore them
+    snapshot_ids = restore_dict['restic_snapshot_ids']
+    restore_seaweedfs(
+            argocd.k8s,
+            'zitadel',
+            zitadel_namespace,
+            argocd.namespace,
+            s3_backup_endpoint,
+            s3_backup_bucket,
+            access_key_id,
+            secret_access_key,
+            restic_repo_password,
+            s3_pvc_capacity,
+            pvc_storage_class,
+            "ReadWriteOnce",
+            snapshot_ids['seaweedfs_volume'],
+            snapshot_ids['seaweedfs_master'],
+            snapshot_ids['seaweedfs_filer']
+            )
+
+    # then we finally can restore the postgres database :D
+    if restore_dict.get("cnpg_restore", False):
+        psql_version = restore_dict.get("postgresql_version", 16)
+        s3_endpoint = secrets.get('s3_endpoint', "")
+        restore_cnpg_cluster('zitadel',
+                             zitadel_namespace,
+                             pgsql_cluster_name,
+                             psql_version,
+                             s3_endpoint,
+                             pg_access_key_id,
+                             pg_secret_access_key,
+                             pgsql_cluster_name,
+                             cnpg_backup_schedule)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,27 +161,30 @@
         log.debug(response.text)
 
         json_blob = response.json()
         self.project_id = json_blob['id']
         self.resource_owner = json_blob['details']['resourceOwner']
 
     def create_user(self,
+                    admin_user: str = "",
                     username: str = "",
                     first_name: str = "",
                     last_name: str = "",
                     email: str = "",
                     gender: str = "",
                     bitwarden: BwCLI = None) -> str:
         """
         Creates an initial user in zitadel.
         prompts a user for username, first name, last name, and email if Arguments
         are not passed in
 
         Returns string of user_id.
         """
+        if admin_user:
+            username = admin_user
         if not username:
             username = Prompt.ask("[green]Enter a new username for Zitadel")
         if not first_name:
             first_name = Prompt.ask("[green]Enter your First name for your profile")
         if not last_name:
             last_name = Prompt.ask("[green]Enter your Last name for your profile")
         if not email:
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,40 +18,40 @@
     """
 
     # install chart and wait
     release = Helm.chart(release_name='cert-manager',
                          chart_name='jetstack/cert-manager',
                          namespace='cert-manager',
                          set_options={'installCRDs': 'true'})
-    release.install(True)
+    release.install(wait=True)
 
     if init_dict['enabled']:
         init_values = init_dict['values']
         create_cluster_issuers(init_values, k8s_obj)
 
 
 def create_cluster_issuers(init_values: dict, k8s_obj: K8s = None) -> None:
     """
     create ClusterIssuers for cert manager
     """
     solver = init_values.get('cluster_issuer_acme_challenge_solver', "http01").lower()
-    if solver == "dns01": 
+    if solver == "dns01":
         # create the cloudflare api token secret
         provider = init_values.get("cluster_issuer_acme_dns01_provider", "")
         if provider == "cloudflare":
             token_dict = {"token": init_values['cloudflare_api_token']}
             k8s_obj.create_secret("cloudflare-api-token",
                                   "cert-manager",
                                   token_dict)
             challenge = {"cloudflare": {
                             "apiTokenSecretRef": {
                                 "name": "cloudflare-api-token",
                                 "key": "token"
-                                } 
-                            } 
+                                }
+                            }
                         }
         else:
             log.error("We currently only support cloudflare as the DNS "
                       "provider for the ACME Issuer type in cert-manager. "
                       f"If you'd like to see {provider} supported, please "
                       "submit a PR and we'll take a look!")
     else:
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 #!/usr/bin/env python3.11
 """
        Name: nginx_ingress_controller
 DESCRIPTION: install the nginx ingress controller
      AUTHOR: @jessebot
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
-# external libraries
-import logging as log
-
 # internal libraries
-from smol_k8s_lab.k8s_tools.argocd_util import install_with_argocd, check_if_argocd_app_exists
 from smol_k8s_lab.k8s_tools.helm import Helm
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 
 
 def configure_ingress_nginx(k8s_obj: K8s, k8s_distro: str) -> None:
     """
     install nginx ingress controller from manifests for kind and helm for k3s
@@ -32,18 +28,7 @@
     else:
         values = {"controller.allowSnippetAnnotations": True}
         release = Helm.chart(release_name='ingress-nginx',
                              chart_name='ingress-nginx/ingress-nginx',
                              namespace='ingress-nginx',
                              set_options=values)
         release.install()
-
-
-def install_ingress_nginx_argocd_app(k8s_obj: K8s, ingress_nginx_dict: dict) -> None:
-    """
-    install the ingress nginx Argo CD Application for easier management
-    """
-    if not check_if_argocd_app_exists("ingress-nginx"):
-        log.info("Installing Argo CD Application: ingress-nginx")
-        install_with_argocd(k8s_obj,
-                            "ingress-nginx",
-                            ingress_nginx_dict['argo'])
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,171 +7,174 @@
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 import logging as log
 from rich.prompt import Prompt
 from ..bitwarden.bw_cli import BwCLI
 from ..k8s_tools.helm import prepare_helm
 from ..k8s_tools.k8s_lib import K8s
+from ..k8s_tools.argocd_util import ArgoCD
 from ..utils.rich_cli.console_logging import header
 from .argocd import configure_argocd
-from .ingress.ingress_nginx_controller import (configure_ingress_nginx,
-                                               install_ingress_nginx_argocd_app)
+from .ingress.ingress_nginx_controller import configure_ingress_nginx
 from .ingress.cert_manager import configure_cert_manager
 # from .identity_provider.keycloak import configure_keycloak
 from .identity_provider.zitadel import configure_zitadel
 from .identity_provider.zitadel_api import Zitadel
 from .identity_provider.vouch import configure_vouch
 from .networking.metallb import configure_metallb
 from .networking.cilium import configure_cilium
 from .secrets_management.external_secrets_operator import configure_external_secrets
 from .secrets_management.infisical import configure_infisical
 from .secrets_management.vault import configure_vault
 from .social.matrix import configure_matrix
 from .social.mastodon import configure_mastodon
 from .social.nextcloud import configure_nextcloud
+from .social.home_assistant import configure_home_assistant
 
 
-def setup_k8s_secrets_management(k8s_obj: K8s,
+def setup_k8s_secrets_management(argocd: ArgoCD,
                                  k8s_distro: str,
                                  eso_dict: dict = {},
                                  eso_provider: str = "",
                                  infisical_dict: dict = {},
                                  vault_dict: dict = {},
                                  bitwarden: BwCLI = None) -> None:
     """
     sets up k8s secrets management tooling
     """
     # secrets management section
     header_msg = "Setting up K8s secret management with [green]"
 
     # setup external secrets operator and bitwarden external secrets
-    if eso_dict['enabled']:
+    if eso_dict.get('enabled', False):
         header_msg += f'External Secrets Operator[/] and [blue]{eso_provider}[/] as the Provider'
         header(header_msg, '🤫')
-        configure_external_secrets(k8s_obj,
+        configure_external_secrets(argocd,
                                    eso_dict,
                                    eso_provider,
                                    k8s_distro,
                                    bitwarden)
 
     # setup infisical - an secrets manager and operator for k8s that replaces eso
-    elif infisical_dict['enabled']:
+    elif infisical_dict.get('enabled', False):
         header_msg += 'Infisical Secrets Operator[/]'
         header(header_msg, '🤫')
-        configure_infisical(k8s_obj, infisical_dict)
+        configure_infisical(argocd, infisical_dict)
 
     # setup hashicorp's vault, a secret key management system that works with eso
-    if vault_dict['enabled']:
-        configure_vault(k8s_obj, vault_dict)
+    if vault_dict.get('enabled', False):
+        configure_vault(argocd, vault_dict)
 
 
-def setup_oidc_provider(k8s_obj: K8s,
+def setup_oidc_provider(argocd: ArgoCD,
                         api_tls_verify: bool = False,
                         zitadel_dict: dict = {},
                         vouch_dict: dict = {},
+                        pvc_storage_class: str = "local-path",
                         bw: BwCLI = None,
                         argocd_fqdn: str = "") -> Zitadel | None:
     """
     sets up oidc provider. only zitadel is supported right now
     if we choose to add keycloak back, we'll be adding the following arg
     keycloak_dict: dict = {}
     """
     header("Setting up [green]OIDC[/]/[green]Oauth[/] Applications")
 
     # keycloak_enabled = keycloak_dict['enabled']
-    zitadel_enabled = zitadel_dict['enabled']
+    zitadel_enabled = zitadel_dict.get('enabled', False)
 
     vouch_enabled = False
     if vouch_dict:
-        vouch_enabled = vouch_dict['enabled']
+        vouch_enabled = vouch_dict.get('enabled', False)
 
     # setup keycloak if we're using that for OIDC
     # if keycloak_enabled:
     #     log.debug("Setting up keycloak")
     #     configure_keycloak(k8s_obj, keycloak_dict, bw)
     #     realm = keycloak_dict['argo']['secret_keys']['default_realm']
     #     user = keycloak_dict['init']['values']['username']
 
     # setup zitadel if we're using that for OIDC
     if zitadel_enabled:
-        zitadel_init_enabled = zitadel_dict['init']['enabled']
+        zitadel_init_enabled = zitadel_dict['init'].get('enabled', False)
         log.debug("Setting up zitadel")
         if zitadel_init_enabled:
             zitadel_obj = configure_zitadel(
-                    k8s_obj=k8s_obj,
-                    config_dict=zitadel_dict,
-                    api_tls_verify=api_tls_verify,
-                    argocd_hostname=argocd_fqdn,
+                    argocd,
+                    zitadel_dict,
+                    pvc_storage_class,
+                    api_tls_verify,
                     bitwarden=bw
                     )
         else:
-            configure_zitadel(k8s_obj=k8s_obj,
-                              config_dict=zitadel_dict,
-                              bitwarden=bw)
+            configure_zitadel(argocd, zitadel_dict, bitwarden=bw)
+        zitadel_hostname = zitadel_dict['argo']['secret_keys']['hostname']
 
     if vouch_enabled:
         log.debug("Setting up vouch")
         # if keycloak_enabled:
         #     keycloak_host = keycloak_dict['argo']['secret_keys']['hostname']
         #     configure_vouch(
         #        k8s_obj=k8s_obj,
         #        vouch_config_dict=vouch_dict,
         #        oidc_provider_name='keycloak',
         #        oidc_provider_hostname=keycloak_host,
         #        bitwarden=bw,
         #        users=[{'user': user}],
         #        realm=realm)
         if zitadel_enabled:
-            configure_vouch(k8s_obj=k8s_obj,
-                            vouch_config_dict=vouch_dict,
-                            oidc_provider_name='zitadel',
-                            oidc_provider_hostname=zitadel_dict['argo']['secret_keys']['hostname'],
+            configure_vouch(argocd=argocd,
+                            cfg=vouch_dict,
+                            oidc_provider_hostname=zitadel_hostname,
                             bitwarden=bw,
-                            users=[],
-                            realm="",
                             zitadel=zitadel_obj)
         else:
-            configure_vouch(k8s_obj, vouch_dict, '', '', bw)
+            configure_vouch(argocd, vouch_dict, '', '', bw)
 
     if zitadel_enabled and zitadel_init_enabled:
         return zitadel_obj
 
 
 def setup_base_apps(k8s_obj: K8s,
                     k8s_distro: str,
                     cilium_dict: dict = {},
                     metallb_dict: dict = {},
                     ingress_dict: dict = {},
                     cert_manager_dict: dict = {},
-                    argo_enabled: bool = False,
-                    argo_secrets_plugin_enabled: bool = False,
+                    cnpg_operator_dict: dict = {},
+                    argocd_dict: dict = {},
                     plugin_secrets: dict = {},
-                    bw: BwCLI = None) -> None:
-    """ 
+                    bw: BwCLI = None) -> ArgoCD:
+    """
     Uses Helm to install all base apps that need to be running being argo cd:
         cilium, metallb, ingess-nginx, cert-manager, argo cd, argocd secrets plugin
     All Needed for getting Argo CD up and running.
+
+    Returns an ArgoCD object for further argo actions
     """
-    metallb_enabled = metallb_dict['enabled']
-    cilium_enabled = cilium_dict['enabled']
-    ingress_nginx_enabled = ingress_dict["enabled"]
+    metallb_enabled = metallb_dict.get('enabled', False)
+    cilium_enabled = cilium_dict.get('enabled', False)
+    ingress_nginx_enabled = ingress_dict.get('enabled', False)
+    cnpg_operator_enabled = cnpg_operator_dict.get('enabled', False)
+    argocd_enabled = argocd_dict.get('enabled', False)
+    argo_secrets_plugin_enabled = argocd_dict['argo']['directory_recursion']
     # make sure helm is installed and the repos are up to date
-    prepare_helm(k8s_distro, argo_enabled, metallb_enabled, cilium_enabled,
-                 argo_secrets_plugin_enabled)
+    prepare_helm(k8s_distro, metallb_enabled, cilium_enabled, cnpg_operator_enabled,
+                 argocd_enabled, argo_secrets_plugin_enabled)
 
     # needed for network policy editor and hubble UI
     if cilium_enabled:
         header("Installing [green]cilium[/green] so we have networking tools",
                '🛜')
         if cilium_dict['init']['enabled']:
             configure_cilium(cilium_dict)
 
     # needed for metal (non-cloud provider) installs
     if metallb_enabled:
-        header("Installing [green]metallb[/green] so we have an IP address pool",
+        header("Installing [green]metallb[/green] so we have an IP address pool.",
                '🛜')
         if metallb_dict['init']['enabled']:
             cidr = metallb_dict['init']['values']['address_pool']
             if not cidr:
                 m = "[green]Please enter a comma seperated list of IPs or CIDRs"
                 cidr = Prompt.ask(m).split(',')
 
@@ -182,40 +185,49 @@
         # nginx just because that's most supported, treafik support may be added later
         header("Installing [green]ingress-nginx-controller[/green] to access web"
                " apps outside the cluster", "🌐")
         configure_ingress_nginx(k8s_obj, k8s_distro)
 
     # manager SSL/TLS certificates via lets-encrypt
     header("Installing [green]cert-manager[/green] for TLS certificates...", '📜')
-    if cert_manager_dict["enabled"]:
+    if cert_manager_dict.get('enabled', False):
         configure_cert_manager(k8s_obj, cert_manager_dict['init'])
 
     # then we install argo cd if it's enabled
-    if argo_enabled:
-        configure_argocd(k8s_obj,
-                         bw, 
-                         argo_secrets_plugin_enabled,
-                         plugin_secrets)
+    if argocd_enabled:
+        argocd = configure_argocd(k8s_obj,
+                                  argocd_dict,
+                                  plugin_secrets,
+                                  bw)
+
+        if ingress_nginx_enabled:
+            argocd.install_app("ingress-nginx", ingress_dict['argo'])
 
-    if ingress_nginx_enabled and argo_enabled:
-        install_ingress_nginx_argocd_app(k8s_obj, ingress_dict)
+        return argocd
 
 
-def setup_federated_apps(k8s_obj: K8s,
+def setup_federated_apps(argocd: ArgoCD,
                          api_tls_verify: bool = False,
+                         home_assistant_dict: dict = {},
                          nextcloud_dict: dict = {},
                          mastodon_dict: dict = {},
                          matrix_dict: dict = {},
+                         pvc_storage_class: str = "local-path",
                          zitadel_hostname: str = "",
                          zitadel_obj: Zitadel = None,
                          bw: BwCLI = None) -> None:
     """
     Setup any federated apps with initialization supported
     """
-    if nextcloud_dict['enabled']:
-        configure_nextcloud(k8s_obj, nextcloud_dict, bw, zitadel_obj)
+    if home_assistant_dict.get('enabled', False):
+        configure_home_assistant(argocd, home_assistant_dict, pvc_storage_class,
+                                 api_tls_verify, bw)
+
+    if nextcloud_dict.get('enabled', False):
+        configure_nextcloud(argocd, nextcloud_dict, pvc_storage_class,
+                            zitadel_obj, bw)
 
-    if mastodon_dict['enabled']:
-        configure_mastodon(k8s_obj, mastodon_dict, bw)
+    if mastodon_dict.get('enabled', False):
+        configure_mastodon(argocd, mastodon_dict, pvc_storage_class, bw)
 
-    if matrix_dict['enabled']:
-        configure_matrix(k8s_obj, matrix_dict, zitadel_obj, bw)
+    if matrix_dict.get('enabled', False):
+        configure_matrix(argocd, matrix_dict, pvc_storage_class, zitadel_obj, bw)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
         yaml.dump(values, values_file)
 
     # install chart and wait
     release = Helm.chart(release_name='cilium',
                          chart_name='cilium/cilium',
                          namespace='cilium',
                          values_file=values_file_name)
-    release.install(True)
+    release.install(wait=True)
 
     return True
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import logging as log
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
 from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                check_if_argocd_app_exists,
-                                                update_argocd_appset_secret)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.rich_cli.console_logging import header
 from smol_k8s_lab.utils.passwords import create_password
 
 
-def configure_netmaker(k8s_obj: K8s,
+def configure_netmaker(argocd: ArgoCD,
                        netmaker_config_dict: dict,
                        oidc_provider_name: str = "",
                        oidc_provider_hostname: str = "",
                        bitwarden: BwCLI = None,
                        zitadel: Zitadel = None) -> None:
     """
     Installs netmaker as an Argo CD application on Kubernetes
 
     Required Args:
-      k8s_obj:                K8s(), for the authenticated k8s client
-      netmaker_config_dict:      Argo CD parameters
+      argocd:                 ArgoCD(), for the argocd operations
+      netmaker_config_dict:   Argo CD parameters
 
     Optional Args:
       oidc_provider_name:     OIDC provider name. options: keycloak, zitadel
       oidc_provider_hostname: OIDC provider hostname e.g. zitadel.example.com
       bitwarden:              BwCLI, to store k8s secrets in bitwarden
-      zitadel:                Zitadel api object 
+      zitadel:                Zitadel api object
     """
     header("Setting up [green]Netmaker[/] to create VPNs", "🗝️")
 
     # make sure netmaker isn't already installed
-    app_installed = check_if_argocd_app_exists("netmaker")
+    app_installed = argocd.check_if_app_exists("netmaker")
     # this handles the netmaker-oauth-config secret data
     secrets = netmaker_config_dict['argo']['secret_keys']
     if secrets:
         netmaker_hostname = secrets['hostname']
         netmaker_dashboard_hostname = secrets['admin_hostname']
         netmaker_api_hostname = secrets['api_hostname']
 
@@ -59,22 +56,22 @@
         netmaker_master_key = create_password()
 
         # if using bitwarden, put the secret in bitarden and ESO will grab it
         if bitwarden:
             fields = [create_custom_field("issuer", f"https://{oidc_provider_hostname}")]
 
             log.debug(f"netmaker oauth fields are {fields}")
-            
+
             postgres_fields = [
                 create_custom_field("host", 'postgresql.svc.cluster.local'),
                 create_custom_field("port", '5432'),
                 create_custom_field("database", 'netmaker'),
                 create_custom_field("postgres_password", postgresPassword),
                 ]
-            
+
             log.info(f"netmaker postgres fields are {postgres_fields}")
 
             # create netmaker super admin credentials bitwarden item
             admin_id = bitwarden.create_login(
                 name=f'{netmaker_hostname}-netmaker-admin-credentials',
                 user=netmaker_user,
                 password=netmaker_pass,
@@ -93,79 +90,79 @@
 
             # create the mqtt bitwarden item
             mq_id = bitwarden.create_login(
                     name=f"{netmaker_hostname}-netmaker-mq-credentials",
                     user='netmaker',
                     password=mqPass
                     )
-            
+
             # create the postgres bitwarden item
             postgres_id = bitwarden.create_login(
                     name=f"{netmaker_hostname}-netmaker-pgsql-credentials",
                     user='netmaker',
                     password=sqlPass,
                     fields=postgres_fields
                     )
 
             # update the netmaker values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'netmaker_oauth_config_bitwarden_id': oauth_id,
                      'netmaker_admin_credentials_bitwarden_id': admin_id,
                      'netmaker_mq_config_bitwarden_id': mq_id,
                      'netmaker_pgsql_config_bitwarden_id': postgres_id})
 
             # reload the bitwarden ESO provider
             try:
-                k8s_obj.reload_deployment('bitwarden-eso-provider', 'external-secrets')
+                argocd.k8s.reload_deployment('bitwarden-eso-provider',
+                                             'external-secrets')
             except Exception as e:
                 log.error(
                         "Couldn't scale down the [magenta]bitwarden-eso-provider[/]"
                         "deployment in [green]external-secrets[/] namespace. Recieved: "
                         f"{e}"
                         )
 
         # create netmaker k8s secrets if we're not using bitwarden
         else:
             # create oauth OIDC k8s secret
-            k8s_obj.create_secret('netmaker-admin-credentials',
-                                  'netmaker',
-                                  {'ADMIN_USER': netmaker_user,
-                                   'ADMIN_PASSWORD': netmaker_pass,
-                                   'MASTER_KEY': netmaker_master_key}
-                                   )
+            argocd.k8s.create_secret('netmaker-admin-credentials',
+                                     'netmaker',
+                                     {'ADMIN_USER': netmaker_user,
+                                      'ADMIN_PASSWORD': netmaker_pass,
+                                      'MASTER_KEY': netmaker_master_key}
+                                      )
 
             # create oauth OIDC k8s secret
-            k8s_obj.create_secret('netmaker-oauth-config',
-                                  'netmaker',
-                                  {'CLIENT_ID': auth_dict['client_id'],
-                                   'CLIENT_SECRET': auth_dict['client_secret'],
-                                   'OIDC_SSUER': f"https://{oidc_provider_hostname}"}
-                                   )
+            argocd.k8s.create_secret('netmaker-oauth-config',
+                                     'netmaker',
+                                     {'CLIENT_ID': auth_dict['client_id'],
+                                      'CLIENT_SECRET': auth_dict['client_secret'],
+                                      'OIDC_SSUER': f"https://{oidc_provider_hostname}"}
+                                      )
 
             # create mqtt k8s secret
-            k8s_obj.create_secret('netmaker-mq-credentials',
-                                  'netmaker',
-                                  {'MQ_PASSWORD': mqPass,
-                                   'MQ_USERNAME': 'netmaker'}
-                                   )
+            argocd.k8s.create_secret('netmaker-mq-credentials',
+                                     'netmaker',
+                                     {'MQ_PASSWORD': mqPass,
+                                      'MQ_USERNAME': 'netmaker'}
+                                      )
 
             # create postgres k8s secret
-            k8s_obj.create_secret('netmaker-pgsql-credentials',
-                                  'netmaker',
-                                  {'postgres_password': postgresPassword,
-                                   'SQL_HOST': 'posgresql.svc.cluster.local',
-                                   'SQL_PORT': '5432',
-                                   'SQL_DB': 'netmaker',
-                                   'SQL_USER': 'netmaker',
-                                   'SQL_PASS': sqlPass}
-                                   )
+            argocd.k8s.create_secret('netmaker-pgsql-credentials',
+                                     'netmaker',
+                                     {'postgres_password': postgresPassword,
+                                      'SQL_HOST': 'posgresql.svc.cluster.local',
+                                      'SQL_PORT': '5432',
+                                      'SQL_DB': 'netmaker',
+                                      'SQL_USER': 'netmaker',
+                                      'SQL_PASS': sqlPass}
+                                      )
 
     if not app_installed:
-        install_with_argocd(k8s_obj, 'netmaker', netmaker_config_dict['argo'])
+        argocd.install_app('netmaker', netmaker_config_dict['argo'])
     else:
         log.info("netmaker already installed 🎉")
 
         # we need to still update the bitwarden IDs if bitwarden and init is enabled
         if netmaker_config_dict['init']['enabled'] and bitwarden:
             log.debug("Updating netmaker-admin-credentials bitwarden ID in the appset secret")
             admin_id = bitwarden.get_item(
@@ -183,16 +180,15 @@
                     )[0]['id']
 
             mq_id = bitwarden.get_item(
                     f"{netmaker_hostname}-netmaker-mq-credentials", False
                     )[0]['id']
 
             # update the netmaker values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'netmaker_oauth_config_bitwarden_id': oauth_id,
                      'netmaker_admin_credentials_bitwarden_id': admin_id,
                      'netmaker_mq_config_bitwarden_id': mq_id,
                      'netmaker_pgsql_config_bitwarden_id': postgres_id})
 
 def create_netmaker_app(provider: str,
                      provider_hostname: str,
@@ -204,24 +200,24 @@
     Creates an OIDC application, for netmaker, in either Keycloak or Zitadel
 
     Arguments:
       provider           - either 'keycloak' or 'zitadel'
       provider_hostname  - hostname of keycloak or zitadel
       dashboard_hostname - hostname of netmaker admina dashboard
       api_hostname       - hostname of netmaker api endpoint
-      zitadel            - Zitadel api object 
+      zitadel            - Zitadel api object
       realm              - realm to use for keycloak if using keycloak
 
     returns [url, client_id, client_secret]
     """
     # create Netmaker OIDC Application
     if provider == 'zitadel':
         log.info("Creating an OIDC application for Netmaker via Zitadel...")
         netmaker_dict = zitadel.create_application(
-                "netmaker", 
+                "netmaker",
                 f"https://{api_hostname}/api/oauth/callback",
                 [f"https://{dashboard_hostname}"]
                 )
         zitadel.create_role("netmaker_users", "Netmaker Users", "netmaker_users")
         zitadel.update_user_grant(['netmaker_users'])
 
         client_id = netmaker_dict['client_id']
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.rich_cli.console_logging import header
-from .longhorn import configure_longhorn
-from .k8up_operater import configure_k8up_operator
-from .minio import configure_minio_operator
-from .postgres_operators import configure_cnpg_operator, configure_postgres_operator
-from .prometheus import configure_prometheus_crds
+from .postgres_operators import configure_postgres_operator
 from .seaweedfs import configure_seaweedfs
 
 
-def setup_operators(k8s_obj: K8s,
+def setup_operators(argocd: ArgoCD,
                     prometheus_config: dict = {},
                     longhorn_config: dict = {},
                     k8up_config: dict = {},
                     minio_config: dict = {},
                     seaweed_config: dict = {},
                     cnpg_config: dict = {},
                     pg_config: dict = {},
@@ -28,32 +24,32 @@
         - cnpg (cloud native postgres) operator
         - zalando postgres operator
     """
     header("Setting up Operators", "⚙️ ")
 
     # deploy the prometheus CRDs before everything else so that apps with metrics don't fail
     if prometheus_config and prometheus_config.get('enabled', False):
-        configure_prometheus_crds(k8s_obj, prometheus_config)
+        argocd.install_app('prometheus-crds', prometheus_config['argo'])
 
     # longhorn operator is used to have expanding volumes that span multiple nodes
     if longhorn_config and longhorn_config.get('enabled', False):
-        configure_longhorn(k8s_obj, longhorn_config)
+        argocd.install_app('longhorn', longhorn_config['argo'])
 
     # k8up operator is a postgres operator for creating postgresql clusters
     if k8up_config and k8up_config.get('enabled', False):
-        configure_k8up_operator(k8s_obj, k8up_config)
+        argocd.install_app('k8up', k8up_config['argo'])
 
     # minio operator is used to spin up minio tenants for isolated s3 endpoints
     if minio_config and minio_config.get('enabled', False):
-        configure_minio_operator(k8s_obj, minio_config)
+        argocd.install_app('minio', minio_config['argo'], True)
 
     # seaweedfs
     if seaweed_config and seaweed_config.get('enabled', False):
-        configure_seaweedfs(k8s_obj, seaweed_config, bitwarden)
+        configure_seaweedfs(argocd, seaweed_config, bitwarden)
 
     # cnpg operator is a postgres operator for creating postgresql clusters
     if cnpg_config and cnpg_config.get('enabled', False):
-        configure_cnpg_operator(k8s_obj, cnpg_config)
+        argocd.install_app('cnpng-operator', cnpg_config['argo'])
 
     # zalando postgres operator is a postgres operator for creating postgresql clusters
     if pg_config and pg_config.get('enabled', False):
-        configure_postgres_operator(k8s_obj, pg_config, bitwarden)
+        configure_postgres_operator(argocd, pg_config, bitwarden)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/minio_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from minio import Minio, MinioAdmin
 from minio.credentials.providers import MinioClientConfigProvider
 from shutil import which
 
 from smol_k8s_lab.constants import HOME_DIR, XDG_CACHE_DIR
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
 from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
-from smol_k8s_lab.k8s_tools.argocd_util import (
-        install_with_argocd, wait_for_argocd_app, check_if_argocd_app_exists)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.passwords import create_password
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.utils.run.subproc import subproc
 
 
 class BetterMinio:
-    """ 
+    """
     a wrapper around the two seperate Minio and MinioAdmin clients to create
     users and buckets with basic policies
     """
 
     def __init__(self,
                  minio_alias: str,
                  api_hostname: str,
@@ -32,14 +30,37 @@
         minio_config_dir = join(HOME_DIR, ".mc/")
         minio_config_file = join(minio_config_dir, "config.json")
         log.debug(f"Checking for config file in {minio_config_file}")
         minio_provider = MinioClientConfigProvider(minio_config_file, minio_alias)
         self.admin_client = MinioAdmin(api_hostname, minio_provider)
         self.client = Minio(api_hostname, access_key, secret_key)
 
+    def get_object(self, bucket: str, s3_object: str, save_file: str = ""):
+        """
+        get an s3_object from an s3 endpoint
+        """
+        if not save_file:
+            file_name = s3_object.split("/")[-1]
+            save_file = join(XDG_CACHE_DIR, f"smol-k8s-lab/{file_name}")
+
+        return self.client.fget_object(bucket, s3_object, save_file)
+
+    def list_object(self,
+                    bucket: str,
+                    s3_object_path: str = "",
+                    recursive: bool = False):
+        """
+        list an s3_object dir from an s3 endpoint
+        """
+        obj_args = {"bucket_name": bucket,
+                    "prefix": s3_object_path,
+                    "recursive": recursive}
+
+        return self.client.list_objects(**obj_args)
+
     def create_access_credentials(self, access_key: str) -> str:
         """
         given an access key name, we create minio access credentials
         using the mc admin client
         return secret_key
         """
         if which("brew") and not which("mc"):
@@ -175,15 +196,15 @@
             dump(policy, policy_file)
 
         # actually create the policy
         self.admin_client.policy_add('minio_read_users', policy_file_name)
         log.info("Created minio_read only user policy for use with OIDC")
 
     def set_anonymous_download(self, bucket: str, prefix: str) -> None:
-        """ 
+        """
         sets anonymous download on a particular bucket and folder
         """
         policy = {
             "Version": "2012-10-17",
             "Statement": [
                 {
                     "Effect": "Allow",
@@ -208,15 +229,15 @@
                 },
             ],
         }
 
         self.client.set_bucket_policy(bucket, dumps(policy))
 
 
-def configure_minio_tenant(k8s_obj: K8s,
+def configure_minio_tenant(argocd: ArgoCD,
                            minio_config: dict,
                            secure: bool = True,
                            zitadel_hostname: str = "",
                            zitadel: Zitadel = None,
                            bitwarden: BwCLI = None) -> BetterMinio | None:
     """
     minio tenant installation and configuration
@@ -232,15 +253,15 @@
 
     if init is enabled we:
       - write a minio config file with alias called minio-root for use with mc cli
       - return a BetterMinio object ready to create users, buckets, and policies
     """
 
     minio_init_enabled = minio_config['init']['enabled']
-    argo_app_exists = check_if_argocd_app_exists('minio-tenant')
+    argo_app_exists = argocd.check_if_app_exists('minio-tenant')
 
     secrets = minio_config['argo']['secret_keys']
     if secrets:
         minio_hostname = secrets.get('api_hostname', "")
         minio_user_console_hostname = secrets.get('user_console_hostname', "")
 
     # if the app already exists and bitwarden is enabled return the credentials
@@ -253,15 +274,15 @@
             return BetterMinio('minio-root', minio_hostname, access_key, secret_key)
         # if app already exists but bitwarden is not enabled, return None
         return
 
     # if the user has enabled smol_k8s_lab init, we create an initial user
     if minio_init_enabled and not argo_app_exists:
         # the namespace probably doesn't exist yet, so we try to create it
-        k8s_obj.create_namespace(minio_config['argo']['namespace'])
+        argocd.k8s.create_namespace(minio_config['argo']['namespace'])
         access_key = minio_config['init']['values']['root_user']
         secret_key = create_password(characters=72)
 
         if zitadel:
             log.info("Creating a MinIO OIDC application via Zitadel...")
             redirect_uris = f"https://{minio_user_console_hostname}/oauth_callback"
             logout_uris = [f"https://{minio_user_console_hostname}/login"]
@@ -287,45 +308,40 @@
                                    """}
         else:
             # creates the initial root credentials secret for the minio tenant
             credentials_exports = {
                     'config.env': f"""MINIO_ROOT_USER={access_key}
             MINIO_ROOT_PASSWORD={secret_key}"""}
 
-        k8s_obj.create_secret('default-tenant-env-config', 'minio',
-                              credentials_exports)
+        argocd.k8s.create_secret('default-tenant-env-config', 'minio',
+                                 credentials_exports)
 
         if bitwarden:
             log.info("Creating MinIO root credentials in Bitwarden")
             # admin credentials + metrics server info token
             bitwarden.create_login(
                     name='minio-tenant-root-credentials',
                     item_url=minio_hostname,
                     user=access_key,
                     password=secret_key
                     )
 
     if not argo_app_exists:
         # actual installation of the minio tenant Argo CD Application
-        install_with_argocd(k8s_obj,
-                            'minio-tenant',
-                            minio_config['argo'])
+        argocd.install_app('minio-tenant', minio_config['argo'], True)
 
 
         # while we wait for the app to come up, update the config file
         if minio_init_enabled:
             create_minio_alias("minio-root",
                                minio_hostname,
                                access_key,
                                secret_key,
                                secure)
 
-        # make sure the app is up before returning
-        wait_for_argocd_app('minio-tenant')
-
         if minio_init_enabled:
             # immediately create an admin and readonly policy
             minio_obj = BetterMinio('minio-root', minio_hostname,
                                     access_key, secret_key)
             # so that zitadel groups names match up with minio policy names
             minio_obj.create_admin_group_policy()
             minio_obj.create_read_user_group_policy()
@@ -342,27 +358,14 @@
 
             return BetterMinio('minio-root',
                                minio_hostname,
                                access_key,
                                secret_key)
 
 
-def configure_minio_operator(k8s_obj: K8s, minio_config: dict) -> None:
-    """
-    setup the MinIO operator as an Argo CD Application
-    """
-    # check if minio is using smol_k8s_lab init and if already present in Argo CD
-    if not check_if_argocd_app_exists('minio'):
-        # actual installation of the minio app
-        install_with_argocd(k8s_obj,
-                            'minio',
-                            minio_config['argo'])
-        wait_for_argocd_app('minio')
-
-
 def create_minio_alias(minio_alias: str,
                        minio_hostname: str,
                        access_key: str,
                        secret_key: str,
                        secure: bool = True) -> None:
     """
     add minio alias for credentials to your local /home/.mc/config.json file
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 # internal libraries
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                update_argocd_appset_secret,
-                                                sync_argocd_app,
-                                                check_if_argocd_app_exists)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.passwords import create_password
 
 # external libraries
 import logging as log
 
 
-def configure_cnpg_operator(k8s_obj: K8s, config: dict) -> None:
-    """
-    setup the CNPG operator as an Argo CD Application
-    """
-    # check if minio is using smol_k8s_lab init and if already present in Argo CD
-    if not check_if_argocd_app_exists('cnpg-operator'):
-        # actual installation of the minio app
-        install_with_argocd(k8s_obj,
-                            'cnpg-operator',
-                            config['argo'])
-
-
-def configure_postgres_operator(k8s_obj: K8s,
+def configure_postgres_operator(argocd: ArgoCD,
                                 config: dict,
                                 bw: BwCLI = None) -> None:
     """
     setup the zalando postgres operator as an Argo CD Application
     """
     # get hostname and if init is enabled
     init_enabled = config['init']['enabled']
     hostname = config['argo']['secret_keys']['hostname']
 
     # check if minio is using smol_k8s_lab init and if already present in Argo CD
-    if not check_if_argocd_app_exists('postgres-operator'):
+    if not argocd.check_if_app_exists('postgres-operator'):
         if init_enabled:
             access_id = config['init']['values']['s3_backup_access_id']
             secret_key = config['init']['values']['s3_backup_secret_key']
             if bw:
                 # s3 credentials for zalando postgres operator access
                 pgsql_s3_pass = create_password()
                 s3_id = bw.create_login(
@@ -62,25 +46,22 @@
                         name='postgres-operator-backups-s3-credentials',
                         item_url=hostname,
                         user=access_id,
                         password=secret_key
                         )
 
                 # update the postgres_operator values for the argocd appset
-                update_argocd_appset_secret(
-                        k8s_obj,
+                argocd.update_appset_secret(
                         {'postgres_operator_s3_admin_credentials_bitwarden_id': s3_admin_id,
                          'postgres_operator_s3_user_credentials_bitwarden_id': s3_id,
                          'postgres_operator_s3_backups_credentials_bitwarden_id': s3_backups_id}
                         )
 
         # actual installation of the minio app
-        install_with_argocd(k8s_obj,
-                            'postgres-operator',
-                            config['argo'])
+        argocd.install_app('postgres-operator', config['argo'])
     else:
         if bw and init_enabled:
             log.debug("Making sure postgres_operator Bitwarden item IDs are in "
                       "appset secret plugin secret")
 
             s3_admin_id = bw.get_item(
                     f"postgres-operator-admin-s3-credentials-{hostname}"
@@ -90,15 +71,14 @@
                     f"postgres-operator-user-s3-credentials-{hostname}", False
                     )[0]['id']
 
             s3_backups_id = bw.get_item(
                     f"postgres-operator-backups-s3-credentials-{hostname}", False
                     )[0]['id']
 
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'postgres_operator_s3_admin_credentials_bitwarden_id': s3_admin_id,
                      'postgres_operator_s3_user_credentials_bitwarden_id': s3_id,
                      'postgres_operator_s3_backups_credentials_bitwarden_id': s3_backups_id
                     })
 
-        sync_argocd_app('postgres-operator')
+        argocd.sync_app('postgres-operator')
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import logging as log
 
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
 from smol_k8s_lab.k8s_apps.operators.minio import create_minio_alias
-from smol_k8s_lab.k8s_tools.argocd_util import (
-        install_with_argocd, 
-        wait_for_argocd_app, 
-        check_if_argocd_app_exists, 
-        update_argocd_appset_secret)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.passwords import create_password
 
 
-def configure_seaweedfs(k8s_obj: K8s,
+def configure_seaweedfs(argocd: ArgoCD,
                         seaweedfs_config: dict,
                         bitwarden: BwCLI = None) -> None:
     """
     seaweedfs tenant installation and configuration
 
     if secure is set to True, we write a config with https:// prefixing the
     hostname, else we use http://
@@ -24,16 +19,17 @@
         We'll store all your secrets in bitwarden
 
     if init is enabled we:
       - write a seaweedfs config file with alias called seaweedfs-root for use with mc cli
       - return a Betterseaweedfs object ready to create users, buckets, and policies
     """
 
+    k8s_obj = argocd.k8s
     seaweedfs_init_enabled = seaweedfs_config['init']['enabled']
-    argo_app_exists = check_if_argocd_app_exists('seaweedfs')
+    argo_app_exists = argocd.check_if_app_exists('seaweedfs')
 
     secrets = seaweedfs_config['argo']['secret_keys']
     if secrets:
         seaweedfs_hostname = secrets.get('s3_endpoint', "")
 
     # if the app already exists and bitwarden is enabled return the credentials
     if seaweedfs_init_enabled and argo_app_exists:
@@ -58,34 +54,30 @@
             s3_id = bitwarden.create_login(
                     name='seaweedfs-admin-credentials',
                     item_url=seaweedfs_hostname,
                     user=access_key,
                     password=secret_key
                     )
             # update the nextcloud values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'seaweedfs_s3_credentials_bitwarden_id': s3_id}
                     )
 
     if not argo_app_exists:
         # actual installation of the seaweedfs tenant Argo CD Application
-        install_with_argocd(k8s_obj, 'seaweedfs', seaweedfs_config['argo'])
+        argocd.install_app('seaweedfs', seaweedfs_config['argo'], True)
 
 
         # while we wait for the app to come up, update the config file
         if seaweedfs_init_enabled:
             create_minio_alias("seaweedfs-root",
                                seaweedfs_hostname,
                                access_key,
                                secret_key)
 
-        # make sure the app is up before returning
-        wait_for_argocd_app('seaweedfs')
-
         # if seaweedfs_init_enabled:
         #     # immediately create an admin and readonly policy
         #     seaweedfs_obj = BetterMinio('seaweedfs-root', seaweedfs_hostname,
         #                             access_key, secret_key)
         #     # so that zitadel groups names match up with seaweedfs policy names
         #     seaweedfs_obj.create_admin_group_policy()
         #     seaweedfs_obj.create_read_user_group_policy()
@@ -93,16 +85,15 @@
         # if the seaweedfs tenant Argo CD app already exists, but init is enabed...
         if bitwarden:
             creds = bitwarden.get_item(
                     f'seaweedfs-admin-credentials-{seaweedfs_hostname}'
                     )[0]
 
             # update the nextcloud values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
+            argocd.update_appset_secret(
                     {'seaweedfs_s3_credentials_bitwarden_id': creds['id']}
                     )
 
         # if seaweedfs_init_enabled:
         #     access_key = creds['login']['username']
         #     secret_key = creds['login']['password']
         #     return BetterMinio('seaweedfs-root',
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,43 +3,45 @@
        Name: external_secrets
 DESCRIPTION: configures external secrets, currently only with Bitwarden and GitLab
              hopefully with more supported providers in the future
      AUTHOR: @jessebot
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI
-from smol_k8s_lab.k8s_tools.argocd_util import install_with_argocd, wait_for_argocd_app
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.utils.run.subproc import subproc
 
 
-def configure_external_secrets(k8s_obj: K8s,
+def configure_external_secrets(argocd: ArgoCD,
                                eso_dict: dict,
                                eso_provider: str = "",
                                distro: str = "",
                                bitwarden: BwCLI = None) -> None:
     """
     configure external secrets and provider. (and optionally bweso or gitlab)
     """
-    k8s_obj.create_namespace("external-secrets")
+    argocd.k8s.create_namespace("external-secrets")
 
     if eso_provider == "bitwarden":
-        setup_bweso_provider(k8s_obj, distro, bitwarden)
+        setup_bweso_provider(argocd.k8s, distro, bitwarden)
     elif eso_provider == "gitlab":
-        setup_gitlab_provider(k8s_obj, eso_dict['init']['values']['gitlab_access_token'])
+        setup_gitlab_provider(argocd.k8s,
+                              eso_dict['init']['values']['gitlab_access_token'])
 
-    install_with_argocd(k8s_obj, 'external-secrets-operator', eso_dict['argo'])
-    wait_for_argocd_app('external-secrets-operator')
+    argocd.install_app('external-secrets-operator', eso_dict['argo'], True)
 
     if bitwarden:
         # wait for bitwarden external secrets provider to be up
-        wait_for_argocd_app('bitwarden-eso-provider', retry=True)
+        argocd.wait_for_app('bitwarden-eso-provider', retry=True)
 
 
-def setup_bweso_provider(k8s_obj: K8s, distro: str, bitwarden: BwCLI = None) -> None:
+def setup_bweso_provider(k8s_obj: K8s,
+                         distro: str,
+                         bitwarden: BwCLI = None) -> None:
     """
     Creates an initial secret for use with the bitwarden provider for ESO
     """
     # this is a standard k8s secrets yaml
     k8s_obj.create_secret('bweso-login',
                           'external-secrets',
                           {"BW_PASSWORD": bitwarden.password,
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,40 +5,38 @@
      AUTHOR: @jessebot
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version python3
              Infisical itself is licensed under Apache 2.0 and we at
              smol-k8s-lab do not claim any of their code
 """
 from rich.prompt import Prompt
 from random import randbytes
-from smol_k8s_lab.k8s_tools.argocd_util import install_with_argocd
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 from smol_k8s_lab.utils.passwords import create_password
-from smol_k8s_lab.utils.rich_cli.console_logging import header
 
 
-def configure_infisical(k8s_obj: K8s, infisical_dict: dict):
+def configure_infisical(argocd: ArgoCD, infisical_dict: dict):
     """
     - configures the infisical app by asking for smtp credentials
     - configures backendEnvironmentVariables secrets to sign JWT tokens
     """
-    header("Installing the Infisical app and Secrets operator...")
-    k8s_obj.create_namespace('infisical')
+    k8s_obj = argocd.k8s
+    argocd.k8s.create_namespace('infisical')
 
     argo_dict = infisical_dict['argo']
 
     if infisical_dict['init']:
         if not k8s_obj.get_secret('infisical-mongo-credentials', 'infisical'):
             mongo_password = create_mongo_secrets(k8s_obj)
         if not k8s_obj.get_secret('infisical-backend-secrets', 'infisical'):
             create_backend_secret(k8s_obj,
                                   mongo_password,
                                   argo_dict['secret_keys']['hostname'])
 
-    install_with_argocd(k8s_obj, 'infisical', argo_dict)
-    return True
+    argocd.install_app(k8s_obj, 'infisical', argo_dict)
 
 
 def create_backend_secret(k8s_obj: K8s,
                           mongo_password: str = "",
                           hostname: str = ""):
     """
     generates an smtp dict for env vars AND 16-bytes hex value, 32-characters hex:
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,61 +6,57 @@
     LICENSE: The setup script is licensed under:
                GNU AFFERO GENERAL PUBLIC LICENSE Version 3 and higher
 
              Hashicorp Vault has a custom license that you can view at their repo:
                  https://github.com/hashicorp/vault/blob/main/LICENSE
 
              smol-k8s-lab do not claim any of Vault as our own and we do not
-             provide any paid support for Vault. If support is needed for the 
-             Vault components of smol-k8s-lab, it must be done unpaid via the 
-             smol-k8s-lab community or via an official enterprise contract from 
+             provide any paid support for Vault. If support is needed for the
+             Vault components of smol-k8s-lab, it must be done unpaid via the
+             smol-k8s-lab community or via an official enterprise contract from
              official Hashicorp channels.
 """
 
 # internal libraries
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                check_if_argocd_app_exists,
-                                                wait_for_argocd_app)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.utils.rich_cli.console_logging import header
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.utils.run.subproc import subproc
 
 # external libraries
 import logging as log
 from time import sleep
 
 
-def configure_vault(k8s_obj: K8s, vault_dict: dict, bitwarden: BwCLI = None) -> None:
+def configure_vault(argocd: ArgoCD,
+                    vault_dict: dict,
+                    bitwarden: BwCLI = None) -> None:
     """
     configures the hashicorp vault helm chart
     """
-    # check immediately if this app is installed
-    app_installed = check_if_argocd_app_exists('vault')
+    argo_dict = vault_dict['argo']
 
     header("Installing the Hashicorp Vault app...", "🔑")
-    argo_dict = vault_dict['argo']
+    installed_app = argocd.install_app('vault', argo_dict, True)
 
     # get any secret keys passed in
     secrets = vault_dict['argo']['secret_keys']
     if secrets:
         vault_cluster_name = secrets['cluster_name']
 
-    if not app_installed:
-        install_with_argocd(k8s_obj, 'vault', argo_dict)
-        wait_for_argocd_app('vault')
-
     init_dict = vault_dict['init']
-    if not app_installed and init_dict['enabled']:
+    if init_dict['enabled'] and not installed_app:
         log.info("Vault init enabled. We'll proceed with the unsealing process")
-        initialize_vault(argo_dict['namespace'], bitwarden, vault_cluster_name)
+        initialize_vault(argo_dict['namespace'], vault_cluster_name, bitwarden)
 
 
-def initialize_vault(namespace: str, bitwarden: BwCLI = None, vault_cluster_name: str = ""):
-    """ 
+def initialize_vault(namespace: str,
+                     vault_cluster_name: str = "",
+                     bitwarden: BwCLI = None):
+    """
     initializes vault and sets up the keys. Puts keys in bitwarden, if BwCLI
     object is passed in
     """
     # first get the vault pod
     vault_pods = None
     cmd = (f"kubectl get pods -l app.kubernetes.io/name=vault -n {namespace} "
            "--no-headers -o custom-columns=NAME:.metadata.name")
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,333 +1,181 @@
 # internal libraries
 from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
 from smol_k8s_lab.k8s_apps.operators.minio import create_minio_alias, BetterMinio
 from smol_k8s_lab.k8s_apps.social.mastodon_rake import generate_rake_secrets
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                check_if_argocd_app_exists,
-                                                wait_for_argocd_app,
-                                                sync_argocd_app,
-                                                update_argocd_appset_secret)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
+from smol_k8s_lab.k8s_tools.restores import restore_seaweedfs, restore_cnpg_cluster
 from smol_k8s_lab.utils.passwords import create_password
 from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.utils.run.subproc import subproc
+from smol_k8s_lab.utils.value_from import extract_secret, process_backup_vals
+from smol_k8s_lab.utils.minio_lib import BetterMinio
 
 # external libraries
 import logging as log
 
 
-def configure_mastodon(k8s_obj: K8s,
-                       config_dict: dict,
+def configure_mastodon(argocd: ArgoCD,
+                       cfg: dict,
+                       pvc_storage_class: str,
                        bitwarden: BwCLI = None,
                        minio_obj: BetterMinio = {}) -> bool:
     """
     creates a mastodon app and initializes it with secrets if you'd like :)
+
+    required:
+        argocd            - ArgoCD() object for Argo CD operations
+        cfg               - dict, with at least argocd key and init key
+        pvc_storage_class - str, storage class of PVC
+
+    optional:
+        bitwarden   - BwCLI() object with session token to create bitwarden items
     """
-    header("Setting up [green]Mastodon[/], so you can self host your social media"
+    # check immediately if the app is installed
+    app_installed = argocd.check_if_app_exists('mastodon')
+
+    # verify if initialization is enabled
+    init = cfg.get('init', {'enabled': True, 'restore': {'enabled': False}})
+    init_enabled = init.get('enabled', True)
+
+    # check if we're restoring and get values for that
+    restore_dict = init.get('restore', {"enabled": False})
+    restore_enabled = restore_dict['enabled']
+
+    # figure out what header to print
+    if restore_enabled:
+        header_start = "Restoring"
+    else:
+        if app_installed:
+            header_start = "Syncing"
+        else:
+            header_start = "Setting up"
+
+    header(f"{header_start} [green]Mastodon[/], so you can self host your social media",
            '🐘')
-    app_installed = check_if_argocd_app_exists('mastodon')
-    init_enabled = config_dict['init']['enabled']
-    secrets = config_dict['argo']['secret_keys']
+
+    # get any secrets for this app
+    secrets = cfg['argo']['secret_keys']
     if secrets:
         mastodon_hostname = secrets['hostname']
 
-    if init_enabled and not app_installed:
-        k8s_obj.create_namespace('mastodon')
+    # we need namespace immediately
+    mastodon_namespace = cfg['argo']['namespace']
 
-        # declare custom values for mastodon
-        init_values = config_dict['init']['values']
+    if init_enabled and not app_installed:
+        argocd.k8s.create_namespace(mastodon_namespace)
 
-        # configure the admin user credentials
-        mastodon_admin_username = init_values['admin_user']
-        mastodon_admin_email = init_values['admin_email']
-
-        # configure the smtp credentials
-        smtp_user = init_values['smtp_user']
-        smtp_pass = init_values['smtp_password']
-        smtp_host = init_values['smtp_host']
+        if not restore_enabled:
+            # declare custom values for mastodon
+            init_values = init.get('values', None)
+            # configure the admin user credentials
+            mastodon_admin_username = init_values.get('admin_user', 'tootadmin')
+            mastodon_admin_email = init_values.get('admin_email', '')
+
+            # configure the smtp credentials
+            mail_user = init_values.get('smtp_user', '')
+            mail_host = init_values.get('smtp_host', '')
+            mail_pass = extract_secret(init_values.get('smtp_password'))
+
+            # main mastodon rake secrets
+            rake_secrets = generate_rake_secrets()
+
+            # configure s3 credentials
+            s3_access_id = 'mastodon'
+            s3_access_key = create_password()
 
         s3_endpoint = secrets.get('s3_endpoint', "")
         log.debug(f"Mastodon s3_endpoint at the start is: {s3_endpoint}")
-        # configure s3 credentials
-        s3_access_id = 'mastodon'
-        s3_access_key = create_password()
-        # credentials of remote backups of s3 PVCs
-        restic_repo_pass = init_values.get('restic_repo_password', "")
-        backups_s3_user = init_values.get('s3_backup_access_id', "")
-        backups_s3_password = init_values.get('s3_backup_secret_key', "")
-
-        # main mastodon rake secrets
-        rake_secrets = generate_rake_secrets()
-
-        # create a local alias to check and make sure mastodon is functional
-        create_minio_alias("mastodon", s3_endpoint, "mastodon", s3_access_key)
-
-        if bitwarden:
-            # S3 credentials
-            # endpoint that gets put into the secret should probably have http in it
-            if "http" not in s3_endpoint:
-                log.debug(f"Mastodon s3_endpoint did not have http in it: {s3_endpoint}")
-                s3_endpoint = "https://" + s3_endpoint
-                log.debug(f"Mastodon s3_endpoint - after prepending 'https://': {s3_endpoint}")
-            mastodon_s3_endpoint_obj = create_custom_field("s3Endpoint", s3_endpoint)
-            mastodon_s3_host_obj = create_custom_field("s3Hostname", s3_endpoint.replace("https://", ""))
-            mastodon_s3_bucket_obj = create_custom_field("s3Bucket", "mastodon")
-            s3_id = bitwarden.create_login(
-                    name='mastodon-user-s3-credentials',
-                    item_url=mastodon_hostname,
-                    user=s3_access_id,
-                    password=s3_access_key,
-                    fields=[
-                        mastodon_s3_endpoint_obj,
-                        mastodon_s3_host_obj,
-                        mastodon_s3_bucket_obj
-                        ]
-                    )
-
-            pgsql_s3_key = create_password()
-            s3_db_id = bitwarden.create_login(
-                    name='mastodon-postgres-s3-credentials',
-                    item_url=mastodon_hostname,
-                    user="mastodon-postgres",
-                    password=pgsql_s3_key
-                    )
-
-            admin_s3_key = create_password()
-            s3_admin_id = bitwarden.create_login(
-                    name='mastodon-admin-s3-credentials',
-                    item_url=mastodon_hostname,
-                    user="mastodon-root",
-                    password=admin_s3_key
-                    )
-
-            # credentials for remote backups of the s3 PVC
-            restic_repo_pass_obj = create_custom_field("resticRepoPassword", restic_repo_pass)
-            s3_backups_id = bitwarden.create_login(
-                    name='mastodon-backups-s3-credentials',
-                    item_url=mastodon_hostname,
-                    user=backups_s3_user,
-                    password=backups_s3_password,
-                    fields=[restic_repo_pass_obj]
-                    )
-
-            # elastic search password
-            mastodon_elasticsearch_password = bitwarden.generate()
-            elastic_id = bitwarden.create_login(
-                    name='mastodon-elasticsearch-credentials',
-                    item_url=mastodon_hostname,
-                    user='mastodon',
-                    password=mastodon_elasticsearch_password
-                    )
-
-            # PostgreSQL credentials
-            mastodon_pgsql_password = bitwarden.generate()
-            postrges_pass_obj = create_custom_field("postgresPassword",
-                                                    mastodon_pgsql_password)
-            db_id = bitwarden.create_login(
-                    name='mastodon-pgsql-credentials',
-                    item_url=mastodon_hostname,
-                    user='mastodon',
-                    password=mastodon_pgsql_password,
-                    fields=[postrges_pass_obj]
-                    )
-
-            # Redis credentials
-            mastodon_redis_password = bitwarden.generate()
-            redis_id = bitwarden.create_login(
-                    name='mastodon-redis-credentials',
-                    item_url=mastodon_hostname,
-                    user='mastodon',
-                    password=mastodon_redis_password
-                    )
-
-            # SMTP credentials
-            mastodon_smtp_host_obj = create_custom_field("smtpHostname", smtp_host)
-            smtp_id = bitwarden.create_login(
-                    name='mastodon-smtp-credentials',
-                    item_url=mastodon_hostname,
-                    user=smtp_user,
-                    password=smtp_pass,
-                    fields=[mastodon_smtp_host_obj]
-                    )
-
-            # admin credentials for mastodon itself
-            # toot_password = create_password()
-            # email_obj = create_custom_field("email", mastodon_admin_email)
-            # admin_id = bitwarden.create_login(
-            #         name='mastodon-admin-credentials',
-            #         item_url=mastodon_hostname,
-            #         user=mastodon_admin_username,
-            #         password=toot_password,
-            #         fields=[email_obj]
-            #         )
-
-            # mastodon secrets
-            secret_key_base_obj = create_custom_field(
-                    "SECRET_KEY_BASE",
-                    rake_secrets['SECRET_KEY_BASE']
-                    )
-            otp_secret_obj = create_custom_field(
-                    "OTP_SECRET",
-                    rake_secrets['OTP_SECRET']
-                    )
-            vapid_pub_key_obj = create_custom_field(
-                    "VAPID_PUBLIC_KEY",
-                    rake_secrets['VAPID_PUBLIC_KEY']
-                    )
-            vapid_priv_key_obj = create_custom_field(
-                    "VAPID_PRIVATE_KEY",
-                    rake_secrets['VAPID_PRIVATE_KEY']
-                    )
-
-            secrets_id = bitwarden.create_login(
-                    name='mastodon-server-secrets',
-                    item_url=mastodon_hostname,
-                    user="mastodon",
-                    password="none",
-                    fields=[
-                        secret_key_base_obj,
-                        otp_secret_obj,
-                        vapid_priv_key_obj,
-                        vapid_pub_key_obj
-                        ]
-                    )
-            
-            # update the mastodon values for the argocd appset
-            # 'mastodon_admin_credentials_bitwarden_id': admin_id,
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {'mastodon_smtp_credentials_bitwarden_id': smtp_id,
-                     'mastodon_postgres_credentials_bitwarden_id': db_id,
-                     'mastodon_redis_bitwarden_id': redis_id,
-                     'mastodon_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                     'mastodon_s3_postgres_credentials_bitwarden_id': s3_db_id,
-                     'mastodon_s3_mastodon_credentials_bitwarden_id': s3_id,
-                     'mastodon_s3_backups_credentials_bitwarden_id': s3_backups_id,
-                     'mastodon_elasticsearch_credentials_bitwarden_id': elastic_id,
-                     'mastodon_server_secrets_bitwarden_id': secrets_id})
-
-            # reload the bitwarden ESO provider
-            try:
-                k8s_obj.reload_deployment('bitwarden-eso-provider', 'external-secrets')
-            except Exception as e:
-                log.error(
-                        "Couldn't scale down the [magenta]bitwarden-eso-provider"
-                        "[/] deployment in [green]external-secrets[/] namespace."
-                        f"Recieved: {e}"
-                        )
+
+        if not restore_enabled:
+            # create a local alias to check and make sure mastodon is functional
+            create_minio_alias("mastodon", s3_endpoint, "mastodon", s3_access_key)
+
+        # backups are their own config.yaml section
+        backup_vals = process_backup_vals(cfg.get('backups', {}), 'mastodon', argocd)
+
+        if bitwarden and not restore_enabled:
+            setup_bitwarden_items(argocd,
+                                  mastodon_hostname,
+                                  s3_endpoint,
+                                  s3_access_id,
+                                  s3_access_key,
+                                  backup_vals['s3_user'],
+                                  backup_vals['s3_password'],
+                                  backup_vals['restic_repo_pass'],
+                                  mastodon_admin_username,
+                                  mail_host,
+                                  mail_user,
+                                  mail_pass,
+                                  rake_secrets,
+                                  bitwarden)
 
         # these are standard k8s secrets yaml
-        else:
+        elif not bitwarden and not restore_enabled:
             # admin creds k8s secret
             # k8s_obj.create_secret('mastodon-admin-credentials', 'mastodon',
             #               {"username": username,
             #                "email": email})
 
             # postgres creds k8s secret
             mastodon_pgsql_password = create_password()
-            k8s_obj.create_secret('mastodon-pgsql-credentials', 'mastodon',
-                          {"password": mastodon_pgsql_password,
-                           'postrgesPassword': mastodon_pgsql_password})
+            argocd.k8s.create_secret(
+                    'mastodon-pgsql-credentials',
+                    'mastodon',
+                    {"password": mastodon_pgsql_password,
+                     'postrgesPassword': mastodon_pgsql_password})
 
             # redis creds k8s secret
             mastodon_redis_password = create_password()
-            k8s_obj.create_secret('mastodon-redis-credentials', 'mastodon',
-                                  {"password": mastodon_redis_password})
+            argocd.k8s.create_secret('mastodon-redis-credentials', 'mastodon',
+                                     {"password": mastodon_redis_password})
 
             # mastodon rake secrets
-            k8s_obj.create_secret('mastodon-server-secrets', 'mastodon',
-                                  rake_secrets)
+            argocd.k8s.create_secret('mastodon-server-secrets', 'mastodon',
+                                     rake_secrets)
 
     if not app_installed:
-        install_with_argocd(k8s_obj=k8s_obj,
-                            app='mastodon',
-                            argo_dict=config_dict['argo']
-                            )
-        if init_enabled:
+        if restore_enabled:
+            restore_mastodon(argocd,
+                             mastodon_hostname,
+                             mastodon_namespace,
+                             cfg['argo'],
+                             secrets,
+                             restore_dict,
+                             backup_vals,
+                             pvc_storage_class,
+                             'mastodon-postgres',
+                             bitwarden)
+
+        if not init_enabled:
+            argocd.install_app('mastodon', cfg['argo'])
+        elif init_enabled and not restore_enabled:
+            argocd.install_app('mastodon', cfg['argo'], True)
             # for for all the mastodon apps to come up
-            wait_for_argocd_app('mastodon')
-            sync_argocd_app('mastodon-web-app')
-            wait_for_argocd_app('mastodon-web-app')
+            argocd.sync_app('mastodon-web-app')
+            argocd.wait_for_app('mastodon-web-app')
 
             # create admin credentials
             password = create_user(mastodon_admin_username,
                                    mastodon_admin_email,
-                                   config_dict['argo']['namespace'])
+                                   cfg['argo']['namespace'])
             if bitwarden:
                 sub_header("Creating secrets in Bitwarden")
                 bitwarden.create_login(
                         name='mastodon-admin-credentials',
                         item_url=mastodon_hostname,
                         user=mastodon_admin_username,
                         password=password,
                         fields=[create_custom_field("email", mastodon_admin_email)]
                         )
     else:
         log.info("mastodon already installed 🎉")
 
-        # if mastodon already installed, but bitwarden and init are enabled
-        # still populate the bitwarden IDs in the appset secret plugin secret
-        if bitwarden and config_dict['init']['enabled']:
-            log.debug("Making sure mastodon Bitwarden item IDs are in appset "
-                      "secret plugin secret")
-
-            # admin_id = bitwarden.get_item(
-            #         f"mastodon-admin-credentials-{mastodon_hostname}"
-            #         )[0]['id']
-
-            db_id = bitwarden.get_item(
-                    f"mastodon-pgsql-credentials-{mastodon_hostname}"
-                    )[0]['id']
-
-            elastic_id = bitwarden.get_item(
-                    f"mastodon-elasticsearch-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            redis_id = bitwarden.get_item(
-                    f"mastodon-redis-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            smtp_id = bitwarden.get_item(
-                    f"mastodon-smtp-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            s3_admin_id = bitwarden.get_item(
-                    f"mastodon-admin-s3-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            s3_db_id = bitwarden.get_item(
-                    f"mastodon-postgres-s3-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            s3_id = bitwarden.get_item(
-                    f"mastodon-user-s3-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            s3_backups_id = bitwarden.get_item(
-                    f"mastodon-backups-s3-credentials-{mastodon_hostname}", False
-                    )[0]['id']
-
-            secrets_id = bitwarden.get_item(
-                    f"mastodon-server-secrets-{mastodon_hostname}", False
-                    )[0]['id']
-
-            # {'mastodon_admin_credentials_bitwarden_id': admin_id,
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {'mastodon_smtp_credentials_bitwarden_id': smtp_id,
-                     'mastodon_postgres_credentials_bitwarden_id': db_id,
-                     'mastodon_redis_bitwarden_id': redis_id,
-                     'mastodon_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                     'mastodon_s3_postgres_credentials_bitwarden_id': s3_db_id,
-                     'mastodon_s3_mastodon_credentials_bitwarden_id': s3_id,
-                     'mastodon_s3_backups_credentials_bitwarden_id': s3_backups_id,
-                     'mastodon_elasticsearch_credentials_bitwarden_id': elastic_id,
-                     'mastodon_server_secrets_bitwarden_id': secrets_id}
-                    )
+        if bitwarden and init_enabled:
+            refresh_bweso(argocd, mastodon_hostname, bitwarden)
 
 
 def create_user(user: str, email: str, pod_namespace: str) -> str:
     """
     given a username, email, and namespace of the mastodon pod, we'll create a
     new mastodon user via tootctl using a kubectl exec command and then we return
     their autogenerated password
@@ -349,7 +197,337 @@
 
     # then process the output from the command and return it
     res = subproc([cmd],
                   shell=True,
                   universal_newlines=True).split()[3]
     print(f"password returned is: {res}")
     return res
+
+
+def refresh_bweso(argocd: ArgoCD,
+                  mastodon_hostname: str,
+                  bitwarden: BwCLI) -> None:
+    """
+    if mastodon already installed, but bitwarden and init are enabled, still
+    populate the bitwarden IDs in the appset secret plugin secret
+    """
+    log.debug("Making sure mastodon Bitwarden item IDs are in appset "
+              "secret plugin secret")
+
+    # admin_id = bitwarden.get_item(
+    #         f"mastodon-admin-credentials-{mastodon_hostname}"
+    #         )[0]['id']
+
+    db_id = bitwarden.get_item(
+            f"mastodon-pgsql-credentials-{mastodon_hostname}"
+            )[0]['id']
+
+    elastic_id = bitwarden.get_item(
+            f"mastodon-elasticsearch-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    redis_id = bitwarden.get_item(
+            f"mastodon-redis-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    smtp_id = bitwarden.get_item(
+            f"mastodon-smtp-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    s3_admin_id = bitwarden.get_item(
+            f"mastodon-admin-s3-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    s3_db_id = bitwarden.get_item(
+            f"mastodon-postgres-s3-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    s3_id = bitwarden.get_item(
+            f"mastodon-user-s3-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    s3_backups_id = bitwarden.get_item(
+            f"mastodon-backups-s3-credentials-{mastodon_hostname}", False
+            )[0]['id']
+
+    secrets_id = bitwarden.get_item(
+            f"mastodon-server-secrets-{mastodon_hostname}", False
+            )[0]['id']
+
+    # {'mastodon_admin_credentials_bitwarden_id': admin_id,
+    argocd.update_appset_secret(
+            {'mastodon_smtp_credentials_bitwarden_id': smtp_id,
+             'mastodon_postgres_credentials_bitwarden_id': db_id,
+             'mastodon_redis_bitwarden_id': redis_id,
+             'mastodon_s3_admin_credentials_bitwarden_id': s3_admin_id,
+             'mastodon_s3_postgres_credentials_bitwarden_id': s3_db_id,
+             'mastodon_s3_mastodon_credentials_bitwarden_id': s3_id,
+             'mastodon_s3_backups_credentials_bitwarden_id': s3_backups_id,
+             'mastodon_elasticsearch_credentials_bitwarden_id': elastic_id,
+             'mastodon_server_secrets_bitwarden_id': secrets_id}
+            )
+
+
+def setup_bitwarden_items(argocd: ArgoCD,
+                          mastodon_hostname: str,
+                          s3_endpoint: str,
+                          s3_access_id: str,
+                          s3_access_key: str,
+                          backups_s3_user: str,
+                          backups_s3_password: str,
+                          restic_repo_pass: str,
+                          admin_user: str,
+                          mail_host: str,
+                          mail_user: str,
+                          mail_pass: str,
+                          rake_secrets: dict,
+                          bitwarden: BwCLI) -> None:
+    # S3 credentials
+    # endpoint that gets put into the secret should probably have http in it
+    if "http" not in s3_endpoint:
+        log.debug(f"Mastodon s3_endpoint did not have http in it: {s3_endpoint}")
+        s3_endpoint = "https://" + s3_endpoint
+        log.debug(f"Mastodon s3_endpoint - after prepending 'https://': {s3_endpoint}")
+
+    mastodon_s3_endpoint_obj = create_custom_field("s3Endpoint", s3_endpoint)
+    mastodon_s3_host_obj = create_custom_field("s3Hostname",
+                                               s3_endpoint.replace("https://",
+                                                                   ""))
+    mastodon_s3_bucket_obj = create_custom_field("s3Bucket", "mastodon")
+    s3_id = bitwarden.create_login(
+            name='mastodon-user-s3-credentials',
+            item_url=mastodon_hostname,
+            user=s3_access_id,
+            password=s3_access_key,
+            fields=[
+                mastodon_s3_endpoint_obj,
+                mastodon_s3_host_obj,
+                mastodon_s3_bucket_obj
+                ]
+            )
+
+    pgsql_s3_key = create_password()
+    s3_db_id = bitwarden.create_login(
+            name='mastodon-postgres-s3-credentials',
+            item_url=mastodon_hostname,
+            user="mastodon-postgres",
+            password=pgsql_s3_key
+            )
+
+    admin_s3_key = create_password()
+    s3_admin_id = bitwarden.create_login(
+            name='mastodon-admin-s3-credentials',
+            item_url=mastodon_hostname,
+            user="mastodon-root",
+            password=admin_s3_key
+            )
+
+    # credentials for remote backups of the s3 PVC
+    restic_repo_pass_obj = create_custom_field("resticRepoPassword", restic_repo_pass)
+    s3_backups_id = bitwarden.create_login(
+            name='mastodon-backups-s3-credentials',
+            item_url=mastodon_hostname,
+            user=backups_s3_user,
+            password=backups_s3_password,
+            fields=[restic_repo_pass_obj]
+            )
+
+    # elastic search password
+    mastodon_elasticsearch_password = bitwarden.generate()
+    elastic_id = bitwarden.create_login(
+            name='mastodon-elasticsearch-credentials',
+            item_url=mastodon_hostname,
+            user='mastodon',
+            password=mastodon_elasticsearch_password
+            )
+
+    # PostgreSQL credentials
+    mastodon_pgsql_password = bitwarden.generate()
+    postrges_pass_obj = create_custom_field("postgresPassword",
+                                            mastodon_pgsql_password)
+    db_id = bitwarden.create_login(
+            name='mastodon-pgsql-credentials',
+            item_url=mastodon_hostname,
+            user='mastodon',
+            password=mastodon_pgsql_password,
+            fields=[postrges_pass_obj]
+            )
+
+    # Redis credentials
+    mastodon_redis_password = bitwarden.generate()
+    redis_id = bitwarden.create_login(
+            name='mastodon-redis-credentials',
+            item_url=mastodon_hostname,
+            user='mastodon',
+            password=mastodon_redis_password
+            )
+
+    # SMTP credentials
+    mastodon_smtp_host_obj = create_custom_field("smtpHostname", mail_host)
+    smtp_id = bitwarden.create_login(
+            name='mastodon-smtp-credentials',
+            item_url=mastodon_hostname,
+            user=mail_user,
+            password=mail_pass,
+            fields=[mastodon_smtp_host_obj]
+            )
+
+    # admin credentials for mastodon itself
+    # toot_password = create_password()
+    # email_obj = create_custom_field("email", mastodon_admin_email)
+    # admin_id = bitwarden.create_login(
+    #         name='mastodon-admin-credentials',
+    #         item_url=mastodon_hostname,
+    #         user=mastodon_admin_username,
+    #         password=toot_password,
+    #         fields=[email_obj]
+    #         )
+
+    # mastodon secrets
+    secret_key_base_obj = create_custom_field(
+            "SECRET_KEY_BASE",
+            rake_secrets['SECRET_KEY_BASE']
+            )
+    otp_secret_obj = create_custom_field(
+            "OTP_SECRET",
+            rake_secrets['OTP_SECRET']
+            )
+    vapid_pub_key_obj = create_custom_field(
+            "VAPID_PUBLIC_KEY",
+            rake_secrets['VAPID_PUBLIC_KEY']
+            )
+    vapid_priv_key_obj = create_custom_field(
+            "VAPID_PRIVATE_KEY",
+            rake_secrets['VAPID_PRIVATE_KEY']
+            )
+
+    secrets_id = bitwarden.create_login(
+            name='mastodon-server-secrets',
+            item_url=mastodon_hostname,
+            user="mastodon",
+            password="none",
+            fields=[
+                secret_key_base_obj,
+                otp_secret_obj,
+                vapid_priv_key_obj,
+                vapid_pub_key_obj
+                ]
+            )
+
+    # update the mastodon values for the argocd appset
+    # 'mastodon_admin_credentials_bitwarden_id': admin_id,
+    argocd.update_appset_secret(
+            {'mastodon_smtp_credentials_bitwarden_id': smtp_id,
+             'mastodon_postgres_credentials_bitwarden_id': db_id,
+             'mastodon_redis_bitwarden_id': redis_id,
+             'mastodon_s3_admin_credentials_bitwarden_id': s3_admin_id,
+             'mastodon_s3_postgres_credentials_bitwarden_id': s3_db_id,
+             'mastodon_s3_mastodon_credentials_bitwarden_id': s3_id,
+             'mastodon_s3_backups_credentials_bitwarden_id': s3_backups_id,
+             'mastodon_elasticsearch_credentials_bitwarden_id': elastic_id,
+             'mastodon_server_secrets_bitwarden_id': secrets_id})
+
+    # reload the bitwarden ESO provider
+    try:
+        argocd.k8s.reload_deployment('bitwarden-eso-provider',
+                                     'external-secrets')
+    except Exception as e:
+        log.error(
+                "Couldn't scale down the [magenta]bitwarden-eso-provider"
+                "[/] deployment in [green]external-secrets[/] namespace."
+                f"Recieved: {e}"
+                )
+
+def restore_mastodon(argocd: ArgoCD,
+                     mastodon_hostname: str,
+                     mastodon_namespace: str,
+                     argo_dict: dict,
+                     secrets: dict,
+                     restore_dict: dict,
+                     backup_dict: dict,
+                     pvc_storage_class: str,
+                     pgsql_cluster_name: str,
+                     bitwarden: BwCLI) -> None:
+    """
+    restore mastodon seaweedfs PVCs, mastodon files and/or config PVC(s),
+    and CNPG postgresql cluster
+    """
+    # this is the info for the REMOTE backups
+    s3_backup_endpoint = backup_dict['endpoint']
+    s3_backup_bucket = backup_dict['bucket']
+    access_key_id = backup_dict["s3_user"]
+    secret_access_key = backup_dict["s3_password"]
+    restic_repo_password = backup_dict['restic_repo_pass']
+    cnpg_backup_schedule = backup_dict['postgres_schedule']
+
+    # first we grab existing bitwarden items if they exist
+    if bitwarden:
+        refresh_bweso(argocd, mastodon_hostname, bitwarden)
+
+        # apply the external secrets so we can immediately use them for restores
+        # ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️
+        # WARNING: change this back to main when done testing
+        # ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️ ⚠️
+        ref = "add-pvc-helm-chart-for-mastodon"
+        external_secrets_yaml = (
+                "https://raw.githubusercontent.com/small-hack/argocd-apps/"
+                f"{ref}/mastodon/app_of_apps/external_secrets_argocd_appset.yaml"
+                )
+        argocd.k8s.apply_manifests(external_secrets_yaml, argocd.namespace)
+
+        # postgresql s3 ID
+        s3_db_creds = bitwarden.get_item(
+                f"mastodon-postgres-s3-credentials-{mastodon_hostname}", False
+                )[0]['login']
+
+        pg_access_key_id = s3_db_creds["username"]
+        pg_secret_access_key = s3_db_creds["password"]
+
+    # these are the remote backups for seaweedfs
+    s3_pvc_capacity = secrets['s3_pvc_capacity']
+
+    # then we create all the seaweedfs pvcs we lost and restore them
+    snapshot_ids = restore_dict['restic_snapshot_ids']
+    restore_seaweedfs(
+            argocd.k8s,
+            'mastodon',
+            mastodon_namespace,
+            argocd.namespace,
+            s3_backup_endpoint,
+            s3_backup_bucket,
+            access_key_id,
+            secret_access_key,
+            restic_repo_password,
+            s3_pvc_capacity,
+            pvc_storage_class,
+            "ReadWriteOnce",
+            snapshot_ids['seaweedfs_volume'],
+            snapshot_ids['seaweedfs_master'],
+            snapshot_ids['seaweedfs_filer']
+            )
+
+    # then we finally can restore the postgres database :D
+    if restore_dict.get("cnpg_restore", False):
+        psql_version = restore_dict.get("postgresql_version", 16)
+        s3_endpoint = secrets.get('s3_endpoint', "")
+        restore_cnpg_cluster('mastodon',
+                             mastodon_namespace,
+                             pgsql_cluster_name,
+                             psql_version,
+                             s3_endpoint,
+                             pg_access_key_id,
+                             pg_secret_access_key,
+                             seaweedf_s3_endpoint,
+                             pgsql_cluster_name,
+                             cnpg_backup_schedule)
+
+    # todo: from here on out, this could be async to start on other tasks
+    # install mastodon as usual
+    argocd.install_app('mastodon', argo_dict)
+
+    # verify mastodon rolled out
+    rollout = (f"kubectl rollout status -n {mastodon_namespace} "
+               "deployment/mastodon-web-app --watch --timeout 10m")
+    while True:
+        rolled_out = subproc([rollout])
+        if "NotFound" not in rolled_out:
+            break
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """ 
 This is just for generating mastodon rake secrets and testing on the cli
 """
-from smol_k8s_lab.utils.subproc import subproc
+from smol_k8s_lab.utils.run.subproc import subproc
 
 
 def generate_rake_secrets() -> None:
     """
     These are required for mastodon:
         https://docs.joinmastodon.org/admin/config/#secrets
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,102 @@
 # internal libraries
+from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
 from smol_k8s_lab.k8s_apps.operators.minio import create_minio_alias
 from smol_k8s_lab.k8s_apps.identity_provider.zitadel_api import Zitadel
-from smol_k8s_lab.bitwarden.bw_cli import BwCLI, create_custom_field
-from smol_k8s_lab.k8s_tools.argocd_util import (install_with_argocd,
-                                                check_if_argocd_app_exists,
-                                                update_argocd_appset_secret)
-from smol_k8s_lab.k8s_tools.k8s_lib import K8s
-from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
+from smol_k8s_lab.k8s_apps.social.nextcloud_occ_commands import Nextcloud
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
+from smol_k8s_lab.k8s_tools.restores import (restore_seaweedfs,
+                                             recreate_pvc,
+                                             k8up_restore_pvc,
+                                             restore_cnpg_cluster)
 from smol_k8s_lab.utils.passwords import create_password
+from smol_k8s_lab.utils.rich_cli.console_logging import sub_header, header
+from smol_k8s_lab.utils.run.subproc import subproc
+from smol_k8s_lab.utils.value_from import extract_secret, process_backup_vals
 
 # external libraries
 import logging as log
 from rich.prompt import Prompt
 
 
-def configure_nextcloud(k8s_obj: K8s,
-                        config_dict: dict,
-                        bitwarden: BwCLI = None,
-                        zitadel: Zitadel = None) -> None:
+def configure_nextcloud(argocd: ArgoCD,
+                        cfg: dict,
+                        pvc_storage_class: str,
+                        zitadel: Zitadel = None,
+                        bitwarden: BwCLI = None) -> None:
     """
     creates a nextcloud app and initializes it with secrets if you'd like :)
 
     required:
-        k8s_obj     - K8s() object with cluster credentials
-        config_dict - dictionary with at least argocd key and init key
+        argocd            - ArgoCD() object for Argo CD operations
+        cfg               - dict, with at least argocd key and init key
+        pvc_storage_class - str, storage class of PVC
 
     optional:
         bitwarden   - BwCLI() object with session token to create bitwarden items
         zitadel     - Zitadel() object with session token to create zitadel oidc app and roles
     """
     # check immediately if this app is installed
-    app_installed = check_if_argocd_app_exists('nextcloud')
+    app_installed = argocd.check_if_app_exists('nextcloud')
 
     # get any secret keys passed in
-    secrets = config_dict['argo']['secret_keys']
+    secrets = cfg['argo']['secret_keys']
     if secrets:
         nextcloud_hostname = secrets['hostname']
 
     # verify if initialization is enabled
-    init_enabled = config_dict['init']['enabled']
+    init = cfg.get('init', {'enabled': True, 'restore': {'enabled': False}})
+    init_enabled = init.get('enabled', True)
+
+    # check if we're restoring and get values for that
+    restore_dict = init.get('restore', {"enabled": False})
+    restore_enabled = restore_dict['enabled']
+
+    # figure out what header to print
+    if restore_enabled:
+        header_start = "Restoring"
+    else:
+        if app_installed:
+            header_start = "Syncing"
+        else:
+            header_start = "Setting up"
+
+    header(f"{header_start} [green]Nextcloud[/], to self host your files",
+           '🩵')
 
     # if the user has chosen to use smol-k8s-lab initialization
     if not app_installed and init_enabled:
-        k8s_obj.create_namespace(config_dict['argo']['namespace'])
-        header("Setting up [green]Nextcloud[/], to self host your files",
-               '🩵')
+        nextcloud_namespace = cfg['argo']['namespace']
+        argocd.k8s.create_namespace(nextcloud_namespace)
+
 
         # grab all possile init values
-        init_values = config_dict['init'].get('values', None)
+        init_values = init.get('values', None)
         if init_values:
             admin_user = init_values.get('admin_user', 'admin')
+
             # stmp config values
             mail_host = init_values.get('smtp_host', None)
             mail_user = init_values.get('smtp_user', None)
-            mail_pass = init_values.get('smtp_password', None)
-            # credentials of remote backups of s3 PVCs
-            restic_repo_pass = init_values.get('restic_repo_password', "")
-            backups_s3_user = init_values.get('s3_backup_access_id', "")
-            backups_s3_password = init_values.get('s3_backup_secret_key', "")
+            mail_pass = extract_secret(init_values.get('smtp_password', ""))
+        else:
+            log.warn("Strange, there's no nextcloud init values...")
+
+        # backups are their own config.yaml section
+        backup_vals = process_backup_vals(cfg.get('backups', {}), 'nextcloud', argocd)
 
         if secrets:
             s3_endpoint = secrets.get('s3_endpoint', "")
-            if s3_endpoint:
+            if s3_endpoint and not restore_enabled:
                 s3_access_key = create_password()
                 # create a local alias to check and make sure nextcloud is functional
-                create_minio_alias("nextcloud", s3_endpoint, "nextcloud", s3_access_key)
+                create_minio_alias(minio_alias="nextcloud",
+                                   minio_hostname=s3_endpoint,
+                                   access_key="nextcloud",
+                                   secret_key=s3_access_key)
 
         # configure SMTP
         if not mail_host:
             mail_host = Prompt.ask(
                     "[green]Please enter the SMTP host for nextcoud"
                     )
 
@@ -77,217 +105,398 @@
             mail_user = Prompt.ask(m)
 
         if not mail_pass:
             m = f"[green]Please enter the SMTP password of {mail_user} on {mail_host}"
             mail_pass = Prompt.ask(m, password=True)
 
         # configure OIDC
-        if zitadel:
+        if zitadel and not restore_enabled:
             log.debug("Creating a Nextcloud OIDC application in Zitadel...")
             redirect_uris = f"https://{nextcloud_hostname}/apps/oidc_login/oidc"
             logout_uris = [f"https://{nextcloud_hostname}"]
             oidc_creds = zitadel.create_application(
                     "nextcloud",
                     redirect_uris,
                     logout_uris
                     )
-            zitadel.create_role("nextcloud_users", "Nextcloud Users", "nextcloud_users")
-            zitadel.create_role("nextcloud_admins", "Nextcloud Admins", "nextcloud_admins")
+            zitadel.create_role("nextcloud_users",
+                                "Nextcloud Users",
+                                "nextcloud_users")
+            zitadel.create_role("nextcloud_admins",
+                                "Nextcloud Admins",
+                                "nextcloud_admins")
             zitadel.update_user_grant(['nextcloud_admins'])
+            zitadel_hostname = zitadel.hostname
+        else:
+            zitadel_hostname = ""
 
         # if bitwarden is enabled, we create login items for each set of credentials
-        if bitwarden:
-            sub_header("Creating Nextcloud items in Bitwarden")
-
-            # s3 credentials creation
-            bucket_obj = create_custom_field('bucket', "nextcloud-data")
-            endpoint_obj = create_custom_field('endpoint', s3_endpoint)
-            s3_id = bitwarden.create_login(
-                    name='nextcloud-user-s3-credentials',
-                    item_url=nextcloud_hostname,
-                    user="nextcloud",
-                    password=s3_access_key,
-                    fields=[bucket_obj, endpoint_obj]
-                    )
-
-            pgsql_s3_key = create_password()
-            s3_db_id = bitwarden.create_login(
-                    name='nextcloud-postgres-s3-credentials',
-                    item_url=nextcloud_hostname,
-                    user="nextcloud-postgres",
-                    password=pgsql_s3_key
-                    )
-
-            admin_s3_key = create_password()
-            s3_admin_id = bitwarden.create_login(
-                    name='nextcloud-admin-s3-credentials',
-                    item_url=nextcloud_hostname,
-                    user="nextcloud-root",
-                    password=admin_s3_key
-                    )
-
-            # credentials for remote backups of the s3 PVC
-            restic_repo_pass_obj = create_custom_field("resticRepoPassword", restic_repo_pass)
-            s3_backups_id = bitwarden.create_login(
-                    name='nextcloud-backups-s3-credentials',
-                    item_url=nextcloud_hostname,
-                    user=backups_s3_user,
-                    password=backups_s3_password,
-                    fields=[restic_repo_pass_obj]
-                    )
-
-            # oidc credentials if they were given, else they're probably already there
-            if oidc_creds:
-                log.debug("Creating OIDC credentials for Nextcloud in Bitwarden...")
-                issuer_obj = create_custom_field("issuer", "https://" + zitadel.hostname)
-                oidc_id = bitwarden.create_login(
-                        name='nextcloud-oidc-credentials',
-                        item_url=nextcloud_hostname,
-                        user=oidc_creds['client_id'],
-                        password=oidc_creds['client_secret'],
-                        fields=[issuer_obj]
-                        )
-            else:
-                oidc_id = bitwarden.get_item(
-                        f"nextcloud-oidc-credentials-{nextcloud_hostname}"
-                        )[0]['id']
-
-            # admin credentials + metrics server info token
-            token = bitwarden.generate()
-            admin_password = bitwarden.generate()
-            serverinfo_token_obj = create_custom_field("serverInfoToken", token)
-            admin_id = bitwarden.create_login(
-                    name='nextcloud-admin-credentials',
-                    item_url=nextcloud_hostname,
-                    user=admin_user,
-                    password=admin_password,
-                    fields=[serverinfo_token_obj]
-                    )
-
-            # smtp credentials
-            smtpHost = create_custom_field("hostname", mail_host)
-            smtp_id = bitwarden.create_login(
-                    name='nextcloud-smtp-credentials',
-                    item_url=nextcloud_hostname,
-                    user=mail_user,
-                    password=mail_pass,
-                    fields=[smtpHost]
-                    )
-
-            # postgres db credentials creation
-            db_id = bitwarden.create_login(
-                    name='nextcloud-pgsql-credentials',
-                    item_url=nextcloud_hostname,
-                    user='nextcloud',
-                    password='we-dont-use-the-password-anymore-we-use-tls'
-                    )
-
-            # redis credentials creation
-            nextcloud_redis_password = bitwarden.generate()
-            redis_id = bitwarden.create_login(
-                    name='nextcloud-redis-credentials',
-                    item_url=nextcloud_hostname,
-                    user='nextcloud',
-                    password=nextcloud_redis_password
-                    )
-
-            # update the nextcloud values for the argocd appset
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {'nextcloud_admin_credentials_bitwarden_id': admin_id,
-                     'nextcloud_oidc_credentials_bitwarden_id': oidc_id,
-                     'nextcloud_smtp_credentials_bitwarden_id': smtp_id,
-                     'nextcloud_postgres_credentials_bitwarden_id': db_id,
-                     'nextcloud_redis_bitwarden_id': redis_id,
-                     'nextcloud_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                     'nextcloud_s3_postgres_credentials_bitwarden_id': s3_db_id,
-                     'nextcloud_s3_nextcloud_credentials_bitwarden_id': s3_id,
-                     'nextcloud_s3_backups_credentials_bitwarden_id': s3_backups_id}
-                    )
+        if bitwarden and not restore_enabled:
+            setup_bitwarden_items(argocd,
+                                  nextcloud_hostname,
+                                  s3_endpoint,
+                                  s3_access_key,
+                                  backup_vals['s3_user'],
+                                  backup_vals['s3_password'],
+                                  backup_vals['restic_repo_pass'],
+                                  admin_user,
+                                  mail_host,
+                                  mail_user,
+                                  mail_pass,
+                                  oidc_creds,
+                                  zitadel_hostname,
+                                  bitwarden)
 
         # these are standard k8s secrets
-        else:
+        elif not bitwarden and not restore_enabled:
             # nextcloud admin credentials and smtp credentials
             token = create_password()
             admin_password = create_password()
-            k8s_obj.create_secret('nextcloud-admin-credentials', 'nextcloud',
-                                  {"username": admin_user,
-                                   "password": admin_password,
-                                   "serverInfoToken": token,
-                                   "smtpHost": mail_host,
-                                   "smtpUsername": mail_user,
-                                   "smtpPassword": mail_pass})
+            argocd.k8s.create_secret('nextcloud-admin-credentials', 'nextcloud',
+                                     {"username": admin_user,
+                                      "password": admin_password,
+                                      "serverInfoToken": token,
+                                      "smtpHost": mail_host,
+                                      "smtpUsername": mail_user,
+                                      "smtpPassword": mail_pass})
 
             # postgres db credentials creation
-            k8s_obj.create_secret('nextcloud-pgsql-credentials', 'nextcloud',
-                                  {"username": 'nextcloud',
-                                   "password": 'we-use-tls-instead-of-password'})
+            argocd.k8s.create_secret('nextcloud-pgsql-credentials', 'nextcloud',
+                                     {"username": 'nextcloud',
+                                      "password": 'we-use-tls-instead-of-password'})
 
             # redis credentials creation
             nextcloud_redis_password = create_password()
-            k8s_obj.create_secret('nextcloud-redis-credentials', 'nextcloud',
-                                  {"password": nextcloud_redis_password})
+            argocd.k8s.create_secret('nextcloud-redis-credentials', 'nextcloud',
+                                     {"password": nextcloud_redis_password})
 
             # s3 credentials creation
-            k8s_obj.create_secret('nextcloud-s3-credentials', 'nextcloud',
-                                  {"S3_USER": "nextcloud",
-                                   "S3_PASSWORD": s3_access_key,
-                                   "S3_ENDPOINT": s3_endpoint})
+            argocd.k8s.create_secret('nextcloud-s3-credentials', 'nextcloud',
+                                     {"accessKeyId": "nextcloud",
+                                      "secretAccessKey": s3_access_key,
+                                      "S3_ENDPOINT": s3_endpoint})
 
     if not app_installed:
-        install_with_argocd(k8s_obj, 'nextcloud', config_dict['argo'])
+        # if the user is restoring, the process is a little different
+        if init_enabled and restore_enabled:
+            restore_nextcloud(argocd,
+                              nextcloud_hostname,
+                              nextcloud_namespace,
+                              cfg['argo'],
+                              secrets,
+                              restore_dict,
+                              backup_vals,
+                              pvc_storage_class,
+                              'nextcloud-postgres',
+                              bitwarden)
+        else:
+            argocd.install_app('nextcloud', cfg['argo'])
     else:
         log.info("nextcloud already installed 🎉")
-
-        # if bitwarden and init are enabled, make sure we populate appset secret
-        # plugin secret with bitwarden item IDs
         if bitwarden and init_enabled:
-            log.debug("Making sure nextcloud Bitwarden item IDs are in appset "
-                      "secret plugin secret")
-            oidc_id = bitwarden.get_item(
-                    f"nextcloud-oidc-credentials-{nextcloud_hostname}"
-                    )[0]['id']
-
-            admin_id = bitwarden.get_item(
-                    f"nextcloud-admin-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            smtp_id = bitwarden.get_item(
-                    f"nextcloud-smtp-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            db_id = bitwarden.get_item(
-                    f"nextcloud-pgsql-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            redis_id = bitwarden.get_item(
-                    f"nextcloud-redis-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            s3_admin_id = bitwarden.get_item(
-                    f"nextcloud-admin-s3-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            s3_db_id = bitwarden.get_item(
-                    f"nextcloud-postgres-s3-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            s3_id = bitwarden.get_item(
-                    f"nextcloud-user-s3-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            s3_backups_id = bitwarden.get_item(
-                    f"nextcloud-backups-s3-credentials-{nextcloud_hostname}", False
-                    )[0]['id']
-
-            update_argocd_appset_secret(
-                    k8s_obj,
-                    {'nextcloud_admin_credentials_bitwarden_id': admin_id,
-                     'nextcloud_oidc_credentials_bitwarden_id': oidc_id,
-                     'nextcloud_smtp_credentials_bitwarden_id': smtp_id,
-                     'nextcloud_postgres_credentials_bitwarden_id': db_id,
-                     'nextcloud_redis_bitwarden_id': redis_id,
-                     'nextcloud_s3_admin_credentials_bitwarden_id': s3_admin_id,
-                     'nextcloud_s3_postgres_credentials_bitwarden_id': s3_db_id,
-                     'nextcloud_s3_nextcloud_credentials_bitwarden_id': s3_id,
-                     'nextcloud_s3_backups_credentials_bitwarden_id': s3_backups_id
-                    })
+            refresh_bweso(argocd, nextcloud_hostname, bitwarden)
+
+
+def restore_nextcloud(argocd: ArgoCD,
+                      nextcloud_hostname: str,
+                      nextcloud_namespace: str,
+                      argo_dict: dict,
+                      secrets: dict,
+                      restore_dict: dict,
+                      backup_dict: dict,
+                      pvc_storage_class: str,
+                      pgsql_cluster_name: str,
+                      bitwarden: BwCLI) -> None:
+    """
+    restore nextcloud seaweedfs PVCs, nextcloud files and/or config PVC(s),
+    and CNPG postgresql cluster
+    """
+    # this is the info for the REMOTE backups
+    s3_backup_endpoint = backup_dict['endpoint']
+    s3_backup_bucket = backup_dict['bucket']
+    access_key_id = backup_dict["s3_user"]
+    secret_access_key = backup_dict["s3_password"]
+    restic_repo_password = backup_dict['restic_repo_pass']
+    cnpg_backup_schedule = backup_dict['postgres_schedule']
+
+    # first we grab existing bitwarden items if they exist
+    if bitwarden:
+        refresh_bweso(argocd, nextcloud_hostname, bitwarden)
+
+        # apply the external secrets so we can immediately use them for restores
+        external_secrets_yaml = (
+                "https://raw.githubusercontent.com/small-hack/argocd-apps/main/"
+                "nextcloud/app_of_apps/external_secrets_argocd_appset.yaml"
+                )
+        argocd.k8s.apply_manifests(external_secrets_yaml, argocd.namespace)
+
+        # postgresql s3 ID
+        s3_db_creds = bitwarden.get_item(
+                f"nextcloud-postgres-s3-credentials-{nextcloud_hostname}", False
+                )[0]['login']
+
+        pg_access_key_id = s3_db_creds["username"]
+        pg_secret_access_key = s3_db_creds["password"]
+
+    # these are the remote backups for seaweedfs
+    s3_pvc_capacity = secrets['s3_pvc_capacity']
+
+    # then we create all the seaweedfs pvcs we lost and restore them
+    snapshot_ids = restore_dict['restic_snapshot_ids']
+    restore_seaweedfs(
+            argocd,
+            'nextcloud',
+            nextcloud_namespace,
+            s3_backup_endpoint,
+            s3_backup_bucket,
+            access_key_id,
+            secret_access_key,
+            restic_repo_password,
+            s3_pvc_capacity,
+            pvc_storage_class,
+            "ReadWriteOnce",
+            snapshot_ids['seaweedfs_volume'],
+            snapshot_ids['seaweedfs_master'],
+            snapshot_ids['seaweedfs_filer']
+            )
+
+    # then we finally can restore the postgres database :D
+    if restore_dict.get("cnpg_restore", False):
+        psql_version = restore_dict.get("postgresql_version", 16)
+        s3_endpoint = secrets.get('s3_endpoint', "")
+        restore_cnpg_cluster(argocd.k8s,
+                             'nextcloud',
+                             nextcloud_namespace,
+                             pgsql_cluster_name,
+                             psql_version,
+                             s3_endpoint,
+                             pg_access_key_id,
+                             pg_secret_access_key,
+                             pgsql_cluster_name,
+                             cnpg_backup_schedule)
+
+    # then we begin the restic restore of all the nextcloud PVCs we lost
+    for pvc in ['files', 'config']:
+        pvc_enabled = secrets.get(f'{pvc}_pvc_enabled', 'false')
+        if pvc_enabled and pvc_enabled.lower() != 'false':
+            # creates the nexcloud pvc
+            recreate_pvc(argocd.k8s,
+                         'nextcloud',
+                         f'nextcloud-{pvc}',
+                         nextcloud_namespace,
+                         secrets[f'{pvc}_storage'],
+                         pvc_storage_class,
+                         secrets[f'{pvc}_access_mode'],
+                         "nextcloud-pvc"
+                         )
+
+            # restores the nextcloud pvc
+            k8up_restore_pvc(argocd.k8s,
+                             'nextcloud',
+                             f'nextcloud-{pvc}',
+                             'nextcloud',
+                             s3_backup_endpoint,
+                             s3_backup_bucket,
+                             access_key_id,
+                             secret_access_key,
+                             restic_repo_password,
+                             snapshot_ids[f'nextcloud_{pvc}']
+                             )
+
+    # todo: from here on out, this could be async to start on other tasks
+    # install nextcloud as usual, but wait on it this time
+    argocd.install_app('nextcloud', argo_dict, True)
+
+    # verify nextcloud rolled out completely, just in case
+    rollout = (f"kubectl rollout status -n {nextcloud_namespace} "
+               "deployment/nextcloud-web-app --watch --timeout 10m")
+    while True:
+        rolled_out = subproc([rollout], error_ok=True)
+        if "NotFound" not in rolled_out:
+            break
+
+    # try to update the maintenance mode of nextcloud to off
+    nextcloud_obj = Nextcloud(argocd.k8s, nextcloud_namespace)
+    nextcloud_obj.set_maintenance_mode("off")
+
+
+def setup_bitwarden_items(argocd: ArgoCD,
+                          nextcloud_hostname: str,
+                          s3_endpoint: str,
+                          s3_access_key: str,
+                          backups_s3_user: str,
+                          backups_s3_password: str,
+                          restic_repo_pass: str,
+                          admin_user: str,
+                          mail_host: str,
+                          mail_user: str,
+                          mail_pass: str,
+                          oidc_creds: dict,
+                          zitadel_hostname: str,
+                          bitwarden: BwCLI) -> None:
+    """
+    setup all the bitwarden items for nextcloud external secrets to be populated
+    """
+    sub_header("Creating Nextcloud items in Bitwarden")
+
+    # s3 credentials creation
+    bucket_obj = create_custom_field('bucket', "nextcloud-data")
+    endpoint_obj = create_custom_field('endpoint', s3_endpoint)
+    s3_id = bitwarden.create_login(
+            name='nextcloud-user-s3-credentials',
+            item_url=nextcloud_hostname,
+            user="nextcloud",
+            password=s3_access_key,
+            fields=[bucket_obj, endpoint_obj]
+            )
+
+    pgsql_s3_key = create_password()
+    s3_db_id = bitwarden.create_login(
+            name='nextcloud-postgres-s3-credentials',
+            item_url=nextcloud_hostname,
+            user="nextcloud-postgres",
+            password=pgsql_s3_key
+            )
+
+    admin_s3_key = create_password()
+    s3_admin_id = bitwarden.create_login(
+            name='nextcloud-admin-s3-credentials',
+            item_url=nextcloud_hostname,
+            user="nextcloud-root",
+            password=admin_s3_key
+            )
+
+    # credentials for remote backups of the s3 PVC
+    restic_repo_pass_obj = create_custom_field("resticRepoPassword", restic_repo_pass)
+    s3_backups_id = bitwarden.create_login(
+            name='nextcloud-backups-s3-credentials',
+            item_url=nextcloud_hostname,
+            user=backups_s3_user,
+            password=backups_s3_password,
+            fields=[restic_repo_pass_obj]
+            )
+
+    # oidc credentials if they were given, else they're probably already there
+    if oidc_creds:
+        log.debug("Creating OIDC credentials for Nextcloud in Bitwarden...")
+        issuer_obj = create_custom_field("issuer", f"https://{zitadel_hostname}")
+        oidc_id = bitwarden.create_login(
+                name='nextcloud-oidc-credentials',
+                item_url=nextcloud_hostname,
+                user=oidc_creds['client_id'],
+                password=oidc_creds['client_secret'],
+                fields=[issuer_obj]
+                )
+    else:
+        oidc_id = bitwarden.get_item(
+                f"nextcloud-oidc-credentials-{nextcloud_hostname}"
+                )[0]['id']
+
+    # admin credentials + metrics server info token
+    token = bitwarden.generate()
+    admin_password = bitwarden.generate()
+    serverinfo_token_obj = create_custom_field("serverInfoToken", token)
+    admin_id = bitwarden.create_login(
+            name='nextcloud-admin-credentials',
+            item_url=nextcloud_hostname,
+            user=admin_user,
+            password=admin_password,
+            fields=[serverinfo_token_obj]
+            )
+
+    # smtp credentials
+    smtpHost = create_custom_field("hostname", mail_host)
+    smtp_id = bitwarden.create_login(
+            name='nextcloud-smtp-credentials',
+            item_url=nextcloud_hostname,
+            user=mail_user,
+            password=mail_pass,
+            fields=[smtpHost]
+            )
+
+    # postgres db credentials creation
+    db_id = bitwarden.create_login(
+            name='nextcloud-pgsql-credentials',
+            item_url=nextcloud_hostname,
+            user='nextcloud',
+            password='we-dont-use-the-password-anymore-we-use-tls'
+            )
+
+    # redis credentials creation
+    nextcloud_redis_password = bitwarden.generate()
+    redis_id = bitwarden.create_login(
+            name='nextcloud-redis-credentials',
+            item_url=nextcloud_hostname,
+            user='nextcloud',
+            password=nextcloud_redis_password
+            )
+
+    # update the nextcloud values for the argocd appset
+    argocd.update_appset_secret(
+            {'nextcloud_admin_credentials_bitwarden_id': admin_id,
+             'nextcloud_oidc_credentials_bitwarden_id': oidc_id,
+             'nextcloud_smtp_credentials_bitwarden_id': smtp_id,
+             'nextcloud_postgres_credentials_bitwarden_id': db_id,
+             'nextcloud_redis_bitwarden_id': redis_id,
+             'nextcloud_s3_admin_credentials_bitwarden_id': s3_admin_id,
+             'nextcloud_s3_postgres_credentials_bitwarden_id': s3_db_id,
+             'nextcloud_s3_nextcloud_credentials_bitwarden_id': s3_id,
+             'nextcloud_s3_backups_credentials_bitwarden_id': s3_backups_id}
+            )
+
+
+def refresh_bweso(argocd: ArgoCD,
+                  nextcloud_hostname: str,
+                  bitwarden: BwCLI) -> None:
+    """
+    if bitwarden and init are enabled, but app is already installed, make sure
+    we populate appset secret plugin secret with nextcloud bitwarden item IDs
+    """
+    log.debug("Making sure nextcloud Bitwarden item IDs are in appset "
+              "secret plugin secret")
+    oidc_id = bitwarden.get_item(
+            f"nextcloud-oidc-credentials-{nextcloud_hostname}"
+            )[0]['id']
+
+    admin_id = bitwarden.get_item(
+            f"nextcloud-admin-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    smtp_id = bitwarden.get_item(
+            f"nextcloud-smtp-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    db_id = bitwarden.get_item(
+            f"nextcloud-pgsql-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    redis_id = bitwarden.get_item(
+            f"nextcloud-redis-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    s3_admin_id = bitwarden.get_item(
+            f"nextcloud-admin-s3-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    s3_db_id = bitwarden.get_item(
+            f"nextcloud-postgres-s3-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    s3_id = bitwarden.get_item(
+            f"nextcloud-user-s3-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    s3_backups_id = bitwarden.get_item(
+            f"nextcloud-backups-s3-credentials-{nextcloud_hostname}", False
+            )[0]['id']
+
+    argocd.update_appset_secret(
+            {'nextcloud_admin_credentials_bitwarden_id': admin_id,
+             'nextcloud_oidc_credentials_bitwarden_id': oidc_id,
+             'nextcloud_smtp_credentials_bitwarden_id': smtp_id,
+             'nextcloud_postgres_credentials_bitwarden_id': db_id,
+             'nextcloud_redis_bitwarden_id': redis_id,
+             'nextcloud_s3_admin_credentials_bitwarden_id': s3_admin_id,
+             'nextcloud_s3_postgres_credentials_bitwarden_id': s3_db_id,
+             'nextcloud_s3_nextcloud_credentials_bitwarden_id': s3_id,
+             'nextcloud_s3_backups_credentials_bitwarden_id': s3_backups_id
+            })
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
        Name: k3d
 DESCRIPTION: install k3d :D Not affiliated with k3s, rancher, or suse. just a fan
      AUTHOR: @Jessebot
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from ..utils.rich_cli.console_logging import sub_header
-from ..utils.subproc import subproc
+from ..utils.run.subproc import subproc
 from ..constants import XDG_CACHE_DIR
 import logging as log
 from yaml import dump
 
 
 # where we write this config
 K3D_CFG_FILENAME = f"{XDG_CACHE_DIR}/k3d-config.yaml"
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION: install k3s :D not affiliated with rancher, suse, or k3s
      AUTHOR: @Jessebot
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 # local libraries
 from ..constants import USER, KUBECONFIG
 from ..constants import XDG_CACHE_DIR
-from ..utils.subproc import subproc
+from ..utils.run.subproc import subproc
 
 # external libraries
 import logging as log
 from os import chmod, remove, path
 import requests
 import stat
 from ruamel.yaml import YAML
@@ -92,35 +92,56 @@
     k3s_cmd = ('\'curl -sfL https://get.k3s.io | '
                f'K3S_URL="https://{internal_ip}:6443" '
                f'K3S_TOKEN="{k3s_token}" sh -\'')
 
     # for each node and it's meta data, ssh in and join the node
     for node, metadata in extra_nodes.items():
         ssh_cmd = "ssh -o StrictHostKeyChecking=no "
+
+        # only add the port if it's not 22
+        ssh_port = metadata.get('ssh_port', '22')
+        if str(ssh_port) != "22":
+            ssh_cmd += f"-p {ssh_port} "
+        else:
+            ssh_cmd += f"{node} "
+
+        # only add the ssh key if it's not id_rsa
         ssh_key = metadata.get('ssh_key', 'id_rsa')
         if ssh_key != "id_rsa":
-            ssh_cmd += f"-i {metadata['ssh_key']} {node} "
+            ssh_cmd += f"-i {ssh_key} {node} "
         else:
             ssh_cmd += f"{node} "
 
         # join node to cluster
         subproc([ssh_cmd + k3s_cmd], shell=True, universal_newlines=True)
 
+
+        # check if we have taints or labels to apply to this new node
         labels = metadata.get('node_labels', None)
         taints = metadata.get('node_taints', None)
+        if labels or taints:
+            log.debug(f"Checking if {node} is ready for labeling and/or tainting.")
+
+            k_get_nodes = subproc(["kubectl get nodes"])
 
-        # after joining the node make sure the labels are up to date
-        if labels:
-            for label in labels:
-                subproc([f"kubectl label nodes {node} {label}"])
-
-        # after joining the node make sure the taints are up to date
-        if taints:
-            for taint in taints:
-                subproc([f"kubectl taint nodes {node} {taint}"], error_ok=True)
+            # if new node is not available, keep checking
+            while node not in k_get_nodes:
+                log.info(f"Waiting for {node} to be available")
+                sleep(1)
+                k_get_nodes = subproc(["kubectl get nodes"])
+
+            # apply labels to new node
+            if labels:
+                for label in labels:
+                    subproc([f"kubectl label nodes {node} {label}"])
+
+            # apply taints to new node
+            if taints:
+                for taint in taints:
+                    subproc([f"kubectl taint nodes {node} {taint}"])
 
 
 def uninstall_k3s(cluster_name: str) ->  str:
     """
     uninstall k3s and cleans up your kubeconfig as well
     returns True
     """
@@ -136,15 +157,15 @@
         return res.join('\n')
     else:
         return res
 
 
 def update_user_kubeconfig(cluster_name: str = 'smol-k8s-lab-k3s') -> None:
     """
-    update the user's kubeconfig with the cluster, user, and context for the new 
+    update the user's kubeconfig with the cluster, user, and context for the new
     cluster by grabbing the k3s generated kubeconfig and using it to update your
     current kubeconfig. Handles both existing kubeconfig and none at all.
 
     cluster_name: string - the name you'd like to give to the cluster and context
     """
     safe_yaml = YAML(typ='safe')
     yaml = YAML()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
        Name: kind
 DESCRIPTION: create or delete a kind cluster, part of smol-k8s-lab
      AUTHOR: <https://github.com/jessebot>
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from ..constants import XDG_CACHE_DIR
 from ..utils.rich_cli.console_logging import sub_header
-from ..utils.subproc import subproc
+from ..utils.run.subproc import subproc
 import logging as log
 from os import path
 from ruamel.yaml import YAML
 from ruamel.yaml.scalarstring import PreservedScalarString as pss
 from shutil import which
 from sys import exit
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/helm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """
 AUTHOR: @jessebot
 LICENSE: AGPLv4
 """
 
 # internal libraries
-from ..utils.subproc import subproc
+from ..utils.run.subproc import subproc
 from ..utils.rich_cli.console_logging import header, sub_header
 
 # external libraries
 from collections import OrderedDict
 import logging as log
 import requests
 from ruamel.yaml import YAML
@@ -17,15 +17,16 @@
 
 # these are the URLs of each manually installed helm chart, so that the appset matches
 APPSET_URLS = {
         "argo-cd": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/argocd/app_of_apps/argocd_appset.yaml",
         "appset-secret-plugin": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/argocd/app_of_apps/appset_secret_plugin/appset_secret_plugin_generator_argocd_app.yaml",
         "cert-manager": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/cert-manager/cert-manager_argocd_app.yaml",
         "ingress-nginx": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/ingress-nginx/ingress-nginx_argocd_app.yaml",
-        "cilium": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/alpha/cilium/cilium_argocd_appset.yaml"
+        "cilium": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/alpha/cilium/cilium_argocd_appset.yaml",
+        "cnpg-cluster": "https://raw.githubusercontent.com/small-hack/argocd-apps/main/nextcloud/app_of_apps/postgres_argocd_appset.yaml"
         }
 
 
 class Helm:
     """
     Local helm management of repos:
     use helm to add/remove/update repos and upgrade/(un)install charts
@@ -66,84 +67,94 @@
             """
             subproc([f'helm repo remove {self.repo_name}'])
 
     class chart:
         """
         installs/uninstalls a helm chart.
         """
-        def __init__(self, **kwargs):
-            """
-            Takes key word args:
-            release_name="", chart_name="", chart_version="", namespace="",
-            values_file="", set_options={}
+        def __init__(self,
+                     release_name: str = "",
+                     chart_name: str = "",
+                     chart_version: str = "",
+                     namespace: str = "default",
+                     values_file: str = "",
+                     set_options: dict = {}):
+            """
+            args:
+              - release_name:  str to call this installation
+              - chart_name:    str of helm chart to use (repo/chart)
+              - chart_version: version of the chart to install
+              - namespace:     str of namespace to deploy release to
+              - values_file:   str of a file to use with --values
+              - set_options:   dict of key/values to be passed with --set
+
             order of operations: values file followed by --set options.
             """
-            # for each keyword arg's key, create self.key for other methods
-            # to reference e.g. pass in namespace='kube-system' and we create
-            # self.namespace='kube-system'
-            self.__dict__.update(kwargs)
-
-            # always install into default namespace unless stated otherwise
-            if not kwargs['namespace']:
-                self.namespace = 'default'
+            self.release_name = release_name
+            self.chart_name = chart_name
+            self.chart_version = chart_version
+            self.namespace = namespace
+            self.values_file = values_file
+            self.set_options = set_options
 
         def check_existing(self,):
             """
             check if we already have an existing install
             """
             cmd = (f'helm list --short --filter {self.release_name} '
                    f' -n {self.namespace}')
             return subproc([cmd], quiet=True)
 
 
-        def install(self, wait: bool = False) -> True:
-            """
-            Installs helm chart to current k8s context, takes optional wait arg
-            Defaults to False, if True, will wait till deployments are up
-            keyword args:
-                - release_name:  str to call this installation
-                - chart_name:    str of helm chart to use (repo/chart)
-                - chart_version: version of the chart to install
-                - namespace:     str of namespace to deploy release to
-                - values_file:   str of a file to use with --values
-                - set_options:   dict of key/values to be passed with --set
-            """
-            if self.check_existing():
-                log.info(f"{self.release_name} is already installed :)")
-                return True
+        def install(self,
+                    wait: bool = False,
+                    upgrade: bool = False,
+                    ) -> True:
+            """
+            Installs helm chart to current k8s context, takes optional args:
+
+            - wait: bool default: False, if True, will wait till helm release stable
+            - upgrade: bool default: False, if True, will upgrade
+            """
+            if not upgrade:
+                if self.check_existing():
+                    log.info(f"{self.release_name} is already installed :)")
+                    return True
 
             cmd = (f'helm upgrade {self.release_name} {self.chart_name}'
                    f' --install -n {self.namespace} --create-namespace')
             # f' --atomic')
 
-            if self.__dict__.get('chart_version', False):
+            if self.chart_version:
                 cmd += f' --version {self.chart_version}'
             else:
                 version = self.get_appset_version()
                 cmd += f' --version {version}'
 
-            if self.__dict__.get('values_file', False):
+            if self.values_file:
                 cmd += f' --values {self.values_file}'
 
-            if self.__dict__.get('set_options', False):
+            if self.set_options:
                 for key, value in self.set_options.items():
                     cmd += f' --set {key}={value}'
 
             if wait:
                 cmd += ' --wait --wait-for-jobs'
 
             subproc([cmd])
-            return True
 
         def get_appset_version(self) -> str:
             """
             go get the version of the helm chart installed by the live appset
             """
             # get the contents of the remote url
-            res = requests.get(APPSET_URLS[self.release_name]).text
+            if "postgres-cluster" in self.release_name:
+                res = requests.get(APPSET_URLS['cnpg-cluster']).text
+            else:
+                res = requests.get(APPSET_URLS[self.release_name]).text
 
             # use the ruamel.yaml library to load the yaml
             yaml = YAML()
             obj = yaml.load(res)
 
             # this is an app
             if obj['kind'] == "Application":
@@ -161,14 +172,15 @@
             subproc([cmd])
             return True
 
 
 def add_default_repos(k8s_distro: str,
                       metallb: bool = False,
                       cilium: bool = False,
+                      cnpg_operator: bool = False,
                       argo: bool = False,
                       argo_secrets: bool = False) -> None:
     """
     Add all the default helm chart repos:
     - metallb is for loadbalancing and assigning ips, on metal...
     - cilium is for networking policy management
     - ingress-nginx allows us to do ingress, so access outside the cluster
@@ -184,14 +196,17 @@
     # cilium comes first, but may be skipped
     if cilium:
         repos['cilium'] = 'https://helm.cilium.io/'
 
     repos['ingress-nginx'] = 'https://kubernetes.github.io/ingress-nginx'
     repos['jetstack'] = 'https://charts.jetstack.io'
 
+    if cnpg_operator:
+        repos['cnpg-cluster'] = 'https://small-hack.github.io/cloudnative-pg-cluster-chart'
+
     if argo:
         repos['argo-cd'] = 'https://argoproj.github.io/argo-helm'
 
     if argo_secrets:
         repos['appset-secret-plugin'] = ('https://small-hack.github.io/'
                                          'appset-secret-plugin')
 
@@ -200,24 +215,25 @@
         repos.pop('ingress-nginx')
 
     # install and update any repos needed
     Helm.repo(repos).add()
 
 
 def prepare_helm(k8s_distro: str,
-                 argo: bool = False,
                  metallb: bool = True,
                  cilium: bool = False,
+                 cnpg_operator: bool = False,
+                 argo: bool = False,
                  argo_app_set: bool = False) -> bool:
     """
     get helm installed if needed, and then install/update all the helm repos
     """
     header("Adding/Updating helm repos...")
     if not which("helm"):
         msg = ("ʕ•́ᴥ•̀ʔ [b]Helm[/b] is [warn]not installed[/warn]. "
                "[i]We'll install it for you.[/i] ʕᵔᴥᵔʔ")
         sub_header(msg)
         subproc(['brew install helm'])
 
     # this is where we add all the helm repos we're going to use
-    add_default_repos(k8s_distro, metallb, cilium, argo, argo_app_set)
+    add_default_repos(k8s_distro, metallb, cilium, cnpg_operator, argo, argo_app_set)
     return True
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from base64 import standard_b64encode as b64enc
 from json import loads
 from kubernetes import client, config
 from kubernetes.client.rest import ApiException
 import logging as log
 from os import path
 from ruamel.yaml import YAML
+from time import sleep
 
 # internal libraries
 from ..constants import XDG_CACHE_DIR
-from ..utils.subproc import subproc, simple_loading_bar
+from ..utils.run.subproc import subproc, simple_loading_bar
 
 
 class K8s():
     """
     Class for the kubernetes python client
     """
 
@@ -56,26 +57,25 @@
             # V1Secret: kubernetes-client/python:kubernetes/docs/V1Secret.md
             body = client.V1Secret(metadata=meta, string_data=str_data)
 
         # output is pretty printed. (optional)
         pretty = True
 
         try:
-            res = self.core_v1_api.create_namespaced_secret(namespace, body,
-                                                            pretty=pretty)
-            log.debug(res)
+            self.core_v1_api.create_namespaced_secret(namespace, body,
+                                                      pretty=pretty)
         except ApiException as e:
             log.error("Exception when calling "
                       f"CoreV1Api->create_namespaced_secret: {e}")
 
             # delete the secret if it already exists
             try:
                 self.core_v1_api.delete_namespaced_secret(name, namespace)
-                res = self.core_v1_api.create_namespaced_secret(namespace, body,
-                                                                pretty=pretty)
+                self.core_v1_api.create_namespaced_secret(namespace, body,
+                                                          pretty=pretty)
             except ApiException as e:
                 log.error("Exception when calling "
                           f"CoreV1Api->create_namespaced_secret: {e}")
 
     def get_secret(self, name: str, namespace: str) -> dict:
         """
         get an existing k8s secret
@@ -90,14 +90,48 @@
         """
         get an existing k8s secret
         """
         log.debug(f"Deleting secret: {name} in namespace: {namespace}")
 
         subproc([f"kubectl delete secret -n {namespace} {name}"])
 
+    def get_nodes(self,) -> list|str:
+        """
+        get all nodes fo current cluster and returns them in a list
+        """
+        # todo: figure out how to parse this data
+        # node_list_sdk = self.core_v1_api.list_node()['items']
+        # print(node_list_sdk)
+
+        list_cmd = "kubectl get nodes --no-headers=true"
+
+        node_list_cmd = subproc([list_cmd]).rstrip().split('\n')
+        return node_list_cmd
+
+    def get_node(self, node: str) -> dict:
+        """
+        checks for specific node and returns info on it as a dict if it exists.
+        returns empty dict if node does not return any info
+        """
+        return_dict = {}
+        node_list_cmd = subproc([f"kubectl get node {node} --no-headers=true"],
+                                error_ok=True)
+
+        # provided there's no errors, create a dict of relevant info for the node
+        if "Error from server" not in node_list_cmd:
+            res = node_list_cmd.split()
+
+            return_dict["name"] = res[0]
+            return_dict["status"] = res[1]
+            return_dict["role"] = res[2]
+            return_dict["age"] = res[3]
+            return_dict["version"] = res[4]
+
+        return return_dict
+
     def get_namespace(self, name: str) -> bool:
         """
         checks for specific namespace and returns True if it exists,
         returns False if namespace does not exist
         """
         nameSpaceList = self.core_v1_api.list_namespace()
         for nameSpace_obj in nameSpaceList.items:
@@ -116,26 +150,62 @@
             meta = client.V1ObjectMeta(name=name)
             namespace = client.V1Namespace(metadata=meta)
 
             self.core_v1_api.create_namespace(namespace)
         else:
             log.debug(f"Namespace, {name}, already exists")
 
-    def reload_deployment(self, name: str, namespace: str) -> None:
+    def reload_deployment(self, name: str, namespace: str, replicas: int = 1) -> None:
         """
         restart a deployment's pod scaling it up and then down again
         currently only works with one pod
         """
-        # HACK: there's got to be a better way, but I don't have time to fix
-        subproc([
-            f"kubectl scale deploy -n {namespace} {name} --replicas=0",
-            "sleep 3",
-            f"kubectl scale deploy -n {namespace} {name} --replicas=1",
-            f"kubectl rollout status deployment -n {namespace} {name}"
-                 ])
+        # check the current pod name
+        pods = self.get_pod_names(name, namespace)
+        if pods:
+            pod_name = pods[0]
+
+        # scale deployment down
+        subproc([f"kubectl scale deploy -n {namespace} {name} --replicas=0",
+                 f"kubectl rollout status deployment -n {namespace} {name}"])
+
+        # make sure the old pod is gone
+        while True:
+            if not pod_name:
+                break
+            if pod_name not in self.get_pod_names(name, namespace):
+                break
+
+        # scale deployment back up
+        subproc([f"kubectl scale deploy -n {namespace} {name} --replicas={replicas}",
+                 f"kubectl rollout status deployment -n {namespace} {name}"])
+
+    def get_pod_names(self,
+                      name: str,
+                      namespace: str,
+                      extra_label: str = "") -> list:
+        """
+        get the pod name from a deployment or job based on the label
+        """
+        pod_cmd = (f"kubectl get pods -n {namespace} --no-headers"
+                   " -o custom-columns=NAME:.metadata.name"
+                   f" -l app.kubernetes.io/instance={name}")
+
+        if extra_label:
+            pod_cmd += "," + extra_label
+
+        pods = subproc([pod_cmd])
+
+        if pods:
+            if "\n" in pods:
+                return pods.split('\n')
+            else:
+                return [pods.strip()]
+        else:
+            return []
 
     # def create_from_manifest_dict(self,
     #                               api_group: str = "",
     #                               api_version: str = "",
     #                               namespace: str = "",
     #                               plural_obj_name: str = "",
     #                               manifest_dict: dict = {}) -> bool:
@@ -161,31 +231,35 @@
 
     def apply_manifests(self,
                         manifest_file_name: str,
                         namespace: str = "default",
                         deployment: str = "",
                         selector: str = "component=controller"):
         """
-        applies a manifest and waits with a nice loading bar if deployment
+        applies a manifest and waits with a nice loading bar if deployment name
+        is passed in
         """
-        cmds = [f"kubectl apply --wait -f {manifest_file_name}"]
+        if not namespace:
+            cmds = [f"kubectl apply --wait -f {manifest_file_name}"]
+        else:
+            cmds = [f"kubectl apply -n {namespace} --wait -f {manifest_file_name}"]
 
         if deployment:
             # these commands let us monitor a deployment rollout
             cmds.append(f"kubectl rollout status -n {namespace} "
                        f"deployment/{deployment}")
 
             cmds.append("kubectl wait --for=condition=ready pod --selector="
-                       f"{selector} --timeout=90s -n {namespace}")
+                       f"{selector} --timeout=5m -n {namespace}")
 
         # loops with progress bar until this succeeds
         subproc(cmds)
         return True
 
-    def apply_custom_resources(self, custom_resource_dict_list: dict):
+    def apply_custom_resources(self, custom_resource_dict_list: list[dict]):
         """
         Does a kube apply on a custom resource dict, and retries if it fails
         using loading bar for progress
         """
         k_cmd = 'kubectl apply --wait -f '
         commands = {}
         log.debug(custom_resource_dict_list)
@@ -237,22 +311,66 @@
         else:
             for key, updated_value in updated_values_dict.items():
                # update the keys in the secret yaml one by one
                secret_data[key] = b64enc(bytes(updated_value))
             self.delete_secret(secret_name, secret_namespace)
             self.create_secret(secret_name, secret_namespace, secret_data)
 
-    def run_k8s_cmd(self, pod_name: str, namespace: str, command: str,
+    def run_k8s_cmd(self,
+                    pod_name: str,
+                    namespace: str,
+                    command: str,
                     container: str = "") -> str:
-        """ 
+        """
         run a given command for a given pod in a given namespace and return the result
         """
         print(f"Running: '{command}' on pod: {pod_name} in container {container}"
               f" in namespace: {namespace}")
 
         run_dict = {'name': pod_name,
                     'namespace': namespace,
                     'command': command}
         if container:
             run_dict['container'] = container
 
         return self.core_v1_api.connect_get_namespaced_pod_exec(**run_dict)
+
+
+    def wait(self,
+             namespace: str,
+             name: str = "",
+             instance: str = "",
+             quiet: bool = False) -> str:
+        """
+        wait for a given deployment, statefulset, pod, or job to complete or be ready.
+        must pass in either name or instance args.
+
+        args:
+            namespace  - str, namespace of resource to wait on
+            name       - str, optional name of resource to wait on
+            instance   - str, optional value for app.kubernetes.io/instance label
+        """
+        wait_cmd = (
+                f'kubectl wait pod -n {namespace} --for=condition=ready --timeout=10m'
+                )
+
+        if instance:
+            wait_cmd += f" -l app.kubernetes.io/instance={instance}"
+        elif name:
+            wait_cmd += f" {name}"
+        else:
+            log.error("Expected [i]name[/i] or [i]instance[/i] for wait command")
+            return
+
+        # keep retrying till we find the thing...
+        while True:
+            if not quiet:
+                res = subproc([wait_cmd], error_ok=True)
+            else:
+                res = subproc([wait_cmd], error_ok=True, quiet=True)
+
+            if "no matching resources found" not in res:
+                log.info("found resource and waited on it")
+                return res
+            else:
+                log.debug("No matching resource found, waiting 3 seconds...")
+                sleep(3)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,171 +1,171 @@
 # smol-k8s-lab libraries
-from smol_k8s_lab.tui.util import (placeholder_grammar, create_sanitized_list)
+from smol_k8s_lab.tui.util import placeholder_grammar
 
 # external libraries
-from ruamel.yaml import CommentedSeq
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Grid, Horizontal
+from textual.containers import Grid, VerticalScroll
+from textual.screen import ModalScreen
 from textual.validation import Length
-from textual.widgets import Input, Label, Static, Collapsible, Button, Switch
+from textual.widgets import Button, Input, Label, Static
 
 
-class SmolK8sLabCollapsibleInputsWidget(Static):
+class ModifyAppGlobals(Static):
     """
-    widget for input fields for an app
-    for argocd that are passed to the argocd appset secrets plugin helm chart
+    tiny widget with a "modify globals" button to launch a modal screen to modify
+    globally available templating parameters for argocd that are passed to
+    the argocd appset secrets plugin helm chart
     """
-    BINDINGS = [Binding(key="b,escape,q",
-                        key_display="b",
-                        action="app.pop_screen",
-                        description="Back")]
-
-    def __init__(self,
-                 app_name: str,
-                 title: str,
-                 collapsible_id: str,
-                 inputs: dict = {},
-                 tooltips: dict = {},
-                 sensitive_inputs: bool = False,
-                 add_fields_button: bool = False) -> None:
-
-        self.app_name = app_name
-        self.title = title
-        self.inputs = inputs
-        self.sensitive = sensitive_inputs
-        self.tooltips = tooltips
-        self.add_fields_button = add_fields_button
-        self.collapsible_id = collapsible_id
+    def compose(self) -> ComposeResult:
+        with Grid(classes="button-grid"):
+            button = Button("✏️  Modify Globals", id="modify-globals-button")
+            button.tooltip = (
+                    "Modify globally available Argo CD ApplicationSet templating values"
+                    )
+            yield button
 
-        super().__init__()
+    def on_button_pressed(self):
+        self.app.push_screen(ModifyAppGlobalsScreen())
 
-    def compose(self) -> ComposeResult:
-        with Collapsible(collapsed=False, title=self.title, id=self.collapsible_id):
-            with Grid(classes="collapsible-updateable-grid"):
-                if self.inputs:
-                    for key, value in self.inputs.items():
-                        yield self.generate_row(key, value)
 
-    def on_mount(self) -> None:
-        """
-        update the grid for all new inputs
-        """
-        if self.add_fields_button:
-            self.query_one(".collapsible-updateable-grid").mount(
-                    Button("➕ new field"))
-
-    def generate_row(self, key: str, value: str | bool) -> Grid | Horizontal:
-        # if key == 'create_minio_tenant':
-        #     return self.generate_switch_row(key, value)
-        return self.generate_input_row(key, value)
-
-    def generate_switch_row(self, key: str, value: bool) -> Horizontal:
-        tooltip = "enable the use of a local minio tenant using the minio operator"
-        switch = Switch(value=value,
-                        classes="bool-switch-row-switch",
-                        name=key,
-                        id=f"{self.app_name}-minio-tenant")
-        switch.tooltip = tooltip
+class ModifyAppGlobalsScreen(ModalScreen):
+    """
+    modal screen with inputs to modify globally available templating parameters
+    for argocd that are passed to the argocd appset secrets plugin helm chart
+    """
+    CSS_PATH = ["../css/base_modal.tcss",
+                "../css/modify_globals_modal.tcss"]
+    BINDINGS = [
+            Binding(key="b,escape,q",
+                    key_display="b",
+                    action="app.pop_screen",
+                    description="Back"),
+            Binding(key="f5",
+                    key_display="f5",
+                    description="Speak",
+                    action="app.speak_element",
+                    show=True)
+            ]
 
-        bool_label = Label("Create MinIO tenant:", classes="argo-config-label")
-        bool_label.tooltip = tooltip
+    def __init__(self) -> None:
+        self.global_params = self.app.cfg["apps_global_config"]
+        super().__init__()
 
-        return Horizontal(bool_label, switch, classes="argo-switch-row")
+    def compose(self) -> ComposeResult:
+        # base screen grid
+        question = ("[#ffaff9]Modify[/] [i]globally[/] available Argo CD ApplicationSet"
+                    " [#C1FF87]templating values[/].")
+
+        with Grid(id="modify-globals-modal-screen"):
+            # grid for app question and buttons
+            with Grid(id="modify-globals-question-box"):
+                yield Label(question, id="modal-text")
+
+                yield VerticalScroll(id="scroll-container-for-globals")
+
+                key_input = Input(placeholder="new key name",
+                                  id="new-secret",
+                                  classes="new-secret-input",
+                                  validators=Length(minimum=2))
+
+                key_input.tooltip = ("🔒key name to pass to the Argo CD ApplicationSet"
+                                     " Secret Plugin Generator for templating non-"
+                                     "sensitive values such as hostnames.")
+
+                add_button = Button("➕", id="new-secret-button",
+                                    classes="new-secret-button")
+                add_button.tooltip = (
+                        "After the input to the right is valid, click to add a "
+                        "new global parameter for all Argo CD ApplicationSets")
+                add_button.disabled = True
+
+                with Grid(classes="app-input-row", id="new-row"):
+                    yield add_button
+                    yield key_input
+
+    def on_mount(self,):
+        if self.global_params:
+            scroll_container = self.get_widget_by_id("scroll-container-for-globals")
+            # iterate through the app's secret keys
+            for secret_key, value in self.global_params.items():
+                scroll_container.mount(self.generate_secret_key_row(secret_key, value))
+
+        question_box = self.get_widget_by_id("modify-globals-question-box")
+        question_box.border_subtitle = "[@click=app.pop_screen]close[/]"
+
+        self.call_after_refresh(self.app.play_screen_audio, screen="modify_globals")
+
+    def generate_secret_key_row(self,
+                                secret_key: str,
+                                value: str = "",
+                                new: bool = False) -> Grid:
+        """
+        add a new row of secret keys to pass to an argocd app
+        if new param is set to True, we also write it to the yaml
+        """
+        if new:
+            self.app.cfg['apps_global_config'][secret_key] = value
+            self.app.write_yaml()
 
-    def generate_input_row(self, key: str, value: str = "") -> Grid:
-        """
-        add a new row of keys to pass to an argocd app
-        """
-        key_label = key.replace("_", " ")
+        key_label = secret_key.replace("_", " ")
 
         # create input
-        placeholder_txt = placeholder_grammar(key_label)
-        input_keys = {"placeholder": placeholder_txt,
-                      "name": key,
-                      "password": self.sensitive,
-                      "id": "-".join([self.app_name, key, "input"]),
+        input_keys = {"placeholder": placeholder_grammar(key_label),
+                      "classes": "app-secret-key-input",
+                      "name": secret_key,
+                      "id": secret_key,
                       "validators": [Length(minimum=2)]}
 
-        # only give an initial value if one was found in the yaml or env var
         if value:
-            # handle ruamel commented sequence (dict from yaml with comments)
-            if isinstance(value, CommentedSeq) or isinstance(value, list):
-                if isinstance(value[0], str):
-                    sequence_value = ", ".join(value)
-
-                elif isinstance(value[0], list):
-                    # we grab value[0] because ruamel.yaml's CommentedSeq is weird
-                    sequence_value = ", ".join(value[0])
+            input_keys['value'] = value
 
-                # reassign value if this is a CommentedSeq for validation later on
-                value = sequence_value
-
-            input_keys["value"] = value
-
-        # add all the input_keys dictionary as args to Input widget
         input = Input(**input_keys)
+        input.validate(value)
 
-        # make sure Input widget has a tooltip
-        tooltip = self.tooltips.get(key, None)
-        if not tooltip:
-            if self.sensitive:
-                env_var = "_".join([self.app_name.upper(), key.upper()])
-                tooltip = (f"To avoid needing to fill in this value manually, you"
-                           f" can export ${env_var} as an environment variable.")
-            else:
-                if key == "s3_provider":
-                    tooltip = "Choose between minio and seaweedfs for a local s3 provider"
-                else:
-                    tooltip = placeholder_txt + "."
-
-        # special metallb tooltip
-        if self.app_name == "metallb":
-            tooltip += (" Be sure the ip addresses you enter already have DNS "
-                        "entries for any apps you'd like to deploy.")
-
-        input.tooltip = tooltip
+        # create the input row
+        secret_label = Label(f"{key_label}:", classes="input-label")
 
-        # immediately validate to get a pink border if input value is invalid
-        input.validate(value)
+        return Grid(secret_label, input, classes="app-input-row")
 
-        # create and return the Label + Input row
-        return Grid(Label(f"{key_label}:", classes="input-label"),
-                    input,
-                    classes="app-input-row")
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        """
+        add a new input row for secret stuff
+        """
+        if event.button.id == "new-secret-button":
+            inputs_box = self.get_widget_by_id("scroll-container-for-globals")
+            input = self.get_widget_by_id("new-secret")
+
+            # add new secret key row
+            inputs_box.mount(
+                    self.generate_secret_key_row(input.value, "", True)
+                    )
+            # clear the input field after we're created the new row and
+            # updated the yaml
+            input.value = ""
 
     @on(Input.Changed)
     def input_validation(self, event: Input.Changed) -> None:
-        if event.validation_result.is_valid:
-            input = event.input
-            if self.sensitive:
-                self.app.sensitive_values[self.app_name][input.name] = input.value
+        if event.input.id == "new-secret":
+            if event.validation_result.is_valid:
+                self.get_widget_by_id("new-secret-button").disabled = False
             else:
-                parent_yaml = self.app.cfg['apps'][self.app_name]['init']['values']
-
-                if event.validation_result.is_valid:
-                    if self.app_name in ["metallb", "vouch"] or "," in input.value:
-                        parent_yaml[input.name] = create_sanitized_list(input.value)
-                    else:
-                        parent_yaml[input.name] = input.value
+                if self.app.cfg['smol_k8s_lab']['tui']['accessibility']['bell']['on_error']:
+                    self.app.bell()
+                # if result is not valid, notify the user why
+                self.notify("\n".join(event.validation_result.failure_descriptions),
+                            severity="warning",
+                            title="⚠️ Input Validation Error\n")
 
-                    self.app.write_yaml()
+                self.get_widget_by_id("new-secret-button").disabled = True
         else:
-            if self.app.bell_on_error:
-                self.app.bell()
-            # if result is not valid, notify the user why
-            self.notify("\n".join(event.validation_result.failure_descriptions),
-                        severity="warning",
-                        title="⚠️ Input Validation Error\n")
-
-    @on(Switch.Changed)
-    def update_base_yaml_for_switch(self, event: Switch.Changed) -> None:
-        """
-        if user changes a boolean init value, we write that out
-        """
-        truthy = event.value
-        self.app.cfg['apps'][self.app_name]['init'][event.switch.name] = truthy
-        self.app.write_yaml()
-
-        if truthy and event.switch.name == "create_minio_tenant":
-            self.app.notify("💡Make sure Argo CD directory recursion is switched on.")
+            if event.validation_result.is_valid:
+                self.app.cfg['apps_global_config'][event.input.name] = event.input.value
+                self.app.write_yaml()
+            else:
+                if self.app.bell_on_error:
+                    self.app.bell()
+                # if result is not valid, notify the user why
+                self.notify("\n".join(event.validation_result.failure_descriptions),
+                            severity="warning",
+                            title="⚠️ Input Validation Error\n")
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,108 @@
 #!/usr/bin/env python3.11
 # external libraries
 from rich.text import Text
 from textual import on
 from textual.binding import Binding
 from textual.app import ComposeResult
 from textual.containers import Grid
-from textual.screen import Screen
-from textual.widgets import DataTable, Footer, Label
+from textual.screen import ModalScreen
+from textual.widgets import DataTable, Footer
 
 
-class InvalidAppsScreen(Screen):
+class InvalidAppsModalScreen(ModalScreen):
     """
     Textual app to show all invalid apps
     """
     CSS_PATH = ["../css/invalid_apps.tcss"]
 
     BINDINGS = [Binding(key="b,q,escape",
                         key_display="b",
                         action="app.pop_screen",
                         description="⬅️ Back"),
+                Binding(key="f5",
+                        key_display="f5",
+                        description="Speak",
+                        action="app.speak_element",
+                        show=True),
                 Binding(key="n",
                         show=False,
                         action="app.bell")]
 
     def __init__(self, invalid_apps: dict) -> None:
         """
-        takes config: dict, should be the entire smol-k8s-lab config.yaml
+        takes invalid apps dict
         """
         self.show_footer = self.app.cfg['smol_k8s_lab']['tui']['show_footer']
         self.invalid_apps = invalid_apps
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
-        Compose app with tabbed content.
+        Compose footer and base grid with datatable
         """
         # Footer to show keys unless the footer is disabled globally
         footer = Footer()
         if not self.show_footer:
             footer.display = False
         yield footer
 
-        # warning label if there's invalid apps
-        warning_label = Label(
-                "\nClick the app links below to fix the errors or disable them.",
-                classes="help-text"
-                )
-        yield Grid(warning_label, id="invalid-apps")
+        # table in grid to be used for invalid apps
+        data_table = DataTable(zebra_stripes=True,
+                               id="invalid-apps-table",
+                               cursor_type="row")
+        yield Grid(data_table, id="invalid-apps")
 
     def on_mount(self) -> None:
         # invalid apps error title styling
         invalid_box = self.get_widget_by_id("invalid-apps")
         border_title = "⚠️ The following app fields are empty"
         invalid_box.border_title = border_title
+        subtitle = "Click the app links above to fix the errors or disable them"
+        invalid_box.border_subtitle = subtitle
 
-        if self.app.speak_screen_titles:
-            self.app.action_say("Screen title: " + border_title)
+        self.call_after_refresh(self.app.play_screen_audio,
+                                screen="invalid_apps")
 
         self.build_pretty_nope_table()
 
     def build_pretty_nope_table(self) -> None:
         """
         No, but with flare ✨
 
-        This is just a grid of apps to update if a user leaves a field blank
+        This is where we populate the DataTable with all the apps to update.
+        If a user leaves a field blank it contains an invalid fields column
+        for all the fields you need to fix
         """
-        nope_container = self.get_widget_by_id("invalid-apps")
-
-        data_table = DataTable(zebra_stripes=True,
-                               id="invalid-apps-table",
-                               cursor_type="row")
+        data_table = self.get_widget_by_id("invalid-apps-table")
 
         # then fill in the cluster table
         data_table.add_column(Text("Application", justify="center"))
         data_table.add_column(Text("Invalid Fields"))
 
         for app, fields in self.invalid_apps.items():
-            # we use an extra line to center the rows vertically 
+            # we use an extra line to center the rows vertically
             styled_row = [
                     Text(str("\n" + app)),
                     Text(str("\n" + ", ".join(fields)))
                           ]
 
             # we add extra height to make the rows more readable
             data_table.add_row(*styled_row, height=3, key=app)
 
-        nope_container.mount(Grid(data_table, id="invalid-apps-table-row"))
+        # immediately set the focus to this data table
+        self.app.set_focus(data_table)
 
     @on(DataTable.RowSelected)
     def app_row_selected(self, event: DataTable.RowSelected) -> None:
         """
-        check which row was selected to launch a app config screen for app 
+        check which row was selected to launch a app config screen for app
         """
         row_index = event.cursor_row
         row = event.data_table.get_row_at(row_index)
 
-        # get the row's first column (app) and remove whitespace
-        app = row[0].plain.strip()
-
-        # try to launch the app screen for the given app again
-        self.app.action_request_apps_cfg(app)
+        # get the row's first column (app) and remove whitespace, and then
+        # do the same for second column, only just grab the first invalid field
+        return_app_field = (row[0].plain.strip(),
+                            row[1].plain.strip().split(", ")[0])
+        # go back to the app screen and scroll to the selected app and field
+        self.dismiss(return_app_field)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,167 +1,165 @@
 # smol-k8s-lab libraries
-from smol_k8s_lab.tui.util import placeholder_grammar
+from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_distros.k3d import delete_k3d_cluster
+from smol_k8s_lab.k8s_distros.k3s import uninstall_k3s
+from smol_k8s_lab.k8s_distros.kind import delete_kind_cluster
+from smol_k8s_lab.utils.run.subproc import subproc
 
 # external libraries
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Grid, VerticalScroll
+from textual.containers import Grid
 from textual.screen import ModalScreen
-from textual.validation import Length
-from textual.widgets import Button, Input, Label, Static
+from textual.widgets import Button, Label
+from textual.widgets.data_table import RowKey
 
-                    
-class ModifyAppGlobals(Static):
-    """
-    tiny widget with a "modify globals" button to launch a modal screen to modify
-    globally available templating parameters for argocd that are passed to
-    the argocd appset secrets plugin helm chart
-    """
-    def compose(self) -> ComposeResult:
-        with Grid(classes="button-grid"):
-            button = Button("✏️  Modify Globals", id="modify-globals")
-            button.tooltip = (
-                    "Modify globally available Argo CD ApplicationSet templating values"
-                    )
-            yield button
-
-    def on_button_pressed(self):
-        self.app.push_screen(ModifyAppGlobalsScreen())
 
-
-class ModifyAppGlobalsScreen(ModalScreen):
+class ClusterModalScreen(ModalScreen):
     """
-    modal screen with inputs to modify globally available templating parameters 
-    for argocd that are passed to the argocd appset secrets plugin helm chart
+    A simple textual modal screen for asking a user what they'd like to do with
+    their cluster.
+
+    Includes a few buttons for launching apps screen, edit nodes screen, and
+    deleting clusters.
     """
-    CSS_PATH = ["../css/base_modal.tcss",
-                "../css/modify_globals_modal.tcss"]
-    BINDINGS = [Binding(key="b,escape,q",
-                        key_display="b",
-                        action="app.pop_screen",
-                        description="Back")]
+    CSS_PATH = ["../css/cluster_modal.tcss"]
+    BINDINGS = [
+            Binding(key="b,escape,q",
+                    key_display="b",
+                    action="cancel_button",
+                    description="Back"),
+            Binding(key="f5",
+                    key_display="f5",
+                    description="Speak",
+                    action="app.speak_element",
+                    show=True)
+            ]
+
+    def __init__(self, cluster: str, distro: str, row_key: RowKey) -> None:
+        self.cluster = cluster
+        self.distro = distro
+        self.row_key = row_key
+        # keep the current context in memory in case the user cancels
+        self.start_current_context = subproc(["kubectl config current-context"],
+                                             spinner=False, quiet=True)
+
+        # set the context to the current cluster so we can operate on it
+        subproc([f"kubectl config use-context {self.cluster}"], spinner=False,
+                quiet=True)
+        self.k8s_ctx = K8s()
 
-    def __init__(self) -> None:
-        self.global_params = self.app.cfg["apps_global_config"]
         super().__init__()
 
     def compose(self) -> ComposeResult:
+
+        question = ('What would you like to do with '
+                    f'[#C1FF87]{self.cluster}[/]?')
         # base screen grid
-        question = ("[#ffaff9]Modify[/] [i]globally[/] available Argo CD ApplicationSet"
-                    " [#C1FF87]templating values[/].")
+        with Grid(id="cluster-question-modal-screen", classes="modify-delete-size"):
+            # grid for cluster question and buttons
+            with Grid(id="cluster-question-box"):
+                yield Label(question, id="cluster-modal-text")
+
+                with Grid(id="modal-button-box"):
+                    # modify button allows user to change apps (and soon distro details)
+                    modify_apps_button = Button("✏️  Modify Apps",
+                                                id="modify-apps-button")
+                    modify_apps_button.tooltip = "Modify the cluster's Applications"
+                    yield modify_apps_button
+
+                    if self.distro == "k3s":
+                        # modify button allows user to change nodes
+                        modify_nodes_button = Button("🖥️ Modify Nodes",
+                                                     id="modify-nodes-button")
+                        modify_nodes_button.tooltip = "Modify the cluster's nodes"
+                        yield modify_nodes_button
+
+                    # delete button deletes the cluster
+                    delete_button = Button("🚮 Delete", id="delete-cluster-first-try")
+                    delete_button.tooltip = "[#ffaff9]Delete[/] the existing cluster 😱"
+                    # we can only delete the following k8s distro types
+                    if self.distro not in ["kind", "k3d", "k3s"]:
+                        delete_button.disabled = False
+                    yield delete_button
 
-        with Grid(id="modify-globals-modal-screen"):
-            # grid for app question and buttons
-            with Grid(id="modify-globals-question-box"):
-                yield Label(question, id="modal-text")
-
-                yield VerticalScroll(id="scroll-container")
-
-                key_input = Input(placeholder="new key name",
-                                  id="new-secret",
-                                  classes="new-secret-input",
-                                  validators=Length(minimum=2))
-
-                key_input.tooltip = ("🔒key name to pass to the Argo CD ApplicationSet"
-                                     " Secret Plugin Generator for templating non-"
-                                     "sensitive values such as hostnames.")
-
-                add_button = Button("➕", id="new-secret-button",
-                                    classes="new-secret-button")
-                add_button.tooltip = (
-                        "After the input to the right is valid, click to add a "
-                        "new global parameter for all Argo CD ApplicationSets")
-                add_button.disabled = True
-
-                with Grid(classes="app-input-row", id="new-row"):
-                    yield add_button
-                    yield key_input
-
-    def on_mount(self,):
-        if self.global_params:
-            scroll_container = self.get_widget_by_id("scroll-container")
-            # iterate through the app's secret keys
-            for secret_key, value in self.global_params.items():
-                scroll_container.mount(self.generate_secret_key_row(secret_key, value))
-
-        question_box = self.get_widget_by_id("modify-globals-question-box")
-        question_box.border_subtitle = "[@click=app.pop_screen]close[/]"
-
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say("Screen title: Modify globally available Argo CD"
-                                " ApplicationSet templating values. You can press "
-                                "escape to close this modal screen.")
-
-    def generate_secret_key_row(self,
-                                secret_key: str,
-                                value: str = "",
-                                new: bool = False) -> Grid:
+    def on_mount(self):
         """
-        add a new row of secret keys to pass to an argocd app
-        if new param is set to True, we also write it to the yaml
+        say the title if that self.app.speak_screen_titles is set to True
         """
-        if new:
-            self.app.cfg['apps_global_config'][secret_key] = value
-            self.app.write_yaml()
+        question_box = self.get_widget_by_id("cluster-question-box")
+        question_box.border_subtitle = "[@click=screen.cancel_button]cancel[/]"
 
-        key_label = secret_key.replace("_", " ")
+        self.call_after_refresh(self.app.play_screen_audio, screen="cluster_modal")
 
-        # create input
-        input_keys = {"placeholder": placeholder_grammar(key_label),
-                      "classes": "app-secret-key-input",
-                      "name": secret_key,
-                      "validators": [Length(minimum=2)]}
+    def action_cancel_button(self):
+        subproc([f"kubectl config use-context {self.start_current_context}"])
+        self.app.pop_screen()
+
+    @on(Button.Pressed)
+    def button_pressed(self, event: Button.Pressed) -> None:
+        if event.button.id == "modify-apps-button":
+            # call the apps page for this cluster
+            self.app.action_request_apps_cfg(app_to_highlight="",
+                                             modify_cluster=True)
+
+        elif event.button.id == "modify-nodes-button":
+            # call the nodes page for this cluster
+            self.app.action_request_nodes_cfg(self.distro, True)
+
+        elif event.button.id == "delete-cluster-first-try":
+            # don't display the first delete button or the modify button
+            event.button.display = False
+            self.get_widget_by_id("modify-apps-button").display = False
+
+            # are you sure, the text
+            confirm_txt = ('Are you [b][i]sure[/][/] you want to [#ffaff9]delete[/]'
+                           f' [#C1FF87]{self.cluster}[/]?')
+            self.get_widget_by_id("cluster-modal-text").update(confirm_txt)
+            self.app.play_screen_audio(screen="cluster_modal", alt=True, say_title=False)
+
+            # are you sure, the button
+            sure_button = Button("🚮 Yes", id="delete-button-second-try")
+            self.get_widget_by_id("modal-button-box").mount(sure_button)
+
+            nope_button = Button("😱 No", id="nope-button")
+            self.get_widget_by_id("modal-button-box").mount(nope_button)
+
+        # if the user really wants to delete a cluster, we do it
+        elif event.button.id == "delete-button-second-try":
+            if self.distro == "k3s":
+                res = uninstall_k3s(self.cluster)
+                self.app.notify(res)
+
+            if self.distro == "k3d":
+                res = delete_k3d_cluster(self.cluster)
+                if "Success" in res:
+                    self.app.notify("Sucessfully deleted cluster",
+                                    severity="information")
+                else:
+                    if self.app.bell_on_error:
+                        self.app.bell()
+                    self.app.notify("Something went wrong with deleting the cluster!",
+                                    timeout=10,
+                                    severity="error")
+
+            if self.distro == "kind":
+                delete_kind_cluster(self.cluster.replace("kind-", ""))
+
+            # after deleting pop the screen
+            self.dismiss([self.cluster, self.row_key])
+
+        elif event.button.id == "nope-button":
+            # resets the modal
+            delete_2nd_try = self.get_widget_by_id("delete-button-second-try")
+            delete_2nd_try.display = False
+            nope = self.get_widget_by_id("nope-button")
+            nope.display = False
+
+            self.get_widget_by_id("modify-apps-button").display = True
+
+            question = f'What would you like to do with [#C1FF87]{self.cluster}[/]?'
+            self.get_widget_by_id("cluster-modal-text").update(question)
+            self.app.play_screen_audio("cluster_modal")
 
-        if value:
-            input_keys['value'] = value
-
-        input = Input(**input_keys)
-        input.validate(value)
-
-        # create the input row
-        secret_label = Label(f"{key_label}:", classes="input-label")
-
-        return Grid(secret_label, input, classes="app-input-row")
-
-    def on_button_pressed(self, event: Button.Pressed) -> None:
-        """
-        add a new input row for secret stuff
-        """
-        if event.button.id == "new-secret-button":
-            inputs_box = self.get_widget_by_id("scroll-container")
-            input = self.get_widget_by_id("new-secret")
-
-            # add new secret key row
-            inputs_box.mount(
-                    self.generate_secret_key_row(input.value, "", True)
-                    )
-            # clear the input field after we're created the new row and
-            # updated the yaml
-            input.value = ""
-
-    @on(Input.Changed)
-    def input_validation(self, event: Input.Changed) -> None:
-        if event.input.id == "new-secret":
-            if event.validation_result.is_valid:
-                self.get_widget_by_id("new-secret-button").disabled = False
-            else:
-                if self.app.bell_on_error:
-                    self.app.bell()
-                # if result is not valid, notify the user why
-                self.notify("\n".join(event.validation_result.failure_descriptions),
-                            severity="warning",
-                            title="⚠️ Input Validation Error\n")
-
-                self.get_widget_by_id("new-secret-button").disabled = True
-        else:
-            if event.validation_result.is_valid:
-                self.app.cfg['apps_global_config'][event.input.name] = event.input.value
-                self.app.write_yaml()
-            else:
-                if self.app.bell_on_error:
-                    self.app.bell()
-                # if result is not valid, notify the user why
-                self.notify("\n".join(event.validation_result.failure_descriptions),
-                            severity="warning",
-                            title="⚠️ Input Validation Error\n")
+            self.get_widget_by_id("delete-cluster-first-try").display = True
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 
 class NewAppModalScreen(ModalScreen):
     CSS_PATH = ["../css/base_modal.tcss",
                 "../css/new_app_modal.tcss"]
     BINDINGS = [Binding(key="b,escape,q",
                         key_display="b",
                         action="app.pop_screen",
-                        description="Back")]
-
+                        description="Back"),
+            Binding(key="f5",
+                    key_display="f5",
+                    description="Speak",
+                    action="app.speak_element",
+                    show=True)]
 
     def __init__(self, current_apps: list = []) -> None:
         self.current_apps = current_apps
         super().__init__()
 
     def compose(self) -> ComposeResult:
         # base screen grid
@@ -46,25 +50,21 @@
                 desc_input.tooltip = desc_placeholder + " to be displayed in the UI."
                 yield desc_input
 
                 with Grid(id="modal-button-box"):
                     submit = Button("submit", id="app-submit")
                     submit.tooltip = "submit name of new Argo CD Application"
                     submit.disabled = True
-                    yield submit 
+                    yield submit
 
     def on_mount(self) -> None:
         box = self.get_widget_by_id("question-box")
         box.border_subtitle = "[@click=app.pop_screen]cancel[/]"
 
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say("Screen title: Please enter a name and description"
-                                " for your Argo CD Application. You can press "
-                                "escape to close this modal screen")
+        self.call_after_refresh(self.app.play_screen_audio, screen="new_app")
 
     @on(Input.Changed)
     def input_validation(self, event: Input.Changed) -> None:
         if event.input.id == "app-name-input":
             if event.validation_result.is_valid:
                 # if result is valid, enable the submit button
                 self.get_widget_by_id("app-submit").disabled = False
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/apps_screen.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,403 +1,190 @@
+#!/usr/bin/env python3.11
 # smol-k8s-lab libraries
-from smol_k8s_lab.constants import INITIAL_USR_CONFIG, XDG_CONFIG_FILE
-from smol_k8s_lab.k8s_distros import check_all_contexts
-from smol_k8s_lab.tui.apps_screen import AppsConfig
-from smol_k8s_lab.tui.base_cluster_modal import ClusterModalScreen
-from smol_k8s_lab.tui.confirm_screen import ConfirmConfig
-from smol_k8s_lab.tui.distro_screen import DistroConfigScreen
-from smol_k8s_lab.tui.help_screen import HelpScreen
-from smol_k8s_lab.tui.app_widgets.invalid_apps import InvalidAppsScreen
-from smol_k8s_lab.tui.smol_k8s_config_screen import SmolK8sLabConfig
-from smol_k8s_lab.tui.tui_config_screen import TuiConfigScreen
-from smol_k8s_lab.tui.validators.already_exists import CheckIfNameAlreadyInUse
+from smol_k8s_lab.utils.run.subproc import subproc
+from smol_k8s_lab.k8s_tools.k8s_lib import K8s
+from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
+from smol_k8s_lab.tui.app_widgets.invalid_apps import InvalidAppsModalScreen
+from smol_k8s_lab.tui.app_widgets.app_inputs_confg import AppInputs
+from smol_k8s_lab.tui.app_widgets.new_app_modal import NewAppModalScreen
+from smol_k8s_lab.tui.app_widgets.modify_globals import ModifyAppGlobals
+from smol_k8s_lab.tui.util import format_description
 
 # external libraries
-from os import environ, system
-from pyfiglet import Figlet
-import random
-from rich.text import Text
-from ruamel.yaml import YAML
-from textual import on
-from textual.app import App, ComposeResult
-from textual.events import DescendantFocus
+from kubernetes.config import ConfigException
+from os import environ
+from textual import on, work
+from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Grid
-from textual.validation import Length
-from textual.widgets import (Footer, Button, DataTable, Input, Static, Label,
-                             Switch, Select, _collapsible)
-
-# list of approved words for nouns
-CUTE_NOUNS = [
-        "bunny", "hoglet", "puppy", "kitten", "knuffel", "friend", "egel",
-        "meerkoet", "raccoon", "wasbeertje"
-        ]
-
-CUTE_ADJECTIVE = [
-        "lovely", "adorable", "cute", "friendly", "nice", "leuke", "mooie",
-        "vriendelijke", "cool", "soft", "smol", "small", "klein"
-        ]
+from textual.containers import VerticalScroll, Container, Grid
+from textual.css.query import NoMatches
+from textual.screen import Screen
+from textual.widgets import Footer, Header, Label, SelectionList
+from textual.widgets._toggle_button import ToggleButton
+from textual.widgets.selection_list import Selection
+
+
+class AppsConfigScreen(Screen):
+    """
+    Textual screen to display smol-k8s-lab applications for configuring
+    """
+    CSS_PATH = ["./css/apps_config.tcss",
+                "./css/apps_init_config.tcss"]
 
-class BaseApp(App):
     BINDINGS = [
-            Binding(key="?,h",
-                    key_display="?",
-                    action="request_help",
-                    description="Help",
-                    show=True),
-            Binding(key="c",
-                    key_display="c",
-                    action="request_config",
-                    description="Config"),
-            Binding(key="f",
-                    key_display="f",
-                    action="toggle_footer",
-                    description="Hide footer"),
-            Binding(key="q,escape",
-                    action="quit",
-                    show=False),
-            Binding(key="f5",
-                    key_display="f5",
-                    description="Speak",
-                    action="app.say",
-                    show=True),
+            Binding(key="b,escape,q",
+                    key_display="b",
+                    action="app.pop_screen",
+                    description="Back"),
+            Binding(key="a",
+                    key_display="a",
+                    action="screen.launch_new_app_modal",
+                    description="New App"),
             Binding(key="n",
                     key_display="n",
-                    description="New Cluster",
-                    action="app.new_cluster",
-                    show=True)
+                    action="screen.try_next_screen",
+                    description="Next")
             ]
 
-    CSS_PATH = ["./css/base.tcss",
-                "./css/help.tcss"]
+    ToggleButton.BUTTON_INNER = '♥'
+
+    def __init__(self,
+                 config: dict,
+                 highlighted_app: str = "",
+                 modify_cluster: bool = False) -> None:
+        # show the footer at bottom of screen or not
+        self.show_footer = self.app.cfg['smol_k8s_lab']['tui']['show_footer']
+
+        # should be the apps section of smol k8s lab config
+        self.cfg = config
+
+        # if this is an active cluster or not
+        self.modify_cluster = modify_cluster
+
+        if self.modify_cluster:
+            argo_namespace = self.cfg['argo_cd']['argo']['namespace']
+            subproc(['kubectl config set-context --current --namespace='
+                     f'{argo_namespace}'])
+
+            try:
+                k8s_obj = K8s()
+            except ConfigException:
+                self.log("hmph, we don't have a cluster yet...")
+                k8s_obj = None
+
+            self.argocd = ArgoCD(self.cfg['argo_cd']['argo']['namespace'],
+                                 self.cfg['argo_cd']['argo']['secret_keys']['hostname'],
+                                 k8s_obj)
 
-    def __init__(self, user_config: dict = INITIAL_USR_CONFIG) -> None:
-        self.cfg = user_config
-        self.show_footer = self.cfg['smol_k8s_lab']['tui']['show_footer']
-        self.cluster_names = []
-        self.current_cluster = ""
+        # this is state storage
+        self.previous_app = ''
+
+        # inital highlight if we got here via a link
+        self.initial_app = highlighted_app
+
+        # sensitive values we are prepared to take so far
         self.sensitive_values = {
                 'cert_manager': {},
                 'nextcloud': {},
                 'home_assistant': {},
                 'matrix': {},
                 'mastodon': {},
                 'postgres_operator': {},
                 'zitadel': {}
                 }
 
-        # configure global accessibility
-        accessibility_opts = self.cfg['smol_k8s_lab']['tui']['accessibility']
-        tts = accessibility_opts['text_to_speech']
-        self.speak_on_focus = tts['on_focus']
-        self.speak_screen_titles = tts['screen_titles']
-        self.speak_on_key_press = tts['on_key_press']
-        self.speech_program = tts['speech_program']
-        self.bell_on_focus = accessibility_opts['bell']['on_focus']
-        self.bell_on_error = accessibility_opts['bell']['on_error']
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
-        Compose app with screens
+        Compose app with for app input content
         """
+        # header to be cute
+        yield Header()
+
         # Footer to show keys
         footer = Footer()
-
         if not self.show_footer:
             footer.display = False
         yield footer
 
-        # full screen container
-        with Grid(id="base-screen-container"):
-            yield Label(Figlet(font="standard").renderText("smol-k8s-lab"),
-                        id="smol-k8s-lab-header")
-
-            with Grid(id="cluster-boxes"):
-                # the actual little box in the middle of screen
-                with Grid(id="base-new-cluster-input-box-grid"):
-                    # container for new cluster buton
-                    with Grid(id="cluster-input-row"):
-                        yield NewClusterInput()
+        with Container(id="apps-config-container"):
+            # top left: the SelectionList of k8s applications
+            with Grid(id="left-apps-container"):
+                yield SelectionList[str](id='selection-list-of-apps')
+                yield Grid(ModifyAppGlobals(), id="left-button-box")
+
+            # top right: vertically scrolling container for all inputs
+            yield VerticalScroll(id='app-config-pane')
+
+            # Bottom half of the screen for select-apps
+            with VerticalScroll(id="app-notes-container"):
+                yield Label("", id="app-description")
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        # main box title
-        title = "[#ffaff9]Create[/] a [i]new[/] [#C1FF87]cluster[/] with the name below"
-        self.get_widget_by_id("base-new-cluster-input-box-grid").border_title = title
-
-        # get all clusters
-        clusters = check_all_contexts()
-
-        if clusters:
-            self.generate_cluster_table(clusters)
-            if self.speak_screen_titles:
-                self.action_say("Welcome to smol-k8s-lab. Press c to configure "
-                                "accessibility options.")
+        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
+        sub_title = f"Apps Configuration for {self.app.current_cluster} (now with more 🦑)"
+        self.sub_title = sub_title
+
+        self.generate_app_selection_list()
+
+        # if text to speech is on, read screen title
+        self.call_after_refresh(self.app.play_screen_audio, screen="apps")
+
+        # scroll down to specific app if requested
+        if self.initial_app:
+            self.scroll_to_app(self.initial_app)
         else:
-            self.get_widget_by_id("base-screen-container").add_class("no-cluster-table")
-            if self.speak_screen_titles:
-                self.action_say("Welcome to smol-k8s-lab. Press tab, then C, to configure "
-                                "accessibility options.")
-
-
-    def generate_cluster_table(self, clusters: list) -> None:
-        """
-        generate a readable table for all the clusters.
-
-        Each row is has a height of 3 and is centered to make it easier to read
-        for people with dyslexia
-        """
-        data_table = DataTable(zebra_stripes=True,
-                               id="clusters-data-table",
-                               cursor_type="row")
-
-        # then fill in the cluster table
-        data_table.add_column(Text("Cluster", justify="center"))
-        data_table.add_column(Text("Distro", justify="center"))
-
-        for row in clusters:
-            # we use an extra line to center the rows vertically
-            styled_row = [Text(str("\n" + cell), justify="center") for cell in row]
-
-            # we add extra height to make the rows more readable
-            data_table.add_row(*styled_row, height=3, key=row[0])
-
-            self.cluster_names.append(row[0])
+            self.update_highlighted_app_view("argo_cd")
 
-        # grid for the cluster data table
-        table_grid = Grid(data_table,
-                          id="table-grid")
-
-        # the actual little box in the middle of screen
-        main_grid = Grid(table_grid, id="base-cluster-table-box-grid")
-
-        # modify clusters box title
-        main_grid.border_title = ("Select a row to [#ffaff9]modify[/] or [#ffaff9]"
-                                  "delete[/] an [i]existing[/] [#C1FF87]cluster[/]")
-
-        cluster_container = self.get_widget_by_id("cluster-boxes")
-        self.get_widget_by_id("base-screen-container").add_class("with-cluster-table")
-        cluster_container.mount(main_grid, before="#base-new-cluster-input-box-grid")
-
-
-    @on(DataTable.RowSelected)
-    def cluster_row_selected(self, event: DataTable.RowSelected) -> None:
+    def generate_app_selection_list(self) -> None:
         """
-        check which row was selected to launch a modal screen
+        populate the selection list and modify global button for apps screen
         """
-        if event.data_table.id == "clusters-data-table":
-            def check_if_cluster_deleted(response: list = []):
-                """
-                check if cluster has been deleted
-                """
-                cluster = response[0]
-                row_key = response[1]
-
-                # make sure we actually got anything, because the user may have hit
-                # the cancel button
-                if cluster and row_key:
-                    data_table = self.query_one(DataTable)
-                    data_table.remove_row(row_key)
-
-                    self.cluster_names.remove(cluster)
-                    self.current_cluster = ""
-
-                    if data_table.row_count < 1:
-                        self.get_widget_by_id("base-cluster-table-box-grid").remove()
-                        screen = self.get_widget_by_id("base-screen-container")
-                        screen.remove_class("with-cluster-table")
-                        screen.add_class("no-cluster-table")
-            row_index = event.cursor_row
-            row = event.data_table.get_row_at(row_index)
-
-            # get the row's first column (the name of the cluster) and remove whitespace
-            cluster_name = row[0].plain.strip()
-            distro = row[1].plain.strip()
+        app_list = self.get_widget_by_id("selection-list-of-apps")
 
-            # set the current cluster name to return after we've done modifications
-            self.current_cluster = cluster_name
+        for app, app_meta in self.cfg.items():
+            item = Selection(app.replace("_","-"), app, app_meta['enabled'])
+            app_list.add_option(item)
 
-            # launch modal UI to ask if they'd like to modify or delete a cluster
-            self.app.push_screen(ClusterModalScreen(cluster_name,
-                                                    distro,
-                                                    event.row_key),
-                                 check_if_cluster_deleted)
+        app_list.border_title = "[#ffaff9]♥[/] [i]select[/] [#C1FF87]apps"
+        app_list.border_subtitle = (
+                "[@click=screen.launch_new_app_modal]✨ [i]new[/] "
+                "[#C1FF87]app[/][/]"
+                )
 
-    @on(DataTable.RowHighlighted)
-    def cluster_row_highlighted(self, event: DataTable.RowHighlighted) -> None:
+    def action_try_next_screen(self) -> None:
         """
-        check which row was selected to launch a modal screen
-        """
-        if self.app.speak_on_focus:
-            self.say_row(event.data_table)
-
-    def action_new_cluster(self):
-        """
-        press button for new cluster
-        """
-        new_cluster_button = self.get_widget_by_id("new-cluster-button")
-        if not new_cluster_button.disabled:
-            new_cluster_button.action_press()
+        verify all the apps fields are valid, and if not, launch a warning
+        modal screen and don't allow continue to next screen
 
-    def action_request_apps_cfg(self,
-                                app_to_highlight: str = "",
-                                modify_cluster: bool = False) -> None:
-        """
-        launches the argo app config screen
-        """
-        self.app.push_screen(AppsConfig(self.cfg['apps'],
-                                        app_to_highlight,
-                                        modify_cluster))
-
-    def action_request_distro_cfg(self) -> None:
-        """
-        launches the k8s distro (k3s,k3d,kind) config screen
+        if all apps fields are valid, try to launch the smol_k8s_cfg screen
         """
-        self.app.push_screen(DistroConfigScreen(self.cfg['k8s_distros']))
+        def check_invalid_apps(app_field_tuple: tuple = None):
+            """
+            process the app we get back scroll to it
+            """
+            if app_field_tuple:
+                app = app_field_tuple[0]
+                # field = app_field[1]
+                self.scroll_to_app(app)
 
-    def action_request_smol_k8s_cfg(self) -> None:
-        """
-        launches the smol-k8s-lab config for the program itself for things like
-        the TUI, but also logging and password management
-        """
         # go check all the apps for empty inputs
-        invalid_apps = self.check_for_invalid_inputs(self.cfg['apps'])
+        invalid_apps = self.check_for_invalid_inputs(self.app.cfg['apps'])
 
         if invalid_apps:
-            self.app.push_screen(InvalidAppsScreen(invalid_apps))
-        else:
-            self.app.push_screen(SmolK8sLabConfig(self.cfg['smol_k8s_lab']))
-
-    def action_request_confirm(self) -> None:
-        """
-        show confirmation screen
-        """
-        self.app.push_screen(ConfirmConfig(self.cfg))
-
-    def action_request_help(self,) -> None:
-        """
-        if the user presses 'h' or '?', show the help modal screen
-        """
-        self.push_screen(HelpScreen())
-
-    def action_request_config(self,) -> None:
-        """
-        if the user pressed 'c', show the TUI config screen
-        """
-        self.push_screen(TuiConfigScreen(self.cfg['smol_k8s_lab']['tui']))
-
-    def action_toggle_footer(self) -> None:
-        """
-        don't display the footer, or do 🤷
-        """
-        footer = self.query_one(Footer)
-
-        if footer.display:
-            footer.display = False
-            self.notify(
-                "\n✨ Press [gold3]f[/] to re-enable the footer",
-                timeout=9,
-                title="Footer disabled"
-            )
-            self.cfg['smol_k8s_lab']['tui']['show_footer'] = False
+            self.app.push_screen(InvalidAppsModalScreen(invalid_apps),
+                                 check_invalid_apps)
         else:
-            footer.display = True
-            self.cfg['smol_k8s_lab']['tui']['show_footer'] = True
-
-    def write_yaml(self, config_file: str = XDG_CONFIG_FILE) -> None:
-        """
-        dump current self.cfg to user's smol-k8s-lab config.yaml
-        """
-        yaml = YAML()
-
-        with open(config_file, 'w') as smol_k8s_config:
-            yaml.dump(self.cfg, smol_k8s_config)
-
-    def action_say(self, text_for_speech: str = "") -> None:
-        """
-        Use the configured speech program to read a string aloud. If no string
-        is passed in, and self.speak_on_key_press is True, we read the currently
-        focused element id
-        """
-        say = self.speech_program
-        if text_for_speech:
-            text_for_speech = text_for_speech.replace("(", "").replace(")", "")
-            text_for_speech = text_for_speech.replace("[i]", "").replace("[/]", "")
-            system(f"{say} {text_for_speech}")
-
-        elif not text_for_speech:
-            # if the use pressed f5, the key to read the widget id aloud
-            if self.speak_on_key_press:
-                focused = self.app.focused
-                if isinstance(focused, _collapsible.CollapsibleTitle):
-                    system(f"{say} element is a Collapsible called {focused.label}.")
-                else:
-                    system(f"{say} element is {focused.id}")
-
-                # if it's a data table, read out the row content
-                if isinstance(focused, DataTable):
-                    self.say_row(focused)
-
-    def say_row(self, data_table: DataTable) -> None:
-        """
-        get the column names and row content of a DataTable and read aloud
-        """
-        row_index = data_table.cursor_row
-        row = data_table.get_row_at(row_index)
-        # get the row's first column and remove whitespace
-        row_column1 = row[0].plain.strip()
-        # change ? to question mark so it reads aloud well
-        if row_column1 == "?":
-            row_column1 = "question mark"
-        row_column2 = row[1].plain.strip()
-
-        # get the column names
-        columns = list(data_table.columns.values())
-        column1 = columns[0].label
-        column2 = columns[1].label
-
-        system(f"{self.speech_program} Selected {column1}: {row_column1}."
-               f" {column2}: {row_column2}")
-
-    @on(DescendantFocus)
-    def on_focus(self, event: DescendantFocus) -> None:
-        """
-        on focus, say the id of each element and the value or label if possible
-        """
-        if self.speak_on_focus:
-            id = event.widget.id
-            self.action_say(f"element is {id}")
-
-            # input fields
-            if isinstance(event.widget, Input):
-                content = event.widget.value
-                placeholder = event.widget.placeholder
-                if content:
-                    self.action_say(f"value is {content}")
-                elif placeholder:
-                    self.action_say(f"place holder text is {placeholder}")
-
-            # buttons
-            elif isinstance(event.widget, Button):
-                self.action_say(f"button text is {event.widget.label}")
-
-            # switches
-            elif isinstance(event.widget, Switch) or isinstance(event.widget, Select):
-                self.action_say(f"value is {event.widget.value}")
-
-            # also read the tooltip if there is one
-            tooltip = event.widget.tooltip
-            if tooltip:
-                self.action_say(f"tooltip is {tooltip}")
-
-        if self.bell_on_focus:
-            self.app.bell()
+            # save our sensitive values temporarily at the app level
+            self.app.sensitive_values = self.sensitive_values
+            self.app.action_request_smol_k8s_cfg()
 
     def check_for_invalid_inputs(self, apps_dict: dict = {}) -> list:
         """
         check each app for any empty init or secret key fields
         """
         invalid_apps = {}
 
@@ -475,74 +262,196 @@
                     # append any missing values to prompt_values
                     prompt_values.append(item.lower())
 
                 self.sensitive_values[app][item.lower()] = value
 
         return set(prompt_values)
 
+    def action_launch_new_app_modal(self) -> None:
+        """
+        action bound to a key for adding a new app to launch the new app modal
+        screen.
+        """
+        def create_new_app_in_yaml(app_response):
+            """
+            after the new app modal screen is closed, if they didn't click cancel
+            it returns the name of the app and description for us to create a new
+            app in the yaml with.
+            """
+            app_name = app_response[0]
+            app_description = app_response[1]
+
+            if app_name and app_description:
+                underscore_name = app_name.replace(" ", "_").replace("-", "_")
+
+                # updates the base user yaml
+                self.app.cfg['apps'][underscore_name] = {
+                    "enabled": True,
+                    "description": app_description,
+                    "argo": {
+                        "secret_keys": {},
+                        "repo": "",
+                        "path": "",
+                        "revision": "",
+                        "namespace": "",
+                        "directory_recursion": False,
+                        "project": {
+                            "source_repos": [""],
+                            "destination": {
+                                "namespaces": ["argocd"]
+                                }
+                            }
+                        }
+                    }
+
+                # adds selection to the app selection list
+                apps = self.app.get_widget_by_id("selection-list-of-apps")
+                apps.add_option(Selection(underscore_name.replace("_", "-"),
+                                          underscore_name, True))
+
+                # scroll down to the new app
+                apps.action_last()
+
+        self.app.push_screen(NewAppModalScreen(["argo-cd"]),
+                             create_new_app_in_yaml)
+
+    def scroll_to_app(self, app_to_highlight: str) -> None:
+        """
+        lets you scroll down to the exact app you need in the app selection list
+        """
+        # get the apps selection list
+        apps = self.query_one(SelectionList)
+
+        # get the app name for the highlighted index
+        highlight_app = apps.get_option_at_index(apps.highlighted).value
+
+        # while the highlighted app is not app_to_highlight, keep scrolling
+        while highlight_app != app_to_highlight:
+            apps.action_cursor_down()
+            highlight_app = apps.get_option_at_index(apps.highlighted).value
+
+    @on(SelectionList.SelectionHighlighted)
+    def capture_selection_highlighted_event(self) -> None:
+        selection_list = self.query_one(SelectionList)
 
-class NewClusterInput(Static):
-    """
-    small widget with an input and button that takes the names of a cluster,
-    and changes the
-    """
-    def compose(self) -> ComposeResult:
-        with Grid(id="new-cluster-button-container"):
-            input = Input(validators=[
-                              Length(minimum=2),
-                              CheckIfNameAlreadyInUse(self.app.cluster_names)
-                              ],
-                          placeholder="Name of your new cluster",
-                          id="cluster-name-input")
-            input.tooltip = ("Name of your ✨ [i]new[/] cluster. Note: The k8s distro"
-                             " (selected on the next screen) will be pre-pended to the "
-                             "name of the cluster by default.")
-            yield input
-
-            new_button = Button("✨ New Cluster", id="new-cluster-button")
-            new_button.tooltip = "Add a new cluster managed by smol-k8s-lab"
-            yield new_button
+        # only the highlighted index
+        highlighted_idx = selection_list.highlighted
 
-    def on_mount(self) -> None:
-        input = self.get_widget_by_id("cluster-name-input")
-        input.value = random.choice(CUTE_ADJECTIVE) + '-' + random.choice(CUTE_NOUNS)
+        # the actual highlighted app
+        highlighted_app = selection_list.get_option_at_index(highlighted_idx).value
 
-    @on(Input.Changed)
-    @on(Input.Submitted)
-    def input_validation(self, event: Input.Changed | Input.Submitted) -> None:
-        """
-        Takes events matching Input.Changed and Input.Submitted events, and
-        checks if input is valid. If the user presses enter (Input.Submitted),
-        and the input is valid, we also press the button for them.
-        """
-        new_cluster_button = self.get_widget_by_id("new-cluster-button")
-
-        if event.validation_result.is_valid:
-            # if result is valid, enable the submit button
-            new_cluster_button.disabled = False
-
-            # if the user pressed enter, we also press the submit button ✨
-            if isinstance(event, Input.Submitted):
-                new_cluster_button.action_press()
-        else:
-            # if result is not valid, notify the user why
-            self.notify("\n".join(event.validation_result.failure_descriptions),
-                        timeout=8,
-                        severity="warning",
-                        title="⚠️ Input Validation Error\n")
+        if self.app.speak_on_focus:
+            self.app.action_say(f"highlighted app is {highlighted_app}")
 
-            # and disable the submit button
-            new_cluster_button.disabled = True
+        self.update_highlighted_app_view(highlighted_app)
 
-    @on(Button.Pressed)
-    def button_pressed(self, event: Button.Pressed) -> None:
-        """
-        get pressed button (Button.Pressed event) and change current screen to
-        the k8s distro config screen
-        """
-        self.app.current_cluster = self.get_widget_by_id("cluster-name-input").value
-        self.app.action_request_distro_cfg()
+    def update_highlighted_app_view(self, highlighted_app: str) -> None:
+        # update the bottom app description to the highlighted_app's description
+        blurb = format_description(self.cfg[highlighted_app]['description'])
+        self.get_widget_by_id('app-description').update(blurb)
+
+        # styling for the select-apps - configure apps container - right
+        app_title = highlighted_app.replace("_", " ").title()
+        app_cfg_title = f"🔧 [i]configure[/] parameters for [#C1FF87]{app_title}"
+        app_inputs_pane = self.get_widget_by_id("app-config-pane")
+        app_inputs_pane.border_title = app_cfg_title
+
+        if self.previous_app != "":
+            app_input = self.get_widget_by_id(f"{self.previous_app}-app-widget")
+            app_input.display = False
+
+        try:
+            app_input = self.get_widget_by_id(f"{highlighted_app}-app-widget")
+            app_input.display = True
+        except NoMatches:
+            app_metadata = self.cfg[highlighted_app]
+            app_input = AppInputs(highlighted_app, app_metadata,
+                                  id=f"{highlighted_app}-app-widget")
+
+            self.get_widget_by_id("app-config-pane").mount(app_input)
+
+        # select-apps styling - bottom
+        app_desc = self.get_widget_by_id("app-notes-container")
+        app_desc.border_title = f"📓 {app_title} [i]notes[/i]"
+
+        self.previous_app = highlighted_app
+
+        self.update_border_buttons(app_inputs_pane, highlighted_app)
+
+    @work(group="check-app-exists-workers")
+    async def update_border_buttons(self, app_inputs_pane, app) -> None:
+        # verify app is actually in Argo CD
+        if self.modify_cluster:
+            if self.argocd.check_if_app_exists(app):
+                self.log(f"Displaying sync and delete buttons for {self.previous_app}")
+                app_inputs_pane.border_subtitle = (
+                        "[@click=screen.sync_argocd_app]🔁 sync[/] / "
+                        "[@click=screen.delete_argocd_app]🗑️ delete[/]"
+                        )
+            else:
+                app_inputs_pane.border_subtitle = ""
+
+    def action_sync_argocd_app(self) -> None:
+        """
+        syncs an existing Argo CD application
+        """
+        app = self.previous_app.replace("_","-")
+
+        # sync the app
+        self.log(f"♻️ Syncing {app} via the TUI...")
+        res = self.argocd.sync_app(app, spinner=False)
+
+        if res:
+            severity = "information"
+            if isinstance(res, list):
+                response = "\n".join(res)
+            else:
+                response = res
+        else:
+            response = "No response recieved from Argo CD sync app... 🤔"
+            severity = "warning"
+
+        # if result is not valid, notify the user why
+        self.notify(response,
+                    timeout=10,
+                    severity=severity,
+                    title=f"🦑 Argo CD Sync [#87ff89]{self.previous_app}[/] Response\n")
+
+    def action_delete_argocd_app(self) -> None:
+        """
+        deletes an existing Argo CD application
+        """
+        app = self.previous_app.replace("_","-")
+
+        # sync the app
+        self.log(f"🗑️  Deleting {app} via the TUI...")
+        res = self.argocd.delete_app(app, spinner=False)
+
+        if res:
+            severity = "information"
+            if isinstance(res, list):
+                response = "\n".join(res)
+            else:
+                response = res
+        else:
+            response = "No response recieved from Argo CD delete app... 🤔"
+            severity = "warning"
 
+        # if result is not valid, notify the user why
+        self.notify(response,
+                    timeout=10,
+                    severity=severity,
+                    title=f"🦑 Argo CD Delete [#87ff89]{self.previous_app}[/] Response\n")
+
+    @on(SelectionList.SelectionToggled)
+    def update_selected_apps(self, event: SelectionList.SelectionToggled) -> None:
+        """
+        when a selection list item is checked or unchecked, update the base app yaml
+        """
+        selection_list = self.query_one(SelectionList)
+        app = selection_list.get_option_at_index(event.selection_index).value
+        if app in selection_list.selected:
+            self.app.cfg['apps'][app]['enabled'] = True
+        else:
+            self.app.cfg['apps'][app]['enabled'] = False
 
-if __name__ == "__main__":
-    app = BaseApp()
-    app.run()
+        self.app.write_yaml()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/confirm_screen.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,51 +58,53 @@
         yield footer
 
         with Grid(id="confirm-container"):
             # Add the TabbedContent widget different config sections
             with TabbedContent(initial="smol-k8s-lab-cfg", id="confirm-tabbed"):
                 # tab 1 - smol-k8s-lab
                 with TabPane("Core Config", id="smol-k8s-lab-cfg"):
-                    with VerticalScroll(classes="pretty-yaml-scroll-container"):
+                    with VerticalScroll(classes="pretty-yaml-scroll-container",
+                                        id="smol-k8s-lab-cfg-scrolling-container"):
                         yield Label("", id="pretty-yaml-smol-k8s-lab")
 
                 # tab 2 - k8s_distros
                 with TabPane("K8s Distro Config", id="k8s-distro-cfg"):
-                    with VerticalScroll(classes="pretty-yaml-scroll-container"):
+                    with VerticalScroll(classes="pretty-yaml-scroll-container",
+                                        id="pretty-yaml-scrolling-container"):
                         yield Label("", id="pretty-yaml-k8s-distro")
 
                 # tab 3 - apps
                 with TabPane("Apps Config", id="apps-cfg"):
-                    with VerticalScroll(classes="pretty-yaml-scroll-container"):
+                    with VerticalScroll(classes="pretty-yaml-scroll-container",
+                                        id="pretty-yaml-scrolling-container"):
                         yield Label("", id="pretty-yaml-apps")
 
                 # tab 3 - apps
                 with TabPane("Global Parameters Config", id="global-apps-cfg"):
-                    with VerticalScroll(classes="pretty-yaml-scroll-container"):
+                    with VerticalScroll(classes="pretty-yaml-scroll-container",
+                                        id="pretty-yaml-scrolling-container"):
                         yield Label("", id="pretty-yaml-global-apps")
 
         # final confirmation button before running smol-k8s-lab
         with Grid(id="final-confirm-button-box"):
             confirm = Button("🚊 Let's roll!", id="confirm-button")
             yield confirm
 
             back = Button("✋Go Back", id="back-button")
             yield back
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
-        sub_title = "Review your configuration (last step!)"
+        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
+        sub_title = f"Review your configuration for {self.app.current_cluster} (last step!)"
         self.sub_title = sub_title
 
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say("Screen title: Review your configuration last step")
+        self.call_after_refresh(self.app.play_screen_audio, screen="confirm")
 
         # confirm box title styling
         confirm_box = self.query_one(TabbedContent)
         confirm_box.border_title = "[i]Review[/] [i]All[/i] [#C1FF87]Values"
 
         # display the current user yaml
         smol_highlighted = syntax_highlighted_yaml({'smol_k8s_lab': self.smol_k8s_cfg})
@@ -183,22 +185,26 @@
         confirm button, we exit the TUI with the final confirmed config dict
 
         If the button is the back-button, we just pop the screen, which goes back
         to the main menu screen.
         """
         if event.button.id == "confirm-button":
             # First, check if we need bitwarden credentials before proceeding
-            pw_mngr = self.smol_k8s_cfg['local_password_manager']
+
+            # check if external secrets provider is enabled and set to use bitwarden
             secrets_provider = self.cfg['apps_global_config']['external_secrets']
-            
+            external_secrets = self.cfg['apps']['external_secrets_operator']['enabled']
+            secrets_provider_bitwarden = external_secrets and secrets_provider == 'bitwarden'
+
             # if local_password_manager is enabled, and is bitwarden
-            local_bitwarden = pw_mngr['enabled'] and pw_mngr['name'] == "bitwarden"
+            pw_mngr = self.smol_k8s_cfg['local_password_manager']
+            pw_mngr_bitwarden = pw_mngr['enabled'] and pw_mngr['name'] == "bitwarden"
 
             # if local password manager is bitwarden/enabled or we're using bweso
-            if local_bitwarden or secrets_provider == 'bitwarden':
+            if pw_mngr_bitwarden or secrets_provider_bitwarden:
                 self.get_bitwarden_credentials()
             else:
                 self.append_sensitive_values()
                 self.app.exit([self.app.current_cluster, self.cfg, None])
 
         if event.button.id == "back-button":
             self.app.pop_screen()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files 20% similar despite different names*

```diff
@@ -10,38 +10,69 @@
 $sky_blue: rgb(92,201,253);
 $cornflower: rgb(95,135,255);
 $light_cornflower: rgb(122,162,247);
 $blue_gray: rgb(86,95,137);
 $dark_gray: rgb(58,58,58);
 $navy: rgb(35,35,54);
 
+/* not sure if this is in use */
+#new-node-button {
+    margin-left: 10;
+}
+
 /* number of nodes box */
 #add-nodes-box {
     background: $navy 60%;
     padding-left: 1;
-    grid-rows: 0.9fr 0.1fr 0.55fr;
+    padding-right: 1;
     align: center middle;
     content-align: center middle;
 }
 
+/* rows for full widget or screen for modifying nodes */
+.add-nodes-box-widget {
+    grid-rows: 0.8fr 0.1fr 0.6fr;
+}
+
+.add-nodes-box-full-screen {
+    grid-rows: 0.9fr 0.15fr 0.6fr;
+}
+
+/* not in use */
 #nodes-data-table {
 }
 
-#nodes-tab {
+#nodes-tab-nodes-widget {
     width: auto;
     height: auto;
 }
 
-#new-node-text {
+/* add new node header */
+.new-node-text-full-screen {
+    background: $dark_gray 80%;
+    width: 100%;
+    color: $light_cornflower;
+    height: 3;
+    content-align: center middle;
+}
+
+.new-node-text-widget {
     background: $dark_gray 80%;
     width: 100%;
     color: $light_cornflower;
 }
 
+/* input fields below the new node header */
 .k3s-node-input-row {
     grid-size: 2;
-    grid-gutter: 1;
+    grid-gutter: 0 2;
 }
 
-#new-node-button {
-    margin-left: 10;
+.k3s-node-input-row .input-row-label {
+    width: 100%;
+}
+
+.input-row-equal {
+    layout: grid;
+    grid-size: 2;
+    grid-columns: 0.4fr 1fr;
 }
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files 26% similar despite different names*

```diff
@@ -34,78 +34,109 @@
 
 /* --------- LEFT TOP HALF OF SCREEN ------------ */
 
 #selection-list-of-apps {
     scrollbar-background: $dark_gray;
     scrollbar-background-active: $dark_gray;
     scrollbar-background-hover: $dark_gray;
-    scrollbar-color-active: $sky_blue;
     scrollbar-color-hover: $light_cornflower;
     scrollbar-color: $cornflower;
-}
-
-#selection-list-of-apps:focus {
-    border: round $light_cornflower
-}
-
-/* matches only the left hand side of top half of screen */
-#select-add-apps {
+    padding-top: 1;
+    padding-bottom: 1;
+    padding-left: 0;
+    padding-right: 0;
     border: round $cornflower;
     border-title-color: $sky_blue;
     border-subtitle-color: $sky_blue;
     link-background-hover: $navy;
     link-color-hover: $orange;
     background: $navy 60%;
-    align: center top;
-    height: auto;
-    scrollbar-background: $dark_gray;
-    scrollbar-background-active: $dark_gray;
-    scrollbar-background-hover: $dark_gray;
-    scrollbar-color-active: $sky_blue;
-    scrollbar-color-hover: $light_cornflower;
-    scrollbar-color: $cornflower;
 }
 
-/* matches the app selection list, the left button container */
+#selection-list-of-apps:focus {
+    border: round $light_cornflower
+}
+
+/* matches the app selection list and the left button container */
 #left-apps-container {
     grid-rows: 1fr 0.2fr;
     align: center top;
     grid-gutter: 1;
-    scrollbar-background: $dark_gray;
-    scrollbar-background-active: $dark_gray;
-    scrollbar-background-hover: $dark_gray;
-    scrollbar-color-active: $sky_blue;
-    scrollbar-color-hover: $light_cornflower;
-    scrollbar-color: $cornflower;
 }
 
 /* new app and modify globals buttons boxes below the app selection list */
 #left-button-box {
     align: center middle;
     grid-gutter: 1;
     width: 100%;
 }
 
 .button-grid {
     align: center middle;
 }
 
+#modify-globals-button {
+    width: 22;
+}
+
 /* ---------------------- RIGHT TOP HALF OF SCREEN ------------------------- */
 
 /* Matches the "Configure parameters for {app}" input list pane itself */
-#app-inputs-pane {
+#app-config-pane {
     border-title-color: $sky_blue;
     border-subtitle-color: $sky_blue;
-    padding-top: 1;
     border: round $cornflower;
     background: $navy 60%;
     margin-right: 1;
-    grid-gutter: 1;
     link-background-hover: $navy;
     link-color-hover: $orange;
+    scrollbar-background: $dark_gray;
+    scrollbar-background-active: $dark_gray;
+    scrollbar-background-hover: $dark_gray;
+    scrollbar-color-hover: $light_cornflower;
+    scrollbar-color: $cornflower;
+}
+
+TabbedContent #--content-tab-init-tab.-active {
+    color: $light_cornflower;
+}
+
+TabbedContent #--content-tab-argocd-tab.-active {
+    color: $light_cornflower;
+}
+
+TabbedContent #--content-tab-restore-tab.-active {
+    color: $light_cornflower;
+}
+
+TabbedContent #--content-tab-backup-tab.-active {
+    color: $light_cornflower;
+}
+
+#init-tab {
+    padding-top: 1;
+    padding-left: 0;
+}
+
+#argocd-tab {
+    padding: 0;
+}
+
+#restore-tab {
+    padding-top: 1;
+    padding: 0;
+}
+
+#backup-tab {
+    padding: 0;
+}
+
+.backups-grid {
+    height: auto;
+    grid-gutter: 1;
 }
 
 /* each collapsible in the app config panel */
 Collapsible {
     background: $navy 60%;
     border-top: none;
     padding-left: 0;
@@ -135,71 +166,65 @@
 }
 
 CollapsibleTitle:focus {
     color: $sky_blue;
     background: $blue_gray 20%;
 }
 
-/* this is the grid present in the SmolK8sLabCollapsibleInputs widget */
+/* this is the grid present in the SmolK8sLabCollapsibleInputs and RestoreAppConfig widgets */
 .collapsible-updateable-grid {
-    grid-gutter: 1;
     align: center top;
     height: auto;
+    grid-gutter: 1;
 }
 
 /* each app input label and input field row */
 .app-input-row {
-   layout: grid;
-   height: auto;
-   grid-size: 2;
-   grid-columns: 0.5fr 1.5fr;
-   padding-bottom: 1;
-   padding-left: 2;
-   padding-right: 1;
+    layout: grid;
+    height: auto;
+    grid-size: 2;
+    grid-columns: 0.5fr 1.5fr;
+    padding-bottom: 1;
+    padding-left: 2;
+    padding-right: 1;
 }
 
 /* argo cd config param section */
 .argo-config-container {
-   align: left top;
-   scrollbar-background: $dark_gray;
-   scrollbar-background-active: $dark_gray;
-   scrollbar-background-hover: $dark_gray;
-   scrollbar-color-active: $sky_blue;
-   scrollbar-color-hover: $light_cornflower;
-   scrollbar-color: $cornflower;
-}
-
-.argo-config-header {
-   width: 100%;
-   content-align: left middle;
-   padding-left: 1;
-   background: $blue_gray 20%;
-   color: $light_cornflower;
-   height: 3;
-   margin-bottom: 1;
+    align: left top;
+    scrollbar-background: $dark_gray;
+    scrollbar-background-active: $dark_gray;
+    scrollbar-background-hover: $dark_gray;
+    scrollbar-color-active: $sky_blue;
+    scrollbar-color-hover: $light_cornflower;
+    scrollbar-color: $cornflower;
 }
 
 .argo-config-row {
-   layout: grid;
-   height: auto;
-   grid-size: 2;
-   grid-columns: 0.5fr 1.5fr;
-   padding-bottom: 1;
-   padding-left: 2;
-   padding-right: 1;
+    layout: grid;
+    height: 3;
+    grid-size: 2;
+    grid-columns: 0.5fr 1.5fr;
+    padding-left: 2;
+    padding-right: 1;
 }
 
 .argo-switch-row {
-   layout: grid;
-   height: 5;
-   grid-size: 2;
-   grid-columns: 0.5fr 1.5fr;
-   padding-bottom: 1;
-   padding-left: 2;
-   padding-right: 1;
+    layout: grid;
+    height: 3;
+    grid-size: 2;
+    grid-columns: 0.5fr 1.5fr;
+    padding-left: 2;
+    padding-right: 1;
+}
+
+.argo-switch {
+    height: 3;
+    width: auto;
+    content-align: left middle;
 }
 
 .argo-config-label {
    height: 3;
    width: auto;
    content-align: left middle;
    color: $bluish_white 90%;
@@ -207,23 +232,71 @@
 
 .argo-config-input {
    height: auto;
    width: 100%;
    content-align: left middle;
 }
 
-/* divider between secret keys and the rest of the argo inputs */
-.secret-key-divider {
-   color: $light_cornflower;
-   height: 3;
-   padding-left: 1;
-   width: 100%;
-   background: $blue_gray 18%;
-   content-align: left middle;
-   margin-bottom: 1;
+/* adding a little extra padding between collapsibles */
+.collapsible-with-some-room {
+    padding-top: 1;
+}
+
+/* entire row for app label, app switch label, and switch for each app with restore enabled */
+.app-init-switch-and-labels-row {
+    background: $blue_gray 43%;
+    layout: grid;
+    grid-size: 4;
+    grid-columns: 1.3fr 0.7fr 0.5fr 0fr;
+    grid-gutter: 1;
+    height: auto;
+}
+
+/* header row for apps config panel */
+.header-row {
+    background: $blue_gray 30%;
+    height: 3;
+    width: 100%;
+    content-align: left middle;
+    margin-top: 1;
+    margin-bottom: 1;
+    padding-left: 1;
+    color: $light_cornflower 90%;
+}
+
+/* this is just for the cnpg restore label */
+.app-less-switch-row {
+    background: $blue_gray 25%;
+    layout: grid;
+    grid-size: 4;
+    grid-columns: 1.3fr 0.7fr 0.5fr 0fr;
+    grid-gutter: 1;
+    height: 3;
+    margin-top: 1;
+}
+
+/* switch label for each app */
+.app-init-switch-label {
+    height: 3;
+    width: 100%;
+    content-align: right middle;
+    color: $sky_blue;
+}
+
+/* stuff for the backup button for instant backups */
+.backup-button-grid {
+    align: center middle;
+    height: 9;
+}
+
+.backup-button {
+    padding-left: 2;
+    padding-right: 2;
+    padding-top: 1;
+    padding-bottom: 1;
 }
 
 /* blurb to let users know that we don't have secret keys for this app, but they can add some */
 .secret-key-help-text {
    width: 100%;
    padding-left: 1;
    padding-right: 1;
@@ -255,7 +328,8 @@
    content-align: left middle;
    width: 100%;
    padding-left: 1;
    padding-right: 1;
    padding-top: 1;
    color: $bluish_white 60%;
 }
+
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files 8% similar despite different names*

```diff
@@ -25,39 +25,23 @@
     height: auto;
 }
 
 .init-inputs-container {
     height: auto;
 }
 
-/* entire row for app label, app switch label, and switch for each app with initialization */
-.app-init-switch-and-labels-row {
-    background: $blue_gray 25%;
-    layout: grid;
-    grid-size: 4;
-    height: 3;
-    grid-columns: 1.3fr 0.7fr 0.5fr 0fr;
-}
-
 /* label for each app in the conigure selected apps pane */
 .initialization-label {
    height: 3;
    width: 100%;
    content-align: left middle;
    padding-left: 1;
    color: $light_cornflower;
 }
 
-/* switch label for each app */
-.app-init-switch-label {
-   height: 3;
-   width: 100%;
-   content-align: right middle;
-}
-
 .app-init-label {
     content-align: left middle;
     align: left middle;
     padding-top: 1;
     width: 100%;
 }
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base.tcss`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 Button {
     color: $light_cornflower;
     background: $lavender 10%;
     border-top: tall $blue_gray 60%;
     border-bottom: tall $dark_gray 50%;
 }
 
+LoadingIndicator {
+    color: $orange;
+}
+
 Input {
     background: $bluish_white 8%;
     color: white 75%;
     border: tall black 18%;
 }
 
 Input.-invalid {
@@ -75,14 +79,27 @@
 }
 
 /* sets the init switch slider color only when it's on */
 Switch.-on > .switch--slider {
     color: $spacechalk_lime 90%;
 }
 
+/* sets the color of the focused slider */
+Switch:focus {
+    border: tall $light_cornflower 70%;
+}
+
+Select:focus > SelectCurrent {
+    border: tall $light_cornflower 70%;
+}
+
+Select.-expanded > SelectCurrent {
+    border: tall $light_cornflower 70%;
+}
+
 /* Matches the "Select apps to install on k8s" Selection List */
 SelectionList {
     background: $navy 40%;
     color: $bluish_white;
     width: 100%;
 }
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files 15% similar despite different names*

```diff
@@ -17,28 +17,44 @@
 
 /* whole modal screen */
 #cluster-question-modal-screen {
     width: 80%;
     align: center middle;
 }
 
+/* individual buttons */
+#modify-apps-button {
+    width: 17;
+}
+
+#modify-nodes-button {
+    width: 18;
+}
+
+#delete-cluster-first-try {
+    width: 10;
+}
+
 .modify-delete-size {
     height: 14;
 }
 
 #cluster-modal-text {
    color: $cornflower;
 }
 
 #cluster-question-box {
     align: center middle;
     content-align: center middle;
     background: $navy 75%;
     border: round $cornflower;
     padding: 1;
+    border-subtitle-color: $lavender;
+    link-background-hover: $navy;
+    link-color-hover: $orange;
 }
 
 #modal-button-box {
     grid-size: 3;
     align: center middle;
     height: auto;
 }
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     background: rgb(35,35,54) 50%;
     link-background-hover: $navy;
     link-color-hover: $orange;
     padding: 2;
     grid-rows: 0.25fr 1fr;
 }
 
-/* TabbedContent box for the kind widget */
+/* TabbedContent box for the k3s widget */
 #k3s-tabbed-content {
     border: round $cornflower;
     border-title-color: $sky_blue;
     border-subtitle-color: $lavender;
     background: $navy 60%;
     width: 100%;
     height: 100%;
@@ -37,24 +37,36 @@
 }
 
 /* tabpane 1 */
 #k3s-yaml-tab {
     height: auto;
 }
 
+TabbedContent #--content-tab-k3s-yaml-tab.-active {
+    color: $light_cornflower;
+}
+
 /* tabpane 2 */
 #k3s-kubelet-tab {
     height: auto;
 }
 
-/* tabpane 2 */
+TabbedContent #--content-tab-k3s-kubelet-tab.-active {
+    color: $light_cornflower;
+}
+
+/* tabpane 3 */
 #k3s-nodes-tab {
     height: auto;
 }
 
+TabbedContent #--content-tab-k3s-nodes-tab.-active {
+    color: $light_cornflower;
+}
+
 /* k3s container itself */
 .k3s-arg-scroll {
     align: center middle;
     scrollbar-background: $dark_gray;
     scrollbar-background-active: $dark_gray;
     scrollbar-background-hover: $dark_gray;
     scrollbar-color-active: $sky_blue;
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/kind.tcss`

 * *Files 13% similar despite different names*

```diff
@@ -28,19 +28,27 @@
 }
 
 /* tabpane 1 */
 #kind-networking-tab {
     height: auto;
 }
 
+TabbedContent #--content-tab-kind-networking-tab.-active {
+    color: $light_cornflower;
+}
+
 /* tabpane 2 */
 #kind-kubelet-tab {
     height: auto;
 }
 
+TabbedContent #--content-tab-kind-kubelet-tab.-active {
+    color: $light_cornflower;
+}
+
 /* kind-networking config container that contains the vertical scroll box */
 #kind-networking-container {
     align: center middle;
     padding-top: 1;
     padding-left: 1;
     padding-right: 1;
     grid-rows: 0.2fr 1fr;
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     link-background-hover: $navy;
     link-color-hover: $orange;
     padding: 1;
     border-subtitle-color: $lavender;
     grid-rows: 0.45fr 0.9fr 0.45fr;
 }
 
-#scroll-container {
+#scroll-container-for-globals {
    scrollbar-background: $dark_gray;
    scrollbar-background-active: $dark_gray;
    scrollbar-background-hover: $dark_gray;
    scrollbar-color-active: $sky_blue;
    scrollbar-color-hover: $cornflower;
    scrollbar-color: $light_cornflower;
    align: center middle;
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     grid-size: 1;
     grid-rows: 0.85fr 1fr 1.2fr;
     margin-left: 1;
     margin-right: 1;
     align: center middle;
     width: 90%;
     height: 92%;
+    grid-gutter: 1;
 }
 
 /* logging config box */
 #logging-config {
     padding: 1;
-    margin-bottom: 2;
     grid-rows: 0.5fr 1fr;
     border: round $cornflower;
     border-title-color: $sky_blue;
     background: $navy 60%;
     align: left middle;
     content-align: left middle;
 }
@@ -153,7 +153,25 @@
 /* this is the help-text at the top of each module */
 .soft-text {
     color: $bluish_white 60%;
     width: 100%;
     padding-left: 1;
     padding-top: 1;
 }
+
+RunCommandConfig {
+    padding: 1;
+    margin-bottom: 1;
+    border: round $cornflower;
+    border-title-color: $sky_blue;
+    background: $navy 60%;
+    align: left middle;
+    content-align: left middle;
+}
+
+#run-command-config-row-grid {
+    grid-size: 2;
+}
+
+#run-command-config-row-grid .selection-row {
+    grid-columns: 0.5fr 1fr;
+}
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files 25% similar despite different names*

```diff
@@ -12,57 +12,45 @@
 $light_cornflower: rgb(122,162,247);
 $blue_gray: rgb(86,95,137);
 $dark_gray: rgb(58,58,58);
 $navy: rgb(35,35,54);
 
 #general-config-screen {
     grid-size: 1;
-    grid-rows: 0.85fr 1fr;
-    grid-gutter: 2;
+    grid-rows: 1.2fr 0.4fr;
     margin-left: 1;
     margin-right: 1;
     align: center middle;
+    content-align: center middle;
     width: 90%;
-    height: 92%;
+    padding-top: 2;
+    padding-bottom: 2;
 }
 
 /* truthy value rows with switches */
 .bool-switch-row {
     align: left middle;
     layout: grid;
     grid-size: 2;
-    grid-gutter: 1;
     grid-columns: 0.82fr 1fr;
 }
 
-/* k9s enabled bool switch row */
-.k9s-enabled {
-   grid-columns: 0.35fr 1fr;
-}
-
 /* show footer bool switch row */
 .show-footer {
-   grid-columns: 0.65fr 1fr;
+    grid-columns: 0.65fr 1fr;
 }
 
 .bool-switch-row-label {
     align: left middle;
     content-align: left middle;
     height: 3;
     color: $bluish_white;
     width: 100%;
 }
 
-/* k9s input field */
-.k9s-input-row .input-row {
-    align: left middle;
-    grid-size: 2;
-    grid-columns: 0.3fr 1fr;
-}
-
 /* any basic "label: input" row */
 .input-row {
     align: left middle;
     layout: grid;
     grid-size: 2;
     grid-columns: 0.2fr 1fr;
 }
@@ -74,63 +62,63 @@
     padding-left: 1;
     padding-top: 1;
 }
 
 /* TUI config box */
 #tui-config {
     padding: 1;
-    grid-rows: 0.4fr 0.5fr 0.45fr;
     margin-top: 2;
     border: round $cornflower;
     border-title-color: $sky_blue;
     background: $navy 60%;
     align: center middle;
     grid-gutter: 1;
 }
 
-/* three bool-switch-rows side by side */
-.triple-switch-row {
-    align: left middle;
-    content-align: left middle;
-    grid-size: 3;
-    grid-gutter: 1;
-    padding-left: 1;
-    height: 3;
-}
-
-#tui-config .input-row-label {
-    content-align: left middle;
-    height: 3;
-    padding-left: 1;
-    padding-right: 1;
-    color: $bluish_white;
-}
-
 #accessibility-config {
-    padding-top: 1;
-    padding-left: 1;
-    padding-right: 2;
-    grid-rows: 0.2fr 0.5fr 0.45fr 0.45fr;
     border: round $cornflower;
     border-title-color: $sky_blue;
     background: $navy 60%;
-    align: center middle;
+    align: center top;
+    padding-left: 1;
+    padding-right: 1;
+    padding-top: 2;
     grid-gutter: 1;
 }
 
 /* bell config row */
 #bell-row {
+    border-top: panel $dark_gray 50%;
+    border-title-color: $light_cornflower;
+}
+
+/* two bool-switch-rows side by side */
+.double-switch-row {
+    align: center middle;
+    content-align: left middle;
     grid-size: 2;
-    padding-left: 1;
+    padding-left: 2;
+    padding-top: 1;
+    height: 5;
 }
 
-/* text to speech config row */
-#tts-row {
-    grid-size: 3;
-    padding-left: 1;
+/* text to speech config rows */
+.tts-row-title {
+    grid-columns: 0.3fr 1fr;
+    color: $bluish_white;
+    padding-top: 1;
+    border-top: panel $dark_gray 50%;
+    border-title-color: $light_cornflower;
 }
 
 #accessibility-config .input-row-label {
     content-align: left middle;
     height: 3;
     padding-left: 1;
 }
+
+.tui-config-row {
+    align: center middle;
+    content-align: left middle;
+    grid-size: 2;
+    padding-left: 2;
+}
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_screen.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,26 +39,28 @@
     """
     CSS_PATH = ["./css/distro_config.tcss",
                 "./css/node_inputs_widget.tcss",
                 "./css/add_nodes_widget.tcss",
                 "./css/k3s.tcss",
                 "./css/kind.tcss"]
 
-    BINDINGS = [Binding(key="b,q,escape",
-                        key_display="b",
-                        action="app.pop_screen",
-                        description="Back"),
-                Binding(key="n",
-                        key_display="n",
-                        action="app.request_apps_cfg",
-                        description="Next"),
-                Binding(key="a",
-                        key_display="a",
-                        action="screen.launch_new_option_modal",
-                        description="add new option")]
+    BINDINGS = [
+            Binding(key="b,q,escape",
+                    key_display="b",
+                    action="app.pop_screen",
+                    description="Back"),
+            Binding(key="n",
+                    key_display="n",
+                    action="app.request_apps_cfg",
+                    description="Next"),
+            Binding(key="ctrl+n",
+                    key_display="ctrl+n",
+                    action="screen.launch_new_option_modal",
+                    description="add new")
+            ]
 
     def __init__(self, config: dict) -> None:
         """
         config dict struct:
             {"distro":
                {"enabled": bool},
                {"k3s_yaml": dict},
@@ -100,28 +102,24 @@
                                 id="distro-description")
 
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
-        sub_title = "Kubernetes distro config"
+        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
+        sub_title = f"Kubernetes distro config for {self.app.current_cluster}"
         self.sub_title = sub_title
 
         top_row = self.get_widget_by_id("top-distro-row")
         top_row.border_title = "🌱 Select a [#C1FF87]k8s distro[/]"
         top_row.border_subtitle = "[i]Inputs below are optional"
 
         main_box = self.get_widget_by_id("distro-config-screen")
 
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say("Screen title: " + sub_title)
-
         if self.current_distro == 'kind':
             main_box.mount(
                     KindConfigWidget(
                         self.cfg.get('kind', DEFAULT_DISTRO_OPTIONS['kind']),
                         id='kind-pseudo-screen'
                         )
                     )
@@ -131,14 +129,16 @@
                         self.current_distro,
                         self.cfg.get(self.current_distro,
                                      DEFAULT_DISTRO_OPTIONS[self.current_distro]),
                         id=self.current_distro + "-pseudo-screen"
                         )
                     )
 
+        self.call_after_refresh(self.app.play_screen_audio, screen="distro")
+
     @on(Select.Changed)
     def update_k8s_distro(self, event: Select.Changed) -> None:
         """
         changed currently enabled kubernetes distro in the TUI
         """
         if event.select.id == "distro-drop-down":
             distro = str(event.value)
@@ -182,14 +182,21 @@
                 self.app.cfg['k8s_distros'][self.current_distro]['enabled'] = False
 
             # write out the yaml
             self.app.write_yaml()
 
             self.current_distro = distro
 
+    def action_add_node_to_widget(self) -> None:
+        """
+        call the add new node button action for the AddNodesBox widget
+        """
+        nodes_box = self.get_widget_by_id("nodes-tab-nodes-widget")
+        nodes_box.action_press_new_node_button()
+
     def action_launch_new_option_modal(self) -> None:
         """
         callable action via link and key binding to display a modal for adding
         a new option to the currently selected tab of the distro's config screen
         """
         def add_new_row(option: str):
             """
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from smol_k8s_lab.tui.distro_widgets.add_nodes import AddNodesBox
 from smol_k8s_lab.tui.util import create_sanitized_list
 from smol_k8s_lab.tui.validators.already_exists import CheckIfNameAlreadyInUse
 
 # external libraries
 from textual import on
 from textual.app import ComposeResult
+from textual.binding import Binding
 from textual.containers import VerticalScroll, Grid
 from textual.screen import ModalScreen
 from textual.suggester import SuggestFromList
 from textual.validation import Length
 from textual.widgets import Input, Button, Label, Static, TabbedContent, TabPane
 
 CFG_FILE = XDG_CACHE_DIR + "/k3s.yaml"
@@ -50,28 +51,32 @@
        "feature-gates=",
        ))
 
 LIST_KEYS = ["disable", "node-label", "kubelet-arg"]
 
 
 class K3sConfigWidget(Static):
-    """ 
+    """
     a widget representing the entire kind configuration
     """
+    BINDINGS = [Binding(key="ctrl+n",
+                        key_display="ctrl+n",
+                        action="add_option_or_node",
+                        description="add new")]
     def __init__(self, distro: str, metadata: dict, id: str = "") -> None:
         self.distro = distro
         self.metadata = metadata
         super().__init__(id=id)
 
     def compose(self) -> ComposeResult:
         if not self.metadata:
             self.metadata = DEFAULT_DISTRO_OPTIONS[self.distro]
 
         with Grid(classes="k8s-distro-config", id=f"{self.distro}-box"):
-            # Add the TabbedContent widget for kind config
+            # Add the TabbedContent widget for k3s config
             with TabbedContent(initial="k3s-yaml-tab", id="k3s-tabbed-content"):
                 # tab 1 - networking options
                 with TabPane("k3s.yaml", id="k3s-yaml-tab"):
                     # take extra k3s args if self.distro is k3s or k3d
                     yield K3sConfig(self.distro,
                                     self.metadata['k3s_yaml'],
                                     id=f"{self.distro}-widget")
@@ -82,15 +87,16 @@
                     kubelet_args = self.metadata['k3s_yaml'].get('kubelet-arg', '')
                     yield KubeletConfig('k3s', kubelet_args)
 
                 if self.distro == "k3s":
                     # tab 3 - add remote nodes
                     with TabPane("🆕 Add [i]Remote[/i] Nodes", id="k3s-nodes-tab"):
                         yield AddNodesBox(self.metadata.get('nodes', []),
-                                          id="nodes-tab")
+                                          existing_cluster=False,
+                                          id="nodes-tab-nodes-widget")
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
         # update tabbed content box
         tabbed_content = self.query_one(TabbedContent)
@@ -125,23 +131,39 @@
         speaks name of tab if tts is on and changes button at the button of border
         """
         tab = event.tab.id
         if self.app.speak_on_focus:
             self.app.action_say(f"Selected tab is {tab}")
 
         # change border subtitle button depending on the tab activated
-        tabbed_content = self.query_one(TabbedContent)
-        if tab == "k3s-nodes-tab":
-           tabbed_content.border_subtitle = (
-                "[b][@click=screen.launch_new_option_modal()] ➕ node[/][/]"
-                )
+        if self.distro == "k3s":
+            tabbed_content = self.query_one(TabbedContent)
+            if "k3s-nodes-tab" in tab:
+               tabbed_content.border_subtitle = (
+                    "[b][@click='screen.add_node_to_widget()'] ➕ node[/][/b]"
+                    )
+               if self.app.speak_on_focus:
+                   self.app.action_say("Pressing Control + A will add a new node"
+                                       "based on your inputs")
+            else:
+               tabbed_content.border_subtitle = (
+                    "[b][@click=screen.launch_new_option_modal()] ➕ k3s option[/][/b]"
+                    )
+               if self.app.speak_on_focus:
+                   self.app.action_say("Pressing Control + A will add a new option")
+
+    def action_add_option_or_node(self) -> None:
+        """
+        call either the add new option or add new node action depending on the
+        current border subtitle action
+        """
+        if "node" in self.query_one(TabbedContent).border_subtitle:
+            self.screen.action_add_node_to_widget()
         else:
-           tabbed_content.border_subtitle = (
-                "[b][@click=screen.launch_new_option_modal()] ➕ k3s option[/][/]"
-                )
+            self.screen.launch_new_option_modal()
 
 
 class K3sConfig(Static):
     """
     k3s args config
     """
 
@@ -225,15 +247,15 @@
 
             self.app.write_yaml()
 
     def generate_row(self, key: str, value: str = "") -> Grid:
         """
         create a new input row
         """
-        # this is the label 
+        # this is the label
         key_label = key.replace("-", " ").replace("_", " ") + ":"
         label = Label(key_label, classes="input-label")
 
         # input values
         row_args = {"placeholder": f"Enter a {key} and press Enter",
                     "classes": f"{self.distro} k3s-arg-input",
                     "suggester": SUGGESTIONS,
@@ -252,15 +274,15 @@
             if isinstance(value, list):
                 row_args['value'] = ", ".join(value)
 
             # else if this is a string, we just set it to that value outright
             if isinstance(value, str):
                 row_args['value'] = value
 
-        # actual input field 
+        # actual input field
         input = Input(**row_args)
         tooltip = (f"If you want to input more than one {key} option, try using "
                    "a comma seperated list.")
 
         # we give a bit more info on disabling
         if key == "disable":
             tooltip += (" If [dim][#C1FF87]metallb[/][/] is [i]enabled[/], we add"
@@ -269,15 +291,15 @@
         input.tooltip = tooltip
 
         # button to delete the field entirely
         button = Button("🚮",
                         id=f"{self.distro}-{key}-delete-button",
                         classes="k3s-arg-del-button")
         button.tooltip = "Delete the arg to the left of this button"
-        
+
         grid = Grid(label, input, button, classes="label-input-delete-row")
         self.get_widget_by_id("k3s-grid").mount(grid)
 
 
 class NewK3sOptionModal(ModalScreen):
 
     CSS_PATH = ["../css/k3s_modal.css"]
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,29 +34,26 @@
                     # modify button allows user to change apps (and soon distro details)
                     modify_button = Button("✏️  Modify", id="modify-node-button")
                     modify_button.tooltip = "Modify the node's metadata"
                     yield modify_button
 
                     # delete button deletes the node
                     delete_button = Button("🚮 Delete", id="delete-node-first-try")
-                    delete_button.tooltip = "[magenta]Delete[/] the node 😱"
+                    delete_button.tooltip = "[#ffaff9]Delete[/] the node 😱"
                     yield delete_button
 
                     cancel = Button("🤷 Cancel", id="cancel")
                     cancel.tooltip = "Return to previous screen"
                     yield cancel
 
     def on_mount(self):
-        """ 
-        say the title if that self.app.speak_screen_titles is set to True
         """
-        if self.app.speak_screen_titles:
-            self.app.action_say(
-                    f"Screen title: What would you like to do with {self.node}?"
-                    )
+        say the title if that tui.tts.screen_titles is set to True
+        """
+        self.call_after_refresh(self.app.play_screen_audio, screen="modify_node_modal")
 
     def action_press_cancel(self) -> None:
         """
         presses the cancel button
         """
         self.get_widget_by_id("cancel").action_press()
 
@@ -70,16 +67,15 @@
             event.button.display = False
             self.get_widget_by_id("modify-node-button").display = False
 
             # are you sure, the text
             confirm_txt = ('Are you [b][i]sure[/][/] you want to [#ffaff9]delete[/]'
                            f' [#C1FF87]{self.node}[/]?')
             self.get_widget_by_id("node-modal-text").update(confirm_txt)
-            if self.app.speak_screen_titles:
-                self.app.action_say(f"Are you sure you want to delete {self.node}?")
+            self.app.play_screen_audio(screen="modify_node_modal", alt=True)
 
             # are you sure, the button
             sure_button = Button("🚮 Yes", id="delete-button-second-try")
             self.get_widget_by_id("modal-button-box").mount(sure_button,
                                                             before="#cancel")
 
         # if the user really wants to delete a node, we do it
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/help_screen.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,20 @@
             Binding(key="?,q,escape",
                     key_display="q",
                     action="disable_help",
                     description="Exit Help Screen",
                     show=True),
             Binding(key="n",
                     show=False,
-                    action="app.bell")
+                    action="app.bell"),
+            Binding(key="f5",
+                    key_display="f5",
+                    description="Speak",
+                    action="app.speak_element",
+                    show=True),
                 ]
 
     def compose(self) -> ComposeResult:
         welcome = ("Use your 🐁 to click anything in the UI ✨ Or use the "
                    "following key bindings. For additional help, check out the "
                    "[steel_blue][link=https://small-hack.github.io/smol-k8s-lab/]docs[/][/]")
 
@@ -39,54 +44,48 @@
         help_container = self.get_widget_by_id("help-container")
         help_container.border_title = select_apps_title
         help_container.border_subtitle = (
                 "made with 💙 + 🐍 + [steel_blue][i][link="
                 "https://github.com/Textualize/textual]textual[/][/][/]"
                 )
 
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say(
-                    "Screen title: Help Screen. Use your mouse to click anything"
-                    " in the UI ✨ Or use the following key bindings. For "
-                    "additional help, checkout smol dash k8s dot org."
-                    )
+        self.call_after_refresh(self.app.play_screen_audio, screen="help")
 
-        self.build_help_table()
+        self.build_keymappings_table()
 
-    def build_help_table(self) -> None:
+    def build_keymappings_table(self) -> None:
         data_table = DataTable(zebra_stripes=True,
-                               id="help-table",
+                               id="key-mappings-table",
                                cursor_type="row")
 
         # then fill in the cluster table
         data_table.add_column(Text("Key Binding", justify="center"))
         data_table.add_column(Text("Description"))
 
         link_help = ("open link; terminal dependent, so meta can be shift,"
                      "\n option, windowsKey, command, or control")
 
         # tips for new/forgetful users (the maintainers are also forgetful <3)
         help_dict = {
-                "➡ ": "complete suggestion in input field",
-                "⬆/⬇": "navigate up and down the app selection list",
+                "right arrow": "complete suggestion in input field",
+                "up and down arrows": "navigate up or down selection lists and data tables",
                 "tab": "focus next element",
                 "shift+tab": "focus previous element",
-                "↩ enter": "save input and/or press button",
-                "?,h": "toggle help screen",
+                "enter": "save input and/or press button",
+                "? or h": "toggle help screen",
                 "spacebar": "select selection option",
                 "meta+click": link_help,
-                "escape,q": "leave current screen and go home",
+                "esc or q": "leave current screen and go home",
                 "c": "launch the config screen",
-                "f5": "read aloud current focused element id",
+                "f5": "read aloud current focused element ID",
                 "f": "toggle showing the footer"
                 }
 
         for key_binding, description in help_dict.items():
-            # we use an extra line to center the rows vertically 
+            # we use an extra line to center the rows vertically
             styled_row = [
                     Text(str("\n" + key_binding)),
                     Text(str("\n" + description))
                           ]
 
             if key_binding == "meta+click":
                 data_table.add_row(*styled_row, height=4, key=key_binding)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/make_screenshots.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 #!/usr/bin/env python
 # thank you to davep for helping me learn this:
 # https://blog.davep.org/2023/07/03/making-my-github-banner.html
 
 from smol_k8s_lab.tui.base import BaseApp
 import asyncio
+from time import sleep
 
 
 screenshot_path = "./docs/assets/images/screenshots"
 
 
 async def make_base_screenshots() -> None:
     """
     make all the screenshots for the start screen, help screen, and TUI config screen
     """
     async with BaseApp().run_test(size=(87, 47)) as pilot:
-        pilot.app.save_screenshot(f"{screenshot_path}/start_screen.svg")
+        sleep(3)
+        # pilot.app.save_screenshot(f"{screenshot_path}/start_screen.svg")
+        await pilot.press("enter")
+        pilot.app.save_screenshot(f"{screenshot_path}/modify_cluster_modal_screen.svg")
 
+    async with BaseApp().run_test(size=(87, 53)) as pilot:
+        # press the "q" key and "h" key for the help screen
+        await pilot.press("tab", "h")
+        pilot.app.save_screenshot(f"{screenshot_path}/tui_help_screen.svg")
+
+    async with BaseApp().run_test(size=(99, 47)) as pilot:
         # press the "tab" key followed by the "c" key
         await pilot.press("tab", "c")
         pilot.app.save_screenshot(f"{screenshot_path}/tui_config_screen.svg")
 
-        # press the "q" key and "h" key for the help screen
-        await pilot.press("q", "h")
-        pilot.app.save_screenshot(f"{screenshot_path}/tui_help_screen.svg")
-
 
 async def make_distro_screen_screenshots() -> None:
     """
     make all the screenshots for the kubernetes distribution config screen
     """
     async with BaseApp().run_test(size=(90, 55)) as pilot:
         # press the "enter" key and then f key to go to the distro screen, then hide the footer
@@ -54,33 +60,33 @@
 
 async def make_apps_screen_screenshots() -> None:
     """
     Make all the screenshots for the Argo CD ApplicationSet configuration screen
     """
     async with BaseApp().run_test(size=(90, 55)) as pilot:
         # press the "enter" key and then the "n" key
-        await pilot.press("enter", "n")
+        await pilot.press("enter", "enter")
         pilot.app.save_screenshot(f"{screenshot_path}/apps_screen.svg")
 
         # press the "a" key to add a new app
         await pilot.press("a")
         pilot.app.save_screenshot(f"{screenshot_path}/new_app_modal_screen.svg")
 
         # press tab, tab, enter to get to the modify_global_parameters button
-        await pilot.press("escape","tab","tab","enter")
+        await pilot.press("escape","tab","enter")
         pilot.app.save_screenshot(f"{screenshot_path}/modify_global_parameters_modal_screen.svg")
 
 
 async def make_confirmation_screen_screenshots() -> None:
     """
     make all the screenshots for the confirmation screen
     """
     async with BaseApp().run_test(size=(87, 47)) as pilot:
         # logging and password config
-        await pilot.press("enter", "n", "n", "n")
+        await pilot.press("enter", "enter", "n", "n")
         pilot.app.save_screenshot(f"{screenshot_path}/logging_password_config.svg")
 
         # confirmation screen finally
         await pilot.press("n")
         pilot.app.save_screenshot(f"{screenshot_path}/confirm_screen.svg")
 
         # enter bitwarden credentials
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,200 +1,239 @@
-#!/usr/bin/env python3.11
 from smol_k8s_lab.tui.util import bool_option, input_field
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Container, Grid
+from textual.containers import Grid
 from textual.screen import Screen
-from textual.widgets import Footer, Header, Input, Label, Switch, Select
+from textual.widgets import Footer, Header, Input, Label, Switch
 from textual.widget import Widget
-from xdg_base_dirs import xdg_state_home
 
 
-XDG_STATE_HOME = str(xdg_state_home()) + "/smol-k8s-lab/smol.log"
-
-logging_tool_tip = (
-        "[deep_sky_blue3]Logging verbosity levels[/]:\n\n"
-        "[on grey11][grey50]error[/]:  only print error messages[/]\n\n"
-        "[grey50]warn[/]:   print warnings, plus errors\n\n"
-        "[on grey11][grey50]info[/]:   check ins at each stage, plus warnings/errors[/]"
-        "\n\n"
-        "[grey50]debug[/]:  most detailed, includes all sorts of variable printing"
-        )
-
-duplicate_tool_tip = (
-    "[deep_sky_blue3]Handling vault item duplicates[/]:\n\n"
-    "[on grey11][grey50]ask[/]:       (default) display a dialog window asking how to "
-    "proceed[/]\n\n"
-    "[grey50]edit[/]:      if 1 item found, edit item. Still ask if multiple found\n\n"
-    "[on grey11][grey50]duplicate[/]: create an additional item with the same name[/]"
-    "\n\n"
-    "[grey50]no_action[/]: don't do anything, just continue on with the script")
-
-
-class SmolK8sLabConfig(Screen):
+class TuiConfigScreen(Screen):
     """
     Textual app to configure smol-k8s-lab itself
     """
-    CSS_PATH = ["./css/smol_k8s_cfg.tcss"]
+    CSS_PATH = ["./css/tui_config.tcss"]
 
     BINDINGS = [Binding(key="b,q,escape",
                         key_display="b",
                         action="app.pop_screen",
                         description="Back"),
                 Binding(key="n",
-                        key_display="n",
-                        action="app.request_confirm",
-                        description="Next")]
+                        show=False,
+                        action="app.bell")]
 
     def __init__(self, config: dict) -> None:
         self.cfg = config
-        self.show_footer = self.app.cfg['smol_k8s_lab']['tui']['show_footer']
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
         Compose app with tabbed content.
         """
         # header to be cute
         yield Header()
 
         # Footer to show help keys, if enabled
         footer = Footer()
-        if not self.show_footer:
-            footer.display = False
+        footer.display = False
         yield footer
 
-        with Grid(id="config-screen"):
-            yield LoggingConfig(self.cfg['log'])
+        with Grid(id="general-config-screen"):
+            # accessibility options config
+            yield AccessibilityWidget(self.cfg['accessibility'])
 
-            # local password manager config for enabled, name, and duplicate strategy
-            yield PasswordManagerConfig(self.cfg['local_password_manager'])
+            # tui config for hide_footer, enabled
+            yield TuiConfig(self.cfg, id="tui-config")
 
     def on_mount(self) -> None:
         """
-        screen and box border styling
+        screen and box border styling and read the screen title aloud
         """
         self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
-        sub_title = "Configure logging and password manager"
+        sub_title = "Configure Terminal UI and Accessibility features"
         self.sub_title = sub_title
 
-        if self.app.speak_screen_titles:
-            # if text to speech is on, read screen title
-            self.app.action_say("Screen title: " + sub_title)
+        # turn on the footer if it's enabled in the root app cfg
+        if self.app.cfg['smol_k8s_lab']['tui']['show_footer']:
+            self.query_one(Footer).display = True
 
+        self.app.play_screen_audio("tui_config")
 
-class LoggingConfig(Widget):
-    def __init__(self, config: dict) -> None:
+
+class TuiConfig(Widget):
+    def __init__(self, config: dict, id: str = "") -> None:
         self.cfg = config
-        super().__init__()
+        super().__init__(id=id)
 
     def compose(self) -> ComposeResult:
         """
-        Compose widget for configuring logging
+        Compose widget for configuring the tui experience
         """
-        # logging config for log.level and log.file
-        logging_opt = self.cfg
-        current_level = logging_opt['level']
-        possible_levels = ['error', 'warn', 'debug', 'info']
-
-        with Grid(id="logging-config"):
-            yield Label("Configure logging for all of smol-k8s-lab.",
-                        classes="soft-text")
-
-            with Grid(id="logging-config-row-grid"):
-                with Grid(classes="selection-row"):
-                    label = Label("level:", classes="selection-label")
-                    label.tooltip = logging_tool_tip
-                    yield label
-
-                    yield Select(((line, line) for line in possible_levels),
-                                 id="log-level-select",
-                                 value=current_level)
-
-                yield input_field(label="file",
-                                  initial_value=logging_opt['file'],
-                                  name="file",
-                                  placeholder=XDG_STATE_HOME,
-                                  tooltip="File to log to. If provided, no console "
-                                          "logging will take place")
+        with Grid(classes="tui-config-row"):
+            yield bool_option(
+                    label="tui enabled",
+                    name="enabled",
+                    switch_value=self.cfg['enabled'],
+                    tooltip=("Enable tui mode by default. Otherwise, you"
+                             " need to pass in the interactive flag on the "
+                             "command line each time")
+                    )
+
+            yield bool_option(
+                    label="footer",
+                    name="show_footer",
+                    switch_value=self.cfg['show_footer'],
+                    tooltip="show the footer at the bottom of the screen"
+                    )
 
     def on_mount(self) -> None:
         """
         box border styling
         """
-        log_title = "🪵[i]Configure[/] [#C1FF87]Logging"
-        self.get_widget_by_id("logging-config").border_title = log_title
+        tui_title = "🖥️ [i]Configure[/] [#C1FF87]Terminal UI"
+        self.border_title = tui_title
+
+    @on(Switch.Changed)
+    def update_parent_config_for_switch(self, event: Switch.Changed) -> None:
+        """
+        update the parent app's config file yaml obj
+        """
+        truthy_value = event.value
+        switch_name = event.switch.name
+
+        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']
+
+        self.cfg[switch_name] = truthy_value
+        parent_cfg[switch_name] = truthy_value
 
-    @on(Select.Changed)
-    def update_parent_for_select(self, event: Select.Changed) -> None:
-        self.app.cfg['smol_k8s_lab']['log']['level'] = str(event.value)
         self.app.write_yaml()
 
     @on(Input.Changed)
     def update_parent_config_for_input(self, event: Input.Changed) -> None:
-        """
-        update self and parent app self config with changed input field
-        """
-        self.app.cfg['smol_k8s_lab']['log'][input.name] = event.input.value
+        input = event.input
+        self.app.cfg['smol_k8s_lab']['tui'][input.name] = input.value
         self.app.write_yaml()
 
 
-class PasswordManagerConfig(Widget):
+class AccessibilityWidget(Widget):
     def __init__(self, config: dict) -> None:
+        """
+        Accessibility widget to allow for configuring the bell and text to speech
+        """
         self.cfg = config
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
-        Compose widget for configuring the local password manager
+        Compose widget for configuring the tui experience
         """
-        with Container(id="password-manager-config"):
-            yield Label("Save app credentials to a local password manager vault. "
-                        "Only Bitwarden is supported at this time, but if enabled,"
-                        " Bitwarden can be used as your k8s external secret provider."
-                        " To avoid a password prompt, export the following env vars: "
-                        "BW_PASSWORD, BW_CLIENTID, BW_CLIENTSECRET",
-                        classes="soft-text")
-
-            enabled_tooltip = "enable storing passwords for apps in a password manager"
-            with Grid(id="password-manager-options-grid"):
-                yield bool_option("enabled",
-                                  self.cfg['enabled'],
-                                  "enabled",
-                                  enabled_tooltip)
-
-                with Grid(classes="selection-row"):
-                    label = Label("duplicate strategy:",
-                                  classes="radioset-row-label")
-                    label.tooltip = duplicate_tool_tip
-                    yield label
-
-                    current_value = self.cfg['duplicate_strategy']
-                    possible_values = ["ask", "edit", "duplicate", "no_action"]
-
-                    yield Select(((line, line) for line in possible_values),
-                                 id="duplicate-strategy-select",
-                                 value=current_value)
+        with Grid(id="accessibility-config"):
+
+            with Grid(id="bell-row", classes="double-switch-row"):
+
+                yield bool_option(
+                        label="bell on focus",
+                        name="bell-on_focus",
+                        switch_value=self.cfg['bell']['on_focus'],
+                        tooltip=(
+                            "Ring the terminal bell each time your focus "
+                            "changes to another element on the screen.")
+                        )
+
+                yield bool_option(
+                        label="bell on error",
+                        name="bell-on_error",
+                        switch_value=self.cfg['bell']['on_error'],
+                        tooltip=(
+                            "Ring the terminal bell anytime there's a warning "
+                            "or error"
+                            )
+                )
+
+            yield input_field(
+                    label="speech program",
+                    name="text-to-speech-speech_program",
+                    initial_value=self.cfg['text_to_speech']['speech_program'],
+                    placeholder="name of program for speech",
+                    tooltip=(
+                        "If text to speech is enabled, this is the name of"
+                        " the command line interface speech program. If not "
+                        "provided, we use pre-generated audio files"
+                        ),
+                    extra_row_class="tts-row-title"
+                    )
+
+            with Grid(id="tts-row", classes="double-switch-row"):
+                yield bool_option(
+                        label="on key press",
+                        name="text-to-speech-on_key_press",
+                        switch_value=self.cfg['text_to_speech']['on_key_press'],
+                        tooltip=(
+                            "Only read aloud the element if the f5 key is pressed. "
+                            "This key will be configurable in the future."
+                            )
+                        )
+                yield bool_option(
+                        label="on focus",
+                        name="text-to-speech-on_focus",
+                        switch_value=self.cfg['text_to_speech']['on_focus'],
+                        tooltip=(
+                            "On each focus of a new element on the screen, "
+                            "read aloud the element id, and value/tooltip if "
+                            "available."
+                            )
+                        )
+
+            with Grid(classes="double-switch-row"):
+                yield bool_option(
+                        label="screen titles",
+                        name="text-to-speech-screen_titles",
+                        switch_value=self.cfg['text_to_speech']['screen_titles'],
+                        tooltip=(
+                            "Read aloud each screen title."
+                            )
+                        )
+
+                yield bool_option(
+                        label="screen descriptions",
+                        name="text-to-speech-screen_descriptions",
+                        switch_value=self.cfg['text_to_speech']['screen_descriptions'],
+                        tooltip=(
+                            "Read aloud each screen description."
+                            )
+                        )
 
     def on_mount(self) -> None:
         """
         box border styling
         """
-        pass_title = "🔒[i]Configure[/] [#C1FF87]Password Manager"
-        self.get_widget_by_id("password-manager-config").border_title = pass_title
+        title = "♿️ [i]Configure[/] [#C1FF87]Accessibility Features"
+        self.get_widget_by_id("accessibility-config").border_title = title
+        self.get_widget_by_id("bell-row").border_title = "Terminal Bell Config"
+        self.query_one(".tts-row-title").border_title = "Text to Speech Config"
 
     @on(Switch.Changed)
-    def update_parent_config(self, event: Switch.Changed) -> None:
+    def update_parent_config_for_switch(self, event: Switch.Changed) -> None:
         """
         update the parent app's config file yaml obj
         """
-        value = event.value
+        truthy_value = event.value
         switch_name = event.switch.name
-        self.app.cfg['smol_k8s_lab']['local_password_manager'][switch_name] = value
+
+        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']['accessibility']
+
+        if "text-to-speech" in switch_name:
+            name = switch_name.replace("text-to-speech-", "")
+            parent_cfg['text_to_speech'][name] = truthy_value
+        else:
+            name = switch_name.replace("bell-", "")
+            parent_cfg['bell'][name] = truthy_value
+
         self.app.write_yaml()
 
-    @on(Select.Changed)
-    def update_parent_for_select(self, event: Select.Changed) -> None:
-        password_cfg = self.app.cfg['smol_k8s_lab']['local_password_manager']
-        password_cfg['duplicate_strategy'] = str(event.value)
+    @on(Input.Changed)
+    def update_parent_config_for_input(self, event: Input.Changed) -> None:
+        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']['accessibility']
+        parent_cfg['text_to_speech']['speech_program'] = event.input.value
+
         self.app.write_yaml()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,280 @@
 #!/usr/bin/env python3.11
 from smol_k8s_lab.tui.util import bool_option, input_field
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Grid
+from textual.containers import Container, Grid
 from textual.screen import Screen
-from textual.widgets import Footer, Header, Input, Label, Switch
+from textual.widgets import Footer, Header, Input, Label, Switch, Select
 from textual.widget import Widget
+from xdg_base_dirs import xdg_state_home
 
 
-class TuiConfigScreen(Screen):
+XDG_STATE_HOME = str(xdg_state_home()) + "/smol-k8s-lab/smol.log"
+
+logging_tool_tip = (
+        "[deep_sky_blue3]Logging verbosity levels[/]:\n\n"
+        "[on grey11][grey50]error[/]:  only print error messages[/]\n\n"
+        "[grey50]warn[/]:   print warnings, plus errors\n\n"
+        "[on grey11][grey50]info[/]:   check ins at each stage, plus warnings/errors[/]"
+        "\n\n"
+        "[grey50]debug[/]:  most detailed, includes all sorts of variable printing"
+        )
+
+duplicate_tool_tip = (
+    "[deep_sky_blue3]Handling vault item duplicates[/]:\n\n"
+    "[on grey11][grey50]ask[/]:       (default) display a dialog window asking how to "
+    "proceed[/]\n\n"
+    "[grey50]edit[/]:      if 1 item found, edit item. Still ask if multiple found\n\n"
+    "[on grey11][grey50]duplicate[/]: create an additional item with the same name[/]"
+    "\n\n"
+    "[grey50]no_action[/]: don't do anything, just continue on with the script")
+
+
+class SmolK8sLabConfig(Screen):
     """
     Textual app to configure smol-k8s-lab itself
     """
-    CSS_PATH = ["./css/tui_config.tcss"]
+    CSS_PATH = ["./css/smol_k8s_cfg.tcss"]
 
     BINDINGS = [Binding(key="b,q,escape",
                         key_display="b",
                         action="app.pop_screen",
                         description="Back"),
                 Binding(key="n",
-                        show=False,
-                        action="app.bell")]
+                        key_display="n",
+                        action="app.request_confirm",
+                        description="Next")]
 
     def __init__(self, config: dict) -> None:
         self.cfg = config
+        self.show_footer = self.app.cfg['smol_k8s_lab']['tui']['show_footer']
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
         Compose app with tabbed content.
         """
         # header to be cute
         yield Header()
 
         # Footer to show help keys, if enabled
         footer = Footer()
-        footer.display = False
+        if not self.show_footer:
+            footer.display = False
         yield footer
 
-        with Grid(id="general-config-screen"):
-            # tui config for hide_footer, enabled, and k9s
-            yield TuiConfig(self.cfg)
+        with Grid(id="config-screen"):
+            yield LoggingConfig(self.cfg['log'])
+
+            # local password manager config for enabled, name, and duplicate strategy
+            yield PasswordManagerConfig(self.cfg['local_password_manager'])
 
-            # accessibility options config
-            yield AccessibilityWidget(self.cfg['accessibility'])
+            # configure command to run after tui phase
+            yield RunCommandConfig(self.cfg['run_command'])
 
     def on_mount(self) -> None:
         """
-        screen and box border styling and read the screen title aloud
+        screen and box border styling
         """
         self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
-        sub_title = (
-                "Screen title: Configure Terminal UI and Accessibility features"
-                )
+        sub_title = "Configure logging and password manager"
         self.sub_title = sub_title
 
-        # turn on the footer if it's enabled in the root app cfg
-        if self.app.cfg['smol_k8s_lab']['tui']['show_footer']:
-            self.query_one(Footer).display = True
-
-        if self.app.speak_screen_titles:
-            self.app.action_say(
-                    self.sub_title + ". There are 2 boxes on the screen. Box 1: "
-                    "Configure Terminal UI. Box 2: Configure Accessibility. Focus"
-                    " starts on Box 1."
-                    )
+        self.call_after_refresh(self.app.play_screen_audio, screen="config")
 
 
-class TuiConfig(Widget):
+class LoggingConfig(Widget):
     def __init__(self, config: dict) -> None:
         self.cfg = config
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
-        Compose widget for configuring the tui experience
+        Compose widget for configuring logging
         """
+        # logging config for log.level and log.file
+        logging_opt = self.cfg
+        current_level = logging_opt['level']
+        possible_levels = ['error', 'warn', 'debug', 'info']
 
-        with Grid(id="tui-config"):
-            yield Label("These parameters are all related to the TUI itself.",
+        with Grid(id="logging-config"):
+            yield Label("Configure logging for all of smol-k8s-lab.",
                         classes="soft-text")
-            with Grid(classes="triple-switch-row"):
-                yield bool_option(
-                        label="enabled",
-                        name="enabled",
-                        switch_value=self.cfg['enabled'],
-                        tooltip=("Enable tui mode by default. Otherwise, you"
-                                 " need to pass in the interactive flag on the "
-                                 "command line each time")
-                        )
-
-                yield bool_option(
-                        label="footer",
-                        name="show_footer",
-                        switch_value=self.cfg['show_footer'],
-                        tooltip="show the footer at the bottom of the screen"
-                        )
-
-                yield bool_option(
-                        label="k9s",
-                        name="k9s-enabled",
-                        switch_value=self.cfg['k9s']['enabled'],
-                        tooltip="launch k9s, a k8s TUI dashboard when cluster is up"
-                        )
-
-            with Grid(classes="k9s-input-row"):
-                yield input_field(
-                        label="k9s_command",
-                        name="k9s-command",
-                        initial_value=self.cfg['k9s']['command'],
-                        placeholder="command to run when k9s starts",
-                        tooltip="if k9s is enabled, run this command when it starts"
-                        )
+
+            with Grid(id="logging-config-row-grid"):
+                with Grid(classes="selection-row"):
+                    label = Label("level:", classes="selection-label")
+                    label.tooltip = logging_tool_tip
+                    yield label
+
+                    yield Select(((line, line) for line in possible_levels),
+                                 id="log-level-select",
+                                 value=current_level)
+
+                yield input_field(label="file",
+                                  initial_value=logging_opt['file'],
+                                  name="file",
+                                  placeholder=XDG_STATE_HOME,
+                                  tooltip="File to log to. If provided, no console "
+                                          "logging will take place")
 
     def on_mount(self) -> None:
         """
         box border styling
         """
-        tui_title = "🖥️ [i]Configure[/] [#C1FF87]Terminal UI"
-        self.get_widget_by_id("tui-config").border_title = tui_title
-
-    @on(Switch.Changed)
-    def update_parent_config_for_switch(self, event: Switch.Changed) -> None:
-        """
-        update the parent app's config file yaml obj
-        """
-        truthy_value = event.value
-        switch_name = event.switch.name
-
-        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']
-
-        if "k9s" in switch_name:
-            name = switch_name.replace("k9s-","")
-            self.cfg['k9s'][name] = truthy_value
-            parent_cfg['k9s'][name] = truthy_value
-        else:
-            self.cfg[switch_name] = truthy_value
-            parent_cfg[switch_name] = truthy_value
+        log_title = "🪵[i]Configure[/] [#C1FF87]Logging"
+        self.get_widget_by_id("logging-config").border_title = log_title
 
+    @on(Select.Changed)
+    def update_parent_for_select(self, event: Select.Changed) -> None:
+        self.app.cfg['smol_k8s_lab']['log']['level'] = str(event.value)
         self.app.write_yaml()
 
     @on(Input.Changed)
     def update_parent_config_for_input(self, event: Input.Changed) -> None:
-        input = event.input
-        input_name = event.input.name
-
-        if "k9s" in input_name:
-            name = input_name.replace("k9s-","")
-            self.cfg['k9s'][name] = input.value
-            self.app.cfg['smol_k8s_lab']['tui']['k9s'][name] = input.value
-        else:
-            self.app.cfg['smol_k8s_lab']['tui'][input.name] = input.value
-
+        """
+        update self and parent app self config with changed input field
+        """
+        self.app.cfg['smol_k8s_lab']['log'][input.name] = event.input.value
         self.app.write_yaml()
 
 
-class AccessibilityWidget(Widget):
+class PasswordManagerConfig(Widget):
     def __init__(self, config: dict) -> None:
-        """ 
-        Accessibility widget to allow for configuring the bell and text to speech
-        """
         self.cfg = config
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """
-        Compose widget for configuring the tui experience
+        Compose widget for configuring the local password manager
         """
-        with Grid(id="accessibility-config"):
-
-            yield Label("These parameters are all related to accessibility, "
-                        "both in the TUI and CLI.",
+        with Container(id="password-manager-config"):
+            yield Label("Save app credentials to a local password manager vault. "
+                        "Only Bitwarden is supported at this time, but if enabled,"
+                        " Bitwarden can be used as your k8s external secret provider."
+                        " To avoid a password prompt, export the following env vars: "
+                        "BW_PASSWORD, BW_CLIENTID, BW_CLIENTSECRET",
                         classes="soft-text")
 
-            with Grid(id="bell-row"):
-
-                yield bool_option(
-                        label="bell_on_focus",
-                        name="bell-on_focus",
-                        switch_value=self.cfg['bell']['on_focus'],
-                        tooltip=(
-                            "Ring the terminal bell each time your focus "
-                            "changes to another element on the screen.")
-                        )
-
-                yield bool_option(
-                        label="bell_on_error",
-                        name="bell-on_error",
-                        switch_value=self.cfg['bell']['on_error'],
-                        tooltip=(
-                            "Ring the terminal bell anytime there's a warning "
-                            "or error"
-                            )
-                )
-
-            with Grid(id="tts-row"):
-                yield bool_option(
-                        label="TTS_screen_titles",
-                        name="text-to-speech-screen_titles",
-                        switch_value=self.cfg['text_to_speech']['screen_titles'],
-                        tooltip=(
-                            "Read aloud each screen title and description aloud."
-                            )
-                        )
-
-                yield bool_option(
-                        label="TTS_on_key_press",
-                        name="text-to-speech-on_key_press",
-                        switch_value=self.cfg['text_to_speech']['on_key_press'],
-                        tooltip=(
-                            "Only read aloud the element if the f5 key is pressed. "
-                            "This key will be configurable in the future."
-                            )
-                        )
-
-                yield bool_option(
-                        label="TTS_on_focus",
-                        name="text-to-speech-on_focus",
-                        switch_value=self.cfg['text_to_speech']['on_focus'],
-                        tooltip=(
-                            "On each focus of a new element on the screen, "
-                            "read aloud the element id, and value/tooltip if "
-                            "available."
-                            )
-                        )
-
-            yield input_field(
-                    label="speech_program",
-                    name="text-to-speech-speech_program",
-                    initial_value=self.cfg['text_to_speech']['speech_program'],
-                    placeholder="name of program for speech",
-                    tooltip=(
-                        "If text to speech is enabled, this is the name of"
-                        " the command line interface speech program. On "
-                        "macOS, we default to 'say'. On Linux we default to espeak"
-                        )
-                    )
+            enabled_tooltip = "enable storing passwords for apps in a password manager"
+            with Grid(id="password-manager-options-grid"):
+                yield bool_option("enabled",
+                                  self.cfg['enabled'],
+                                  "enabled",
+                                  enabled_tooltip)
+
+                with Grid(classes="selection-row"):
+                    label = Label("duplicate strategy:",
+                                  classes="radioset-row-label")
+                    label.tooltip = duplicate_tool_tip
+                    yield label
+
+                    current_value = self.cfg['duplicate_strategy']
+                    possible_values = ["ask", "edit", "duplicate", "no_action"]
+
+                    yield Select(((line, line) for line in possible_values),
+                                 id="duplicate-strategy-select",
+                                 value=current_value)
 
     def on_mount(self) -> None:
         """
         box border styling
         """
-        title = "♿️ [i]Configure[/] [#C1FF87]Accessibility"
-        self.get_widget_by_id("accessibility-config").border_title = title
+        pass_title = "🔒[i]Configure[/] [#C1FF87]Password Manager"
+        self.get_widget_by_id("password-manager-config").border_title = pass_title
 
     @on(Switch.Changed)
-    def update_parent_config_for_switch(self, event: Switch.Changed) -> None:
+    def update_parent_config(self, event: Switch.Changed) -> None:
         """
         update the parent app's config file yaml obj
         """
-        truthy_value = event.value
+        value = event.value
         switch_name = event.switch.name
+        self.app.cfg['smol_k8s_lab']['local_password_manager'][switch_name] = value
+        self.app.write_yaml()
 
-        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']['accessibility']
+    @on(Select.Changed)
+    def update_parent_for_select(self, event: Select.Changed) -> None:
+        password_cfg = self.app.cfg['smol_k8s_lab']['local_password_manager']
+        password_cfg['duplicate_strategy'] = str(event.value)
+        self.app.write_yaml()
 
-        if "text-to-speech" in switch_name:
-            name = switch_name.replace("text-to-speech-", "")
-            parent_cfg['text_to_speech'][name] = truthy_value
-        else:
-            name = switch_name.replace("bell-", "")
-            parent_cfg['bell'][name] = truthy_value
 
+class RunCommandConfig(Widget):
+    def __init__(self, config: dict) -> None:
+        self.cfg = config
+        super().__init__()
+
+    def compose(self) -> ComposeResult:
+        """
+        Compose widget for configuring run-command
+        """
+        tip = ("If window behavior is set to same window, command runs "
+               "[i]after[/i] smol-k8s-lab has completed.")
+        # run-command config for log.level and log.file
+        with Grid(id="run-command-config"):
+
+            yield Label(tip, classes="soft-text")
+
+            with Grid(id="run-command-config-row-grid"):
+                with Grid(classes="selection-row"):
+                    label = Label("terminal:", classes="selection-label")
+                    label.tooltip = (
+                            "terminal to use for running command in split pane,"
+                            " new tab, or new window. Not used if [b]window "
+                            "behavior[/b] set to [b]same window[/b]"
+                            )
+                    yield label
+
+                    yield Select(((line, line) for line in ['wezterm', 'zellij']),
+                                 id="terminal-select",
+                                 name="terminal",
+                                 value=self.cfg['terminal'],
+                                 allow_blank=False)
+
+                window_behavior_list = ['same window', 'split left', 'split right',
+                                        'split top', 'split bottom', 'new tab',
+                                        'new window']
+
+                with Grid(classes="selection-row"):
+                    label = Label("window behavior:", classes="selection-label")
+                    label.tooltip = (
+                            "terminal to use for running command in split pane,"
+                            " new tab, or new window. Not used if window "
+                            "behavior set to default"
+                            )
+                    yield label
+
+                    yield Select(((line, line) for line in window_behavior_list),
+                                 id="window-behavior-select",
+                                 value=self.cfg['window_behavior'],
+                                 allow_blank=False)
+
+            yield input_field(label="command",
+                              initial_value=self.cfg['command'],
+                              name="command",
+                              placeholder="command to run after config stage",
+                              tooltip="Command to run at start of CLI phase")
+
+    def on_mount(self) -> None:
+        """
+        box border styling
+        """
+        self.border_title = "💻 [i]Configure[/] [#C1FF87]command to run after config"
+
+    @on(Select.Changed)
+    def update_parent_for_select(self, event: Select.Changed) -> None:
+        if event.select.name == "terminal":
+            self.app.cfg['smol_k8s_lab']['run_command']['terminal'] = str(event.value)
+        else:
+            self.app.cfg['smol_k8s_lab']['run_command']['window_behavior'] = str(event.value)
         self.app.write_yaml()
 
     @on(Input.Changed)
     def update_parent_config_for_input(self, event: Input.Changed) -> None:
-        parent_cfg = self.app.cfg['smol_k8s_lab']['tui']['accessibility']
-        parent_cfg['text_to_speech']['speech_program'] = event.input.value
-
+        """
+        update self and parent app self config with changed input field
+        """
+        self.app.cfg['smol_k8s_lab']['run_command'][event.input.name] = event.input.value
         self.app.write_yaml()
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -234,55 +234,72 @@
     return Horizontal(bool_label, switch, classes=f"bool-switch-row {extra_class}")
 
 
 def drop_down(values: list,
               name: str,
               tooltip: str,
               select_value: str = "",
-              label: str = "") -> Horizontal:
+              label: str = "",
+              extra_row_class: str = "") -> Horizontal:
     """
     returns a label and switch row in a Horizontal container
     """
     if label:
-        select_label = Label(label.replace("_", " ") + ":", classes="input-row-label")
+        select_label = Label(label.replace("_", " ") + ":",
+                             classes="input-row-label")
         select_label.tooltip = tooltip
         id = label.replace("_", "-")
     else:
         id = name.replace("_", "-")
 
     select = Select.from_values(values,
                                 name=name,
                                 value=select_value,
                                 classes="dropdown-row-dropdown",
                                 id=id
                                 )
     select.tooltip = tooltip
 
-    extra_class = name.replace('_',"-")
-    if label:
-        return Horizontal(select_label, select,
-                          classes=f"{extra_class}")
+    if extra_row_class:
+        classes = f"input-row {name.replace('_',"-")} {extra_row_class}"
     else:
-        return Horizontal(select, classes=f"{extra_class}")
+        classes = f"input-row {name.replace('_',"-")}"
 
+    if label:
+        return Horizontal(select_label, select, classes=classes)
+    else:
+        return Horizontal(select, classes=classes)
 
-def input_field(label: str, initial_value: str, name: str, placeholder: str,
-                tooltip: str = "") -> Horizontal:
+def input_field(label: str,
+                initial_value: str,
+                name: str,
+                placeholder: str,
+                tooltip: str = "",
+                validate_empty: bool = False,
+                extra_row_class: str = "") -> Horizontal:
     """
     returns an input label and field within a Horizontal container
     """
     input_label = Label(label.replace("_", " ") + ":", classes="input-row-label")
     input_label.tooltip = tooltip
 
     input_dict = {"placeholder": placeholder,
                   "classes": "input-row-input",
-                  "id": label.replace("_","-"),
+                  "id": label.replace("_","-").replace(" ", "-"),
                   "name": name}
     if initial_value:
         input_dict["value"] = initial_value
     else:
         input_dict["value"] = ""
 
+    if validate_empty:
+        input_dict["validators"] = [Length(1)]
+
     input = Input(**input_dict)
     input.tooltip = tooltip
 
-    return Horizontal(input_label, input, classes="input-row")
+    if extra_row_class:
+        classes = f"input-row {extra_row_class}"
+    else:
+        classes = "input-row"
+
+    return Horizontal(input_label, input, classes=classes)
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     help_dict = {
         'delete':
         'Delete an existing cluster by name.',
 
         'interactive':
         '⚙️ Interactively configures smol-k8s-lab',
 
+        'command':
+        'Run command immediately after smol-k8s-lab before main cli phase',
+
         'version':
         f'Print the version of smol-k8s-lab (v{VERSION})'
         }
 
     if RECORD:
         help_dict['config'] = (
         'Full path and name of the YAML config file to parse.\nDefaults to '
```

### Comparing `smol_k8s_lab-4.0.2/smol_k8s_lab/utils/subproc.py` & `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/subproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 so during long running commands, the user isn't wondering what's going on,
 even if you don't actually output anything from stdout/stderr of the command.
 """
 import logging as log
 from subprocess import Popen, PIPE
 import re
 from rich.console import Console
+from rich.markup import MarkupError
 from rich.theme import Theme
 from rich.progress import Progress
 from time import sleep
 
 
 soft_theme = Theme({"info": "dim cornflower_blue",
                     "warn": "bold black on yellow",
@@ -87,22 +88,21 @@
     return output
 
 
 def run_subprocess(command: str, decode_ascii: bool = False, **kwargs):
     """
     Takes a str commmand to run in BASH in a subprocess.
     Typically run from subproc, which handles output printing.
-    error_ok=False, directory="", shell=False
     Optional keyword vars:
         error_ok  - bool, catch errors, defaults to False
         cwd       - str, current working dir which is the dir to run command in
-        shell     - bool, run shell or not
         env       - environment variables you'd like to pass in
-        decode_ascii - decode ascii strings instead of the default UTF-8
+        shell     - bool, run shell or not
         text, universal_newlines - allow for "" in commands
+        decode_ascii - decode ascii strings instead of the default UTF-8
     """
     # get the values if passed in, otherwise, set defaults
     quiet = kwargs.pop('quiet', False)
     error_ok = kwargs.pop('error_ok', False)
 
     try:
         if kwargs.get('universal_newlines', None):
@@ -129,15 +129,21 @@
         res_stdout = ansi_escape.sub('', res[0].decode('UTF-8'))
         res_stderr = ansi_escape.sub('', res[1].decode('UTF-8'))
     else:
         res_stdout, res_stderr = res[0].decode('UTF-8'), res[1].decode('UTF-8')
 
     # if quiet = True, or res_stdout is empty, we hide this
     if res_stdout and not quiet:
-        log.info(res_stdout)
+        try:
+            log.info(res_stdout)
+        except MarkupError:
+            log.debug(
+                "Rich logging errored because there's special characters in the"
+                " output and rich can't render the markdown.")
+            log.info(res_stdout, extra={"markup": False})
 
     if res_stderr and not quiet:
         log.info(res_stderr)
 
     # check return code, raise error if failure
     if not return_code or return_code != 0:
         # also scan both stdout and stdin for weird errors
@@ -152,15 +158,15 @@
 
     # sometimes stderr is empty, but sometimes stdout is empty
     for output in [res_stdout, res_stderr]:
         if output:
             return output
 
 
-def simple_loading_bar(tasks: dict, time_to_wait: int = 120):
+def simple_loading_bar(tasks: dict, time_to_wait: int = 120) -> None:
     """
     Prints a small loading bar using rich.
     Accepts a dict of {"task_name": "task"}
     example: {'Installing custom resource', 'kubectl apply -f thing.yml'}
 
     read more here:
         https://rich.readthedocs.io/en/stable/progress.html
```

### Comparing `smol_k8s_lab-4.0.2/PKG-INFO` & `smol_k8s_lab-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 4.0.2
+Version: 5.0.0
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Installation/Setup
-Requires-Dist: bcrypt (>=4.0,<5.0)
+Requires-Dist: bcrypt (>=4.1,<5.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: cryptography (>=42.0,<43.0)
 Requires-Dist: kubernetes (>=29,<30)
 Requires-Dist: minio (>=7.2,<8.0)
 Requires-Dist: pyfiglet (>=1.0,<2.0)
+Requires-Dist: pygame (>=2.5.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: ruamel-yaml (>=0.18,<0.19)
 Requires-Dist: ruamel-yaml-string (>=0.1,<0.2)
-Requires-Dist: textual (>=0.56,<0.57)
+Requires-Dist: textual (>=0.60,<0.61)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
 Project-URL: Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues
 Project-URL: Documentation, https://small-hack.github.io/smol-k8s-lab
 Project-URL: Repository, http://github.com/small-hack/smol-k8s-lab
 Description-Content-Type: text/markdown
 
 <h2 align="center">
@@ -65,15 +66,15 @@
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
 # Installation
-B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` or `brew`.
+B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon).
 
 ## pipx
 `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https://small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able to:
 
 ```bash
 # install the CLI
 pipx install smol-k8s-lab
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 4.0.2 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.0.0 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
-Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
+Author-email: jessebot@linux.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: System ::
-Installation/Setup Requires-Dist: bcrypt (>=4.0,<5.0) Requires-Dist: click
+Installation/Setup Requires-Dist: bcrypt (>=4.1,<5.0) Requires-Dist: click
 (>=8.1,<9.0) Requires-Dist: cryptography (>=42.0,<43.0) Requires-Dist:
 kubernetes (>=29,<30) Requires-Dist: minio (>=7.2,<8.0) Requires-Dist: pyfiglet
-(>=1.0,<2.0) Requires-Dist: pyjwt (>=2.8,<3.0) Requires-Dist: pyyaml
-(>=6.0,<7.0) Requires-Dist: requests (>=2.28,<3.0) Requires-Dist: rich
-(>=13.0,<14.0) Requires-Dist: ruamel-yaml (>=0.18,<0.19) Requires-Dist: ruamel-
-yaml-string (>=0.1,<0.2) Requires-Dist: textual (>=0.56,<0.57) Requires-Dist:
-xdg-base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/small-
-hack/smol-k8s-lab/issues Project-URL: Documentation, https://small-
-hack.github.io/smol-k8s-lab Project-URL: Repository, http://github.com/small-
-hack/smol-k8s-lab Description-Content-Type: text/markdown
+(>=1.0,<2.0) Requires-Dist: pygame (>=2.5.2,<3.0.0) Requires-Dist: pyjwt
+(>=2.8,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
+(>=2.28,<3.0) Requires-Dist: rich (>=13.0,<14.0) Requires-Dist: ruamel-yaml
+(>=0.18,<0.19) Requires-Dist: ruamel-yaml-string (>=0.1,<0.2) Requires-Dist:
+textual (>=0.60,<0.61) Requires-Dist: xdg-base-dirs (>=6.0,<7.0) Project-URL:
+Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues Project-URL:
+Documentation, https://small-hack.github.io/smol-k8s-lab Project-URL:
+Repository, http://github.com/small-hack/smol-k8s-lab Description-Content-Type:
+text/markdown
   ********** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ccaattppppuucccciinn//ccaattppppuucccciinn//mmaaiinn//aasssseettss//
 mmiisscc//ttrraannssppaarreenntt..ppnngg]]?ð??§?¸ ssmmooll--kk88ss--llaabb_[[_hh_tt_tt_pp_ss_::_//_//_ii_mm_gg_.._ss_hh_ii_ee_ll_dd_ss_.._ii_oo_//_gg_ii_tt_hh_uu_bb_//_vv_//_rr_ee_ll_ee_aa_ss_ee_//
                              _ss_mm_aa_ll_ll_--_hh_aa_cc_kk_//_ss_mm_oo_ll_--_kk_88_ss_--
  _ll_aa_bb_??_ss_tt_yy_ll_ee_==_pp_ll_aa_ss_tt_ii_cc_&&_ll_aa_bb_ee_ll_CC_oo_ll_oo_rr_==_44_88_44_88_44_88_&&_cc_oo_ll_oo_rr_==_33_CC_AA_33_22_44_&&_ll_oo_gg_oo_==_GG_ii_tt_HH_uu_bb_&&_ll_oo_gg_oo_CC_oo_ll_oo_rr_==_ww_hh_ii_tt_ee_]]
                                      **********
  A terminal based tool to install slimmer k8s distros on metal, with batteries
                                    included!
@@ -39,27 +40,27 @@
 (#supported-k8s-distributions) - Specializes in using Bitwarden (though not
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
 hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - Lots o' [docs](https://
 small-hack.github.io/smol-k8s-lab) # Installation B sure to check out our full
 [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
-but the gist of it is `smol-k8s-lab` can be installed via `pipx` or `brew`. ##
-pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
-pipx)). If you've already got both and [other pre-reqs](https://small-
-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
-to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
-before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
-the future preferred installation method for macOS/Debian/Ubuntu, as this will
-also install any non-python prerequisites you need, so you don't need to worry
-about them. This method is new, so please [let us know if anything isn't
-working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
-tap the special homebrew repo for our formula and install it brew install
-small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
-and cli options with: ```bash smol-k8s-lab --help ```
+but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
+coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
+github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
+/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
+able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
+menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
+[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
+as this will also install any non-python prerequisites you need, so you don't
+need to worry about them. This method is new, so please [let us know if
+anything isn't working for you](https://github.com/small-hack/homebrew-tap/
+issues). ```bash # tap the special homebrew repo for our formula and install it
+brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
+the version and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
```

