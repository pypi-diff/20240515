# Comparing `tmp/freva_deployment-2309.0.1.tar.gz` & `tmp/freva_deployment-2405.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2309.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freva_deployment-2405.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freva_deployment-2309.0.1.tar` & `freva_deployment-2405.0.0.tar`

### file list

```diff
@@ -1,86 +1,108 @@
--rw-r--r--   0        0        0      125 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      121 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/dependabot/constraints.txt
--rw-r--r--   0        0        0     2755 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/build_job.yml
--rw-r--r--   0        0        0     2051 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/ci_job.yml
--rw-r--r--   0        0        0     1577 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/docker_job.yml
--rw-r--r--   0        0        0      918 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/pypi_job.yml
--rw-r--r--   0        0        0      318 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.gitignore
--rw-r--r--   0        0        0     1301 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      135 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1078 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/LICENSE
--rw-r--r--   0        0        0       15 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/MANIFEST.in
--rw-r--r--   0        0        0    15470 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/README.md
--rw-r--r--   0        0        0    11564 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/config/create_tables.sql
--rw-r--r--   0        0        0     2578 2023-09-15 05:58:20.422150 freva_deployment-2309.0.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
--rw-r--r--   0        0        0    10590 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/config/inventory.toml
--rw-r--r--   0        0        0     1360 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/password_rotate.py
--rw-r--r--   0        0        0      388 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/reset_root_pw.sh
--rw-r--r--   0        0        0     5040 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/core-server-playbook.yml
--rw-r--r--   0        0        0     5830 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/db-server-playbook.yml
--rw-r--r--   0        0        0     1957 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/server-map-playbook.yml
--rw-r--r--   0        0        0     3815 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/solr-server-playbook.yml
--rw-r--r--   0        0        0     3584 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/vault-server-playbook.yml
--rw-r--r--   0        0        0     7769 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/web-server-playbook.yml
--rwxr-xr-x   0        0        0      351 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_cron.sh
--rw-r--r--   0        0        0     4182 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_systemd.py
--rwxr-xr-x   0        0        0    16851 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/docker-or-podman
--rwxr-xr-x   0        0        0       66 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/dump_sql
--rwxr-xr-x   0        0        0      160 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/prepare-httpd
--rw-r--r--   0        0        0      527 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/Dockerfile
--rw-r--r--   0        0        0      102 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/freva/servers.toml
--rw-r--r--   0        0        0     5857 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/restservice.py
--rw-r--r--   0        0        0      686 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/Dockerfile
--rw-r--r--   0        0        0     1398 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/deploy_vault.py
--rw-r--r--   0        0        0       50 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/policy-file.hcl
--rw-r--r--   0        0        0     4934 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/runserver.py
--rw-r--r--   0        0        0      175 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
--rw-r--r--   0        0        0      569 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/vault-server-tls.hcl
--rwxr-xr-x   0        0        0     2305 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/Dockerfile
--rwxr-xr-x   0        0        0       38 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/docker_cmd.sh
--rwxr-xr-x   0        0        0       17 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/entrypoint.sh
--rw-r--r--   0        0        0    15874 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/freva_web.conf
--rw-r--r--   0        0        0     6965 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/AfterDeployment.md
--rw-r--r--   0        0        0     5483 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Architecture.md
--rwxr-xr-x   0        0        0    43499 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Concept_Map.png
--rw-r--r--   0        0        0     8596 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Configure.md
--rw-r--r--   0        0        0     6837 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Folders.md
--rw-r--r--   0        0        0     5998 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Installation.md
--rw-r--r--   0        0        0    11811 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/LegalNotes.md
--rw-r--r--   0        0        0      634 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Makefile
--rw-r--r--   0        0        0     2238 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Services.md
--rw-r--r--   0        0        0    57311 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography.png
--rwxr-xr-x   0        0        0    41164 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_1.png
--rwxr-xr-x   0        0        0    29463 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_2.png
--rwxr-xr-x   0        0        0    46480 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_3.png
--rw-r--r--   0        0        0    12634 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Transition.md
--rw-r--r--   0        0        0    16780 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/TuiHowto.md
--rw-r--r--   0        0        0    14354 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Variable.png
--rw-r--r--   0        0        0     3430 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/conf.py
--rw-r--r--   0        0        0      288 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/environment.yml
--rw-r--r--   0        0        0   119110 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/freva_flowchart-new.jpg
--rw-r--r--   0        0        0     8432 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/freva_owl.svg
--rw-r--r--   0        0        0     2412 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/make.bat
--rw-r--r--   0        0        0      649 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/modules.rst
--rw-r--r--   0        0        0   153459 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_core.png
--rw-r--r--   0        0        0    76747 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_db.png
--rw-r--r--   0        0        0    95292 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_run.png
--rw-r--r--   0        0        0    70322 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_solr.png
--rw-r--r--   0        0        0   153250 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_web.png
--rw-r--r--   0        0        0      750 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/mypy.ini
--rw-r--r--   0        0        0       89 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/pyinstaller/pyinstaller-script.py
--rw-r--r--   0        0        0     1862 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/pyproject.toml
--rw-r--r--   0        0        0      221 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/__init__.py
--rw-r--r--   0        0        0      394 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/__init__.py
--rw-r--r--   0        0        0     2256 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0        0        0     7596 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0        0        0     4095 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0        0        0     7203 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_service.py
--rw-r--r--   0        0        0    24342 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/deploy.py
--rw-r--r--   0        0        0        0 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/__init__.py
--rw-r--r--   0        0        0     1701 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0        0        0    13254 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0        0        0    35152 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0        0        0    10252 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0        0        0    11889 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/utils.py
--rw-r--r--   0        0        0    17151 1970-01-01 00:00:00.000000 freva_deployment-2309.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.dockerignore
+-rw-r--r--   0        0        0      125 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      121 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/dependabot/constraints.txt
+-rw-r--r--   0        0        0     2946 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/workflows/build_containers.yml
+-rw-r--r--   0        0        0     3693 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/workflows/build_job.yml
+-rw-r--r--   0        0        0     1192 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/workflows/bump_version.yml
+-rw-r--r--   0        0        0     1230 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.github/workflows/ci_job.yml
+-rw-r--r--   0        0        0      346 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.gitignore
+-rw-r--r--   0        0        0     1301 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      135 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      935 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/Dockerfile
+-rw-r--r--   0        0        0     1078 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      449 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/Makefile
+-rw-r--r--   0        0        0    15618 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/README.md
+-rw-r--r--   0        0        0    11564 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/config/create_tables.sql
+-rw-r--r--   0        0        0     2578 2024-05-15 11:58:35.387537 freva_deployment-2405.0.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
+-rw-r--r--   0        0        0    11849 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/config/inventory.toml
+-rw-r--r--   0        0        0    11896 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/config/unprivileged-user.toml
+-rw-r--r--   0        0        0     1360 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/db_service/password_rotate.py
+-rw-r--r--   0        0        0      388 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/db_service/reset_root_pw.sh
+-rw-r--r--   0        0        0     6772 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/core-server-playbook.yml
+-rw-r--r--   0        0        0     1370 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/db-server-compose-template.yml
+-rw-r--r--   0        0        0     9150 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/db-server-playbook.yml
+-rw-r--r--   0        0        0     1866 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/freva_rest-server-compose-template.yml
+-rw-r--r--   0        0        0     7280 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/freva_rest-server-playbook.yml
+-rw-r--r--   0        0        0     2325 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/versions.yaml
+-rw-r--r--   0        0        0     3019 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/web-server-compose-template.yml
+-rw-r--r--   0        0        0     9360 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/playbooks/web-server-playbook.yml
+-rwxr-xr-x   0        0        0     1036 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/create_cron.sh
+-rw-r--r--   0        0        0     4754 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/create_systemd.py
+-rwxr-xr-x   0        0        0    18447 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/docker-or-podman
+-rwxr-xr-x   0        0        0     1856 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/download.py
+-rwxr-xr-x   0        0        0       66 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/dump_sql
+-rwxr-xr-x   0        0        0      792 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/inspect.sh
+-rwxr-xr-x   0        0        0      160 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/prepare-httpd
+-rw-r--r--   0        0        0     1067 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/Dockerfile
+-rw-r--r--   0        0        0     1005 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/add-vault-secret
+-rw-r--r--   0        0        0     1610 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/checks.py
+-rw-r--r--   0        0        0     1398 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/deploy_vault.py
+-rw-r--r--   0        0        0      246 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/mypy.ini
+-rw-r--r--   0        0        0       80 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/policy-file.hcl
+-rwxr-xr-x   0        0        0     9196 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/runserver.py
+-rw-r--r--   0        0        0      175 2024-05-15 11:58:34.899534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
+-rw-r--r--   0        0        0      190 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/assets/share/freva/deployment/vault/vault-server-tls.hcl
+-rwxr-xr-x   0        0        0     2305 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/assets/share/freva/deployment/web/Dockerfile
+-rwxr-xr-x   0        0        0       38 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/assets/share/freva/deployment/web/docker_cmd.sh
+-rwxr-xr-x   0        0        0       17 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/assets/share/freva/deployment/web/entrypoint.sh
+-rw-r--r--   0        0        0    16008 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/assets/share/freva/deployment/web/freva_web.conf
+-rwxr-xr-x   0        0        0     4095 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/cloud-init/start-vm.sh
+-rwxr-xr-x   0        0        0    43499 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/Concept_Map.png
+-rw-r--r--   0        0        0      634 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/_static/.keep
+-rw-r--r--   0        0        0     8432 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/_static/freva_owl.svg
+-rw-r--r--   0        0        0     4595 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/after-deployment/AfterDeployment.md
+-rw-r--r--   0        0        0    11811 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/after-deployment/LegalNotes.md
+-rw-r--r--   0        0        0     9862 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/after-deployment/TransitionPlugins.md
+-rw-r--r--   0        0        0     2783 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/after-deployment/TransitionService.md
+-rw-r--r--   0        0        0      427 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/after-deployment/index.rst
+-rw-r--r--   0        0        0     5510 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/Architecture.md
+-rw-r--r--   0        0        0     6832 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/Folders.md
+-rwxr-xr-x   0        0        0    43499 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/Concept_Map.png
+-rw-r--r--   0        0        0    57311 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/Topography.png
+-rwxr-xr-x   0        0        0    41164 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/Topography_1.png
+-rwxr-xr-x   0        0        0    29463 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/Topography_2.png
+-rwxr-xr-x   0        0        0    46480 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/Topography_3.png
+-rw-r--r--   0        0        0   119110 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/_static/freva_flowchart-new.jpg
+-rw-r--r--   0        0        0     2129 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/architecture/index.rst
+-rw-r--r--   0        0        0     4200 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/conf.py
+-rw-r--r--   0        0        0     3440 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/contributing.md
+-rw-r--r--   0        0        0    24540 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/deployment/Config.md
+-rw-r--r--   0        0        0    12942 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/deployment/Configure.md
+-rw-r--r--   0        0        0     3244 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/deployment/Installation.md
+-rw-r--r--   0        0        0    16690 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/deployment/TuiHowto.md
+-rw-r--r--   0        0        0    14354 2024-05-15 11:58:34.903534 freva_deployment-2405.0.0/docs/deployment/_static/Variable.png
+-rw-r--r--   0        0        0   153459 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/_static/tui_core.png
+-rw-r--r--   0        0        0    76747 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/_static/tui_db.png
+-rw-r--r--   0        0        0    95292 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/_static/tui_run.png
+-rw-r--r--   0        0        0    70322 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/_static/tui_solr.png
+-rw-r--r--   0        0        0   153250 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/_static/tui_web.png
+-rw-r--r--   0        0        0     1421 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/deployment/index.rst
+-rw-r--r--   0        0        0      132 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/environment.yml
+-rw-r--r--   0        0        0     2429 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/make.bat
+-rw-r--r--   0        0        0     1295 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/docs/whatsnew.rst
+-rw-r--r--   0        0        0      750 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/mypy.ini
+-rw-r--r--   0        0        0       89 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/pyinstaller/pyinstaller-script.py
+-rw-r--r--   0        0        0     2674 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/pyproject.toml
+-rw-r--r--   0        0        0    15726 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/release.py
+-rw-r--r--   0        0        0     1400 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0        0        0     7554 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0        0        0    36891 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/deploy.py
+-rw-r--r--   0        0        0     2813 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/error.py
+-rw-r--r--   0        0        0     5611 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/keys.py
+-rw-r--r--   0        0        0      602 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/logger.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/py.typed
+-rw-r--r--   0        0        0     1949 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/runner.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:58:34.907534 freva_deployment-2405.0.0/src/freva_deployment/ui/__init__.py
+-rw-r--r--   0        0        0     2113 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0        0        0    13384 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0        0        0    35764 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0        0        0    10872 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0        0        0    10774 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/utils.py
+-rw-r--r--   0        0        0      121 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/versions.json
+-rw-r--r--   0        0        0     2990 2024-05-15 11:58:34.911534 freva_deployment-2405.0.0/src/freva_deployment/versions.py
+-rw-r--r--   0        0        0    17358 1970-01-01 00:00:00.000000 freva_deployment-2405.0.0/PKG-INFO
```

### Comparing `freva_deployment-2309.0.1/.github/workflows/build_job.yml` & `freva_deployment-2405.0.0/.github/workflows/build_job.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,58 @@
-name: Building
-run-name: ${{ github.actor }} is building the tui 🧉
+name: Create a new release
+run-name: ${{ github.actor }} creating a new release 🧉
 
 # Set the access for individual scopes, or use permissions: write-all
 permissions:
   pull-requests: write
+  contents: write
+  packages: write
+
 on:
   push:
     tags:
-      - "*"
+      - "v*.*.*"
 
 jobs:
+  tests:
+    uses: ./.github/workflows/ci_job.yml
+  pypi:
+    name: Create Pip package
+    permissions:
+      id-token: write
+    needs: [tests]
+    runs-on: ubuntu-latest
+    steps:
+      -
+        name: Checkout
+        uses: actions/checkout@v4
+      -
+        name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+      - name: Adding the evaluation config file
+        run: python src/freva_deployment/__init__.py
+      -
+        name: Install flit
+        run: python -m pip install flit
+      -
+        name: Building freva-deployment 📦 with flit
+        run: flit build
+      -
+        name: publish distribution 📦 to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.PYPI_API_TOKEN }}
+          skip-existing: true
+          verbose: true
   createrelease:
     name: Create Release
     runs-on: [ubuntu-latest]
+    needs: pypi
     steps:
       - name: Create Release
         id: create_release
         uses: actions/create-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.ASSET_TOKEN }}
         with:
@@ -29,15 +65,15 @@
       - name: Save Release URL File for publish
         uses: actions/upload-artifact@v1
         with:
           name: release_url
           path: release_url.txt
   build:
     name: Build packages
-    needs: createrelease
+    needs: [pypi, createrelease]
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
           - os: macos-latest
             TARGET: macos
             CMD_BUILD: >
@@ -46,19 +82,19 @@
             ASSET_MIME: application/octet-stream
           - os: windows-latest
             TARGET: windows
             CMD_BUILD: pyinstaller pyinstaller/pyinstaller-script.py -c --name deploy-freva --onefile
             OUT_FILE_NAME: deploy-freva.exe
             ASSET_MIME: application/vnd.microsoft.portable-executable
     steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python 3.11
+      - uses: actions/checkout@v4
+      - name: Set up Python 3.X
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11
+          python-version: "3.X"
       - name: Install dependencies
         run: |
           python3 -m pip install --upgrade pip
           python3 -m pip install pyinstaller ansible .
       - name: Build with pyinstaller for ${{matrix.TARGET}}
         run: ${{matrix.CMD_BUILD}}
       - name: Load Release URL File from release job
```

### Comparing `freva_deployment-2309.0.1/.github/workflows/docker_job.yml` & `freva_deployment-2405.0.0/.github/workflows/ci_job.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,51 @@
-name: Build and publish the container image
-run-name: ${{ github.actor }} is building the container
-
-"on":
-  workflow_dispatch:
-  push:
-    branches:
-      - main
+name: CLI Test
+run-name: ${{ github.actor }} is testing the cli 🧉
 
+on: [push, workflow_call]
 jobs:
-  build-and-push-vault-image:
+  linting-and-testing:
     runs-on: ubuntu-latest
-    permissions:
-      contents: read
-      packages: write
     steps:
-      -
-        name: Checkout repository
-        uses: actions/checkout@v2
-        with:
-          fetch-depth: 0
+    -
+      name: Checkout
+      uses: actions/checkout@v4
+    -
+      name: Set up Python 3.11
+      uses: actions/setup-python@v4
+      with:
+        python-version: "3.11"
+    -
+      name: Install packages
+      run: |
+        python3 -m pip install tox
+        mkdir .mypy_cache
+    -
+      name: Running tests with tox
+      run: tox -p 3 --parallel-no-spinner
 
-      -
-        name: Get tag
-        id: repository
-        run: |
-          echo "repo=$(echo ${{ github.repository }}|tr 'A-Z' 'a-z')" >> $GITHUB_OUTPUT
-
-      -
-        name: Set up QEMU
-        uses: docker/setup-qemu-action@v1
+  vault-test:
+    name: Simple functional tests for the vault image
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
 
-      -
-        name: Set up Docker Buildx
+      - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v1
 
-      -
-        name: Log in to the Container registry
-        uses: docker/login-action@v2
-        with:
-          registry: ghcr.io
-          username: ${{ github.actor }}
-          password: ${{ secrets.GITHUB_TOKEN }}
-
-      -
-        name: Build and push vault image
+      - name: Build vault image
         uses: docker/build-push-action@v4
         with:
           context: assets/share/freva/deployment/vault/
           platforms: linux/amd64
-          push: true
-          tags: |
-            ghcr.io/${{ steps.repository.outputs.repo }}/vault:latest
+          push: false
+          load: true
+          tags: vault
 
-      -
-        name: Build and push server map image
-        uses: docker/build-push-action@v4
+      - name: Set up Python
+        uses: actions/setup-python@v4
         with:
-          context: assets/share/freva/deployment/servers/
-          platforms: linux/amd64
-          push: true
-          tags: |
-            ghcr.io/${{ steps.repository.outputs.repo }}/freva-map:latest
+          python-version: "3.x"
+
+      - name: Check vault image
+        run: python3 assets/share/freva/deployment/vault/checks.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `freva_deployment-2309.0.1/.gitlab-ci.yml` & `freva_deployment-2405.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/LICENSE` & `freva_deployment-2405.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/README.md` & `freva_deployment-2405.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,66 @@
+Metadata-Version: 2.1
+Name: freva-deployment
+Version: 2405.0.0
+Summary: Deployment of the Free Evaluation Framework Freva
+Author-email: "DKRZ, Clint" <freva@dkrz.de>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: appdirs
+Requires-Dist: ansible
+Requires-Dist: ansible-runner
+Requires-Dist: npyscreen
+Requires-Dist: PyMySQL
+Requires-Dist: PyYAML
+Requires-Dist: rich
+Requires-Dist: rich-argparse
+Requires-Dist: toml
+Requires-Dist: tomlkit
+Requires-Dist: requests
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: tox ; extra == "dev"
+Requires-Dist: pydata-sphinx-theme ; extra == "doc"
+Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: sphinx-copybutton ; extra == "doc"
+Requires-Dist: recommonmark ; extra == "doc"
+Requires-Dist: sphinx_sitemap ; extra == "doc"
+Requires-Dist: sphinx_favicon ; extra == "doc"
+Requires-Dist: sphinx_togglebutton ; extra == "doc"
+Requires-Dist: myst-parser ; extra == "doc"
+Requires-Dist: sphinx-design ; extra == "doc"
+Requires-Dist: linkify ; extra == "doc"
+Requires-Dist: sphinx-execute-code-python3 ; extra == "doc"
+Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
+Project-URL: Home, https://freva-deployment.readthedocs.io/en/latest
+Project-URL: Issues, https://github.com/FREVA-CLINT/freva-deployment/issues
+Project-URL: Source, https://github.com/FREVA-CLINT/freva-deployment
+Provides-Extra: dev
+Provides-Extra: doc
+
 # Deployment of the Free Evaluation Framework Freva
 
 [![Documentation Status](https://readthedocs.org/projects/freva-deployment/badge/?version=latest)](https://freva-deployment.readthedocs.io/en/latest/?badge=latest)
 
 The code in this repository is used to deploy freva in different computing
 environments. The general strategy is to split the deployment into
 4 different steps, these are :
 - Deploy MariaDB service via docker
 - Deploy a Hashicorp Vault service for storing and retrieving passwords
   and other sensitive data via docker
   (this step get automatically activated once the MariaDB service is set)
-- Deploy Apache Solr service via docker
+- Deploy [Databrowser API](https://github.com/FREVA-CLINT/databrowserAPI) service via docker
 - Deploy command line interface backend ([evaluation_system](https://github.com/FREVA-CLINT/freva))
-- Deploy web front end ([freva_web](https://gitlab.dkrz.de/freva/freva_web))
+- Deploy web front end ([freva_web](https://github.com/FREVA-CLINT/freva-web))
 
 
 > **_Note:_** A vault server is auto deployed once the mariadb server is deployed.
 The vault centrally stores all passwords and other sensitive data.
 During the deployment of the vault server a public key is generated which is
 used to open the vault. This public key will be saved in the `evaluation_system`
 backend root directory. Only if saved this key and the key in the vault match,
@@ -27,44 +72,19 @@
 install ansible via the `install_ansible` you'll have to use `conda` to
 install libselinux for your CentOS version.
 For example : `conda install -c conda-forge  libselinux-cos7-x86_64`
 
 # Pre-Requisites
 The main work will be done by
 [ansible](https://docs.ansible.com/ansible/latest/index.html), hence some level
-of familiarity with ansible is advantagous. Since we are using ansible we can
+of familiarity with ansible is advantageous. Since we are using ansible we can
 use this deployment routine from a workstation computer (like a Mac-book).
-You do not need to run the depoyment on the machines where things get installed.
+You do not need to run the deployment on the machines where things get installed.
 The only requirement is that you have to setup ansible and you can establish
 ssh connections to the servers.
-### Preparation on windows based system (without wsl).
-Currently ansible is not natively available on windows based systems. You can use
-the unix runtime environment [cygwin](https://www.cygwin.com) to download
-and install the needed software. Just follow the steps listed on the web page
-to setup cygwin on your windows system. In order to be able to install the
-freva deployment programm you'll first need to install the following packages
-via cygwin:
-
-- python3
-- python3-devel
-- git
-- make
-- python3.X-paramiko
-- libffi-devel
-- ansible
-
-We also recommend installing a command line based text editor like vim, nano, etc.
-
-After installing the above listed packages via cygwin you can clone and
-install the freva deployment:
-
-```console
-python3 -m pip install -U freva-deployment
-```
-Add the `--user` flag if you don't have sufficient rights.
 ## Installation on \*nix systems or wsl.
 If you're using Linux, OsX or a Windows subsystem for Linux (WSL) it should
 be sufficient to issues the following commands:
 
 ```console
 python3 pip install -U freva-deployment
 ```
@@ -73,14 +93,25 @@
 > **_Note:_** On *CentOS* python SELinux libraries need to be installed.
 > You will need to install libselinux for your CentOS version.
 
 ```console
 python3 -m pip install libselinux-python3
 ```
 
+## Using docker
+
+A pre-build docker image is available to run the deployment
+
+```console
+docker run -it -v /path/to/config:/opt/freva-deployment:z ghcr.io/freva-clint/freva-deployment
+```
+The `-it` flags are important in order to interact with the program. To use
+and save existing configurations you can mount the directories of the config
+files into the container.
+
 ## Commands after installation:
 The `pip install` command will create *four* different commands:
 - `deploy-freva-map`: To setup a service that keeps track of all deployed
    freva instances and their services.
 - `deploy-freva`: Text user interface to configure and run the deployment.
 - `deploy-freva-cmd`: Run already configured deployment.
 - `freva-service`: Start|Stop|Restart|Check services of freva instances.
@@ -92,56 +123,27 @@
 the following command to your local `.bashrc`:
 
 ```console
 export PATH=$PATH:$HOME/.local/bin
 ```
 
 
-## Installing docker/podman and sudo access to the service servers
-Since the services of MariaDB, Apache Solr and Apache web will be deployed on
-docker container images, docker needs to be available on the target servers.
-Usually installing and running docker requires *root* privileges.
-Hence, on the servers that will be running docker you will need root access.
-There exist an option to install and run docker without root,
-information on a root-less docker option
+## Installing docker-compose/podman-compose and sudo access to the service servers
+Because the services of MariaDB, DatabrowserAPI and Apache httpd will be deployed
+on docker container images, docker needs to be available on the target servers.
+Since version *v2309.0.0* of the deployment the containers are set up
+using `doker-compose`. Hence `docker-compose` (or `podman-compose`) has to be
+installed on the host systems. Usually installing and running docker
+requires *root* privileges. Hence, on the servers that will be running docker
+you will need root access. There exists an option to install and run docker
+without root, information on a root-less docker option
 can be found [on the docker docs](https://docs.docker.com/engine/security/rootless/)
 > **_Note:_** Some systems use `podman` instead of `docker`. The deployment
 routine is able to distinguish and use the right service.
 
-## Setting up a service that maps the server structure (Optional)
-Since the services might be scattered across different servers it might be hard
-to keep track of the host names of the servers where all services are running.
-We have created a service that keeps track of the locations of all services for
-a certain freva instance. Although not strictly needed we recommend you to setup
-this special server mapping service. To do so use the following command:
-
-```console
-deploy-freva-map --help
-usage: deploy-freva-map [-h] [--port PORT] [--wipe] [--user USER] [--python-path PYTHON_PATH] [-v] [-V] servername
-
-Create service that maps the freva server architecture.
-
-positional arguments:
-  servername            The server name where the infrastructure mapping service is deployed
-
-options:
-  -h, --help            show this help message and exit
-  --port PORT           The port the service is listing to (default: 6111)
-  --wipe                Delete any existing data. (default: False)
-  --user USER           Username to log on to the target server. (default: None)
-  --python-path PYTHON_PATH
-                        Path to the default python3 interpreter on the target machine. (default: /usr/bin/python)
-  -v, --verbose         Verbosity level (default: 0)
-  -V, --version         show program's version number and exit
-```
-> **_Note_:** As the service keeps track of all freva instances within your
-institution, this has to be deployed only *once*. Please make sure that other
-admins who might need to install freva are aware of the host name
-for this service. *This step is optional*
-
 # Configuring the deployment
 A complete freva instance will need the following services:
 
 - solrservers (hostname of the apache solr server)
 - dbservers (hostname of the MariaDB server)
 - webservers (hostname that will host the web site)
 - backendservers (hostname(s) where the command line interface will be installed)
@@ -196,70 +198,37 @@
 `migration` of an old freva system.
 
 ## Deployment with existing configuration.
 If you already have a configuration saved in a toml base inventory file you can
 issue the `deploy-freva-cmd` command:
 
 ```bash
