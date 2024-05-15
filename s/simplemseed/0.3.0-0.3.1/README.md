# Comparing `tmp/simplemseed-0.3.0.tar.gz` & `tmp/simplemseed-0.3.1.tar.gz`

## Comparing `simplemseed-0.3.0.tar` & `simplemseed-0.3.1.tar`

### file list

```diff
@@ -1,126 +1,128 @@
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 simplemseed-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 simplemseed-0.3.0/build-hints.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/make.bat
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/.gitignore
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/readme_link.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/requirements.txt
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/index.rst
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.exceptions.rst
--rw-r--r--   0        0        0    16453 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.fdsnsourceid.rst
--rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.miniseed.rst
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed2to3.rst
--rw-r--r--   0        0        0    15385 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3.rst
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3details.rst
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3merge.rst
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.rst
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.seedcodec.rst
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steim1.rst
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steim2.rst
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steimframeblock.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/.gitignore
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/fdsnws_mseed3.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/ginormous_ms3.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/long_sid.ms3
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/long_sid.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/minimal_rw_mseed3.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/miniseed2to3.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/read_miniseed2.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/readwrite_miniseed3.py
--rwxr-xr-x   0        0        0      227 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/run_all.sh
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/sourceid.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/test.ms3
--rw-r--r--   0        0        0 13824266 2020-02-02 00:00:00.000000 simplemseed-0.3.0/examples/test_ginormous.ms3
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/__init__.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/bandcode.json
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/exceptions.py
--rw-r--r--   0        0        0    16054 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/fdsnsourceid.py
--rw-r--r--   0        0        0    25371 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/miniseed.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/mseed2to3.py
--rw-r--r--   0        0        0    25756 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/mseed3.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/mseed3details.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/mseed3merge.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/py.typed
--rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/seedcodec.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/sourcecode.json
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/steim1.py
--rw-r--r--   0        0        0    17193 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/steim2.py
--rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 simplemseed-0.3.0/src/simplemseed/steimframeblock.py
--rw-r--r--   0        0        0    44984 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/bird_jsc.ms3
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/casee.mseed2
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/casee.mseed3
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/casee_two.ms3
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_convert2to3.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_mseed2.py
--rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_mseed3.py
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_sourceid.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_steim1.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/test_steim2.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/Makefile
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/README.md
--rw-r--r--   0        0        0    25856 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/appendix-24mapping.rst
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/appendix.rst
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/background.rst
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/changes.rst
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/conf.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/data-encodings.rst
--rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/definition.rst
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/fdsn-reserved.rst
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/make.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/requirements.txt
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/software.rst
--rw-r--r--   0        0        0   122378 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/FDSN-logo.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/favicon.ico
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/css/custom.css
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/css/fdsn_rtd_theme.css
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/css/schema_doc.css
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/js/schema_doc.min.js
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/_static/js/sidebar_context.js
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-All.json
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-Detection.json
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-Other.json
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-TQ-ED.json
--rw-r--r--   0        0        0    23304 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2020-12.json
--rw-r--r--   0        0        0    23305 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2023-07.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-detectiononly.json
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-detectiononly.mseed3
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-detectiononly.txt
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.json
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.mseed3
--rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.txt
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.mseed3
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.txt
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.json
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.mseed3
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.txt
--rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.json
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.mseed3
--rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.txt
--rw-r--r--   0        0        0    12332 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.json
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.mseed3
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.txt
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int16.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int16.mseed3
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int16.txt
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.json
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.mseed3
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.txt
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.mseed3
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.txt
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.mseed3
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.txt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-text.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-text.mseed3
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-text.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 simplemseed-0.3.0/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 simplemseed-0.3.0/LICENSE
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 simplemseed-0.3.0/README.md
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 simplemseed-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 simplemseed-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 simplemseed-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0   206018 2020-02-02 00:00:00.000000 simplemseed-0.3.1/CO_HAW.staxml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 simplemseed-0.3.1/build-hints.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 simplemseed-0.3.1/updatestaxml.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/.gitignore
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/readme_link.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/requirements.txt
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/index.rst
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.exceptions.rst
+-rw-r--r--   0        0        0    16453 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.fdsnsourceid.rst
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.miniseed.rst
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed2to3.rst
+-rw-r--r--   0        0        0    14803 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3.rst
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3details.rst
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3merge.rst
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.rst
+-rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.seedcodec.rst
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steim1.rst
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steim2.rst
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steimframeblock.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/.gitignore
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/fdsnws_mseed3.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/ginormous_ms3.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/long_sid.ms3
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/long_sid.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/minimal_rw_mseed3.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/miniseed2to3.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/read_miniseed2.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/readwrite_miniseed3.py
+-rwxr-xr-x   0        0        0      227 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/run_all.sh
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/sourceid.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/test.ms3
+-rw-r--r--   0        0        0 13824266 2020-02-02 00:00:00.000000 simplemseed-0.3.1/examples/test_ginormous.ms3
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/__init__.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/bandcode.json
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/exceptions.py
+-rw-r--r--   0        0        0    16054 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/fdsnsourceid.py
+-rw-r--r--   0        0        0    25373 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/miniseed.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/mseed2to3.py
+-rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/mseed3.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/mseed3details.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/mseed3merge.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/py.typed
+-rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/seedcodec.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/sourcecode.json
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/steim1.py
+-rw-r--r--   0        0        0    17193 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/steim2.py
+-rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 simplemseed-0.3.1/src/simplemseed/steimframeblock.py
+-rw-r--r--   0        0        0    44984 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/bird_jsc.ms3
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/casee.mseed2
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/casee.mseed3
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/casee_two.ms3
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_convert2to3.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_mseed2.py
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_mseed3.py
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_sourceid.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_steim1.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/test_steim2.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/Makefile
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/README.md
+-rw-r--r--   0        0        0    25856 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/appendix-24mapping.rst
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/appendix.rst
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/background.rst
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/changes.rst
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/conf.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/data-encodings.rst
+-rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/definition.rst
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/fdsn-reserved.rst
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/make.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/requirements.txt
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/software.rst
+-rw-r--r--   0        0        0   122378 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/FDSN-logo.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/favicon.ico
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/css/custom.css
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/css/fdsn_rtd_theme.css
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/css/schema_doc.css
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/js/schema_doc.min.js
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/_static/js/sidebar_context.js
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-All.json
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-Detection.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-Other.json
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-TQ-ED.json
+-rw-r--r--   0        0        0    23304 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2020-12.json
+-rw-r--r--   0        0        0    23305 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2023-07.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-detectiononly.json
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-detectiononly.mseed3
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-detectiononly.txt
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.json
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.mseed3
+-rw-r--r--   0        0        0    13370 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.txt
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.mseed3
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.txt
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.json
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.mseed3
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.txt
+-rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.mseed3
+-rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.txt
+-rw-r--r--   0        0        0    12332 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.json
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.mseed3
+-rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.txt
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int16.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int16.mseed3
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int16.txt
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.mseed3
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.txt
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.mseed3
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.txt
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.mseed3
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.txt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-text.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-text.mseed3
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-text.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 simplemseed-0.3.1/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 simplemseed-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 simplemseed-0.3.1/README.md
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 simplemseed-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 simplemseed-0.3.1/PKG-INFO
```

