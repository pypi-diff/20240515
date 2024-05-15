# Comparing `tmp/linktools-0.8.5rc1.tar.gz` & `tmp/linktools-0.8.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.5rc1.tar", last modified: Sun May  5 10:14:27 2024, max compression
+gzip compressed data, was "linktools-0.8.6rc0.tar", last modified: Wed May 15 15:42:03 2024, max compression
```

## Comparing `linktools-0.8.5rc1.tar` & `linktools-0.8.6rc0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35010 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.756403 linktools-0.8.5rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.764403 linktools-0.8.5rc1/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.764403 linktools-0.8.5rc1/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-05-05 10:14:22.000000 linktools-0.8.5rc1/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 10:14:22.000000 linktools-0.8.5rc1/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.756403 linktools-0.8.5rc1/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-05-05 10:12:12.000000 linktools-0.8.5rc1/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-05-05 10:12:12.000000 linktools-0.8.5rc1/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.760403 linktools-0.8.5rc1/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.772403 linktools-0.8.5rc1/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.772403 linktools-0.8.5rc1/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19476 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35010 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35455 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33405 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:42:03.391425 linktools-0.8.6rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.367425 linktools-0.8.6rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.375425 linktools-0.8.6rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-05-15 15:41:57.000000 linktools-0.8.6rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-15 15:41:57.000000 linktools-0.8.6rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.371425 linktools-0.8.6rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-05-15 15:40:20.000000 linktools-0.8.6rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-05-15 15:40:21.000000 linktools-0.8.6rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.371425 linktools-0.8.6rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.379425 linktools-0.8.6rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7405 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6351 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.383425 linktools-0.8.6rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ios/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19476 2024-05-15 15:40:14.000000 linktools-0.8.6rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:42:03.387425 linktools-0.8.6rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35455 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:42:03.000000 linktools-0.8.6rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.5rc1/LICENSE` & `linktools-0.8.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/PKG-INFO` & `linktools-0.8.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.5rc1
+Version: 0.8.6rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -68,26 +68,37 @@
 # python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
-对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
+对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置，简化调用方式，如：
 
 ```bash
-eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
+# 对于未正确设置PATH环境变量，或者使用venv安装模块
+# 会出现命令找不到的情况（command not found: lt）
+# 可通过以下命令生成alias脚本添加相关命令
+eval "$(python3 -m linktools.cli.commands.common.env --silent alias --shell bash)"
 
+# 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)"  
+
+# 配置全局java环境，指定java版本号（如：11.0.23/17.0.11/22.0.1）
+eval "$(ct-env --silent java 17.0.11 --shell bash)"
+
+# alias简化调用
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
+# alias简化各类工具调用
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools burpsuite"
-alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias jadx="ct-tools --set version=1.5.0 jadx-gui"  # 指定jadx版本号
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
@@ -203,15 +214,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/template/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc1/README.md` & `linktools-0.8.6rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,37 @@
 # python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
-对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
+对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置，简化调用方式，如：
 
 ```bash
-eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
+# 对于未正确设置PATH环境变量，或者使用venv安装模块
+# 会出现命令找不到的情况（command not found: lt）
+# 可通过以下命令生成alias脚本添加相关命令
+eval "$(python3 -m linktools.cli.commands.common.env --silent alias --shell bash)"
 
+# 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)"  
+
+# 配置全局java环境，指定java版本号（如：11.0.23/17.0.11/22.0.1）
+eval "$(ct-env --silent java 17.0.11 --shell bash)"
+
+# alias简化调用
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
+# alias简化各类工具调用
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools burpsuite"
-alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias jadx="ct-tools --set version=1.5.0 jadx-gui"  # 指定jadx版本号
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
@@ -152,15 +163,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/template/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc1/pyproject.toml` & `linktools-0.8.6rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/setup.py` & `linktools-0.8.6rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import json
 import os
 import pkgutil
 
 import yaml
```

### Comparing `linktools-0.8.5rc1/src/linktools/__init__.py` & `linktools-0.8.6rc0/src/linktools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from . import metadata
 from . import utils
 from . import decorator
 from ._url import DownloadError, DownloadHttpError
-from ._tools import Tools, Tool, ToolError, ToolNotFound, ToolExecError
+from ._tools import Tools, Tool, ToolError, ToolNotFound, ToolNotSupport, ToolExecError
 from ._config import Config, ConfigError
 from ._environ import BaseEnviron, environ
```

### Comparing `linktools-0.8.5rc1/src/linktools/__main__.py` & `linktools-0.8.6rc0/src/linktools/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from typing import Any
 
 from .cli import commands, BaseCommandGroup
```

### Comparing `linktools-0.8.5rc1/src/linktools/_config.py` & `linktools-0.8.6rc0/src/linktools/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import abc
 import configparser
 import errno
 import json
```

### Comparing `linktools-0.8.5rc1/src/linktools/_environ.py` & `linktools-0.8.6rc0/src/linktools/_environ.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import json
 import logging
 import os
 import pathlib
@@ -307,41 +307,52 @@
         """
         更新配置
         :param key: 配置键
         :param value: 配置值
         """
         self.config.set(key, value)
 
-    def _create_tools(self) -> "Dict[str, Tool]":
+    def _create_tools(self) -> "Tools":
         from ._tools import Tools
+        from ._config import ConfigDict
+
+        config = ConfigDict()
 
-        result = dict()
+        yaml_path = environ.get_path("template", "tools.yml")
+        if metadata.__release__ or not os.path.exists(yaml_path):
+            config.update_from_file(
+                environ.get_asset_path("tools.json"),
+                json.load
+            )
+        else:
+            import yaml
+            config.update_from_file(
+                yaml_path,
+                yaml.safe_load
+            )
+
+        tools = Tools(self, config)
 
         # set environment variable
         index = 0
         dir_names = os.environ["PATH"].split(os.pathsep)
-        for tool in Tools(self):
-            if not tool.supported:
-                if self.debug:
-                    self.logger.debug(f"Tool not supported: {tool.name}")
-                continue
+        for tool in Tools(self, config):
             if tool.executable:
                 # dirname(executable[0]) -> environ["PATH"]
                 dir_name = tool.dirname
                 if dir_name and dir_name not in dir_names:
                     # insert to head
                     dir_names.insert(index, tool.dirname)
                     index += 1
-            result[tool.name] = tool
         os.environ["PATH"] = os.pathsep.join(dir_names)
 
-        return result
+        return tools
 
     @cached_property
