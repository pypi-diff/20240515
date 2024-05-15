# Comparing `tmp/freva_deployment-2309.0.0.tar.gz` & `tmp/freva_deployment-2309.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2309.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freva_deployment-2309.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freva_deployment-2309.0.0.tar` & `freva_deployment-2309.0.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      125 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      121 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/dependabot/constraints.txt
--rw-r--r--   0        0        0     2755 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/workflows/build_job.yml
--rw-r--r--   0        0        0     2051 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/workflows/ci_job.yml
--rw-r--r--   0        0        0     1577 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/workflows/docker_job.yml
--rw-r--r--   0        0        0      838 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.github/workflows/pypi_job.yml
--rw-r--r--   0        0        0      318 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.gitignore
--rw-r--r--   0        0        0     1301 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      135 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1078 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/LICENSE
--rw-r--r--   0        0        0       15 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/MANIFEST.in
--rw-r--r--   0        0        0    15470 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/README.md
--rw-r--r--   0        0        0    11564 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/config/create_tables.sql
--rw-r--r--   0        0        0     2578 2023-09-14 10:17:07.920885 freva_deployment-2309.0.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
--rw-r--r--   0        0        0    10590 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/config/inventory.toml
--rw-r--r--   0        0        0     1360 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/db_service/password_rotate.py
--rw-r--r--   0        0        0      388 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/db_service/reset_root_pw.sh
--rw-r--r--   0        0        0     5040 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/core-server-playbook.yml
--rw-r--r--   0        0        0     5830 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/db-server-playbook.yml
--rw-r--r--   0        0        0     1957 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/server-map-playbook.yml
--rw-r--r--   0        0        0     3815 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/solr-server-playbook.yml
--rw-r--r--   0        0        0     3584 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/vault-server-playbook.yml
--rw-r--r--   0        0        0     7769 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/web-server-playbook.yml
--rwxr-xr-x   0        0        0      351 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/create_cron.sh
--rw-r--r--   0        0        0     4182 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/create_systemd.py
--rwxr-xr-x   0        0        0    16851 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/docker-or-podman
--rwxr-xr-x   0        0        0       66 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/dump_sql
--rwxr-xr-x   0        0        0      160 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/prepare-httpd
--rw-r--r--   0        0        0      527 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/servers/Dockerfile
--rw-r--r--   0        0        0      102 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/servers/freva/servers.toml
--rw-r--r--   0        0        0     5857 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/servers/restservice.py
--rw-r--r--   0        0        0      686 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/Dockerfile
--rw-r--r--   0        0        0     1398 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/deploy_vault.py
--rw-r--r--   0        0        0       50 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/policy-file.hcl
--rw-r--r--   0        0        0     4934 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/runserver.py
--rw-r--r--   0        0        0      175 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
--rw-r--r--   0        0        0      569 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/vault/vault-server-tls.hcl
--rwxr-xr-x   0        0        0     2305 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/web/Dockerfile
--rwxr-xr-x   0        0        0       38 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/web/docker_cmd.sh
--rwxr-xr-x   0        0        0       17 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/web/entrypoint.sh
--rw-r--r--   0        0        0    15874 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/assets/share/freva/deployment/web/freva_web.conf
--rw-r--r--   0        0        0     6965 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/AfterDeployment.md
--rw-r--r--   0        0        0     5483 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Architecture.md
--rwxr-xr-x   0        0        0    43499 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Concept_Map.png
--rw-r--r--   0        0        0     8596 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Configure.md
--rw-r--r--   0        0        0     6837 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Folders.md
--rw-r--r--   0        0        0     5998 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Installation.md
--rw-r--r--   0        0        0    11811 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/LegalNotes.md
--rw-r--r--   0        0        0      634 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Makefile
--rw-r--r--   0        0        0     2238 2023-09-14 10:17:05.668854 freva_deployment-2309.0.0/docs/Services.md
--rw-r--r--   0        0        0    57311 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Topography.png
--rwxr-xr-x   0        0        0    41164 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Topography_1.png
--rwxr-xr-x   0        0        0    29463 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Topography_2.png
--rwxr-xr-x   0        0        0    46480 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Topography_3.png
--rw-r--r--   0        0        0    12634 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Transition.md
--rw-r--r--   0        0        0    16780 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/TuiHowto.md
--rw-r--r--   0        0        0    14354 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/Variable.png
--rw-r--r--   0        0        0     3430 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/conf.py
--rw-r--r--   0        0        0      288 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/environment.yml
--rw-r--r--   0        0        0   119110 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/freva_flowchart-new.jpg
--rw-r--r--   0        0        0     8432 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/freva_owl.svg
--rw-r--r--   0        0        0     2412 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/make.bat
--rw-r--r--   0        0        0      649 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/modules.rst
--rw-r--r--   0        0        0   153459 2023-09-14 10:17:05.672854 freva_deployment-2309.0.0/docs/tui_core.png
--rw-r--r--   0        0        0    76747 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/docs/tui_db.png
--rw-r--r--   0        0        0    95292 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/docs/tui_run.png
--rw-r--r--   0        0        0    70322 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/docs/tui_solr.png
--rw-r--r--   0        0        0   153250 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/docs/tui_web.png
--rw-r--r--   0        0        0      750 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/mypy.ini
--rw-r--r--   0        0        0       89 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/pyinstaller/pyinstaller-script.py
--rw-r--r--   0        0        0     1862 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/__init__.py
--rw-r--r--   0        0        0      394 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/cli/__init__.py
--rw-r--r--   0        0        0     2256 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0        0        0     7596 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0        0        0     4095 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0        0        0     7203 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/cli/_service.py
--rw-r--r--   0        0        0    24342 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/deploy.py
--rw-r--r--   0        0        0        0 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/ui/__init__.py
--rw-r--r--   0        0        0     1701 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0        0        0    13254 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0        0        0    35152 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0        0        0    10252 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0        0        0    11889 2023-09-14 10:17:05.676854 freva_deployment-2309.0.0/src/freva_deployment/utils.py
--rw-r--r--   0        0        0    17151 1970-01-01 00:00:00.000000 freva_deployment-2309.0.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      121 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/dependabot/constraints.txt
+-rw-r--r--   0        0        0     2755 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/build_job.yml
+-rw-r--r--   0        0        0     2051 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/ci_job.yml
+-rw-r--r--   0        0        0     1577 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/docker_job.yml
+-rw-r--r--   0        0        0      918 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.github/workflows/pypi_job.yml
+-rw-r--r--   0        0        0      318 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.gitignore
+-rw-r--r--   0        0        0     1301 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      135 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1078 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/LICENSE
+-rw-r--r--   0        0        0       15 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/MANIFEST.in
+-rw-r--r--   0        0        0    15470 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/README.md
+-rw-r--r--   0        0        0    11564 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/config/create_tables.sql
+-rw-r--r--   0        0        0     2578 2023-09-15 05:58:20.422150 freva_deployment-2309.0.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
+-rw-r--r--   0        0        0    10590 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/config/inventory.toml
+-rw-r--r--   0        0        0     1360 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/password_rotate.py
+-rw-r--r--   0        0        0      388 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/reset_root_pw.sh
+-rw-r--r--   0        0        0     5040 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/core-server-playbook.yml
+-rw-r--r--   0        0        0     5830 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/db-server-playbook.yml
+-rw-r--r--   0        0        0     1957 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/server-map-playbook.yml
+-rw-r--r--   0        0        0     3815 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/solr-server-playbook.yml
+-rw-r--r--   0        0        0     3584 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/vault-server-playbook.yml
+-rw-r--r--   0        0        0     7769 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/web-server-playbook.yml
+-rwxr-xr-x   0        0        0      351 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_cron.sh
+-rw-r--r--   0        0        0     4182 2023-09-15 05:58:19.802151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_systemd.py
+-rwxr-xr-x   0        0        0    16851 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/docker-or-podman
+-rwxr-xr-x   0        0        0       66 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/dump_sql
+-rwxr-xr-x   0        0        0      160 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/prepare-httpd
+-rw-r--r--   0        0        0      527 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/Dockerfile
+-rw-r--r--   0        0        0      102 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/freva/servers.toml
+-rw-r--r--   0        0        0     5857 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/servers/restservice.py
+-rw-r--r--   0        0        0      686 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/Dockerfile
+-rw-r--r--   0        0        0     1398 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/deploy_vault.py
+-rw-r--r--   0        0        0       50 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/policy-file.hcl
+-rw-r--r--   0        0        0     4934 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/runserver.py
+-rw-r--r--   0        0        0      175 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
+-rw-r--r--   0        0        0      569 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/vault/vault-server-tls.hcl
+-rwxr-xr-x   0        0        0     2305 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/Dockerfile
+-rwxr-xr-x   0        0        0       38 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/docker_cmd.sh
+-rwxr-xr-x   0        0        0       17 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/entrypoint.sh
+-rw-r--r--   0        0        0    15874 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/assets/share/freva/deployment/web/freva_web.conf
+-rw-r--r--   0        0        0     6965 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/AfterDeployment.md
+-rw-r--r--   0        0        0     5483 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Architecture.md
+-rwxr-xr-x   0        0        0    43499 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Concept_Map.png
+-rw-r--r--   0        0        0     8596 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Configure.md
+-rw-r--r--   0        0        0     6837 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Folders.md
+-rw-r--r--   0        0        0     5998 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Installation.md
+-rw-r--r--   0        0        0    11811 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/LegalNotes.md
+-rw-r--r--   0        0        0      634 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Makefile
+-rw-r--r--   0        0        0     2238 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Services.md
+-rw-r--r--   0        0        0    57311 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography.png
+-rwxr-xr-x   0        0        0    41164 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_1.png
+-rwxr-xr-x   0        0        0    29463 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_2.png
+-rwxr-xr-x   0        0        0    46480 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Topography_3.png
+-rw-r--r--   0        0        0    12634 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Transition.md
+-rw-r--r--   0        0        0    16780 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/TuiHowto.md
+-rw-r--r--   0        0        0    14354 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/Variable.png
+-rw-r--r--   0        0        0     3430 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/conf.py
+-rw-r--r--   0        0        0      288 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/environment.yml
+-rw-r--r--   0        0        0   119110 2023-09-15 05:58:19.806151 freva_deployment-2309.0.1/docs/freva_flowchart-new.jpg
+-rw-r--r--   0        0        0     8432 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/freva_owl.svg
+-rw-r--r--   0        0        0     2412 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/make.bat
+-rw-r--r--   0        0        0      649 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/modules.rst
+-rw-r--r--   0        0        0   153459 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_core.png
+-rw-r--r--   0        0        0    76747 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_db.png
+-rw-r--r--   0        0        0    95292 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_run.png
+-rw-r--r--   0        0        0    70322 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_solr.png
+-rw-r--r--   0        0        0   153250 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/docs/tui_web.png
+-rw-r--r--   0        0        0      750 2023-09-15 05:58:19.810151 freva_deployment-2309.0.1/mypy.ini
+-rw-r--r--   0        0        0       89 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/pyinstaller/pyinstaller-script.py
+-rw-r--r--   0        0        0     1862 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/__init__.py
+-rw-r--r--   0        0        0      394 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0        0        0     2256 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0        0        0     7596 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0        0        0     4095 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0        0        0     7203 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/cli/_service.py
+-rw-r--r--   0        0        0    24342 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/deploy.py
+-rw-r--r--   0        0        0        0 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/__init__.py
+-rw-r--r--   0        0        0     1701 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0        0        0    13254 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0        0        0    35152 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0        0        0    10252 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0        0        0    11889 2023-09-15 05:58:19.814151 freva_deployment-2309.0.1/src/freva_deployment/utils.py
+-rw-r--r--   0        0        0    17151 1970-01-01 00:00:00.000000 freva_deployment-2309.0.1/PKG-INFO
```

### Comparing `freva_deployment-2309.0.0/.github/workflows/build_job.yml` & `freva_deployment-2309.0.1/.github/workflows/build_job.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/.github/workflows/ci_job.yml` & `freva_deployment-2309.0.1/.github/workflows/ci_job.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/.github/workflows/docker_job.yml` & `freva_deployment-2309.0.1/.github/workflows/docker_job.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/.github/workflows/pypi_job.yml` & `freva_deployment-2309.0.1/.github/workflows/pypi_job.yml`

 * *Files 27% similar despite different names*

```diff
@@ -5,17 +5,14 @@
   push:
     tags:
       - "*"
 
 jobs:
   pipy:
     runs-on: ubuntu-latest
