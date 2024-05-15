# Comparing `tmp/itkdb-0.6.5.tar.gz` & `tmp/itkdb-0.6.6.tar.gz`

## Comparing `itkdb-0.6.5.tar` & `itkdb-0.6.6.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itkdb-0.6.5/.gitlab-ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.6.5/.linkcheckerrc
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 itkdb-0.6.5/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.6.5/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.6.5/add_comment.py
--rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.6.5/generatePlots.py
--rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.6.5/getContentSummary.py
--rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.6.5/getInventory.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.6.5/mkdocs.yml
--rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.6.5/registerComponent.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.6.5/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.6.5/ci/pre-commit-update.sh
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/config.md
--rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/examples.md
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/history.md
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/index.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/install.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/macros.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/.overrides/main.html
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/assets/css/custom.css
--rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/meta/authors.md
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/meta/faq.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/reference/gen_ref_nav.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/reference/cli/itkdb.md
--rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts.css
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
--rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
--rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
--rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
--rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
--rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
--rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
--rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
--rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
--rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
--rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/_version.pyi
--rw-r--r--   0        0        0    19627 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/client.py
--rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/commandline.py
--rw-r--r--   0        0        0    15267 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/core.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/eos.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/py.typed
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/responses.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/typing.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/README.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/data/tiny.root
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/models/component.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/models/file.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 itkdb-0.6.5/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/conftest.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_cli.py
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_client.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_image.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_response.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_scripts.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_session.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_user.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_cache.py
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_institution.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_models.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_session.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_user.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_json.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_tests.test_duplicate_test_run.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.6.5/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.6.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.6.5/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.6.5/LICENSE
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.6.5/README.md
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 itkdb-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 itkdb-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itkdb-0.6.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.6.6/.linkcheckerrc
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 itkdb-0.6.6/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.6.6/add_attachment.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.6.6/add_comment.py
+-rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.6.6/generatePlots.py
+-rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.6.6/getContentSummary.py
+-rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.6.6/getInventory.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.6.6/mkdocs.yml
+-rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.6.6/registerComponent.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.6.6/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.6.6/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/config.md
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/examples.md
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/history.md
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/index.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/install.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/macros.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/.overrides/main.html
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/meta/authors.md
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/meta/faq.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/reference/gen_ref_nav.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/reference/cli/itkdb.md
+-rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts.css
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
+-rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
+-rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
+-rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
+-rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
+-rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
+-rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
+-rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
+-rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
+-rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/_version.pyi
+-rw-r--r--   0        0        0    19803 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/client.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/commandline.py
+-rw-r--r--   0        0        0    15267 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/core.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/eos.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/py.typed
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/responses.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/typing.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/caching/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/caching/adapter.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/caching/controller.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/caching/utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/1x1.jpg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/1x1.sh
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/CERN_chain.pem
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/README.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/data/tiny.root
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/models/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/models/component.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/models/file.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/models/institution.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/settings/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 itkdb-0.6.6/src/itkdb/settings/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/conftest.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_cli.py
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_client.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_image.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_response.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_scripts.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_session.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_user.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/test_utils.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_attachments.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_binaryData.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_cache.py
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_components.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_institution.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_models.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_projects.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_session.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_shipments.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_summary.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_testproperties.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_tests.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_user.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/test_warning.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_attachments.test_add_attachment.json
+-rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_image.json
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_json.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_plainText.json
+-rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_issue4.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_add_comment.json
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
+-rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_get.json
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_bulk.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_info_code.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_info_serial.json
+-rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
+-rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
+-rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_componentsv1.json
+-rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_componentsv2.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_institution.test_get.json
+-rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_institution.test_pagination.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_projects.test_list_projects.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_session.test_fake_route.json
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_session.test_invalid_project.json
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_session.test_missing_required.json
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_session.test_no_bearer.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_session.test_unauthorized.json
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_stats.test_get.json
+-rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_summary.test_get_summary.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_tests.test_duplicate_test_run.json
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_tests.test_list_test_types.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_anonymous_login.json
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_bad_login.json
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_good_login.json
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.6.6/tests/integration/cassettes/test_warnings.test_get_component.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.6.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.6.6/COPYING
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.6.6/LICENSE
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.6.6/README.md
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 itkdb-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 itkdb-0.6.6/PKG-INFO
```

### Comparing `itkdb-0.6.5/.gitlab-ci.yml` & `itkdb-0.6.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/.pre-commit-config.yaml` & `itkdb-0.6.6/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.2
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.10.0"
     hooks:
```

### Comparing `itkdb-0.6.5/generatePlots.py` & `itkdb-0.6.6/generatePlots.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/getContentSummary.py` & `itkdb-0.6.6/getContentSummary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/getInventory.py` & `itkdb-0.6.6/getInventory.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/mkdocs.yml` & `itkdb-0.6.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/registerComponent.py` & `itkdb-0.6.6/registerComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tbump.toml` & `itkdb-0.6.6/tbump.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e36 2e35 220a 0a23 2045  t = "0.6.5"..# E
+00000010: 7420 3d20 2230 2e36 2e36 220a 0a23 2045  t = "0.6.6"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 362e  mp version: 0.6.
-00000150: 3520 e286 9220 7b6e 6577 5f76 6572 7369  5 ... {new_versi
+00000150: 3620 e286 9220 7b6e 6577 5f76 6572 7369  6 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `itkdb-0.6.5/ci/pre-commit-update.sh` & `itkdb-0.6.6/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/config.md` & `itkdb-0.6.6/docs/config.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/examples.md` & `itkdb-0.6.6/docs/examples.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/history.md` & `itkdb-0.6.6/docs/history.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 **_Fixed:_**
 
 ## [0.6.5](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.5) - 2024-05-03 ## {: #itkdb-v0.6.5 }
 
 **_Changed:_**
 
-- [itkdb.Client.post][] for `allow_duplicate` was modified in #101 (thanks to [Lingxin Meng](https://gitlab.cern.ch/lmeng) for following up in the [production database meeting](https://indico.cern.ch/event/1408721/) to remove `runNumber` and parameter result fields with `dataType == 'image'` from being used to determine duplicate test runs
+- [itkdb.Client.post][] for `allow_duplicate` was modified in !101, thanks to [Lingxin Meng](https://gitlab.cern.ch/lmeng) for following up in the [production database meeting](https://indico.cern.ch/event/1408721/) to remove `runNumber` and parameter result fields with `dataType == 'image'` from being used to determine duplicate test runs
 
 ## [0.6.4](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.4) - 2024-04-18 ## {: #itkdb-v0.6.4 }
 
 **_Added:_**
 
 - [itkdb.Client.post][] now has a keyword argument `allow_duplicate` which defaults to `True`. If set to `False`, will check if a duplicate object exists before POST'ing it to the production database. Currently, this logic is implemented for `uploadTestRunResults`. Refer to documentation of [itkdb.Client.post][] to see what other endpoints are supported.
```

### Comparing `itkdb-0.6.5/docs/index.md` & `itkdb-0.6.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/install.md` & `itkdb-0.6.6/docs/install.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/macros.py` & `itkdb-0.6.6/docs/macros.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/assets/css/custom.css` & `itkdb-0.6.6/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/assets/images/logo.svg` & `itkdb-0.6.6/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/meta/faq.md` & `itkdb-0.6.6/docs/meta/faq.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/reference/gen_ref_nav.py` & `itkdb-0.6.6/docs/reference/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts.css` & `itkdb-0.6.6/docs/stylesheets/fonts.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2` & `itkdb-0.6.6/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/client.py` & `itkdb-0.6.6/src/itkdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,17 @@
             for key in ["passed", "problems"]:
                 if test_run[key] != new_test_run.get(key, False):
                     log.info(
                         "  - %s does not have the same %s value", test_run["id"], key
                     )
                     test_run_ids.remove(test_run["id"])
                     continue
+            # if the test run has been removed by the previous check then move to the next test run
+            if test_run["id"] not in test_run_ids:
+                continue
 
             # then check properties, defects, comments, parameters
             properties = {
                 prop["code"]: prop["value"]
                 for prop in (test_run.get("properties", []) or [])
             }
             if properties != new_test_run["properties"]:
```

### Comparing `itkdb-0.6.5/src/itkdb/commandline.py` & `itkdb-0.6.6/src/itkdb/commandline.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/core.py` & `itkdb-0.6.6/src/itkdb/core.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/eos.py` & `itkdb-0.6.6/src/itkdb/eos.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/exceptions.py` & `itkdb-0.6.6/src/itkdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/responses.py` & `itkdb-0.6.6/src/itkdb/responses.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/typing.py` & `itkdb-0.6.6/src/itkdb/typing.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/utils.py` & `itkdb-0.6.6/src/itkdb/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/caching/adapter.py` & `itkdb-0.6.6/src/itkdb/caching/adapter.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/caching/controller.py` & `itkdb-0.6.6/src/itkdb/caching/controller.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/caching/utils.py` & `itkdb-0.6.6/src/itkdb/caching/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/data/1x1.sh` & `itkdb-0.6.6/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/data/CERN_chain.pem` & `itkdb-0.6.6/src/itkdb/data/CERN_chain.pem`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/data/README.md` & `itkdb-0.6.6/src/itkdb/data/README.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/models/component.py` & `itkdb-0.6.6/src/itkdb/models/component.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/models/file.py` & `itkdb-0.6.6/src/itkdb/models/file.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/models/institution.py` & `itkdb-0.6.6/src/itkdb/models/institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/src/itkdb/settings/base.py` & `itkdb-0.6.6/src/itkdb/settings/base.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/conftest.py` & `itkdb-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_cli.py` & `itkdb-0.6.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_client.py` & `itkdb-0.6.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_image.py` & `itkdb-0.6.6/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_response.py` & `itkdb-0.6.6/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_scripts.py` & `itkdb-0.6.6/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_session.py` & `itkdb-0.6.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_user.py` & `itkdb-0.6.6/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/test_utils.py` & `itkdb-0.6.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_attachments.py` & `itkdb-0.6.6/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_binaryData.py` & `itkdb-0.6.6/tests/integration/test_binaryData.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_cache.py` & `itkdb-0.6.6/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_components.py` & `itkdb-0.6.6/tests/integration/test_components.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_institution.py` & `itkdb-0.6.6/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_session.py` & `itkdb-0.6.6/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_shipments.py` & `itkdb-0.6.6/tests/integration/test_shipments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_summary.py` & `itkdb-0.6.6/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_testproperties.py` & `itkdb-0.6.6/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_tests.py` & `itkdb-0.6.6/tests/integration/test_tests.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_user.py` & `itkdb-0.6.6/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/test_warning.py` & `itkdb-0.6.6/tests/integration/test_warning.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.6.6/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.6.6/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_empty_file.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_empty_file.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_json.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_json.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.6.6/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.6.6/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.6.6/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.6.6/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.6.6/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.6.6/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.6.6/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.6.6/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.6.6/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.6.6/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.6.6/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.6.6/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.6.6/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.6.6/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.6.6/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_tests.test_duplicate_test_run.json` & `itkdb-0.6.6/tests/integration/cassettes/test_tests.test_duplicate_test_run.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.6.6/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.6.6/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.6.6/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/.gitignore` & `itkdb-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/COPYING` & `itkdb-0.6.6/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/LICENSE` & `itkdb-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.5/README.md` & `itkdb-0.6.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ITk DB v0.6.5
+# ITk DB v0.6.6
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itkdb-0.6.5/pyproject.toml` & `itkdb-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 [tool.hatch.envs.default]
 dependencies = [
     "tbump>=6.7.0",
     "pylint",
     "build",
     "twine",
 ]
+installer = "uv"
 
 [tool.hatch.envs.default.scripts]
 tag = "tbump {args}"
 lint = "pylint src"
 build = "python -m build"
 validate = "twine check dist/*"
 # https://github.com/linkchecker/linkchecker/issues/678
```

### Comparing `itkdb-0.6.5/PKG-INFO` & `itkdb-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkdb
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python wrapper to interface with ITk DB.
 Project-URL: Documentation, https://itkdb.docs.cern.ch/0.6/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>
@@ -42,15 +42,15 @@
 Requires-Dist: urllib3>=1.26.11
 Provides-Extra: contrib
 Requires-Dist: html2text; extra == 'contrib'
 Provides-Extra: eos
 Requires-Dist: pycurl; extra == 'eos'
 Description-Content-Type: text/markdown
 
-# ITk DB v0.6.5
+# ITk DB v0.6.6
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