-    def tools(self) -> "Dict[str, Tool]":
+    def tools(self) -> "Tools":
         """
         工具集
         """
         return self._create_tools()
 
     def get_tool(self, name: str, **kwargs) -> "Tool":
         """
@@ -398,27 +409,14 @@
 
         # 导入configs文件夹中所有配置文件
         config.update_from_file(
             self.get_asset_path("android-tools.json"),
             load=json.load
         )
 
-        yaml_path = self.get_path("template", "tools.yml")
-        if metadata.__release__ or not os.path.exists(yaml_path):
-            config.update_from_file(
-                self.get_asset_path("tools.json"),
-                json.load
-            )
-        else:
-            import yaml
-            config.update_from_file(
-                yaml_path,
-                yaml.safe_load
-            )
-
         return config
 
     def get_asset_path(self, *paths: str) -> str:
         return self.get_path("assets", *paths)
 
 
 environ = Environ()
```

### Comparing `linktools-0.8.5rc1/src/linktools/_tools.py` & `linktools-0.8.6rc0/src/linktools/_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,118 +18,117 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import os
 import pickle
 import shutil
+import sys
 import warnings
-from typing import TYPE_CHECKING, Dict, Union, Mapping, Iterator, Any, Tuple, List, Type, Optional
+from typing import TYPE_CHECKING, Dict, Iterator, Any, Tuple, List, Type, Optional, Generator
 
 from . import utils
 from .decorator import cached_property
 from .metadata import __missing__
 
 if TYPE_CHECKING:
     from ._environ import BaseEnviron
 
+VALIDATE_KEYS = set()
+INTERNAL_KEYS = set()
+
 
 class Parser(object):
 
     def __init__(self, *items):
-        self._conditions = tuple(self._get_condition(item) for item in items)
+        self._validations = tuple(self._get_validation(item) for item in items)
 
-    def parse(self, cfg: Dict):
+    def parse(self, config: Dict):
         result = {}
-        for key in cfg:
-            result[key] = self._extend_field(cfg, key)
+        for key in config:
+            result[key] = self._extend_field(config, key)
         return result
 
-    def _extend_field(self, cfg, key: str, default=None):
-        value = utils.get_item(cfg, key, default=default)
-        if isinstance(value, dict) and "case" in value:
-            # parse case block:
-            # -----------------------------------------
-            #   field:
-            #     case:                                 <== case_block
-            #       - when: {system: [darwin, linux]}
-            #         then: xxx
-            #       - when: {system: windows}
-            #         then: yyy
-            #       - else: ~
-            # -----------------------------------------
-            case_block = value.get("case")
-            for cond_block in case_block:
-
-                when_block = utils.get_item(cond_block, "when")
-                if when_block is not None:
-                    # if it is a "when" block, verify it
-                    # -----------------------------------------
-                    #   field:
-                    #     case:
-                    #       - when: {system: [darwin, linux]}   <== when_block
-                    #         then: xxx
-                    #       - when: {system: windows}
-                    #         then: yyy
-                    #       - else: ~
-                    # -----------------------------------------
-                    is_verified = True
-                    for condition in self._conditions:
-                        if not condition(cfg, when_block):
-                            is_verified = False
-                            break
-
-                    # if any one of the verification fails, skip
-                    if not is_verified:
-                        continue
+    def _extend_field(self, config, key: str, default=None):
+        value = utils.get_item(config, key, default=default)
 
+        if not isinstance(value, dict) or "case" not in value:
+            # not found "case", use config value
+            return value
+
+        # parse case block:
+        # -----------------------------------------
+        #   field:
+        #     case:                                 <== case_block
+        #       - when: {system: [darwin, linux]}
+        #         then: xxx
+        #       - when: {system: windows}
+        #         then: yyy
+        #       - else: ~
+        # -----------------------------------------
+        case_block = value.get("case")
+        for cond_block in case_block:
+
+            when_block = utils.get_item(cond_block, "when")
+            if when_block is not None:
+                # if it is a "when" block, verify it
+                # -----------------------------------------
+                #   field:
+                #     case:
+                #       - when: {system: [darwin, linux]}   <== when_block
+                #         then: xxx
+                #       - when: {system: windows}
+                #         then: yyy
+                #       - else: ~
+                # -----------------------------------------
+                for validate in self._validations:
+                    if not validate(config, when_block):
+                        break
+                else:
                     # all items are verified, return "then"
                     # -----------------------------------------
                     #   field:
                     #     case:
                     #       - when: {system: [darwin, linux]}
                     #         then: xxx                         <== then_block
                     #       - when: {system: windows}
                     #         then: yyy
                     #       - else: ~
                     # -----------------------------------------
-                    return utils.get_item(cond_block, "then", default=default)  # ==> find "case" "when" "then"
+                    return utils.get_item(cond_block, "then", default=default)
 
-                else_block = utils.get_item(cond_block, "else")
-                if else_block is not None:  # ==> find "case" => "else"
-                    # if it is an else block, return "else"
-                    # -----------------------------------------
-                    #   field:
-                    #     case:
-                    #       - when: {system: [darwin, linux]}
-                    #         then: xxx
-                    #       - when: {system: windows}
-                    #         then: yyy
-                    #       - else: ~                           <== else_block
-                    # -----------------------------------------
-                    return else_block
-
-            # use default value
-            return default  # ==> not found "else"
+            else_block = utils.get_item(cond_block, "else")
+            if else_block is not None:
+                # if it is an else block, return "else"
+                # -----------------------------------------
+                #   field:
+                #     case:
+                #       - when: {system: [darwin, linux]}
+                #         then: xxx
+                #       - when: {system: windows}
+                #         then: yyy
+                #       - else: ~                           <== else_block
+                # -----------------------------------------
+                return else_block
 
-        # use config value
-        return value  # ==> not found "case"
+        # use default value
+        return default  # ==> not found "else"
 
     @classmethod
-    def _get_condition(cls, item: str):
+    def _get_validation(cls, item: str):
 
-        def check(config, when_block):
+        def validate(config, when_block):
             when_scope = utils.get_item(when_block, item)
             if when_scope is not None:
                 # -----------------------------------------
                 #   field:
                 #     case:
                 #       - when: {system: [darwin, linux]}   <== when_scope (system: [darwin, linux])
                 #         then: xxx
@@ -142,166 +141,194 @@
                     if value != when_scope:
                         return False
                 elif isinstance(when_scope, (tuple, list, set)):
                     if value not in when_scope:
                         return False
             return True
 
-        return check
+        return validate
 
 
 class ToolProperty(object):
 
-    def __init__(self, name=None, default=None):
+    def __init__(self, name=None, raw: bool = False, default: Any = None,
+                 internal: bool = False, validate: bool = False):
         self.name = name
+        self.raw = raw
         self.default = default
+        self.internal = internal
+        self.validate = validate
 
 
 class ToolMeta(type):
 
     def __new__(mcs, name, bases, attrs):
-        # initialize __parser__
-        attrs["__parser__"] = Parser("system", "machine")
-        # initialize __default__
-        attrs["__default__"] = {}
+        default = {}
         for key in list(attrs.keys()):
             if isinstance(attrs[key], ToolProperty):
-                var = attrs[key]
-                var_name = var.name or key
-                attrs["__default__"][var_name] = var.default
-                attrs[key] = property(mcs.make_fget(var_name))
+                prop: ToolProperty = attrs[key]
+                prop_name = prop.name or key
+                if prop.validate:
+                    VALIDATE_KEYS.add(prop_name)
+                if prop.internal:
+                    INTERNAL_KEYS.add(prop_name)
+                default[prop_name] = prop.default
+                attrs[key] = mcs._make_property(prop, prop_name)
+        attrs["__default__"] = default
+        attrs["__parser__"] = Parser(*VALIDATE_KEYS)
         return type.__new__(mcs, name, bases, attrs)
 
     @classmethod
-    def make_fget(mcs, key):
-        return lambda self: self.config.get(key)
+    def _make_property(mcs, prop: ToolProperty, name: str):
+        return property(lambda self: self._raw_config.get(name)) \
+            if prop.raw \
+            else property(lambda self: self.config.get(name))
 
 
 class ToolError(Exception):
     pass
 
 
 class ToolNotFound(ToolError):
     pass
 
 
+class ToolNotSupport(ToolError):
+    pass
+
+
 class ToolExecError(ToolError):
     pass
 
 
 class Tool(metaclass=ToolMeta):
     __default__: Dict
     __parser__: Parser
 
-    name: str = ToolProperty(default=__missing__)
-    depends_on: tuple = ToolProperty(default=[])
+    name: str = ToolProperty(default=__missing__, raw=True, internal=True)
+    system: str = ToolProperty(default=__missing__, raw=True, internal=True, validate=True)
+    machine: str = ToolProperty(default=__missing__, raw=True, internal=True, validate=True)
+    depends_on: tuple = ToolProperty(default=[], internal=True)
     download_url: str = ToolProperty(default=__missing__)
-    target_path: bool = ToolProperty(default=__missing__)
-    root_path: str = ToolProperty(default=__missing__)
-    unpack_path: str = ToolProperty(default=__missing__)
-    absolute_path: str = ToolProperty(default=__missing__)
+    target_path: bool = ToolProperty(default=__missing__, internal=True)
+    root_path: str = ToolProperty(default=__missing__, internal=True)
+    unpack_path: str = ToolProperty(default=__missing__, internal=True)
+    absolute_path: str = ToolProperty(default=__missing__, internal=True)
     cmdline: str = ToolProperty(default=__missing__)
-    executable: bool = ToolProperty(default=True)
-    executable_cmdline: tuple = ToolProperty(default=[])
-    environment: Dict[str, str] = ToolProperty(default={})
+    executable: bool = ToolProperty(default=True, internal=True)
+    executable_cmdline: tuple = ToolProperty(default=[], internal=True)
+    environment: Dict[str, str] = ToolProperty(default={}, internal=True)
 
-    def __init__(self, tools: "Tools", config: Union[dict, str], **kwargs):
+    def __init__(self, tools: "Tools", name: str, config: Dict[str, Any], **kwargs):
         self._tools = tools
         self._config = config
 
-        self._raw_config = pickle.loads(pickle.dumps(self.__default__))
-        self._raw_config.update(tools.config)
+        self._raw_config: Dict = pickle.loads(pickle.dumps(self.__default__))
         self._raw_config.update(config)
+        if self._raw_config.get("name") == __missing__:
+            self._raw_config["name"] = name
+        if self._raw_config.get("system") == __missing__:
+            self._raw_config["system"] = self._tools.environ.system
+        if self._raw_config.get("machine") == __missing__:
+            self._raw_config["machine"] = self._tools.environ.machine
+
+        prefix = self.name.replace("-", "_")
+        for key, value in self._raw_config.items():
+            if key not in INTERNAL_KEYS:
+                new_value = self._tools.config.get(f"{prefix}_{key}".upper(), default=None)
+                if new_value is not None:
+                    self._raw_config[key] = new_value
+
         self._raw_config.update(kwargs)
 
     @cached_property
     def config(self) -> dict:
         config = self.__parser__.parse(self._raw_config)
 
         depends_on = utils.get_item(config, "depends_on") or []
         assert isinstance(depends_on, (str, Tuple, List)), \
-            f"Tool<{config['name']}>.depends_on type error, " \
+            f"{self} depends_on type error, " \
             f"str/tuple/list was expects, got {type(depends_on)}"
         if isinstance(depends_on, str):
             depends_on = [depends_on]
         for dependency in depends_on:
-            assert dependency in self._tools.items, \
-                f"Tool<{config['name']}>.depends_on error: not found Tool<{dependency}>"
+            assert dependency in self._tools.all, \
+                f"{self}.depends_on error: not found Tool<{dependency}>"
         config["depends_on"] = depends_on
 
         # download url
         download_url = utils.get_item(config, "download_url") or ""
         if download_url == __missing__:
             download_url = ""
         assert isinstance(download_url, str), \
-            f"Tool<{config['name']}>.download_url type error, " \
+            f"{self} download_url type error, " \
             f"str was expects, got {type(download_url)}"
         config["download_url"] = download_url.format(tools=self._tools, **config)
 
         unpack_path = utils.get_item(config, "unpack_path") or ""
         if unpack_path == __missing__:
             unpack_path = ""
         assert isinstance(unpack_path, str), \
-            f"Tool<{config['name']}>.unpack_path type error, " \
+            f"{self} unpack_path type error, " \
             f"str was expects, got {type(unpack_path)}"
 
         target_path = utils.get_item(config, "target_path") or ""
         if target_path == __missing__:
             target_path = ""
         assert isinstance(target_path, str), \
-            f"Tool<{config['name']}>.target_path type error, " \
+            f"{self} target_path type error, " \
             f"str was expects, got {type(target_path)}"
 
         absolute_path = utils.get_item(config, "absolute_path") or ""
         if absolute_path == __missing__:
             absolute_path = ""
         assert isinstance(absolute_path, str), \
-            f"Tool<{config['name']}>.absolute_path type error, " \
+            f"{self} absolute_path type error, " \
             f"str was expects, got {type(absolute_path)}"
 
         if download_url and not unpack_path and not target_path:
             target_path = utils.guess_file_name(download_url)
 
         # target path: {target_path}
         # unpack path: {unpack_path}
         # root path: {data_path}/tools/{unpack_path}/
         # absolute path: {data_path}/tools/{unpack_path}/{target_path}
-        config["target_path"] = target_path.format(tools=self._tools, **config)
-        config["unpack_path"] = unpack_path.format(tools=self._tools, **config)
+        config["target_path"] = target_path = target_path.format(tools=self._tools, **config)
+        config["unpack_path"] = unpack_path = unpack_path.format(tools=self._tools, **config)
         paths = ["tools"]
-        if not utils.is_empty(config["unpack_path"]):
-            paths.append(config["unpack_path"])
-        config["root_path"] = self._tools.environ.get_data_dir(*paths)
+        if not utils.is_empty(unpack_path):
+            paths.append(unpack_path)
+        config["root_path"] = root_path = self._tools.environ.get_data_dir(*paths)
 
         if absolute_path:
             config["absolute_path"] = absolute_path.format(tools=self._tools, **config)
         elif config["target_path"]:
-            config["absolute_path"] = os.path.join(config["root_path"], config["target_path"])
+            config["absolute_path"] = os.path.join(root_path, target_path)
         else:
             config["absolute_path"] = ""
 
         # set executable cmdline
         cmdline = utils.get_item(config, "cmdline") or ""
         if cmdline == __missing__:
             cmdline = config["name"]
         assert isinstance(cmdline, str), \
-            f"Tool<{config['name']}>.cmdline type error, " \
-            f"str was expects, got {type(absolute_path)}"
+            f"{self} cmdline type error, " \
+            f"str was expects, got {type(cmdline)}"
         config["cmdline"] = cmdline
 
         if not utils.is_empty(cmdline):
             cmdline = shutil.which(cmdline)
         if not utils.is_empty(cmdline):
             config["absolute_path"] = cmdline
             config["executable_cmdline"] = [cmdline]
         else:
             executable_cmdline = utils.get_item(config, "executable_cmdline")
             if executable_cmdline:
-                assert isinstance(executable_cmdline, (str, Tuple, List)), \
-                    f"Tool<{config['name']}>.executable_cmdline type error, " \
+                assert isinstance(executable_cmdline, (str, tuple, list)), \
+                    f"{self} executable_cmdline type error, " \
                     f"str/tuple/list was expects, got {type(executable_cmdline)}"
                 # if executable_cmdline is not empty,
                 # set the executable flag to false
                 config["executable"] = False
             else:
                 # if executable_cmdline is empty,
                 # set absolute_path as executable_cmdline
@@ -323,28 +350,34 @@
     def exists(self) -> bool:
         return True if self.absolute_path and os.path.exists(self.absolute_path) else False
 
     @property
     def dirname(self) -> Optional[str]:
         return None if not self.absolute_path else os.path.dirname(self.absolute_path)
 
+    def get(self, key: str, default: Any = None) -> Any:
+        value = self.config.get(key, default)
+        if isinstance(value, str):
+            value = value.format(tools=self._tools, **self.config)
+        return value
+
     def copy(self, **kwargs) -> "Tool":
-        return Tool(self._tools, self._config, **kwargs)
+        return Tool(self._tools, self.name, self._config, **kwargs)
 
     def prepare(self) -> None:
+        if not self.supported:
+            raise ToolNotSupport(
+                f"{self} does not support on "
+                f"{self._tools.environ.system} ({self._tools.environ.machine})")
+
         for dependency in self.depends_on:
             tool = self._tools[dependency]
             tool.prepare()
 
         # download and unzip file
-        if not self.supported:
-            raise ToolError(
-                f"{self} does not support on "
-                f"{self._tools.environ.system} ({self._tools.environ.machine})")
-
         if not self.exists:
             self._tools.logger.info(f"Download {self}: {self.download_url}")
             url_file = self._tools.environ.get_url_file(self.download_url)
             temp_dir = self._tools.environ.get_temp_path("tools", "cache")
             temp_path = url_file.save(to_dir=temp_dir)
             if not utils.is_empty(self.unpack_path):
                 self._tools.logger.debug(f"Unpack {self} to {self.root_path}")
@@ -377,17 +410,17 @@
             env = kwargs.get("default_env", {})
             for key, value in self.environment.items():
                 env.setdefault(key, value)
             kwargs["default_env"] = env
 
         # java or other
         executable_cmdline = self.executable_cmdline
-        if executable_cmdline[0] in self._tools.items:
+        if executable_cmdline[0] in self._tools.all:
             args = [*executable_cmdline[1:], *args]
-            tool = self._tools.items[executable_cmdline[0]]
+            tool = self._tools[executable_cmdline[0]]
             return tool.popen(*args, **kwargs)
 
         return utils.Process(*[*executable_cmdline, *args], **kwargs)
 
     @utils.timeoutable
     def exec(
             self,
@@ -436,42 +469,71 @@
 
     def __repr__(self):
         return f"Tool<{self.name}>"
 
 
 class Tools(object):
 
-    def __init__(self, environ: "BaseEnviron"):
+    def __init__(self, environ: "BaseEnviron", config: Dict[str, Dict]):
         self.environ = environ
         self.logger = environ.get_logger("tools")
-        self.config = dict(
-            system=environ.system,
-            machine=environ.machine,
-        )
+        self.config = environ.wrap_config(prefix="")
+        self.all = self._parse_items(config)
 
-    @cached_property
-    def items(self) -> Mapping[str, Tool]:
-        items = {}
-        for key in self.environ.config.keys():
-            if not key.startswith("TOOL_"):
-                continue
-            value = self.environ.config.get(key)
+    def _parse_items(self, config: Dict[str, Dict]) -> Dict[str, Tool]:
+        result = {
+            "shell": Tool(self, "shell", {
+                "cmdline": None,
+                "absolute_path": utils.get_shell_path(),
+            }),
+            "python": Tool(self, "python", {
+                "cmdline": None,
+                "absolute_path": sys.executable,
+            }),
+        }
+
+        for key, value in config.items():
             if not isinstance(value, dict):
                 warnings.warn(f"dict was expected, got {type(value)}, ignored.")
                 continue
-            key = key[len("TOOL_"):].lower()
-            name = value.setdefault("name", key)
-            items[name] = Tool(self, value)
-        return items
+            name = value.get("name", None)
+            if name is None:
+                if key.startswith("TOOL_"):
+                    key = key[len("TOOL_"):]
+                name = value["name"] = key.lower()
+            result[name] = Tool(self, name, value)
+
+        return result
+
+    def keys(self) -> Generator[str, None, None]:
+        for k, v in self.all.items():
+            if v.supported:
+                yield k
+
+    def values(self) -> Generator[Tool, None, None]:
+        for k, v in self.all.items():
+            if v.supported:
+                yield v
+
+    def items(self) -> Generator[Tuple[str, Tool], None, None]:
+        for k, v in self.all.items():
+            if v.supported:
+                yield k, v
 
     def __iter__(self) -> Iterator[Tool]:
-        return iter(self.items.values())
+        return iter([t for t in self.all.values() if t.supported])
 
-    def __getitem__(self, item) -> Tool:
-        if item not in self.items:
+    def __getitem__(self, item: str) -> Tool:
+        tool = self.all.get(item, None)
+        if tool is None:
             raise ToolNotFound(f"Not found tool {item}")
-        return self.items[item]
+        if not tool.supported:
+            raise ToolNotSupport(
+                f"{tool} does not support on "
+                f"{self.environ.system} ({self.environ.machine})")
+        return tool
 
-    def __getattr__(self, item) -> Tool:
-        if item not in self.items:
-            raise ToolNotFound(f"Not found tool {item}")
-        return self.items[item]
+    def __getattr__(self, item: str) -> Tool:
+        return self[item]
+
+    def __setitem__(self, key: str, value: Tool):
+        self.all[key] = value
```

### Comparing `linktools-0.8.5rc1/src/linktools/_url.py` & `linktools-0.8.6rc0/src/linktools/_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import contextlib
 import os
 import shelve
 import shutil
```

### Comparing `linktools-0.8.5rc1/src/linktools/android/__init__.py` & `linktools-0.8.6rc0/src/linktools/container/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : __init__.py
-@time    : 2020/03/01
+@file    : __init__.py.py 
+@time    : 2023/05/21
 @site    :  
 @software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
@@ -18,14 +18,14 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .adb import Adb, Device, AdbError
-from .struct import App, Permission, Component, Activity, Service, Receiver, Provider, IntentFilter
+from .container import ContainerError, BaseContainer, ExposeLink, ExposeCategory
+from .manager import ContainerManager
```

### Comparing `linktools-0.8.5rc1/src/linktools/android/adb.py` & `linktools-0.8.6rc0/src/linktools/android/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import json
 import re
 import time
 from typing import Any, Generator, List
```

### Comparing `linktools-0.8.5rc1/src/linktools/android/struct.py` & `linktools-0.8.6rc0/src/linktools/android/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from typing import Optional
 
 from .. import utils
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/android-tools.apk` & `linktools-0.8.6rc0/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/android-tools.json` & `linktools-0.8.6rc0/src/linktools/assets/android-tools.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'time': '2024-05-15 23:41:57'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
         "md5": "c419cb85594b69ee31bae8730718c425",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-05-05 18:14:22"
+        "time": "2024-05-15 23:41:57"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/chrome-driver.json` & `linktools-0.8.6rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import os
 import re
 import shutil
 import textwrap
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.6rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from linktools.container import BaseContainer, ExposeLink
 from linktools.decorator import cached_property
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,25 @@
   flare:
     image: soulteary/flare:{{ FLARE_TAG }}
     user: '{{ DOCKER_UID }}:{{ DOCKER_GID }}'
 #   {% if int(FLARE_EXPOSE_PORT, 0) > 0 %}
     ports:
       - '{{ FLARE_EXPOSE_PORT }}:5005'
 #   {% endif %}
-#   {% if bool(FLARE_DISABLE_LOGIN) %}
-    command: flare --disable_login=1 --visibility=private
-    environment:
-      - 'FLARE_DISABLE_LOGIN=1'
-      - 'FLARE_GUIDE=1'
-#   {% else %}
-    command: flare --disable_login=0 --visibility=private
+    command: flare
     environment:
+#   {% if bool(FLARE_ENABLE_LOGIN) %}
       - 'FLARE_DISABLE_LOGIN=0'
+      - 'FLARE_VISIBILITY=PRIVATE'
       - 'FLARE_USER={{ FLARE_USER }}'
       - 'FLARE_PASS={{ FLARE_PASSWORD }}'
-      - 'FLARE_GUIDE=1'
+#   {% else %}
+      - 'FLARE_DISABLE_LOGIN=1'
 #   {% endif %}
+      - 'FLARE_GUIDE=1'
     volumes:
       - '{{ container.get_app_path("app") }}:/app'
     networks:
       - nginx
 
 networks:
   nginx:
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import yaml
 
 from linktools import Config, utils
 from linktools.container import BaseContainer
@@ -39,15 +39,15 @@
 
     @cached_property
     def configs(self):
         return dict(
             WILDCARD_DOMAIN=True,
 
             FLARE_TAG="latest",
-            FLARE_DISABLE_LOGIN=Config.Confirm(default=True, cached=True),
+            FLARE_ENABLE_LOGIN=Config.Confirm(default=False, cached=True),
             FLARE_DOAMIN=self.get_nginx_domain(""),
             FLARE_EXPOSE_PORT=None,
             FLARE_USER=Config.Prompt(default="admin", cached=True),
             FLARE_PASSWORD=Config.Prompt(cached=True),
         )
 
     @cached_property
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.6rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/fake_useragent.json` & `linktools-0.8.6rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/frida.js` & `linktools-0.8.6rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/frida.min.js` & `linktools-0.8.6rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.6rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 from typing import Any
 
 import click
 from objection.state.app import app_state
@@ -42,15 +42,15 @@
 
 class LinktoolsPlugin(Plugin, FridaScriptHandler):
 
     def __init__(self, ns):
         self.script_path = environ.get_asset_path("frida.js")
 
         super().__init__(__file__, ns, {
-            'meta': f'"{environ.name}',
+            'meta': f'{environ.name}',
             'commands': {
                 'eval': {
                     'meta': 'eval code',
                     'exec': self.eval_code
                 }
             }
         })
```

### Comparing `linktools-0.8.5rc1/src/linktools/assets/tools.json` & `linktools-0.8.6rc0/src/linktools/assets/tools.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.880756353021978%*

 * *Differences: {"'TOOL_AAPT'": "{'version': 'r34', 'version_name': 'android-14'}",*

 * * "'TOOL_AAPT2'": "OrderedDict([('version', 'r34'), ('version_name', 'android-14'), "*

 * *                 "('download_url', OrderedDict([('case', [OrderedDict([('when', "*

 * *                 "OrderedDict([('system', 'darwin')])), ('then', "*

 * *                 "'https://dl.google.com/android/repository/build-tools_{version}-macosx.zip')]), "*

 * *                 "OrderedDict([('when', OrderedDict([('system', 'linux')])), ('then', "*

 * *                 "'htt […]*

```diff
@@ -44,19 +44,71 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "build-tools-{version}",
-        "version": "r33",
-        "version_name": "android-13"
+        "version": "r34",
+        "version_name": "android-14"
+    },
+    "TOOL_AAPT2": {
+        "download_url": {
+            "case": [
+                {
+                    "then": "https://dl.google.com/android/repository/build-tools_{version}-macosx.zip",
+                    "when": {
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "https://dl.google.com/android/repository/build-tools_{version}-linux.zip",
+                    "when": {
+                        "system": "linux"
+                    }
+                },
+                {
+                    "then": "https://dl.google.com/android/repository/build-tools_{version}-windows.zip",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "target_path": {
+            "case": [
+                {
+                    "then": "{version_name}/{name}",
+                    "when": {
+                        "system": [
+                            "darwin",
+                            "linux"
+                        ]
+                    }
+                },
+                {
+                    "then": "{version_name}\\{name}.exe",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "unpack_path": "build-tools-{version}",
+        "version": "r34",
+        "version_name": "android-14"
     },
     "TOOL_ADB": {
-        "download_url": "https://dl.google.com/android/repository/platform-tools-latest-{system}.zip",
+        "download_url": "https://dl.google.com/android/repository/platform-tools-{version}-{system}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "platform-tools/{name}",
                     "when": {
                         "system": [
                             "darwin",
@@ -71,15 +123,16 @@
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
-        "unpack_path": "platform-tools"
+        "unpack_path": "platform-tools-{version}",
+        "version": "latest"
     },
     "TOOL_APKSIGNER": {
         "download_url": {
             "case": [
                 {
                     "then": "https://dl.google.com/android/repository/build-tools_{version}-macosx.zip",
                     "when": {
@@ -122,26 +175,26 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "build-tools-{version}",
-        "version": "r33",
-        "version_name": "android-13"
+        "version": "r34",
+        "version_name": "android-14"
     },
     "TOOL_APKTOOL": {
         "depends_on": "java",
         "download_url": "https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
-        "version": "2.8.1"
+        "version": "2.9.3"
     },
     "TOOL_APPCRAWLER": {
         "depends_on": "java",
         "download_url": "https://github.com/seveniruby/AppCrawler/releases/download/{version}/appcrawler-{version}-hogwarts.jar",
         "executable_cmdline": [
             "java",
             "-jar",
@@ -200,25 +253,26 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "target_path": "burpsuite_pro_v{version}.jar",
-        "version": "2023.10"
+        "version": "2024.4.2"
     },
     "TOOL_BURPSUITE_KEYGEN": {
         "depends_on": "java",
-        "download_url": "https://github.com/ice-black-tea/archives/releases/download/burp-loader-keygen-2_1_06/burp-loader-keygen-2_1_06.jar",
+        "download_url": "https://github.com/ice-black-tea/archives/releases/download/burp-loader-keygen-{version}/burp-loader-keygen-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
-        "name": "burpsuite-keygen"
+        "name": "burpsuite-keygen",
+        "version": "2_1_06"
     },
     "TOOL_CHROMEDRIVER": {
         "base_url": "http://chromedriver.storage.googleapis.com",
         "download_url": {
             "case": [
                 {
                     "then": "{base_url}/{version}/chromedriver_mac64_m1.zip",
@@ -339,43 +393,42 @@
                 }
             ]
         },
         "unpack_path": "compact_dex_converter-{version}",
         "version": "20240430"
     },
     "TOOL_DEX2JAR": {
-        "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
+        "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}/dex-tools-v{version}.zip",
         "target_path": {
             "case": [
                 {
-                    "then": "dex-tools-{version}/d2j-{name}.sh",
+                    "then": "dex-tools-v{version}/d2j-{name}.sh",
                     "when": {
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}\\d2j-{name}.bat",
+                    "then": "dex-tools-v{version}\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "dex2jar-{version}",
-        "version": "2.2-SNAPSHOT",
-        "version_suffix": "-2021-10-31"
+        "version": "2.4"
     },
     "TOOL_FASTBOOT": {
-        "download_url": "https://dl.google.com/android/repository/platform-tools-latest-{system}.zip",
+        "download_url": "https://dl.google.com/android/repository/platform-tools-{version}-{system}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "platform-tools/{name}",
                     "when": {
                         "system": [
                             "darwin",
@@ -390,21 +443,22 @@
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
-        "unpack_path": "platform-tools"
+        "unpack_path": "platform-tools-{version}",
+        "version": "latest"
     },
     "TOOL_FLINUX": {
         "download_url": {
             "case": [
                 {
-                    "then": "https://github.com/ice-black-tea/archives/releases/download/flinux-20240505/flinux.exe",
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/flinux-{version}/flinux.zip",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -419,15 +473,16 @@
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
-        "version": "0.21"
+        "unpack_path": "flinux-{version}",
+        "version": "20240505"
     },
     "TOOL_IPATOOL": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/majd/ipatool/releases/download/v{version}/ipatool-{version}-macos-arm64.tar.gz",
                     "when": {
@@ -496,15 +551,19 @@
                 }
             ]
         },
         "unpack_path": "ipatool-{version}",
         "version": "2.1.3"
     },
     "TOOL_JADX": {
+        "depends_on": "java",
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
+        "environment": {
+            "JAVA_OPTS": "-Xmx8g"
+        },
         "target_path": {
             "case": [
                 {
                     "then": "bin/{name}",
                     "when": {
                         "system": [
                             "darwin",
@@ -523,14 +582,15 @@
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
         "version": "1.5.0"
     },
     "TOOL_JADX_GUI": {
+        "depends_on": "java",
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
         "environment": {
             "JAVA_OPTS": "-Xmx8g"
         },
         "name": "jadx-gui",
         "target_path": {
             "case": [
@@ -554,40 +614,39 @@
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
         "version": "1.5.0"
     },
     "TOOL_JAR2DEX": {
-        "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
+        "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}/dex-tools-v{version}.zip",
         "target_path": {
             "case": [
                 {
-                    "then": "dex-tools-{version}/d2j-{name}.sh",
+                    "then": "dex-tools-v{version}/d2j-{name}.sh",
                     "when": {
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}\\d2j-{name}.bat",
+                    "then": "dex-tools-v{version}\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "dex2jar-{version}",
-        "version": "2.2-SNAPSHOT",
-        "version_suffix": "-2021-10-31"
+        "version": "2.4"
     },
     "TOOL_JARSIGNER": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/SAP/SapMachine/releases/download/sapmachine-{version}/sapmachine-jdk-{version}_macos-aarch64_bin.tar.gz",
                     "when": {
@@ -617,14 +676,36 @@
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
+        "home_path": {
+            "case": [
+                {
+                    "then": "{root_path}/sapmachine-jdk-{version}.jdk/Contents/Home",
+                    "when": {
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "{root_path}/sapmachine-jdk-{version}",
+                    "when": {
+                        "system": "linux"
+                    }
+                },
+                {
+                    "then": "{root_path}\\sapmachine-jdk-{version}",
+                    "when": {
+                        "system": "windows"
+                    }
+                }
+            ]
+        },
         "target_path": {
             "case": [
                 {
                     "then": "sapmachine-jdk-{version}.jdk/Contents/Home/bin/{name}",
                     "when": {
                         "system": "darwin"
                     }
@@ -681,14 +762,36 @@
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
+        "home_path": {
+            "case": [
+                {
+                    "then": "{root_path}/sapmachine-jdk-{version}.jdk/Contents/Home",
+                    "when": {
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "{root_path}/sapmachine-jdk-{version}",
+                    "when": {
+                        "system": "linux"
+                    }
+                },
+                {
+                    "then": "{root_path}\\sapmachine-jdk-{version}",
+                    "when": {
+                        "system": "windows"
+                    }
+                }
+            ]
+        },
         "target_path": {
             "case": [
                 {
                     "then": "sapmachine-jdk-{version}.jdk/Contents/Home/bin/{name}",
                     "when": {
                         "system": "darwin"
                     }
@@ -899,11 +1002,11 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "build-tools-{version}",
-        "version": "r33",
-        "version_name": "android-13"
+        "version": "r34",
+        "version_name": "android-14"
     }
 }
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/__init__.py` & `linktools-0.8.6rc0/src/linktools/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from . import argparse
 
 from .command import \
     BaseCommand, BaseCommandGroup, CommandError, \
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/argparse.py` & `linktools-0.8.6rc0/src/linktools/cli/argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import argparse
 import sys
 import typing
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/command.py` & `linktools-0.8.6rc0/src/linktools/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import abc
 import inspect
 import logging
 import os
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools.cli import AndroidCommand
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools import utils
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/app.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools import utils, environ
 from linktools.android import App, Permission, \
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools import utils
 from linktools.cli import AndroidCommand
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/frida.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,25 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import re
 from argparse import ArgumentParser, Namespace
 from typing import Optional, List, Type
 
 from linktools import utils, environ, DownloadError
 from linktools.cli import CommandError, AndroidCommand
-from linktools.cli.argparse import range_type, KeyValueAction
+from linktools.cli.argparse import range_type, KeyValueAction, BooleanOptionalAction
 from linktools.frida import FridaApplication, FridaShareScript, FridaScriptFile, FridaEvalCode
 from linktools.frida.android import AndroidFridaServer
 
 
 class Command(AndroidCommand):
     """
     Easy to use frida (require Android device rooted)
