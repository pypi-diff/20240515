# Comparing `tmp/tljh_repo2docker-2.0.0a0.tar.gz` & `tmp/tljh_repo2docker-2.0.0a1.tar.gz`

## Comparing `tljh_repo2docker-2.0.0a0.tar` & `tljh_repo2docker-2.0.0a1.tar`

### file list

```diff
@@ -1,139 +1,173 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/.prettierignore
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/CONTRIBUTING.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/dev-requirements.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/jupyterhub_config.py
--rw-r--r--   0        0        0   279512 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/package-lock.json
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/package.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/pytest.ini
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tsconfig.json
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/webpack.config.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/AxiosContext.tsx
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/ButtonWithConfirm.tsx
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/JupyterhubContext.ts
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/LoadingAnimation.tsx
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/SmallTextField.tsx
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/axiosclient.ts
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/style.css
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/theme.ts
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/utils.ts
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/App.tsx
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/EnvironmentList.tsx
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/LogDialog.tsx
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/NewEnvironmentDialog.tsx
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/RemoveEnvironmentButton.tsx
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/main.tsx
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/types.ts
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/App.tsx
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/NewServerDialog.tsx
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/OpenServerButton.tsx
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/RemoveServerButton.tsx
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/ServersList.tsx
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/main.tsx
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/types.ts
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/__main__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/_version.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/app.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/base.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/builder.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/docker.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/environments.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/logs.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/model.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/servers.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/servers_api.py
--rw-r--r--   0        0        0    11453 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/images/jupyterhub-80.png
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1431d1cef06ad04f5458.woff2
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/169619821ea93019d1bb.woff2
--rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/182712ab85f1472cdb2f.woff
--rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/198a421f279162d59143.woff
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1a05a4887ccb810cb4dd.woff
--rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1f075502d0094a398e21.woff
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/227c93190fe7f82de3f8.woff2
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/249853776d22a271b2b5.woff
--rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/252057e589a0379208ed.woff
--rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/268f264f58eba5c07c88.woff
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3230f9b040f3c630e0c3.woff2
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/32fc45a3d1e8ea11fabc.woff2
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3425a701027d0699e369.woff2
--rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3503ec5cc6330e21f695.woff
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/35b9d6be04b95f0f0530.woff2
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/392a45a84c081c4b412d.woff
--rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3f2b9a42f643e62a49b7.woff
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4777461b144e55145268.woff2
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4df79f684fcbca8386bd.woff
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/50e795c1345353b0e996.woff2
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/5b5f2f31962967dfc22c.woff
--rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/62ced72e5832f02c2796.woff2
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/657896dad292ee9a0a0a.woff
--rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/662bc4c2c037bb0bd529.woff
--rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/666d7a2f9db53cf52e2d.woff
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/6fb9cffb1d3e72bf9293.woff2
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/71a33b6b50457b2c903a.woff2
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/804378952da8a10faae2.woff2
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8472d69545c7409091b4.woff
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/861b791f9de857a6e7bc.woff2
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8ecd7085cfe9bc2c22ac.woff
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9165081d10e1ba601384.woff2
--rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/965aebef74db72eaf236.woff
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9ac81fefbe6c319ea40b.woff2
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/a84892c56152037b3552.woff
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/af4d91666ea345601bea.woff
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/b009a76ad6afe4ebd301.woff2
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/bd9854c751441ccc1a70.woff2
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/be4d02458ce53887dc37.woff2
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1cc6d6fc851b3a2f79d.woff
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1d66054fe23e181d92c.woff
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c35e4c3958e209d17b31.woff2
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c48fb6765a9fcb00b330.woff2
--rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/cad7d3d9cb265e334e58.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d010f1f324e111a22e53.woff2
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d8642a3d1d4ef6179644.woff2
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/db2632771401f61463fe.woff2
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dc7dcec8e3f654e0ed63.woff2
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dfdff8fa12eac629d29f.woff
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/e0e8ba725ebd107367a8.woff
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/eaa367bbd0b333a7f80b.woff
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/ed67ad54b1a8f5d21150.woff2
--rw-r--r--   0        0        0  1060959 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js.LICENSE.txt
--rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f25d774ecfe0996f8eb5.woff2
--rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f52426bf18280380fe67.woff
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f708607d2a7290fb8bfa.woff
--rw-r--r--   0        0        0     8660 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f8a034d72aa6828199d4.woff
--rw-r--r--   0        0        0  1062513 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js.LICENSE.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/images.html
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/page.html
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/servers.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/__init__.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/conftest.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_builder.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_images.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_logs.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/utils.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/package-lock.json
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/package.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts
--rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/admin-linux.png
--rw-r--r--   0        0        0   108741 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-console-linux.png
--rw-r--r--   0        0        0    51218 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png
--rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-list-linux.png
--rw-r--r--   0        0        0    43210 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-remove-confirm-linux.png
--rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-removed-linux.png
--rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environments-page-linux.png
--rw-r--r--   0        0        0    29865 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/login-page-linux.png
--rw-r--r--   0        0        0    25943 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/running-servers-linux.png
--rw-r--r--   0        0        0    41305 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-remove-confirm-linux.png
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-removed-linux.png
--rw-r--r--   0        0        0    49850 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-dialog-linux.png
--rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-page-linux.png
--rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/user-linux.png
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/LICENSE
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/README.md
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/.prettierignore
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/dev-requirements.txt
+-rw-r--r--   0        0        0   279512 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/package-lock.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/package.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/pytest.ini
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tsconfig.json
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/webpack.config.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/AxiosContext.tsx
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/ButtonWithConfirm.tsx
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/JupyterhubContext.ts
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/LoadingAnimation.tsx
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/SmallTextField.tsx
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/axiosclient.ts
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/style.css
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/theme.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/common/utils.ts
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/App.tsx
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/EnvironmentList.tsx
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/LogDialog.tsx
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/NewEnvironmentDialog.tsx
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/RemoveEnvironmentButton.tsx
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/main.tsx
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/environments/types.ts
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/App.tsx
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/NewServerDialog.tsx
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/OpenServerButton.tsx
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/RemoveServerButton.tsx
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/ServersList.tsx
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/main.tsx
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/src/servers/types.ts
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/__main__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/_version.py
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/app.py
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/base.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/binderhub_builder.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/binderhub_log.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/builder.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/dbutil.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/docker.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/environments.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/logs.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/model.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/servers.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/servers_api.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/alembic/alembic.ini
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/alembic/script.py.mako
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/alembic/versions/ac1b4e7e52f3_first_migration.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/database/manager.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/database/model.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/database/schemas.py
+-rw-r--r--   0        0        0    11453 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/images/jupyterhub-80.png
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1431d1cef06ad04f5458.woff2
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/169619821ea93019d1bb.woff2
+-rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/182712ab85f1472cdb2f.woff
+-rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/198a421f279162d59143.woff
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1a05a4887ccb810cb4dd.woff
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1f075502d0094a398e21.woff
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/227c93190fe7f82de3f8.woff2
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/249853776d22a271b2b5.woff
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/252057e589a0379208ed.woff
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/268f264f58eba5c07c88.woff
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3230f9b040f3c630e0c3.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/32fc45a3d1e8ea11fabc.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3425a701027d0699e369.woff2
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3503ec5cc6330e21f695.woff
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/35b9d6be04b95f0f0530.woff2
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/392a45a84c081c4b412d.woff
+-rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3f2b9a42f643e62a49b7.woff
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/4777461b144e55145268.woff2
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/4df79f684fcbca8386bd.woff
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/50e795c1345353b0e996.woff2
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/5b5f2f31962967dfc22c.woff
+-rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/62ced72e5832f02c2796.woff2
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/657896dad292ee9a0a0a.woff
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/662bc4c2c037bb0bd529.woff
+-rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/666d7a2f9db53cf52e2d.woff
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/6fb9cffb1d3e72bf9293.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/71a33b6b50457b2c903a.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/804378952da8a10faae2.woff2
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/8472d69545c7409091b4.woff
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/861b791f9de857a6e7bc.woff2
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/8ecd7085cfe9bc2c22ac.woff
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/9165081d10e1ba601384.woff2
+-rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/965aebef74db72eaf236.woff
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/9ac81fefbe6c319ea40b.woff2
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/a84892c56152037b3552.woff
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/af4d91666ea345601bea.woff
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/bd9854c751441ccc1a70.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/be4d02458ce53887dc37.woff2
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c1cc6d6fc851b3a2f79d.woff
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c1d66054fe23e181d92c.woff
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c35e4c3958e209d17b31.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c48fb6765a9fcb00b330.woff2
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/cad7d3d9cb265e334e58.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/d010f1f324e111a22e53.woff2
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/d8642a3d1d4ef6179644.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/db2632771401f61463fe.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/dc7dcec8e3f654e0ed63.woff2
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/dfdff8fa12eac629d29f.woff
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/e0e8ba725ebd107367a8.woff
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/eaa367bbd0b333a7f80b.woff
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/ed67ad54b1a8f5d21150.woff2
+-rw-r--r--   0        0        0  1062137 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/environments.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/environments.js.LICENSE.txt
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f25d774ecfe0996f8eb5.woff2
+-rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f52426bf18280380fe67.woff
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f708607d2a7290fb8bfa.woff
+-rw-r--r--   0        0        0     8660 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f8a034d72aa6828199d4.woff
+-rw-r--r--   0        0        0  1062999 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/servers.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/servers.js.LICENSE.txt
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/templates/images.html
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/templates/page.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/templates/servers.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/conftest.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/__init__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/conftest.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/test_builder.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/test_images.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/test_logs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/conftest.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/test_builder.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/test_images.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/test_logs.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_config.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/jupyterhub_config_binderhub.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/jupyterhub_config_local.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/package-lock.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/package.json
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/tljh_repo2docker_binderhub.py
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/admin.png
+-rw-r--r--   0        0        0   108741 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-console.png
+-rw-r--r--   0        0        0    51212 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-dialog.png
+-rw-r--r--   0        0        0    29892 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-list.png
+-rw-r--r--   0        0        0    43210 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-remove-confirm.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-removed.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environments-page.png
+-rw-r--r--   0        0        0    29865 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/login-page.png
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/running-servers.png
+-rw-r--r--   0        0        0    42002 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/server-remove-confirm.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/server-removed.png
+-rw-r--r--   0        0        0    49850 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/servers-dialog.png
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/servers-page.png
+-rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/user.png
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/admin.png
+-rw-r--r--   0        0        0   108741 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-console.png
+-rw-r--r--   0        0        0    51218 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png
+-rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-list.png
+-rw-r--r--   0        0        0    43210 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-remove-confirm.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-removed.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environments-page.png
+-rw-r--r--   0        0        0    29865 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/login-page.png
+-rw-r--r--   0        0        0    25943 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/running-servers.png
+-rw-r--r--   0        0        0    41305 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/server-remove-confirm.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/server-removed.png
+-rw-r--r--   0        0        0    49850 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/servers-dialog.png
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/servers-page.png
+-rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/user.png
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/ui-tests/tests/ui.test.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     9474 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a1/PKG-INFO
```