### Comparing `simplemseed-0.3.0/.readthedocs.yaml` & `simplemseed-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/build-hints.md` & `simplemseed-0.3.1/build-hints.md`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/Makefile` & `simplemseed-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/make.bat` & `simplemseed-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/conf.py` & `simplemseed-0.3.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'SimpleMSeed'
 copyright = '2024, Philip Crotwell'
 author = 'Philip Crotwell'
 release = '0.3'
-version = '0.3.0'
+version = '0.3.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
```

### Comparing `simplemseed-0.3.0/docs/source/index.rst` & `simplemseed-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.exceptions.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.exceptions.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.fdsnsourceid.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.fdsnsourceid.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.miniseed.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.miniseed.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,14 @@
 .. list-table::
    :class: autosummary longtable
    :align: left
 
    * - :py:obj:`B1000_SIZE <simplemseed.miniseed.B1000_SIZE>`
      - .. autodoc2-docstring:: simplemseed.miniseed.B1000_SIZE
           :summary:
-   * - :py:obj:`BIG_ENDIAN <simplemseed.miniseed.BIG_ENDIAN>`
-     - .. autodoc2-docstring:: simplemseed.miniseed.BIG_ENDIAN
-          :summary:
    * - :py:obj:`BTime <simplemseed.miniseed.BTime>`
      - .. autodoc2-docstring:: simplemseed.miniseed.BTime
           :summary:
    * - :py:obj:`Blockette100 <simplemseed.miniseed.Blockette100>`
      - .. autodoc2-docstring:: simplemseed.miniseed.Blockette100
           :summary:
    * - :py:obj:`Blockette1000 <simplemseed.miniseed.Blockette1000>`
@@ -94,17 +91,14 @@
           :summary:
    * - :py:obj:`ENC_SHORT <simplemseed.miniseed.ENC_SHORT>`
      - .. autodoc2-docstring:: simplemseed.miniseed.ENC_SHORT
           :summary:
    * - :py:obj:`HEADER_SIZE <simplemseed.miniseed.HEADER_SIZE>`
      - .. autodoc2-docstring:: simplemseed.miniseed.HEADER_SIZE
           :summary:
-   * - :py:obj:`LITTLE_ENDIAN <simplemseed.miniseed.LITTLE_ENDIAN>`
-     - .. autodoc2-docstring:: simplemseed.miniseed.LITTLE_ENDIAN
-          :summary:
    * - :py:obj:`MAX_INT_PER_512 <simplemseed.miniseed.MAX_INT_PER_512>`
      - .. autodoc2-docstring:: simplemseed.miniseed.MAX_INT_PER_512
           :summary:
    * - :py:obj:`MAX_SHORT_PER_512 <simplemseed.miniseed.MAX_SHORT_PER_512>`
      - .. autodoc2-docstring:: simplemseed.miniseed.MAX_SHORT_PER_512
           :summary:
    * - :py:obj:`MICRO <simplemseed.miniseed.MICRO>`
@@ -116,20 +110,14 @@
 
 .. py:data:: B1000_SIZE
    :canonical: simplemseed.miniseed.B1000_SIZE
    :value: 8
 
    .. autodoc2-docstring:: simplemseed.miniseed.B1000_SIZE
 
-.. py:data:: BIG_ENDIAN
-   :canonical: simplemseed.miniseed.BIG_ENDIAN
-   :value: 1
-
-   .. autodoc2-docstring:: simplemseed.miniseed.BIG_ENDIAN
-
 .. py:data:: BTime
    :canonical: simplemseed.miniseed.BTime
    :value: 'namedtuple(...)'
 
    .. autodoc2-docstring:: simplemseed.miniseed.BTime
 
 .. py:data:: Blockette100
@@ -176,20 +164,14 @@
 
 .. py:data:: HEADER_SIZE
    :canonical: simplemseed.miniseed.HEADER_SIZE
    :value: 48
 
    .. autodoc2-docstring:: simplemseed.miniseed.HEADER_SIZE
 
-.. py:data:: LITTLE_ENDIAN
-   :canonical: simplemseed.miniseed.LITTLE_ENDIAN
-   :value: 0
-
-   .. autodoc2-docstring:: simplemseed.miniseed.LITTLE_ENDIAN
-
 .. py:data:: MAX_INT_PER_512
    :canonical: simplemseed.miniseed.MAX_INT_PER_512
    :value: None
 
    .. autodoc2-docstring:: simplemseed.miniseed.MAX_INT_PER_512
 
 .. py:data:: MAX_SHORT_PER_512