@@ -68,24 +68,38 @@
         parser.add_argument("-e", "--eval", metavar="CODE", action="append", dest="user_scripts",
                             type=lambda o: FridaEvalCode(o),
                             help="evaluate code")
         parser.add_argument("-c", "--codeshare", metavar="URL", action="append", dest="user_scripts",
                             type=lambda o: FridaShareScript(o, cached=False),
                             help="load share script url")
 
+        parser.add_argument("-a", "--auto-start", action="store_true", default=False,
+                            help="automatically start when all processes exits")
+
+        parser.add_argument("--serve", action=BooleanOptionalAction, default=True,
+                            help="serve frida server (default: true)")
+        parser.add_argument("--local-port", metavar="PORT", action="store", dest="local_port",
+                            type=range_type(1, 65536), default=None,
+                            help="local frida port (default: unused port)")
+        parser.add_argument("--remote-port", metavar="PORT", action="store", dest="remote_port",
+                            type=range_type(1, 65536), default=27042,
+                            help="remote frida port (default: 27042)")
+
+        parser.add_argument("--spawn-gating", action=BooleanOptionalAction, default=True,
+                            help="enable spawn gating (default: true)")
+        parser.add_argument("--child-gating", action=BooleanOptionalAction, default=False,
+                            help="enable child gating (default: false)")
+
         parser.add_argument("--redirect-address", metavar="ADDRESS", action="store", dest="redirect_address",
                             type=str,
                             help="redirect traffic to target address (default: localhost)")
         parser.add_argument("--redirect-port", metavar="PORT", action="store", dest="redirect_port",
                             type=range_type(1, 65536),
                             help="redirect traffic to target port (default: 8080)")
 