-    env:
-      FLIT_USERNAME: __token__
-      FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
     steps:
       -
         name: Checkout
         uses: actions/checkout@v4
       -
         name: Setup Python
         uses: actions/setup-python@v4
@@ -23,9 +20,14 @@
           python-version: "3.x"
       - name: Adding the evaluation config file
         run: wget https://raw.githubusercontent.com/FREVA-CLINT/freva/main/assets/evaluation_system.conf -O assets/share/freva/deployment/config/evaluation_system.conf.tmpl
       -
         name: Install flit
         run: python -m pip install flit
       -
-        name: Publishing freva-deployment 📦 to PyPI
-        run: flit publish
+        name: Building freva-deployment 📦 with flit
+        run: flit build
+      -
+        name: publish distribution 📦 to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `freva_deployment-2309.0.0/.gitlab-ci.yml` & `freva_deployment-2309.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/LICENSE` & `freva_deployment-2309.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/README.md` & `freva_deployment-2309.0.1/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/config/create_tables.sql` & `freva_deployment-2309.0.1/assets/share/freva/deployment/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl` & `freva_deployment-2309.0.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/config/inventory.toml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/config/inventory.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/db_service/password_rotate.py` & `freva_deployment-2309.0.1/assets/share/freva/deployment/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/core-server-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/db-server-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/server-map-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/server-map-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/solr-server-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/solr-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/vault-server-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/vault-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/playbooks/web-server-playbook.yml` & `freva_deployment-2309.0.1/assets/share/freva/deployment/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/create_systemd.py` & `freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/scripts/docker-or-podman` & `freva_deployment-2309.0.1/assets/share/freva/deployment/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/servers/Dockerfile` & `freva_deployment-2309.0.1/assets/share/freva/deployment/servers/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/servers/restservice.py` & `freva_deployment-2309.0.1/assets/share/freva/deployment/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/vault/Dockerfile` & `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/vault/deploy_vault.py` & `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/vault/runserver.py` & `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/vault/vault-server-tls.hcl` & `freva_deployment-2309.0.1/assets/share/freva/deployment/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/web/Dockerfile` & `freva_deployment-2309.0.1/assets/share/freva/deployment/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/assets/share/freva/deployment/web/freva_web.conf` & `freva_deployment-2309.0.1/assets/share/freva/deployment/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/AfterDeployment.md` & `freva_deployment-2309.0.1/docs/AfterDeployment.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Architecture.md` & `freva_deployment-2309.0.1/docs/Architecture.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Concept_Map.png` & `freva_deployment-2309.0.1/docs/Concept_Map.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Configure.md` & `freva_deployment-2309.0.1/docs/Configure.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Folders.md` & `freva_deployment-2309.0.1/docs/Folders.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Installation.md` & `freva_deployment-2309.0.1/docs/Installation.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/LegalNotes.md` & `freva_deployment-2309.0.1/docs/LegalNotes.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Makefile` & `freva_deployment-2309.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Services.md` & `freva_deployment-2309.0.1/docs/Services.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Topography.png` & `freva_deployment-2309.0.1/docs/Topography.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Topography_1.png` & `freva_deployment-2309.0.1/docs/Topography_1.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Topography_2.png` & `freva_deployment-2309.0.1/docs/Topography_2.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Topography_3.png` & `freva_deployment-2309.0.1/docs/Topography_3.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Transition.md` & `freva_deployment-2309.0.1/docs/Transition.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/TuiHowto.md` & `freva_deployment-2309.0.1/docs/TuiHowto.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/Variable.png` & `freva_deployment-2309.0.1/docs/Variable.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/conf.py` & `freva_deployment-2309.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/freva_flowchart-new.jpg` & `freva_deployment-2309.0.1/docs/freva_flowchart-new.jpg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/freva_owl.svg` & `freva_deployment-2309.0.1/docs/freva_owl.svg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/index.rst` & `freva_deployment-2309.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/make.bat` & `freva_deployment-2309.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/modules.rst` & `freva_deployment-2309.0.1/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/tui_core.png` & `freva_deployment-2309.0.1/docs/tui_core.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/tui_db.png` & `freva_deployment-2309.0.1/docs/tui_db.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/tui_run.png` & `freva_deployment-2309.0.1/docs/tui_run.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/tui_solr.png` & `freva_deployment-2309.0.1/docs/tui_solr.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/docs/tui_web.png` & `freva_deployment-2309.0.1/docs/tui_web.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/mypy.ini` & `freva_deployment-2309.0.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/pyproject.toml` & `freva_deployment-2309.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2309.0.1/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2309.0.1/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2309.0.1/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/cli/_service.py` & `freva_deployment-2309.0.1/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/deploy.py` & `freva_deployment-2309.0.1/src/freva_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2309.0.1/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/src/freva_deployment/utils.py` & `freva_deployment-2309.0.1/src/freva_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2309.0.0/PKG-INFO` & `freva_deployment-2309.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2309.0.0
+Version: 2309.0.1
 Summary: Deployment of the Free Evaluation Framework Freva
 Author-email: "DKRZ, Clint" <freva@dkrz.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