-deploy-freva-cmd --help
-usage: deploy-freva-cmd [-h] [--server-map SERVER_MAP] [--config CONFIG]
-                        [--steps {services,web,core,db,solr,backup} [{services,web,core,db,solr,backup} ...]] [--ask-pass] [-v] [-V]
+eploy-freva-cmd --help
+usage: deploy-freva-cmd [-h] [--config CONFIG] [--steps {web,core,db,databrowser} [{web,core,db,databrowser} ...]] [--ask-pass] [--ssh-port SSH_PORT] [-v] [-l]
+                        [--gen-keys] [-V]
 
 Deploy freva and its services on different machines.
 
 options:
   -h, --help            show this help message and exit
-  --server-map SERVER_MAP
-                        Hostname of the service mapping the freva server archtiecture, Note: you can create a server map by running
-                        the deploy-freva-map command (default: None)
   --config CONFIG, -c CONFIG
-                        Path to ansible inventory file. (default: /home/wilfred/.config/freva/deployment/inventory.toml)
-  --steps {services,web,core,db,solr,backup} [{services,web,core,db,solr,backup} ...]
-                        The services/code stack to be deployed (default: ['services', 'web', 'core'])
+                        Path to ansible inventory file. (default: /home/wilfred/.anaconda3/share/freva/deployment/inventory.toml)
+  --steps {web,core,db,databrowser} [{web,core,db,databrowser} ...]
+                        The services/code stack to be deployed (default: ['db', 'databrowser', 'web', 'core'])
   --ask-pass            Connect to server via ssh passwd instead of public key. (default: False)
+  --ssh-port SSH_PORT   Set the ssh port, in 99.9% of the cases this should be 22 (default: 22)
   -v, --verbose         Verbosity level (default: 0)
+  -l, --local           Deploy services on the local machine, debug purpose. (default: False)
+  --gen-keys            Generate public and private web certs, use with caution. (default: False)
   -V, --version         show program's version number and exit
-```
-
-The `--steps` flags can be used if not all services should be deployed.
 
-# Accessing the services after deployment:
-If the target machine where the services (solr, mariadb, web) were deployed
-is a Linux machine you will have a `systemd` unit service was created.
-You can control the service via the `freva-service` command:
-
-```console
-freva-service --help
-usage: freva-service [-h] [--server-map SERVER_MAP] [--services {web,db,solr} [{web,db,solr} ...]] [--user USER] [-v] [-V]
-                     {start,stop,restart,status} [project_name]
-
-Interact with installed freva services.
-
-positional arguments:
-  {start,stop,restart,status}
-                        The start|stop|restart|status command for the service
-  project_name          Name of the project (default: all)
 
-options:
-  -h, --help            show this help message and exit
-  --server-map SERVER_MAP
-                        Hostname of the service mapping the freva server archtiecture, Note: you can create a server map by running
-                        the deploy-freva-map command (default: None)
-  --services {web,db,solr} [{web,db,solr} ...]
-                        The services to be started|stopped|restarted|checked (default: ['solr', 'db', 'web'])
-  --user USER, -u USER  connect as this user (default: None)
-  -v, --verbose         Verbosity level (default: 0)
-  -V, --version         show program's version number and exit
 ```
-The following command restarts `web` server for the `xces`:
-```console
-freva-service restart xces --services web --user k12345
-```
-All services (`db`, `web` and `solr`) will be selected if the `--services` option
-is omitted.
+
+The `--steps` flags can be used if not all services should be deployed.
 
 # Kown Issues:
 Below are possible solutions to some known issues:
 
 ### SSH connection fails:
 
 ```python
@@ -302,7 +271,123 @@
 git config --global user.name your_user
 git config --global user.email your@email.com
 ```
 
 
 # Advanced: Adjusting the playbook
 Playbook templates and be found the in the `playbooks` directory. You can also add new variables to the playbook if they are present in the `config/inventory` file.
+
+# Contributing to freva-deployment
+
+We welcome contributions from the community! Before you start contributing,
+please follow these steps to set up your development environment.
+Make sure you have the following prerequisites installed:
+
+- Python (>=3.x)
+- Git
+- Make
+
+```console
+git clone https://github.com/FREVA-CLINT/freva-deployment.git
+cd freva-deployment.git
+make
+```
+
+The deployment routine is supposed to interact with the user - this can
+can be asking for user names or passwords. To avoid such interaction you can
+set the following environment variables.
+
+- `MASTER_PASSWD`: the admin/root password for all services (db, web etc).
+- `EMAIL_USER`: the user name for email server login credentials.
+- `EMAIL_PASSWD`: the password for email server login credentials.
+- `ANSIBLE_BECOME_PASSWORD`: the password used in any *sudo* command.
+
+These environment variables have only an effect when the deployment is
+applied in debug or local mode using the `-l` flag.
+
+## Using a local VM for testing.
+A test freva instance can be deployed on a dedicated local virtual machine.
+This virtual machine is based on a minimal ubuntu server image and has
+docker and podman pre installed. To create the virtual machine simply
+run the following script.
+
+```console
+cloud-init/start-vm.sh -h
+```
+
+```bash
+Usage: start-vm.sh [-k|--kill], [-p|--port PORT]
+Create a new virtual machine (VM) ready for freva deployment.
+Options:
+  -k, --kill     Kill the virtual machine
+  -p, --port     Set the port of the service that is used to configure the VM default: 8000
+```
+
+> **_Note:_** *Before* running the script you will have to install [qemu](https://www.qemu.org/docs/master/).
+> The script has only been tested on Linux systems.
+
+You can then make use of the pre configured inventory file in
+`assets/share/freva/deployment/config/inventory.toml`. In order to deploy
+freva on the newly created VM you will have to instruct ansible to use
+ssh port 2222 instead of 22.
+
+The following command will install freva along all with it's components to
+the local VM:
+
+```console
+deploy-freva-cmd  assets/share/freva/deployment/config/inventory.toml --gen-keys --ssh-port 2222
+```
+
+If you want to tear down the created VM you can either press CTRL+C in the
+terminal where you created the VM or use the kill command:
+
+```console
+./cloud-init/start-vm.sh -k
+```
+
+## Development Workflow
+
+To install the code in development mode use:
+```console
+make
+```
+
+Unit tests, building the documentation, type annotations and code style tests
+are done with [tox](https://tox.wiki/en/latest/). To run all tests, linting
+in parallel simply execute the following command:
+
+```console
+tox -p 3
+```
+You can also run the each part alone, for example to only check the code style:
+
+```console
+tox -e lint
+```
+available options are ``lint``, ``types``, ``test`` and ``docs``.
+
+Tox runs in a separate python environment to run the tests in the current
+environment use:
+
+```console
+pytest
+```
+
+To reformat and do type checking:
+```console
+make lint
+```
+### Creating a new release.
+
+Once the development is finished and you decide that it's time for a new
+release of the software use the following command to trigger a release
+procedure:
+
+```console
+tox -e release
+```
+
+This will check the current version of the `main` branch and trigger
+a GitHub continuous integration pipeline to create a new release. The procedure
+performs a couple of checks, if theses checks fail please make sure to address
+the issues.
+
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/config/create_tables.sql` & `freva_deployment-2405.0.0/assets/share/freva/deployment/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl` & `freva_deployment-2405.0.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [evaluation_system]
 # Freva - Free Evaluation System Framework configuration file
 # This file contains the necessary configuration information
 # which is needed to run freva
 #
-# Username(s) - comma separated - of the admins of the proejct
+# Username(s) - comma separated - of the admins of the project
 admins=
 #
-# An Infromative project name
+# An Informative project name
 project_name=freva
 # The url the freva web ui can be accessed with
 project_website=
 
 # Main configuration path of the freva instance default to the etc dir
 # of the python environment
 root_dir=
@@ -20,15 +20,15 @@
 #: Type of directory structure that will be used to maintain state:
 #:
 #:    local   := <home>/<base_dir>...
 #:    central := <base_dir_location>/<username>/<base_dir>...
 #:
 directory_structure_type=central
 
-# The location of the work direcotry for is user specific data
+# The location of the work directory for is user specific data
 # This setting will have no effect if you have set the `directory_structure_type`
 # to central
 base_dir_location=${root_dir}/freva_output
 
 # The directory name of the <base_dir> (only used if `directory_structure_type`
 # is set to central - defaults to `project_name`
 base_dir=${project_name}
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/config/inventory.toml` & `freva_deployment-2405.0.0/assets/share/freva/deployment/config/unprivileged-user.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,238 +1,254 @@
-# This is the "defaut" freva deployment configuration file.
+# This is the "default" freva deployment configuration file.
 #
 #   - The files syntax follows the `toml` markup language (https://toml.io)
 #   - Comments begin with the "#" character
 #   - Blank lines are ignored
 #   - Groups of hosts are delimited by [header] elements
 #   - The groups define different deployment steps
-#   - Additional configuration for each group is set in the confg section
+#   - Additional configuration for each group is set in the config section
 #     of each header -> [header.config]
-#   - You can enter hostnames or ip addresses
-#   - A hostname/ip can be a member of multiple groups
+#   - You can enter host names or IP addresses
+#   - A host name/IP can be a member of multiple groups
 
 
 ## The first part of this configuration defines general configuration that
 ## is common among all deployment steps.
 
-# The the project name that should be used for this freva instance
+# The project name that should be used for this freva instance
 # NOTE: this key has to be the first in the file
-project_name = ""
+project_name = "freva-local"
 
-## Set the path to the SSL certfificate files that is used to make password
-## queries to the vault server or used as web certfificates.
+## Set the path to the SSL certificate files that is used to make password
+## queries to the vault server or used as web certificates.
 [certificates]
 
-## Path to the public keyfile
+## Path to the public key file
 public_keyfile = ""
 
-## Path to the private keyfile
-privat_keyfile = ""
+## Path to the private key file
+private_keyfile = ""
 
 ## Path to the chain file
 chain_keyfile = ""
 
 
 
 [web]
-# Set the hostnames where all services web ui will be deployed
-hosts = ""
+# Set the host names where all services web UI will be deployed
+hosts = "localhost"
 
 # If you have multiple hosts following a pattern you can specify
 # them like this:
 
 ## hosts = "alpha.example.org,beta.example.org,192.168.1.100,192.168.1.110"
 ## hosts = "www[001:006].example.com"
 
 ## Ex : A collection of database servers in the "dbservers" group
 
 ## Here"s another example of host ranges, this time there are no
 ## leading 0s:
 
 ## hosts = "db-[99:101]-node.example.com"
-[solr]
-## Set the hostnames running the apache solr service
-hosts = ""
+[freva_rest]
+## Set the host names running the freva-rest service
+hosts = "localhost"
 
 [db]
-## Set the hostnames running the mariadb service
-hosts = ""
+## Set the host names running the mariadb service
+hosts = "localhost"
 
 [core]
-### Set the hostnames where the command line interface of freva will be installed
-hosts = ""
+### Set the host names where the command line interface of freva will be installed
+hosts = "localhost"
 
 
 ### CONFIGURATION VARIABLES
 ##The following section defines important variables, which have to be set
 ##in order to deploy the system correctly
 ##
 [db.config]
 
 ## Config variables for the database service
-port = 3306
-user = ""
-db = ""
+port = 3307
+user = "freva"
+db = "frevadb"
 
-##If you need a different user name you can set it here:
-#ansible_user = "username"
+##If you need a different user name you can set it here (defaults to current user):
+ansible_user = "freva"
 
-## You can set the db_host seperately, if none is given (default)
-## the one from the hostsnames above are taken
+## You can set the db_host separately, if none is given (default)
+## the one from the hosts names above are taken
 
-db_host = ""
+db_host = "freva"
 
 ## Set the become (sudo) user name to change to for installing the services
-ansible_become_user = "root"
+## leave blank to utilise a non privileged user based installation
+ansible_become_user = ""
 
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
-#ansible_python_interpreter = ""
-
-##If you need a different user name you can set it here:
-
-#ansible_python_interpreter="/usr/bin/python3"
+ansible_python_interpreter = ""
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
-##(Useful for a truely fresh start) (default: False)
+##(Useful for a truly fresh start) (default: False)
 wipe = false
 
+## Set the path where the permanent database data should be stored. By default
+## this is set to /opt/freva/<project_name>/db_service
+data_path = "~/freva-local/services"
+
 ## In case you want to set a custom path to a ansible playbook,
 ## you can do this here, by default the deployment will use the playbook
 ## located in the user config directory.
 ## NOTE: only adjust this if you know what you are doing, if you leave this
 ## blank the system will used the default playbook (standard procedure)
 db_playbook = ""
-vault_playbook = ""
 
-[solr.config]
-## Config variables for the solr service
-port = 8983
+[freva_rest.config]
+# Set the memory for the solr server (solr is the search engine in the background)
+solr_mem = "1g"
 
-# Set the memory for the solr server
-mem = "4g"
+# Set the port the freva-rest should be running on
+freva_rest_port = 7778
 
 ## Set the become (sudo) user name to change to for installing the services
-ansible_become_user = "root"
+## leave blank to utilise a non privileged user based installation
+ansible_become_user = ""
 
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
 
-#ansible_python_interpreter = ""
+ansible_python_interpreter = ""
 
-## If you need a different user name you can set it here:
-#ansible_user = "username"
+## If you need a different user name you can set it here (default to current user):
+ansible_user = "freva"
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
-##(Useful for a truely fresh start) (default: False)
+##(Useful for a truly fresh start) (default: False)
 wipe = false
+
+## Set the path where the permanent freva-rest data should be stored.
+## By default this is set to /opt/freva
+data_path = "~/freva-local/services"
+
 ## In case you want to set a custom path to a ansible playbook,
 ## you can do this here, by default the deployment will use the playbook
 ## located in the user config directory.
 ## NOTE: only adjust this if you know what you are doing, if you leave this
 ## blank the system will used the default playbook (standard procedure)
-solr_playbook = ""
+freva_rest_playbook = ""
 
 
 
 [core.config]
 ## List of user(s) that can alter the configuration of the freva cmd line interface
 ## If blank, the user that runs the deployment is chosen
 admins = ""
 
 ## The path where the core should be installed
-install_dir=""
+install_dir="~/freva-env"
 
-## Set the path to any existing conda executable on the target machine,
-## if not existing (default) a tmporary conda distribution will be downloaded
-conda_exec_path=""
-
-## The directory where the project configuration files will be stored, leave
-## blank to use the same directory as `install_dir`
+## The directory where the project configuration files will be stored.
+## This can be useful if you want to set up multiple freva instances with
+## the same software stack. leave blank to use the same directory as
+## `install_dir`
 root_dir = ""
 
 ## If you which not to install a core instance but only configure one set the
 ## install variable to false. This can be useful if you have a central instance
 ## of freva deployed and want to setup a project specific configuration that
 ## uses this central instance
 install = true
 
-## The directory where the user specific output will be stored
+## The directory where the user specific output will be stored,
+## if left blank then it defaults to `root_dir/work`
 base_dir_location = ""
 
 ## Set the directory holding the user content, like plots, for the web user
 ## interface. Note: after plugin application, display content of the plugin
 ## output will be copied to this directory. The default location of this
 ## directory (if left value left blank) is ${base_dir_location}/share/preview
 preview_path = ""
 
 ## Set the workload manager system, currently available are:
 ## "local", "slurm", "pbs", "lfs", "moab", "oar", "sge"
 scheduler_system = "local"
 
-## Set the path to the directory that containes the stdout of the plugings,
-## this directory must be accessible to the web ui. The workload manager
+## Set the path to the directory that contains the stdout of the plugins,
+## this directory must be accessible to the web UI. The workload manager
 ## will write the stdout into this directory. Defaults to ${base_dir_location}/share
 scheduler_output_dir = ""
 
-# Set the target architecutre of the system where the backend will be installed
+# Set the target architecture of the system where the backend will be installed
 # to. You can choose from the following options:
 # Linux-x86_64 (default), Linux-aarch64, Linux-ppc64le, Linux-s390x, MacOSX-x86_64
 arch = "Linux-x86_64"
 
 ## If you need to install the core or its configuration as a different user you can
-## set the ansible_become_user variable, this will install the the core as a
-## different user
-# ansible_become_user = "user_name"
+## set the ansible_become_user variable, this will install the core as a
+## different user. Leave blank for if not needed.
+ansible_become_user = ""
 
-##If you need a different user name you can set it here:
-#ansible_user = "username"
+##If you need a different user name you can set it here (defaults to current user):
+ansible_user = "freva"
 
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
-#ansible_python_interpreter = ""
+ansible_python_interpreter = ""
 
-## The core deployment needs git, if git is not in the default PATH vraiable
+## The core deployment needs git, if git is not in the default PATH variable
 ## you can set the path to the git executable
-#git_path = ""
+git_path = "/usr/bin/git"
+
+## If you want to set special group rights for freva configuration files
+## you can set the admin_group variable. If `admin_group` is set then config
+## files and directories in the `base_dir_location` are only writable to
+## `admin_group`
+admin_grup = ""
 
 ##Indicate whether or not to empty any pre-existing folders/docker volumes.
-##(Useful for a truely fresh start) (default: False)
+##(Useful for a truly fresh start) (default: False)
 wipe = false
 
 ## In case you want to set a custom path to a ansible playbook,
 ## you can do this here, by default the deployment will use the playbook
 ## located in the user config directory.
 ## NOTE: only adjust this if you know what you are doing, if you leave this
 ## blank the system will used the default playbook (standard procedure)
 core_playbook = ""
 
 [web.config]
 ## List of user that can alter the configuration of freva web
 project_website = "www.freva.dkrz.de"
 
 ## Ansible needs a python3 interpreter, which can be set for custom python3 instances
-#ansible_python_interpreter = ""
+ansible_python_interpreter = ""
 
-##If you need a different user name you can set it here:
-#ansible_user = "username"
+##If you need a different user name you can set it here (defaults to current user):
+ansible_user = "freva"
+
+## Set the path where the permanent web data should be stored. By default
+## this is set to /opt/freva
+data_path = "~/freva-local/services"
 
 ##Set html colors
 main_color = "Tomato"
 border_color = "#6c2e1f"
 hover_color = "#d0513a"
 
 ## The about us text is a small blurb about freva within the project
 about_us_text = ""
 
 ## Set the path to the institution logo, this should be the path to the logo
-## as seen by the target system
-institution_logo = "/path/to/logo/on/target/machine"
+## seen by the target system - make sure that this path exists on the target
+## machine
+institution_logo = ""
 
-## Set a an email addresses acting a a contact point for users
+## Set an email addresses acting as contact point for users
 contacts = ""
 
-## Set the smpt email server that will be used to send emails to contacts via the web ui
+## Set the smpt email server that will be used to send emails to contacts via the web UI
 email_host = ""
 
 ## Now set postal address
 imprint = "Project name, German Climate Computing Centre (DKRZ), Bundesstr. 45a, 20146 Hamburg, Germany."
 
 ## Here you can set a lengthy project description.
 ## You can also set a path to a filename that contains the information.
@@ -242,20 +258,20 @@
 ## Set a one line blurb of the project
 homepage_heading = "Short description of the project."
 
 ## Set the name of the project/institution
 institution_name = "Freva"
 
 ## Set the slurm scheduler host
-scheduler_host = ["levante.dkrz.de"]
+scheduler_host = ["localhost"]
 
 ## Settings for ldap
 
 ## Ldap server name(s)
-auth_ldap_server_uri = "ldap://idm-dmz.dkrz.de"
+auth_ldap_server_uri = ""
 
 ## Set the group that will be allowed to log on
 allowed_group = "test_group"
 
 ## Set the ldap search user base
 ldap_user_base = "cn=users,cn=accounts,dc=dkrz,dc=de"
 
@@ -270,15 +286,15 @@
 
 ## Set ldap last name search key
 ldap_last_name_field = "givenname"
 
 ## Set ldap first name search key
 ldap_first_name_field = "sn"
 
-## Set ldap email earch key
+## Set ldap email search key
 ldap_email_name_field = "mail"
 
 ## Set the ldap group class name
 ldap_group_class = "groupOfNames"
 
 ## Set the ldap group type, available values are are [posix, nested]
 ldap_group_type = "nested"
@@ -311,10 +327,15 @@
 ## you can do this here, by default the deployment will use the playbook
 ## located in the user config directory.
 ## NOTE: only adjust this if you know what you are doing, if you leave this
 ## blank the system will used the default playbook (standard procedure)
 web_playbook = ""
 
 ## Set the become (sudo) user name to change to for installing the services
-ansible_become_user = "root"
-
+## leave blank to utilise a non privileged user based installation
+ansible_become_user = ""
 
+# Deploy a http reverse proxy. Turn off the deployment (set to false) of an
+# reverse proxy doesn't the user that deploys the web doesn't have access to
+# port 80 and 443 in this case you will have to deploy the reverse proxy
+# yourself.
+deploy_web_server = false
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/password_rotate.py` & `freva_deployment-2405.0.0/assets/share/freva/deployment/db_service/password_rotate.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import os
 import random
 import shlex
-from subprocess import run
 import string
+from subprocess import run
 
 import requests
 
 SQL_ENTRY = (
     "mysql -h {host} -u root -p'{root_pw}' -e "
     "\"FLUSH PRIVILEGES; ALTER USER {user}@'%' IDENTIFIED BY "
     "'{passwd}'; FLUSH PRIVILEGES\""
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_systemd.py` & `freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/create_systemd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 import argparse
-from pathlib import Path
 import os
 import shlex
-import sys
 import subprocess
+import sys
+from pathlib import Path
 from typing import Dict, List, Tuple
 
 SYSTEMD_TMPL = dict(
     Unit=dict(
         Description="Start/Stop freva services containers",
         After="network-online.target",
     ),
     Service=dict(
         TimeoutStartSec="35s",
         TimeoutStopSec="35s",
-        ExecStartPre="{delete_command}",
+        ExecStartPre='/bin/sh -c "{delete_command}"',
         ExecStart='/bin/sh -c "{container_cmd} {container_args}"',
+        ExecStop='/bin/sh -c "{delete_command}"',
         Restart="no",
     ),
     Install=dict(WantedBy="default.target"),
 )
 
 
 def parse_args() -> Tuple[str, str, List[str], bool]:
@@ -34,15 +35,18 @@
         "--enable",
         action="store_true",
         default=False,
         help="Enable this unit.",
     )
     app.add_argument("--requires", type=str, nargs="+", default=[])
     args, other = app.parse_known_args()
-    return " ".join(other), args.name, args.requires, args.enable
+    enable = args.enable
+    if os.environ.get("DEBUG", "false").lower() == "true":
+        enable = False
+    return " ".join(other), args.name, args.requires, enable
 
 
 def _parse_dict(tmp_dict: Dict[str, Dict[str, str]]) -> str:
     systemd_unit = ""
     for section, keys in tmp_dict.items():
         systemd_unit += "[{}]\n".format(section)
         for key, values in keys.items():
@@ -82,45 +86,55 @@
     env = os.environ.copy()
     env["PATH"] = path
     cmd = ["/tmp/docker-or-podman", "--print-only"] + shlex.split(args)
     res = subprocess.run(
         cmd,
         check=True,
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
         env=env,
     )
     out = res.stdout.decode().split()
     if out:
-        return out[0], " ".join(out[1:]).replace("%", "%%")
+        return out[0], " ".join(out[1:])
     return "", ""
 
 
-def create_unit(
-    args: str, unit: str, requires: List[str], enable: bool
-) -> None:
+def create_unit(args: str, unit: str, requires: List[str], enable: bool) -> None:
     """Create the systemd unit."""
     container_cmd, container_args = get_container_cmd(args)
-    _, delete_command = get_container_cmd("rm -f {}".format(unit))
+    cmd = args.split()
+    if "compose" in cmd and "up" in cmd:
+        new_cmd = []
+        for word in cmd:
+            if word == "up":
+                new_cmd.append("down")
+            elif word not in ("-d", "--detach"):
+                new_cmd.append(word)
+        _, delete_command = get_container_cmd(" ".join(new_cmd))
+    else:
+        _, delete_command = get_container_cmd("rm -f {}".format(unit))
     if delete_command:
         delete_command = "{} {}".format(container_cmd, delete_command)
     else:
         delete_command = ""
     if "docker" in container_cmd:
         SYSTEMD_TMPL["Unit"]["Requires"] = "docker.service"
         SYSTEMD_TMPL["Unit"]["After"] += " docker.service"
+    # else:
+    #    SYSTEMD_TMPL["Service"]["Environment"] = "PODMAN_USERNS=keep-id"
     for key in ("ExecStart",):
         SYSTEMD_TMPL["Service"][key] = SYSTEMD_TMPL["Service"][key].format(
             container_cmd=container_cmd,
             container_args=container_args,
             unit=unit,
         )
-    SYSTEMD_TMPL["Service"]["ExecStartPre"] = SYSTEMD_TMPL["Service"][
-        "ExecStartPre"
-    ].format(delete_command=delete_command)
+    for key in ("ExecStartPre", "ExecStop"):
+        SYSTEMD_TMPL["Service"][key] = SYSTEMD_TMPL["Service"][key].format(
+            delete_command=delete_command
+        )
     for service in requires:
         for key in ("After", "Requires"):
             try:
                 SYSTEMD_TMPL["Unit"][key] += " {}.service".format(service)
             except KeyError:
                 SYSTEMD_TMPL["Unit"][key] = " {}.service".format(service)
     load_unit(unit, _parse_dict(SYSTEMD_TMPL), enable)
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/docker-or-podman` & `freva_deployment-2405.0.0/assets/share/freva/deployment/scripts/docker-or-podman`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 #!/usr/bin/env python3
-"""A script that wraps docker/podman/apptainer commands."""
+"""A script that wraps docker/podman commands."""
 
 
 import abc
 import argparse
+import shlex
 import shutil
 import subprocess
 import sys
 from datetime import datetime
+from getpass import getuser
 from pathlib import Path