-        parser.add_argument("-a", "--auto-start", action="store_true", default=False,
-                            help="automatically start when all processes exits")
-
     def run(self, args: Namespace) -> Optional[int]:
 
         user_parameters = args.user_parameters
         user_scripts = args.user_scripts
 
         device = args.device_picker.pick()
         package = args.package
@@ -96,37 +110,44 @@
                 environ.logger.info(f"{session} detached, reason={reason}")
                 if reason in ("connection-terminated", "device-lost"):
                     self.stop()
                 elif len(self.sessions) == 0:
                     if args.auto_start:
                         app.load_script(app.device.spawn(package), resume=True)
 
-        with AndroidFridaServer(device=device, local_port=utils.pick_unused_port()) as server:
+        server = AndroidFridaServer(
+            device=device,
+            local_port=args.local_port or utils.pick_unused_port(),
+            remote_port=args.remote_port,
+            serve=args.serve
+        )
 
+        with server:
             # 如果没有填包名，则找到顶层应用
             if utils.is_empty(package):
                 target_app = server.get_frontmost_application()
                 if target_app is None:
                     raise CommandError("Unknown frontmost application")
                 package = target_app.identifier
             environ.logger.info(f"Frida inject target application: {package}")
 
             app = Application(
                 server,
                 target_identifiers=rf"^{re.escape(package)}($|:)",
                 user_parameters=user_parameters,
                 user_scripts=user_scripts,
-                enable_spawn_gating=True,
+                enable_spawn_gating=args.spawn_gating,
+                enable_child_gating=args.child_gating
             )
 
             if args.spawn:
                 # 打开进程后注入
                 app.load_script(app.device.spawn(package), resume=True)
 
