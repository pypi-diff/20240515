# Comparing `tmp/collabconnector-0.1.1715284491.tar.gz` & `tmp/collabconnector-0.1.1715796177.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collabconnector-0.1.1715284491.tar", last modified: Thu May  9 19:54:56 2024, max compression
+gzip compressed data, was "collabconnector-0.1.1715796177.tar", last modified: Wed May 15 18:03:01 2024, max compression
```

## Comparing `collabconnector-0.1.1715284491.tar` & `collabconnector-0.1.1715796177.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.975807 collabconnector-0.1.1715284491/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1715284491/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 19:54:56.975517 collabconnector-0.1.1715284491/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1715284491/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1715284491/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-09 19:54:56.977330 collabconnector-0.1.1715284491/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.478556 collabconnector-0.1.1715284491/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.511376 collabconnector-0.1.1715284491/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.515318 collabconnector-0.1.1715284491/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1715284491/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.517265 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.519300 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.523265 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/AXL.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.483829 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.530594 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.556925 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.589752 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.683589 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.718119 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.760622 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.771569 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.796300 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.806049 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.824790 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.846239 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.869176 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.885990 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.888613 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.891168 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.894017 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.895654 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.897168 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.899084 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.901153 collabconnector-0.1.1715284491/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.902903 collabconnector-0.1.1715284491/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1715284491/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1715284491/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.905287 collabconnector-0.1.1715284491/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1715284491/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1715284491/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.907269 collabconnector-0.1.1715284491/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.920084 collabconnector-0.1.1715284491/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1715284491/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.923418 collabconnector-0.1.1715284491/src/CollabConnector/Webex/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.927438 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/TXT.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/WhatsApp.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.929328 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Consent/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Consent/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Consent/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.946079 collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15624 2024-05-09 19:54:48.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.952632 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.971638 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Phone/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1715284491/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1715284491/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:54:56.973885 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 19:54:56.000000 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4522 2024-05-09 19:54:56.000000 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-09 19:54:56.000000 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-09 19:54:56.000000 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-09 19:54:56.000000 collabconnector-0.1.1715284491/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.295672 collabconnector-0.1.1715796177/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1715796177/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-15 18:03:01.295401 collabconnector-0.1.1715796177/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1715796177/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1715796177/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-15 18:03:01.296864 collabconnector-0.1.1715796177/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.958579 collabconnector-0.1.1715796177/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.969081 collabconnector-0.1.1715796177/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.972719 collabconnector-0.1.1715796177/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1715796177/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.974321 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.975864 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.979719 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/AXL.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.962033 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:00.985734 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.004162 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.028162 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.053610 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.081257 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.127292 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.135278 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.160220 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.167420 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.185322 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.209540 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.232745 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.251272 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.253230 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.255303 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.258043 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.259872 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.261488 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.263288 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.265364 collabconnector-0.1.1715796177/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.267434 collabconnector-0.1.1715796177/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1715796177/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1715796177/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.269679 collabconnector-0.1.1715796177/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1715796177/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1715796177/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.271916 collabconnector-0.1.1715796177/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.273719 collabconnector-0.1.1715796177/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1715796177/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.276481 collabconnector-0.1.1715796177/src/CollabConnector/Webex/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.280801 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/TXT.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/WhatsApp.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.283435 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Consent/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Consent/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Consent/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.286450 collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15750 2024-05-15 18:02:55.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.291491 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.293190 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Phone/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1715796177/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1715796177/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-15 18:03:01.294386 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-15 18:03:00.000000 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4522 2024-05-15 18:03:00.000000 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-15 18:03:00.000000 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-15 18:03:00.000000 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-15 18:03:00.000000 collabconnector-0.1.1715796177/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `collabconnector-0.1.1715284491/LICENSE` & `collabconnector-0.1.1715796177/LICENSE`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/PKG-INFO` & `collabconnector-0.1.1715796177/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1715284491
+Version: 0.1.1715796177
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1715284491/README.md` & `collabconnector-0.1.1715796177/README.md`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/setup.cfg` & `collabconnector-0.1.1715796177/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1715284491
+version = 0.1.1715796177
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CER/CER.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AST/AST.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/AXL.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/CDR.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/CUCM.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/DIME/DIME.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Logs/Logs.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Phone/Phone.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Risport/Risport.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCM/UDS/UDS.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/CUCX/CUCX.py` & `collabconnector-0.1.1715796177/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Expressway/Expressway.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/IOS/IOS.py` & `collabconnector-0.1.1715796177/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/PAWS/PAWS.py` & `collabconnector-0.1.1715796177/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/UCCX/UCCX.py` & `collabconnector-0.1.1715796177/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/REST.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/TXT.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/TXT.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Connect/WhatsApp.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Connect/WhatsApp.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Consent/REST.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Consent/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Consent/__init__.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Consent/__init__.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/ContactCenter.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/ContactCenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,29 +132,29 @@
 
     # get next page for large requests
     @staticmethod
     def find_next_page(call_response):
         return True
 
     #  set headers
-    def headers(self, payload: bool = False):
+    def headers(self, payload: bool = False, debug: bool = False):
         if payload:
             return {
                 "Accept": "application/json",
                 "Content-Type":  "application/json",
                 "Authorization": f"Bearer {self.token.access_token}"
             }
         else:
             return {
                 "Accept": "application/json",
                 "Authorization": f"Bearer {self.token.access_token}"
             }
 
     # basic REST GET
-    def get(self, uri, data={}, page_size=50, page=0):
+    def get(self, uri, data={}, page_size=50, page=0, debug: bool = False):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
         elif uri.find("/v1/") > -1 and self.org_id is not None:
             data['orgId'] = self.org_id
 
         if uri.find("{orgid}") > -1: # remove {orgid} syntax from documentation to make it easy
             uri = uri.replace("/{orgid}/", f"/{self.org_id}/")
@@ -231,15 +231,15 @@
                     TextStyle.error("Webex Admin token invalid.  Generate new token.")
                     return False
 
                 else:
                     TextStyle.error(f"Error sending CC GET to Webex - {uri}{data} {response}{response.text}")
                     return False
 
-    def delete(self, uri):
+    def delete(self, uri, debug: bool = False):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.delete(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                            headers=self.headers(),
@@ -257,15 +257,15 @@
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     TextStyle.error(f"Error sending CC DELETE to Webex - {uri} {response}{response.text}")
                     return False
 
-    def post(self, uri, data):
+    def post(self, uri, data, debug: bool = False):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.post(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                          headers=self.headers(payload =True),
@@ -284,15 +284,15 @@
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     TextStyle.error(f"Error sending POST to Webex - {uri} {response}{response.text}")
                     return False
 
-    def put(self, uri, data):
+    def put(self, uri, data, debug: bool = False):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.put(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                         headers=self.headers(payload =True),
@@ -311,15 +311,15 @@
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     TextStyle.error(f"Error sending PUT to Webex - {uri} {response}{response.text}")
                     return False
 
-    def patch(self, uri, data):
+    def patch(self, uri, data, debug: bool = False):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.patch(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                           headers=self.headers(payload =True),
```

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/ContactCenter/OutputStyle.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/ContactCenter/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/Chat.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/Chat.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/REST.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/Team.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Engage/User.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Phone/Phone.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector/Webex/Webex.py` & `collabconnector-0.1.1715796177/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector.egg-info/PKG-INFO` & `collabconnector-0.1.1715796177/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1715284491
+Version: 0.1.1715796177
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1715284491/src/CollabConnector.egg-info/SOURCES.txt` & `collabconnector-0.1.1715796177/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