```

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed2to3.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed2to3.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,14 @@
 Data
 ~~~~
 
 .. list-table::
    :class: autosummary longtable
    :align: left
 
-   * - :py:obj:`BIG_ENDIAN <simplemseed.mseed3.BIG_ENDIAN>`
-     - .. autodoc2-docstring:: simplemseed.mseed3.BIG_ENDIAN
-          :summary:
    * - :py:obj:`CRC_OFFSET <simplemseed.mseed3.CRC_OFFSET>`
      - .. autodoc2-docstring:: simplemseed.mseed3.CRC_OFFSET
           :summary:
    * - :py:obj:`ENDIAN <simplemseed.mseed3.ENDIAN>`
      - .. autodoc2-docstring:: simplemseed.mseed3.ENDIAN
           :summary:
    * - :py:obj:`FDSN_PREFIX <simplemseed.mseed3.FDSN_PREFIX>`
@@ -73,33 +70,24 @@
           :summary:
    * - :py:obj:`FIXED_HEADER_SIZE <simplemseed.mseed3.FIXED_HEADER_SIZE>`
      - .. autodoc2-docstring:: simplemseed.mseed3.FIXED_HEADER_SIZE
           :summary:
    * - :py:obj:`HEADER_PACK_FORMAT <simplemseed.mseed3.HEADER_PACK_FORMAT>`
      - .. autodoc2-docstring:: simplemseed.mseed3.HEADER_PACK_FORMAT
           :summary:
-   * - :py:obj:`LITTLE_ENDIAN <simplemseed.mseed3.LITTLE_ENDIAN>`
-     - .. autodoc2-docstring:: simplemseed.mseed3.LITTLE_ENDIAN
-          :summary:
    * - :py:obj:`MINISEED_THREE_MIME <simplemseed.mseed3.MINISEED_THREE_MIME>`
      - .. autodoc2-docstring:: simplemseed.mseed3.MINISEED_THREE_MIME
           :summary:
    * - :py:obj:`UNKNOWN_DATA_VERSION <simplemseed.mseed3.UNKNOWN_DATA_VERSION>`
      - .. autodoc2-docstring:: simplemseed.mseed3.UNKNOWN_DATA_VERSION
           :summary:
 
 API
 ~~~
 
-.. py:data:: BIG_ENDIAN
-   :canonical: simplemseed.mseed3.BIG_ENDIAN
-   :value: 1
-
-   .. autodoc2-docstring:: simplemseed.mseed3.BIG_ENDIAN
-
 .. py:data:: CRC_OFFSET
    :canonical: simplemseed.mseed3.CRC_OFFSET
    :value: 28
 
    .. autodoc2-docstring:: simplemseed.mseed3.CRC_OFFSET
 
 .. py:data:: ENDIAN
@@ -122,20 +110,14 @@
 
 .. py:data:: HEADER_PACK_FORMAT
    :canonical: simplemseed.mseed3.HEADER_PACK_FORMAT
    :value: '<ccBBIHHBBBBdIIBBHI'
 
    .. autodoc2-docstring:: simplemseed.mseed3.HEADER_PACK_FORMAT
 
-.. py:data:: LITTLE_ENDIAN
-   :canonical: simplemseed.mseed3.LITTLE_ENDIAN
-   :value: 0
-
-   .. autodoc2-docstring:: simplemseed.mseed3.LITTLE_ENDIAN
-
 .. py:data:: MINISEED_THREE_MIME
    :canonical: simplemseed.mseed3.MINISEED_THREE_MIME
    :value: 'application/vnd.fdsn.mseed3'
 
    .. autodoc2-docstring:: simplemseed.mseed3.MINISEED_THREE_MIME
 
 .. py:class:: MSeed3Header()
```

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3details.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3details.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.mseed3merge.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.mseed3merge.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
    :canonical: simplemseed.__all__
    :value: ['MiniseedHeader', 'MiniseedRecord', 'MiniseedException', 'unpackMiniseedHeader', 'unpackMiniseedRec...
 
    .. autodoc2-docstring:: simplemseed.__all__
 
 .. py:data:: __version__
    :canonical: simplemseed.__version__
-   :value: '0.3.0'
+   :value: '0.3.1'
 
    .. autodoc2-docstring:: simplemseed.__version__
```

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.seedcodec.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.seedcodec.rst`

 * *Files 11% similar despite different names*

```diff
@@ -41,14 +41,17 @@
           :summary:
    * - :py:obj:`getFloat64 <simplemseed.seedcodec.getFloat64>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.getFloat64
           :summary:
    * - :py:obj:`isFloatCompression <simplemseed.seedcodec.isFloatCompression>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.isFloatCompression
           :summary:
+   * - :py:obj:`isPrimitiveCompression <simplemseed.seedcodec.isPrimitiveCompression>`
+     - .. autodoc2-docstring:: simplemseed.seedcodec.isPrimitiveCompression
+          :summary:
    * - :py:obj:`mseed3EncodingFromArrayTypecode <simplemseed.seedcodec.mseed3EncodingFromArrayTypecode>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.mseed3EncodingFromArrayTypecode
           :summary:
    * - :py:obj:`mseed3EncodingFromNumpyDT <simplemseed.seedcodec.mseed3EncodingFromNumpyDT>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.mseed3EncodingFromNumpyDT
           :summary:
    * - :py:obj:`numpyDTFromMseed3Encoding <simplemseed.seedcodec.numpyDTFromMseed3Encoding>`
@@ -61,14 +64,17 @@
 .. list-table::
    :class: autosummary longtable
    :align: left
 
    * - :py:obj:`ASCII <simplemseed.seedcodec.ASCII>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.ASCII
           :summary:
+   * - :py:obj:`BIG_ENDIAN <simplemseed.seedcodec.BIG_ENDIAN>`
+     - .. autodoc2-docstring:: simplemseed.seedcodec.BIG_ENDIAN
+          :summary:
    * - :py:obj:`CDSN <simplemseed.seedcodec.CDSN>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.CDSN
           :summary:
    * - :py:obj:`DOUBLE <simplemseed.seedcodec.DOUBLE>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.DOUBLE
           :summary:
    * - :py:obj:`DWWSSN <simplemseed.seedcodec.DWWSSN>`
@@ -79,14 +85,17 @@
           :summary:
    * - :py:obj:`INT24 <simplemseed.seedcodec.INT24>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.INT24
           :summary:
    * - :py:obj:`INTEGER <simplemseed.seedcodec.INTEGER>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.INTEGER
           :summary:
+   * - :py:obj:`LITTLE_ENDIAN <simplemseed.seedcodec.LITTLE_ENDIAN>`
+     - .. autodoc2-docstring:: simplemseed.seedcodec.LITTLE_ENDIAN
+          :summary:
    * - :py:obj:`SHORT <simplemseed.seedcodec.SHORT>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.SHORT
           :summary:
    * - :py:obj:`SRO <simplemseed.seedcodec.SRO>`
      - .. autodoc2-docstring:: simplemseed.seedcodec.SRO
           :summary:
    * - :py:obj:`STEIM1 <simplemseed.seedcodec.STEIM1>`
@@ -105,14 +114,20 @@
 .. py:data:: ASCII
    :canonical: simplemseed.seedcodec.ASCII
    :type: int
    :value: 0
 
    .. autodoc2-docstring:: simplemseed.seedcodec.ASCII
 
+.. py:data:: BIG_ENDIAN
+   :canonical: simplemseed.seedcodec.BIG_ENDIAN
+   :value: 1
+
+   .. autodoc2-docstring:: simplemseed.seedcodec.BIG_ENDIAN
+
 .. py:data:: CDSN
    :canonical: simplemseed.seedcodec.CDSN
    :type: int
    :value: 16
 
    .. autodoc2-docstring:: simplemseed.seedcodec.CDSN
 
@@ -194,14 +209,20 @@
 .. py:data:: INTEGER
    :canonical: simplemseed.seedcodec.INTEGER
    :type: int
    :value: 3
 
    .. autodoc2-docstring:: simplemseed.seedcodec.INTEGER
 
+.. py:data:: LITTLE_ENDIAN
+   :canonical: simplemseed.seedcodec.LITTLE_ENDIAN
+   :value: 0
+
+   .. autodoc2-docstring:: simplemseed.seedcodec.LITTLE_ENDIAN
+
 .. py:data:: SHORT
    :canonical: simplemseed.seedcodec.SHORT
    :type: int
    :value: 1
 
    .. autodoc2-docstring:: simplemseed.seedcodec.SHORT
 
@@ -259,14 +280,19 @@
    .. autodoc2-docstring:: simplemseed.seedcodec.getFloat64
 
 .. py:function:: isFloatCompression(compressionType: int) -> bool
    :canonical: simplemseed.seedcodec.isFloatCompression
 
    .. autodoc2-docstring:: simplemseed.seedcodec.isFloatCompression
 
+.. py:function:: isPrimitiveCompression(compressionType: int) -> bool
+   :canonical: simplemseed.seedcodec.isPrimitiveCompression
+
+   .. autodoc2-docstring:: simplemseed.seedcodec.isPrimitiveCompression
+
 .. py:function:: mseed3EncodingFromArrayTypecode(typecode: str, itemsize: int) -> int
    :canonical: simplemseed.seedcodec.mseed3EncodingFromArrayTypecode
 
    .. autodoc2-docstring:: simplemseed.seedcodec.mseed3EncodingFromArrayTypecode
 
 .. py:function:: mseed3EncodingFromNumpyDT(dt: numpy.dtype) -> int
    :canonical: simplemseed.seedcodec.mseed3EncodingFromNumpyDT
```

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steim1.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steim1.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steim2.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steim2.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/docs/source/apidocs/simplemseed/simplemseed.steimframeblock.rst` & `simplemseed-0.3.1/docs/source/apidocs/simplemseed/simplemseed.steimframeblock.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/fdsnws_mseed3.py` & `simplemseed-0.3.1/examples/fdsnws_mseed3.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/ginormous_ms3.py` & `simplemseed-0.3.1/examples/ginormous_ms3.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/long_sid.py` & `simplemseed-0.3.1/examples/long_sid.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/minimal_rw_mseed3.py` & `simplemseed-0.3.1/examples/minimal_rw_mseed3.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/readwrite_miniseed3.py` & `simplemseed-0.3.1/examples/readwrite_miniseed3.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/sourceid.py` & `simplemseed-0.3.1/examples/sourceid.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/test.ms3` & `simplemseed-0.3.1/examples/test.ms3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/examples/test_ginormous.ms3` & `simplemseed-0.3.1/examples/test_ginormous.ms3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/__init__.py` & `simplemseed-0.3.1/src/simplemseed/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 from .mseed3 import (
     unpackMSeed3Record,
     unpackMSeed3FixedHeader,
     readMSeed3Records,
     MSeed3Header,
     MSeed3Record,
@@ -34,14 +34,17 @@
     bandCodeDescribe,
     sourceCodeDescribe,
 )
 from .seedcodec import (
     encode,
     decompress,
     canDecompress,
+    BIG_ENDIAN,
+    LITTLE_ENDIAN,
+    isPrimitiveCompression,
 )
 from .exceptions import (
     CodecException,
     UnsupportedCompressionType,
 )
 from .steim1 import decodeSteim1, encodeSteim1, encodeSteim1FrameBlock
 from .steim2 import decodeSteim2, encodeSteim2, encodeSteim2FrameBlock
@@ -85,8 +88,11 @@
     "encodeSteim2",
     "encodeSteim2FrameBlock",
     "SteimFrameBlock",
     "mseed2to3",
     "crcAsHex",
     "isoWZ",
     "mseed3merge",
+    "BIG_ENDIAN",
+    "LITTLE_ENDIAN",
+    "isPrimitiveCompression",
 ]