-            elif app.inject_all():
+            elif app.inject_all(resume=True):
                 # 注入所有进程进程
                 pass
 
             elif args.auto_start:
                 # 进程不存在，打开进程后注入
                 app.load_script(app.device.spawn(package), resume=True)
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/info.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools import environ
 from linktools.cli import AndroidCommand
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import os
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools.cli import subcommand, subcommand_argument, AndroidCommand
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,93 +18,90 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional, List, Type
 
 from linktools import utils, environ, DownloadError
-from linktools.cli import CommandError, AndroidCommand
+from linktools.cli import CommandError, IOSCommand
 from linktools.cli.argparse import range_type
-from linktools.frida.android import AndroidFridaServer
+from linktools.frida.ios import IOSFridaServer
 
 
-class Command(AndroidCommand):
+class Command(IOSCommand):
     """
-    Easy to use objection (require Android device rooted)
+    Easy to use objection (require iOS device jailbreak)
     """
 
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         return super().known_errors + [DownloadError]
 
     def init_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument("-p", "--package", action="store", default=None,
-                            help="target package (default: frontmost application)")
+        parser.add_argument("-b", "--bundle-id", action="store", default=None,
+                            help="target bundle id (default: frontmost application)")
         parser.add_argument("-s", "--startup-command", action="append", default=[],
                             help="A command to run before the repl polls the device for information.")
         parser.add_argument("-c", "--file-commands", action="store",
                             help="A file containing objection commands, separated by a "
                                  "newline, that will run before the repl polls the device for information.")
         parser.add_argument("-S", "--startup-script", action="store",
                             help="A script to import and run before the repl polls the device for information.")
         parser.add_argument("-P", "--plugin-folder", action="store", default=environ.get_asset_path("objection"),
                             help="The folder to load plugins from.")
 
-        parser.add_argument("--redirect-address", metavar="ADDRESS", action="store", dest="redirect_address",
-                            type=str,
-                            help="redirect traffic to target address (default: localhost)")
-        parser.add_argument("--redirect-port", metavar="PORT", action="store", dest="redirect_port",
-                            type=range_type(1, 65536),
-                            help="redirect traffic to target port (default: 8080)")
+        parser.add_argument("--local-port", metavar="PORT", action="store", dest="local_port",
+                            type=range_type(1, 65536), default=None,
+                            help="local frida port (default: unused port)")
+        parser.add_argument("--remote-port", metavar="PORT", action="store", dest="remote_port",
+                            type=range_type(1, 65536), default=27042,
+                            help="remote frida port (default: 27042)")
 
     def run(self, args: Namespace) -> Optional[int]:
         device = args.device_picker.pick()
 
-        with AndroidFridaServer(device=device, local_port=utils.pick_unused_port()) as server:
+        server = IOSFridaServer(
+            device=device,
+            local_port=args.local_port or utils.pick_unused_port(),
+            remote_port=args.remote_port,
+        )
 
+        with server:
             objection_args = ["objection"]
             if environ.debug:
                 objection_args += ["--debug"]
             objection_args += ["-N", "-p", server.local_port]
 
-            package = args.package
-            if utils.is_empty(package):
+            bundle_id = args.bundle_id
+            if utils.is_empty(bundle_id):
                 target_app = server.get_frontmost_application()
                 if target_app is None:
                     raise CommandError("Unknown frontmost application")
-                package = target_app.identifier
-            environ.logger.info(f"Frida inject target application: {package}")
+                bundle_id = target_app.identifier
+            environ.logger.info(f"Frida inject target application: {bundle_id}")
 
-            objection_args += ["-g", package]
+            objection_args += ["-g", bundle_id]
             objection_args += ["explore"]
 
             for command in args.startup_command:
                 objection_args += ["--startup-command", command]
             if args.file_commands:
                 objection_args += ["--file-commands", args.file_commands]
             if args.startup_script:
                 objection_args += ["--startup-script", args.startup_script]
             if args.plugin_folder:
                 objection_args += ["--plugin-folder", args.plugin_folder]
 