### Comparing `tljh_repo2docker-2.0.0a0/CHANGELOG.md` & `tljh_repo2docker-2.0.0a1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -55,14 +55,38 @@
 - @TimoRoth made their first contribution in https://github.com/plasmabio/tljh-repo2docker/pull/34
 - @yamaton made their first contribution in https://github.com/plasmabio/tljh-repo2docker/pull/61
 
 **Full Changelog**: https://github.com/plasmabio/tljh-repo2docker/commits/v1
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 2.0.0a1
+
+([Full Changelog](https://github.com/plasmabio/tljh-repo2docker/compare/v2.0.0a0...78fe0248148f114c72e4260f42ea1088ab285153))
+
+### Enhancements made
+
+- Adopt `binderhub` [#83](https://github.com/plasmabio/tljh-repo2docker/pull/83) ([@trungleduc](https://github.com/trungleduc))
+
+### Maintenance and upkeep improvements
+
+- Make npm package private [#86](https://github.com/plasmabio/tljh-repo2docker/pull/86) ([@trungleduc](https://github.com/trungleduc))
+
+### Other merged PRs
+
+- Update snapshot [#85](https://github.com/plasmabio/tljh-repo2docker/pull/85) ([@trungleduc](https://github.com/trungleduc))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/plasmabio/tljh-repo2docker/graphs/contributors?from=2024-04-04&to=2024-05-15&type=c))
+
+[@jtpio](https://github.com/search?q=repo%3Aplasmabio%2Ftljh-repo2docker+involves%3Ajtpio+updated%3A2024-04-04..2024-05-15&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Aplasmabio%2Ftljh-repo2docker+involves%3Atrungleduc+updated%3A2024-04-04..2024-05-15&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 2.0.0a0
 
 ([Full Changelog](https://github.com/plasmabio/tljh-repo2docker/compare/v1.0.1...094e4635ca9329ccab20e06eb1c0fefa4b8aa664))
 
 ### Enhancements made
 
 - Start single server from backend [#81](https://github.com/plasmabio/tljh-repo2docker/pull/81) ([@trungleduc](https://github.com/trungleduc))
@@ -75,16 +99,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/plasmabio/tljh-repo2docker/graphs/contributors?from=2024-03-11&to=2024-04-03&type=c))
 
 [@jtpio](https://github.com/search?q=repo%3Aplasmabio%2Ftljh-repo2docker+involves%3Ajtpio+updated%3A2024-03-11..2024-04-03&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Aplasmabio%2Ftljh-repo2docker+involves%3Atrungleduc+updated%3A2024-03-11..2024-04-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.1
 
 ([Full Changelog](https://github.com/plasmabio/tljh-repo2docker/compare/v1.0.0...98eaec34e3617c1e9bb83b2b4b09b2e4866fe8a0))
 
 ### Bugs fixed
 
 - Resolve 'Show Logs' issue by adding \_xsrf token [#61](https://github.com/plasmabio/tljh-repo2docker/pull/61) ([@yamaton](https://github.com/yamaton))
```

### Comparing `tljh_repo2docker-2.0.0a0/CONTRIBUTING.md` & `tljh_repo2docker-2.0.0a1/CONTRIBUTING.md`

 * *Files 7% similar despite different names*

```diff
@@ -42,18 +42,24 @@
 
 ```bash
 docker pull quay.io/jupyterhub/repo2docker:main
 ```
 
 ## Run
 
-Finally, start `jupyterhub` with the config in `debug` mode:
+Finally, start `jupyterhub` with local build backend:
 
 ```bash
-python -m jupyterhub -f jupyterhub_config.py --debug
+python -m jupyterhub -f ui-tests/jupyterhub_config_local.py --debug
+```
+
+or using `binderhub` build backend
+
+```bash
+python -m jupyterhub -f ui-tests/jupyterhub_config_binderhub.py --debug
 ```
 
 Open https://localhost:8000 in a web browser.
 
 ## Tests
 
 Tests are located in the [tests](./tests) folder.
```

### Comparing `tljh_repo2docker-2.0.0a0/jupyterhub_config.py` & `tljh_repo2docker-2.0.0a1/ui-tests/jupyterhub_config_local.py`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/package-lock.json` & `tljh_repo2docker-2.0.0a1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999903288201161%*

 * *Differences: {"'packages'": "{'': {'version': '2.0.0-a1'}}", "'version'": "'2.0.0-a1'"}*

```diff
@@ -40,15 +40,15 @@
                 "ts-loader": "^9.2.6",
                 "typescript": "^5",
                 "webpack": "^5.74.0",
                 "webpack-cli": "^5.1.4"
             },
             "license": "BSD-3-Clause",
             "name": "tljh_repo2docker_ui",
-            "version": "2.0.0-a0"
+            "version": "2.0.0-a1"
         },
         "node_modules/@aashutoshrathi/word-wrap": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==",
@@ -6525,9 +6525,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "2.0.0-a0"
+    "version": "2.0.0-a1"
 }
```

### Comparing `tljh_repo2docker-2.0.0a0/package.json` & `tljh_repo2docker-2.0.0a1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8928571428571429%*

 * *Differences: {"'private'": "'true'", "'version'": "'2.0.0-a1'"}*

```diff
@@ -122,14 +122,15 @@
                     "tabWidth": 4
                 }
             }
         ],
         "singleQuote": true,
         "trailingComma": "none"
     },
+    "private": "true",
     "repository": {
         "type": "git",
         "url": "https://github.com/plasmabio/tljh-repo2docker.git"
     },
     "scripts": {
         "build": "cross-env NODE_ENV=development webpack --config webpack.config.js",
         "build:prod": "cross-env NODE_ENV=production webpack --config webpack.config.js",
@@ -138,9 +139,9 @@
         "eslint:check": "eslint --ext .js,.jsx,.ts,.tsx src/",
         "lint": "npm run prettier && npm run eslint",
         "lint:check": "npm run prettier:check && npm run eslint:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "watch": "cross-env NODE_ENV=development webpack watch --config webpack.config.js"
     },
-    "version": "2.0.0-a0"
+    "version": "2.0.0-a1"
 }
```

### Comparing `tljh_repo2docker-2.0.0a0/tsconfig.json` & `tljh_repo2docker-2.0.0a1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/webpack.config.js` & `tljh_repo2docker-2.0.0a1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/common/ButtonWithConfirm.tsx` & `tljh_repo2docker-2.0.0a1/src/common/ButtonWithConfirm.tsx`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/common/axiosclient.ts` & `tljh_repo2docker-2.0.0a1/src/common/axiosclient.ts`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/common/utils.ts` & `tljh_repo2docker-2.0.0a1/src/common/utils.ts`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/App.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/App.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import { useJupyterhub } from '../common/JupyterhubContext';
 
 export interface IAppProps {
   images: IEnvironmentData[];
   default_cpu_limit: string;
   default_mem_limit: string;
   machine_profiles: IMachineProfile[];
+  use_binderhub: boolean;
+  repo_providers?: { label: string; value: string }[];
 }
 export default function App(props: IAppProps) {
   const jhData = useJupyterhub();
 
   const serviceClient = useMemo(() => {
     const baseUrl = jhData.servicePrefix;
     const xsrfToken = jhData.xsrfToken;
@@ -31,14 +33,16 @@
       <AxiosContext.Provider value={{ serviceClient }}>
         <ScopedCssBaseline>
           <Stack sx={{ padding: 1 }} spacing={1}>
             <NewEnvironmentDialog
               default_cpu_limit={props.default_cpu_limit}
               default_mem_limit={props.default_mem_limit}
               machine_profiles={props.machine_profiles}
+              use_binderhub={props.use_binderhub}
+              repo_providers={props.repo_providers}
             />
             <EnvironmentList {...props} />
           </Stack>
         </ScopedCssBaseline>
       </AxiosContext.Provider>
     </ThemeProvider>
   );
```

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/EnvironmentList.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/EnvironmentList.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
       return params.value === 'built' ? (
         <IconButton>
           <CheckIcon color="success" />
         </IconButton>
       ) : params.value === 'building' ? (
         <EnvironmentLogButton
           name={params.row.display_name}
-          image={params.row.image_name}
+          image={params.row.uid ?? params.row.image_name}
         />
       ) : null;
     }
   },
   {
     field: 'remove',
     headerName: '',
@@ -71,15 +71,15 @@
     filterable: false,
     sortable: false,
     hideable: false,
     renderCell: params => {
       return (
         <RemoveEnvironmentButton
           name={params.row.display_name}
-          image={params.row.image_name}
+          image={params.row.uid ?? params.row.image_name}
         />
       );
     }
   }
 ];
 
 export interface IEnvironmentListProps {
```

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/LogDialog.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/LogDialog.tsx`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,21 +61,21 @@
         console.error('Failed to construct event stream', err);
         eventSource.close();
       };
 
       eventSource.onmessage = event => {
         const data = JSON.parse(event.data);
 
+        terminal.write(data.message);
+        fitAddon.fit();
         if (data.phase === 'built') {
           eventSource.close();
           setBuilt(true);
           return;
         }
-        terminal.write(data.message);
-        fitAddon.fit();
       };
     }
   }, [jhData, props.image]);
   const handleClose = (
     event?: any,
     reason?: 'backdropClick' | 'escapeKeyDown'
   ) => {
```

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/NewEnvironmentDialog.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/NewEnvironmentDialog.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -9,32 +9,42 @@
   FormControl,
   InputLabel,
   MenuItem,
   OutlinedTextFieldProps,
   Select,
   Typography
 } from '@mui/material';
-import { Fragment, memo, useCallback, useMemo, useState } from 'react';
+import {
+  Fragment,
+  memo,
+  useCallback,
+  useEffect,
+  useMemo,
+  useState
+} from 'react';
 
 import { useAxios } from '../common/AxiosContext';
 import { SmallTextField } from '../common/SmallTextField';
 import { ENV_PREFIX } from './types';
 
 export interface IMachineProfile {
   label: string;
   cpu: string;
   memory: string;
 }
 export interface INewEnvironmentDialogProps {
   default_cpu_limit: string;
   default_mem_limit: string;
   machine_profiles: IMachineProfile[];
+  use_binderhub: boolean;
+  repo_providers?: { label: string; value: string }[];
 }
 
 interface IFormValues {
+  provider?: string;
   repo?: string;
   ref?: string;
   name?: string;
   memory?: number;
   cpu?: number;
   buildargs?: string;
   username?: string;
@@ -70,19 +80,61 @@
       setFormValues(old => {
         return { ...old, [key]: value };
       });
     },
     [setFormValues]
   );
   const validated = useMemo(() => {
-    return Boolean(formValues.repo) && Boolean(formValues.ref);
-  }, [formValues]);
+    return Boolean(formValues.repo);
+  }, [formValues.repo]);
 
   const [selectedProfile, setSelectedProfile] = useState<number>(0);
+  const [selectedProvider, setSelectedProvider] = useState<number>(0);
 
+  const onMachineProfileChange = useCallback(
+    (value?: string | number) => {
+      if (value !== undefined) {
+        const index = parseInt(value + '');
+        const selected = props.machine_profiles[index];
+        if (selected !== undefined) {
+          updateFormValue('cpu', selected.cpu + '');
+          updateFormValue('memory', selected.memory + '');
+          setSelectedProfile(index);
+        }
+      }
+    },
+    [props.machine_profiles, updateFormValue]
+  );
+
+  const onRepoProviderChange = useCallback(
+    (value?: string | number) => {
+      if (value !== undefined) {
+        const index = parseInt(value + '');
+        const selected = props.repo_providers?.[index];
+        if (selected !== undefined) {
+          updateFormValue('provider', selected.value);
+          setSelectedProvider(index);
+        }
+      }
+    },
+    [props.repo_providers, updateFormValue]
+  );
+  useEffect(() => {
+    if (props.machine_profiles.length > 0) {
+      onMachineProfileChange(0);
+    }
+    if (props.repo_providers && props.repo_providers.length > 0) {
+      onRepoProviderChange(0);
+    }
+  }, [
+    props.machine_profiles,
+    props.repo_providers,
+    onMachineProfileChange,
+    onRepoProviderChange
+  ]);
   const MemoryCpuSelector = useMemo(() => {
     return (
       <Fragment>
         <SmallTextField
           {...commonInputProps}
           id="mem_limit"
           name="mem_limit"
@@ -116,36 +168,28 @@
         </InputLabel>
         <Select
           labelId="machine-profiles-select-label"
           id="machine-profiles-select"
           value={selectedProfile}
           label="Machine profile"
           size="small"
-          onChange={e => {
-            const value = e.target.value;
-            if (value) {
-              const index = parseInt(value + '');
-              const selected = props.machine_profiles[index];
-              updateFormValue('cpu', selected.cpu + '');
-              updateFormValue('memory', selected.memory + '');
-              setSelectedProfile(index);
-            }
-          }}
+          onChange={e => onMachineProfileChange(e.target.value)}
         >
           {props.machine_profiles.map((it, idx) => {
             return (
               <MenuItem key={idx} value={idx}>
                 {it.label} ({it.cpu} CPU - {it.memory}G Memory)
               </MenuItem>
             );
           })}
         </Select>
       </FormControl>
     );
-  }, [updateFormValue, props.machine_profiles, selectedProfile]);
+  }, [props.machine_profiles, selectedProfile, onMachineProfileChange]);
+
   return (
     <Fragment>
       <Box sx={{ display: 'flex', flexDirection: 'row-reverse' }}>
         <Button onClick={handleOpen} variant="contained">
           Create new environment
         </Button>
       </Box>
@@ -163,14 +207,15 @@
             data.name =
               data.name ??
               (data.repo as string)
                 .replace('http://', '')
                 .replace('https://', '')
                 .replace(/\//g, '-')
                 .replace(/\./g, '-');
+            data.ref = data.ref && data.ref.length > 0 ? data.ref : 'HEAD';
             data.cpu = data.cpu ?? '2';
             data.memory = data.memory ?? '2';
             data.username = data.username ?? '';
             data.password = data.password ?? '';
             const response = await axios.serviceClient.request({
               method: 'post',
               path: ENV_PREFIX,
@@ -182,14 +227,37 @@
               handleClose();
             }
           }
         }}
       >
         <DialogTitle>Create a new environment</DialogTitle>
         <DialogContent>
+          {props.use_binderhub && props.repo_providers && (
+            <FormControl fullWidth sx={{ marginTop: '8px' }}>
+              <InputLabel id="git-provider-select-label">
+                Repository provider
+              </InputLabel>
+              <Select
+                labelId="git-provider-select-label"
+                id="git-provider-select"
+                value={selectedProvider}
+                label="Repository provider"
+                size="small"
+                onChange={e => onRepoProviderChange(e.target.value)}
+              >
+                {props.repo_providers.map((it, idx) => {
+                  return (
+                    <MenuItem key={idx} value={idx}>
+                      {it.label}
+                    </MenuItem>
+                  );
+                })}
+              </Select>
+            </FormControl>
+          )}
           <SmallTextField
             {...commonInputProps}
             id="repo"
             size="small"
             name="repo"
             label="Repository URL"
             type="text"
@@ -200,14 +268,15 @@
             {...commonInputProps}
             id="ref"
             name="ref"
             size="small"
             label="Reference (git commit)"
             type="text"
             placeholder="HEAD"
+            required={false}
             onChange={e => updateFormValue('ref', e.target.value)}
             value={formValues.ref ?? ''}
           />
           <SmallTextField
             {...commonInputProps}
             id="name"
             name="name"
@@ -217,64 +286,72 @@
             required={false}
             placeholder="Example: course-python-101-B37"
             onChange={e => updateFormValue('name', e.target.value)}
           />
           {props.machine_profiles.length > 0
             ? MachineProfileSelector
             : MemoryCpuSelector}
-          <Divider
-            variant="fullWidth"
-            textAlign="left"
-            sx={{ marginTop: '6px' }}
-          >
-            <Typography sx={{ fontWeight: 500, fontSize: '1.4rem' }}>
-              Advanced
-            </Typography>
-          </Divider>
-          <SmallTextField
-            {...commonInputProps}
-            id="build_args"
-            name="build_args"
-            label="Build arguments"
-            type="text"
-            size="small"
-            multiline
-            rows={4}
-            required={false}
-            placeholder="Build arguments in the form of arg1=val1..."
-            onChange={e => updateFormValue('buildargs', e.target.value)}
-          />
-          <Divider
-            variant="fullWidth"
-            textAlign="left"
-            sx={{ marginTop: '6px' }}
-          >
-            <Typography sx={{ fontWeight: 500, fontSize: '1.4rem' }}>
-              Credentials
-            </Typography>
-          </Divider>
-          <SmallTextField
-            {...commonInputProps}
-            id="git_user"
-            name="git_user"
-            size="small"
-            label="Git user name"
-            type="text"
-            required={false}
-            onChange={e => updateFormValue('username', e.target.value)}
-          />
-          <SmallTextField
-            {...commonInputProps}
-            id="git_password"
-            name="git_password"
-            size="small"
-            label="Git password"
-            type="password"
-            required={false}
-          />
+          {!props.use_binderhub && (
+            <Fragment>
+              <Divider
+                variant="fullWidth"
+                textAlign="left"
+                sx={{ marginTop: '6px' }}
+              >
+                <Typography sx={{ fontWeight: 500, fontSize: '1.4rem' }}>
+                  Advanced
+                </Typography>
+              </Divider>
+              <SmallTextField
+                {...commonInputProps}
+                id="build_args"
+                name="build_args"
+                label="Build arguments"
+                type="text"
+                size="small"
+                multiline
+                rows={4}
+                required={false}
+                placeholder="Build arguments in the form of arg1=val1..."
+                onChange={e => updateFormValue('buildargs', e.target.value)}
+              />
+            </Fragment>
+          )}
+          {!props.use_binderhub && (
+            <Fragment>
+              <Divider
+                variant="fullWidth"
+                textAlign="left"
+                sx={{ marginTop: '6px' }}
+              >
+                <Typography sx={{ fontWeight: 500, fontSize: '1.4rem' }}>
+                  Credentials
+                </Typography>
+              </Divider>
+              <SmallTextField
+                {...commonInputProps}
+                id="git_user"
+                name="git_user"
+                size="small"
+                label="Git user name"
+                type="text"
+                required={false}
+                onChange={e => updateFormValue('username', e.target.value)}
+              />
+              <SmallTextField
+                {...commonInputProps}
+                id="git_password"
+                name="git_password"
+                size="small"
+                label="Git password"
+                type="password"
+                required={false}
+              />
+            </Fragment>
+          )}
         </DialogContent>
         <DialogActions>
           <Button variant="contained" color="error" onClick={handleClose}>
             Cancel
           </Button>
           <Button
             variant="contained"
```

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/RemoveEnvironmentButton.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/RemoveEnvironmentButton.tsx`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/environments/main.tsx` & `tljh_repo2docker-2.0.0a1/src/environments/main.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 if (rootElement) {
   const root = createRoot(rootElement);
   const dataElement = document.getElementById('tljh-page-data');
   let configData: IAppProps = {
     images: [],
     default_cpu_limit: '2',
     default_mem_limit: '2G',
-    machine_profiles: []
+    machine_profiles: [],
+    use_binderhub: false
   };
   if (dataElement) {
     configData = JSON.parse(dataElement.textContent || '') as IAppProps;
   }
   const jhData = (window as any).jhdata;
   const {
     base_url,
```

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/App.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/App.tsx`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/NewServerDialog.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/NewServerDialog.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         setRowSelectionModel(selected);
       }
     },
     [setRowSelectionModel]
   );
 
   const createServer = useCallback(async () => {
-    const imageName = props.images[rowSelectionModel[0] as number].image_name;
+    const imageData = props.images[rowSelectionModel[0] as number];
+    const imageName = imageData.uid ?? imageData.image_name;
     const data: { [key: string]: string } = {
       imageName,
       userName: jhData.user,
       serverName
     };
     try {
       setLoading(true);
```

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/OpenServerButton.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/OpenServerButton.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { Button } from '@mui/material';
-import { Fragment, memo, useCallback } from 'react';
+import { Fragment, memo, useCallback, useMemo } from 'react';
 
 import { useAxios } from '../common/AxiosContext';
 import { useJupyterhub } from '../common/JupyterhubContext';
 import { SERVER_PREFIX } from './types';
 
 interface IOpenServerButton {
   url: string;
@@ -32,18 +32,22 @@
       window.open(props.url, '_blank')?.focus();
       window.location.reload();
     } catch (e: any) {
       console.error(e);
     }
   }, [props, axios, jhData]);
 
+  const pendingUrl = useMemo(() => {
+    const url = props.url.replace('user', 'hub/spawn-pending');
+    return url.endsWith('/') ? url.slice(0, -1) : url;
+  }, [props.url]);
   return (
     <Fragment>
       {props.active && (
-        <Button href={props.url} target="_blank">
+        <Button href={pendingUrl} target="_blank">
           Open Server
         </Button>
       )}
 
       {!props.active && <Button onClick={createServer}>Launch server</Button>}
     </Fragment>
   );
```

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/RemoveServerButton.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/RemoveServerButton.tsx`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/ServersList.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/ServersList.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     sortable: false,
     hideable: false,
     renderCell: params => {
       return (
         <OpenServerButton
           url={params.row.url}
           serverName={params.row.name}
-          imageName={params.row.image}
+          imageName={params.row.uid ?? params.row.image}
           active={params.row.active}
         />
       );
     }
   }
 ];
 
@@ -82,15 +82,17 @@
   const rows = useMemo(() => {
     let servers = [...props.servers];
     if (props.defaultServer.active) {
       servers = [props.defaultServer, ...servers];
     }
     const allServers = servers.map((it, id) => {
       const newItem: any = { ...it, id };
-      newItem.image = it.user_options.image ?? '';
+      newItem.image =
+        it.user_options?.display_name ?? it.user_options.image ?? '';
+      newItem.uid = it.user_options?.uid ?? null;
       newItem.last_activity = formatTime(newItem.last_activity);
       return newItem;
     });
 
     return allServers;
   }, [props]);
   return (
```

### Comparing `tljh_repo2docker-2.0.0a0/src/servers/main.tsx` & `tljh_repo2docker-2.0.0a1/src/servers/main.tsx`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/__init__.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from aiodocker import Docker
 from dockerspawner import DockerSpawner
 from jinja2 import BaseLoader, Environment
 from jupyter_client.localinterfaces import public_ips
 from jupyterhub.traitlets import ByteSpecification
-from tljh.configurer import load_config
-from tljh.hooks import hookimpl
 from traitlets import Unicode
 from traitlets.config import Configurable
 
+try:
+    from tljh.hooks import hookimpl
+except ModuleNotFoundError:
+    hookimpl = None
+
 from .docker import list_images
 
 # Default CPU period
 # See: https://docs.docker.com/config/containers/resource_constraints/#limit-a-containers-access-to-memory#configure-the-default-cfs-scheduler
 CPU_PERIOD = 100_000
 
 TLJH_R2D_ADMIN_SCOPE = "custom:tljh_repo2docker:admin"
@@ -93,15 +96,18 @@
         """
         return await list_images()
 
     async def get_options_form(self):
         """
         Override the default form to handle the case when there is only one image.
         """
-        images = await self.list_images()
+        try:
+            images = await self.list_images()
+        except ValueError:
+            images = []
 
         # make default limits human readable
         default_mem_limit = self.mem_limit
         if isinstance(default_mem_limit, (float, int)):
             # default memory unit is in GB
             default_mem_limit /= ByteSpecification.UNIT_SUFFIXES["G"]
             if float(default_mem_limit).is_integer():
@@ -156,23 +162,28 @@
     """
 
     async def start(self, *args, **kwargs):
         await self.set_limits()
         return await super().start(*args, **kwargs)
 
 
-@hookimpl
-def tljh_custom_jupyterhub_config(c):
-    # hub
-    c.JupyterHub.hub_ip = public_ips()[0]
-    c.JupyterHub.cleanup_servers = False
-    c.JupyterHub.spawner_class = Repo2DockerSpawner
-
-    # spawner
-    c.DockerSpawner.cmd = ["jupyterhub-singleuser"]
-    c.DockerSpawner.pull_policy = "Never"
-    c.DockerSpawner.remove = True
-
-
-@hookimpl
-def tljh_extra_hub_pip_packages():
-    return ["dockerspawner~=0.11", "jupyter_client>=6.1,<8", "aiodocker~=0.19"]
+if hookimpl:
+
+    @hookimpl
+    def tljh_custom_jupyterhub_config(c):
+        # hub
+        c.JupyterHub.hub_ip = public_ips()[0]
+        c.JupyterHub.cleanup_servers = False
+        c.JupyterHub.spawner_class = Repo2DockerSpawner
+
+        # spawner
+        c.DockerSpawner.cmd = ["jupyterhub-singleuser"]
+        c.DockerSpawner.pull_policy = "Never"
+        c.DockerSpawner.remove = True
+
+    @hookimpl
+    def tljh_extra_hub_pip_packages():
+        return ["dockerspawner~=0.11", "jupyter_client>=6.1,<8", "aiodocker~=0.19"]
+
+else:
+    tljh_custom_jupyterhub_config = None
+    tljh_extra_hub_pip_packages = None
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/app.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import logging
 import os
 import socket
 import typing as tp
 from pathlib import Path
+from urllib.parse import urlparse
 
 from jinja2 import Environment, PackageLoader
 from jupyterhub.app import DATA_FILES_PATH
 from jupyterhub.handlers.static import LogoHandler
 from jupyterhub.utils import url_path_join
 from tornado import ioloop, web
 from traitlets import Dict, Int, List, Unicode, default, validate
 from traitlets.config.application import Application
 
+from .binderhub_builder import BinderHubBuildHandler
+from .binderhub_log import BinderHubLogsHandler
 from .builder import BuildHandler
+from .database.manager import ImagesDatabaseManager
+from .dbutil import async_session_context_factory, sync_to_async_url, upgrade_if_needed
 from .environments import EnvironmentsHandler
 from .logs import LogsHandler
 from .servers import ServersHandler
 from .servers_api import ServersAPIHandler
 
 if os.environ.get("JUPYTERHUB_API_TOKEN"):
     from jupyterhub.services.auth import HubOAuthCallbackHandler
@@ -114,24 +119,62 @@
     default_memory_limit = Unicode(
         None,
         config=True,
         help="Default Memory limit.",
         allow_none=True,
     )
 
+    db_url = Unicode(
+        "sqlite:///tljh_repo2docker.sqlite",
+        help="url for the database.",
+        config=True,
+    )
+
+    config_file = Unicode(
+        "tljh_repo2docker_config.py",
+        help="""
+        Config file to load.
+
+        If a relative path is provided, it is taken relative to current directory
+        """,
+        config=True,
+    )
+
+    binderhub_url = Unicode(
+        None, help="URL of the binderhub service.", allow_none=True, config=True
+    )
+
+    repo_providers = List(
+        default_value=[
+            {"label": "Git", "value": "git"},
+        ],
+        trait=Dict,
+        help="""
+        Dict of available repo providers in the form of {"label":"value"}.
+        The references are taken from the binderhub documentation
+        """,
+        config=True,
+    )
+
     aliases = {
         "port": "TljhRepo2Docker.port",
         "ip": "TljhRepo2Docker.ip",
+        "config": "TljhRepo2Docker.config_file",
         "default_memory_limit": "TljhRepo2Docker.default_memory_limit",
         "default_cpu_limit": "TljhRepo2Docker.default_cpu_limit",
         "machine_profiles": "TljhRepo2Docker.machine_profiles",
+        "binderhub_url": "TljhRepo2Docker.binderhub_url",
+        "db_url": "TljhRepo2Docker.db_url",
     }
 
     def init_settings(self) -> tp.Dict:
         """Initialize settings for the service application."""
+
+        self.load_config_file(self.config_file)
+
         static_path = DATA_FILES_PATH + "/static/"
         static_url_prefix = self.service_prefix + "static/"
         env_opt = {"autoescape": True}
 
         env = Environment(
             loader=PackageLoader("tljh_repo2docker"),
             **env_opt,
@@ -146,15 +189,21 @@
             cookie_secret=os.urandom(32),
             base_url=self.base_url,
             hub_prefix=url_path_join(self.base_url, "/hub/"),
             service_prefix=self.service_prefix,
             default_mem_limit=self.default_memory_limit,
             default_cpu_limit=self.default_cpu_limit,
             machine_profiles=self.machine_profiles,
+            binderhub_url=self.binderhub_url,
+            repo_providers=self.repo_providers,
         )
+        if hasattr(self, "db_context"):
+            settings["db_context"] = self.db_context
+        if hasattr(self, "image_db_manager"):
+            settings["image_db_manager"] = self.image_db_manager
         return settings
 
     def init_handlers(self) -> tp.List:
         """Initialize handlers for service application."""
         handlers = []
         static_path = str(HERE / "static")
         server_url = url_path_join(self.service_prefix, r"servers")
@@ -180,38 +229,82 @@
                     url_path_join(self.service_prefix, r"api/servers"),
                     ServersAPIHandler,
                 ),
                 (
                     url_path_join(self.service_prefix, r"environments"),
                     EnvironmentsHandler,
                 ),
-                (url_path_join(self.service_prefix, r"api/environments"), BuildHandler),
-                (
-                    url_path_join(
-                        self.service_prefix, r"api/environments/([^/]+)/logs"
-                    ),
-                    LogsHandler,
-                ),
             ]
         )
-
+        if self.binderhub_url:
+            handlers.extend(
+                [
+                    (
+                        url_path_join(
+                            self.service_prefix, r"api/environments/([^/]+)/logs"
+                        ),
+                        BinderHubLogsHandler,
+                    ),
+                    (
+                        url_path_join(self.service_prefix, r"api/environments"),
+                        BinderHubBuildHandler,
+                    ),
+                ]
+            )
+        else:
+            handlers.extend(
+                [
+                    (
+                        url_path_join(
+                            self.service_prefix, r"api/environments/([^/]+)/logs"
+                        ),
+                        LogsHandler,
+                    ),
+                    (
+                        url_path_join(self.service_prefix, r"api/environments"),
+                        BuildHandler,
+                    ),
+                ]
+            )
         return handlers
 
+    def init_db(self):
+        async_db_url = sync_to_async_url(self.db_url)
+        urlinfo = urlparse(async_db_url)
+        if urlinfo.password:
+            # avoid logging the database password
+            urlinfo = urlinfo._replace(
+                netloc=f"{urlinfo.username}:[redacted]@{urlinfo.hostname}:{urlinfo.port}"
+            )
+            db_log_url = urlinfo.geturl()
+        else:
+            db_log_url = async_db_url
+        self.log.info("Connecting to db: %s", db_log_url)
+        upgrade_if_needed(async_db_url, log=self.log)
+        try:
+            self.db_context = async_session_context_factory(async_db_url)
+        except Exception:
+            self.log.error("Failed to connect to db: %s", db_log_url)
+            self.log.debug("Database error was:", exc_info=True)
+
+        self.image_db_manager = ImagesDatabaseManager()
+
     def make_app(self) -> web.Application:
         """Create the tornado web application.
         Returns:
             The tornado web application.
         """
 
         application = web.Application()
         application.listen(self.port, self.ip)
         return application
 
     def start(self):
         """Start the server."""
+        self.init_db()
         settings = self.init_settings()
 
         self.app = web.Application(**settings)
         self.app.settings.update(self.tornado_settings)
         handlers = self.init_handlers()
         self.app.add_handlers(".*$", handlers)
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/builder.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/builder.py`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/docker.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/docker.py`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/logs.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/logs.py`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/model.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/model.py`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/servers_api.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/servers_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,45 @@
+from uuid import UUID
+
 from jupyterhub.utils import url_path_join
 from tornado import web
 
 from .base import BaseHandler
 
 
 class ServersAPIHandler(BaseHandler):
     """
     Handler to manage single servers
     """
 
     @web.authenticated
     async def post(self):
         data = self.get_json_body()
-        image_name = data.get("imageName", None)
+
+        image_name_or_uid = data.get("imageName", None)
         user_name = data.get("userName", None)
         server_name = data.get("serverName", "")
         if user_name != self.current_user["name"]:
             raise web.HTTPError(403, "Unauthorized")
-        if not image_name:
+        if not image_name_or_uid:
             raise web.HTTPError(400, "Missing image name")
 
+        if self.use_binderhub:
+            db_context, image_db_manager = self.get_db_handlers()
+            if not db_context or not image_db_manager:
+                raise web.HTTPError(500, "Server error, missing database")
+
+            async with db_context() as db:
+                image = await image_db_manager.read(db, UUID(image_name_or_uid))
+                if not image:
+                    raise web.HTTPError(404, "Image not found")
+                image_name = image.name
+        else:
+            image_name = image_name_or_uid
+
         post_data = {"image": image_name}
 
         path = ""
         if len(server_name) > 0:
             path = url_path_join("users", user_name, "servers", server_name)
         else:
             path = url_path_join("users", user_name, "server")
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/images/jupyterhub-80.png` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/images/jupyterhub-80.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1431d1cef06ad04f5458.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1431d1cef06ad04f5458.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/169619821ea93019d1bb.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/169619821ea93019d1bb.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/182712ab85f1472cdb2f.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/182712ab85f1472cdb2f.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/198a421f279162d59143.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/198a421f279162d59143.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1a05a4887ccb810cb4dd.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1a05a4887ccb810cb4dd.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1f075502d0094a398e21.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/1f075502d0094a398e21.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/227c93190fe7f82de3f8.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/227c93190fe7f82de3f8.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/249853776d22a271b2b5.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/249853776d22a271b2b5.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/252057e589a0379208ed.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/252057e589a0379208ed.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/268f264f58eba5c07c88.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/268f264f58eba5c07c88.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3230f9b040f3c630e0c3.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3230f9b040f3c630e0c3.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/32fc45a3d1e8ea11fabc.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/32fc45a3d1e8ea11fabc.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3425a701027d0699e369.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3425a701027d0699e369.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3503ec5cc6330e21f695.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3503ec5cc6330e21f695.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/35b9d6be04b95f0f0530.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/35b9d6be04b95f0f0530.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/392a45a84c081c4b412d.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/392a45a84c081c4b412d.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3f2b9a42f643e62a49b7.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/3f2b9a42f643e62a49b7.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4777461b144e55145268.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/4777461b144e55145268.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4df79f684fcbca8386bd.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/4df79f684fcbca8386bd.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/50e795c1345353b0e996.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/50e795c1345353b0e996.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/5b5f2f31962967dfc22c.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/5b5f2f31962967dfc22c.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/62ced72e5832f02c2796.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/62ced72e5832f02c2796.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/657896dad292ee9a0a0a.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/657896dad292ee9a0a0a.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/662bc4c2c037bb0bd529.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/662bc4c2c037bb0bd529.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/666d7a2f9db53cf52e2d.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/666d7a2f9db53cf52e2d.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/6fb9cffb1d3e72bf9293.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/6fb9cffb1d3e72bf9293.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/71a33b6b50457b2c903a.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/71a33b6b50457b2c903a.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/804378952da8a10faae2.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/804378952da8a10faae2.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8472d69545c7409091b4.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/8472d69545c7409091b4.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/861b791f9de857a6e7bc.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/861b791f9de857a6e7bc.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8ecd7085cfe9bc2c22ac.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/8ecd7085cfe9bc2c22ac.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9165081d10e1ba601384.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/9165081d10e1ba601384.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/965aebef74db72eaf236.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/965aebef74db72eaf236.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9ac81fefbe6c319ea40b.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/9ac81fefbe6c319ea40b.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/a84892c56152037b3552.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/a84892c56152037b3552.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/af4d91666ea345601bea.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/af4d91666ea345601bea.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/b009a76ad6afe4ebd301.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/b009a76ad6afe4ebd301.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/bd9854c751441ccc1a70.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/bd9854c751441ccc1a70.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/be4d02458ce53887dc37.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/be4d02458ce53887dc37.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1cc6d6fc851b3a2f79d.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c1cc6d6fc851b3a2f79d.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1d66054fe23e181d92c.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c1d66054fe23e181d92c.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c35e4c3958e209d17b31.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c35e4c3958e209d17b31.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c48fb6765a9fcb00b330.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/c48fb6765a9fcb00b330.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/cad7d3d9cb265e334e58.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/cad7d3d9cb265e334e58.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d010f1f324e111a22e53.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/d010f1f324e111a22e53.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d8642a3d1d4ef6179644.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/d8642a3d1d4ef6179644.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/db2632771401f61463fe.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/db2632771401f61463fe.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dc7dcec8e3f654e0ed63.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/dc7dcec8e3f654e0ed63.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dfdff8fa12eac629d29f.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/dfdff8fa12eac629d29f.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/e0e8ba725ebd107367a8.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/e0e8ba725ebd107367a8.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/eaa367bbd0b333a7f80b.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/eaa367bbd0b333a7f80b.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/ed67ad54b1a8f5d21150.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/ed67ad54b1a8f5d21150.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/environments.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -43309,16 +43309,15 @@
                                 c = c + e + "_xsrf=" + i
                             }
                             const u = new EventSource(c);
                             u.onerror = e => {
                                 console.error("Failed to construct event stream", e), u.close()
                             }, u.onmessage = e => {
                                 const r = JSON.parse(e.data);
-                                if ("built" === r.phase) return u.close(), void s(!0);
-                                t.write(r.message), n.fit()
+                                if (t.write(r.message), n.fit(), "built" === r.phase) return u.close(), void s(!0)
                             }
                         }
                     }), [r, e.image]),
                     u = (e, t) => {
                         t && "backdropClick" === t || (l.current.terminal.dispose(), a.current && (a.current.innerHTML = ""), o(!1))
                     };
                 return (0, t.jsxs)(x.Fragment, {
@@ -43395,33 +43394,39 @@
                 headerName: "CPU Limit",
                 width: 100
             }, {
                 field: "status",
                 headerName: "Status",
                 width: 100,
                 hideSortIcons: !0,
-                renderCell: e => "built" === e.value ? (0, t.jsx)(ft, {
-                    children: (0, t.jsx)(Vy.A, {
-                        color: "success"
-                    })
-                }) : "building" === e.value ? (0, t.jsx)(SC, {
-                    name: e.row.display_name,
-                    image: e.row.image_name
-                }) : null
+                renderCell: e => {
+                    var r;
+                    return "built" === e.value ? (0, t.jsx)(ft, {
+                        children: (0, t.jsx)(Vy.A, {
+                            color: "success"
+                        })
+                    }) : "building" === e.value ? (0, t.jsx)(SC, {
+                        name: e.row.display_name,
+                        image: null !== (r = e.row.uid) && void 0 !== r ? r : e.row.image_name
+                    }) : null
+                }
             }, {
                 field: "remove",
                 headerName: "",
                 width: 100,
                 filterable: !1,
                 sortable: !1,
                 hideable: !1,
-                renderCell: e => (0, t.jsx)(gC, {
-                    name: e.row.display_name,
-                    image: e.row.image_name
-                })
+                renderCell: e => {
+                    var r;
+                    return (0, t.jsx)(gC, {
+                        name: e.row.display_name,
+                        image: null !== (r = e.row.uid) && void 0 !== r ? r : e.row.image_name
+                    })
+                }
             }],
             AC = (0, x.memo)((function(e) {
                 var r, n;
                 const o = (0, x.useMemo)((() => e.images.map(((t, r) => {
                     var n, o;
                     const i = {
                         ...t,
@@ -43489,17 +43494,36 @@
                     [l, c] = (0, x.useState)({}),
                     u = (0, x.useCallback)(((e, t) => {
                         c((r => ({
                             ...r,
                             [e]: t
                         })))
                     }), [c]),
-                    d = (0, x.useMemo)((() => Boolean(l.repo) && Boolean(l.ref)), [l]),
+                    d = (0, x.useMemo)((() => Boolean(l.repo)), [l.repo]),
                     [h, f] = (0, x.useState)(0),
-                    p = (0, x.useMemo)((() => (0, t.jsxs)(x.Fragment, {
+                    [p, m] = (0, x.useState)(0),
+                    g = (0, x.useCallback)((t => {
+                        if (void 0 !== t) {
+                            const r = parseInt(t + ""),
+                                n = e.machine_profiles[r];
+                            void 0 !== n && (u("cpu", n.cpu + ""), u("memory", n.memory + ""), f(r))
+                        }
+                    }), [e.machine_profiles, u]),
+                    v = (0, x.useCallback)((t => {
+                        var r;
+                        if (void 0 !== t) {
+                            const n = parseInt(t + ""),
+                                o = null === (r = e.repo_providers) || void 0 === r ? void 0 : r[n];
+                            void 0 !== o && (u("provider", o.value), m(n))
+                        }
+                    }), [e.repo_providers, u]);
+                (0, x.useEffect)((() => {
+                    e.machine_profiles.length > 0 && g(0), e.repo_providers && e.repo_providers.length > 0 && v(0)
+                }), [e.machine_profiles, e.repo_providers, g, v]);
+                const b = (0, x.useMemo)((() => (0, t.jsxs)(x.Fragment, {
                         children: [(0, t.jsx)(kC, {
                             ...RC,
                             id: "mem_limit",
                             name: "mem_limit",
                             label: "Memory limit (GB)",
                             size: "small",
                             type: "number",
@@ -43514,42 +43538,35 @@
                             label: "CPU limit (number of cores)",
                             type: "number",
                             helperText: "If empty, defaults to 2 cores",
                             required: !1,
                             onChange: e => u("cpu", e.target.value)
                         })]
                     })), [u]),
-                    m = (0, x.useMemo)((() => (0, t.jsxs)(Uv, {
+                    y = (0, x.useMemo)((() => (0, t.jsxs)(Uv, {
                         fullWidth: !0,
                         sx: {
                             marginTop: "8px"
                         },
                         children: [(0, t.jsx)($v, {
                             id: "machine-profiles-select-label",
                             children: "Machine profile"
                         }), (0, t.jsx)(vp, {
                             labelId: "machine-profiles-select-label",
                             id: "machine-profiles-select",
                             value: h,
                             label: "Machine profile",
                             size: "small",
-                            onChange: t => {
-                                const r = t.target.value;
-                                if (r) {
-                                    const t = parseInt(r + ""),
-                                        n = e.machine_profiles[t];
-                                    u("cpu", n.cpu + ""), u("memory", n.memory + ""), f(t)
-                                }
-                            },
+                            onChange: e => g(e.target.value),
                             children: e.machine_profiles.map(((e, r) => (0, t.jsxs)(Nu, {
                                 value: r,
                                 children: [e.label, " (", e.cpu, " CPU - ", e.memory, "G Memory)"]
                             }, r)))
                         })]
-                    })), [u, e.machine_profiles, h]);
+                    })), [e.machine_profiles, h, g]);
                 return (0, t.jsxs)(x.Fragment, {
                     children: [(0, t.jsx)(Jy, {
                         sx: {
                             display: "flex",
                             flexDirection: "row-reverse"
                         },
                         children: (0, t.jsx)(vb, {
@@ -43568,27 +43585,47 @@
                             component: "form",
                             onSubmit: async e => {
                                 var t, r, n, i, s;
                                 e.preventDefault();
                                 const c = {
                                     ...l
                                 };
-                                c.repo = c.repo.trim(), c.name = null !== (t = c.name) && void 0 !== t ? t : c.repo.replace("http://", "").replace("https://", "").replace(/\//g, "-").replace(/\./g, "-"), c.cpu = null !== (r = c.cpu) && void 0 !== r ? r : "2", c.memory = null !== (n = c.memory) && void 0 !== n ? n : "2", c.username = null !== (i = c.username) && void 0 !== i ? i : "", c.password = null !== (s = c.password) && void 0 !== s ? s : "";
+                                c.repo = c.repo.trim(), c.name = null !== (t = c.name) && void 0 !== t ? t : c.repo.replace("http://", "").replace("https://", "").replace(/\//g, "-").replace(/\./g, "-"), c.ref = c.ref && c.ref.length > 0 ? c.ref : "HEAD", c.cpu = null !== (r = c.cpu) && void 0 !== r ? r : "2", c.memory = null !== (n = c.memory) && void 0 !== n ? n : "2", c.username = null !== (i = c.username) && void 0 !== i ? i : "", c.password = null !== (s = c.password) && void 0 !== s ? s : "";
                                 const u = await o.serviceClient.request({
                                     method: "post",
                                     path: mC,
                                     data: c
                                 });
                                 "ok" === (null == u ? void 0 : u.status) ? window.location.reload(): a()
                             }
                         },
                         children: [(0, t.jsx)(hC, {
                             children: "Create a new environment"
                         }), (0, t.jsxs)(cC, {
-                            children: [(0, t.jsx)(kC, {
+                            children: [e.use_binderhub && e.repo_providers && (0, t.jsxs)(Uv, {
+                                fullWidth: !0,
+                                sx: {
+                                    marginTop: "8px"
+                                },
+                                children: [(0, t.jsx)($v, {
+                                    id: "git-provider-select-label",
+                                    children: "Repository provider"
+                                }), (0, t.jsx)(vp, {
+                                    labelId: "git-provider-select-label",
+                                    id: "git-provider-select",
+                                    value: p,
+                                    label: "Repository provider",
+                                    size: "small",
+                                    onChange: e => v(e.target.value),
+                                    children: e.repo_providers.map(((e, r) => (0, t.jsx)(Nu, {
+                                        value: r,
+                                        children: e.label
+                                    }, r)))
+                                })]
+                            }), (0, t.jsx)(kC, {
                                 ...RC,
                                 id: "repo",
                                 size: "small",
                                 name: "repo",
                                 label: "Repository URL",
                                 type: "text",
                                 onChange: e => u("repo", e.target.value),
@@ -43597,81 +43634,86 @@
                                 ...RC,
                                 id: "ref",
                                 name: "ref",
                                 size: "small",
                                 label: "Reference (git commit)",
                                 type: "text",
                                 placeholder: "HEAD",
+                                required: !1,
                                 onChange: e => u("ref", e.target.value),
                                 value: null !== (n = l.ref) && void 0 !== n ? n : ""
                             }), (0, t.jsx)(kC, {
                                 ...RC,
                                 id: "name",
                                 name: "name",
                                 size: "small",
                                 label: "Environment name",
                                 type: "text",
                                 required: !1,
                                 placeholder: "Example: course-python-101-B37",
                                 onChange: e => u("name", e.target.value)
-                            }), e.machine_profiles.length > 0 ? m : p, (0, t.jsx)(qg, {
-                                variant: "fullWidth",
-                                textAlign: "left",
-                                sx: {
-                                    marginTop: "6px"
-                                },
-                                children: (0, t.jsx)(Mm, {
+                            }), e.machine_profiles.length > 0 ? y : b, !e.use_binderhub && (0, t.jsxs)(x.Fragment, {
+                                children: [(0, t.jsx)(qg, {
+                                    variant: "fullWidth",
+                                    textAlign: "left",
                                     sx: {
-                                        fontWeight: 500,
-                                        fontSize: "1.4rem"
+                                        marginTop: "6px"
                                     },
-                                    children: "Advanced"
-                                })
-                            }), (0, t.jsx)(kC, {
-                                ...RC,
-                                id: "build_args",
-                                name: "build_args",
-                                label: "Build arguments",
-                                type: "text",
-                                size: "small",
-                                multiline: !0,
-                                rows: 4,
-                                required: !1,
-                                placeholder: "Build arguments in the form of arg1=val1...",
-                                onChange: e => u("buildargs", e.target.value)
-                            }), (0, t.jsx)(qg, {
-                                variant: "fullWidth",
-                                textAlign: "left",
-                                sx: {
-                                    marginTop: "6px"
-                                },
-                                children: (0, t.jsx)(Mm, {
+                                    children: (0, t.jsx)(Mm, {
+                                        sx: {
+                                            fontWeight: 500,
+                                            fontSize: "1.4rem"
+                                        },
+                                        children: "Advanced"
+                                    })
+                                }), (0, t.jsx)(kC, {
+                                    ...RC,
+                                    id: "build_args",
+                                    name: "build_args",
+                                    label: "Build arguments",
+                                    type: "text",
+                                    size: "small",
+                                    multiline: !0,
+                                    rows: 4,
+                                    required: !1,
+                                    placeholder: "Build arguments in the form of arg1=val1...",
+                                    onChange: e => u("buildargs", e.target.value)
+                                })]
+                            }), !e.use_binderhub && (0, t.jsxs)(x.Fragment, {
+                                children: [(0, t.jsx)(qg, {
+                                    variant: "fullWidth",
+                                    textAlign: "left",
                                     sx: {
-                                        fontWeight: 500,
-                                        fontSize: "1.4rem"
+                                        marginTop: "6px"
                                     },
-                                    children: "Credentials"
-                                })
-                            }), (0, t.jsx)(kC, {
-                                ...RC,
-                                id: "git_user",
-                                name: "git_user",
-                                size: "small",
-                                label: "Git user name",
-                                type: "text",
-                                required: !1,
-                                onChange: e => u("username", e.target.value)
-                            }), (0, t.jsx)(kC, {
-                                ...RC,
-                                id: "git_password",
-                                name: "git_password",
-                                size: "small",
-                                label: "Git password",
-                                type: "password",
-                                required: !1
+                                    children: (0, t.jsx)(Mm, {
+                                        sx: {
+                                            fontWeight: 500,
+                                            fontSize: "1.4rem"
+                                        },
+                                        children: "Credentials"
+                                    })
+                                }), (0, t.jsx)(kC, {
+                                    ...RC,
+                                    id: "git_user",
+                                    name: "git_user",
+                                    size: "small",
+                                    label: "Git user name",
+                                    type: "text",
+                                    required: !1,
+                                    onChange: e => u("username", e.target.value)
+                                }), (0, t.jsx)(kC, {
+                                    ...RC,
+                                    id: "git_password",
+                                    name: "git_password",
+                                    size: "small",
+                                    label: "Git password",
+                                    type: "password",
+                                    required: !1
+                                })]
                             })]
                         }), (0, t.jsxs)(nC, {
                             children: [(0, t.jsx)(vb, {
                                 variant: "contained",
                                 color: "error",
                                 onClick: a,
                                 children: "Cancel"
@@ -43690,15 +43732,16 @@
         if (MC) {
             const e = (0, S.H)(MC),
                 r = document.getElementById("tljh-page-data");
             let n = {
                 images: [],
                 default_cpu_limit: "2",
                 default_mem_limit: "2G",
-                machine_profiles: []
+                machine_profiles: [],
+                use_binderhub: !1
             };
             r && (n = JSON.parse(r.textContent || ""));
             const o = window.jhdata,
                 {
                     base_url: i,
                     xsrf_token: s,
                     user: a,
@@ -43736,15 +43779,17 @@
                                     sx: {
                                         padding: 1
                                     },
                                     spacing: 1,
                                     children: [(0, t.jsx)(EC, {
                                         default_cpu_limit: e.default_cpu_limit,
                                         default_mem_limit: e.default_mem_limit,
-                                        machine_profiles: e.machine_profiles
+                                        machine_profiles: e.machine_profiles,
+                                        use_binderhub: e.use_binderhub,
+                                        repo_providers: e.repo_providers
                                     }), (0, t.jsx)(AC, {
                                         ...e
                                     })]
                                 })
                             })
                         })
                     })
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js.LICENSE.txt` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/environments.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f25d774ecfe0996f8eb5.woff2` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f25d774ecfe0996f8eb5.woff2`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f52426bf18280380fe67.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f52426bf18280380fe67.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f708607d2a7290fb8bfa.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f708607d2a7290fb8bfa.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f8a034d72aa6828199d4.woff` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/f8a034d72aa6828199d4.woff`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/servers.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -43304,18 +43304,22 @@
                                 method: "post",
                                 path: pS,
                                 data: o
                             }), null === (t = window.open(e.url, "_blank")) || void 0 === t || t.focus(), window.location.reload()
                         } catch (e) {
                             console.error(e)
                         }