```

### Comparing `simplemseed-0.3.0/src/simplemseed/bandcode.json` & `simplemseed-0.3.1/src/simplemseed/bandcode.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/exceptions.py` & `simplemseed-0.3.1/src/simplemseed/exceptions.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/fdsnsourceid.py` & `simplemseed-0.3.1/src/simplemseed/fdsnsourceid.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/miniseed.py` & `simplemseed-0.3.1/src/simplemseed/miniseed.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from .seedcodec import (
     decompress,
     encode,
     mseed3EncodingFromArrayTypecode,
     mseed3EncodingFromNumpyDT,
     EncodedDataSegment,
     numpyDTFromMseed3Encoding,
+    BIG_ENDIAN,
+    LITTLE_ENDIAN,
 )
 
 MICRO = 1000000
 
 EMPTY_SEQ = "      ".encode("UTF-8")
 ENC_SHORT = 1
 ENC_INT = 3
 
-BIG_ENDIAN = 1
-LITTLE_ENDIAN = 0
 
 HEADER_SIZE = 48
 B1000_SIZE = 8
 MAX_INT_PER_512 = (512 - HEADER_SIZE - B1000_SIZE) // 4
 MAX_SHORT_PER_512 = (512 - HEADER_SIZE - B1000_SIZE) // 2
 
 BTime = namedtuple("BTime", "year yday hour minute second tenthMilli")