-            if args.redirect_address or args.redirect_port:
-                # 如果需要重定向到本地端口
-                address = args.redirect_address
-                port = args.redirect_port or 8080
-                uid = device.get_uid(package)
-                with device.redirect(address, port, uid):
-                    return utils.Process(*objection_args).call()
-            else:
-                return utils.Process(*objection_args).call()
+            return utils.Process(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/android/top.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/top.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import datetime
 import sys
 from argparse import ArgumentParser, Namespace
 from typing import Optional
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import hashlib
 import os
 from argparse import ArgumentParser, Namespace
 from datetime import datetime
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import Namespace, ArgumentParser
 from subprocess import SubprocessError
 from typing import Optional, List, Type, Dict, Tuple, Any
 
 import yaml
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/common/env.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,25 +18,25 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import os
 import sys
 from typing import Any
 
 from linktools import utils
-from linktools.cli import subcommand, subcommand_argument, SubCommandWrapper, BaseCommandGroup, iter_command_modules, \
-    commands
+from linktools.cli import subcommand, subcommand_argument, SubCommandWrapper, BaseCommandGroup, \
+    iter_command_modules, commands
 from linktools.cli.argparse import auto_complete
 from linktools.utils import get_system, list2cmdline
 
 DEFAULT_SHELL = "bash" if get_system() != "windows" else "powershell"
 
 
 class InitCommand(BaseCommandGroup):
@@ -137,17 +137,14 @@
         path = self.environ.get_data_path("scripts", f"alias_{self.environ.version}", create_parent=True)
         if not sync and os.path.exists(path):
             self.logger.info(f"Found alias script: {path}")
             print(utils.read_file(path, text=True), flush=True)
             return 0
 
         lines = []
-        if shell not in ("powershell",):
-            lines.append(f"#!/usr/bin/env {shell}")
-
         modules = {c.name: c for c in iter_command_modules(commands, onerror="warn")}
         for module in modules.values():
             if module.command:
                 temp = module
                 names = [module.command_name]
                 while temp.parent_name in modules:
                     temp = modules[temp.parent_name]
@@ -164,14 +161,57 @@
                     lines.append(f"function __{executable}__ {{ {cmdline} $args }}")
                     lines.append(f"Set-Alias -Name {executable} -Value __{executable}__")
 
         result = os.linesep.join(lines)
         utils.write_file(path, result)
         print(result, flush=True)
 
+    @subcommand("java", help="generate java environment script")
+    @subcommand_argument("-s", "--shell", help="output code for the specified shell",
+                         choices=["bash", "zsh", "tcsh", "fish", "powershell"])
+    @subcommand_argument("version", metavar="VERSION", nargs="?",
+                         help="java version, such as 11.0.23 / 17.0.11 / 22.0.1")
+    def on_java_home(self, version: str = None, shell: str = DEFAULT_SHELL):
+        from linktools.cli.commands.common import tools
+        cmdline = list2cmdline([sys.executable, "-m", tools.__name__, "java"])
+
+        java = self.environ.tools["java"]
+        if version:
+            java = java.copy(version=version)
+
+        lines = []
+        if shell in ("bash", "zsh"):
+            lines.append(f"alias java='{cmdline}'")
+            lines.append(f"export JAVA_CMDLINE=''")
+            lines.append(f"export JAVA_VERSION='{java.get('version')}'")
+            lines.append(f"export JAVA_HOME='{java.get('home_path')}'")
+            lines.append(f"export PATH=\"$JAVA_HOME/bin:$PATH\"")
+        elif shell in ("fish",):
+            lines.append(f"alias java '{cmdline}'")
+            lines.append(f"set -x JAVA_CMDLINE ''")
+            lines.append(f"set -x JAVA_VERSION '{java.get('version')}'")
+            lines.append(f"set -x JAVA_HOME '{java.get('home_path')}'")
+            lines.append(f"set -x PATH \"$JAVA_HOME/bin\" \"$PATH\"")
+        elif shell in ("tcsh",):
+            lines.append(f"alias java '{cmdline}'")
+            lines.append(f"setenv JAVA_CMDLINE ''")
+            lines.append(f"setenv JAVA_VERSION '{java.get('version')}'")
+            lines.append(f"setenv JAVA_HOME '{java.get('home_path')}'")
+            lines.append(f"setenv PATH \"$JAVA_HOME/bin:$PATH\"")
+        elif shell in ("powershell",):
+            lines.append(f"function __tool_java__ {{ {cmdline} $args }}")
+            lines.append(f"Set-Alias -Name java -Value __tool_java__")
+            lines.append(f"$env:JAVA_CMDLINE=' '")
+            lines.append(f"$env:JAVA_VERSION='{java.get('version')}'")
+            lines.append(f"$env:JAVA_HOME='{java.get('home_path')}'")
+            lines.append(f"$env:PATH=\"$env:JAVA_HOME\\bin;$env:PATH\"")
+
+        result = os.linesep.join(lines)
+        print(result, flush=True)
+
     @subcommand("clean", help="clean temporary files")
     @subcommand_argument("days", metavar="DAYS", nargs="?", help="expire days")
     def on_clean(self, days: int = 7):
         self.environ.clean_temp_files(days)
 
 
 command = Command()
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/grep.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 import os
 import re
 import shutil
 import zipfile
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/common/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import json
 import subprocess
 from argparse import ArgumentParser, Namespace
 from typing import Optional, Type, List
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/android/objection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : at_frida.py
-@time    : 2018/11/25
-@site    :
-@software: PyCharm
+@file    : objection.py 
+@time    : 2022/11/20
+@site    :  
+@software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -18,114 +18,108 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
-import re
 from argparse import ArgumentParser, Namespace
-from typing import Optional, Type, List
+from typing import Optional, List, Type
 
 from linktools import utils, environ, DownloadError
-from linktools.cli import CommandError, IOSCommand
-from linktools.cli.argparse import KeyValueAction
-from linktools.frida import FridaApplication, FridaShareScript, FridaScriptFile, FridaEvalCode
-from linktools.frida.ios import IOSFridaServer
+from linktools.cli import CommandError, AndroidCommand
+from linktools.cli.argparse import range_type, BooleanOptionalAction
+from linktools.frida.android import AndroidFridaServer
 
 
-class Command(IOSCommand):
+class Command(AndroidCommand):
     """
-    Easy to use frida (require iOS device jailbreak)
+    Easy to use objection (require Android device rooted)
     """
 
-    def main(self, *args, **kwargs) -> None:
-        self.environ.config.set_default("SHOW_LOG_LEVEL", True)
-        self.environ.config.set_default("SHOW_LOG_TIME", True)
-        return super().main(*args, **kwargs)
-
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         return super().known_errors + [DownloadError]
 
     def init_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument("-b", "--bundle-id", action="store", default=None,
-                            help="target bundle id (default: frontmost application)")
-        parser.add_argument("--spawn", action="store_true", default=False,
-                            help="inject after spawn (default: false)")
-
-        parser.add_argument("-P", "--parameters",
-                            action=KeyValueAction, nargs="+", dest="user_parameters",
-                            help="user script parameters")
-
-        parser.add_argument("-l", "--load", metavar="SCRIPT",
-                            action="append", dest="user_scripts", default=[],
-                            type=lambda o: FridaScriptFile(o),
-                            help="load user script")
-        parser.add_argument("-e", "--eval", metavar="CODE", action="append", dest="user_scripts",
-                            type=lambda o: FridaEvalCode(o),
-                            help="evaluate code")
-        parser.add_argument("-c", "--codeshare", metavar="URL", action="append", dest="user_scripts",
-                            type=lambda o: FridaShareScript(o, cached=False),
-                            help="load share script url")
-
-        parser.add_argument("-a", "--auto-start", action="store_true", default=False,
-                            help="automatically start when all processes exits")
+        parser.add_argument("-p", "--package", action="store", default=None,
+                            help="target package (default: frontmost application)")
+        parser.add_argument("-s", "--startup-command", action="append", default=[],
+                            help="A command to run before the repl polls the device for information.")
+        parser.add_argument("-c", "--file-commands", action="store",
+                            help="A file containing objection commands, separated by a "
+                                 "newline, that will run before the repl polls the device for information.")
+        parser.add_argument("-S", "--startup-script", action="store",
+                            help="A script to import and run before the repl polls the device for information.")
+        parser.add_argument("-P", "--plugin-folder", action="store", default=environ.get_asset_path("objection"),
+                            help="The folder to load plugins from.")
+
+        parser.add_argument("--serve", action=BooleanOptionalAction, default=True,
+                            help="serve frida server (default: true)")
+        parser.add_argument("--local-port", metavar="PORT", action="store", dest="local_port",
+                            type=range_type(1, 65536), default=None,
+                            help="local frida port (default: unused port)")
+        parser.add_argument("--remote-port", metavar="PORT", action="store", dest="remote_port",
+                            type=range_type(1, 65536), default=27042,
+                            help="remote frida port (default: 27042)")
+
+        parser.add_argument("--redirect-address", metavar="ADDRESS", action="store", dest="redirect_address",
+                            type=str,
+                            help="redirect traffic to target address (default: localhost)")
+        parser.add_argument("--redirect-port", metavar="PORT", action="store", dest="redirect_port",
+                            type=range_type(1, 65536),
+                            help="redirect traffic to target port (default: 8080)")
 
     def run(self, args: Namespace) -> Optional[int]:
-
-        user_parameters = args.user_parameters
-        user_scripts = args.user_scripts
-
         device = args.device_picker.pick()
-        bundle_id = args.bundle_id
-
-        class Application(FridaApplication):
-
-            def on_session_detached(self, session, reason, crash) -> None:
-                environ.logger.info(f"{session} detached, reason={reason}")
-                if reason in ("connection-terminated", "device-lost"):
-                    self.stop()
-                elif len(self.sessions) == 0:
-                    if args.auto_start:
-                        app.load_script(app.device.spawn(bundle_id), resume=True)
 
-        with IOSFridaServer(device=device, local_port=utils.pick_unused_port()) as server:
+        server = AndroidFridaServer(
+            device=device,
+            local_port=args.local_port or utils.pick_unused_port(),
+            remote_port=args.remote_port,
+            serve=args.serve
+        )
+
+        with server:
+            objection_args = ["objection"]
+            if environ.debug:
+                objection_args += ["--debug"]
+            objection_args += ["-N", "-p", server.local_port]
 
-            # 如果没有填包名，则找到顶层应用
-            if utils.is_empty(bundle_id):
+            package = args.package
+            if utils.is_empty(package):
                 target_app = server.get_frontmost_application()
                 if target_app is None:
                     raise CommandError("Unknown frontmost application")
-                bundle_id = target_app.identifier
-            environ.logger.info(f"Frida inject target application: {bundle_id}")
+                package = target_app.identifier
+            environ.logger.info(f"Frida inject target application: {package}")
 
-            app = Application(
-                server,
-                target_identifiers=rf"^{re.escape(bundle_id)}$",
-                user_parameters=user_parameters,
-                user_scripts=user_scripts,
-                enable_spawn_gating=True
-            )
-
-            if args.spawn:
-                # 打开进程后注入
-                app.load_script(app.device.spawn(bundle_id), resume=True)
-
-            elif app.inject_all():
-                # 注入所有进程进程
-                pass
-
-            elif args.auto_start:
-                # 进程不存在，打开进程后注入
-                app.load_script(app.device.spawn(bundle_id), resume=True)
+            objection_args += ["-g", package]
+            objection_args += ["explore"]
 
-            return app.run()
+            for command in args.startup_command:
+                objection_args += ["--startup-command", command]
+            if args.file_commands:
+                objection_args += ["--file-commands", args.file_commands]
+            if args.startup_script:
+                objection_args += ["--startup-script", args.startup_script]
+            if args.plugin_folder:
+                objection_args += ["--plugin-folder", args.plugin_folder]
+
+            if args.redirect_address or args.redirect_port:
+                # 如果需要重定向到本地端口
+                address = args.redirect_address
+                port = args.redirect_port or 8080
+                uid = device.get_uid(package)
+                with device.redirect(address, port, uid):
+                    return utils.Process(*objection_args).call()
+            else:
+                return utils.Process(*objection_args).call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.6rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional, Type, List
 
 import paramiko
 from paramiko.ssh_exception import SSHException
```

### Comparing `linktools-0.8.5rc1/src/linktools/cli/device.py` & `linktools-0.8.6rc0/src/linktools/cli/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import abc
 import functools
 import os
 from argparse import ArgumentParser, Action, Namespace
```

### Comparing `linktools-0.8.5rc1/src/linktools/container/__init__.py` & `linktools-0.8.6rc0/src/linktools/frida/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : __init__.py.py 
-@time    : 2023/05/21
-@site    :  
-@software: PyCharm 
+@file    : frida.py
+@time    : 2018/11/25
+@site    :
+@software: PyCharm
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -18,14 +18,15 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .container import ContainerError, BaseContainer, ExposeLink, ExposeCategory
-from .manager import ContainerManager
+from .app import FridaApplication
+from .script import FridaScriptFile, FridaShareScript, FridaEvalCode
+from .server import FridaServer
```

### Comparing `linktools-0.8.5rc1/src/linktools/container/container.py` & `linktools-0.8.6rc0/src/linktools/container/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import os
 import re
 import textwrap
 from typing import TYPE_CHECKING, Dict, Any, List, Optional
```

### Comparing `linktools-0.8.5rc1/src/linktools/container/manager.py` & `linktools-0.8.6rc0/src/linktools/container/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 import json
 import os
 import os.path
 import shutil
```

### Comparing `linktools-0.8.5rc1/src/linktools/container/repository.py` & `linktools-0.8.6rc0/src/linktools/container/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from git import Repo, RemoteProgress
 from git.util import CallableRemoteProgress
 
 from .. import utils
 from ..rich import create_simple_progress
```

### Comparing `linktools-0.8.5rc1/src/linktools/decorator.py` & `linktools-0.8.6rc0/src/linktools/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 import threading
 from typing import TYPE_CHECKING, TypeVar, Type, Any, Callable, Tuple
 
 from .metadata import __missing__
```

### Comparing `linktools-0.8.5rc1/src/linktools/device.py` & `linktools-0.8.6rc0/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/frida/__init__.py` & `linktools-0.8.6rc0/src/linktools/android/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : frida.py
-@time    : 2018/11/25
-@site    :
-@software: PyCharm
+@file    : __init__.py
+@time    : 2020/03/01
+@site    :  
+@software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -18,15 +18,14 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .app import FridaApplication
-from .script import FridaScriptFile, FridaShareScript, FridaEvalCode
-from .server import FridaServer
+from .adb import Adb, Device, AdbError
+from .struct import App, Permission, Component, Activity, Service, Receiver, Provider, IntentFilter
```

### Comparing `linktools-0.8.5rc1/src/linktools/frida/android.py` & `linktools-0.8.6rc0/src/linktools/frida/android.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,22 @@
 
 
 class AndroidFridaServer(FridaServer):
     """
     android server
     """
 
-    def __init__(self, device: Device = None, local_port: int = 47042, remote_port: int = 47042):
+    def __init__(self, device: Device = None, local_port: int = 47042, remote_port: int = 47042, serve: bool = True):
         super().__init__(frida.get_device_manager().add_remote_device(f"localhost:{local_port}"))
         self._device = device or Device()
         self._local_port = local_port
         self._remote_port = remote_port
         self._forward: Optional[Stoppable] = None
 
+        self._serve = serve
         self._server_prefix = "fs-ln-"
         self._server_name = f"{self._server_prefix}{utils.make_uuid()}"
         self._server_dir = self._device.get_data_path("fs-ln")
         self._server_path = self._device.get_data_path("fs-ln", self._server_name)
 
     @property
     def local_port(self):
@@ -48,49 +49,51 @@
     @property
     def remote_port(self):
         return self._remote_port
 
     def _start(self):
 
         try:
-            server_path = self._prepare_executable()
-
             # 转发端口
             if self._forward is not None:
                 self._forward.stop()
             self._forward = self._device.forward(
                 f"tcp:{self._local_port}",
                 f"tcp:{self._remote_port}"
             )
 
-            # 创建软链
-            self._device.sudo("mkdir", "-p", self._server_dir)
-            self._device.sudo("ln", "-s", server_path, self._server_path)
-
-            # 接下来新开一个进程运行frida server，并且输出一下是否出错
-            self._device.sudo(
-                self._server_path,
-                "-d", "fs-binaries",
-                "-l", f"0.0.0.0:{self._remote_port}",
-                "-D", "&",
-                ignore_errors=True,
-                log_output=True,
-            )
+            if self._serve:
+                # 创建软链
+                server_path = self._prepare_executable()
+                self._device.sudo("mkdir", "-p", self._server_dir)
+                self._device.sudo("ln", "-s", server_path, self._server_path)
+
+                # 接下来新开一个进程运行frida server，并且输出一下是否出错
+                self._device.sudo(
+                    self._server_path,
+                    "-d", "fs-binaries",
+                    "-l", f"0.0.0.0:{self._remote_port}",
+                    "-D", "&",
+                    ignore_errors=True,
+                    log_output=True,
+                )
         finally:
-            # 删除软连接
-            self._device.sudo("rm", self._server_path, ignore_errors=True)
+            if self._serve:
+                # 删除软连接
+                self._device.sudo("rm", self._server_path, ignore_errors=True)
 
     def _stop(self):
         try:
-            # 就算杀死adb进程，frida server也不一定真的结束了，所以kill一下frida server进程
-            process_name_lc = f"{self._server_prefix}*".lower()
-            for process in self._device.get_processes():
-                if fnmatch.fnmatchcase(process.name.lower(), process_name_lc):
-                    _logger.debug(f"Find frida server process({process.name}:{process.pid}), kill it")
-                    self._device.sudo("kill", "-9", process.pid, ignore_errors=True)
+            if self._serve:
+                # 就算杀死adb进程，frida server也不一定真的结束了，所以kill一下frida server进程
+                process_name_lc = f"{self._server_prefix}*".lower()
+                for process in self._device.get_processes():
+                    if fnmatch.fnmatchcase(process.name.lower(), process_name_lc):
+                        _logger.debug(f"Find frida server process({process.name}:{process.pid}), kill it")
+                        self._device.sudo("kill", "-9", process.pid, ignore_errors=True)
         finally:
             # 把转发端口给移除了，不然会一直占用这个端口
             if self._forward is not None:
                 self._forward.stop()
                 self._forward = None
 
     @classmethod
```

### Comparing `linktools-0.8.5rc1/src/linktools/frida/app.py` & `linktools-0.8.6rc0/src/linktools/frida/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,18 +320,18 @@
             return f"Group({', '.join(self._names)})"
 
 
 class FridaManager:
 
     def __init__(self, reactor: FridaReactor):
         self._reactor = reactor
-        self._cancel_handlers = {}
+        self._cancel_handlers: "Dict[str, Callable[[], Any]]" = {}
 
         self._lock = threading.RLock()
-        self._sessions: Dict[int, FridaSession] = {}
+        self._sessions: "Dict[int, FridaSession]" = {}
 
     @property
     def sessions(self) -> Dict[int, FridaSession]:
         with self._lock:
             sessions = {}
             for pid in list(self._sessions.keys()):
                 session = self._sessions.get(pid)
@@ -351,15 +351,15 @@
             return None
 
     def set_session(self, session: FridaSession):
         with self._lock:
             self._sessions[session.pid] = session
 
     def add_device_handler(self, device: frida.core.Device, handler: FridaDeviceHandler):
-        self._cancel(device)
+        self._call_cancel_handler(device)
 
         cb_spawn_added = lambda spawn: threading.Thread(target=handler.on_spawn_added, args=(spawn,)).start()
         cb_spawn_removed = lambda spawn: self._reactor.schedule(lambda: handler.on_spawn_removed(spawn))
         cb_child_added = lambda child: self._reactor.schedule(lambda: handler.on_child_added(child))
         cb_child_removed = lambda child: self._reactor.schedule(lambda: handler.on_child_removed(child))
         cb_output = lambda pid, fd, data: self._reactor.schedule(lambda: handler.on_output(pid, fd, data))
         cb_lost = lambda: self._reactor.schedule(lambda: handler.on_device_lost())
@@ -379,62 +379,62 @@
             utils.ignore_error(device.off, args=("child-added", cb_child_added))
             utils.ignore_error(device.off, args=("child-removed", cb_child_removed))
             utils.ignore_error(device.off, args=("output", cb_output))
             # utils.ignore_error(device.off, args=("process-crashed", cb_process_crashed))
             # utils.ignore_error(device.off, args=("uninjected", cb_uninjected))
             utils.ignore_error(device.off, args=("lost", cb_lost))
 
-        self._register_cancel(device, cancel)
+        self._register_cancel_handler(device, cancel)
 
     def remove_device_handler(self, device: frida.core.Device):
-        self._cancel(device)
+        self._call_cancel_handler(device)
 
     def add_session_handler(self, session: FridaSession, handler: FridaSessionHandler):
-        self._cancel(session)
+        self._call_cancel_handler(session)
 
         def on_detached(reason, crash):
-            self._reactor.schedule(lambda: self._cancel(session))
+            self._reactor.schedule(lambda: self._call_cancel_handler(session))
             with self._lock:
                 self._sessions.pop(session.pid, None)
             self._reactor.schedule(lambda: handler.on_session_detached(session, reason, crash))
 
         session.on("detached", on_detached)
 
         def cancel():
             utils.ignore_error(session.off, args=("detached", on_detached))
 
-        self._register_cancel(session, cancel)
+        self._register_cancel_handler(session, cancel)
 
     def remove_session_handler(self, session: FridaSession):
-        self._cancel(session)
+        self._call_cancel_handler(session)
 
     def add_script_handler(self, script: FridaScript, handler: FridaScriptHandler):
-        self._cancel(script)
+        self._call_cancel_handler(script)
 
         def on_message(msg, data):
             return handler.on_script_message(script, msg, data)
 
         def on_destroyed():
-            self._reactor.schedule(lambda: self._cancel(script))
+            self._reactor.schedule(lambda: self._call_cancel_handler(script))
             return handler.on_script_destroyed(script)
 
         script.on("message", on_message)
         script.on("destroyed", on_destroyed)
 
         def cancel():
             utils.ignore_error(script.off, args=("message", on_message))
             utils.ignore_error(script.off, args=("destroyed", on_destroyed))
 
-        self._register_cancel(script, cancel)
+        self._register_cancel_handler(script, cancel)
 
     def remove_script_handler(self, script: FridaScript):
-        self._cancel(script)
+        self._call_cancel_handler(script)
 
     def add_file_handler(self, files: [FridaScriptFile], handler: FridaFileHandler):
-        self._cancel(files)
+        self._call_cancel_handler(files)
 
         last_change_id = 0
         monitors: Dict[str, frida.FileMonitor] = {}
 
         def make_monitor(file):
             _logger.debug(f"Monitor file: {file.path}")
             monitor = frida.FileMonitor(file.path)
@@ -460,23 +460,23 @@
             if file.path not in monitors:
                 monitors[file.path] = make_monitor(file)
 
         def cancel():
             for monitor in monitors.values():
                 monitor.disable()
 
-        self._register_cancel(files, cancel)
+        self._register_cancel_handler(files, cancel)
 
     def remove_file_handler(self, files: [FridaScriptFile]):
-        self._cancel(files)
+        self._call_cancel_handler(files)
 
-    def _register_cancel(self, key: Any, handler: Callable[[], Any]):
+    def _register_cancel_handler(self, key: Any, handler: Callable[[], Any]):
         self._cancel_handlers[self._make_key(key)] = handler
 
-    def _cancel(self, key: Any):
+    def _call_cancel_handler(self, key: Any):
         handler = self._cancel_handlers.pop(self._make_key(key), None)
         if handler:
             handler()
 
     @classmethod
     def _make_key(cls, key: Any):
         if isinstance(key, (list, tuple, set)):
@@ -591,15 +591,23 @@
             user_script.load()
 
         self._finished.clear()
         self._manager.add_file_handler(self._user_files, self)
         self._manager.add_device_handler(self.device, self)
 
         if self._enable_spawn_gating:
-            self.device.enable_spawn_gating()
+            try:
+                self.device.enable_spawn_gating()
+            except frida.NotSupportedError:
+                _logger.warning(f"Enable child gating is not supported, ignore")
+        else:
+            try:
+                self.device.disable_spawn_gating()
+            except frida.NotSupportedError:
+                pass
 
     def _deinit(self):
         _logger.debug(f"FridaApplication deinit")
 
         self._manager.remove_device_handler(self.device)
         self._manager.remove_file_handler(self._user_files)
         self._finished.set()
@@ -647,15 +655,15 @@
         """
         加载脚本，注入到指定进程
         :param pid: 进程id
         :param resume: 注入后是否需要resume进程
         """
         self._reactor.schedule(lambda: self._load_script(pid, resume))
 
-    def inject_all(self) -> [int]:
+    def inject_all(self, resume: bool = False) -> [int]:
         """
         根据target_identifiers注入所有匹配的进程
         :return: 注入的进程pid
         """
 
         target_pids = set()
 
@@ -670,15 +678,15 @@
             for target_process in self.device.enumerate_processes():
                 if target_process.pid > 0 and identifier.search(target_process.name):
                     target_pids.add(target_process.pid)
 
         if len(target_pids) > 0:
             # 进程存在，直接注入
             for pid in target_pids:
-                self.load_script(pid)
+                self.load_script(pid, resume=resume)
 
         return target_pids
 
     @property
     def sessions(self) -> Dict[int, FridaSession]:
         """
         所有已注入的session
@@ -757,16 +765,23 @@
             raise frida.ProcessNotFoundError(f"unable to find process with pid '{pid}'")
 
         session = self.device.attach(target_process.pid)
         session = FridaSession(session, target_process.name)
         self._manager.set_session(session)
 
         if self._enable_child_gating:
-            _logger.debug(f"Enable child gating: {pid}")
-            session.enable_child_gating()
+            try:
+                session.enable_child_gating()
+            except frida.NotSupportedError:
+                _logger.warning(f"Enable child gating is not supported, ignore")
+        else:
+            try:
+                session.disable_child_gating()
+            except frida.NotSupportedError:
+                pass
 
         self._manager.add_session_handler(session, self)
         self._reactor.schedule(lambda: self.on_session_attached(session))
 
         return session
 
     def _detach_session(self, session: FridaSession):
```

### Comparing `linktools-0.8.5rc1/src/linktools/frida/ios.py` & `linktools-0.8.6rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/frida/script.py` & `linktools-0.8.6rc0/src/linktools/frida/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import json
 import os
 import threading
 from typing import Union, Optional
```

### Comparing `linktools-0.8.5rc1/src/linktools/frida/server.py` & `linktools-0.8.6rc0/src/linktools/frida/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import time
 
 import frida
 
@@ -55,29 +55,36 @@
             return False
 
     def start(self) -> bool:
         """
         根据frida版本和设备abi类型下载并运行server
         :return: 运行成功为True，否则为False
         """
-        if self.is_running:
-            _logger.info("Frida server is running ...")
-            return True
-
-        _logger.info("Start frida server ...")
-        self._start()
+        try:
 
-        timeout = utils.Timeout(10)
-        while timeout.check():
             if self.is_running:
                 _logger.info("Frida server is running ...")
                 return True
-            time.sleep(min(timeout.remain, 0.5))
 
-        raise frida.ServerNotRunningError("Frida server failed to run ...")
+            _logger.info("Start frida server ...")
+            self._start()
+
+            timeout = utils.Timeout(10)
+            while timeout.check():
+                if self.is_running:
+                    _logger.info("Frida server is running ...")
+                    return True
+                time.sleep(min(timeout.remain, 0.5))
+
+            raise frida.ServerNotRunningError("Frida server failed to run ...")
+
+        except BaseException as e:
+            _logger.debug("Kill frida server ...")
+            utils.ignore_error(self._stop)
+            raise e
 
     def stop(self) -> bool:
         """
         强制结束frida server
         :return: 结束成功为True，否则为False
         """
         _logger.info("Kill frida server ...")
@@ -94,17 +101,12 @@
         pass
 
     @abc.abstractmethod
     def _stop(self):
         pass
 
     def __enter__(self):
-        try:
-            self.start()
-        except:
-            _logger.debug("Kill frida server ...")
-            utils.ignore_error(self._stop)
-            raise
+        self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
```

### Comparing `linktools-0.8.5rc1/src/linktools/ida/__init__.py` & `linktools-0.8.6rc0/src/linktools/ida/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,11 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
```

### Comparing `linktools-0.8.5rc1/src/linktools/ida/ida.py` & `linktools-0.8.6rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/ios/ipa.py` & `linktools-0.8.6rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/ios/sib.py` & `linktools-0.8.6rc0/src/linktools/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/ios/struct.py` & `linktools-0.8.6rc0/src/linktools/ios/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from .. import utils
 
 
 class App:
```

### Comparing `linktools-0.8.5rc1/src/linktools/metadata.py` & `linktools-0.8.6rc0/src/linktools/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,30 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
     __repr__ = lambda _: "__missing__"
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.5rc1"
+__version__ = "0.8.6rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.5rc1)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.6rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.5rc1/src/linktools/reactor.py` & `linktools-0.8.6rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.6rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.6rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/rich.py` & `linktools-0.8.6rc0/src/linktools/rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import logging
 import os
 from datetime import datetime
 from typing import TYPE_CHECKING, Optional, Union, List, Dict, Type, TypeVar, TextIO, Iterable
```

### Comparing `linktools-0.8.5rc1/src/linktools/ssh.py` & `linktools-0.8.6rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/utils/__init__.py` & `linktools-0.8.6rc0/src/linktools/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from ._utils import (
     timeoutable, Timeout, InterruptableEvent,
     ignore_error,
     cast, cast_int as int, cast_bool as bool,
```

### Comparing `linktools-0.8.5rc1/src/linktools/utils/_port.py` & `linktools-0.8.6rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/utils/_proxy.py` & `linktools-0.8.6rc0/src/linktools/utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/utils/_subprocess.py` & `linktools-0.8.6rc0/src/linktools/utils/_subprocess.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools/utils/_utils.py` & `linktools-0.8.6rc0/src/linktools/utils/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
       |  |                 |  |  |/----|`---=    |      |
       |  |                 |  |  |   ,/|==== ooo |      ;
       |  |                 |  |  |  // |(((( [33]|    ,"
       |  `-----------------'  |," .;'| |((((     |  ,"
       +-----------------------+  ;;  | |         |,"
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
-   /  oooooooooooooooo  .o.  oooo /,   \,"-----------
-  / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
+   /  oooooooooooooooo  .o.  oooo /,   `,"-----------
+  / ==ooooooooooooooo==.o.  ooo= //   ,``--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import functools
 import getpass
 import gzip
 import hashlib
 import inspect
```

### Comparing `linktools-0.8.5rc1/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.6rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.5rc1
+Version: 0.8.6rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -68,26 +68,37 @@
 # python3 -m pip install --ignore-installed "linktools@ git+https://github.com/ice-black-tea/linktools.git@master"
 ```
 
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
-对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
+对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置，简化调用方式，如：
 
 ```bash
-eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
+# 对于未正确设置PATH环境变量，或者使用venv安装模块
+# 会出现命令找不到的情况（command not found: lt）
+# 可通过以下命令生成alias脚本添加相关命令
+eval "$(python3 -m linktools.cli.commands.common.env --silent alias --shell bash)"
 
+# 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)"  
+
+# 配置全局java环境，指定java版本号（如：11.0.23/17.0.11/22.0.1）
+eval "$(ct-env --silent java 17.0.11 --shell bash)"
+
+# alias简化调用
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
+# alias简化各类工具调用
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools burpsuite"
-alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias jadx="ct-tools --set version=1.5.0 jadx-gui"  # 指定jadx版本号
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
@@ -203,15 +214,15 @@
 </details>
 
 #### 👉 ct-tools
 
 <details>
 <summary>读取配置文件，即可下载使用对应工具，声明了adb、jadx、apktool、baksmali等常用工具</summary>
 
-所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/assets/tools.yml)查看
+所有声明的工具可通过[配置文件](https://raw.githubusercontent.com/ice-black-tea/linktools/master/src/linktools/template/tools.yml)查看
 
 ```
 $ usage: ct-tools [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c | --download | --clear | -d] ...
 
 Tools downloaded from the web
 
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc1/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc1/src/linktools.egg-info/requires.txt` & `linktools-0.8.6rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

