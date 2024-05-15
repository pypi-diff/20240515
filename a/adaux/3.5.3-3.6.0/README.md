# Comparing `tmp/adaux-3.5.3.tar.gz` & `tmp/adaux-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-3.5.3.tar", last modified: Wed Mar 20 15:48:03 2024, max compression
+gzip compressed data, was "adaux-3.6.0.tar", last modified: Wed May 15 12:28:35 2024, max compression
```

## Comparing `adaux-3.5.3.tar` & `adaux-3.6.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.155061 adaux-3.5.3/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-03-10 17:43:30.000000 adaux-3.5.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-20 15:48:03.155061 adaux-3.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-03-20 15:48:03.155061 adaux-3.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-10 17:43:30.000000 adaux-3.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.139061 adaux-3.5.3/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.143061 adaux-3.5.3/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-03-20 15:38:17.000000 adaux-3.5.3/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14881 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_cli_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)    18271 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_cli_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_cli_multimanage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4954 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5686 2024-03-12 15:13:55.000000 adaux-3.5.3/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5083 2024-03-13 05:25:21.000000 adaux-3.5.3/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_04_migrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     6506 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_05_python_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5026 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-03-12 20:23:30.000000 adaux-3.5.3/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4614 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5780 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     7067 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_12a_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     3653 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_12b_ruff.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     1175 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_13b_entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    20588 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    16446 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    19110 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     7252 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_21_multi_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     4050 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12782 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    22464 2024-03-13 05:25:21.000000 adaux-3.5.3/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2024-03-13 05:25:21.000000 adaux-3.5.3/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    16452 2024-03-18 05:27:21.000000 adaux-3.5.3/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     9119 2024-03-13 05:25:21.000000 adaux-3.5.3/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     8891 2024-03-20 15:46:13.000000 adaux-3.5.3/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 15:47:49.000000 adaux-3.5.3/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1222 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/needs.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/services.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/tags.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/CI/jinja-snippets/variables.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.139061 adaux-3.5.3/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      639 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy-ext/
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy-ext/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/devenv/
--rw-rw-rw-   0 root         (0) root         (0)      713 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/devenv/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/devenv/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-18 05:27:21.000000 adaux-3.5.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/docs/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/gitlab-release/
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/gitlab-release/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1916 2024-03-13 05:22:56.000000 adaux-3.5.3/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      734 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/image/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.147061 adaux-3.5.3/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-03-12 14:01:29.000000 adaux-3.5.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/image-pytest/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/entry_points_add.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/entry_points_rm.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-03-12 14:01:29.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-03-14 08:13:13.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/pip_uv.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      680 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pkg-gitlab/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pkg-pypi/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1395 2024-03-12 14:58:32.000000 adaux-3.5.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-03-12 20:23:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pre-commit/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pycov/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pytest/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-14 08:10:44.000000 adaux-3.5.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/pytest-standalone/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-03-14 08:10:44.000000 adaux-3.5.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docker/services/python-deps/compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4878 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      586 2024-03-12 14:01:29.000000 adaux-3.5.3/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.139061 adaux-3.5.3/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     6630 2024-03-20 15:47:54.000000 adaux-3.5.3/source/adaux/src/payload/python/__pycache__/functions.cpython-311.pyc
--rw-rw-rw-   0 root         (0) root         (0)     4380 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.151061 adaux-3.5.3/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.155061 adaux-3.5.3/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5678 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.155061 adaux-3.5.3/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.155061 adaux-3.5.3/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-10 17:43:30.000000 adaux-3.5.3/source/adaux/src/root/source/gitignore.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 15:48:03.143061 adaux-3.5.3/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6073 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 15:47:53.000000 adaux-3.5.3/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      254 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-20 15:48:03.000000 adaux-3.5.3/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-15 09:50:41.000000 adaux-3.6.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-15 12:28:35.762982 adaux-3.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-15 12:28:35.762982 adaux-3.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-26 04:41:01.000000 adaux-3.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.746981 adaux-3.6.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.750981 adaux-3.6.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14881 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_cli_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)    18271 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_cli_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_cli_multimanage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.754981 adaux-3.6.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4954 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5083 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_04_migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6506 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_05_python_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5026 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4614 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5780 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7167 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_12a_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3750 2024-05-15 11:56:59.000000 adaux-3.6.0/source/adaux/_components/_12b_ruff.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_13b_entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20588 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    16446 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    19110 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_21_multi_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12782 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.754981 adaux-3.6.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    16452 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     9119 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8891 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 12:28:09.000000 adaux-3.6.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.754981 adaux-3.6.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.754981 adaux-3.6.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/needs.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/services.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/CI/jinja-snippets/variables.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.750981 adaux-3.6.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy-ext/
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy-ext/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/devenv/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/devenv/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/devenv/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/docs/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/gitlab-release/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/gitlab-release/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      734 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/image/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/image-pytest/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/ansible_deploy.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/ansible_env.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/entry_points_add.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/entry_points_rm.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/pip_uv.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pkg-gitlab/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pkg-pypi/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pre-commit/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      612 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pycov/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pytest/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.758982 adaux-3.6.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/pytest-standalone/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docker/services/python-deps/compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4878 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      586 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.750981 adaux-3.6.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     6630 2024-05-15 12:28:14.000000 adaux-3.6.0/source/adaux/src/payload/python/__pycache__/functions.cpython-311.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2024-05-15 11:56:59.000000 adaux-3.6.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.762982 adaux-3.6.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-15 09:50:41.000000 adaux-3.6.0/source/adaux/src/root/source/gitignore.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:28:35.750981 adaux-3.6.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6073 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 12:28:13.000000 adaux-3.6.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      259 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 12:28:35.000000 adaux-3.6.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-3.5.3/LICENSE.txt` & `adaux-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/setup.cfg` & `adaux-3.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 package_dir = 
 	= source
 python_requires = >=3.8
 install_requires = 
 	click~=8.1.7
 	click-help-colors~=0.9.1
 	colorlog~=6.7.0