```

### Comparing `simplemseed-0.3.0/src/simplemseed/mseed2to3.py` & `simplemseed-0.3.1/src/simplemseed/mseed2to3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import argparse
 import json
 
 from .mseed3 import MSeed3Record, MSeed3Header, UNKNOWN_DATA_VERSION
 from .miniseed import MiniseedRecord, MiniseedException, readMiniseed2Records
 from .fdsnsourceid import FDSNSourceId
+from .seedcodec import isPrimitiveCompression, BIG_ENDIAN
 
 
 def mseed2to3(ms2: MiniseedRecord) -> MSeed3Record:
     """
     Very simple conversion of a Miniseed version 2 record to miniseed verion 3.
     Most values in blockettes, other than 100, 1000, 1001 are ignored.
     """
@@ -41,16 +42,20 @@
             b1000 = b
     if b1000 is None:
         raise MiniseedException("Missing blockette 1000")
 
     ms3Header.encoding = b1000.encoding
     ms3Header.publicationVersion = UNKNOWN_DATA_VERSION
     if ms2.encodedData is not None:
-        ms3Header.dataLength = len(ms2.encodedData)
-        data = ms2.encodedData
+        if isPrimitiveCompression(b1000.encoding) and ms2H.byteorder == BIG_ENDIAN:
+            # need to decompress to byte swap primitive array
+            data = ms2.decompressed().byteswap()
+        else:
+            ms3Header.dataLength = len(ms2.encodedData)
+            data = ms2.encodedData
     else:
         data = ms2.decompressed()
     identifier = FDSNSourceId.fromNslc(
         ms2H.network, ms2H.station, ms2H.location, ms2H.channel
     )
 
     ms3Extras = {}
@@ -94,14 +99,15 @@
     if len(fdsnExtras) > 0:
         ms3Extras["FDSN"] = fdsnExtras
     if len(ms3Extras) == 0:
         ms3ExtrasStr = ""
     else:
         ms3ExtrasStr = json.dumps(ms3Extras)
         ms3Header.extraHeadersLength = len(ms3ExtrasStr.encode("UTF-8"))
+
     ms3 = MSeed3Record(ms3Header, str(identifier), data, ms3ExtrasStr)
 
     return ms3
 
 
 def do_parseargs():
     parser = argparse.ArgumentParser(
```

### Comparing `simplemseed-0.3.0/src/simplemseed/mseed3.py` & `simplemseed-0.3.1/src/simplemseed/mseed3.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     STEIM2,
     STEIM3,
     EncodedDataSegment,
     mseed3EncodingFromArrayTypecode,
     mseed3EncodingFromNumpyDT,
     numpyDTFromMseed3Encoding,
     UnsupportedCompressionType,
+    BIG_ENDIAN,
+    LITTLE_ENDIAN,
 )
 from .fdsnsourceid import FDSNSourceId
 
 
 MINISEED_THREE_MIME = "application/vnd.fdsn.mseed3"
 
 # const for unknown data version, 0 */
@@ -42,17 +44,14 @@
 # LITTLE_ENDIAN = True
 ENDIAN = "<"
 
 # const for big endian, false */
 # BIG_ENDIAN = False;
 
 