-from typing import (
-    Any,
-    ClassVar,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
+from typing import ClassVar, Dict, List, Optional, Tuple, Union, cast
 
 FlagType = Union[str, List[str], bool, None]
 """Type for additional command line arguments."""
 
 
 class CommandFactory(metaclass=abc.ABCMeta):
     """A simple command wrapper for running container commands.
@@ -41,19 +34,58 @@
     def __init__(self, images: List[str], print_only=False):
         self._images = images
         self._print_only = print_only
 
     @staticmethod
     def get_container_cmd() -> str:
         """Get the command of the container."""
-        for cmd in ("apptainer", "podman", "docker"):
+        engines = ["docker", "podman"]
+        if getuser() != "root":
+            engines = engines[::-1]
+        for cmd in engines:
             cont_cmd = shutil.which(cmd)
             if cont_cmd:
                 return cont_cmd
-        raise ValueError("Docker, Podman or Apptainer must be installed")
+        raise ValueError("Docker or Podman must be installed")
+
+    def compose(self, *args, **kwargs) -> List[str]:
+        """User the compose command.
+
+        Parameters
+        ----------
+        **kwargs: Any
+            Additional command line arguments
+        Returns
+        -------
+        list[str]: Constructed command line arguemnts.
+        """
+        container_cmd = Path(self.get_container_cmd()).name
+        command = shutil.which(f"{container_cmd}-compose")
+        if not command:
+            install_cmd = f"python3 -m pip install {container_cmd}-compose"
+            try:
+                subprocess.run(
+                    shlex.split(install_cmd),
+                    check=True,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                )
+            except subprocess.CalledProcessError:
+                txt = (
+                    f"{container_cmd} is available but not {container_cmd}-compose"
+                    " which should be installed on the system."
+                )
+                print(txt, file=sys.stderr)
+                raise ValueError(txt)
+            command = (
+                shutil.which(f"{container_cmd}-compose")
+                or f"{container_cmd}-compose"
+            )
+        _args = self._kwargs_to_list(**kwargs)
+        return [command] + _args + list(args)
 
     def network(self, sub_command: str, *flags: str) -> List[str]:
         """Interact with the network sub commands.
 
         Parameters
         ----------
         sub_commnds: str
@@ -102,14 +134,40 @@
         -------
         list[str]: Constructed commmand line arguments.
         """
 
         cli_command = [self.get_container_cmd(), "pull"]
         return cli_command + self._kwargs_to_list(**kwargs) + self.images
 
+    def stop(self, time_out: Optional[int] = None) -> List[str]:
+        """Stop running containers."""
+
+        cli_command = [self.get_container_cmd(), "stop"]
+        if time_out is not None:
+            cli_command += ["-t", str(time_out)]
+        return cli_command + self.images
+
+    def inspect(self, **kwargs: FlagType) -> List[str]:
+        """Inspect images/containers.
+
+        Parameters
+        ----------
+        **kwargs:
+            Additional command line arguments
+
+        Returns
+        -------
+        list[str]: Constructed commmand line arguments.
+        """
+        return (
+            [self.get_container_cmd(), "inspect"]
+            + self._kwargs_to_list(**kwargs)
+            + self.images
+        )
+
     def rm(self, sub_command: str, **kwargs: FlagType) -> List[str]:
         """Remove images/containers.
 
         Parameters
         ----------
         sub_command: str
             The sub command used for deleting containers/images.
@@ -173,97 +231,14 @@
 
 class Podman(CommandFactory):
     """Wrapping the podman commands."""
 
     command = "podman"
 
 
-class Apptainer(CommandFactory):
-    """Wrapping the apptainer commands."""
-
-    command = "apptainer"
-
-    @property
-    def images(self) -> List[str]:
-        """Get the location of the image."""
-        return ["docker://{}".format(image) for image in self._images]
-
-    def network(self, sub_command: str, *flags: str) -> List[str]:
-        """The network sub command doesn't seem to work in apptainer."""
-        return []
-
-    def pull(self, **kwargs: FlagType) -> List[str]:
-        """Pull a container.
-
-        Parameters
-        ----------
-        **kwargs: Any
-            Additional command line arguments
-
-        Returns
-        -------
-        list[str]: Constructed commmand line arguments.
-        """
-        cli_command = [self.get_container_cmd(), "pull", "-F"]
-        return cli_command + self.images
-
-    def rm(self, sub_command: str, **kwargs: Any) -> List[str]:
-        """Remove images/containers.
-
-        Parameters
-        ----------
-        sub_command: str
-            The sub command used for deleting containers/images.
-        **kwargs:
-            Additional command line arguments
-
-        Returns
-        -------
-        list[str]: Constructed commmand line arguments.
-        """
-
-        if sub_command == "rmi":
-            new_command = ["delete"]
-        else:
-            # this is not ideal since 'oci' is for root only.
-            return []
-            # new_command = ["oci", "delete"]
-        cli_command = [self.get_container_cmd()] + new_command
-        return cli_command + self.images
-
-    def _translate(self, options: Dict[str, FlagType]) -> Dict[str, FlagType]:
-        """Translate the docker commands to an apptainer command."""
-        output: Dict[str, FlagType] = {
-            "env": options.get("env") or [],
-            "mount": [],
-            "dns": None,
-            "network-args": [],
-        }
-        for volume in cast(List[str], options.get("volume", [])) or []:
-            mounts = volume.split(":", 2)
-            cast(List[str], output["mount"]).append(
-                "type=bind,source={},destination={}".format(
-                    mounts[0], mounts[1]
-                )
-            )
-        for port in cast(List[str], options.get("publish", [])) or []:
-            in_port, _, out_port = port.partition(":")
-            cast(List[str], output["network-args"]).append(
-                "portmap={}:{}/tcp".format(in_port, out_port)
-            )
-        output = {k: v for (k, v) in output.items() if v}
-        if "net" in options:
-            output["network"] = "bridge"
-            output["fakeroot"] = True
-        if "network" in options or "network-args" in options:
-            output["net"] = True
-            output["fakeroot"] = True
-        return output
-
-
 def add_standard_args() -> argparse.ArgumentParser:
     """Add common arguments to a parser."""
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument(
         "container",
         nargs=1,
         type=str,
@@ -365,14 +340,38 @@
     parser_pull.add_argument(
         "-q",
         "--quiet",
         help="Suppress verbose output",
         action="store_true",
     )
 
+    # -------------------------- Compose commands -----------------------------
+    parser_compose = subparsers.add_parser(
+        "compose",
+        help="Define and run multi-container applications",
+    )
+    parser_compose.add_argument("-p", "--project-name", help="Project name")
+    parser_compose.add_argument(
+        "-f",
+        "--file",
+        help="Compose configuration files",
+    )
+    parser_compose.add_argument(
+        "--project-directory",
+        help=(
+            "Specify an alternate working directory "
+            "(default: the path of the, first specified, Compose file)"
+        ),
+    )
+    parser_compose.add_argument(
+        "command",
+        nargs=argparse.REMAINDER,
+        type=str,
+        metavar="command",
+    )
     # -------------------------- Exec commands --------------------------------
 
     _ = subparsers.add_parser(
         "exec",
         help="Execute a command in a running container",
         parents=[parent],
     )
@@ -398,14 +397,17 @@
     )
     parser_run.add_argument("--hostname", help="Container host name")
     parser_run.add_argument("--name", help="Assign a name to the container")
     parser_run.add_argument(
         "--network", help="Connect a container to a network"
     )
     parser_run.add_argument(
+        "--network-alias", help="Add network-scoped alias for the container"
+    )
+    parser_run.add_argument(
         "-v", "--volume", help="Bind mount a volume", action="append"
     )
     parser_run.add_argument(
         "-p",
         "--publish",
         help="Publish a container's port(s) to the host",
         action="append",
@@ -434,14 +436,33 @@
     parser_run.add_argument(
         "--cap-add",
         type=str,
         help="Linux capabilities",
         action="append",
     )
 
+    # -------------------------- stop commands --------------------------------
+
+    parser_stop = subparsers.add_parser(
+        "stop", help="Stop one or more running containers"
+    )
+    parser_stop.add_argument(
+        "container",
+        nargs="+",
+        type=str,
+        metavar="CONTAINER",
+        help="Name of the container(s)",
+    )
+    parser_stop.add_argument(
+        "-t",
+        "--time-out",
+        type=int,
+        help="Timout",
+    )
+
     # -------------------------- rm commands ----------------------------------
 
     parser_rm = subparsers.add_parser(
         "rm", help="Remove one or more containers"
     )
     parser_rm.add_argument(
         "container",
@@ -499,41 +520,72 @@
     parser_network.add_argument(
         "flags",
         nargs=argparse.REMAINDER,
         type=str,
         metavar="flags",
     )
 
+    # -------------------------- inspect commands -----------------------------
+
+    parser_inspect = subparsers.add_parser(
+        "inspect",
+        help="Return low-level information on Docker objects",
+        add_help=False,
+    )
+    parser_inspect.add_argument(
+        "container",
+        nargs="+",
+        type=str,
+        metavar="CONTAINER",
+        help="Name of the images(s)",
+    )
+    parser_inspect.add_argument(
+        "--format",
+        "-f",
+        type=str,
+    )
+    parser_inspect.add_argument(
+        "--size",
+        "-s",
+        action="store_true",
+    )
+    parser_inspect.add_argument("--type", type=str)
+
     # -------------------------------------------------------------------------
 
     args = parser.parse_args()
     container_cmd = Path(Docker.get_container_cmd()).name
     container_cls = {
         "podman": Podman,
-        "apptainer": Apptainer,
         "docker": Docker,
     }
     container_inst = container_cls[container_cmd](
-        args.container, print_only=args.print_only
+        getattr(args, "container", None), print_only=args.print_only
     )
     kwargs = {
         k.replace("_", "-"): v
         for (k, v) in args._get_kwargs()
         if k not in ("subcommand", "container", "command", "print_only")
     }
     if args.subcommand in ("run", "exec"):
         cmd = container_inst.run(args.subcommand, *args.command, **kwargs)
     elif args.subcommand in ("rm", "rmi"):
         cmd = container_inst.rm(args.subcommand, **kwargs)
+    elif args.subcommand in ("inspect",):
+        cmd = container_inst.inspect(**kwargs)
+    elif args.subcommand in ("stop",):
+        cmd = container_inst.stop(args.time_out)
     elif args.subcommand in ("pull",):
         cmd = container_inst.pull(**kwargs)
     elif args.subcommand in ("network",):
         cmd = container_inst.network(
             args.subcommand, args.command, *args.flags
         )
+    elif args.subcommand in ("compose",):
+        cmd = container_inst.compose(*args.command, **kwargs)
     else:
         cmd = []
     if args.print_only:
         print(" ".join(cmd))
         return []
     return cmd
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/Dockerfile` & `freva_deployment-2405.0.0/assets/share/freva/deployment/vault/Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 FROM docker.io/hashicorp/vault:latest
-
-LABEL maintainer="DRKZ-CLINT"
-LABEL repository="https://github.com/FREVA-CLINT/freva.git"
+ARG VERSION
+LABEL org.opencontainers.image.authors="DRKZ-CLINT"
+LABEL org.opencontainers.image.source="https://github.com/FREVA-CLINT/freva-deployment.git"
+LABEL org.opencontainers.image.version="$VERSION"
 
 ENV VAULT_ADDR='http://127.0.0.1:8200'
-COPY runserver.py /bin/runserver
-COPY --chown=vault:vault vault-server-tls.hcl /vault
-COPY --chown=vault:vault policy-file.hcl /vault
+ENV VERSION=$VERSION
+ENV HOME=/vault
+COPY runserver.py /bin/runserver.py
+COPY add-vault-secret /bin/add-vault-secret
 RUN set -ex &&\
-    chmod +x /bin/runserver &&\
+    mkdir -p /opt/vault && chown -R vault:vault /opt/vault &&\
+    chmod +x /bin/runserver.py /bin/add-vault-secret &&\
     mkdir -p /data && chown -R vault:vault /data &&\
-    apk add --update --no-cache python3 mysql mysql-client &&\
+    apk add --update --no-cache python3 &&\
     ln -sf python3 /usr/bin/python
+COPY --chown=vault:vault vault-server-tls.hcl /opt/vault/
+COPY --chown=vault:vault policy-file.hcl /opt/vault/
 
 RUN python3 -m ensurepip
 RUN pip3 install --no-cache --upgrade pip setuptools &&\
-    pip3 install requests flask flask_restful
+    pip3 install hvac requests pyopenssl fastapi uvicorn
 
 EXPOSE 5002
-VOLUME /vault/file
-CMD ["/bin/runserver"]
+VOLUME /vault
+CMD python3 /bin/runserver.py &&\
+    uvicorn --workers 2 --app-dir /bin runserver:app \
+    --host 0.0.0.0 --port 5002
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/deploy_vault.py` & `freva_deployment-2405.0.0/assets/share/freva/deployment/vault/deploy_vault.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 
-from subprocess import run, PIPE
-import shlex
 import os
+import shlex
+from subprocess import PIPE, run
 
 if __name__ == "__main__":
 
     cmd = shlex.split("vault operator init")
     env = os.environ.copy()
     env["VAULT_ADDR"] = "https://127.0.0.1:8200"
     env["VAULT_SKIP_VERIFY"] = "true"
```

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/web/Dockerfile` & `freva_deployment-2405.0.0/assets/share/freva/deployment/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/assets/share/freva/deployment/web/freva_web.conf` & `freva_deployment-2405.0.0/assets/share/freva/deployment/web/freva_web.conf`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ServerRoot "/usr/local/apache2"
-Listen 80
+Listen ${HTTPD_PORT}
 
 #
 # Dynamic Shared Object (DSO) Support
 #
 # To be able to use the functionality of a module which was built as a DSO you
 # have to place corresponding `LoadModule' lines at this location so the
 # directives contained in it are actually available _before_ they are used.
@@ -172,25 +172,27 @@
 Timeout 60
 KeepAliveTimeout 5
 
 RewriteEngine On
 RewriteCond %{HTTPS} off
 RewriteRule ^ https://%{HTTP_HOST}%{REQUEST_URI}
 
-Listen 443
+Listen ${HTTPDS_PORT}
 
 #SSLPassPhraseDialog exec:/usr/libexec/httpd-ssl-pass-dialog
 SSLSessionCache         shmcb:/run/httpd/sslcache(512000)
 SSLSessionCacheTimeout  300
 SSLRandomSeed startup file:/dev/urandom  256
 SSLRandomSeed connect builtin
 SSLCryptoDevice builtin
 
-<VirtualHost *:443>
+<VirtualHost *:${HTTPDS_PORT}>
     ProxyPass /static/ !
+    ProxyPass /api/databrowser http://${DATABROWSER_HOST}/api/databrowser
+    ProxyPassReverse /api/databrowser http://${DATABROWSER_HOST}/api/databrowser
     ProxyPass / http://${FREVA_HOST}:8000/
     ProxyPassReverse / http://${FREVA_HOST}:8000/
     RequestHeader set X-Forwarded-Proto 'https' env=HTTPS
     SSLEngine on
     Alias /static /srv/static/
     Alias /robots.txt /srv/static/robots.txt
     Alias /favicon.ico /srv/static/favicon.ico
@@ -201,15 +203,14 @@
     Header set X-Frame-Options "SAMEORIGIN"
 
     SSLCipherSuite ECDHE-RSA-AES256-GCM-SHA384:DHE-RSA-AES256-GCM-SHA384:ECDHE-RSA-AES128-GCM-SHA256:DHE-RSA-AES128-GCM-SHA256
     SSLHonorCipherOrder on
 
     SSLCertificateFile /etc/ssl/certs/server-cert.crt
     SSLCertificateKeyFile /etc/ssl/private/server-key.key
-    SSLCertificateChainFile /etc/ssl/certs/cacert.pem
     SetOutputFilter DEFLATE
     SetEnvIfNoCase Request_URI "\.(?:gif|jpe?g|png)$" no-gzip
     Header always set Strict-Transport-Security "max-age=15552000; includeSubdomains;"
     <Directory /srv/*>
         Options Indexes MultiViews
         AllowOverride None
         Require all granted
```

### Comparing `freva_deployment-2309.0.1/docs/Architecture.md` & `freva_deployment-2405.0.0/docs/architecture/Architecture.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Deployment Architecture
+# Freva Architecture
 
 
 The Free evaluation system framework (Freva) consists of three basic parts:
 
 
 - core library (`evaluation_system`) that handles request to the data search engine and database as well as configuring and submitting data analysis plugins
 - command line interface and a python client as user interface to the core library.
 - services, such as a apache solr data search service, mariadb database and web service providing a web-based user interface (web ui) to the core library
 
 Command line interface, python client and web ui make use of the core library, the core library on the other hand makes use of the apache solr and mariadb services. This hierachy is outlined in the figure below:
 
-![](Concept_Map.png)
+![](_static/Concept_Map.png)
 
 ### Core library and command line interface:
 
 The core library (`evaluation_system`) and the command line interface (cli) are
 installed within the anaconda environments. Anaconda has the advantage
 that it comes with its own python distribution and hence any python instance
 can be made independent of the host system. The disadvantage is that it
@@ -66,41 +66,41 @@
 client requests to the django web application.
 
 ## Setups
 The next sections propose various deployment strategies for the framework:
 
 ### One service one machine set up:
 
-![](Topography_1.png)
+![](_static/Topography_1.png)
 
 *One service one machine*: Every service is installed on a dedicated machine
 
 
 This setup deploys the cli on a central instance and the services on dedicated machines (VM or bare metal).
 We recommend this setup since it minimises the load on each host machine and minimises failure due to load issues.
 In a typical scenario the core configuration stored in a central location is made accessible to the machine hosting the web ui container.
 The cli also connects and communicates to machines hosting the apache solr and mariadb containers.
 The vault server will always be running on the same machine that hosts the mariadb service.
 
 
 
 ### All services on one machine set up:
-![](Topography_2.png)
+![](_static/Topography_2.png)
 
 *All services on one machine*: All services are installed on the same machine
 
 This setup deploys the cli on a central instance and all services on one single machine
 (VM or bare metal). While this set up might be prone to load failure unless
 enough resources a allocated to the machine, it is probably most simple
 to administer since all services are running on one entry point.
 
 
 ### Multi-cli setup:
 
-![](Topography_3.png)
+![](_static/Topography_3.png)
 
 *Multi-cli*: The command line interface and core library are installed on many compute nodes
 
 
 Distributed file systems, such as gpfs or lustre, can be slow - therefore
 it is recommend to NOT deploy the anaconda environments for cli and core library on such file systems.
 The above above mentioned anaconda setup creates a considerable amount of small
```

### Comparing `freva_deployment-2309.0.1/docs/Concept_Map.png` & `freva_deployment-2405.0.0/docs/Concept_Map.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Configure.md` & `freva_deployment-2405.0.0/docs/after-deployment/TransitionPlugins.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,149 +1,223 @@
-# Running and configuring the deployment
-A complete Freva instance will need the following services:
+# Transitioning of the Plugins
 
-- solr servers (hostname of the apache solr server)
-- db servers (hostname of the MariaDB server)
-- web servers (hostname that will serve web ui)
-- core servers (hostname(s) where the command line interface will be installed)
+The Freva plugins are an essential part of Freva.
+Most likely the transitioning from the old python2 to the new python3 based
+system, needs special care. A complete rewrite of the plugin manager is planned.
+This section should therefore be seen as intermediate solutions for plugin transitioning.
 
-## Setting the python and git path
-Some systems do not have access to python3.4+ (/usr/bin/python3) or git by default.
-In such cases you can overwrite the `ansible_python_interpreter` in the inventory
-settings of the server section to point ansible to a custom `python3` bindary. For example
+Currently we recommend creating an anaconda environment for each plugin.
+This approach has several advantages:
 
-```
-ansible_python_interpreter=/sw/spack-rhel6/miniforge3-4.9.2-3-Linux-x86_64-pwdbqi/bin/python3
-```
-
-The same applies to the path to the git binary:
+- reproducible as each plugin will get a anaconda environment file.
+- no version and dependency conflicts occur.
+- once set up easy to maintain.
 
-```
-git_path=/sw/spack-levante/git-2.31.1-25ve7r/bin/git
-```
-## A map of your server infrastructure (optional)
-Different Freva instances are installed across different server hosts. Usually
-the different Freva instances running at an institution are distinguished by
-a unique project name for example `clex`.
-To keep track of all server and services we have created a service that keeps
-track of the locations of all services for certain Freva instances.
-*Before* the first deployment we recommend to setup this server map by issuing
-the `deploy-freva-map` command. Please also refer to the [installation section](Installation.html#setting-up-a-service-that-maps-the-server-structure)
-for more details. This step is only necessary *once* per institution, please talk
-to the admins of any other Freva instances at your institution if this service
-has already been set up.
+These are the disadvantages of this method:
 
+- an anaconda environment file has to be created for each plugin.
 
-## Running the deployment
-After successful configuration you can run the deployment.
-The command `deploy-freva` opens a text user interface (tui) that will walk
-you through the setup of the deployment.
-> **_Note:_** Navigation is similar to the one of the *nano* text editor.
-The shortcuts start with a `^` which indicates `CTRL+`.
 
-Please refer to the [Appendix I](TuiHowto.html) on tui usage instructions.
+## Transitioning steps:
 
-### Deployment with existing configuration.
-If you already have a configuration saved in a toml inventory file you can
-issue the `deploy-freva-cmd` command:
+There are multiple ways of how you can get your old plugin back to the new
+Freva system. We do recommend a deployment strategy involving conda.
+While this strategy is not strictly necessary it offers the best as
+possible reproducibility and is host system independent.
+Meaning your plugins can be easily transitioned to other institutions and
+are more likely to work after major system updates on your host system.
+Here we briefly cover the steps that are needed to bring your old plugin back
+to life in the new Freva system. We will also discuss alternatives
+to using conda. Regardless of choice on using conda or not the first two
+steps will be necessary.
 
-```console
-deploy-freva-cmd --help
-usage: deploy-freva-cmd [-h] [--server-map SERVER_MAP] [--config CONFIG] [--steps {web,core,db,solr} [{web,core,db,solr} ...]]
-                        [--ask-pass] [-v] [-V]
-
-Deploy Freva and its services on different machines.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --server-map SERVER_MAP
-                        Hostname of the service mapping the Freva server architecture, Note: you can create a server map by running
-                        the deploy-freva-map command (default: None)
-  --config CONFIG, -c CONFIG
-                        Path to ansible inventory file. (default: /home/wilfred/.config/freva/deployment/inventory.toml)
-  --steps {web,core,db,solr} [{web,core,db,solr} ...]
-                        The services/code stack to be deployed (default: ['db', 'solr', 'web', 'core'])
-  --ask-pass            Connect to server via ssh passwd instead of public key. (default: False)
-  -v, --verbose         Verbosity level (default: 0)
-  -V, --version         show program's version number and exit
-```
-
-The `--steps` flags can be used if not all services should be deployed.
-
-## Using environment variables
-Once the deployment configuration is set up it might be useful to store the
-config and all the files that are needed to run the deployment at a central,
-yet *secure* location. This can be useful if multiple admins will have to take
-turns in (re)-deploying the system and thus the configuration has to be up to
-date for those admins. The problem that arises is that the setup might differ
-slightly for each person and computer running the deployment. For instance the
-`ansible_user` key might differ. For this purpose the deployment supports setting
-environment variables. Those environment variables can be used in the configuration
-file. Like `ansible_user = $USER`. You can then set up the `USER` variable with
-help of the deployment tui. To do so open the main menu (`CTRL+x`) and then
-choose the add set variables options (`CTRL+v`). You can then add or edit
-variables. In the figure below the `USER` variable is set to a specific user
-name. If the deployment encounters an entry using `$USER` variable it will be
-replaced by the according value that points to the `$USER` variable.
-
-![Add Variable](Variable.png)
-
-### Relative paths using the $CFD variable
-Instead of setting the absolute paths in the configuration files
-for example the path to the public certificate files, you should give the
-paths *relative* to the configuration file. To indicate that the
-freva-deployment machinery should create paths relative to the configuration
-you should set all paths starting with the `$CFD` (current file directory)
-variable. For example if the configuration file is located in
-`/home/user/config/foo/foo.toml` and the public cert file is located in the
-same directory as the configuration file then you can set the path to the cert
-file in the configuration files via `$CFD/foo.crt`.
-
-This will assure that paths will work from any other machine.
-
-## Advanced: Adjusting the playbook
-Playbook templates and be found the in the `~/.config/freva/deployment/playbooks` directory.
-You can customise those playbooks if the standard installation procedure is
-not well suited. Each deployment section offers the option to set paths
-to custom playbook files instead of the standard playbook files. To change
-the behaviour of the installation for a certain freva instance, simply adjust
-the path to the playbook for that step in the inventory file or tui. For example:
+### Common steps:
 
-- `web_playbook = '/home/myuser/playbooks/my-web.yml'`
+1. clone the repository of a plugin, change into the directory and create a new branch.
 
+2. export the user plugin variable:
+```console
+export EVALUATION_SYSTEM_PLUGINS=$PWD/path_to_wrapper_file,class_name
+freva plugin -l
+```
+Most certainly, the plugin manager will output a warning that the plugin could
+not be loaded. If it does, change the plugin accordingly to make the
+warning messages go away.
+
+### a. Using conda:
+As mentioned above this step has the advantage that you increase the reproducibility
+of your plugin. Transitioning your plugin to other institutions is also easy
+because all libraries are encapsulated from the host system and hence independent.
+While not strictly necessary it is a good idea to familiarise yourself with
+[anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/index.html).
+
+3. Download the [conda environment file template](https://swift.dkrz.de/v1/dkrz_3d3c7abc-1681-4012-b656-3cc1058c52a9/k204230/freva-transition/plugin-env.yml) and the [Makefile template](https://swift.dkrz.de/v1/dkrz_3d3c7abc-1681-4012-b656-3cc1058c52a9/k204230/freva-transition/Makefile)
+
+4. Add all dependencies to the `plugin-env.yml` file. In doubt search [anaconda.org](https://anaconda.org) for dependencies.
+
+5. If needed adjust the `build` step in the `Makefile` for compiling plugin dependencies, e.g. fortran dependencies.
+
+6. Execute `make all` to install the conda environment and build the plugin dependencies.
+
+7. Execute the plugin and check if everything goes well.
+
+8. Format the plugin using black: `black -t py310 path_to_plugin.py`
+
+### b. Using the environment of freva
+If your plugin doesn't need many libraries you can simply try to use everything
+the comes with freva. This is the easiest way as you don't have to do anything.
+Simply try to execute all commands that come with your plugin and see what
+happens.
+
+### c. Using software of the host system
+You can also make use of the software installed on the host system. For
+example via spack. Many HPC systems offer the `module` command. Using this
+approach will result in a plugin that is tailored around the current host system
+you are using. Future updates may break usage and you defiantly won't be able
+to use your plugin at other institutions.
+
+## Transitioning `python2` plugins
+Python plugins (especially python2) need special care. The recommended strategy
+is to convert the plugin content to python3. If this is not possible an anaconda
+python2 environment should be created.
+
+If in the original plugin the plugin code is directly executed in the `run_rool`
+method (formerly named `runTool`) this code has to be split from the new `run_tool` method. The
+transition strategy is gathering the essential information in a `json` file that
+is passed to the actual core part of the plugin. The code below shows a simple
+python2 plugin:
 
-## Known Issues:
-Below are possible solutions to some known issues:
+```python
 
-#### SSH connection fails:
+def runTool(self, config_dict={}):
+    """This is the old `runTool` method.
+    The plugin configuration is passed into this method and the code
+    is directly executed in this method."""
+
+    from src.plugin import calculate
+    from evaluation_system.model.file import DRSFile
+    search_kw = dict()
+    search_kw["variable"] = config_dict["variable"]
+    search_kw["model"] = config_dict["model"]
+    search_kw["experiment"] = config_dict["experiment"]
+    search_kw["ensemble"] = config_dict["ensemble"]
+    search_kw["project"] = config_dict["project"]
+    search_kw["product"] = config_dict["product"]
+    search_kw["time_frequency"] = config["time_frequency"]
+    files = files = sorted(DRSFile.solr_search(path_only=True, **search_kw))
+    calculate(search_kw["variable"], files, config_dict["output_dir"])
+    return self.prepareOutput(config_dict["output_dir"])
+```
+
+The above code should be split into two components, one that makes use of
+`evaluation_system` to gather the data. And one that executes the actual plugin
+code.
 
 ```python
-fatal: [host.name]: FAILED! => {"msg": "Using a SSH password instead of a key is not possible because Host Key checking is enabled and sshpass does not support this.  Please add this host's fingerprint to your known_hosts file to manage this host."}
+
+def run_tool(self, config_dict={}):
+    """This is the wrapper API part of the plugin.
+    It gathers the plugin information and passes the needed information
+    to the actual plugin code that is split into another python file."""
+
+    import json
+    from evaluation_system.model.file import DRSFile
+    from tempfile import NamedTemporaryFile
+    from pathlib import Path
+    search_kw = dict()
+    search_kw["variable"] = config_dict["variable"]
+    search_kw["model"] = config_dict["model"]
+    search_kw["experiment"] = config_dict["experiment"]
+    search_kw["ensemble"] = config_dict["ensemble"]
+    search_kw["project"] = config_dict["project"]
+    search_kw["product"] = config_dict["product"]
+    search_kw["time_frequency"] = config["time_frequency"]
+    files = sorted(DRSFile.solr_search(path_only=True, **search_kw))
+    compute_kw = dict(variable=search_kw["variable"],
+                      files=files,
+                      output_dir=config_dict["output_dir"]
+                )
+    with NamedTemporaryFile(suffix=".json") as tf:
+        with open(tf.name, "w"):
+            json.dump(**compute_kw, f, indent=3)
+        self.call(f"python2 {Path(__file__).parent / 'compute_python2'} {tf.name}")
+    return self.prepare_output(config_dict["output_dir"])
 ```
-- This means that you've never logged on to the server. You can avoid this error message by simply logging on to the server for the first time.
 
-#### Playbook complains about refused connections for the solr or db playbook
+The below code demonstrates the usage of the above created `json` file.
 
-```python
-fatal: [localhost]: FAILED! => {"changed": true, "cmd": "docker run --name \"test_ces_db\" -e MYSQL_ROOT_PASSWORD=\"T3st\" -p \"3306\":3306 -d docker.io/library/mariadb", "delta": "0:00:00.229695", "end": "2021-05-27 16:10:58.553280", "msg": "non-zero return code", "rc": 125, "start": "2021-05-27 16:10:58.323585", "stderr": "docker: Error response from daemon: driver failed programming external connectivity on endpoint test_ces_db (d106bf1fe310a2ae0e012685df5a897874c61870c5241f7a2af2c4ce461794c2): Error starting userland proxy: listen tcp4 0.0.0.0:3306: bind: address already in use.", "stderr_lines": ["docker: Error response from daemon: driver failed programming external connectivity on endpoint test_ces_db (d106bf1fe310a2ae0e012685df5a897874c61870c5241f7a2af2c4ce461794c2): Error starting userland proxy: listen tcp4 0.0.0.0:3306: bind: address already in use."], "stdout": "895ba35cdf5dcf2d4ec86997aedf0637bf4020f2e9d3e5775221966dcfb820a5", "stdout_lines": ["895ba35cdf5dcf2d4ec86997aedf0637bf4020f2e9d3e5775221966dcfb820a5"]}
-```
-- This means that there is already a service running on this port - in this case a local mariadb service. To avoid this error chose a different port in your `config/inventory` file.
 
-#### Playbook cannot create database tables because connections fails
+```python
+"""This file is the python2 plugin part.
+This file calls the calculations of the python2 plugin. The configuration
+is passed via a json file into this part.
+"""
+
+if __name__ == "__main__":
+    from src.plugin import calculate
+    import sys
+    import json
+    try:
+        with open(sys.argv[1]) as f:
+            config = json.load(f)
+    except IndexError:
+        raise ValueError("Usage: {} path_to_json_file.json".format(sys.argv[0]))
+    calculate(config["variable"], config["files"], config["output_dir"])
+```
+
+If you want to use the json file in a bash script you must install the `jq`
+json parser. Simply add `jq` to your `plugin-env.yml` file and read the
+[docs of jq](https://stedolan.github.io/jq/tutorial/).
+
+## After conda deployment: Increasing reproducibility of your plugin
+If you have successfully deployed your plugin environment using conda you
+can increase the reproducibility by "freezing" all packages that have
+been installed by conda. This will increase the reproducibility of your package
+because the versions of your packages will exactly match the one you are
+using at this point in time. Every time you re-install the plugin environment
+you will have the same dependency versions. To fix the package versions
+execute the following command:
+```
+./plugin_env/bin/conda list  --explicit > spec-file.txt
+```
+Add and commit the created `spec-file.txt` to your repository. Afterwards
+you can replace
+`conda env create --prefix ./plugin_env -f plugin-env.yml --force` in the `conda`
+section of your `Makefile` by:
+
+```
+conda env create --prefix ./plugin_env -f spec-file.txt --force
+```
+And you're done.
+
+## Problem: conda doesn't finish resolving dependencies
+Sometimes conda is unable/won't finish to solve all dependencies. You have a
+couple of options in that case. First you can try replacing the `conda` command
+by `mamba` in your Makefile. `mamba` is written in C and comes with a
+different dependency solver. Most of the time switching from `conda` to `mamba`
+solves the problem. If the issues persists with `mamba` you can try identifying
+the problematic package(s). Usually by guessing which package(s) might be the
+offending ones and removing them from the `plugin-env.yml` file. Once the
+package(s) have been circled you can create an additional conda environment.
+For example by adding the following line into the `conda` section of the
+`Makefile`. For example:
+
+```
+conda create -c conda-forge -p ./plugin_env2 cdo netcdf-fortran
+``
+
+If you want to use resources from this environment in your plugin you need
+to modify the environment in your API wrapper. Following the example
+above, this modification could look like this:
 
 ```python
-fatal: [localhost]: FAILED! => {"changed": false, "msg": "ERROR 1698 (28000): Access denied for user 'root'@'localhost'\n"}
-```
-- This is a common problem if you've set the mariadb docker host to be localhost. You can avoid the problem by setting the `db_host` variable to a non localhost type IP like 172.17.0.1. If you're not sure what IP to use try the following command
-```
-docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' db_docker_name
-```
-you can figure out the `db_docker_name` using the following command:
-```
-docker container ls
-```
+env = os.environ.copy()
+this_dir = os.path.dirname(os.path.abspath(__file__))
+env["PATH"] = env["PATH"] + ":" + os.path.join(this_dir, "plugin_env2", "bin")
+env["LD_LIBRARY_PATH"] = os.path.join(this_dir, "plugin_env2", "lib")
+self.call(your_command_here, env=env)
 
-### Stuck in load/save dialogue in the tui
-The load/save forms can be exited by pressing the `<TAB>` key
-which will get you to input field at the bottom of the screen. If the input
-field has text delete it an press the `<ESC>` key, this will bring you get to
-the screen where you started.
+```
+If you need to compile additional libraries you probably also want to adjust
+the `PATH` and `LD_LIBRARY_PATH` variable in the file that executes the compile
+step to be able to pick up the `lib` and `bin` folders in the `plugin_env2`
+conda environment.
```

### Comparing `freva_deployment-2309.0.1/docs/Folders.md` & `freva_deployment-2405.0.0/docs/architecture/Folders.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Primer: Basic Freva configuration
+# Basic Freva configuration
 
 Because the framework consists of multiple parts, Freva has to be configured
 to work with those different parts. This is especially true for the web ui
 and the `evaluation_system` core running on an HPC system. The central
 building block of the freva configuration is the `evaluation_system.conf`
 configuration file. This file holds information on the server infrastructure,
 that is host names for apache solr and mariadb servers, project specific
@@ -10,15 +10,15 @@
 
 This part of the documentation will emphasis on the directory structure, which
 is important for the interplay of the `evaluation_system` core and the web ui.
 
 The content of the initial `evaluation_system.conf` file looks like the
 following:
 
-```
+```ini
 [evaluation_system]
 # Freva - Free Evaluation System Framework configuration file
 # This file contains the necessary configuration information
 # which is needed to run Freva
 #
 # Username(s) - comma separated - of the admins of the project
 admins=
```

### Comparing `freva_deployment-2309.0.1/docs/LegalNotes.md` & `freva_deployment-2405.0.0/docs/after-deployment/LegalNotes.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Makefile` & `freva_deployment-2405.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Topography.png` & `freva_deployment-2405.0.0/docs/architecture/_static/Topography.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Topography_1.png` & `freva_deployment-2405.0.0/docs/architecture/_static/Topography_1.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Topography_2.png` & `freva_deployment-2405.0.0/docs/architecture/_static/Topography_2.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/Topography_3.png` & `freva_deployment-2405.0.0/docs/architecture/_static/Topography_3.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/TuiHowto.md` & `freva_deployment-2405.0.0/docs/deployment/TuiHowto.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Usage of the text user interface
 We have create a simple text user interface (tui) that helps you setting up a
 Freva instance at your institution. At this stage the documentation assumes that
 you have installed the necessary server infrastructure and pre-requisites.
-Please refer to the [installation](Installation.html) and [configuration section](Configuration.html)
+Please refer to the [installation](Installation) and [configuration section](Configure)
 for more details.
 
-After [Installation](Installation.html) the command `deploy-freva` will open
+After [Installation](Installation) the command `deploy-freva` will open
 the tui. The tui is organized in five different screens. The first four screens
 are used to configure the services (core, solr, database, web) the last screen
 (run screen) configures variables that are common amongst all services.
 The code of the tui is written using the [npyscreen](https://npyscreen.readthedocs.io/index.html)
 library.
 
 ## General usage
@@ -39,15 +39,15 @@
 The first screen configures the setup of Freva at the HPC system. We refer to
 this step as the *core* deployment. At the top of the screen you'll see a tick
 box, which indicates whether or not this step is used for deployment. If this
 box is *un*ticked - tick/untick using the `<SPACE>` key - the deployment will
 skip the core installation on the HPC system. The following explains the
 essential setup steps:
 
-![](tui_core.png)
+![](_static/tui_core.png)
 
 1. The host name(s) where the core installation is executed. You can use all
    [multi host patterns](https://docs.ansible.com/ansible/latest/user_guide/intro_patterns.html#common-patterns)
    that ansible supports.
 2. The installation directory of the anaconda environment where the
    `evaluation_system` library is installed.
 3. Tick/Untick this box to install (override) a new anaconda environment. Unticking
@@ -105,15 +105,15 @@
 ## Web ui setup
 The second screen configures the setup web ui. At the top of the screen
 you'll see a tick box, which indicates whether or not this step is used for
 deployment. If this box is *un*ticked - tick/untick using the `<SPACE>` key -
 the deployment will skip the web ui setup entirely. The following explains the
 essential setup steps:
 
-![](tui_web.png)
+![](_static/tui_web.png)
 
 1. The host name where the web ui should be installed. This should be a single
    host name.
 2. The url the web ui can be accessed. Users will use this url to get access
    to the url.
 3. Main html color scheme.
 4. Html color for borders.
@@ -194,55 +194,53 @@
 it easy for users to communicate and share results with other users.
 Login credentials are needed to connect to the email server and send emails.
 Your credentials won't be saved anywhere on disk but securely stored in the
 vault service that gets deployed when setting up the database.
 
 
 
-## Solr server setup
-The third screen configures the setup apache solr serch server. At the top of
+## Databrowser server setup
+The third screen configures the setup databrowser server. At the top of
 the screen you'll see a tick box, which indicates whether or not this step is
 used for deployment. If this box is *un*ticked - tick/untick using the
-`<SPACE>` key - the deployment will skip the setup of solr entirely. The
+`<SPACE>` key - the deployment will skip the setup of databrowser entirely. The
 following explains the essential setup steps:
 
-![](tui_solr.png)
+![](_static/tui_solr.png)
 
 1. The host name where the solr server should be installed. This should be a single
    host name.
-2. Tick this box (`<SPACE>`) if you want to delete any pre existing solr data.
-3. Select how much memory you want to allocate for the solr server process.
-4. Select the port the solr server is running on.
+2. Tick this box (`<SPACE>`) if you want to delete any pre existing databrowser data.
+3. Select how much memory you want to allocate for the databrowser server process.
+4. Select the port the databrowser server is running on.
 5. If you want to customise the installation process you can set the path
    to a custom ansible playbook here. If this is set then the deployment
    will use this playbook instead of the default playbook that ships with
    the system. Leave blank for default behaviour.
 6. Set the user name that should execute the container commands, defaults
    to root. Leave blank if no special user is needed.
 7. Set the path to the `python3.4+` binary, this should be set if the python
    binary is not part of the `$PATH` variable.
 8. Set the login user name for the remote machine.
 
-### Notes on the solr setup
-Although still configurable, the name of the solr core (files) might be
-fixed in the future. Therefore we recommend using the default value. Any
-existing solr data is *not* overridden if you deploy
-a new solr server and do not chose to delete any pre existing data. The
-solr core data will be saved to `/opt/freva/<project_name>/solr_service/`
-on the host name the solr server is running on.
+### Notes on the databrowser setup
+Any existing data is *not* overridden if you deploy
+a new server and do not chose to delete any pre existing data. The
+data will be saved to `/opt/freva/<project_name>/databrowser_service/`
+on the host name the databrowser server is running on.
 
 
 ## Database server setup
 The fourth screen configures the setup database server. At the top of
 the screen you'll see a tick box, which indicates whether or not this step is
 used for deployment. If this box is *un*ticked - tick/untick using the
 `<SPACE>` key - the deployment will skip the setup of the database entirely. The
 following explains the essential setup steps:
 
-![](tui_db.png)
+![](_static/tui_db.png)
 
 1. The host name where the database server should be installed. This should be a single
    host name.
 2. Tick this box (`<SPACE>`) if you want to delete any pre existing databases.
 3. Set the database user name.
 4. Set the database name.
 5. Set the port the database server is running on.
@@ -271,15 +269,15 @@
 
 ## The run screen.
 The last of the five screen is the so called run screen. This screen sets up a
 configuration that is common among the above described steps. You can enter this
 screen by pressing the `CTRL+r` key combination. The following options are
 available:
 
-![](tui_run.png)
+![](_static/tui_run.png)
 
 1. Set a unique project name for this specific Freva instance, for example
    `clex-ces`.
 2. If desired you can save the already configured settings to a
 [`toml`](https://toml.io/en/) configuration file.
 3. If you've set up a service that keeps track of all installed Freva instances
 at your institution you can specify the host name here. Please refer to the
```

### Comparing `freva_deployment-2309.0.1/docs/Variable.png` & `freva_deployment-2405.0.0/docs/deployment/_static/Variable.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/conf.py` & `freva_deployment-2405.0.0/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 from datetime import date
+
 from recommonmark.parser import CommonMarkParser
 
 sys.path.insert(0, os.path.abspath("."))
 sys.path.insert(0, os.path.abspath("../../src"))
 
 from freva_deployment import __version__
 
@@ -35,19 +36,17 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
-    "nbsphinx",
     "recommonmark",
-    "sphinx.ext.viewcode",
-    "sphinxcontrib_github_alt",
     "sphinx_copybutton",
+    "sphinx_togglebutton",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -57,54 +56,74 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-html_logo = "freva_owl.svg"
-html_favicon = "freva_owl.svg"
+html_logo = "_static/freva_owl.svg"
+html_favicon = "_static/freva_owl.svg"
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
+html_sidebars = {"pagename": []}
 html_static_path = ["_static"]
+html_context = {
+    "github_user": "FREVA-CLINT",
+    "github_repo": "freva",
+    "github_version": "main",
+    "doc_path": "docs",
+}
+html_sidebars = {
+    "community/index": [
+        "sidebar-nav-bs",
+        "custom-template",
+    ],  # This ensures we test for custom sidebars
+}
+
+source_parsers = {
+    ".md": CommonMarkParser,
+}
 html_theme_options = {
     "icon_links": [
         {
             "name": "GitHub",
             "url": "https://github.com/FREVA-CLINT/freva-deployment",
             "icon": "fa-brands fa-github",
-        }
+        },
+        {
+            "name": "PyPI",
+            "url": "https://pypi.org/project/freva-deployment",
+            "icon": "fa-custom fa-pypi",
+        },
     ],
-    "navigation_with_keys": True,
+    # "navbar_start": [],  # Remove navigation links from the top bar
+    "navbar_center": ["navbar-nav"],  # Add navigation links to the left sidebar
     "collapse_navigation": False,
-    "top_of_page_button": "edit",
     "navigation_depth": 4,
     "navbar_align": "left",
     "show_nav_level": 2,
-    "navigation_depth": 4,
-    #    "primary_sidebar_end": ["indices.html", "sidebar-ethical-ads.html"],
-    "navbar_center": ["navbar-nav"],
     "secondary_sidebar_items": ["page-toc"],
-    "light_css_variables": {
-        "color-brand-primary": "tomato",
-    },
 }
-html_context = {
-    "github_user": "FREVA-CLINT",
-    "github_repo": "freva",
-    "github_version": "main",
-    "doc_path": "docs",
-}
-# html_sidebars = {
-#    "**": [
-#        "search-field.html",
-#        "sidebar-nav-bs.html",
-#        "sidebar-ethical-ads.html",
-#    ]
-# }
+html_sidebars = {"**": ["sidebar-nav-bs", "sidebar-ethical-ads"]}
 
-source_parsers = {
-    ".md": CommonMarkParser,
-}
 
 source_suffix = [".rst", ".md"]
+
+
+# -- MyST options ------------------------------------------------------------
+
+# This allows us to use ::: to denote directives, useful for admonitions
+myst_enable_extensions = ["colon_fence", "linkify", "substitution"]
+myst_heading_anchors = 2
+myst_substitutions = {"rtd": "[Read the Docs](https://readthedocs.org/)"}
+
+# ReadTheDocs has its own way of generating sitemaps, etc.
+if not os.environ.get("READTHEDOCS"):
+    extensions += ["sphinx_sitemap"]
+
+    html_baseurl = os.environ.get("SITEMAP_URL_BASE", "http://127.0.0.1:8000/")
+    sitemap_locales = [None]
+    sitemap_url_scheme = "{link}"
+
+# specifying the natural language populates some key tags
+language = "en"
```

### Comparing `freva_deployment-2309.0.1/docs/freva_flowchart-new.jpg` & `freva_deployment-2405.0.0/docs/architecture/_static/freva_flowchart-new.jpg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/freva_owl.svg` & `freva_deployment-2405.0.0/docs/_static/freva_owl.svg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/index.rst` & `freva_deployment-2405.0.0/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .. freva-deployment documentation master file, created by
    sphinx-quickstart on Tue Mar  1 16:19:20 2022.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-Welcome to freva admin documentation!
-=====================================
+The freva admin documentation!
+==============================
 
-.. image:: freva_flowchart-new.jpg
+.. image:: architecture/_static/freva_flowchart-new.jpg
    :width: 320
    :align: center
 
 
 
 Freva, the free evaluation system framework, is a data search and analysis
 platform developed by the atmospheric science community for the atmospheric
@@ -44,30 +44,33 @@
 Because Freva is a software that is meant to run on HPC type distributed systems
 this documentation first gives an overview of various deployment strategies.
 After this section a basic configuration that is necessary to make the different
 components of Freva work with each other is introduced. This is followed by a
 documentation on how to install the Freva deployment software. After this section
 basic deployment setup and servicing Freva will be introduced.
 
+.. note::
+
+    Please check :ref:`whatsnew` for any update announcments.
+
+
+
+
 .. toctree::
-   :maxdepth: 3
-   :caption: Contents:
+   :maxdepth: 2
 
-   Architecture
-   Folders
-   Installation
-   Configure
-   AfterDeployment
-   Services
-   TuiHowto
-   Transition
-   LegalNotes
-   modules
+   architecture/index
 
+.. toctree::
+   :maxdepth: 2
+
+   deployment/index
+.. toctree::
+   :maxdepth: 2
 
+   after-deployment/index
+
+.. toctree::
+   :maxdepth: 1
 
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+   whatsnew
+   contributing
```

### Comparing `freva_deployment-2309.0.1/docs/make.bat` & `freva_deployment-2405.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/tui_core.png` & `freva_deployment-2405.0.0/docs/deployment/_static/tui_core.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/tui_db.png` & `freva_deployment-2405.0.0/docs/deployment/_static/tui_db.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/tui_run.png` & `freva_deployment-2405.0.0/docs/deployment/_static/tui_run.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/tui_solr.png` & `freva_deployment-2405.0.0/docs/deployment/_static/tui_solr.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/docs/tui_web.png` & `freva_deployment-2405.0.0/docs/deployment/_static/tui_web.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/mypy.ini` & `freva_deployment-2405.0.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.1/pyproject.toml` & `freva_deployment-2405.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core >=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "freva-deployment"
 authors = [{name = "DKRZ, Clint", email = "freva@dkrz.de"}]
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -14,51 +14,95 @@
                "Intended Audience :: Science/Research",
                "License :: OSI Approved :: BSD License",
                "Operating System :: POSIX :: Linux",
                "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
 description = "Deployment of the Free Evaluation Framework Freva"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [ "appdirs",
-             "ansible>=2.10",
+             "ansible",
+             "ansible-runner",
              "npyscreen",
-             "numpy",
              "PyMySQL",
              "PyYAML",
              "rich",
+             "rich-argparse",
              "toml",
              "tomlkit",
              "requests",
 ]
 [project.optional-dependencies]
-docs = [
-    "pydata-sphinx-theme",
-    "sphinx",
-    "sphinx-copybutton",
-    "nbsphinx",
-    "recommonmark",
-    "sphinx_rtd_theme",
-    "ipython",
-    "sphinxcontrib_github_alt",
+dev = ["flit", "tox"]
+doc = ["pydata-sphinx-theme",
+       "sphinx",
+       "sphinx-copybutton",
+       "recommonmark",
+       "sphinx_sitemap",
+       "sphinx_favicon",
+       "sphinx_togglebutton",
+       "myst-parser",
+       "sphinx-design",
+       "linkify",
+       "sphinx-execute-code-python3",
 ]
-test = ["mypy", "black", "isort", "types-toml", "types-PyMySQL"]
 
 [project.urls]
 Documentation = "https://freva-deployment.readthedocs.io/en/latest/"
-Issues = "https://github.com/FREVA-CLINT/freva/issues"
-Source = "https://github.com/FREVA-CLINT/freva"
+Issues = "https://github.com/FREVA-CLINT/freva-deployment/issues"
+Source = "https://github.com/FREVA-CLINT/freva-deployment"
 Home = "https://freva-deployment.readthedocs.io/en/latest"
 
 [project.scripts]
 deploy-freva-cmd = "freva_deployment.cli:deploy"
-deploy-freva-map = "freva_deployment.cli:server_map"
-freva-service = "freva_deployment.cli:service"
 freva-migrate = "freva_deployment.cli:migrate"
 deploy-freva = "freva_deployment.ui.deployment_tui:tui"
 
 
 [tool.flit.sdist]
 include = ["assets/*"]
 
 [tool.flit.external-data]
 directory = "assets"
+
+[package-data]
+freva_deployment = ["py.typed", "versions.json"]
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+min_version = 4.0
+env_list = types, lint, test
+[testenv]
+parallel_show_output = false
+[testenv:test]
+deps = -e .
+
+commands =
+    deploy-freva-cmd --help
+    deploy-freva --help
+
+[testenv:docs]
+deps = .[doc]
+allowlist_externals = make
+commands = make -C docs clean
+           make -C docs html
+[testenv:lint]
+deps = .
+       black
+       isort
+commands =
+    isort --check --profile black -t py311 -l 79 src
+[testenv:types]
+deps = .
+       mypy
+       types-toml
+       pytest-stub
+       types-PyMySQL
+commands = mypy --install-types --non-interactive
+[testenv:release]
+deps = git-python
+       packaging
+       tomli
+       requests
+commands = python3 release.py tag freva_deployment -b versions
+"""
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2405.0.0/src/freva_deployment/cli/_deploy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,106 @@
 """Command line interface for the deployment."""
+
 from __future__ import annotations
 
 import argparse
 import sys
 from pathlib import Path
 
+from rich_argparse import ArgumentDefaultsRichHelpFormatter
+
 from freva_deployment import __version__
 
 from ..deploy import DeployFactory
-from ..utils import config_dir, guess_map_server, set_log_level
+from ..error import DeploymentError
+from ..logger import set_log_level
+from ..utils import config_dir
+from ..versions import VersionAction, display_versions
 
 
 def parse_args(argv: list[str] | None) -> argparse.Namespace:
     """Consturct command line argument parser."""
 
     ap = argparse.ArgumentParser(
         prog="deploy-freva-cmd",
         description="Deploy freva and its services on different machines.",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-    ap.add_argument(
-        "--server-map",
-        type=str,
-        default=None,
-        help=(
-            "Hostname of the service mapping the freva server "
-            "archtiecture, Note: you can create a server map by "
-            "running the deploy-freva-map command"
-        ),
+        formatter_class=ArgumentDefaultsRichHelpFormatter,
     )
     ap.add_argument(
         "--config",
         "-c",
         type=Path,
         help="Path to ansible inventory file.",
         default=config_dir / "inventory.toml",
     )
     ap.add_argument(
         "--steps",
+        "-s",
         type=str,
         nargs="+",
-        default=["db", "solr", "web", "core"],
-        choices=["web", "core", "db", "solr"],
-        help="The services/code stack to be deployed",
+        default=["db", "freva-rest", "web", "core"],
+        choices=["web", "core", "db", "freva-rest", "auto"],
+        help=(
+            "The services/code stack to be deployed. Use [it]auto[/it]"
+            " to only deploy outdated services"
+        ),
     )
     ap.add_argument(
         "--ask-pass",
         help="Connect to server via ssh passwd instead of public key.",
         action="store_true",
         default=False,
     )
     ap.add_argument(
+        "--ssh-port",
+        help="Set the ssh port, in 99.9%% of the cases this should be 22",
+        type=int,
+        default=22,
+    )
+    ap.add_argument(
         "-v", "--verbose", action="count", help="Verbosity level", default=0
     )
     ap.add_argument(
+        "-l",
+        "--local",
+        help="Deploy services on the local machine, debug purpose.",
+        action="store_true",
+        default=False,
+    )
+    ap.add_argument(
+        "-g",
+        "--gen-keys",
+        help="Generate public and private web certs, use with caution.",
+        action="store_true",
+        default=False,
+    )
+    ap.add_argument(
         "-V",
         "--version",
-        action="version",
-        version="%(prog)s {version}".format(version=__version__),
+        action=VersionAction,
+        version="[b][red]%(prog)s[/red] {version}[/b]{services}".format(
+            version=__version__, services=display_versions()
+        ),
     )
     return ap.parse_args()
 
 
 def cli(argv: list[str] | None = None) -> None:
     """Run the command line interface."""
     args = parse_args(argv)
-    if args.server_map:
-        server_map = guess_map_server(args.server_map, mandatory=False)
-    else:
-        server_map = ""
     set_log_level(args.verbose)
     with DeployFactory(
-        steps=args.steps,
+        steps=[s.replace("-", "_") for s in args.steps],
         config_file=args.config,
+        local_debug=args.local,
+        gen_keys=args.gen_keys,
     ) as DF:
-        DF.play(server_map, args.ask_pass, args.verbose)
+        try:
+            _ = DF.play(args.ask_pass, args.verbose, ssh_port=args.ssh_port)
+        except KeyboardInterrupt:
+            raise SystemExit(130)
+        except DeploymentError:
+            raise SystemExit(1)
 
 
 if __name__ == "__main__":
     cli(sys.argv[1:])
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2405.0.0/src/freva_deployment/cli/_migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI to assist with migrating the system."""
+
 from __future__ import annotations
 
 import argparse
 import json
 import os
 import shlex
 import shutil
@@ -13,22 +14,16 @@
 from typing import TextIO, cast
 
 import pymysql
 import toml
 
 from freva_deployment import __version__
 
-from ..utils import (
-    download_server_map,
-    get_setup_for_service,
-    guess_map_server,
-    logger,
-    read_db_credentials,
-    set_log_level,
-)
+from ..logger import logger, set_log_level
+from ..utils import read_db_credentials
 
 DUMP_SCRIPT = """#!{python_bin}
 import json
 import sys
 sys.path.insert(0, "{python_path}")
 from evaluation_system.model.file import DRSFile
 
@@ -136,15 +131,17 @@
             )
             exec_command(dump_command, stdout=f_obj)
             _add_new_db(new_db_cfg, temp_file.name)
 
 
 def _migrate_drs(parser: argparse.Namespace) -> None:
     python_path = parser.python_path or _get_python_path_from_env()
-    config = json.loads(execute_script_and_get_config(python_path, DUMP_SCRIPT))
+    config = json.loads(
+        execute_script_and_get_config(python_path, DUMP_SCRIPT)
+    )
     logger.debug("Writing toml file to drs_config.toml")
     this_file = (Path(".") / "drs_config.toml").absolute()
     with open(this_file, "w") as f_obj:
         toml.dump(config, f_obj)
     logger.info(
         "Toml file has been written to %s, you can copy the file to its new "
         "location next to the evaluation_system.conf file\n Note: The "
@@ -167,15 +164,17 @@
     )
     parser.add_argument(
         "-V",
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
     )
-    subparsers = parser.add_subparsers(help="Migration commands:", required=True)
+    subparsers = parser.add_subparsers(
+        help="Migration commands:", required=True
+    )
     db_parser = subparsers.add_parser(
         "database",
         description="Freva database migration",
         help="Use this command to migrate an existing freva database "
         "to a recently set up system.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/deploy.py` & `freva_deployment-2405.0.0/src/freva_deployment/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,353 +1,515 @@
 """Module to run the freva deployment."""
+
 from __future__ import annotations
 
+import json
 import os
 import random
-import shlex
+import signal
 import string
 import sys
+import time
+from copy import deepcopy
 from getpass import getuser
+from io import StringIO
 from pathlib import Path
-from subprocess import run
-from tempfile import TemporaryDirectory
-from typing import Any
+from socket import gethostbyname, gethostname
+from typing import Any, cast
 from urllib.parse import urlparse
 
 import tomlkit
 import yaml
-from numpy import sign
-
+from ansible_runner import run
+from ansible_runner.runner import Runner
+from rich import print as pprint
+from rich.console import Console
+from rich.live import Live
+from rich.prompt import Prompt
+from rich.spinner import Spinner
+
+from freva_deployment import FREVA_PYTHON_VERSION
+
+from .error import ConfigurationError, DeploymentError, handled_exception
+from .keys import RandomKeys
+from .logger import logger
+from .runner import RunnerDir
 from .utils import (
-    AssetDir,
     RichConsole,
     asset_dir,
     config_dir,
     get_email_credentials,
     get_passwd,
     load_config,
-    logger,
-    upload_server_map,
 )
+from .versions import get_steps_from_versions
 
 
 class DeployFactory:
     """Apply freva deployment and its services.
 
     Parameters
     ----------
     project_name: str
         The name of the project to distinguish this instance from others.
-    steps: list[str], default: ["services", "core", "web"]
+    steps: list[str], default: ["core", "web", "freva_rest", "db"]
         The components that are going to be deployed.
     config_file: os.PathLike, default: None
         Path to any existing deployment configuration file.
+    local_debug: bool, default: False
+        Run deployment only on local machine, debug mode.
+    gen_keys: bool, default: False
+        Create new set of certificates, if they don't already exist.
 
     Examples
     --------
 
     >>> from freva_deployment import DeployFactory as DF
-    >>> deploy = DF(steps=["solr"])
+    >>> deploy = DF(steps=["freva_rest"])
     >>> deploy.play(ask_pass=True)
     """
 
-    step_order: tuple[str, ...] = ("vault", "db", "solr", "core", "web")
-    _steps_with_cert: tuple[str, ...] = ("db", "vault", "core", "web")
+    step_order: tuple[str, ...] = ("core", "db", "freva_rest", "web")
+    _steps_with_cert: tuple[str, ...] = ("core", "db", "web")
 
+    @handled_exception
     def __init__(
         self,
         steps: list[str] | None = None,
         config_file: Path | str | None = None,
+        local_debug: bool = False,
+        gen_keys: bool = False,
     ) -> None:
+        self.gen_keys = gen_keys or local_debug
+        self.local_debug = local_debug
         self._config_keys: list[str] = []
-        self.master_pass: str = ""
+        self._master_pass: str = ""
         self.email_password: str = ""
-        self._td: TemporaryDirectory = TemporaryDirectory(prefix="inventory")
-        self.inventory_file: Path = Path(self._td.name) / "inventory.yaml"
+        self._td: RunnerDir = RunnerDir()
         self.eval_conf_file: Path = (
-            Path(self._td.name) / "evaluation_system.conf"
+            self._td.parent_dir / "evaluation_system.conf"
         )
-        self.web_conf_file: Path = Path(self._td.name) / "freva_web.toml"
-        self.apache_config: Path = Path(self._td.name) / "freva_web.conf"
+        self.web_conf_file: Path = self._td.parent_dir / "freva_web.toml"
+        self.apache_config: Path = self._td.parent_dir / "freva_web.conf"
         self._db_pass: str = ""
-        self._steps = steps or ["services", "core", "web"]
+        self._steps = steps or ["db", "freva_rest", "web", "core"]
+        if self._steps == ["auto"] or self._steps == "auto":
+            self._steps = []
         self._inv_tmpl = Path(config_file or config_dir / "inventory.toml")
         self._cfg_tmpl = self.aux_dir / "evaluation_system.conf.tmpl"
         self.cfg = self._read_cfg()
         self.project_name = self.cfg.pop("project_name", None)
+        self._random_key = RandomKeys(self.project_name or "freva")
         self.playbooks: dict[str, Path | None] = {}
         if not self.project_name:
-            raise ValueError("You must set a project name")
+            raise ConfigurationError("You must set a project name") from None
+        self._set_hostnames()
+        self.current_step = ""
+        self._check_steps_()
+
+    def _check_steps_(self) -> None:
+        """Before we do anything check if something is wrong with the config."""
+        # First the steps that are needed
+        old_master = self._master_pass
+        self._master_pass = old_master or "foo"
+        not_in_use = set(["db", "freva_rest", "web", "core"]) - set(self.steps)
+        # We temporary set the env variables for email user and email password
+        # This is not pretty but prevents the password dialogs, which aren't
+        # needed at this step to show up.
+        # Later we will set everything back as it was.
+        current_values = {}
+        for key in ("EMAIL_USER", "EMAIL_PASSWD"):
+            current_values[key] = os.environ.get(key, "")
+            os.environ[key] = current_values[key] or "foo"
+        for step in self.steps:
+            getattr(self, f"_prep_{step.replace('-', '_')}")()
+        for step in not_in_use:
+            try:
+                getattr(self, f"_prep_{step.replace('-', '_')}")()
+            except ConfigurationError as error:
+                logger.warning("Some of your config isn't valid:\n%s", error)
+        for key, value in current_values.items():
+            os.environ[key] = current_values[key]
+        self._master_pass = old_master
+
+    @property
+    def master_pass(self) -> str:
+        """Define the master password."""
+        if self._master_pass:
+            return self._master_pass
+        self._master_pass = get_passwd(os.environ.get("MASTER_PASSWD", ""))
+        return self._master_pass
 
     @property
     def public_key_file(self) -> str:
         """Path to the public certificate file."""
         public_keyfile = self.cfg["certificates"].get("public_keyfile")
         chain_keyfile = self.cfg["certificates"].get("chain_keyfile")
         if public_keyfile:
             return str(Path(public_keyfile).expanduser().absolute())
         if chain_keyfile:
             return str(Path(chain_keyfile).expanduser().absolute())
-        raise ValueError("You must give a valid path to a public key file.")
+        if self.gen_keys:
+            return self._random_key.public_chain_file
+        raise ConfigurationError(
+            "You must give a valid path to a public key file."
+        ) from None
 
     @property
     def private_key_file(self) -> str:
         """Path to the private key file."""
         keyfile = self.cfg["certificates"].get("private_keyfile")
         if keyfile:
             return str(Path(keyfile).expanduser().absolute())
-        raise ValueError("You must give a valid path to a private key file.")
-
-    @property
-    def chain_key_file(self) -> str:
-        """Path to the private key file."""
-        keyfile = self.cfg["certificates"].get("chain_keyfile")
-        if keyfile:
-            return str(Path(keyfile).expanduser().absolute())
-        return ""
+        if self.gen_keys:
+            return self._random_key.private_key_file
+        raise ConfigurationError(
+            "You must give a valid path to a private key file."
+        ) from None
 
     def _prep_vault(self) -> None:
         """Prepare the vault."""
-        self._config_keys.append("vault")
-        self.cfg["vault"] = self.cfg["db"].copy()
         self.cfg["vault"]["config"].setdefault("ansible_become_user", "root")
-        self.playbooks["vault"] = self.cfg["db"]["config"].get(
-            "vault_playbook"
-        )
-        if not self.master_pass:
-            self.master_pass = get_passwd()
+        self.cfg["vault"]["config"].pop("db_playbook", "")
+        self.cfg["vault"]["config"]["db_port"] = self.cfg["vault"][
+            "config"
+        ].get("port", 3306)
+        self.cfg["vault"]["config"]["db_user"] = self.cfg["vault"][
+            "config"
+        ].get("user", "")
         self.cfg["vault"]["config"]["root_passwd"] = self.master_pass
         self.cfg["vault"]["config"]["passwd"] = self.db_pass
         self.cfg["vault"]["config"]["keyfile"] = self.public_key_file
         self.cfg["vault"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
+        self.cfg["vault"]["config"]["db_host"] = self.cfg["db"]["config"][
+            "host"
+        ]
 
     def _prep_db(self) -> None:
         """prepare the mariadb service."""
         self._config_keys.append("db")
         self.cfg["db"]["config"].setdefault("ansible_become_user", "root")
-        if not self.master_pass:
-            self.master_pass = get_passwd()
         host = self.cfg["db"]["hosts"]
         self.cfg["db"]["config"]["root_passwd"] = self.master_pass
         self.cfg["db"]["config"]["passwd"] = self.db_pass
         self.cfg["db"]["config"]["keyfile"] = self.public_key_file
+        data_path = Path(
+            cast(
+                str,
+                self.cfg["db"]["config"].get("data_path", "/opt/freva"),
+            )
+        )
+        self.cfg["db"]["config"]["data_path"] = str(data_path)
         for key in ("name", "user", "db"):
             self.cfg["db"]["config"][key] = (
                 self.cfg["db"]["config"].get(key) or "freva"
             )
-        db_host = self.cfg["db"]["config"].get("host", "")
+        db_host = self.cfg["db"]["config"].get("host", "").strip()
         if not db_host:
             self.cfg["db"]["config"]["host"] = host
         self.cfg["db"]["config"].setdefault("port", "3306")
         self.cfg["db"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
         self.playbooks["db"] = self.cfg["db"]["config"].get("db_playbook")
         self._prep_vault()
+        self._prep_web(False)
 
-    def _prep_solr(self) -> None:
-        """prepare the apache solr service."""
-        self._config_keys.append("solr")
-        self.cfg["solr"]["config"].setdefault("ansible_become_user", "root")
-        self.cfg["solr"]["config"].pop("core", None)
-        self.playbooks["solr"] = self.cfg["solr"]["config"].get(
-            "solr_playbook"
-        )
-        for key, default in dict(mem="4g", port=8983).items():
-            self.cfg["solr"]["config"][key] = (
-                self.cfg["solr"]["config"].get(key) or default
+    def _prep_freva_rest(self, prep_web=True) -> None:
+        """prepare the freva_rest service."""
+        self._config_keys.append("freva_rest")
+        self.cfg["freva_rest"]["config"].setdefault(
+            "ansible_become_user", "root"
+        )
+        self.cfg["freva_rest"]["config"]["root_passwd"] = self.master_pass
+        self.cfg["freva_rest"]["config"].pop("core", None)
+        data_path = Path(
+            cast(
+                str,
+                self.cfg["freva_rest"]["config"].get(
+                    "data_path", "/opt/freva"
+                ),
             )
-        self.cfg["solr"]["config"]["email"] = self.cfg["web"]["config"].get(
-            "contacts", ""
         )
+        self.cfg["freva_rest"]["config"]["data_path"] = str(data_path)
+        self.playbooks["freva_rest"] = self.cfg["freva_rest"]["config"].get(
+            "freva_rest_playbook"
+        )
+        for key, default in dict(solr_mem="4g", freva_rest_port=7777).items():
+            self.cfg["freva_rest"]["config"][key] = (
+                self.cfg["freva_rest"]["config"].get(key) or default
+            )
+        self.cfg["freva_rest"]["config"]["email"] = self.cfg["web"][
+            "config"
+        ].get("contacts", "")
+        if prep_web:
+            self._prep_web(False)
 
     def _prep_core(self) -> None:
         """prepare the core deployment."""
         self._config_keys.append("core")
         self.cfg["core"]["config"].setdefault("ansible_become_user", "")
         self.playbooks["core"] = self.cfg["core"]["config"].get(
             "core_playbook"
         )
+        # Legacy args as we are going to use micromamba
+        self.cfg["core"]["config"]["arch"] = (
+            self.cfg["core"]["config"]
+            .get("arch", "linux-64")
+            .lower()
+            .replace("x86_", "")
+            .replace("mac", "")
+        )
+        self.cfg["core"]["config"]["python_version"] = FREVA_PYTHON_VERSION
         self.cfg["core"]["config"]["admins"] = (
             self.cfg["core"]["config"].get("admins") or getuser()
         )
         if not self.cfg["core"]["config"]["admins"]:
             self.cfg["core"]["config"]["admins"] = getuser()
-        install_dir = self.cfg["core"]["config"]["install_dir"]
-        root_dir = self.cfg["core"]["config"].get("root_dir", "")
-        if not root_dir:
-            self.cfg["core"]["config"]["root_dir"] = install_dir
+        install_dir = Path(self.cfg["core"]["config"]["install_dir"])
+        root_dir = Path(
+            self.cfg["core"]["config"].get("root_dir", "") or install_dir
+        )
+        self.cfg["core"]["config"]["install_dir"] = str(install_dir)
+        self.cfg["core"]["config"]["root_dir"] = str(root_dir)
         preview_path = self.cfg["core"]["config"].get("preview_path", "")
         base_dir_location = self.cfg["core"]["config"].get(
             "base_dir_location", ""
-        )
+        ) or str(root_dir / "work")
+        self.cfg["core"]["config"]["base_dir_location"] = base_dir_location
         scheduler_output_dir = self.cfg["core"]["config"].get(
             "scheduler_output_dir", ""
         )
         scheduler_system = self.cfg["core"]["config"].get(
             "scheduler_system", "local"
         )
         if not preview_path:
-            if base_dir_location:
-                self.cfg["core"]["config"]["preview_path"] = str(
-                    Path(base_dir_location) / "share" / "preview"
-                )
-            else:
-                self.cfg["core"]["config"]["preview_path"] = ""
+            self.cfg["core"]["config"]["preview_path"] = str(
+                Path(base_dir_location) / "share" / "preview"
+            )
         if not scheduler_output_dir:
             scheduler_output_dir = str(Path(base_dir_location) / "share")
-        scheduler_output_dir = Path(scheduler_output_dir) / scheduler_system
+        elif Path(scheduler_output_dir).parts[-1] != scheduler_system:
+            scheduler_output_dir = (
+                Path(scheduler_output_dir) / scheduler_system
+            )
         self.cfg["core"]["config"]["scheduler_output_dir"] = str(
             scheduler_output_dir
         )
         self.cfg["core"]["config"]["keyfile"] = self.public_key_file
         git_exe = self.cfg["core"]["config"].get("git_path")
         self.cfg["core"]["config"]["git_path"] = git_exe or "git"
         self.cfg["core"]["config"][
             "git_url"
         ] = "https://github.com/FREVA-CLINT/freva.git"
 
-    def _prep_web(self) -> None:
+    def _prep_web(self, ask_pass: bool = True) -> None:
         """prepare the web deployment."""
         self._config_keys.append("web")
         self.playbooks["web"] = self.cfg["web"]["config"].get("web_playbook")
         self.cfg["web"]["config"].setdefault("ansible_become_user", "root")
         self._prep_core()
+        freva_rest_host = (
+            f'{self.cfg["freva_rest"]["hosts"]}:'
+            f'{self.cfg["freva_rest"]["config"]["freva_rest_port"]}'
+        )
+        self.cfg["web"]["config"]["freva_rest_host"] = freva_rest_host
+        self.cfg["web"]["config"].setdefault("deploy_web_server", True)
+        data_path = Path(
+            cast(
+                str,
+                self.cfg["web"]["config"].get("data_path", "/opt/freva"),
+            )
+        )
+        self.cfg["web"]["config"]["data_path"] = str(data_path)
         admin = self.cfg["core"]["config"]["admins"]
+        try:
+            for k, v in self.cfg["web"]["config"].items():
+                self.cfg["web"]["config"].setdefault(k, "")
+        except KeyError:
+            raise ConfigurationError(
+                "No web config section given, please configure the web.config"
+            ) from None
         if not isinstance(admin, str):
             self.cfg["web"]["config"]["admin"] = admin[0]
         else:
             self.cfg["web"]["config"]["admin"] = admin
-        _webserver_items = {}
-        try:
-            for k, v in self.cfg["web"]["config"].items():
-                key = k.replace("web_", "").upper()
-                if key not in ("LDAP_USER_PW", "LDAP_USER_DN"):
-                    _webserver_items[key] = v
-                else:
-                    self.cfg["web"]["config"].setdefault(k, "")
-        except KeyError as error:
-            raise KeyError(
-                "No web config section given, please configure the web.config"
-            ) from error
-        _webserver_items["ALLOWED_HOSTS"].append(self.cfg["web"]["hosts"])
-        _webserver_items["REDIS_HOST"] = self.cfg["web"]["hosts"]
+        allowed_hosts = self.cfg["web"]["config"].get("allowed_hosts") or [
+            "localhost"
+        ]
+        allowed_hosts.append(self.cfg["web"]["hosts"])
+        allowed_hosts.append(f"{self.project_name}-httpd")
+        self.cfg["web"]["config"]["allowed_hosts"] = list(set(allowed_hosts))
+        self.cfg["web"]["config"].setdefault("allowed_hosts", ["localhost"])
+
+        _webserver_items = {
+            "institution_logo": self.cfg["web"]["config"].get(
+                "institution_logo", ""
+            ),
+            "main_color": self.cfg["web"]["config"].get(
+                "main_color", "Tomato"
+            ),
+            "border_color": self.cfg["web"]["config"].get(
+                "border_color", "#6c2e1f"
+            ),
+            "hover_color": self.cfg["web"]["config"].get(
+                "hover_color", "#d0513a"
+            ),
+            "homepage_text": self.cfg["web"]["config"].get(
+                "homepage_text", ""
+            ),
+            "imprint": self.cfg["web"]["config"].get("imprint", []),
+            "homepage_heading": self.cfg["web"]["config"].get(
+                "homepage_heading", ""
+            ),
+            "about_us_text": self.cfg["web"]["config"].get(
+                "about_us_text", ""
+            ),
+            "contacts": self.cfg["web"]["config"].get("contacts", []),
+            "insitution_name": self.cfg["web"]["config"].get(
+                "insitution_name", ""
+            ),
+            "menu_entries": self.cfg["web"]["config"].get("menu_entries", []),
+        }
         try:
             with Path(_webserver_items["homepage_text"]).open("r") as f_obj:
                 _webserver_items["homepage_text"] = f_obj.read()
         except (FileNotFoundError, IOError, KeyError):
             pass
+        try:
+            with Path(_webserver_items["about_us_text"]).open() as f_obj:
+                _webserver_items["about_us_text"] = f_obj.read()
+        except (FileNotFoundError, IOError, KeyError):
+            pass
+        with self.web_conf_file.open("w") as f_obj:
+            tomlkit.dump(_webserver_items, f_obj)
+
+        if self.local_debug:
+            self.cfg["web"]["config"]["redis_host"] = self.cfg["web"]["hosts"]
+        else:
+            self.cfg["web"]["config"][
+                "redis_host"
+            ] = f"{self.project_name}-redis"
+
         server_name = self.cfg["web"]["config"].pop("server_name", [])
         if isinstance(server_name, str):
             server_name = server_name.split(",")
         server_name = ",".join([a for a in server_name if a.strip()])
         if not server_name:
             server_name = self.cfg["web"]["hosts"]
         self.cfg["web"]["config"]["server_name"] = server_name
         web_host = self.cfg["web"]["hosts"]
         if web_host == "127.0.0.1":
             web_host = "localhost"
         self.cfg["web"]["config"]["host"] = web_host
-        _webserver_items["CSRF_TRUSTED_ORIGINS"] = []
+        self.cfg["web"]["config"]["csrf_trusted_origins"] = []
         for url in (server_name, self.cfg["web"]["config"]["project_website"]):
             trusted_origin = urlparse(url)
 
             if trusted_origin.scheme:
-                _webserver_items["CSRF_TRUSTED_ORIGINS"].append(
+                self.cfg["web"]["config"]["csrf_trusted_origins"].append(
                     f"https://{trusted_origin.netloc}"
                 )
             else:
-                _webserver_items["CSRF_TRUSTED_ORIGINS"].append(
+                self.cfg["web"]["config"]["csrf_trusted_origins"].append(
                     f"https://{trusted_origin.path}"
                 )
-        _webserver_items["FREVA_BIN"] = os.path.join(
+        self.cfg["web"]["config"]["freva_bin"] = os.path.join(
             self.cfg["core"]["config"]["install_dir"], "bin"
         )
-        try:
-            with Path(_webserver_items["ABOUT_US_TEXT"]).open() as f_obj:
-                _webserver_items["ABOUT_US_TEXT"] = f_obj.read()
-        except (FileNotFoundError, IOError, KeyError):
-            pass
-        try:
-            _webserver_items["IMPRINT"] = _webserver_items["IMPRINT"].split(
-                ","
-            )
-        except AttributeError:
-            pass
-        with self.web_conf_file.open("w") as f_obj:
-            tomlkit.dump(_webserver_items, f_obj)
         for key in ("core", "web"):
             self.cfg[key]["config"]["config_toml_file"] = str(
                 self.web_conf_file
             )
-        if not self.master_pass:
-            self.master_pass = get_passwd()
-        email_user, self.email_password = get_email_credentials()
         self._prep_vault()
+        if ask_pass:
+            email_user, self.email_password = get_email_credentials()
+            self.cfg["vault"]["config"]["email_user"] = email_user
+            self.cfg["vault"]["config"]["email_password"] = self.email_password
         self.cfg["vault"]["config"]["ansible_python_interpreter"] = self.cfg[
             "db"
         ]["config"].get("ansible_python_interpreter", "/usr/bin/python3")
-        self.cfg["vault"]["config"]["email_user"] = email_user
-        self.cfg["vault"]["config"]["email_password"] = self.email_password
         self.cfg["web"]["config"]["root_passwd"] = self.master_pass
         self.cfg["web"]["config"]["private_keyfile"] = self.private_key_file
         self.cfg["web"]["config"]["public_keyfile"] = self.public_key_file
-        self.cfg["web"]["config"]["chain_keyfile"] = (
-            self.chain_key_file or self.public_key_file
-        )
         self.cfg["web"]["config"]["apache_config_file"] = str(
             self.apache_config
         )
-        self._prep_apache_config()
+        if ask_pass:
+            self._prep_apache_config()
 
     def _prep_apache_config(self):
-        config = []
-        with (Path(asset_dir) / "web" / "freva_web.conf").open() as f_obj:
-            for line in f_obj.readlines():
+        with open(self.apache_config, "w") as f_obj:
+            f_obj.write(
+                (Path(asset_dir) / "web" / "freva_web.conf").read_text()
+            )
+
+    def _set_hostnames(self) -> None:
+        """Set the hostnames from the config or if debug the alias."""
+        default_ports = {"db": 3306, "freva_rest": 8080}
+        if self.local_debug:
+            for step in self.steps:
                 if (
-                    not self.chain_key_file
-                    and "SSLCertificateChainFile" in line
+                    isinstance(self.cfg[step], dict)
+                    and "hosts" in self.cfg[step]
                 ):
-                    continue
-                config.append(line)
-        with open(self.apache_config, "w") as f_obj:
-            f_obj.write("".join(config))
+                    self.cfg[step]["hosts"] = gethostbyname(gethostname())
+                if step in ("db", "freva_rest"):
+                    self.cfg[step]["config"]["port"] = default_ports[step]
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self._td.cleanup()
 
     def _read_cfg(self) -> dict[str, Any]:
         try:
-            return dict(load_config(self._inv_tmpl))
-        except FileNotFoundError as error:
-            raise FileNotFoundError(
+            config = dict(load_config(self._inv_tmpl).items())
+            config["vault"] = deepcopy(config["db"])
+            return config
+        except FileNotFoundError:
+            raise ConfigurationError(
                 f"No such file {self._inv_tmpl}"
-            ) from error
+            ) from None
+        except KeyError:
+            raise ConfigurationError("You must define a db section") from None
 
     def _check_config(self) -> None:
         sections = []
+        config_keys = deepcopy(self._config_keys)
+        if "db" in config_keys:
+            config_keys.append("vault")
         for section in self.cfg.keys():
-            for step in self._config_keys:
+            for step in config_keys:
                 if section.startswith(step) and section not in sections:
                     sections.append(section)
         for section in sections:
             for key, value in self.cfg[section]["config"].items():
                 if (
                     not value
                     and not self._empty_ok
                     and not isinstance(value, bool)
                 ):
-                    raise ValueError(
+                    raise ConfigurationError(
                         f"{key} in {section} is empty in {self._inv_tmpl}"
-                    )
+                    ) from None
+
+    @property
+    def ask_become_password(self) -> bool:
+        """Check if we have to ask for the sudo passwd at all."""
+        cfg = deepcopy(self.cfg)
+        solr_config = cfg.get("databrowser", cfg.get("solr", {}))
+        cfg.setdefault("freva_rest", solr_config)
+        for step in self.step_order:
+            if cfg[step]["config"].get("ansible_become_user", "") or "root":
+                return True
+        return False
 
     @property
     def _empty_ok(self) -> list[str]:
         """Define all keys that can be empty."""
         return [
             "admins",
             "conda_exec_path",
@@ -361,25 +523,21 @@
         ).get(key, None)
 
     @property
     def db_pass(self) -> str:
         """Create a password for the database."""
         if self._db_pass:
             return self._db_pass
-        punctuations = "!@$^&*()_+-;:|,.%"
-        num_chars, num_digits, num_punctuations = 20, 4, 4
-        num_chars -= num_digits + num_punctuations
+        num_chars, num_digits = 30, 8
+        num_chars -= num_digits
         characters = [
             "".join(
                 [random.choice(string.ascii_letters) for i in range(num_chars)]
             ),
             "".join([random.choice(string.digits) for i in range(num_digits)]),
-            "".join(
-                [random.choice(punctuations) for i in range(num_punctuations)]
-            ),
         ]
         str_characters = "".join(characters)
         _db_pass = "".join(random.sample(str_characters, len(str_characters)))
         while _db_pass.startswith("@"):
             # Vault treats values starting with "@" as file names.
             _db_pass = "".join(
                 random.sample(str_characters, len(str_characters))
@@ -417,37 +575,72 @@
             self.cfg[step]["config"].get("ansible_python_interpreter")
             or "/usr/bin/python3"
         )
         dump_file = self._get_files_copy(step)
         if dump_file:
             config[step]["vars"][f"{step}_dump"] = str(dump_file)
 
-    def parse_config(self) -> str:
+    def parse_config(self, steps: list[str]) -> str | None:
         """Create config files for anisble and evaluation_system.conf."""
+        versions = json.loads(
+            (Path(__file__).parent / "versions.json").read_text()
+        )
+        additional_steps = set(steps) - set(self.steps)
+        if additional_steps:
+            pprint(
+                "The following, [b]not selected[/b] steps will be auto "
+                f"updated.\n[green]{', '.join(additional_steps)}[/]"
+            )
+            time.sleep(3)
+        new_steps = set(steps + self.steps)
+        if not new_steps:
+            return None
+        self._steps = list(new_steps)
+        playbook = self.create_playbooks()
         logger.info("Parsing configurations")
         self._check_config()
         config: dict[str, dict[str, dict[str, str | int | bool]]] = {}
-        for step in set(self._config_keys):
-            config[step] = {}
+        info: dict[str, dict[str, dict[str, str | int | bool]]] = {}
+        config_keys = deepcopy(self._config_keys)
+        if "db" in config_keys:
+            config_keys.append("vault")
+        for step in set(config_keys):
+            config[step], info[step] = {}, {}
             config[step]["hosts"] = self.cfg[step]["hosts"]
-            config[step]["vars"] = {}
+            info[step]["hosts"] = self.cfg[step]["hosts"]
+            config[step]["vars"], info[step]["vars"] = {}, {}
             for key, value in self.cfg[step]["config"].items():
-                if key in ("root_passwd",):
+                if key in ("root_passwd",) or key.startswith(step):
                     new_key = key
                 else:
-                    new_key = f"{step}_{key}"
+                    new_key = f"{step.replace('-', '_')}_{key}"
                 config[step]["vars"][new_key] = value
             config[step]["vars"]["project_name"] = self.project_name
+            config[step]["vars"][f"{step.replace('-', '_')}_version"] = (
+                versions.get(step, "")
+            )
+            config[step]["vars"]["debug"] = self.local_debug
             # Add additional keys
             self._set_additional_config_values(step, config)
-        return yaml.dump(config)
-
-    @property
-    def _playbook_file(self) -> Path:
-        return Path(self._td.name) / "ansible-playbook.yml"
+        if "freva_rest" in config:
+            config["freva_rest"]["vars"]["solr_version"] = versions["solr"]
+        for step in info:
+            for key, value in config[step]["vars"].items():
+                if (
+                    f"{{{{{key}}}}}" in playbook
+                    or f"{{{{ {key} }}}}" in playbook
+                    or key == "debug"
+                ):
+                    info[step]["vars"][key] = value
+        info_str = yaml.dump(json.loads(json.dumps(info)))
+        for passwd in (self.email_password, self.master_pass):
+            if passwd:
+                info_str = info_str.replace(passwd, "***")
+        RichConsole.print(info_str, style="bold", markup=True)
+        return yaml.dump(json.loads(json.dumps(config)))
 
     @property
     def python_prefix(self) -> Path:
         """Get the path of the new conda evnironment."""
         return Path(sys.exec_prefix) / "bin" / "python3"
 
     @property
@@ -458,39 +651,39 @@
     @property
     def playbook_dir(self) -> Path:
         """The location of all playbooks."""
         return asset_dir / "playbooks"
 
     @property
     def steps(self) -> list[str]:
-        """Set all the deploment steps."""
+        """Set all the deployment steps."""
         steps = []
         for step in self._steps:
             steps.append(step)
-            if step == "db":
+            if step == "db" and "vault" not in steps:
                 steps.append("vault")
         return [s for s in self.step_order if s in steps]
 
-    def create_playbooks(self):
+    def create_playbooks(self) -> str:
         """Create the ansible playbook form all steps."""
         logger.info("Creating Ansible playbooks")
         playbook = []
+        self.current_step = "foo"
+        _ = [getattr(self, f"_prep_{step}")() for step in self.steps]
         for step in self.steps:
-            getattr(self, f"_prep_{step}")()
             playbook_file = (
                 self.playbooks.get(step)
                 or self.playbook_dir / f"{step}-server-playbook.yml"
             )
-            with Path(playbook_file).open() as f_obj:
+            with Path(playbook_file).open(encoding="utf-8") as f_obj:
                 playbook += yaml.safe_load(f_obj)
-        with self._playbook_file.open("w") as f_obj:
-            yaml.dump(playbook, f_obj)
+        return self._td.create_playbook(playbook)
 
     def create_eval_config(self) -> None:
-        """Create and dump the evaluation_systme.config."""
+        """Create and dump the evaluation_system.config."""
         logger.info("Creating evaluation_system.conf")
         keys = (
             ("core", "admins"),
             ("web", "project_website"),
             ("core", "root_dir"),
             ("core", "base_dir_location"),
             ("core", "preview_path"),
@@ -504,123 +697,233 @@
                 if line.startswith("project_name"):
                     lines[num] = f"project_name={self.project_name}\n"
                 for key, value in keys:
                     if line.startswith(value):
                         cfg = self.cfg[key]["config"].get(value, "")
                         if cfg:
                             lines[num] = f"{value}={cfg}\n"
-                for step in ("solr", "db"):
+                for step in ("freva_rest", "db"):
                     cfg = self.cfg[step]["config"].get("port", "")
                     if line.startswith(f"{step}.port"):
                         lines[num] = f"{step}.port={cfg}\n"
                     if line.startswith(f"{step}.host"):
                         lines[num] = f"{step}.host={self.cfg[step]['hosts']}\n"
+                if line.startswith("solr.host"):
+                    lines[num] = f"solr.host={self.cfg[step]['hosts']}\n"
+                if line.startswith("db.host"):
+                    lines[num] = (
+                        f"db.host={self.cfg['db']['config']['host']}\n"
+                    )
         dump_file = self._get_files_copy("core")
         if dump_file:
             with dump_file.open("w") as f_obj:
                 f_obj.write("".join(lines))
 
-    def _run(self, verbosity: int = 0, ask_pass: bool = False) -> None:
-        from ansible.executor.playbook_executor import PlaybookExecutor
-        from ansible.inventory.manager import InventoryManager
-        from ansible.parsing.dataloader import DataLoader
-        from ansible.playbook.play import Play
-        from ansible.vars.manager import VariableManager
-
-        loader = DataLoader()
-        inventory = InventoryManager(
-            loader=loader, sources=[str(self.inventory_file)]
-        )
-        variable_manager = VariableManager(loader=loader, inventory=inventory)
-        options = {
-            "verbosity": verbosity,
-            "ask_pass": ask_pass,
-            "become": True,
-            "ask_become_pass": True,
-        }
-        executor = PlaybookExecutor(
-            playbooks=[str(self._playbook_file)],
-            inventory=inventory,
-            variable_manager=variable_manager,
-            loader=loader,
-            options=options,
-        )
-        results = executor.run()
-        stats = executor._tqm._stats
-        print(stats)
+    def get_ansible_password(self, ask_pass: bool = False) -> dict[str, str]:
+        """The passwords for the ansible environments."""
+        ssh_pass_msg = "Give the [b]ssh[/b] password for remote login"
+        sudo_pass_msg = (
+            "Give the password elevating user privilege ([b]sudo[/b])"
+        )
+        if ask_pass:
+            sudo_pass_msg += ", defaults to ssh password"
+        passwords = {}
+        sudo_key = "^BECOME password.*:\\s*?$"
+        ssh_key = "^SSH password:\\s*?$"
+        passwords[sudo_key] = (
+            os.environ.get("ANSIBLE_BECOME_PASSWORD", "") or ""
+        )
+        passwords[ssh_key] = os.environ.get("ANSIBLE_SSH_PASSWORD", "") or ""
+        if ask_pass and not passwords[ssh_key]:
+            passwords[ssh_key] = Prompt.ask(
+                f"[green]{ssh_pass_msg}[/green]", password=True
+            )
+        if not passwords[sudo_key] and self.ask_become_password:
+            passwords[sudo_key] = Prompt.ask(
+                f"[green]{sudo_pass_msg}[/green]", password=True
+            )
+            if not passwords[sudo_key]:
+                passwords[sudo_key] = passwords.get(ssh_key, "")
+        return passwords
 
+    @handled_exception
     def play(
+        self, ask_pass: bool = True, verbosity: int = 0, ssh_port: int = 22
+    ) -> Runner | None:
+        """Play the ansible playbook.
+
+        Parameters
+        ----------
+        ask_pass: bool, default: True
+            Instruct Ansible to ask for the ssh password instead of using a
+            ssh key
+        verbosity: int, default: 0
+            Verbosity level, default 0
+        ssh_port: int, default: 22
+            Set the ssh port, in 99.9% of cases this should be left at port 22
+        """
+        try:
+            return self._play(
+                ask_pass=ask_pass, verbosity=verbosity, ssh_port=ssh_port
+            )
+        except KeyboardInterrupt:
+            pprint(
+                " [red][ERROR]: User interrupted execution[/]", file=sys.stderr
+            )
+            raise KeyboardInterrupt() from None
+
+    def get_steps_from_versions(
+        self,
+        envvars: dict[str, str],
+        extravars: dict[str, str | int],
+        cmdline: str,
+        passwords: dict[str, str],
+        verbosity: int,
+    ) -> list[str]:
+        """Check the versions of the different freva parts."""
+        config: dict[str, dict[str, dict[str, str | int | bool]]] = {}
+        steps = set(self.step_order) - set(self.steps)
+        if not steps or self.local_debug:
+            # The user has selected all steps anyway, nothing to do here:
+            return []
+        cfg = deepcopy(self.cfg)
+        if cfg.get("freva_rest") is None:
+            cfg["freva_rest"] = cfg.get("databrowser", cfg.get("solr", {}))
+        for step in steps:
+            config[step] = {}
+            config[step]["hosts"] = cfg[step]["hosts"]
+            if "ansible_become_user" not in cfg[step]["config"]:
+                become_user = "root"
+            else:
+                become_user = cfg[step]["config"]["ansible_become_user"]
+            config[step]["vars"] = {
+                f"{step}_ansible_become_user": become_user,
+                "asset_dir": str(asset_dir),
+                f"{step}_ansible_user": cfg[step]["config"].get(
+                    "ansible_user", getuser()
+                ),
+            }
+        config.setdefault("core", {})
+        config["core"].setdefault("vars", {})
+        config["core"]["vars"]["core_install_dir"] = cfg["core"]["config"][
+            "install_dir"
+        ]
+        stdout = sys.stdout
+        buffer = StringIO()
+        sig_handler = signal.getsignal(signal.SIGINT)
+        text = "Getting versions of micro-services ..."
+        spinner = Spinner("weather", text=text)
+        status_text = {
+            "successful": " [green]ok[/green]",
+            "canceled": " [yellow]canceled[/yellow]",
+            "failed": " [red]failed[/red]",
+        }
+        with Live(spinner, refresh_per_second=3, console=Console(stderr=True)):
+            extravars["forks"] = 4
+            try:
+                sys.stdout = buffer
+                sys.stdout.write("\n")
+                event = run(
+                    playbook=str(asset_dir / "playbooks" / "versions.yaml"),
+                    inventory=config,
+                    envvars=envvars,
+                    passwords=passwords,
+                    extravars=extravars,
+                    cmdline=cmdline,
+                    verbosity=verbosity,
+                    forks=4,
+                )
+            finally:
+                sys.stdout = stdout
+                signal.signal(signal.SIGINT, sig_handler)
+            spinner.update(
+                text=text + status_text.get(event.status, " [red]failed[/red]")
+            )
+
+        if event.status not in ["successful", "canceled"]:
+            raise DeploymentError(buffer.getvalue()) from None
+        if event.status == "canceled":
+            raise KeyboardInterrupt() from None
+        if verbosity > 0:
+            print(buffer.getvalue())
+        versions = {}
+        for res in event.events:
+            msg = res.get("event_data", {}).get("res", {}).get("msg")
+            title = res.get("event_data", {}).get("task", "").lower()
+            if msg is not None and title.startswith("display"):
+                service = res.get("event_data", {}).get("task", "").split()[1]
+                versions[service] = msg.strip()
+        additional_steps = get_steps_from_versions(versions)
+        return additional_steps
+
+    def _play(
         self,
-        server_map: str | None = None,
         ask_pass: bool = True,
         verbosity: int = 0,
-    ) -> None:
+        ssh_port: int = 22,
+    ) -> Runner | None:
         """Play the ansible playbook.
 
         Parameters
         ----------
-        server_map: str, default: None
-            Hostname running the service that keeps track of the server
-            infrastructure, if None given (default) no new deployed services
-            are added.
         ask_pass: bool, default: True
-            Instruct Ansible to ask for the ssh passord instead of using a
+            Instruct Ansible to ask for the ssh password instead of using a
             ssh key
         verbosity: int, default: 0
             Verbosity level, default 0
+        ssh_port: int, default: 22
+            Set the ssh port, in 99.9% of cases this should be left at port 22
         """
-        self.create_playbooks()
-        inventory = self.parse_config()
-        self.create_eval_config()
-        with self.inventory_file.open("w") as f_obj:
-            f_obj.write(inventory)
-        inventory_str = inventory
-        for passwd in (self.email_password, self.master_pass):
-            if passwd:
-                inventory_str = inventory_str.replace(
-                    passwd, "*" * len(passwd)
-                )
-        RichConsole.print(inventory, style="bold", markup=True)
-        logger.info("Playing the playbooks with ansible")
-        RichConsole.print(
-            "[b]Note:[/] The [blue]BECOME[/] password refers to the "
-            "[blue]sudo[/] password",
-            markup=True,
-        )
-        # try:
-        #    self._run(ask_pass=ask_pass, verbosity=verbosity)
-        # except KeyboardInterrupt:
-        #    pass
-        # return
-        v_string = sign(verbosity) * "-" + verbosity * "v"
-        cmd = (
-            f"ansible-playbook {v_string} -i {self.inventory_file} "
-            f"{self._playbook_file} --ask-become-pass"
-        )
+        envvars: dict[str, str] = {
+            "ANSIBLE_STDOUT_CALLBACK": "yaml",
+            "ANSIBLE_CONFIG": self._td.ansible_config_file,
+        }
+        extravars: dict[str, str | int] = {
+            "ansible_port": ssh_port,
+            "ansible_ssh_args": "-o ForwardX11=no",
+        }
+        if self.local_debug:
+            extravars["ansible_connection"] = "local"
+
+        cmdline = "--ask-become"
         if ask_pass:
-            cmd += " --ask-pass"
-        env = os.environ.copy()
-        env["PATH"] += f":{AssetDir.get_dirs(user=True, key='scripts')}"
+            cmdline += " --ask-pass"
+        passwords = self.get_ansible_password(ask_pass)
+        steps = self.get_steps_from_versions(
+            envvars.copy(),
+            extravars.copy(),
+            cmdline,
+            passwords.copy(),
+            verbosity,
+        )
+        inventory = self.parse_config(steps)
+        if inventory is None:
+            logger.info("Services up to date, nothing to do!")
+            return None
+        self.create_eval_config()
+        logger.debug(inventory)
+        logger.info(
+            "Playing the playbooks for %s with ansible", ", ".join(self.steps)
+        )
+        logger.debug(self.playbooks)
+        time.sleep(3)
+        sig_handler = signal.getsignal(signal.SIGINT)
         try:
-            _ = run(
-                shlex.split(cmd),
-                env=env,
-                cwd=str(asset_dir),
-                check=True,
+            result = run(
+                private_data_dir=str(self._td.parent_dir),
+                playbook=str(self._td.playbook_file),
+                inventory=inventory,
+                envvars=envvars,
+                passwords=passwords,
+                extravars=extravars,
+                cmdline=cmdline,
+                verbosity=verbosity,
             )
-        except KeyboardInterrupt:
-            pass
-        if server_map:
-            self.upload_server_info(server_map, inventory)
-
-    def upload_server_info(self, server_map: str, inventory: str) -> None:
-        """Upload information on server information to shared nextcloud."""
-        deployment_setup: dict[str, dict[str, str]] = {}
-        for step, info in yaml.safe_load(inventory).items():
-            ansible_step = dict(
-                python_path=info["vars"][f"{step}_ansible_python_interpreter"]
-            )
-            ansible_step["hosts"] = info["hosts"]
-            deployment_setup[step] = ansible_step
-            if step == "web":
-                deployment_setup["redis"] = ansible_step
-        upload_server_map(server_map, self.project_name, deployment_setup)
+        finally:
+            signal.signal(signal.SIGINT, sig_handler)
+        if result.status in ("timeout", "failed"):
+            raise DeploymentError(
+                f"Deployment not successful: {result.status}"
+            )
+        elif result.status == "canceled":
+            raise KeyboardInterrupt() from None
+        return result
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Call the freva tui."""
+
 from __future__ import annotations
 
 import argparse
 
 from freva_deployment import __version__
 from freva_deployment.deploy import DeployFactory
-from freva_deployment.utils import RichConsole, set_log_level
+from freva_deployment.error import DeploymentError
+from freva_deployment.logger import set_log_level
+from freva_deployment.utils import RichConsole
+from freva_deployment.versions import VersionAction, display_versions
 
 from .main_window import MainApp
 
 
 def parse_args() -> int:
     """Construct command line argument parser."""
     app = argparse.ArgumentParser(
@@ -19,16 +23,18 @@
     )
     app.add_argument(
         "-v", "--verbose", action="count", help="Verbosity level", default=0
     )
     app.add_argument(
         "-V",
         "--version",
-        action="version",
-        version="%(prog)s {version}".format(version=__version__),
+        action=VersionAction,
+        version="[b][red]%(prog)s[/red] {version}[/b]{services}".format(
+            version=__version__, services=display_versions()
+        ),
     )
     parser = app.parse_args()
     return parser.verbose
 
 
 def tui() -> None:
     """Create and run Text User Interface (TUI) for deployment."""
@@ -45,13 +51,18 @@
             )
         except AttributeError:
             pass
         return
     setup = main_app.setup
     main_app.thread_stop.set()
     if setup:
-        server_map = setup.pop("server_map")
         ask_pass = setup.pop("ask_pass")
         steps = ", ".join(setup["steps"])
+        ssh_port = setup.pop("ssh_port")
         RichConsole.print(f"Playing steps: [i]{steps}[/] with ansible")
         with DeployFactory(**setup) as DF:
-            DF.play(server_map, ask_pass, verbosity)
+            try:
+                DF.play(ask_pass, verbosity, ssh_port=ssh_port)
+            except KeyboardInterrupt:
+                raise SystemExit(130)
+            except DeploymentError:
+                raise SystemExit(1)
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,14 @@
             except AttributeError:
                 value = obj.value
             if isinstance(value, str):
                 if not value and self.use.value and mandatory and notify:
                     msg = f"MISSING ENTRY FOR {self.step}: {obj.name}"
                     npyscreen.notify_confirm(msg, title="ERROR")
                     return None
-                elif not value and not mandatory:
-                    continue
             config[key] = value
         cfg = dict(hosts=config.pop("hosts"))
         cfg["config"] = config
         for key, value in cfg["config"].items():
             if key in self.list_keys:
                 cfg["config"][key] = value.split(",")
         return cfg
@@ -196,14 +194,16 @@
 
     def change_forms(self, *args, reverse=False, **keywords) -> None:
         """Cycle between the deployment config forms."""
         for step in self.parentApp._steps_lookup.keys():
             if self.name.lower().startswith(step):
                 name = step
                 break
+            elif "rest" in self.name.lower():
+                name = "freva_rest"
             elif self.name.lower().startswith("database"):
                 name = "db"
                 break
         keys = self.parentApp._steps_lookup.keys()
         steps = list(self.parentApp._steps_lookup.values())
         if reverse:
             change_to = dict(zip(keys, [steps[-1]] + steps[:-1]))
@@ -235,17 +235,17 @@
         self.parentApp.DEFAULT_THEME = theme
         self.create()
         self.display()
         self.display()
 
     def create(self) -> None:
         """Setup the form."""
-        self.how_exited_handers[
-            npyscreen.wgwidget.EXITED_ESCAPE
-        ] = self.parentApp.exit_application
+        self.how_exited_handers[npyscreen.wgwidget.EXITED_ESCAPE] = (
+            self.parentApp.exit_application
+        )
         self.add_handlers({"^O": self.parentApp.load_dialog})
         self.add_handlers({"^S": self.parentApp.save_dialog})
         self.add_handlers({"^K": self.previews_form})
         self.add_handlers({"^L": self.change_forms})
         self.add_handlers({"^R": self.run_deployment})
         self.add_handlers({"^E": self.parentApp.exit_application})
         # The menus are created here.
@@ -263,15 +263,21 @@
             ]
         )
         self.submenu.addItemsFromList(
             [
                 ("Core Deployment", self._change_form, "c", "c", ("MAIN",)),
                 ("Web Deployment", self._change_form, "w", "w", ("SECOND",)),
                 ("DB Deployment", self._change_form, "d", "d", ("THIRD",)),
-                ("Solr Deployment", self._change_form, "s", "s", ("FOURTH",)),
+                (
+                    "Freva-Rest Deployment",
+                    self._change_form,
+                    "s",
+                    "s",
+                    ("FOURTH",),
+                ),
                 ("Run Deployment", self.run_deployment, "^R"),
             ]
         )
         self.use = self.add(
             npyscreen.CheckBox,
             max_height=2,
             value=self.step in self.parentApp._steps,
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,48 +75,44 @@
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=f"{self.num}Anaconda installation dir. for core:",
                     value=cfg.get("install_dir", ""),
                 ),
                 True,
             ),
-            install=(
-                self.add_widget_intelligent(
-                    npyscreen.RoundCheckBox,
-                    max_height=2,
-                    value=cfg.get("install", True),
-                    editable=True,
-                    name=(f"{self.num}Install a new Freva anaconda environment?"),
-                    scroll_exit=True,
-                ),
-                True,
-            ),
             root_dir=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Directory where project configuration is stored "
-                        "(defaults to `anaconda installation dir.` in #3):"
+                        f"(defaults to `anaconda installation dir.` in #{self._num-1}):"
                     ),
                     value=cfg.get("root_dir", ""),
                 ),
                 False,
             ),
             base_dir_location=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
-                    name=f"{self.num}User data directory:",
+                    name=(
+                        f"{self.num}User data directory, defaults to "
+                        f"project config. dir given in #{self._num-1}."
+                    ),
                     value=cfg.get("base_dir_location", ""),
                 ),
                 False,
             ),
             preview_path=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
-                    name=f"{self.num}Plugin output dir for the web UI (preview path):",
+                    name=(
+                        f"{self.num}Plugin output dir for the web UI "
+                        "(preview path), defaults to user data dir"
+                        f" given in #{self._num - 1}."
+                    ),
                     value=cfg.get("preview_path", ""),
                 ),
                 False,
             ),
             scheduler_system=(
                 self.add_widget_intelligent(
                     npyscreen.TitleCombo,
@@ -161,26 +157,14 @@
                         f"{self.num}Become (sudo) user name to change to on "
                         "remote machine, leave blank if not needed:"
                     ),
                     value=cfg.get("ansible_become_user", ""),
                 ),
                 False,
             ),
-            conda_exec_path=(
-                self.add_widget_intelligent(
-                    npyscreen.TitleText,
-                    name=(
-                        f"{self.num}Path to any existing conda installation - "
-                        "leave blank to "
-                        "install a temporary conda distribution:"
-                    ),
-                    value=cfg.get("conda_exec_path", ""),
-                ),
-                False,
-            ),
             arch=(
                 self.add_widget_intelligent(
                     npyscreen.TitleCombo,
                     name=(
                         f"{self.num}Set the target architecture of the system where "
                         "the backend will be installed:"
                     ),
@@ -227,15 +211,15 @@
         )
 
 
 class WebScreen(BaseForm):
     """Form for the web deployment configuration."""
 
     step: str = "web"
-    certificates: list[str] = ["public", "private", "chain"]
+    certificates: list[str] = ["public", "private"]
     """The type of certificate files this step needs."""
 
     def get_index(self, choices: list[str], key: str):
         """Get the key value pair for a combo box"""
         for nn, choice in enumerate(choices):
             if choice == key:
                 return nn
@@ -245,24 +229,42 @@
         """Add widgets to the screen."""
         self.list_keys = "imprint", "scheduler_host", "allowed_hosts"
         cfg = self.get_config(self.step)
         for key in self.list_keys:
             if key in cfg and isinstance(cfg[key], str):
                 value = cast(str, cfg[key])
                 cfg[key] = [v.strip() for v in value.split(",") if v.strip()]
-                logger.warning(key, cfg[key])
+        availalbe_ldab_models = [
+            "MiklipUserInformation",
+            "UCARUserInformation",
+            "DWDUserInformation",
+            "FUUserInformation",
+        ]
+        current_ldab_model = get_index(
+            availalbe_ldab_models,
+            cast(str, cfg.get("ldap_model", "MiklipUserInformation")),
+            0,
+        )
         self.input_fields: dict[str, tuple[npyscreen.TitleText, bool]] = dict(
             hosts=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=f"{self.num}Server Name(s) the web service is deployed on:",
                     value=self.get_host("web"),
                 ),
                 True,
             ),
+            data_path=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleText,
+                    name=f"{self.num}Parent directory for any permanent data:",
+                    value=cast(str, cfg.get("data_path", "/opt/freva")),
+                ),
+                True,
+            ),
             project_website=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=f"{self.num}Url of the Freva home page:",
                     value=cfg.get("project_website", ""),
                 ),
                 True,
@@ -536,17 +538,18 @@
                     ),
                     values=["posix", "nested"],
                 ),
                 True,
             ),
             ldap_model=(
                 self.add_widget_intelligent(
-                    npyscreen.TitleText,
+                    npyscreen.TitleCombo,
                     name=(f"{self.num}Ldap tools class to be used for authentication."),
-                    value=cfg.get("ldap_model", "MiklipUserInformation"),
+                    value=current_ldab_model,
+                    values=availalbe_ldab_models,
                 ),
                 True,
             ),
             web_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
@@ -558,15 +561,15 @@
                 False,
             ),
             ansible_become_user=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(
                         f"{self.num}Become (sudo) user name to change to on "
-                        "remote machine, leave blank if not needed:"
+                        "remote machine, leave blank for root less deployment:"
                     ),
                     value=cfg.get("ansible_become_user", "root"),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
@@ -643,42 +646,39 @@
                     npyscreen.TitleCombo,
                     name=f"{self.num}Database Port:",
                     value=port_idx,
                     values=db_ports,
                 ),
                 True,
             ),
-            db_playbook=(
+            data_path=(
                 self.add_widget_intelligent(
-                    npyscreen.TitleFilename,
-                    name=(
-                        f"{self.num}Set the path to the db playbook used for"
-                        " setting up the system."
-                    ),
-                    value=cfg.get("db_playbook", ""),
+                    npyscreen.TitleText,
+                    name=(f"{self.num}Parent directory for any permanent data:"),
+                    value=cast(str, cfg.get("data_path", "/opt/freva")),
                 ),
-                False,
+                True,
             ),
-            vault_playbook=(
+            db_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
-                        f"{self.num}Set the path to the vault playbook used for"
+                        f"{self.num}Set the path to the db playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get("vault_playbook", ""),
+                    value=cfg.get("db_playbook", ""),
                 ),
                 False,
             ),
             ansible_become_user=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(
                         f"{self.num}Become (sudo) user name to change to on "
-                        "remote machine, leave blank if not needed:"
+                        "remote machine, leave blank for root less deployment:"
                     ),
                     value=cfg.get("ansible_become_user", "root"),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
@@ -695,82 +695,96 @@
                     value=cfg.get("ansible_user", getuser()),
                 ),
                 False,
             ),
         )
 
 
-class SolrScreen(BaseForm):
-    """Form for the solr deployment configuration."""
+class FrevaRestScreen(BaseForm):
+    """Form for the freva-rest deployment configuration."""
 
-    step: str = "solr"
+    step: str = "freva_rest"
 
     def _add_widgets(self) -> None:
         """Add widgets to the screen."""
         self.list_keys: list[str] = []
         cfg = self.get_config(self.step)
-        solr_ports: list[int] = list(range(8980, 9000))
-        port_idx = get_index(
-            [str(p) for p in solr_ports], str(cfg.get("port", 8983)), 3
+        freva_rest_ports: list[int] = list(range(7770, 7780))
+        solr_mem_values = [f"{i}g" for i in range(1, 10)]
+        solr_mem_select = get_index(
+            solr_mem_values, cast(str, cfg.get("solr_mem", "4g")), 3
+        )
+        freva_rest_port_idx = get_index(
+            [str(p) for p in freva_rest_ports],
+            str(cfg.get("freva_rest_port", 7777)),
+            7,
         )
         self.input_fields: dict[str, tuple[npyscreen.TitleText, bool]] = dict(
             hosts=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
-                    name=f"{self.num}Server Name(s) where the solr service is deployed:",
-                    value=self.get_host("solr"),
+                    name=f"{self.num}Server Name(s) where the freva-rest service is deployed:",
+                    value=self.get_host("freva_rest"),
                 ),
                 True,
             ),
             wipe=(
                 self.add_widget_intelligent(
                     npyscreen.RoundCheckBox,
                     max_height=2,
                     value=cfg.get("wipe", False),
                     editable=True,
                     name=(f"{self.num}Delete existing data?"),
                     scroll_exit=True,
                 ),
                 True,
             ),
-            mem=(
+            solr_mem=(
                 self.add_widget_intelligent(
                     npyscreen.TitleCombo,
-                    name=f"{self.num}Virtual memory (in GB) for the solr server:",
-                    value=3,
-                    values=[f"{i}g" for i in range(1, 10)],
+                    name=f"{self.num}Virtual memory (in GB) for the search engine service:",
+                    value=solr_mem_select,
+                    values=solr_mem_values,
                 ),
                 True,
             ),
-            port=(
+            freva_rest_port=(
                 self.add_widget_intelligent(
                     npyscreen.TitleCombo,
-                    name=f"{self.num}Solr port:",
-                    value=port_idx,
-                    values=solr_ports,
+                    name=f"{self.num}Freva-rest API port:",
+                    value=freva_rest_port_idx,
+                    values=freva_rest_ports,
+                ),
+                True,
+            ),
+            data_path=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleText,
+                    name=f"{self.num}Parent directory for any permanent data:",
+                    value=cast(str, cfg.get("data_path", "/opt/freva")),
                 ),
                 True,
             ),
-            solr_playbook=(
+            freva_rest_playbook=(
                 self.add_widget_intelligent(
                     npyscreen.TitleFilename,
                     name=(
                         f"{self.num}Set the path to the playbook used for"
                         " setting up the system."
                     ),
-                    value=cfg.get("solr_playbook", ""),
+                    value=cfg.get("freva_rest_playbook", ""),
                 ),
                 False,
             ),
             ansible_become_user=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(
                         f"{self.num}Become (sudo) user name to change to on "
-                        "remote machine, leave blank if not needed:"
+                        "remote machine, leave blank for root less deployment:"
                     ),
                     value=cfg.get("ansible_become_user", "root"),
                 ),
                 False,
             ),
             ansible_python_interpreter=(
                 self.add_widget_intelligent(
@@ -805,68 +819,61 @@
     def on_ok(self) -> None:
         """Define what happens once the `ok` for applying the deployment is hit."""
 
         self.parentApp.thread_stop.set()
         if not self.project_name.value:
             npyscreen.notify_confirm("You have to set a project name", title="ERROR")
             return
-        if not self.server_map.value:
-            value = npyscreen.notify_yes_no(
-                "If you don't set a map server value you wont be able "
-                "to start|stop the services. Continue anyway?",
-                title="WARNING",
-            )
-            if not value:
-                return
         missing_form: None | str = self.parentApp.check_missing_config()
         if missing_form:
             self.parentApp.change_form(missing_form)
             return
-        public_keyfile = self.public_keyfile.value or self.chain_keyfile.value
+        public_keyfile = self.public_keyfile.value
         cert_files = dict(
             public=public_keyfile or "",
             private=self.private_keyfile.value or "",
         )
         save_file = Path(
             self.parentApp.get_save_file(self.inventory_file.value or None)
         )
+        if isinstance(self.gen_keys.value, list):
+            gen_keys = bool(self.gen_keys.value[0])
+        else:
+            gen_keys = bool(self.gen_keys.value)
         for key_type, keyfile in cert_files.items():
             key_file = Path(get_current_file_dir(save_file.parent, str(keyfile)))
             for step, deploy_form in self.parentApp._forms.items():
                 if not keyfile or not Path(key_file).is_file():
                     if (
                         key_type in deploy_form.certificates
                         and step in self.parentApp.steps
+                        and gen_keys is False
                     ):
                         if keyfile:
                             msg = (
                                 f"{key_type} certificate file `{key_file}` must exist."
                             )
                         else:
                             msg = f"You must give a {key_type} certificate file."
                         npyscreen.notify_confirm(msg, title="ERROR")
                         return
-
-        cert_files["chain"] = self.chain_keyfile.value or ""
-        if not cert_files["chain"]:
-            value = npyscreen.notify_yes_no(
-                "It is advised to create a chained certificate file. "
-                "This enhances the web ui security. Continue anyway?",
-                title="WARNING",
-            )
-            if not value:
-                return
         _ = self.parentApp.save_config_to_file(
             save_file=save_file, write_toml_file=True
         )
+        try:
+            ssh_port = int(self.ssh_port.value)
+        except ValueError:
+            ssh_port = 22
         self.parentApp.setup = {
-            "server_map": self.server_map.value,
             "steps": list(set(self.parentApp.steps)),
             "ask_pass": bool(self.use_ssh_pw.value),
             "config_file": str(save_file) or None,
+            "ssh_port": ssh_port,
+            "local_debug": bool(self.local_debug.value),
+            "gen_keys": bool(gen_keys),
         }
         self.parentApp.exit_application(
             save_file=save_file, msg="Do you want to continue?"
         )
 
     def on_cancel(self) -> None:
         """Define what happens after the the cancel button is hit."""
@@ -877,57 +884,64 @@
                 # Tell the MyTestApp object to change forms.
                 self.parentApp.change_form(form_name)
                 return
         self.parentApp.change_form("MAIN")
 
     def create(self) -> None:
         """Custom definitions executed when the from gets created."""
-        self.how_exited_handers[
-            npyscreen.wgwidget.EXITED_ESCAPE
-        ] = self.parentApp.exit_application
+        self.how_exited_handers[npyscreen.wgwidget.EXITED_ESCAPE] = (
+            self.parentApp.exit_application
+        )
         self._add_widgets()
 
     def _add_widgets(self) -> None:
         """Add the widgets to the form."""
 
         project_name = self.parentApp.config.get(
             "project_name", self.parentApp._read_cache("project_name", "")
         )
-        ssh_pw = self.parentApp._read_cache("ssh_pw", True)
         self.project_name = self.add_widget_intelligent(
             npyscreen.TitleText,
             name=f"{self.num}Set the name of the project",
             value=project_name,
         )
         self.inventory_file = self.add_widget_intelligent(
             npyscreen.TitleFilename,
             name=f"{self.num}Save config as",
             value=str(self.parentApp.save_file or ""),
         )
-        self.server_map = self.add_widget_intelligent(
-            npyscreen.TitleText,
-            name=(f"{self.num}Hostname of the service mapping the freva server arch."),
-            value=self.parentApp._read_cache("server_map", ""),
-        )
         self.public_keyfile = self.add_widget_intelligent(
             npyscreen.TitleFilename,
             name=f"{self.num}Select a public certificate file; needed for steps web, core, db",
             value=self.parentApp.read_cert_file("public_keyfile"),
         )
         self.private_keyfile = self.add_widget_intelligent(
             npyscreen.TitleFilename,
             name=f"{self.num}Select a private certificate file; needed for steps web",
             value=self.parentApp.read_cert_file("private_keyfile"),
         )
-        self.chain_keyfile = self.add_widget_intelligent(
-            npyscreen.TitleFilename,
-            name=f"{self.num}Select a chain certificate file; needed for steps web",
-            value=self.parentApp.read_cert_file("chain_keyfile"),
+        self.gen_keys = self.add_widget_intelligent(
+            npyscreen.RoundCheckBox,
+            max_height=2,
+            value=self.parentApp._read_cache("gen_keys", False),
+            name=f"{self.num}Generate a pair web certificates, debugging",
         )
         self.use_ssh_pw = self.add_widget_intelligent(
             npyscreen.RoundCheckBox,
             max_height=2,
-            value=ssh_pw,
             editable=True,
+            value=self.parentApp._read_cache("ssh_pw", False),
             name=f"{self.num}Use password for ssh connection",
             scroll_exit=True,
         )
+        self.ssh_port = self.add_widget_intelligent(
+            npyscreen.TitleText,
+            name=f"{self.num}If you need to, you can change the ssh port here",
+            value=str(self.parentApp._read_cache("ssh_port", 22)),
+        )
+        self.local_debug = self.add_widget_intelligent(
+            npyscreen.RoundCheckBox,
+            max_height=2,
+            value=self.parentApp._read_cache("local_debug", False),
+            editable=True,
+            name=f"{self.num}Deploy services on the local machine, debug",
+        )
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2405.0.0/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """The Freva deployment Text User Interface (TUI) helps to configure a
 deployment setup for a new instance of freva."""
+
 from __future__ import annotations
 
 import json
 import threading
 import time
 from pathlib import Path
 from typing import Any, Dict, List, cast
 
 import appdirs
 import npyscreen
 import tomlkit
 
-from freva_deployment.utils import asset_dir, config_dir
+from freva_deployment.utils import asset_dir, config_dir, load_config
 
 from .base import BaseForm, VarForm, selectFile
-from .deploy_forms import CoreScreen, DBScreen, RunForm, SolrScreen, WebScreen
+from .deploy_forms import (
+    CoreScreen,
+    DBScreen,
+    FrevaRestScreen,
+    RunForm,
+    WebScreen,
+)
 
 
 class MainApp(npyscreen.NPSAppManaged):
     config: dict[str, Any] = dict()
 
     @property
     def steps(self) -> list[str]:
@@ -34,25 +41,32 @@
         """When Application starts, set up the Forms that will be used."""
         npyscreen.setTheme(npyscreen.Themes.ElegantTheme)
         self.cache_dir.mkdir(exist_ok=True, parents=True)
         self.setup: dict[str, Any] = {}
         self._forms: dict[str, BaseForm] = {}
         self.current_form = "core"
         self.init()
+        self._auto_save_active = False
         self.thread_stop = threading.Event()
         self.start_auto_save()
 
     def init(self) -> None:
         self._steps_lookup = {
             "core": "MAIN",
             "web": "SECOND",
-            "solr": "FOURTH",
+            "freva_rest": "FOURTH",
             "db": "THIRD",
         }
+        save_file = cast(str, self._read_cache("save_file", ""))
         self.config = cast(Dict[str, Any], self._read_cache("config", {}))
+        if save_file and Path(save_file).is_file():
+            try:
+                self.config = load_config(save_file)
+            except Exception:
+                pass
         for step in self._steps_lookup.keys():
             self.config.setdefault(step, {"hosts": "", "config": {}})
         self._add_froms()
 
     def reset(self) -> None:
         npyscreen.blank_terminal()
         self.init()
@@ -68,23 +82,27 @@
         self._forms["core"] = self.addForm(
             "MAIN",
             CoreScreen,
             name="Core deployment",
         )
         self._forms["web"] = self.addForm("SECOND", WebScreen, name="Web deployment")
         self._forms["db"] = self.addForm("THIRD", DBScreen, name="Database deployment")
-        self._forms["solr"] = self.addForm("FOURTH", SolrScreen, name="Solr deployment")
+        self._forms["freva_rest"] = self.addForm(
+            "FOURTH", FrevaRestScreen, name="Freva Rest deployment"
+        )
         self._setup_form = self.addForm("SETUP", RunForm, name="Apply the Deployment")
 
     def exit_application(self, *args, **kwargs) -> None:
         value = npyscreen.notify_ok_cancel(
             kwargs.get("msg", "Exit Application?"), title=""
         )
         if value is True:
             self.thread_stop.set()
+            while self._auto_save_active is True:
+                time.sleep(0.1)
             self.setNextForm(None)
             self.save_config_to_file(save_file=kwargs.get("save_file"))
             self.editing = False
             self.switchFormNow()
 
     def change_form(self, name: str) -> None:
         # Switch forms.  NB. Do *not* call the .edit() method directly (which
@@ -101,49 +119,49 @@
         for step, form_obj in self._forms.items():
             cfg = form_obj.check_config(notify=stop_at_missing)
             if cfg is None and stop_at_missing:
                 return self._steps_lookup[step]
             try:
                 self.config[step] = cfg
             except Exception as error:
-                raise ValueError((step, cfg))
-                raise error
+                raise ValueError((step, cfg)) from None
         return None
 
     def _auto_save(self) -> None:
         """Auto save the current configuration."""
+        self._auto_save_active = True
         while not self.thread_stop.is_set():
             time.sleep(0.5)
             if self.thread_stop.is_set():
                 break
             try:
                 self.check_missing_config(stop_at_missing=False)
                 self.save_config_to_file()
             except Exception:
                 pass
+        self._auto_save_active = False
 
     def save_dialog(self, *args, **kwargs) -> None:
         """Create a dialoge that allows for saving the config file."""
 
         the_selected_file = selectFile(
             select_dir=False, must_exist=False, file_extentions=[".toml"]
         )
         if the_selected_file:
             the_selected_file = Path(the_selected_file).with_suffix(".toml")
             the_selected_file = str(the_selected_file.expanduser().absolute())
             self.check_missing_config(stop_at_missing=False)
             self._setup_form.inventory_file.value = the_selected_file
-            self.save_config_to_file(write_toml_file=True)
+            self.save_config_to_file(save_file=the_selected_file, write_toml_file=True)
 
     def _update_config(self, config_file: Path | str) -> None:
         """Update the main window after a new configuration has been loaded."""
 
         try:
-            with open(config_file) as f:
-                self.config = tomlkit.load(f)
+            self.config = load_config(config_file)
         except Exception:
             return
         self.resetHistory()
         self.editing = True
         self.switchFormNow()
         self._add_froms()
         self._setup_form.inventory_file.value = config_file
@@ -163,60 +181,68 @@
         try:
             return self._save_config_to_file(**kwargs)
         except Exception as error:
             npyscreen.notify_confirm(
                 title="Error",
                 message=f"Couldn't save config:\n{error}",
             )
-        return None
+            raise
 
     def get_save_file(self, save_file: Path | None = None) -> str:
         """Get the name of the file where the config should be stored to."""
-        cache_file = self.cache_dir / ".temp_file.toml"
+        cache_file = self.cache_dir / "temp_file.toml"
         if save_file:
             save_file = Path(save_file).expanduser().absolute()
         return str(save_file or cache_file)
 
     def _save_config_to_file(
         self,
         write_toml_file: bool = False,
         save_file: Path | None = None,
     ) -> Path | None:
         cert_files = dict(
             public_keyfile=self._setup_form.public_keyfile.value or "",
             private_keyfile=self._setup_form.private_keyfile.value or "",
-            chain_keyfile=self._setup_form.chain_keyfile.value or "",
         )
         for key, value in cert_files.items():
             if value and "cfd" not in value.lower():
                 cert_files[key] = str(Path(value).expanduser().absolute())
         project_name = self._setup_form.project_name.value
-        server_map = self._setup_form.server_map.value
-        ssh_pw = self._setup_form.use_ssh_pw.value
-        if isinstance(ssh_pw, list):
-            ssh_pw = bool(ssh_pw[0])
+        bools = {}
+        for key, value in (
+            ("ssh_pw", self._setup_form.use_ssh_pw.value),
+            ("local_debug", self._setup_form.local_debug.value),
+            ("gen_keys", self._setup_form.gen_keys.value),
+        ):
+            if isinstance(value, list):
+                bools[key] = bool(value[0])
+            else:
+                bools[key] = bool(value)
+        try:
+            ssh_port = int(self._setup_form.ssh_port.value)
+        except ValueError:
+            ssh_port = 22
         self.config["certificates"] = cert_files
         self.config["project_name"] = project_name or ""
         config = {
-            "save_file": self.get_save_file(save_file),
-            "steps": self.steps,
-            "ssh_pw": ssh_pw,
-            "server_map": server_map,
-            "config": self.config,
+            **bools,
+            **{
+                "save_file": str(save_file or ""),
+                "steps": self.steps,
+                "ssh_port": ssh_port,
+                "config": self.config,
+            },
         }
         with open(self.cache_dir / "freva_deployment.json", "w") as f:
             json.dump({k: v for (k, v) in config.items()}, f, indent=3)
         if write_toml_file is False:
             return None
+
         try:
-            with open(self.save_file) as f:
-                config_tmpl = cast(Dict[str, Any], tomlkit.load(f))
-        except FileNotFoundError:
-            with open(asset_dir / "config" / "inventory.toml") as f:
-                config_tmpl = cast(Dict[str, Any], tomlkit.load(f))
+            config_tmpl = load_config(asset_dir / "config" / "inventory.toml")
         except Exception:
             config_tmpl = self.config
         config_tmpl["certificates"] = cert_files
         config_tmpl["project_name"] = project_name
         for step, settings in self.config.items():
             if step in ("certificates", "project_name"):
                 continue
@@ -242,15 +268,18 @@
                 return json.load(f).get(key, default)
         except (FileNotFoundError, json.decoder.JSONDecodeError):
             return default
 
     @property
     def _steps(self) -> list[str]:
         """Read the deployment-steps from the cache."""
-        return cast(List[str], self._read_cache("steps", ["core", "web", "db", "solr"]))
+        return cast(
+            List[str],
+            self._read_cache("steps", ["core", "web", "db", "freva_rest"]),
+        )
 
     def read_cert_file(self, key: str) -> str:
         """Read the certificate file from the cache."""
         cert_file = cast(str, self.config.get("certificates", {}).get(key, ""))
         if cert_file:
             return cert_file
         return cast(str, self._read_cache(key, ""))
```

### Comparing `freva_deployment-2309.0.1/src/freva_deployment/utils.py` & `freva_deployment-2405.0.0/src/freva_deployment/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Collection of utils for deployment."""
+
 from __future__ import annotations
 
 import hashlib
-import json
-import logging
 import os
 import re
 import shutil
 import sys
 import sysconfig
 from pathlib import Path
-from typing import Any, NamedTuple, cast
+from typing import Any, Dict, MutableMapping, NamedTuple, Optional, Union, cast
 
 import appdirs
 import requests
-import toml
+import tomlkit
 from rich.console import Console
 from rich.prompt import Prompt
 
-logging.basicConfig(
-    format="%(name)s - %(levelname)s - %(message)s", level=logging.INFO
-)
-logger = logging.getLogger("freva-deployment")
+from .error import ConfigurationError
+from .logger import logger
 
 RichConsole = Console(markup=True, force_terminal=True)
 
 config_text = """
 ### This is the global config file for the freva deployment
 [general]
 [variables]
@@ -39,33 +36,30 @@
 # USER_GROUP = "myusergroup"
 """
 
 password_prompt = (
     "[green]Choose[/] a [b]master password[/], this password will be used to:\n"
     "- create the [magenta]mysql root[/] password\n"
     "- set the [magenta]django admin[/] web password\n"
+    "- set the [magenta]mongo db[/] user password\n"
     "[b]Note:[/] Ideally this password can be shared amongst other [i]admins[/].\n"
     "[b][green]choose[/] master password[/]"
 )
 
 ServiceInfo = NamedTuple(
     "ServiceInfo", [("name", str), ("python_path", str), ("hosts", str)]
 )
 
 
 class AssetDir:
     this_module = "freva_deployment"
 
     def __init__(self):
-        self._user_asset_dir = (
-            Path(appdirs.user_data_dir()) / "freva" / "deployment"
-        )
-        self._user_config_dir = (
-            Path(appdirs.user_config_dir()) / "freva" / "deployment"
-        )
+        self._user_asset_dir = Path(appdirs.user_data_dir()) / "freva" / "deployment"
+        self._user_config_dir = Path(appdirs.user_config_dir()) / "freva" / "deployment"
 
     @staticmethod
     def get_dirs(user: bool = True, key: str = "data") -> Path:
         """Get the 'scripts' and 'purelib' directories we'll install into.
 
         This is now a thin wrapper around sysconfig.get_paths(). It's not inlined,
         because some tests mock it out to install to a different location.
@@ -84,31 +78,33 @@
     @property
     def asset_dir(self) -> Path:
         data_dir = self.get_dirs(False) / "share" / "freva" / "deployment"
         user_dir = self.get_dirs(True) / "share" / "freva" / "deployment"
         for path in (data_dir, user_dir):
             if path.is_dir():
                 return path
-        raise ValueError(
+        raise ConfigurationError(
             "Could not find asset dir, please consider reinstalling the package."
         )
 
     @property
+    def inventory_file(self) -> Path:
+        return self.asset_dir / "config" / "inventory.toml"
+
+    @property
     def config_dir(self):
         inventory_file = self._user_config_dir / "inventory.toml"
         if inventory_file.exists():
             return self.asset_dir
         inventory_file.parent.mkdir(exist_ok=True, parents=True)
         try:
             inventory_file.unlink()
         except FileNotFoundError:
             pass
-        shutil.copy2(
-            self.asset_dir / "config" / "inventory.toml", inventory_file
-        )
+        shutil.copy2(self.asset_dir / "config" / "inventory.toml", inventory_file)
         return self._user_config_dir
 
     @property
     def config_file(self):
         cfg_file = self.config_dir / "freva-deployment.config"
         if not cfg_file.exists():
             cfg_file.parent.mkdir(exist_ok=True, parents=True)
@@ -144,226 +140,167 @@
             for varn, variable in variables.items():
                 if f"${{{varn}}}" in value or f"${varn}" in value:
                     value = value.replace(f"${{{varn}}}", f"${varn}")
                     value = value.replace(f"${varn}", variable)
             inp_dict[key] = get_current_file_dir(cfd, value)
 
 
+def _update_config(
+    new_config: MutableMapping[str, Any], old_config: MutableMapping[str, Any]
+) -> None:
+    for key, value in old_config.items():
+        if key in new_config and isinstance(value, dict):
+            _update_config(new_config[key], old_config[key])
+        else:
+            new_config[key] = value
+
+
+def _create_new_config(inp_file: Path) -> Path:
+    """Update any old configuration file to a newer version."""
+    config = cast(
+        Dict[str, Dict[str, Dict[str, Union[str, float, int, bool]]]],
+        tomlkit.loads(inp_file.read_text()),
+    )
+    create_backup = False
+    config_tmpl = tomlkit.loads(AD.inventory_file.read_text())
+    # Legacy solr:
+    if "solr" in config or "databrowser" in config:
+        create_backup = True
+        if "solr" in config:
+            config["freva_rest"] = config.pop("solr")
+            for key in ("port", "mem"):
+                if key in config["freva_rest"]["config"]:
+                    config["freva_rest"]["config"][f"solr_{key}"] = config[
+                        "freva_rest"
+                    ]["config"].pop(key)
+        else:
+            config["freva_rest"] = config.pop("databrowser")
+            config["freva_rest"]["config"]["freva_rest_port"] = config["freva_rest"][
+                "config"
+            ].pop("databrowser_port", "")
+            config["freva_rest"]["config"]["freva_rest_playbook"] = config[
+                "freva_rest"
+            ]["config"].pop("databrowser_playbook", "")
+    if create_backup:
+        backup_file = inp_file.with_suffix(inp_file.suffix + ".bck")
+        logger.info(
+            "Updating config file, original config can be found in %s",
+            backup_file,
+        )
+        backup_file.write_text(inp_file.read_text())
+        _update_config(config_tmpl, config)
+        inp_file.write_text(tomlkit.dumps(config_tmpl))
+    return inp_file
+
+
 def load_config(inp_file: str | Path) -> dict[str, Any]:
     """Load the inventory toml file and replace all environment variables."""
-    inp_file = Path(inp_file).expanduser().absolute()
+    inp_file = _create_new_config(Path(inp_file).expanduser().absolute())
     variables = cast(
-        dict[str, str], toml.loads(config_file.read_text())["variables"]
+        dict[str, str], tomlkit.loads(config_file.read_text())["variables"]
     )
-    config = toml.loads(inp_file.read_text())
+    config = tomlkit.loads(inp_file.read_text())
     _convert_dict(config, variables, inp_file.parent)
     return config
 
 
-def guess_map_server(
-    inp_server: str | None, default_port: int = 6111, mandatory: bool = True
-) -> str:
-    """Try to get the server name mapping the freva infrastructure.
-
-    Parameters
-    ----------
-    inp_server: str | None
-        Input server name, if None given, the code tries to read the
-        the server name from a previous deployment setup.
-    default_port: int, default: 6111
-        The port to connect to
-    mandatory: bool, default: True
-        If mandatory is set and no server could be found an error is risen.
-
-    Returns
-    -------
-    str: hostname of the server that runs the server map service
-
-    Raises
-    ------
-    ValueError: If no server could be found a ValueError is raised.
-    """
-    inp_server = inp_server or ""
-    if inp_server:
-        host_name, _, port = inp_server.partition(":")
-        port = port or str(default_port)
-        return f"{host_name}:{port}"
-    cache_dir = Path(appdirs.user_cache_dir()) / "freva-deployment"
-    try:
-        with (cache_dir / "freva_deployment.json").open() as f_obj:
-            inp_server = cast(str, json.load(f_obj)["server_map"])
-            host_name, _, port = inp_server.partition(":")
-            port = port or str(default_port)
-            return f"{host_name}:{port}"
-    except (
-        FileNotFoundError,
-        IOError,
-        ValueError,
-        KeyError,
-        json.JSONDecodeError,
-    ):
-        pass
-    if mandatory:
-        raise ValueError(
-            "You have to set the hostname to the services mapping "
-            "the freva infrastructure using the --server-map flag."
-        )
-    return ""
-
-
-def set_log_level(verbosity: int) -> None:
-    """Set the log level of the logger."""
-    logger.setLevel(max(logging.INFO - 10 * verbosity, logging.DEBUG))
-
-
-def get_setup_for_service(
-    service: str, setups: list[ServiceInfo]
-) -> tuple[str, str]:
+def get_setup_for_service(service: str, setups: list[ServiceInfo]) -> tuple[str, str]:
     """Get the setup of a service configuration."""
     for setup in setups:
         if setup.name == service:
             return setup.python_path, setup.hosts
-    raise KeyError("Service not found")
+    raise ConfigurationError("Service not found")
 
 
 def read_db_credentials(
     cert_file: Path, db_host: str, port: int = 5002
 ) -> dict[str, str]:
     """Read database config."""
     with cert_file.open() as f_obj:
-        key = "".join(
-            [k.strip() for k in f_obj.readlines() if not k.startswith("-")]
-        )
+        key = "".join([k.strip() for k in f_obj.readlines() if not k.startswith("-")])
         sha = hashlib.sha512(key.encode()).hexdigest()
     url = f"http://{db_host}:{port}/vault/data/{sha}"
     return requests.get(url).json()
 
 
-def download_server_map(
-    server_map,
-) -> dict[str, list[ServiceInfo]]:
-    """Download server information from the service that stores the server arch.
-
-    Parameters
-    ----------
-    server_map: str,
-        The hostname holding the server archtiecture information.
-    Returns
-    -------
-    dict[str, list[NamedTuple("service", [("name", str), ("python_path", str),
-                                     ("hosts", str)])]]
-    """
-    info: dict[str, list[ServiceInfo]] = {}
-    host, _, port = server_map.partition(":")
-    port = port or "6111"
-    req = requests.get(f"http://{host}:{port}")
-    if req.status_code != 200:
-        logger.error(req.json())
-        return {}
-    for proj, conf in req.json().items():
-        info[cast(str, proj)] = [
-            ServiceInfo(name=s, python_path=c[0], hosts=c[-1])
-            for (s, c) in conf.items()
-        ]
-    return info
-
-
-def upload_server_map(
-    server_map: str,
-    project_name: str,
-    deployment_setup: dict[str, dict[str, str]],
-) -> None:
-    """Upload server information to service that stores server archtiecture.
-
-    Parameters
-    ----------
-    server_map: str
-        The hostname holding the server archtiecture information.
-    project_name: str
-        Name of the freva project
-    deployment_setup: dict[str, str]
-        Server names for each deployed service
-    """
-    _upload_data: dict[str, dict[str, str]] = {}
-    for service, config in deployment_setup.items():
-        _upload_data[service] = config
-    host, _, port = server_map.partition(":")
-    port = port or "6111"
-    req_data = dict(config=toml.dumps(_upload_data))
-    logger.debug("Uploading %s", req_data)
-    req = requests.put(f"http://{host}:{port}/{project_name}", data=req_data)
-    if req.status_code == 201:
-        logger.info("Server information updated at %s", host)
-    else:
-        logger.error("Could not update server information %s", req.json())
-
-
 def get_email_credentials() -> tuple[str, str]:
     """Read login credentials for email server.
 
     Returns
     =======
     tuple: username and password
     """
-
+    username: str = os.environ.get("EMAIL_USER", "") or ""
+    password: str = os.environ.get("EMAIL_PASSWD", "") or ""
     msg = (
         "\nThe web will need login credentials to connect to the [b green]mail server [/]"
         "that has been set up.\nYou should now enter your [it]login credentials[/].\n"
         "[b]Note:[/]These credentials will be securely stored in an encrypted vault\n"
     )
-    RichConsole.print(msg)
-    username = Prompt.ask("[green b]Username[/] for mail server")
-    password = Prompt.ask(
-        "[green b]Password[/] for mail server", password=True
-    )
+    if not username or not password:
+        RichConsole.print(msg)
+        if not username:
+            username = Prompt.ask("[green b]Username[/] for mail server")
+        if not password:
+            password = Prompt.ask("[green b]Password[/] for mail server", password=True)
     return username, password
 
 
-def get_passwd(min_characters: int = 8) -> str:
+def get_passwd(master_pass: Optional[str] = None, min_characters: int = 8) -> str:
     """Create a secure pasword.
 
     Parameters
     ==========
     min_characters:
         The minimum lenght of the password (default 8)
 
     Returns
     =======
     str: The password
     """
-    logger.info("Creating Password")
+    logger.debug("Creating Password")
     msg = ""
-    RichConsole
     while True:
         try:
+            if master_pass:
+                return _passwd_is_good(master_pass, min_characters)
             return _create_passwd(min_characters, msg)
         except ValueError as e:
-            RichConsole.print(f"[red]{e.__str__()}[/]")
+            RichConsole.print(f"[red]{e}[/]")
             msg = "[b red]re-enter[/] master password"
+            master_pass = ""
 
 
-def _create_passwd(min_characters: int, msg: str = "") -> str:
-    """Create passwords."""
-    master_pass = Prompt.ask(msg or password_prompt, password=True)
+def _passwd_is_good(master_pass: str, min_characters: int) -> str:
+
     is_ok: bool = len(master_pass) > min_characters
     for check in ("[a-z]", "[A-Z]", "[0-9]"):
         if not re.search(check, master_pass):
             is_ok = False
             break
-    is_safe: bool = (
-        len([True for c in "[_@$#$%^&*-!]" if c in master_pass]) > 0
-    )
-    if is_ok is False or is_safe is False:
+    forbidden_characters = ":/?#[]@%"
+    is_ok = is_ok and len([True for c in "[_$^&*-!]" if c in master_pass]) > 0
+    for character in forbidden_characters:
+        if character in master_pass:
+            is_ok = False
+            break
+    if not is_ok:
         raise ValueError(
             (
                 "Password must confirm the following constraints:\n"
                 f"- {min_characters} alphanumeric characters long,\n"
                 "- have both, lower and upper case characters,\n"
-                "- have at least one special special character."
+                "- have at least one special special character.\n"
+                f"- must *not* not contain: {forbidden_characters}"
             )
         )
-    master_pass_2 = Prompt.ask(
-        "[bold green]re-enter[/] master password", password=True
-    )
+    return master_pass
+
+
+def _create_passwd(min_characters: int, msg: str = "") -> str:
+    """Create passwords."""
+    master_pass = Prompt.ask(msg or password_prompt, password=True)
+    _passwd_is_good(master_pass, min_characters)
+    master_pass_2 = Prompt.ask("[bold green]re-enter[/] master password", password=True)
     if master_pass != master_pass_2:
         raise ValueError("Passwords do not match")
     return master_pass
```

### Comparing `freva_deployment-2309.0.1/PKG-INFO` & `freva_deployment-2405.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,21 @@
-Metadata-Version: 2.1
-Name: freva-deployment
-Version: 2309.0.1
-Summary: Deployment of the Free Evaluation Framework Freva
-Author-email: "DKRZ, Clint" <freva@dkrz.de>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: appdirs
-Requires-Dist: ansible>=2.10
-Requires-Dist: npyscreen
-Requires-Dist: numpy
-Requires-Dist: PyMySQL
-Requires-Dist: PyYAML
-Requires-Dist: rich
-Requires-Dist: toml
-Requires-Dist: tomlkit
-Requires-Dist: requests
-Requires-Dist: pydata-sphinx-theme ; extra == "docs"
-Requires-Dist: sphinx ; extra == "docs"
-Requires-Dist: sphinx-copybutton ; extra == "docs"
-Requires-Dist: nbsphinx ; extra == "docs"
-Requires-Dist: recommonmark ; extra == "docs"
-Requires-Dist: sphinx_rtd_theme ; extra == "docs"
-Requires-Dist: ipython ; extra == "docs"
-Requires-Dist: sphinxcontrib_github_alt ; extra == "docs"
-Requires-Dist: mypy ; extra == "test"
-Requires-Dist: black ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: types-toml ; extra == "test"
-Requires-Dist: types-PyMySQL ; extra == "test"
-Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
-Project-URL: Home, https://freva-deployment.readthedocs.io/en/latest
-Project-URL: Issues, https://github.com/FREVA-CLINT/freva/issues
-Project-URL: Source, https://github.com/FREVA-CLINT/freva
-Provides-Extra: docs
-Provides-Extra: test
-
 # Deployment of the Free Evaluation Framework Freva
 
 [![Documentation Status](https://readthedocs.org/projects/freva-deployment/badge/?version=latest)](https://freva-deployment.readthedocs.io/en/latest/?badge=latest)
 
 The code in this repository is used to deploy freva in different computing
 environments. The general strategy is to split the deployment into
 4 different steps, these are :
 - Deploy MariaDB service via docker
 - Deploy a Hashicorp Vault service for storing and retrieving passwords
   and other sensitive data via docker
   (this step get automatically activated once the MariaDB service is set)
-- Deploy Apache Solr service via docker
+- Deploy [Databrowser API](https://github.com/FREVA-CLINT/databrowserAPI) service via docker
 - Deploy command line interface backend ([evaluation_system](https://github.com/FREVA-CLINT/freva))
-- Deploy web front end ([freva_web](https://gitlab.dkrz.de/freva/freva_web))
+- Deploy web front end ([freva_web](https://github.com/FREVA-CLINT/freva-web))
 
 
 > **_Note:_** A vault server is auto deployed once the mariadb server is deployed.
 The vault centrally stores all passwords and other sensitive data.
 During the deployment of the vault server a public key is generated which is
 used to open the vault. This public key will be saved in the `evaluation_system`
 backend root directory. Only if saved this key and the key in the vault match,
@@ -71,44 +27,19 @@
 install ansible via the `install_ansible` you'll have to use `conda` to
 install libselinux for your CentOS version.
 For example : `conda install -c conda-forge  libselinux-cos7-x86_64`
 
 # Pre-Requisites
 The main work will be done by
 [ansible](https://docs.ansible.com/ansible/latest/index.html), hence some level
-of familiarity with ansible is advantagous. Since we are using ansible we can
+of familiarity with ansible is advantageous. Since we are using ansible we can
 use this deployment routine from a workstation computer (like a Mac-book).
-You do not need to run the depoyment on the machines where things get installed.
+You do not need to run the deployment on the machines where things get installed.
 The only requirement is that you have to setup ansible and you can establish
 ssh connections to the servers.
-### Preparation on windows based system (without wsl).
-Currently ansible is not natively available on windows based systems. You can use
-the unix runtime environment [cygwin](https://www.cygwin.com) to download
-and install the needed software. Just follow the steps listed on the web page
-to setup cygwin on your windows system. In order to be able to install the
-freva deployment programm you'll first need to install the following packages
-via cygwin:
-
-- python3
-- python3-devel
-- git
-- make
-- python3.X-paramiko
-- libffi-devel
-- ansible
-
-We also recommend installing a command line based text editor like vim, nano, etc.
-
-After installing the above listed packages via cygwin you can clone and
-install the freva deployment:
-
-```console
-python3 -m pip install -U freva-deployment
-```
-Add the `--user` flag if you don't have sufficient rights.
 ## Installation on \*nix systems or wsl.
 If you're using Linux, OsX or a Windows subsystem for Linux (WSL) it should
 be sufficient to issues the following commands:
 
 ```console
 python3 pip install -U freva-deployment
 ```
@@ -117,14 +48,25 @@
 > **_Note:_** On *CentOS* python SELinux libraries need to be installed.
 > You will need to install libselinux for your CentOS version.
 
 ```console
 python3 -m pip install libselinux-python3
 ```
 
+## Using docker
+
+A pre-build docker image is available to run the deployment
+
+```console
+docker run -it -v /path/to/config:/opt/freva-deployment:z ghcr.io/freva-clint/freva-deployment
+```
+The `-it` flags are important in order to interact with the program. To use
+and save existing configurations you can mount the directories of the config
+files into the container.
+
 ## Commands after installation:
 The `pip install` command will create *four* different commands:
 - `deploy-freva-map`: To setup a service that keeps track of all deployed
    freva instances and their services.
 - `deploy-freva`: Text user interface to configure and run the deployment.
 - `deploy-freva-cmd`: Run already configured deployment.
 - `freva-service`: Start|Stop|Restart|Check services of freva instances.
@@ -136,56 +78,27 @@
 the following command to your local `.bashrc`:
 
 ```console
 export PATH=$PATH:$HOME/.local/bin
 ```
 
 
-## Installing docker/podman and sudo access to the service servers
-Since the services of MariaDB, Apache Solr and Apache web will be deployed on
-docker container images, docker needs to be available on the target servers.
-Usually installing and running docker requires *root* privileges.
-Hence, on the servers that will be running docker you will need root access.
-There exist an option to install and run docker without root,
-information on a root-less docker option
+## Installing docker-compose/podman-compose and sudo access to the service servers
+Because the services of MariaDB, DatabrowserAPI and Apache httpd will be deployed
+on docker container images, docker needs to be available on the target servers.
+Since version *v2309.0.0* of the deployment the containers are set up
+using `doker-compose`. Hence `docker-compose` (or `podman-compose`) has to be
+installed on the host systems. Usually installing and running docker
+requires *root* privileges. Hence, on the servers that will be running docker
+you will need root access. There exists an option to install and run docker
+without root, information on a root-less docker option
 can be found [on the docker docs](https://docs.docker.com/engine/security/rootless/)
 > **_Note:_** Some systems use `podman` instead of `docker`. The deployment
 routine is able to distinguish and use the right service.
 
-## Setting up a service that maps the server structure (Optional)
-Since the services might be scattered across different servers it might be hard
-to keep track of the host names of the servers where all services are running.
-We have created a service that keeps track of the locations of all services for
-a certain freva instance. Although not strictly needed we recommend you to setup
-this special server mapping service. To do so use the following command:
-
-```console
-deploy-freva-map --help
-usage: deploy-freva-map [-h] [--port PORT] [--wipe] [--user USER] [--python-path PYTHON_PATH] [-v] [-V] servername
-
-Create service that maps the freva server architecture.
-
-positional arguments:
-  servername            The server name where the infrastructure mapping service is deployed
-
-options:
-  -h, --help            show this help message and exit
-  --port PORT           The port the service is listing to (default: 6111)
-  --wipe                Delete any existing data. (default: False)
-  --user USER           Username to log on to the target server. (default: None)
-  --python-path PYTHON_PATH
-                        Path to the default python3 interpreter on the target machine. (default: /usr/bin/python)
-  -v, --verbose         Verbosity level (default: 0)
-  -V, --version         show program's version number and exit
-```
-> **_Note_:** As the service keeps track of all freva instances within your
-institution, this has to be deployed only *once*. Please make sure that other
-admins who might need to install freva are aware of the host name
-for this service. *This step is optional*
-
 # Configuring the deployment
 A complete freva instance will need the following services:
 
 - solrservers (hostname of the apache solr server)
 - dbservers (hostname of the MariaDB server)
 - webservers (hostname that will host the web site)
 - backendservers (hostname(s) where the command line interface will be installed)
@@ -240,70 +153,37 @@
 `migration` of an old freva system.
 
 ## Deployment with existing configuration.
 If you already have a configuration saved in a toml base inventory file you can
 issue the `deploy-freva-cmd` command:
 
 ```bash
-deploy-freva-cmd --help
-usage: deploy-freva-cmd [-h] [--server-map SERVER_MAP] [--config CONFIG]
-                        [--steps {services,web,core,db,solr,backup} [{services,web,core,db,solr,backup} ...]] [--ask-pass] [-v] [-V]
+eploy-freva-cmd --help
+usage: deploy-freva-cmd [-h] [--config CONFIG] [--steps {web,core,db,databrowser} [{web,core,db,databrowser} ...]] [--ask-pass] [--ssh-port SSH_PORT] [-v] [-l]
+                        [--gen-keys] [-V]
 
 Deploy freva and its services on different machines.
 
 options:
   -h, --help            show this help message and exit
-  --server-map SERVER_MAP
-                        Hostname of the service mapping the freva server archtiecture, Note: you can create a server map by running
-                        the deploy-freva-map command (default: None)
   --config CONFIG, -c CONFIG
-                        Path to ansible inventory file. (default: /home/wilfred/.config/freva/deployment/inventory.toml)
-  --steps {services,web,core,db,solr,backup} [{services,web,core,db,solr,backup} ...]
-                        The services/code stack to be deployed (default: ['services', 'web', 'core'])
+                        Path to ansible inventory file. (default: /home/wilfred/.anaconda3/share/freva/deployment/inventory.toml)
+  --steps {web,core,db,databrowser} [{web,core,db,databrowser} ...]
+                        The services/code stack to be deployed (default: ['db', 'databrowser', 'web', 'core'])
   --ask-pass            Connect to server via ssh passwd instead of public key. (default: False)
+  --ssh-port SSH_PORT   Set the ssh port, in 99.9% of the cases this should be 22 (default: 22)
   -v, --verbose         Verbosity level (default: 0)
+  -l, --local           Deploy services on the local machine, debug purpose. (default: False)
+  --gen-keys            Generate public and private web certs, use with caution. (default: False)
   -V, --version         show program's version number and exit
-```
 
-The `--steps` flags can be used if not all services should be deployed.
 
-# Accessing the services after deployment:
-If the target machine where the services (solr, mariadb, web) were deployed
-is a Linux machine you will have a `systemd` unit service was created.
-You can control the service via the `freva-service` command:
-
-```console
-freva-service --help
-usage: freva-service [-h] [--server-map SERVER_MAP] [--services {web,db,solr} [{web,db,solr} ...]] [--user USER] [-v] [-V]
-                     {start,stop,restart,status} [project_name]
-
-Interact with installed freva services.
-
-positional arguments:
-  {start,stop,restart,status}
-                        The start|stop|restart|status command for the service
-  project_name          Name of the project (default: all)
-
-options:
-  -h, --help            show this help message and exit
-  --server-map SERVER_MAP
-                        Hostname of the service mapping the freva server archtiecture, Note: you can create a server map by running
-                        the deploy-freva-map command (default: None)
-  --services {web,db,solr} [{web,db,solr} ...]
-                        The services to be started|stopped|restarted|checked (default: ['solr', 'db', 'web'])
-  --user USER, -u USER  connect as this user (default: None)
-  -v, --verbose         Verbosity level (default: 0)
-  -V, --version         show program's version number and exit
-```
-The following command restarts `web` server for the `xces`:
-```console
-freva-service restart xces --services web --user k12345
 ```
-All services (`db`, `web` and `solr`) will be selected if the `--services` option
-is omitted.
+
+The `--steps` flags can be used if not all services should be deployed.
 
 # Kown Issues:
 Below are possible solutions to some known issues:
 
 ### SSH connection fails:
 
 ```python
@@ -347,7 +227,121 @@
 git config --global user.email your@email.com
 ```
 
 
 # Advanced: Adjusting the playbook
 Playbook templates and be found the in the `playbooks` directory. You can also add new variables to the playbook if they are present in the `config/inventory` file.
 
+# Contributing to freva-deployment
+
+We welcome contributions from the community! Before you start contributing,
+please follow these steps to set up your development environment.
+Make sure you have the following prerequisites installed:
+
+- Python (>=3.x)
+- Git
+- Make
+
+```console
+git clone https://github.com/FREVA-CLINT/freva-deployment.git
+cd freva-deployment.git
+make
+```
+
+The deployment routine is supposed to interact with the user - this can
+can be asking for user names or passwords. To avoid such interaction you can
+set the following environment variables.
+
+- `MASTER_PASSWD`: the admin/root password for all services (db, web etc).
+- `EMAIL_USER`: the user name for email server login credentials.
+- `EMAIL_PASSWD`: the password for email server login credentials.
+- `ANSIBLE_BECOME_PASSWORD`: the password used in any *sudo* command.
+
+These environment variables have only an effect when the deployment is
+applied in debug or local mode using the `-l` flag.
+
+## Using a local VM for testing.
+A test freva instance can be deployed on a dedicated local virtual machine.
+This virtual machine is based on a minimal ubuntu server image and has
+docker and podman pre installed. To create the virtual machine simply
+run the following script.
+
+```console
+cloud-init/start-vm.sh -h
+```
+
+```bash
+Usage: start-vm.sh [-k|--kill], [-p|--port PORT]
+Create a new virtual machine (VM) ready for freva deployment.
+Options:
+  -k, --kill     Kill the virtual machine
+  -p, --port     Set the port of the service that is used to configure the VM default: 8000
+```
+
+> **_Note:_** *Before* running the script you will have to install [qemu](https://www.qemu.org/docs/master/).
+> The script has only been tested on Linux systems.
+
+You can then make use of the pre configured inventory file in
+`assets/share/freva/deployment/config/inventory.toml`. In order to deploy
+freva on the newly created VM you will have to instruct ansible to use
+ssh port 2222 instead of 22.
+
+The following command will install freva along all with it's components to
+the local VM:
+
+```console
+deploy-freva-cmd  assets/share/freva/deployment/config/inventory.toml --gen-keys --ssh-port 2222
+```
+
+If you want to tear down the created VM you can either press CTRL+C in the
+terminal where you created the VM or use the kill command:
+
+```console
+./cloud-init/start-vm.sh -k
+```
+
+## Development Workflow
+
+To install the code in development mode use:
+```console
+make
+```
+
+Unit tests, building the documentation, type annotations and code style tests
+are done with [tox](https://tox.wiki/en/latest/). To run all tests, linting
+in parallel simply execute the following command:
+
+```console
+tox -p 3
+```
+You can also run the each part alone, for example to only check the code style:
+
+```console
+tox -e lint
+```
+available options are ``lint``, ``types``, ``test`` and ``docs``.
+
+Tox runs in a separate python environment to run the tests in the current
+environment use:
+
+```console
+pytest
+```
+
+To reformat and do type checking:
+```console
+make lint
+```
+### Creating a new release.
+
+Once the development is finished and you decide that it's time for a new
+release of the software use the following command to trigger a release
+procedure:
+
+```console
+tox -e release
+```
+
+This will check the current version of the `main` branch and trigger
+a GitHub continuous integration pipeline to create a new release. The procedure
+performs a couple of checks, if theses checks fail please make sure to address
+the issues.
```