-	pylint>=3.1.0
+	pylint>=3.2.0
 	jinja2~=3.0
 	ruamel.yaml>=0.17
 	requests[use_chardet_on_py3]~=2.0
 	beautifulsoup4~=4.11
 scripts = 
 
 [options.packages.find]
@@ -39,20 +39,20 @@
 	src/*/*
 	src/*/*/*
 	src/*/*/*/*
 
 [options.extras_require]
 dev = 
 	pre-commit>=3.3.3
-	ruff==v0.3.2
-	mypy>=1.9.0
+	ruff==v0.4.4
+	mypy>=1.10.0
 	types-requests
 test = 
-	pytest~=8.1
-	pytest-cov~=4.1
+	pytest~=8.2.0
+	pytest-cov~=5.0.0
 
 [tool:pytest]
 markers = 
 	merge_only: run test only on merge request
 	local: run local tests that need docker
 addopts = --strict-markers -m "not merge_only and not local"
 cache_dir = devops/cache/pytest
```

### Comparing `adaux-3.5.3/source/adaux/_base_parser.py` & `adaux-3.6.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_cli.py` & `adaux-3.6.0/source/adaux/_cli.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_cli_gitlab.py` & `adaux-3.6.0/source/adaux/_cli_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_cli_mixin.py` & `adaux-3.6.0/source/adaux/_cli_mixin.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_cli_multimanage.py` & `adaux-3.6.0/source/adaux/_cli_multimanage.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 @click.argument("cmd_parts", nargs=-1)
 def a(ctx: click.Context, cmd_parts: tp.Tuple[str]) -> None:
     """
     Run adaux command / Shorthand for "adaux mm run adaux"
     """
     with convert_runtime_to_click_error(ctx):
         with ctx.obj.extra():
+            cmd_str = ""
             if len(cmd_parts) == 0:
                 ctx.exit(1)
             elif len(cmd_parts) > 1:
                 cmd_str = shlex.join(cmd_parts)
             else:
                 cmd_str = cmd_parts[0]
             ctx.obj.mm_adaux(cmd_str)
```

### Comparing `adaux-3.5.3/source/adaux/_components/_01_file_io_support.py` & `adaux-3.6.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_02_base.py` & `adaux-3.6.0/source/adaux/_components/_02_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 from ._01_file_io_support import FileIOSupport
 
 
 class BaseComponent(FileIOSupport):
     def __init__(self) -> None:
         super().__init__()
         self.versions = _ProtoNamespace(
-            pytest="pytest~=8.1",
-            pytest_cov="pytest-cov~=4.1",
+            pytest="pytest~=8.2.0",
+            pytest_cov="pytest-cov~=5.0.0",
             pre_commit="pre-commit>=3.3.3",
-            mypy="mypy==1.9.0",
-            pylint="pylint==3.1.0",
-            black="black==24.2.0",
+            mypy="mypy==1.10.0",
+            pylint="pylint==3.2.0",
+            black="black==24.4.2",
             sphinx="sphinx==6.2.1",  # rtd-theme forces sphinx <7
             sphinx_rtd_theme="sphinx-rtd-theme>=1.2.2",
             sphinx_click="sphinx-click>=4.4.0",
             jupyter_sphinx="jupyter-sphinx>=0.4",
             bash_kernel="bash_kernel>=0.8",
             blacken_docs="blacken-docs==1.16.0",
-            pre_commit_hooks="pre-commit-hooks==v4.5.0",
-            pyupgrade="pyupgrade==v3.15.1",
+            pre_commit_hooks="pre-commit-hooks==v4.6.0",
+            pyupgrade="pyupgrade==v3.15.2",
             pycln="pycln==v2.4.0",
             reorder_python_imports="reorder_python_imports==v3.12.0",
             isort="isort==5.12.0",
             encryption_check="encryption_check==v1.0.0",
             docstr_coverage="docstr-coverage==v2.3.0",
             requests="requests==2.31.0",
             types_requests="types-requests",
             adaux=f"adaux=={LazyVersionStr()}",
             docker_compose_file="3.8",
             ci_docker_image="docker:24.0.6",  # if you touch this, build build-docker-with-adaux locally first
             ci_precursor_image="registry.gitlab.prostructura.ch/administratum/auxilium/dind-with-precursor:latest",
             ci_adaux_image=f"docker.io/prostructura/adaux:{LazyVersionStr()}",
-            ruff="ruff==v0.3.2",
+            ruff="ruff==v0.4.4",
         )
         self.auxcon = _ProtoNamespace()
 
     def migrate(self) -> None:
         logger.info("no migration plugin detected")
 
     def formatted(self) -> None:
```

### Comparing `adaux-3.5.3/source/adaux/_components/_03_meta.py` & `adaux-3.6.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_04_migrate.py` & `adaux-3.6.0/source/adaux/_components/_04_migrate.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_04_monotonic_version.py` & `adaux-3.6.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_05_project.py` & `adaux-3.6.0/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_05_python_project.py` & `adaux-3.6.0/source/adaux/_components/_05_python_project.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_06_dependency.py` & `adaux-3.6.0/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_07_package.py` & `adaux-3.6.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_08_pip.py` & `adaux-3.6.0/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_09_gitignore.py` & `adaux-3.6.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_10_gitlab.py` & `adaux-3.6.0/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_11_precommit.py` & `adaux-3.6.0/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_12a_pylint.py` & `adaux-3.6.0/source/adaux/_components/_12a_pylint.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return (
             "disable",
             "good_names",
             "class_attr_rgx",
             "min_similarity_lines",
+            "max_module_lines",
             "argument_rgx",
             "attr_rgx",
             "function_rgx",
             "variable_rgx",
             "method_rgx",
         )
 
@@ -135,14 +136,15 @@
                 configs.append(config)
 
             key = key.replace("-", "_")
             for key1, key2, key3 in [
                 ("MESSAGES CONTROL", "disable", "disable"),
                 ("BASIC", "good-names", "good_names"),
                 ("SIMILARITIES", "min-similarity-lines", "min_similarity_lines"),
+                ("FORMAT", "max-module-lines", "max_module_lines"),
                 ("BASIC", "variable-rgx", "variable_rgx"),
                 ("BASIC", "const-rgx", "const_rgx"),
                 ("BASIC", "function-rgx", "function_rgx"),
                 ("BASIC", "argument-rgx", "argument_rgx"),
                 ("BASIC", "class-rgx", "class_rgx"),
                 ("BASIC", "attr-rgx", "attr_rgx"),
                 ("BASIC", "method-rgx", "method_rgx"),
```

### Comparing `adaux-3.5.3/source/adaux/_components/_12b_ruff.py` & `adaux-3.6.0/source/adaux/_components/_12b_ruff.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,32 +70,36 @@
             self.auxd.ruff_test.setdefault(key, [])
 
     def bake(self) -> None:  # pylint: disable=too-many-locals,too-many-branches
         super().bake()
         if "ruff" not in self.auxf:
             return
         dest = self.target / "pre-commit/ruff.toml"
-        data = copy.copy(self.auxe.ruff)
+        res = copy.copy(self.auxe.ruff)
+        data = {"lint": res}
         data["cache-dir"] = "devops/cache/ruff"
         for key in ["per_file_ignores"]:
-            data[key.replace("_", "-")] = data.pop(key)
+            res[key.replace("_", "-")] = res.pop(key)
+
         written = TomlParser.write(data, dest)
         if written:
             self._print(f"baked {dest}", fg="green")
 
         for key, val in self.auxf.get("ruff_test", {}).items():
             prev = data.get(key, None)
             if prev is None:
                 updated = val
-            if isinstance(prev, list):
+            elif isinstance(prev, list):
                 assert isinstance(val, list)
                 updated = prev + val
-            if isinstance(prev, dict):
+            elif isinstance(prev, dict):
                 print(prev, val)
                 assert isinstance(val, dict)
                 updated = {**prev, **val}
+            else:
+                raise NotImplementedError(prev)
             data[key] = updated
 
         dest = self.target / "pre-commit/ruff-test.toml"
         written = TomlParser.write(data, dest)
         if written:
             self._print(f"baked {dest}", fg="green")
```

### Comparing `adaux-3.5.3/source/adaux/_components/_13_executable.py` & `adaux-3.6.0/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_13b_entry_points.py` & `adaux-3.6.0/source/adaux/_components/_13b_entry_points.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_14_mypy.py` & `adaux-3.6.0/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_15_pytest.py` & `adaux-3.6.0/source/adaux/_components/_15_pytest.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_17_docs.py` & `adaux-3.6.0/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_18_payload.py` & `adaux-3.6.0/source/adaux/_components/_18_payload.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_19_docker.py` & `adaux-3.6.0/source/adaux/_components/_19_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_20_ci.py` & `adaux-3.6.0/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_21_multi_manage.py` & `adaux-3.6.0/source/adaux/_components/_21_multi_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,17 @@
             columns, _ = shutil.get_terminal_size((80, 20))
             msg = f"> {cmd_str}"
             padding = columns - len(msg)
             self._print(msg, fg="blue", nl=not kwgs["capture_output"])
         cmd = shlex.split(cmd_str)
         try:
             res = subprocess_run(cmd, *args, **kwgs)
-            if show and kwgs["capture_output"]:
-                self._print((padding - 4) * " " + "[ok]", fg="green")
+            if show:
+                if kwgs["capture_output"]:
+                    self._print((padding - 4) * " " + "[ok]", fg="green")
             return res
         except subprocess.CalledProcessError as err:
             if show and kwgs["capture_output"]:
                 self._print((padding - 6) * " " + "[fail]", fg="red")
             raise RuntimeError(f"error when running {cmd}, see error above") from err
 
     def subprocess_run_shlex_out(self, *args: tp.Any, **kwgs: tp.Any) -> str:
```

### Comparing `adaux-3.5.3/source/adaux/_components/_98_sentinel.py` & `adaux-3.6.0/source/adaux/_components/_98_sentinel.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         if self._extra_counter[level] == 0:
             del self.auxh
 
     @contextlib.contextmanager
     def extra(
         self, level: ExtraLevel = ExtraLevel.ENRICHED
     ) -> tp.Iterator[_ProtoNamespace]:
+        # pylint: disable=contextmanager-generator-missing-cleanup
         if self._extra_counter[level] == 0:
             logger.debug("enabled %s", level)
         if level == ExtraLevel.TEMPLATED:
             self.templated()
             with self.with_formatted() as aux:
                 yield aux
         elif level == ExtraLevel.TEMPLATED_WITH_NEGATIVE:
@@ -91,15 +92,15 @@
             with self.with_formatted() as aux:
                 yield aux
         elif level == ExtraLevel.DEMODATA:
             self.templated()
             self.demodata()
             with self.with_formatted() as aux:
                 yield aux
-        if level == ExtraLevel.RAW:
+        elif level == ExtraLevel.RAW:
             yield self.auxcon
         elif level == ExtraLevel.FORMATTED:
             with self.with_formatted() as aux:
                 yield aux
         elif level == ExtraLevel.DEFAULTED:
             with self.with_formatted(), self.with_defaulted() as aux:
                 yield aux
```

### Comparing `adaux-3.5.3/source/adaux/_components/_99_all.py` & `adaux-3.6.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_aux_ci.py` & `adaux-3.6.0/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/__init__.py` & `adaux-3.6.0/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_base.py` & `adaux-3.6.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_docker.py` & `adaux-3.6.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_docker_build.py` & `adaux-3.6.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_docker_executors.py` & `adaux-3.6.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_docker_run.py` & `adaux-3.6.0/source/adaux/_components/_payload/_docker_run.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_python.py` & `adaux-3.6.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_components/_payload/_with_dependency.py` & `adaux-3.6.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_create_badge.py` & `adaux-3.6.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_gitlab.py` & `adaux-3.6.0/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_logging.py` & `adaux-3.6.0/source/adaux/_logging.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_parser.py` & `adaux-3.6.0/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_proto_namespace.py` & `adaux-3.6.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_tick.py` & `adaux-3.6.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_todo.py` & `adaux-3.6.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/_util.py` & `adaux-3.6.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-3.6.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-3.6.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/devenv/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/devenv/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/devenv/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/devenv/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/docs/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/docs/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/gitlab-release/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/gitlab-release/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/image/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/image/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/jinja-snippets/macros.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pkg-gitlab/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pkg-gitlab/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pkg-pypi/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pkg-pypi/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pre-commit/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pre-commit/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pycov/compose.yml.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pycov/compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-3.6.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-3.6.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/docs/postprocess_html.py` & `adaux-3.6.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/install-dev.sh.jinja2` & `adaux-3.6.0/source/adaux/src/install-dev.sh.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-3.6.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-3.6.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/license/MIT.txt.jinja2` & `adaux-3.6.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/payload/python/__pycache__/functions.cpython-311.pyc` & `adaux-3.6.0/source/adaux/src/payload/python/__pycache__/functions.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x42f1ed65 (Sun Mar 10 17:43:30 2024 UTC)
+moddate:  0x71854466 (Wed May 15 09:50:41 2024 UTC)
 files sz: 4380
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
```

### Comparing `adaux-3.5.3/source/adaux/src/payload/python/functions.py` & `adaux-3.6.0/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-3.6.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-3.5.3/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-3.6.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         types:
         - python
         exclude: devops/|playground/
 -   repo: local
     hooks:
     -   id: ruff
         name: ruff            - python style enforcer
-        entry: ruff
+        entry: ruff check
         language: system
         args:
         - --config=devops/pre-commit/ruff.toml
         types:
         - python
         exclude: devops/|playground/
 -   repo: local
```

### Comparing `adaux-3.5.3/source/adaux.egg-info/SOURCES.txt` & `adaux-3.6.0/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