-BIG_ENDIAN = 1
-LITTLE_ENDIAN = 0
-
 HEADER_PACK_FORMAT = "<ccBBIHHBBBBdIIBBHI"
 
 
 class MSeed3Header:
     """
     Represents the fixed header section of a mseed3 record.
 
@@ -417,15 +416,15 @@
                 + self.header.dataLength
             )
         return None
 
     def encodedDataBytes(self):
         if isinstance(self._data, (bytearray, bytes)):
             return self._data
-        return encode(self._data, self.header.encoding).dataBytes
+        return encode(self._data, self.header.encoding, littleEndian = True).dataBytes
 
     def pack(self):
         """
         Pack the record contents into a bytearray. Header values for the lengths
         are updated, so the record header represents the output bytes after
         packing.
         """
@@ -445,15 +444,15 @@
             extraHeadersStr = ""
         extraHeadersBytes = extraHeadersStr.encode("UTF-8")
         self.header.extraHeadersLength = len(extraHeadersBytes)
         if isinstance(self._data, (bytearray, bytes)):
             # already byte-like, so just use
             dataBytes = self._data
         else:
-            encData = encode(self._data, self.header.encoding)
+            encData = encode(self._data, self.header.encoding, littleEndian=True)
             if encData.compressionType != self.header.encoding:
                 raise Miniseed3Exception(
                     f"Header encoding {self.header.encoding} not same as data {encData.compressionType}"
                 )
             dataBytes = encData.dataBytes
 
         self.header.dataLength = len(dataBytes)
```

### Comparing `simplemseed-0.3.0/src/simplemseed/mseed3details.py` & `simplemseed-0.3.1/src/simplemseed/mseed3details.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/mseed3merge.py` & `simplemseed-0.3.1/src/simplemseed/mseed3merge.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/seedcodec.py` & `simplemseed-0.3.1/src/simplemseed/seedcodec.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 import numpy
 
 from .exceptions import CodecException, UnsupportedCompressionType
 from .steim1 import decodeSteim1
 from .steim2 import decodeSteim2
 
 
+BIG_ENDIAN = 1
+LITTLE_ENDIAN = 0
+
 # ascii
 ASCII: int = 0
 
 # 16 bit integer, or java short
 SHORT: int = 1
 
 # 24 bit integer
@@ -61,14 +64,20 @@
     True if the compression is not representable by integers, so not
     compressable via the standard compression types.
     """
     if compressionType in (FLOAT, DOUBLE):
         return True
     return False
 
+def isPrimitiveCompression(compressionType: int) -> bool:
+    """
+    True if the compression is one of the primitive types, short, int
+    float or double.
+    """
+    return compressionType in (SHORT, INTEGER, FLOAT, DOUBLE)
 
 class EncodedDataSegment:
     """
     A holder for compressed data independent of the file format.
     """
 
     compressionType: int
@@ -178,15 +187,15 @@
 def encode(data, encoding=None, littleEndian=True):
     """
     Encode the given numpy.ndarray or array.array into bytes.
 
     Note that currently no actual compression is done, the resulting
     bytes will occupy the same space, just converted for output.
     If encoding is not given, the encoding will be guessed from the array type.
-    If endian is given, defaults to little endian.
+    If endian is not given, defaults to little endian.
     """
     if isinstance(data, (bytearray, bytes)):
         # already byte-like, so ???
         raise UnsupportedCompressionType("Unable to encode data, already bytes-like")
     if encoding is None or encoding < 0:
         # try to guess a primitive encoding
         if isinstance(data, numpy.ndarray):
```

### Comparing `simplemseed-0.3.0/src/simplemseed/sourcecode.json` & `simplemseed-0.3.1/src/simplemseed/sourcecode.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/steim1.py` & `simplemseed-0.3.1/src/simplemseed/steim1.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/steim2.py` & `simplemseed-0.3.1/src/simplemseed/steim2.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/src/simplemseed/steimframeblock.py` & `simplemseed-0.3.1/src/simplemseed/steimframeblock.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/bird_jsc.ms3` & `simplemseed-0.3.1/tests/bird_jsc.ms3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/casee.mseed2` & `simplemseed-0.3.1/tests/casee.mseed2`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/casee_two.ms3` & `simplemseed-0.3.1/tests/casee_two.ms3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/test_convert2to3.py` & `simplemseed-0.3.1/tests/test_convert2to3.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/test_mseed2.py` & `simplemseed-0.3.1/tests/test_mseed2.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/test_mseed3.py` & `simplemseed-0.3.1/tests/test_mseed3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import json
 import numpy
 import os
+import sys
 import simplemseed
 from datetime import datetime
 from pathlib import Path
 
 TEST_DIR = Path(__file__).parent
 
 githubUrl = "git clone https://github.com/FDSN/miniSEED3.git"
@@ -244,10 +245,38 @@
             == simplemseed.seedcodec.DOUBLE
         )
         assert (
             simplemseed.seedcodec.mseed3EncodingFromArrayTypecode("d", 8)
             == simplemseed.seedcodec.DOUBLE
         )
 
+    def testCreateFromBigEndian(self):
+        data = numpy.array([1, 256, 8755, -16245, 65000, -65000], dtype=numpy.dtype('<i4'))
+        bigdata = data.newbyteorder('>').byteswap()
+        assert(data.dtype.byteorder == '<'
+               or (data.dtype.byteorder == '=' and sys.byteorder == 'little'))
+        assert(bigdata.dtype.byteorder == '>')
+        for i in range(len(data)):
+            assert(data[i] == bigdata[i])
+
+        header = simplemseed.MSeed3Header()
+        identifier = simplemseed.FDSNSourceId.createUnknown(header.sampleRate)
+        record = simplemseed.MSeed3Record(header, identifier, data)
+        recordBytes = record.pack()
+        bigrecord = simplemseed.MSeed3Record(header, identifier, bigdata)
+        bigrecordBytes = bigrecord.pack()
+        outRecord = simplemseed.unpackMSeed3Record(recordBytes)
+        assert identifier == outRecord.parseIdentifier()
+        decomp_data = outRecord.decompress()
+
+        bigoutRecord = simplemseed.unpackMSeed3Record(bigrecordBytes)
+        assert identifier == bigoutRecord.parseIdentifier()
+        bigdecomp_data = bigoutRecord.decompress()
+        for i in range(len(data)):
+            assert data[i] == decomp_data[i]
+            assert data[i] == bigdecomp_data[i]
+
+
+
 
 if __name__ == "__main__":
     TestMSeed3().test_ref_data()
```