-                    }), [e, r, n]);
+                    }), [e, r, n]),
+                    i = (0, x.useMemo)((() => {
+                        const t = e.url.replace("user", "hub/spawn-pending");
+                        return t.endsWith("/") ? t.slice(0, -1) : t
+                    }), [e.url]);
                 return (0, t.jsxs)(x.Fragment, {
                     children: [e.active && (0, t.jsx)(c_, {
-                        href: e.url,
+                        href: i,
                         target: "_blank",
                         children: "Open Server"
                     }), !e.active && (0, t.jsx)(c_, {
                         onClick: o,
                         children: "Launch server"
                     })]
                 })
@@ -43361,31 +43365,34 @@
             }, {
                 field: "action",
                 headerName: "",
                 width: 125,
                 filterable: !1,
                 sortable: !1,
                 hideable: !1,
-                renderCell: e => (0, t.jsx)(gS, {
-                    url: e.row.url,
-                    serverName: e.row.name,
-                    imageName: e.row.image,
-                    active: e.row.active
-                })
+                renderCell: e => {
+                    var r;
+                    return (0, t.jsx)(gS, {
+                        url: e.row.url,
+                        serverName: e.row.name,
+                        imageName: null !== (r = e.row.uid) && void 0 !== r ? r : e.row.image,
+                        active: e.row.active
+                    })
+                }
             }],
             _S = (0, x.memo)((function(e) {
                 const r = (0, x.useMemo)((() => {
                     let t = [...e.servers];
                     return e.defaultServer.active && (t = [e.defaultServer, ...t]), t.map(((e, t) => {
-                        var r;
-                        const n = {
+                        var r, n, o, i, s;
+                        const a = {
                             ...e,
                             id: t
                         };
-                        return n.image = null !== (r = e.user_options.image) && void 0 !== r ? r : "", n.last_activity = function(e) {
+                        return a.image = null !== (o = null !== (n = null === (r = e.user_options) || void 0 === r ? void 0 : r.display_name) && void 0 !== n ? n : e.user_options.image) && void 0 !== o ? o : "", a.uid = null !== (s = null === (i = e.user_options) || void 0 === i ? void 0 : i.uid) && void 0 !== s ? s : null, a.last_activity = function(e) {
                             if (!e || 0 === e.length) return "unknown";
                             const t = {
                                     year: 31536e6,
                                     month: 2628e6,
                                     day: 864e5,
                                     hour: 36e5,
                                     minute: 6e4,
@@ -43396,15 +43403,15 @@
                                 }),
                                 n = new Date(e),
                                 o = new Date,
                                 i = n.getTime() - o.getTime();
                             for (const e in t)
                                 if (Math.abs(i) > t[e] || "second" === e) return r.format(Math.round(i / t[e]), e);
                             return "unknown"
-                        }(n.last_activity), n
+                        }(a.last_activity), a
                     }))
                 }), [e]);
                 return (0, t.jsx)(Hw, {
                     sx: {
                         padding: 1
                     },
                     children: (0, t.jsx)(Fw, {
@@ -43537,16 +43544,15 @@
                                 c = c + e + "_xsrf=" + i
                             }
                             const u = new EventSource(c);
                             u.onerror = e => {
                                 console.error("Failed to construct event stream", e), u.close()
                             }, u.onmessage = e => {
                                 const r = JSON.parse(e.data);
-                                if ("built" === r.phase) return u.close(), void s(!0);
-                                t.write(r.message), n.fit()
+                                if (t.write(r.message), n.fit(), "built" === r.phase) return u.close(), void s(!0)
                             }
                         }
                     }), [r, e.image]),
                     u = (e, t) => {
                         t && "backdropClick" === t || (l.current.terminal.dispose(), a.current && (a.current.innerHTML = ""), o(!1))
                     };
                 return (0, t.jsxs)(x.Fragment, {
@@ -43623,33 +43629,39 @@
                 headerName: "CPU Limit",
                 width: 100
             }, {
                 field: "status",
                 headerName: "Status",
                 width: 100,
                 hideSortIcons: !0,
-                renderCell: e => "built" === e.value ? (0, t.jsx)(nc, {
-                    children: (0, t.jsx)(vS.A, {
-                        color: "success"
-                    })
-                }) : "building" === e.value ? (0, t.jsx)(OS, {
-                    name: e.row.display_name,
-                    image: e.row.image_name
-                }) : null
+                renderCell: e => {
+                    var r;
+                    return "built" === e.value ? (0, t.jsx)(nc, {
+                        children: (0, t.jsx)(vS.A, {
+                            color: "success"
+                        })
+                    }) : "building" === e.value ? (0, t.jsx)(OS, {
+                        name: e.row.display_name,
+                        image: null !== (r = e.row.uid) && void 0 !== r ? r : e.row.image_name
+                    }) : null
+                }
             }, {
                 field: "remove",
                 headerName: "",
                 width: 100,
                 filterable: !1,
                 sortable: !1,
                 hideable: !1,
-                renderCell: e => (0, t.jsx)(AS, {
-                    name: e.row.display_name,
-                    image: e.row.image_name
-                })
+                renderCell: e => {
+                    var r;
+                    return (0, t.jsx)(AS, {
+                        name: e.row.display_name,
+                        image: null !== (r = e.row.uid) && void 0 !== r ? r : e.row.image_name
+                    })
+                }
             }],
             LS = (0, x.memo)((function(e) {
                 var r, n;
                 const o = (0, x.useMemo)((() => e.images.map(((t, r) => {
                     var n, o;
                     const i = {
                         ...t,
@@ -43717,24 +43729,26 @@
                         t && "backdropClick" === t || i(!1)
                     },
                     [d, h] = (0, x.useState)([]),
                     f = (0, x.useCallback)((e => {
                         e.length > 1 ? h([e[e.length - 1]]) : h(e)
                     }), [h]),
                     p = (0, x.useCallback)((async () => {
-                        const t = {
-                            imageName: e.images[d[0]].image_name,
-                            userName: n.user,
-                            serverName: l
-                        };
+                        var t;
+                        const o = e.images[d[0]],
+                            i = {
+                                imageName: null !== (t = o.uid) && void 0 !== t ? t : o.image_name,
+                                userName: n.user,
+                                serverName: l
+                            };
                         try {
                             a(!0), await r.serviceClient.request({
                                 method: "post",
                                 path: pS,
-                                data: t
+                                data: i
                             }), window.location.reload()
                         } catch (e) {
                             a(!1), alert(e)
                         }
                     }), [l, d, e.images, r, n]),
                     m = (0, x.useMemo)((() => 0 === d.length || (0 === l.length ? !!e.defaultRunning : void 0)), [d, l, e.defaultRunning]);
                 return (0, t.jsxs)(x.Fragment, {
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js.LICENSE.txt` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/static/js/servers.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/page.html` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/templates/page.html`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/conftest.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/binderhub_build/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import sys
+from pathlib import Path
 
 import pytest
-from aiodocker import Docker, DockerError
+import sqlalchemy as sa
+from sqlalchemy.orm import sessionmaker
 from traitlets.config import Config
 
 from tljh_repo2docker import tljh_custom_jupyterhub_config
+from tljh_repo2docker.database.model import DockerImageSQL
 
+ROOT = Path(__file__).parents[3]
 
-async def remove_docker_image(image_name):
-    async with Docker() as docker:
-        try:
-            await docker.images.delete(image_name, force=True)
-        except DockerError:
-            pass
+binderhub_service_name = "binder"
+binderhub_config = ROOT / "ui-tests" / "binderhub_config.py"
+tljh_repo2docker_config = ROOT / "ui-tests" / "tljh_repo2docker_binderhub.py"
 
-
-@pytest.fixture(scope="module")
-def minimal_repo():
-    return "https://github.com/plasmabio/tljh-repo2docker-test-binder"
-
-
-@pytest.fixture(scope="module")
-def minimal_repo_uppercase():
-    return "https://github.com/plasmabio/TLJH-REPO2DOCKER-TEST-BINDER"
+db_url = "sqlite:///tljh_repo2docker.sqlite"
 
 
 @pytest.fixture(scope="module")
 def generated_image_name():
-    return "plasmabio-tljh-repo2docker-test-binder:HEAD"
+    return "https-3a-2f-2fgithub-2ecom-2fplasmabio-2ftljh-2drepo2docker-2dtest-2dbinder-3f035a:06bb545ab3a2888477cbddfed0ea77eae313cfed"
 
 
 @pytest.fixture(scope="module")
 def image_name():
     return "tljh-repo2docker-test:HEAD"
 
 
@@ -39,41 +32,71 @@
 async def app(hub_app):
     config = Config()
     tljh_custom_jupyterhub_config(config)
 
     config.JupyterHub.services.extend(
         [
             {
+                "name": binderhub_service_name,
+                "admin": True,
+                "command": [
+                    sys.executable,
+                    "-m",
+                    "binderhub",
+                    f"--config={binderhub_config}",
+                ],
+                "url": "http://localhost:8585",
+                "oauth_client_id": "service-binderhub",
+                "oauth_no_confirm": True,
+            },
+            {
                 "name": "tljh_repo2docker",
                 "url": "http://127.0.0.1:6789",
                 "command": [
                     sys.executable,
                     "-m",
                     "tljh_repo2docker",
                     "--ip",
                     "127.0.0.1",
                     "--port",
                     "6789",
+                    "--binderhub_url",
+                    "http://localhost:8585/@/space%20word/services/binder/",
                 ],
                 "oauth_no_confirm": True,
-            }
+            },
         ]
     )
 
     config.JupyterHub.load_roles = [
         {
             "description": "Role for tljh_repo2docker service",
             "name": "tljh-repo2docker-service",
-            "scopes": ["read:users", "read:servers", "read:roles:users"],
+            "scopes": [
+                "read:users",
+                "read:roles:users",
+                "admin:servers",
+                "access:services!service=binder",
+            ],
             "services": ["tljh_repo2docker"],
         }
     ]
 
     app = await hub_app(config=config)
     return app
 
 
-@pytest.fixture(autouse=True)
-async def remove_all_test_images(image_name, generated_image_name, app):
-    yield
-    await remove_docker_image(image_name)
-    await remove_docker_image(generated_image_name)
+@pytest.fixture(scope="session")
+def db_session():
+    engine = sa.create_engine(db_url)
+    Session = sessionmaker(
+        bind=engine,
+        expire_on_commit=False,
+        autocommit=False,
+        autoflush=False,
+    )
+
+    session = Session()
+    yield session
+    session.query(DockerImageSQL).delete()
+    session.commit()
+    session.close()
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_builder.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/test_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from aiodocker import Docker, DockerError
 
-from .utils import add_environment, remove_environment, wait_for_image
+from ..utils import add_environment, remove_environment, wait_for_image
 
 
 @pytest.mark.asyncio
 async def test_add_environment(app, minimal_repo, image_name):
     name, ref = image_name.split(":")
     r = await add_environment(app, repo=minimal_repo, name=name, ref=ref)
     assert r.status_code == 200
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_images.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/local_build/test_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pytest
 from jupyterhub.tests.utils import get_page
 
-from .utils import add_environment, get_service_page, wait_for_image
+from ..utils import add_environment, get_service_page, wait_for_image
 
 
 @pytest.mark.asyncio
 async def test_images_list_admin(app):
     cookies = await app.login_user("admin")
     r = await get_service_page(
         "environments",
         app,
         cookies=cookies,
         allow_redirects=True,
     )
     r.raise_for_status()
     assert (
-        '{"images": [], "default_mem_limit": "None", "default_cpu_limit":"None", "machine_profiles": []}'
+        '{"repo_providers": [{"label": "Git", "value": "git"}], "use_binderhub": false, "images": [], "default_mem_limit": "None", "default_cpu_limit":"None", "machine_profiles": []}'
         in r.text
     )
 
 
 @pytest.mark.asyncio
 async def test_images_list_not_admin(app):
     cookies = await app.login_user("wash")
```

### Comparing `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/utils.py` & `tljh_repo2docker-2.0.0a1/tljh_repo2docker/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import asyncio
 import json
 
 from aiodocker import Docker, DockerError
-from jupyterhub.tests.utils import (async_requests, auth_header,
-                                    check_db_locks, public_host, public_url)
+from jupyterhub.tests.utils import (
+    async_requests,
+    auth_header,
+    check_db_locks,
+    public_host,
+    public_url,
+)
 from jupyterhub.utils import url_path_join as ujoin
 from tornado.httputil import url_concat
 
 
 @check_db_locks
 async def api_request(app, *api_path, method="get", noauth=False, **kwargs):
     """Make an API request"""
@@ -40,29 +45,32 @@
 def get_service_page(path, app, **kw):
     prefix = app.base_url
     service_prefix = "services/tljh_repo2docker"
     url = ujoin(public_host(app), prefix, service_prefix, path)
     return async_requests.get(url, **kw)
 
 
-async def add_environment(app, *, repo, ref="HEAD", name="", memory="", cpu=""):
+async def add_environment(
+    app, *, repo, ref="HEAD", name="", memory="", cpu="", provider=None
+):
     """Use the POST endpoint to add a new environment"""
+    data = {
+        "repo": repo,
+        "ref": ref,
+        "name": name,
+        "memory": memory,
+        "cpu": cpu,
+    }
+    if provider:
+        data["provider"] = provider
     r = await api_request(
         app,
         "environments",
         method="post",
-        data=json.dumps(
-            {
-                "repo": repo,
-                "ref": ref,
-                "name": name,
-                "memory": memory,
-                "cpu": cpu,
-            }
-        ),
+        data=json.dumps(data),
     )
     return r
 
 
 async def wait_for_image(*, image_name):
     """wait until an image is built"""
     count, retries = 0, 60 * 10
@@ -89,7 +97,28 @@
         data=json.dumps(
             {
                 "name": image_name,
             }
         ),
     )
     return r
+
+
+async def remove_docker_image(image_name):
+    async with Docker() as docker:
+        try:
+            await docker.images.delete(image_name, force=True)
+        except DockerError:
+            pass
+
+
+def next_event(it):
+    """read an event from an eventstream
+    From: https://github.com/jupyterhub/jupyterhub/blob/81d423d6c674765400a6fe88064c1366b7070f94/jupyterhub/tests/test_api.py#L692-L700
+    """
+    while True:
+        try:
+            line = next(it)
+        except StopIteration:
+            return
+        if line.startswith("data:"):
+            return json.loads(line.split(":", 1)[1])
```

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/package-lock.json` & `tljh_repo2docker-2.0.0a1/ui-tests/package-lock.json`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts` & `tljh_repo2docker-2.0.0a1/ui-tests/tests/ui.test.ts`

 * *Files 0% similar despite different names*

```diff
@@ -94,18 +94,17 @@
     await page.waitForTimeout(1000);
     await page.waitForURL('**/environments');
     await page
       .getByRole('row', { name: 'python-env https://github.com' })
       .getByRole('button')
       .first()
       .click();
-    await page.waitForSelector(
-      'span:has-text("Successfully tagged python-env:HEAD")',
-      { timeout: 600000 }
-    );
+    await page.waitForSelector('span:has-text("Successfully tagged")', {
+      timeout: 600000
+    });
     expect(await page.screenshot()).toMatchSnapshot('environment-console.png', {
       maxDiffPixelRatio: 0.05
     });
     await page.getByRole('button', { name: 'Close' }).click();
     await page.waitForTimeout(500);
     expect(await page.screenshot()).toMatchSnapshot('environment-list.png');
   });
@@ -139,15 +138,15 @@
     await page.waitForSelector('div:has-text("1 row selected")', {
       timeout: 1000
     });
     const createServer = await page.getByRole('button', {
       name: 'Create Server'
     });
     await createServer.click();
-    await expect(createServer).toHaveCount(0);
+    await expect(createServer).toHaveCount(0, { timeout: 20000 });
     await page.waitForURL('**/servers');
     await page.waitForTimeout(1000);
 
     expect(await page.screenshot()).toMatchSnapshot('running-servers.png');
   });
 
   test('Remove server', async ({ page }) => {
```

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/admin-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/admin.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-console-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-console.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-list-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/environment-list.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-remove-confirm-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-remove-confirm.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-removed-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environment-removed.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environments-page-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/environments-page.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/login-page-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/login-page.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/running-servers-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/running-servers.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-remove-confirm-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/local_snapshots/ui.test.ts/server-remove-confirm.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-removed-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/server-removed.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-dialog-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/servers-dialog.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-page-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/servers-page.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/user-linux.png` & `tljh_repo2docker-2.0.0a1/ui-tests/binderhub_snapshots/ui.test.ts/user.png`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/LICENSE` & `tljh_repo2docker-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tljh_repo2docker-2.0.0a0/README.md` & `tljh_repo2docker-2.0.0a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tljh-repo2docker
 
 ![Github Actions Status](https://github.com/plasmabio/tljh-repo2docker/workflows/Tests/badge.svg)
 
-TLJH plugin providing a JupyterHub service to build and use Docker images as user environments. The Docker images are built using [`repo2docker`](https://repo2docker.readthedocs.io/en/latest/).
+TLJH plugin provides a JupyterHub service to build and use Docker images as user environments. The Docker images can be built locally using [`repo2docker`](https://repo2docker.readthedocs.io/en/latest/) or via the [`binderhub`](https://binderhub.readthedocs.io/en/latest/) service.
 
 ## Requirements
 
 This plugin requires [The Littlest JupyterHub](https://tljh.jupyter.org) 1.0 or later (running on JupyterHub 4+).
 
 ## Installation
 
@@ -42,16 +42,18 @@
 The available settings for this service are:
 
 - `port`: Port of the service; defaults to 6789
 - `ip`: Internal IP of the service; defaults to 127.0.0.1
 - `default_memory_limit`: Default memory limit of a user server; defaults to `None`
 - `default_cpu_limit`: Default CPU limit of a user server; defaults to `None`
 - `machine_profiles`: Instead of entering directly the CPU and Memory value, `tljh-repo2docker` can be configured with pre-defined machine profiles and users can only choose from the available option; defaults to `[]`
+- `binderhub_url`: The optional URL of the `binderhub` service. If it is available, `tljh-repo2docker` will use this service to build images.
+- `db_url`: The connection string of the database. `tljh-repo2docker` needs a database to store the image metadata. By default, it will create a `sqlite` database in the starting directory of the service. To use other databases (`PostgreSQL` or `MySQL`), users need to specify the connection string via this config and install the additional drivers (`asyncpg` or `aiomysql`).
 
-This service requires the following scopes : `read:users`, `admin:servers` and `read:roles:users`. Here is an example of registering `tljh_repo2docker`'s service with JupyterHub
+This service requires the following scopes : `read:users`, `admin:servers` and `read:roles:users`. If `binderhub` service is used, ` access:services!service=binder`is also needed. Here is an example of registering `tljh_repo2docker`'s service with JupyterHub
 
 ```python
 # jupyterhub_config.py
 
 from tljh_repo2docker import TLJH_R2D_ADMIN_SCOPE
 import sys
 
@@ -74,15 +76,20 @@
     ]
 )
 # Set required scopes for the service and users
 c.JupyterHub.load_roles = [
     {
         "description": "Role for tljh_repo2docker service",
         "name": "tljh-repo2docker-service",
-        "scopes": ["read:users", "admin:servers", "read:roles:users"],
+        "scopes": [
+            "read:users",
+            "read:roles:users",
+            "admin:servers",
+            "access:services!service=binder",
+        ],
         "services": ["tljh_repo2docker"],
     },
     {
         "name": "user",
         "scopes": [
             "self",
             # access to the serve page
@@ -143,46 +150,54 @@
 
 ## Usage
 
 ### List the environments
 
 The _Environments_ page shows the list of built environments, as well as the ones currently being built:
 
-![environments](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-list-linux.png)
+![environments](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-list.png)
 
 ### Add a new environment
 
 Just like on [Binder](https://mybinder.org), new environments can be added by clicking on the _Add New_ button and providing a URL to the repository. Optional names, memory, and CPU limits can also be set for the environment:
 
-![add-new](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png)
+![add-new](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png)
+
+> [!NOTE]
+> If the build backend is `binderhub` service, users need to select the [repository provider](https://binderhub.readthedocs.io/en/latest/developer/repoproviders.html) and can not specify the custom build arguments
+
+![add-new-binderhub](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/binderhub_snapshots/ui.test.ts/environment-dialog.png)
 
 ### Follow the build logs
 
 Clicking on the _Logs_ button will open a new dialog with the build logs:
 
-![logs](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-console-linux.png)
+![logs](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-console.png)
 
 ### Select an environment
 
 Once ready, the environments can be selected from the JupyterHub spawn page:
 
-![select-env](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/servers-dialog-linux.png)
+![select-env](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/servers-dialog.png)
 
 ### Private Repositories
 
 `tljh-repo2docker` also supports building environments from private repositories.
 
 It is possible to provide the `username` and `password` in the `Credentials` section of the form:
 
-![image](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png)
+![image](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png)
 
 On GitHub and GitLab, a user might have to first create an access token with `read` access to use as the password:
 
 ![image](https://user-images.githubusercontent.com/591645/107350843-39c3bf80-6aca-11eb-8b82-6fa95ba4c7e4.png)
 
+> [!NOTE]
+> The `binderhub` build backend does not support configuring private repositories credentials from the interface.
+
 ### Machine profiles
 
 Instead of entering directly the CPU and Memory value, `tljh-repo2docker` can be configured with pre-defined machine profiles and users can only choose from the available options. The following configuration will add 3 machines with labels Small, Medium and Large to the profile list:
 
 ```python
 c.JupyterHub.services.extend(
     [
```

### Comparing `tljh_repo2docker-2.0.0a0/pyproject.toml` & `tljh_repo2docker-2.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,29 @@
 requires = ["hatchling>=1.5.0,<2", "hatch-nodejs-version>=0.3.2"]
 
 [project]
 dependencies = [
   "aiodocker~=0.19",
   "dockerspawner~=12.1",
   "jupyter_client>=6.1,<8",
-  "httpx"
+  "httpx",
+  "sqlalchemy>=2",
+  "pydantic>=2,<3",
+  "alembic>=1.13,<2",
+  "jupyter-repo2docker>=2024,<2025",
+  "aiosqlite~=0.19.0"
 ]
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "tljh-repo2docker"
 readme = "README.md"
 
+[project.scripts]
+tljh_repo2docker_upgrade_db = "tljh_repo2docker.dbutil:main"
+
 [project.entry-points.tljh]
 tljh_repo2docker = "tljh_repo2docker"
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.build.targets.sdist]
@@ -52,16 +60,13 @@
 npm = ["npm"]
 source_dir = "src"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
-before-build-npm = [
-  "npm install",
-  "npm run build:prod",
-]
+before-build-npm = ["npm install", "npm run build:prod"]
 before-build-python = ["npm run clean"]
 before-bump-version = ["python -m pip install hatch"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `tljh_repo2docker-2.0.0a0/PKG-INFO` & `tljh_repo2docker-2.0.0a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tljh-repo2docker
-Version: 2.0.0a0
+Version: 2.0.0a1
 License: BSD 3-Clause License
         
         Copyright (c) 2020, tljh-repo2docker
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -28,24 +28,29 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Requires-Dist: aiodocker~=0.19
+Requires-Dist: aiosqlite~=0.19.0
+Requires-Dist: alembic<2,>=1.13
 Requires-Dist: dockerspawner~=12.1
 Requires-Dist: httpx
 Requires-Dist: jupyter-client<8,>=6.1
+Requires-Dist: jupyter-repo2docker<2025,>=2024
+Requires-Dist: pydantic<3,>=2
+Requires-Dist: sqlalchemy>=2
 Description-Content-Type: text/markdown
 
 # tljh-repo2docker
 
 ![Github Actions Status](https://github.com/plasmabio/tljh-repo2docker/workflows/Tests/badge.svg)
 
-TLJH plugin providing a JupyterHub service to build and use Docker images as user environments. The Docker images are built using [`repo2docker`](https://repo2docker.readthedocs.io/en/latest/).
+TLJH plugin provides a JupyterHub service to build and use Docker images as user environments. The Docker images can be built locally using [`repo2docker`](https://repo2docker.readthedocs.io/en/latest/) or via the [`binderhub`](https://binderhub.readthedocs.io/en/latest/) service.
 
 ## Requirements
 
 This plugin requires [The Littlest JupyterHub](https://tljh.jupyter.org) 1.0 or later (running on JupyterHub 4+).
 
 ## Installation
 
@@ -81,16 +86,18 @@
 The available settings for this service are:
 
 - `port`: Port of the service; defaults to 6789
 - `ip`: Internal IP of the service; defaults to 127.0.0.1
 - `default_memory_limit`: Default memory limit of a user server; defaults to `None`
 - `default_cpu_limit`: Default CPU limit of a user server; defaults to `None`
 - `machine_profiles`: Instead of entering directly the CPU and Memory value, `tljh-repo2docker` can be configured with pre-defined machine profiles and users can only choose from the available option; defaults to `[]`
+- `binderhub_url`: The optional URL of the `binderhub` service. If it is available, `tljh-repo2docker` will use this service to build images.
+- `db_url`: The connection string of the database. `tljh-repo2docker` needs a database to store the image metadata. By default, it will create a `sqlite` database in the starting directory of the service. To use other databases (`PostgreSQL` or `MySQL`), users need to specify the connection string via this config and install the additional drivers (`asyncpg` or `aiomysql`).
 
-This service requires the following scopes : `read:users`, `admin:servers` and `read:roles:users`. Here is an example of registering `tljh_repo2docker`'s service with JupyterHub
+This service requires the following scopes : `read:users`, `admin:servers` and `read:roles:users`. If `binderhub` service is used, ` access:services!service=binder`is also needed. Here is an example of registering `tljh_repo2docker`'s service with JupyterHub
 
 ```python
 # jupyterhub_config.py
 
 from tljh_repo2docker import TLJH_R2D_ADMIN_SCOPE
 import sys
 
@@ -113,15 +120,20 @@
     ]
 )
 # Set required scopes for the service and users
 c.JupyterHub.load_roles = [
     {
         "description": "Role for tljh_repo2docker service",
         "name": "tljh-repo2docker-service",
-        "scopes": ["read:users", "admin:servers", "read:roles:users"],
+        "scopes": [
+            "read:users",
+            "read:roles:users",
+            "admin:servers",
+            "access:services!service=binder",
+        ],
         "services": ["tljh_repo2docker"],
     },
     {
         "name": "user",
         "scopes": [
             "self",
             # access to the serve page
@@ -182,46 +194,54 @@
 
 ## Usage
 
 ### List the environments
 
 The _Environments_ page shows the list of built environments, as well as the ones currently being built:
 
-![environments](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-list-linux.png)
+![environments](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-list.png)
 
 ### Add a new environment
 
 Just like on [Binder](https://mybinder.org), new environments can be added by clicking on the _Add New_ button and providing a URL to the repository. Optional names, memory, and CPU limits can also be set for the environment:
 
-![add-new](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png)
+![add-new](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png)
+
+> [!NOTE]
+> If the build backend is `binderhub` service, users need to select the [repository provider](https://binderhub.readthedocs.io/en/latest/developer/repoproviders.html) and can not specify the custom build arguments
+
+![add-new-binderhub](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/binderhub_snapshots/ui.test.ts/environment-dialog.png)
 
 ### Follow the build logs
 
 Clicking on the _Logs_ button will open a new dialog with the build logs:
 
-![logs](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-console-linux.png)
+![logs](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-console.png)
 
 ### Select an environment
 
 Once ready, the environments can be selected from the JupyterHub spawn page:
 
-![select-env](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/servers-dialog-linux.png)
+![select-env](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/servers-dialog.png)
 
 ### Private Repositories
 
 `tljh-repo2docker` also supports building environments from private repositories.
 
 It is possible to provide the `username` and `password` in the `Credentials` section of the form:
 
-![image](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png)
+![image](https://raw.githubusercontent.com/plasmabio/tljh-repo2docker/master/ui-tests/local_snapshots/ui.test.ts/environment-dialog.png)
 
 On GitHub and GitLab, a user might have to first create an access token with `read` access to use as the password:
 
 ![image](https://user-images.githubusercontent.com/591645/107350843-39c3bf80-6aca-11eb-8b82-6fa95ba4c7e4.png)
 
+> [!NOTE]
+> The `binderhub` build backend does not support configuring private repositories credentials from the interface.
+
 ### Machine profiles
 
 Instead of entering directly the CPU and Memory value, `tljh-repo2docker` can be configured with pre-defined machine profiles and users can only choose from the available options. The following configuration will add 3 machines with labels Small, Medium and Large to the profile list:
 
 ```python
 c.JupyterHub.services.extend(
     [
```