### Comparing `simplemseed-0.3.0/tests/test_sourceid.py` & `simplemseed-0.3.1/tests/test_sourceid.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/test_steim1.py` & `simplemseed-0.3.1/tests/test_steim1.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/test_steim2.py` & `simplemseed-0.3.1/tests/test_steim2.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/Makefile` & `simplemseed-0.3.1/tests/miniSEED3/Makefile`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/README.md` & `simplemseed-0.3.1/tests/miniSEED3/README.md`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/appendix-24mapping.rst` & `simplemseed-0.3.1/tests/miniSEED3/appendix-24mapping.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/appendix.rst` & `simplemseed-0.3.1/tests/miniSEED3/appendix.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/background.rst` & `simplemseed-0.3.1/tests/miniSEED3/background.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/conf.py` & `simplemseed-0.3.1/tests/miniSEED3/conf.py`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/data-encodings.rst` & `simplemseed-0.3.1/tests/miniSEED3/data-encodings.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/definition.rst` & `simplemseed-0.3.1/tests/miniSEED3/definition.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/extra-headers.rst` & `simplemseed-0.3.1/tests/miniSEED3/extra-headers.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/fdsn-reserved.rst` & `simplemseed-0.3.1/tests/miniSEED3/fdsn-reserved.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/index.rst` & `simplemseed-0.3.1/tests/miniSEED3/index.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/make.bat` & `simplemseed-0.3.1/tests/miniSEED3/make.bat`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/software.rst` & `simplemseed-0.3.1/tests/miniSEED3/software.rst`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/FDSN-logo.png` & `simplemseed-0.3.1/tests/miniSEED3/_static/FDSN-logo.png`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/favicon.ico` & `simplemseed-0.3.1/tests/miniSEED3/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/css/fdsn_rtd_theme.css` & `simplemseed-0.3.1/tests/miniSEED3/_static/css/fdsn_rtd_theme.css`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/css/schema_doc.css` & `simplemseed-0.3.1/tests/miniSEED3/_static/css/schema_doc.css`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/js/schema_doc.min.js` & `simplemseed-0.3.1/tests/miniSEED3/_static/js/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/_static/js/sidebar_context.js` & `simplemseed-0.3.1/tests/miniSEED3/_static/js/sidebar_context.js`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-All.json` & `simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-All.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-TQ-ED.json` & `simplemseed-0.3.1/tests/miniSEED3/extra-headers/Example-ExtraHeaders-FDSN-TQ-ED.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2020-12.json` & `simplemseed-0.3.1/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2020-12.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2023-07.json` & `simplemseed-0.3.1/tests/miniSEED3/extra-headers/ExtraHeaders-FDSN-v1.0.schema-2023-07.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-detectiononly.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-detectiononly.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-detectiononly.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-detectiononly.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-All.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-FDSN-Other.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-TQ-TC-ED.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float32.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float32.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-float64.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-float64.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int16.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int16.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int16.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int16.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-int32.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-int32.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim1.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim1.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.mseed3` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.mseed3`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-sinusoid-steim2.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-sinusoid-steim2.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-text.json` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-text.json`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/tests/miniSEED3/reference-data/reference-text.txt` & `simplemseed-0.3.1/tests/miniSEED3/reference-data/reference-text.txt`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/.gitignore` & `simplemseed-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/LICENSE` & `simplemseed-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/README.md` & `simplemseed-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/pyproject.toml` & `simplemseed-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simplemseed-0.3.0/PKG-INFO` & `simplemseed-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simplemseed
-Version: 0.3.0
+Version: 0.3.1
 Summary: miniseed3 in pure python
 Project-URL: Homepage, https://github.com/crotwell/simplemseed
 Project-URL: Documentation, https://simplemseed.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/crotwell/simplemseed
 Project-URL: Issues, https://github.com/crotwell/simplemseed/issues
 Author-email: Philip Crotwell <crotwell@seis.sc.edu>
 License-File: LICENSE
```

