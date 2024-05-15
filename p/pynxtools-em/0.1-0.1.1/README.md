# Comparing `tmp/pynxtools_em-0.1.tar.gz` & `tmp/pynxtools_em-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools_em-0.1.tar", last modified: Fri Apr 26 16:40:09 2024, max compression
+gzip compressed data, was "pynxtools_em-0.1.1.tar", last modified: Wed May 15 07:26:16 2024, max compression
```

## Comparing `pynxtools_em-0.1.tar` & `pynxtools_em-0.1.1.tar`

### file list

```diff
@@ -1,162 +1,156 @@
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.544473 pynxtools_em-0.1/.github/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.544473 pynxtools_em-0.1/.github/workflows/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.github/workflows/build_docs.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      745 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.github/workflows/publish.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      855 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.github/workflows/pylint.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      764 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.github/workflows/pytest.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3882 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.gitignore
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      200 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.precommit-config.yaml
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.544473 pynxtools_em-0.1/.vscode/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      506 2024-04-26 16:38:47.000000 pynxtools_em-0.1/.vscode/settings.json
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11357 2024-04-26 16:38:47.000000 pynxtools_em-0.1/LICENSE
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     4991 2024-04-26 16:40:09.552473 pynxtools_em-0.1/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3501 2024-04-26 16:38:47.000000 pynxtools_em-0.1/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9869 2024-04-26 16:38:47.000000 pynxtools_em-0.1/dev-requirements.txt
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.544473 pynxtools_em-0.1/docs/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.544473 pynxtools_em-0.1/docs/explanation/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8630 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/explanation/implementation.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      524 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/explanation/learn.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/explanation/media/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      419 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/explanation/media/workflow.mermaid
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   101879 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/explanation/media/workflow.png
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/how-tos/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        9 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/howto.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      849 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/kikuchi.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/how-tos/media/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      419 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/media/kikuchi.mermaid
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   118857 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/media/kikuchi.png
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2311 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/mtex.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2003 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/how-tos/pyxem.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1884 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/index.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      526 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/macros.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/reference/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      369 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/apex.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2147 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/contextualization.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      184 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/nion.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      438 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/png.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      391 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/tiff.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      370 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/reference/vemd.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/stylesheets/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1097 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/stylesheets/extra.css
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/tutorial/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/docs/tutorial/media/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    69876 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/tutorial/media/upload-processing.gif
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       31 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/tutorial/nexusio.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      513 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/tutorial/oasis.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1048 2024-04-26 16:38:47.000000 pynxtools_em-0.1/docs/tutorial/standalone.md
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      451 2024-04-26 16:38:47.000000 pynxtools_em-0.1/eln.batch.sh
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/examples/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2019 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/README_Ebsd.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1166 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/README_Nion.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1150 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/README_Spctrscpy.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10861 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/Write.NXem_ebsd.Example.1.ipynb
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7944 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/Write.NXem_nion.Example.1.ipynb
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9277 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/Write.NXem_spctrscpy.Example.1.ipynb
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      251 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/eln_data.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1711 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/eln_data_em_nion.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2121 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/eln_data_em_om.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1367 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/eln_data_em_spctrscpy.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      793 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/em.oasis.specific.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11254 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/image_png_protochips_to_nexus.ods
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11631 2024-04-26 16:38:47.000000 pynxtools_em-0.1/examples/image_tiff_tfs_to_nexus.ods
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      896 2024-04-26 16:38:47.000000 pynxtools_em-0.1/hfive.batch.sh
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     1101 2024-04-26 16:38:47.000000 pynxtools_em-0.1/imgs.batch.sh
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1241 2024-04-26 16:38:47.000000 pynxtools_em-0.1/mkdocs.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6940 2024-04-26 16:38:47.000000 pynxtools_em-0.1/nexus_concept_resolving.ipynb
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/pynxtools_em/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3193 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/__init__.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/pynxtools_em/concepts/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       79 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    12029 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/concept_mapper.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2317 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/nxs_concepts.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2249 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/nxs_em_eds_indexing.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3006 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/nxs_image_r_set.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2665 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/nxs_object.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3219 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/concepts/nxs_spectrum_set.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/pynxtools_em/config/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      643 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2183 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/eln_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4994 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/image_png_protochips_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3385 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/image_tiff_tfs_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1357 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/oasis_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5340 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/config/rsciio_velox_cfg.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/pynxtools_em/examples/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      366 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/examples/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9629 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/examples/ebsd_database.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.548473 pynxtools_em-0.1/pynxtools_em/geometry/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      153 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3207 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/convention_mapper.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2281 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/euler_angle_convention.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5170 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/geometry.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    23913 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/handed_cartesian.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1808 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/geometry/msmse_convention.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6773 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/pynxtools_em/subparsers/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       85 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    41754 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_apex.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    24984 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_base.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    13840 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_bruker.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3385 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_concept.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21527 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_dreamthreed.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    13984 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_ebsd.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16208 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_edax.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2405 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_emsoft.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    15522 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/hfive_oxford.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1891 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/image_base.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    20320 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/image_png_protochips.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4995 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    14769 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff_tfs.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8332 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff_tfs_concepts.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2918 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/nxs_imgs.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7423 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/nxs_mtex.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    17275 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/nxs_nion.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    40630 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/nxs_pyxem.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4392 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/oasis_config_reader.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8047 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/oasis_eln_reader.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2184 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_base.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3031 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_bruker.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    30565 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_velox.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/pynxtools_em/utils/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       85 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1124 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/get_file_checksum.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1195 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/get_gitrepo_commit.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4521 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/get_scan_points.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8239 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/get_sqr_grid.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1379 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/get_xrayline_iupac_names.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3908 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/hfive_utils.py
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      793 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/hfive_web_constants.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1064 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/hfive_web_utils.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1668 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/image_processing.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1431 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/image_utils.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4204 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/io_case_logic.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1415 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/nion_utils.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2007 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/nx_default_plots.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3420 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/rsciio_hspy_utils.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1251 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/sorting.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1496 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/string_conversions.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      869 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/string_encoding.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1698 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pynxtools_em/utils/xml_utils.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/pynxtools_em.egg-info/
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     4991 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4509 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       53 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/entry_points.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      243 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/requires.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       13 2024-04-26 16:40:09.000000 pynxtools_em-0.1/pynxtools_em.egg-info/top_level.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2606 2024-04-26 16:38:47.000000 pynxtools_em-0.1/pyproject.toml
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     1688 2024-04-26 16:38:47.000000 pynxtools_em-0.1/rsciio_velox.batch.sh
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3929 2024-04-26 16:38:47.000000 pynxtools_em-0.1/rsciio_velox.ipynb
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-04-26 16:40:09.552473 pynxtools_em-0.1/setup.cfg
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/tests/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/tests/data/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      182 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/README.Ebsd.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      193 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/README.Spctrscpy.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      193 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/README_Nion.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        2 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/config_file.json
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:40:09.552473 pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    50534 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.ebsd.schema.archive.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21715 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.nion.schema.archive.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21854 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.spctrscpy.schema.archive.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1861 2024-04-26 16:38:47.000000 pynxtools_em-0.1/tests/test_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.680426 pynxtools_em-0.1.1/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.660425 pynxtools_em-0.1.1/.github/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.660425 pynxtools_em-0.1.1/.github/workflows/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.github/workflows/build_docs.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      745 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.github/workflows/publish.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      855 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.github/workflows/pylint.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      764 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.github/workflows/pytest.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3882 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.gitignore
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      200 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.precommit-config.yaml
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.660425 pynxtools_em-0.1.1/.vscode/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      506 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/.vscode/settings.json
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11357 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/LICENSE
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     5127 2024-05-15 07:26:16.680426 pynxtools_em-0.1.1/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3506 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    14445 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/dev-requirements.txt
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.660425 pynxtools_em-0.1.1/docs/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.660425 pynxtools_em-0.1.1/docs/explanation/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8630 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/explanation/implementation.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      524 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/explanation/learn.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/explanation/media/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      419 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/explanation/media/workflow.mermaid
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   101879 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/explanation/media/workflow.png
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/how-tos/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        9 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/howto.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      849 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/kikuchi.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/how-tos/media/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      419 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/media/kikuchi.mermaid
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   118857 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/media/kikuchi.png
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2311 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/mtex.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2003 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/how-tos/pyxem.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1884 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/index.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      526 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/macros.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/reference/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      369 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/apex.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2147 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/contextualization.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      184 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/nion.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      438 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/png.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      391 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/tiff.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      370 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/reference/vemd.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/stylesheets/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1097 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/stylesheets/extra.css
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/tutorial/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/docs/tutorial/media/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    69876 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/tutorial/media/upload-processing.gif
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       31 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/tutorial/nexusio.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      513 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/tutorial/oasis.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1048 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/docs/tutorial/standalone.md
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      451 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/eln.batch.sh
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.664425 pynxtools_em-0.1.1/examples/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8675 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/examples/HowToUseTutorial.ipynb
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1313 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/examples/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      425 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/examples/eln_data.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      793 2024-04-26 16:38:47.000000 pynxtools_em-0.1.1/examples/em.oasis.specific.yaml
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      896 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/hfive.batch.sh
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     1101 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/imgs.batch.sh
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1241 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/mkdocs.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6940 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/nexus_concept_resolving.ipynb
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.668425 pynxtools_em-0.1.1/pynxtools_em/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3193 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/__init__.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.668425 pynxtools_em-0.1.1/pynxtools_em/concepts/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       79 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11503 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/concept_mapper.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16374 2024-05-11 14:17:44.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/mapping_functors.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1732 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_concepts.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2249 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_em_eds_indexing.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3006 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_image_r_set.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2613 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_object.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3219 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_spectrum_set.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.668425 pynxtools_em-0.1.1/pynxtools_em/config/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      643 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/config/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2507 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/config/eln_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4994 2024-05-11 11:09:54.000000 pynxtools_em-0.1.1/pynxtools_em/config/image_png_protochips_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3385 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/config/image_tiff_tfs_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1352 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/config/oasis_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5340 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/config/rsciio_velox_cfg.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.668425 pynxtools_em-0.1.1/pynxtools_em/examples/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      366 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/examples/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9629 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/examples/ebsd_database.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.668425 pynxtools_em-0.1.1/pynxtools_em/geometry/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      153 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3207 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/convention_mapper.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2281 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/euler_angle_convention.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5170 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/geometry.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    23913 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/handed_cartesian.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1808 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/geometry/msmse_convention.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6223 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.672425 pynxtools_em-0.1.1/pynxtools_em/subparsers/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       85 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    41754 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_apex.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    24984 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_base.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    13840 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_bruker.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3385 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_concept.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21527 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_dreamthreed.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    13984 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_ebsd.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16208 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_edax.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2405 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_emsoft.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    15505 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_oxford.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1938 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/image_base.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    20546 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/image_png_protochips.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4995 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    14979 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff_tfs.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8332 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff_tfs_concepts.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2918 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_imgs.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7423 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_mtex.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    17199 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_nion.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    40733 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_pyxem.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3554 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/oasis_config_reader.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4022 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/oasis_eln_reader.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2184 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_base.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3031 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_bruker.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    30825 2024-05-15 07:21:31.000000 pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_velox.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.676425 pynxtools_em-0.1.1/pynxtools_em/utils/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       85 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1124 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/get_file_checksum.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1195 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/get_gitrepo_commit.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4492 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/get_scan_points.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8208 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/get_sqr_grid.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1379 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/get_xrayline_iupac_names.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3908 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/hfive_utils.py
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      793 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/hfive_web_constants.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1064 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/hfive_web_utils.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1639 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/image_processing.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1431 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/image_utils.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1249 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/interpret_boolean.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4150 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/io_case_logic.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1386 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/nion_utils.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4989 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/nx_default_plots.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3420 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/rsciio_hspy_utils.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1251 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/sorting.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1496 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/string_conversions.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      869 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/string_encoding.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1155 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pynxtools_em/utils/versioning.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1698 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/pynxtools_em/utils/xml_utils.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.676425 pynxtools_em-0.1.1/pynxtools_em.egg-info/
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     5127 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4294 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       53 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/entry_points.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      279 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/requires.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       13 2024-05-15 07:26:16.000000 pynxtools_em-0.1.1/pynxtools_em.egg-info/top_level.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2662 2024-05-10 11:47:51.000000 pynxtools_em-0.1.1/pyproject.toml
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     1688 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/rsciio_velox.batch.sh
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3929 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/rsciio_velox.ipynb
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-05-15 07:26:16.680426 pynxtools_em-0.1.1/setup.cfg
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.676425 pynxtools_em-0.1.1/tests/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.676425 pynxtools_em-0.1.1/tests/data/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      182 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/README.Ebsd.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      193 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/README.Spctrscpy.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      193 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/README_Nion.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        2 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/config_file.json
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:26:16.676425 pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    50534 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.ebsd.schema.archive.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21715 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.nion.schema.archive.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    21854 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.spctrscpy.schema.archive.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1861 2024-05-08 10:42:58.000000 pynxtools_em-0.1.1/tests/test_reader.py
```

### Comparing `pynxtools_em-0.1/.github/workflows/build_docs.yml` & `pynxtools_em-0.1.1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/.github/workflows/publish.yml` & `pynxtools_em-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/.github/workflows/pylint.yml` & `pynxtools_em-0.1.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/.github/workflows/pytest.yml` & `pynxtools_em-0.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/.gitignore` & `pynxtools_em-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/LICENSE` & `pynxtools_em-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/PKG-INFO` & `pynxtools_em-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-em
-Version: 0.1
+Version: 0.1.1
 Summary: Make electron microscopy results interoperable via NeXus
 Author-email: Markus Kühbach <markus.kuehbach@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-em
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-em/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,14 +32,17 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: jupyterlab-h5web; extra == "dev"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/pylint.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/pynxtools-em)
 ![](https://img.shields.io/pypi/l/pynxtools-em)
@@ -83,15 +86,15 @@
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-em.git --branch main --recursive pynxtools_em
 cd pynxtools_em
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
```

### Comparing `pynxtools_em-0.1/README.md` & `pynxtools_em-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-em.git --branch main --recursive pynxtools_em
 cd pynxtools_em
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
```

### Comparing `pynxtools_em-0.1/dev-requirements.txt` & `pynxtools_em-0.1.1/dev-requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,54 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev --extra=docs --output-file=dev-requirements.txt pyproject.toml
 #
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
+argon2-cffi==23.1.0
+    # via jupyter-server
+argon2-cffi-bindings==21.2.0
+    # via argon2-cffi
+arrow==1.3.0
+    # via isoduration
 asciitree==0.3.3
     # via zarr
 ase==3.22.1
     # via pynxtools
 asteval==0.9.32
     # via lmfit
 asttokens==2.4.1
     # via stack-data
+async-lru==2.0.4
+    # via jupyterlab
+attrs==23.2.0
+    # via
+    #   jsonschema
+    #   referencing
 babel==2.14.0
-    # via mkdocs-material
+    # via
+    #   jupyterlab-server
+    #   mkdocs-material
+beautifulsoup4==4.12.3
+    # via nbconvert
+bleach==6.1.0
+    # via nbconvert
 build==1.2.1
     # via pip-tools
 certifi==2024.2.2
-    # via requests
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
+cffi==1.16.0
+    # via argon2-cffi-bindings
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   click-default-group
     #   dask
     #   mkdocs
@@ -30,15 +57,17 @@
 click-default-group==1.2.4
     # via pynxtools
 cloudpickle==3.0.0
     # via dask
 colorama==0.4.6
     # via mkdocs-material
 comm==0.2.2
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipywidgets
 contourpy==1.2.0
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 dask[array]==2024.4.0
     # via
     #   hyperspy
@@ -48,14 +77,16 @@
     #   rosettasciio
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via
     #   ipyparallel
     #   ipython
+defusedxml==0.7.1
+    # via nbconvert
 diffpy-structure==3.1.0
     # via
     #   diffsims
     #   kikuchipy
     #   orix
 diffsims==0.5.2
     # via
@@ -69,48 +100,66 @@
     # via stack-data
 fabio==2023.10.0
     # via
     #   pyfai
     #   silx
 fasteners==0.19
     # via zarr
+fastjsonschema==2.19.1
+    # via nbformat
 flatdict==4.0.1
     # via pynxtools-em (pyproject.toml)
 fonttools==4.50.0
     # via matplotlib
+fqdn==1.5.1
+    # via jsonschema
 fsspec==2024.3.1
     # via
     #   dask
     #   hyperspy
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
 greenlet==3.0.3
     # via sqlalchemy
+h11==0.14.0
+    # via httpcore
+h5grove==2.1.0
+    # via jupyterlab-h5web
 h5py==3.10.0
     # via
     #   fabio
+    #   h5grove
     #   hdf5plugin
     #   hyperspy
+    #   jupyterlab-h5web
     #   kikuchipy
     #   nionswift
     #   orix
     #   pyfai
     #   pynxtools
     #   pyxem
     #   silx
 hdf5plugin==4.4.0
     # via fabio
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
 hyperspy==1.7.6
     # via
     #   kikuchipy
     #   pyxem
 idna==3.6
-    # via requests
+    # via
+    #   anyio
+    #   httpx
+    #   jsonschema
+    #   requests
 imageio==2.27.0
     # via
     #   hyperspy
     #   kikuchipy
     #   nionswift
     #   nionswift-io
     #   nionui
@@ -119,40 +168,109 @@
     # via
     #   dask
     #   hyperspy
     #   pynxtools
 iniconfig==2.0.0
     # via pytest
 ipykernel==6.29.4
-    # via ipyparallel
+    # via
+    #   ipyparallel
+    #   jupyter
+    #   jupyter-console
+    #   jupyterlab
+    #   qtconsole
 ipyparallel==8.7.0
     # via hyperspy
 ipython==8.23.0
     # via
     #   hyperspy
     #   ipykernel
     #   ipyparallel
+    #   ipywidgets
+    #   jupyter-console
+ipywidgets==8.1.2
+    # via jupyter
+isoduration==20.11.0
+    # via jsonschema
 jedi==0.19.1
     # via ipython
 jinja2==3.1.3
     # via
     #   hyperspy
+    #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   mkdocs
     #   mkdocs-macros-plugin
     #   mkdocs-material
+    #   nbconvert
 joblib==1.3.2
     # via scikit-learn
+json5==0.9.25
+    # via jupyterlab-server
+jsonpointer==2.4
+    # via jsonschema
+jsonschema[format-nongpl]==4.22.0
+    # via
+    #   jupyter-events
+    #   jupyterlab-server
+    #   nbformat
+jsonschema-specifications==2023.12.1
+    # via jsonschema
+jupyter==1.0.0
+    # via pynxtools-em (pyproject.toml)
 jupyter-client==8.6.1
     # via
     #   ipykernel
     #   ipyparallel
+    #   jupyter-console
+    #   jupyter-server
+    #   nbclient
+    #   qtconsole
+jupyter-console==6.6.3
+    # via jupyter
 jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
+    #   jupyter-console
+    #   jupyter-server
+    #   jupyterlab
+    #   nbclient
+    #   nbconvert
+    #   nbformat
+    #   qtconsole
+jupyter-events==0.10.0
+    # via jupyter-server
+jupyter-lsp==2.2.5
+    # via jupyterlab
+jupyter-server==2.14.0
+    # via
+    #   jupyter-lsp
+    #   jupyterlab
+    #   jupyterlab-h5web
+    #   jupyterlab-server
+    #   notebook
+    #   notebook-shim
+jupyter-server-terminals==0.5.3
+    # via jupyter-server
+jupyterlab==4.1.8
+    # via
+    #   notebook
+    #   pynxtools-em (pyproject.toml)
+jupyterlab-h5web==12.1.0
+    # via pynxtools-em (pyproject.toml)
+jupyterlab-pygments==0.3.0
+    # via nbconvert
+jupyterlab-server==2.27.1
+    # via
+    #   jupyterlab
+    #   notebook
+jupyterlab-widgets==3.0.10
+    # via ipywidgets
 kikuchipy==0.9.0
     # via pynxtools-em (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lazy-loader==0.3
     # via scikit-image
 llvmlite==0.42.0
@@ -170,14 +288,15 @@
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
+    #   nbconvert
 matplotlib==3.8.3
     # via
     #   ase
     #   diffsims
     #   hyperspy
     #   kikuchipy
     #   matplotlib-scalebar
@@ -190,14 +309,16 @@
     #   ipython
 matplotlib-scalebar==0.8.1
     # via orix
 mergedeep==1.3.4
     # via
     #   mkdocs
     #   pynxtools
+mistune==3.0.2
+    # via nbconvert
 mkdocs==1.5.3
     # via
     #   mkdocs-macros-plugin
     #   mkdocs-material
     #   pynxtools-em (pyproject.toml)
 mkdocs-macros-plugin==1.0.5
     # via pynxtools-em (pyproject.toml)
@@ -211,14 +332,25 @@
     # via sympy
 mypy==1.9.0
     # via pynxtools-em (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
 natsort==8.4.0
     # via hyperspy
+nbclient==0.10.0
+    # via nbconvert
+nbconvert==7.16.4
+    # via
+    #   jupyter
+    #   jupyter-server
+nbformat==5.10.4
+    # via
+    #   jupyter-server
+    #   nbclient
+    #   nbconvert
 nest-asyncio==1.6.0
     # via ipykernel
 networkx==3.2.1
     # via scikit-image
 niondata==15.6.2
     # via
     #   nionswift
@@ -231,14 +363,20 @@
     # via nionswift
 nionutils==0.4.10
     # via
     #   niondata
     #   nionswift
     #   nionswift-io
     #   nionui
+notebook==7.1.3
+    # via jupyter
+notebook-shim==0.2.4
+    # via
+    #   jupyterlab
+    #   notebook
 numba==0.59.1
     # via
     #   diffsims
     #   hyperspy
     #   kikuchipy
     #   orix
     #   pyxem
@@ -253,14 +391,15 @@
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   dask
     #   diffsims
     #   fabio
+    #   h5grove
     #   h5py
     #   hyperspy
     #   imageio
     #   kikuchipy
     #   lmfit
     #   matplotlib
     #   niondata
@@ -290,34 +429,46 @@
 numpy-quaternion==2023.0.3
     # via orix
 orix==0.11.1
     # via
     #   diffsims
     #   kikuchipy
     #   pyxem
+orjson==3.10.3
+    # via h5grove
+overrides==7.7.0
+    # via jupyter-server
 packaging==24.0
     # via
     #   build
     #   dask
     #   hyperspy
     #   ipykernel
+    #   jupyter-server
+    #   jupyterlab
+    #   jupyterlab-server
     #   matplotlib
     #   mkdocs
+    #   nbconvert
     #   pooch
     #   pytest
+    #   qtconsole
+    #   qtpy
     #   scikit-image
     #   silx
     #   xarray
     #   xraydb
 paginate==0.5.6
     # via mkdocs-material
 pandas==2.2.1
     # via
     #   pynxtools
     #   xarray
+pandocfilters==1.5.1
+    # via nbconvert
 parso==0.8.3
     # via jedi
 partd==1.4.1
     # via dask
 pathspec==0.12.1
     # via mkdocs
 pexpect==4.9.0
@@ -348,34 +499,45 @@
     # via pycifrw
 pooch==1.8.1
     # via
     #   kikuchipy
     #   orix
 prettytable==3.10.0
     # via hyperspy
+prometheus-client==0.20.0
+    # via jupyter-server
 prompt-toolkit==3.0.43
-    # via ipython
+    # via
+    #   ipython
+    #   jupyter-console
 psutil==5.9.8
     # via
     #   diffsims
     #   ipykernel
     #   ipyparallel
     #   pyxem
 ptyprocess==0.7.0
-    # via pexpect
+    # via
+    #   pexpect
+    #   terminado
 pure-eval==0.2.2
     # via stack-data
 pycifrw==4.4.6
     # via diffpy-structure
+pycparser==2.22
+    # via cffi
 pyfai==2024.2.0
     # via pyxem
 pygments==2.17.2
     # via
     #   ipython
+    #   jupyter-console
     #   mkdocs-material
+    #   nbconvert
+    #   qtconsole
 pymdown-extensions==10.8
     # via mkdocs-material
 pynxtools==0.2.1
     # via pynxtools-em (pyproject.toml)
 pyparsing==3.1.2
     # via matplotlib
 pyproject-hooks==1.0.0
@@ -384,55 +546,84 @@
     #   pip-tools
 pytest==8.1.1
     # via pynxtools-em (pyproject.toml)
 python-box==6.1.0
     # via rosettasciio
 python-dateutil==2.9.0.post0
     # via
+    #   arrow
     #   ghp-import
     #   hyperspy
     #   ipyparallel
     #   jupyter-client
     #   matplotlib
     #   mkdocs-macros-plugin
     #   pandas
     #   rosettasciio
+python-json-logger==2.0.7
+    # via jupyter-events
 pytz==2024.1
     # via
     #   nionswift
     #   pandas
 pyxem==0.16.0
     # via pynxtools-em (pyproject.toml)
 pyyaml==6.0.1
     # via
     #   dask
     #   hyperspy
+    #   jupyter-events
     #   kikuchipy
     #   mkdocs
     #   mkdocs-macros-plugin
     #   pymdown-extensions
     #   pynxtools
     #   pyyaml-env-tag
     #   rosettasciio
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==25.1.2
     # via
     #   ipykernel
     #   ipyparallel
     #   jupyter-client
+    #   jupyter-console
+    #   jupyter-server
+    #   qtconsole
+qtconsole==5.5.2
+    # via jupyter
+qtpy==2.4.1
+    # via qtconsole
+referencing==0.35.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   jupyter-events
 regex==2024.4.16
     # via mkdocs-material
 requests==2.31.0
     # via
     #   hyperspy
+    #   jupyterlab-server
     #   mkdocs-material
     #   pooch
+rfc3339-validator==0.1.4
+    # via
+    #   jsonschema
+    #   jupyter-events
+rfc3986-validator==0.1.1
+    # via
+    #   jsonschema
+    #   jupyter-events
 rosettasciio==0.4
     # via pynxtools-em (pyproject.toml)
+rpds-py==0.18.1
+    # via
+    #   jsonschema
+    #   referencing
 ruff==0.3.4
     # via pynxtools-em (pyproject.toml)
 scikit-image==0.22.0
     # via
     #   hyperspy
     #   kikuchipy
     #   pyxem
@@ -452,98 +643,143 @@
     #   orix
     #   pyfai
     #   pyxem
     #   scikit-image
     #   scikit-learn
     #   sparse
     #   xraydb
+send2trash==1.8.3
+    # via jupyter-server
 silx==2.0.1
     # via pyfai
 six==1.16.0
     # via
     #   asttokens
+    #   bleach
     #   diffpy-structure
     #   python-dateutil
+    #   rfc3339-validator
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
+soupsieve==2.5
+    # via beautifulsoup4
 sparse==0.15.1
     # via hyperspy
 sqlalchemy==2.0.29
     # via xraydb
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via hyperspy
 termcolor==2.4.0
     # via mkdocs-macros-plugin
+terminado==0.18.1
+    # via
+    #   jupyter-server
+    #   jupyter-server-terminals
 threadpoolctl==3.4.0
     # via scikit-learn
 tifffile==2024.2.12
     # via
+    #   h5grove
     #   hyperspy
     #   scikit-image
+tinycss2==1.3.0
+    # via nbconvert
 toolz==0.12.1
     # via
     #   dask
     #   hyperspy
     #   partd
 tornado==6.4
     # via
     #   ipykernel
     #   ipyparallel
     #   jupyter-client
+    #   jupyter-server
+    #   jupyterlab
+    #   notebook
+    #   terminado
 tqdm==4.66.2
     # via
     #   diffsims
     #   hyperspy
     #   ipyparallel
     #   kikuchipy
     #   orix
     #   pyxem
 traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipyparallel
     #   ipython
+    #   ipywidgets
     #   jupyter-client
+    #   jupyter-console
     #   jupyter-core
+    #   jupyter-events
+    #   jupyter-server
+    #   jupyterlab
     #   matplotlib-inline
+    #   nbclient
+    #   nbconvert
+    #   nbformat
+    #   qtconsole
 traits==6.4.3
     # via
     #   hyperspy
     #   pyxem
 transforms3d==0.4.1
     # via
     #   diffsims
     #   pyxem
+types-python-dateutil==2.9.0.20240316
+    # via arrow
 types-pyyaml==6.0.12.20240311
     # via pynxtools-em (pyproject.toml)
 typing-extensions==4.10.0
     # via
+    #   h5grove
     #   ipython
     #   mypy
     #   pint
     #   sqlalchemy
 tzdata==2024.1
     # via pandas
 tzlocal==5.2
     # via
     #   nionswift
     #   pynxtools-em (pyproject.toml)
 uncertainties==3.1.7
     # via lmfit
+uri-template==1.3.0
+    # via jsonschema
 urllib3==2.2.1
     # via requests
 watchdog==4.0.0
     # via mkdocs
 wcwidth==0.2.13
     # via
     #   prettytable
     #   prompt-toolkit
+webcolors==1.13
+    # via jsonschema
+webencodings==0.5.1
+    # via
+    #   bleach
+    #   tinycss2
+websocket-client==1.8.0
+    # via jupyter-server
 wheel==0.43.0
     # via pip-tools
+widgetsnbextension==4.0.10
+    # via ipywidgets
 xarray==2024.3.0
     # via pynxtools
 xmltodict==0.13.0
     # via pynxtools-em (pyproject.toml)
 xraydb==4.5.4
     # via pynxtools-em (pyproject.toml)
 zarr==2.17.1
```

### Comparing `pynxtools_em-0.1/docs/explanation/implementation.md` & `pynxtools_em-0.1.1/docs/explanation/implementation.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/explanation/learn.md` & `pynxtools_em-0.1.1/docs/explanation/learn.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/explanation/media/workflow.png` & `pynxtools_em-0.1.1/docs/explanation/media/workflow.png`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/how-tos/kikuchi.md` & `pynxtools_em-0.1.1/docs/how-tos/kikuchi.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/how-tos/media/kikuchi.png` & `pynxtools_em-0.1.1/docs/how-tos/media/kikuchi.png`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/how-tos/mtex.md` & `pynxtools_em-0.1.1/docs/how-tos/mtex.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/how-tos/pyxem.md` & `pynxtools_em-0.1.1/docs/how-tos/pyxem.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/index.md` & `pynxtools_em-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/macros.py` & `pynxtools_em-0.1.1/docs/macros.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/reference/contextualization.md` & `pynxtools_em-0.1.1/docs/reference/contextualization.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/stylesheets/extra.css` & `pynxtools_em-0.1.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/tutorial/media/upload-processing.gif` & `pynxtools_em-0.1.1/docs/tutorial/media/upload-processing.gif`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/tutorial/oasis.md` & `pynxtools_em-0.1.1/docs/tutorial/oasis.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/docs/tutorial/standalone.md` & `pynxtools_em-0.1.1/docs/tutorial/standalone.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/examples/Write.NXem_ebsd.Example.1.ipynb` & `pynxtools_em-0.1.1/examples/HowToUseTutorial.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8887760659819484%*

 * *Differences: {"'cells'": "{0: {'source': ['# How to convert electron microscopy (meta)data to NeXus/HDF5']}, 1: "*

 * *            "{'metadata': {replace: OrderedDict()}, 'source': ['The aim of this tutorial is to "*

 * *            'guide users how to create a NeXus/HDF5 file to parse and normalize pieces of '*

 * *            "information<br>\\n', 'from typical file formats of the electron microscopy community "*

 * *            "into a common form. The tool assures that this NeXus file<br>\\n', 'matches to the "*

 * *            'NXem applic […]*

```diff
@@ -1,14 +1,30 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Using dataconverter/em_om for mapping EBSD/Orientation Microscopy to NeXus/HDF5/NXem_ebsd"
+                "# How to convert electron microscopy (meta)data to NeXus/HDF5"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The aim of this tutorial is to guide users how to create a NeXus/HDF5 file to parse and normalize pieces of information<br>\n",
+                "from typical file formats of the electron microscopy community into a common form. The tool assures that this NeXus file<br>\n",
+                "matches to the NXem application definition. Such documented conceptually, the file can be used for sharing electron<br>\n",
+                "microscopy research with others (colleagues, project partners, the public), for uploading a summary of the (meta)data to<br>\n",
+                "public repositories and thus avoid additional work that typically comes with having to write documentation of metadata<br>\n",
+                "in such repositories by hand but use a research data management system like NOMAD Oasis instead.<br>\n",
+                "\n",
+                "The benefit of the data normalization that pynxtools-em performs is that all pieces of information are represents in the<br>\n",
+                "same conceptual way with the benefit that most of the so far required format conversions when interfacing with software<br>\n",
+                "from the technology partners or scientific community are no longer necessary.<br>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
@@ -26,20 +42,18 @@
                 "- How to set up a development environment as in the main README  \n",
                 "- Lauch the jupyter lab from this environement as in the README of folder `examples`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "! pip list | grep \"h5py\\|nexus\\|jupyter\" && jupyter serverextension list && jupyter labextension list && python -V"
+                "! pip list | grep \"h5py\\|nexus\\|jupyter\\|jupyterlab_h5web\\|pynxtools\\|pynxtools-em\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Set the pynxtools directory and start H5Web for interactive exploring of HDF5 files."
@@ -48,308 +62,152 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
+                "import zipfile as zp\n",
+                "import numpy as np\n",
                 "from jupyterlab_h5web import H5Web\n",
                 "print(f\"Current working directory: {os.getcwd()}\")\n",
-                "print(f\"So-called base, home, or root directory of the pynxtools: {os.getcwd().replace('/examples/em_om', '')}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### **Step 2:** Download EM-OM-specific example data or use your own datasets."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "Example data can be found on Zenodo https://dx.doi.org/10.5281/zenodo.7885531."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import zipfile as zp"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "! curl --output em_om_sprint14_01.zip https://zenodo.org/record/7885531/files/em_om_sprint14_01.zip\n",
-                "! curl --output em_om_sprint14_02.zip https://zenodo.org/record/7885531/files/em_om_sprint14_02.zip"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "zp.ZipFile(\"em_om_sprint14_01.zip\").extractall(path=\"\", members=None, pwd=None)\n",
-                "zp.ZipFile(\"em_om_sprint14_02.zip\").extractall(path=\"\", members=None, pwd=None)"
+                "print(f\"So-called base, home, or root directory of the pynxtools: {os.getcwd().replace('/examples/em', '')}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "These files should serve exclusively as examples. <font color=\"orange\">The dataconverter for EM-OM always requires at least one file</font>:\n",
-                "\n",
-                "**When you only would like to store conventions**:<br>\n",
-                "* **YAML file with metadata** (either edited manually or via an ELN).<br>\n",
-                "  The eln_data_em_om.yaml file in the example can be edited with a text editor.\n",
-                "\n",
-                "**When you would like to store conventions surplus stack of simulated Kikuchi images**:<br>\n",
-                "* **YAML file with metadata**<br>\n",
-                "* **ZIP archive with images all using the same format, rectangular dimensions, and file type**<br>\n",
-                "\n",
-                "**When you would like to store conventions surplus H5OINA EBSD mapping**:<br>\n",
-                "* **YAML file with metadata**<br>\n",
-                "* **H5OINA file as obtained from Oxford Instrument AZTec (>=5.0)**<br>\n",
-                "\n",
-                "**When you would like to store conventions surplus have transcoded EBSD results from MTex**:<br>\n",
-                "* **YAML file with metadata**<br>\n",
-                "* **\\*.mtex file as obtained by running the specific MTex to NeXus transcoder** (see second info box below for details)<br>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-block alert-info\">\n",
-                "For GUI-based editing, a NOMAD OASIS instance is needed.<br>\n",
-                "</div>"
+                "### **Step 2:** Use your own data or download an example"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-block alert-danger\">\n",
-                "Please note that the metadata inside the provided eln_data_em_om.yaml file are example values.<br>\n",
-                "These reflect not necessarily the conditions when the raw data for the example were collected!<br>\n",
-                "The file is meant to be edited by you if you work with datasets others than the here provided!<br>\n",
-                "</div>"
+                "Please note that the metadata inside the provided em.oasis.specific.yaml and eln_data_apm.yaml files<br>\n",
+                "contain exemplar values. These do not necessarily reflect the conditions when the raw data of example<br>\n",
+                "above-mentioned were collected by the scientists. Instead, these file are meant to be edited by you,<br>\n",
+                "either and preferably programmatically e.g. using output from an electronic lab notebook or manually.</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<div class=\"alert alert-block alert-info\">\n",
-                "Feel free to contact the maintainer of this example to learn more about the parsing capabilities of SEM/EBSD data in NOMAD.<br>\n",
-                "We have also a draft version which supports importing results from MatLab/MTex and DREAM.3D. We would like to get in contact<br>\n",
-                "to document and develop these further, ideally using as diverse examples as possible, maybe also including one of your examples?<br>\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "### **Step 3:** Run the EBSD-specific dataconverter on the example data."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Now we run our parser. The --reader flag takes the em_om reader, the --nxdl flag takes the application definition for this technique NXem_ebsd."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### **Step 3a:** Optionally see the command line help of the dataconverter."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "! dataconverter --help"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### **Step 3b:** Optionally explore all paths which NXem provides."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "! dataconverter --nxdl NXem_ebsd --reader em_om --generate-template"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### **Step 3c**: Convert the files in the example into an NXem_ebsd-compliant NeXus/HDF5 file."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-block alert-info\">\n",
-                "In what follows we will show several of the examples that have been implemented for SEM/EBSD.<br>\n",
-                "</div>"
+                "This example shows the types of files from which the parser collects and normalizes pieces of information:<br>\n",
+                "* **eln_data.yaml** metadata collected with an electronic lab notebook (ELN) such as a NOMAD Oasis custom schema<br>\n",
+                "* **em.oasis.specific.yaml** frequently used metadata that are often the same for many datasets to avoid having to<br>\n",
+                "  type it every time in ELN templates. This file can be considered a configuration file whereby e.g. coordinate system<br>\n",
+                "  conventions can be injected or details about the atom probe instrument communicated if that is part of frequently used<br>\n",
+                "  lab equipment. The benefit of such an approach is that eventual all relevant metadata to an instrument can be read from\n",
+                "  this configuration file via guiding the user e.g. through the ELN with an option to select the instrument.<br>\n",
+                "* **collected data** in community, technology partner format with images, spectra, and other metadata.<br>\n",
+                "\n",
+                "The tool several of the currently frequently used file formats of the electron microscopy community. Given that there is<br>\n",
+                "though a large number of these and different versions users should also be aware that we had to prioritize the implementation<br>\n",
+                "strongly. We cannot implement every request to add support for further formats or additional pieces of information in those<br>\n",
+                "formats we currently do support with the resources in the FAIRmat project. Nevertheless, please raise an issue to document<br>\n",
+                "where we should place our priorities.<br>\n",
+                "Consult the reference part of the documentation to get a detailed view on how specific formats are supported.<br>"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "#### Only conventions:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
-            "source": [
-                "# parser-nexus/tests/data/tools/dataconverter/readers/em/\n",
-                "output_file_name = [\"em_om.case0.nxs\"]\n",
-                "! dataconverter \\\n",
-                "--reader em_om \\\n",
-                "--nxdl NXem_ebsd \\\n",
-                "--input-file eln_data_em_om.yaml \\\n",
-                "--output \"em_om.case0.nxs\""
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
             "source": [
-                "#### Conventions and different data sources:"
+                "### **Step 3:** Run the parser"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "scrolled": true,
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "#parser-nexus/tests/data/tools/dataconverter/readers/em_om/\n",
-                "import numpy as np\n",
-                "eln_data_file_name = [\"eln_data_em_om.yaml\"]\n",
-                "input_data_file_name = [\"PrcShanghaiShi.EBSPs70deg.zip\",\n",
-                "                        \"H5OINA_examples_Specimen_1_Map_EDS_+_EBSD_Map_Data_2.h5oina\",\n",
-                "                        \"Forsterite.ctf.mtex\",\n",
-                "                        \"SmallIN100_Final.dream3d\"]\n",
-                "output_file_name = [\"em_om.case1.nxs\",\n",
-                "                    \"em_om.case2.nxs\",\n",
-                "                    \"em_om.case3e.nxs\",\n",
-                "                    \"em_om.case4.nxs\"]\n",
-                "for case_id in np.arange(0, 3 + 1):\n",
-                "    ELN = eln_data_file_name[0]\n",
-                "    INPUT = input_data_file_name[case_id]\n",
+                "eln_data = [\"eln_data.yaml\"]\n",
+                "deployment_specific = [\"em.oasis.specific.yaml\"]\n",
+                "tech_partner = [\"CHANGEME YOUR TECH PARTNER FILE (e.g. EMD, Nion, etc.)\"]\n",
+                "output_file_name = [\"em.nxs\"]\n",
+                "for case_id in np.arange(0, 1):\n",
+                "    ELN = eln_data[case_id]\n",
+                "    CFG = deployment_specific[case_id]\n",
+                "    DATA = tech_partner[case_id]\n",
                 "    OUTPUT = output_file_name[case_id]\n",
                 "\n",
-                "    ! dataconverter --reader em_om --nxdl NXem_ebsd --input-file $ELN --input-file $INPUT --output $OUTPUT"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The key take home message is that the command above-specified triggers the automatic creation of the HDF5 file. This *.nxs file, is an HDF5 file."
+                "    # CHANGEME activate the following line\n",
+                "    # ! dataconverter convert $ELN $CFG $DATA --reader em --nxdl NXem --output $OUTPUT"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "### **Step 4:** Inspect the HDF5/NeXus file using H5Web"
+                "### **Step 4:** Inspect the NeXus/HDF5 file using H5Web."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# H5Web(OUTPUT)\n",
-                "H5Web(\"em_om.case0.nxs\")\n",
-                "# H5Web(\"em_om.case1.nxs\")\n",
-                "# H5Web(\"em_om.case2.nxs\")\n",
-                "# H5Web(\"em_om.case3e.nxs\")\n",
-                "# H5Web(\"em_om.case4.nxs\")"
+                "# CHANGEME activate the following line to view the data\n",
+                "# H5Web(OUTPUT)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here is where the general template ends. Continue with filling in the notebook with your own post-processing of this *.nxs file."
+                "The NeXus file an also be viewed with H5Web by opening it via the file explorer panel to the left side of this Jupyter lab window."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Conclusions:\n",
                 "***"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Contact person for this example in FAIRmat:\n",
-                "Markus K\u00fchbach"
+                "This tutorial showed how you can call the pynxtools-em parser via a jupyter notebook. This opens many possibilities<br>\n",
+                "like processing the results further with Python such as through e.g. <a href=\"https://conda.io/projects/conda/en/latest/user-guide/install/index.html\">conda</a> on your local computer, <a href=\"https://docs.python.org/3/tutorial/venv.html\">a virtual environment</a><br>\n",
+                "or to interface with community software to do further processing of your data.<br>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Contact person for the apm reader and related examples in FAIRmat:\n",
-                "Markus K\u00fchbach, 2023/08/31<br>\n",
+                "### Contact person for pynxtools-apm and related examples in FAIRmat:\n",
+                "Dr.-Ing. Markus K\u00fchbach, 2024/05/10<br>\n",
                 "\n",
                 "### Funding\n",
                 "<a href=\"https://www.fairmat-nfdi.eu/fairmat\">FAIRmat</a> is a consortium on research data management which is part of the German NFDI.<br>\n",
                 "The project is funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) \u2013 project 460197019."
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -360,18 +218,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "fb9c1bd38c7663f011bf442e740f4844d912585f80182885cfafffa0a1ff37a6"
-            }
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pynxtools_em-0.1/examples/em.oasis.specific.yaml` & `pynxtools_em-0.1.1/examples/em.oasis.specific.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/hfive.batch.sh` & `pynxtools_em-0.1.1/hfive.batch.sh`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/imgs.batch.sh` & `pynxtools_em-0.1.1/imgs.batch.sh`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/mkdocs.yaml` & `pynxtools_em-0.1.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/nexus_concept_resolving.ipynb` & `pynxtools_em-0.1.1/nexus_concept_resolving.ipynb`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/README.md` & `pynxtools_em-0.1.1/pynxtools_em/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/concept_mapper.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/concept_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Utilities for working with NeXus concepts encoded as Python dicts in the concepts dir."""
 
+# these mapping functions are considered deprecated and
+# should be replaced with those from mapping_functors !!
+
 from datetime import datetime
-import pytz
+
 import flatdict as fd
 import numpy as np
+import pytz
 
+from pynxtools_em.concepts.mapping_functors import variadic_path_to_specific_path
 from pynxtools_em.utils.string_conversions import string_to_number
 
 
 def load_from_modifier(terms, fd_dct):
     """Implement modifier which reads values of different type from fd_dct."""
     if isinstance(terms, str):
         if terms in fd_dct.keys():
@@ -90,33 +95,15 @@
             # with the jsonmap reader Sherjeel conceptualized "link"
             return None
     if isinstance(modifier, str):
         return modifier
     return None
 
 
-def variadic_path_to_specific_path(path: str, instance_identifier: list):
-    """Transforms a variadic path to an actual path with instances."""
-    if (path is not None) and (path != ""):
-        narguments = path.count("*")
-        if narguments == 0:  # path is not variadic
-            return path
-        if len(instance_identifier) >= narguments:
-            tmp = path.split("*")
-            if len(tmp) == narguments + 1:
-                nx_specific_path = ""
-                for idx in range(0, narguments):
-                    nx_specific_path += f"{tmp[idx]}{instance_identifier[idx]}"
-                    idx += 1
-                nx_specific_path += f"{tmp[-1]}"
-                return nx_specific_path
-    return None
-
-
-def add_specific_metadata(
+def add_specific_metadata_deprecate(
     concept_mapping: dict, orgmeta: fd.FlatDict, identifier: list, template: dict
 ) -> dict:
     """Map specific concept src on specific NeXus concept trg.
 
     concept_mapping: translation dict how trg and src are to be mapped
     orgmeta: instance data of src concepts
     identifier: list of identifier to resolve variadic paths
```

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/nxs_concepts.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_concepts.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,53 +13,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Implement NeXus-specific groups and fields to document software and versions used."""
 
-from pynxtools_em.concepts.concept_mapper import variadic_path_to_specific_path
+from pynxtools_em.concepts.mapping_functors import add_specific_metadata
+from pynxtools_em.utils.versioning import NX_EM_EXEC_NAME, NX_EM_EXEC_VERSION
 
-
-PYNXTOOLS_EM_VERSION = "Redundant, see metadata in NXroot header"
-PYNXTOOLS_EM_URL = "Redundant, see metadata in NXroot header"
-
-NXEM_NAME = "NXem"
-NXEM_VERSION = "Redundant, see metadata in NXroot header"
-NXEM_URL = "Redundant, see metadata in NXroot header"
-
-EM_APPDEF = {
-    "prefix": "/ENTRY[entry*]",
+EM_PYNX_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]/profiling",
     "use": [
-        ("PROGRAM[program1]/program", "pynxtools/dataconverter/readers/em"),
-        ("PROGRAM[program1]/program/@version", PYNXTOOLS_EM_VERSION),
-        ("PROGRAM[program1]/program/@url", PYNXTOOLS_EM_URL),
-        ("definition", NXEM_NAME),
-        ("definition/@version", NXEM_VERSION),
-        ("definition/@url", NXEM_URL),
+        ("PROGRAM[program1]/program", NX_EM_EXEC_NAME),
+        ("PROGRAM[program1]/program/@version", NX_EM_EXEC_VERSION),
     ],
 }
 
 
 class NxEmAppDef:
     """Add NeXus NXem appdef specific contextualization."""
 
     def __init__(self):
         pass
 
     def parse(
         self, template: dict, entry_id: int = 1, cmd_line_args: tuple = ()
     ) -> dict:
         """Parse application definition."""
-        variadic_prefix = EM_APPDEF["prefix"]
-        for entry in EM_APPDEF["use"]:
-            if isinstance(entry, tuple) and len(entry) == 2:
-                trg = variadic_path_to_specific_path(
-                    f"{variadic_prefix}/{entry[0]}", [entry_id]
-                )
-                template[trg] = entry[1]
+        identifier = [entry_id]
+        add_specific_metadata(EM_PYNX_TO_NEXUS, {}, identifier, template)
 
-        if cmd_line_args != [] and all(isinstance(item, str) for item in cmd_line_args):
-            template[f"/ENTRY[entry{entry_id}]/profiling/command_line_call"] = (
+        if cmd_line_args != () and all(isinstance(item, str) for item in cmd_line_args):
+            template[f"/ENTRY[entry{entry_id}]/profiling/command_line_call"] = " ".join(
                 cmd_line_args
             )
         return template
```

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/nxs_em_eds_indexing.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_em_eds_indexing.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/nxs_image_r_set.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_image_r_set.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/nxs_object.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """NXobject (element of a labelled property graph) to store instance data."""
 
-# pylint: disable=no-member,too-few-public-methods
+from typing import Dict
 
 import numpy as np
 
-from typing import Dict
-
 
 class NxObject:
     """An object in a graph e.g. an attribute, dataset, or group in NeXus."""
 
     def __init__(
         self, name: str = None, unit: str = None, dtype=None, value=None, **kwargs
     ):
```

### Comparing `pynxtools_em-0.1/pynxtools_em/concepts/nxs_spectrum_set.py` & `pynxtools_em-0.1.1/pynxtools_em/concepts/nxs_spectrum_set.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/config/README.md` & `pynxtools_em-0.1.1/pynxtools_em/config/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/config/eln_cfg.py` & `pynxtools_em-0.1.1/pynxtools_em/config/eln_cfg.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,37 +26,54 @@
 #           e.g. in the example below "name" means
 #           ("/ENTRY[entry*]/USER[user*]/name, "load", "name")
 #           if pair load the value pointed to by src and copy into trg
 #       difference between load and map_to is that load assumes no e.g. string to real
 #       conversion is required while map_does not assume this
 #       and instead does the conversion also
 
-EM_EXAMPLE_ENTRY_TO_NEXUS = {
-    "prefix": "/ENTRY[entry*]",
-    "load": ["experiment_alias"],
-    "iso8601": ["start_time"],
+EM_ENTRY_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]",
+    "prefix_src": "entry/",
+    "map_to_str": [
+        "experiment_alias",
+        "start_time",
+        "end_time",
+        "experiment_description",
+    ],
 }
 
 
-EM_EXAMPLE_SAMPLE_TO_NEXUS = {
-    "prefix": "/ENTRY[entry*]/sample",
-    "load": ["method", "atom_types"],
-    "iso8601": ["preparation_date"],
+EM_SAMPLE_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]/sample",
+    "prefix_src": "sample/",
+    "map_to_str": [("thickness/@units", "thickness/unit")],
+    "map": [
+        "method",
+        "name",
+        "atom_types",
+        "preparation_date",
+        ("thickness", "thickness/value"),
+    ],
 }
 
 
-EM_EXAMPLE_USER_TO_NEXUS = {
-    "prefix": "/ENTRY[entry*]/USER[user*]",
-    "use": [
-        ("IDENTIFIER[identifier]/identifier", "orcid"),
-        ("IDENTIFIER[identifier]/service", "orcid"),
-        ("IDENTIFIER[identifier]/is_persistent", False),
-    ],
-    "load": [
+EM_USER_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]/USER[user*]",
+    "map": [
         "name",
         "affiliation",
         "address",
         "email",
         "telephone_number",
         "role",
     ],
 }
+
+
+EM_USER_IDENTIFIER_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]/USER[user*]",
+    "use": [
+        ("IDENTIFIER[identifier]/identifier", "orcid"),
+        ("IDENTIFIER[identifier]/service", "orcid"),
+        ("IDENTIFIER[identifier]/is_persistent", True),
+    ],
+}
```

### Comparing `pynxtools_em-0.1/pynxtools_em/config/image_png_protochips_cfg.py` & `pynxtools_em-0.1.1/pynxtools_em/config/image_png_protochips_cfg.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/config/image_tiff_tfs_cfg.py` & `pynxtools_em-0.1.1/pynxtools_em/config/image_tiff_tfs_cfg.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/config/oasis_cfg.py` & `pynxtools_em-0.1.1/pynxtools_em/config/oasis_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 """Dict mapping values for a specifically configured NOMAD Oasis."""
 
 # see specific comments about the design that should be moved to mkdocs
 
 # import datetime as dt
 # f"{dt.datetime.now(dt.timezone.utc).isoformat().replace('+00:00', 'Z')}",
 
-EM_EXAMPLE_CSYS_TO_NEXUS = {
-    "prefix": "/ENTRY[entry*]/coordinate_system_set/COORDINATE_SYSTEM[coordinate_system*]",
-    "load": [
+EM_CSYS_TO_NEXUS = {
+    "prefix_trg": "/ENTRY[entry*]/coordinate_system_set/COORDINATE_SYSTEM[coordinate_system*]",
+    "map": [
         "alias",
         "type",
         "handedness",
         ("x_direction", "xaxis_direction"),
         ("x_alias", "xaxis_alias"),
         ("y_direction", "yaxis_direction"),
         ("y_alias", "yaxis_alias"),
```

### Comparing `pynxtools_em-0.1/pynxtools_em/config/rsciio_velox_cfg.py` & `pynxtools_em-0.1.1/pynxtools_em/config/rsciio_velox_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
         ("tilt1", "Stage/AlphaTilt"),
         ("tilt2", "Stage/BetaTilt"),
         ("position", ["Stage/Position/x", "Stage/Position/y", "Stage/Position/z"]),
     ],
 }
 # we do not know whether the angle is radiant or degree, in all examples
 # the instance values are very small so can be both :( needs clarification
-# we also cannot document this into the NeXus file like @units = "Check this"
-# because then the dataconverter (rightly so complains) that the string "Check this"
+# we also cannot document this into the NeXus file like @units = "check this"
+# because then the dataconverter (rightly so complains) that the string "check this"
 # is not a proper unit for an instance of NX_VOLTAGE
 
 
 VELOX_DYNAMIC_TO_NX_EM = {
     "prefix": "/ENTRY[entry*]/measurement/event_data_em_set/EVENT_DATA_EM[event_data_em*]",
     "unix_to_iso8601": [
         ("start_time", "Acquisition/AcquisitionStartDatetime/DateTime")
```

### Comparing `pynxtools_em-0.1/pynxtools_em/examples/ebsd_database.py` & `pynxtools_em-0.1.1/pynxtools_em/examples/ebsd_database.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/geometry/convention_mapper.py` & `pynxtools_em-0.1.1/pynxtools_em/geometry/convention_mapper.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/geometry/euler_angle_convention.py` & `pynxtools_em-0.1.1/pynxtools_em/geometry/euler_angle_convention.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/geometry/geometry.py` & `pynxtools_em-0.1.1/pynxtools_em/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/geometry/handed_cartesian.py` & `pynxtools_em-0.1.1/pynxtools_em/geometry/handed_cartesian.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/geometry/msmse_convention.py` & `pynxtools_em-0.1.1/pynxtools_em/geometry/msmse_convention.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/reader.py` & `pynxtools_em-0.1.1/pynxtools_em/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,46 +15,44 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Parser for loading generic orientation microscopy data based on ."""
 
 from os import getcwd
 from time import perf_counter_ns
-from typing import Tuple, Any
-import numpy as np
+from typing import Any, Tuple
 
+import numpy as np
 from pynxtools.dataconverter.readers.base.reader import BaseReader
-from pynxtools_em.utils.io_case_logic import (
-    EmUseCaseSelector,
-)
 
-# from pynxtools_em.subparsers.nxs_mtex import NxEmNxsMTexSubParser
-from pynxtools_em.subparsers.nxs_pyxem import NxEmNxsPyxemSubParser
+from pynxtools_em.concepts.nxs_concepts import NxEmAppDef
 from pynxtools_em.subparsers.nxs_imgs import NxEmImagesSubParser
+from pynxtools_em.subparsers.nxs_nion import ZipNionProjectSubParser
 
-# from pynxtools_em.subparsers.nxs_nion import NxEmZippedNionProjectSubParser
+# from pynxtools_em.subparsers.nxs_mtex import NxEmNxsMTexSubParser
+from pynxtools_em.subparsers.nxs_pyxem import NxEmNxsPyxemSubParser
+from pynxtools_em.subparsers.oasis_config_reader import (
+    NxEmNomadOasisConfigurationParser,
+)
+from pynxtools_em.subparsers.oasis_eln_reader import NxEmNomadOasisElnSchemaParser
 from pynxtools_em.subparsers.rsciio_velox import RsciioVeloxSubParser
+from pynxtools_em.utils.io_case_logic import (
+    EmUseCaseSelector,
+)
+
 ## from pynxtools_em.utils.default_plots import NxEmDefaultPlotResolver
 # from pynxtools_em.geometry.convention_mapper import NxEmConventionMapper
-
 # remaining subparsers to be implemented and merged into this one
 # from pynxtools.dataconverter.readers.em_om.utils.orix_ebsd_parser \
 #     import NxEmOmOrixEbsdParser
 # from pynxtools.dataconverter.readers.em_om.utils.mtex_ebsd_parser \
 #     import NxEmOmMtexEbsdParser
 # from pynxtools.dataconverter.readers.em_om.utils.zip_ebsd_parser \
 #     import NxEmOmZipEbsdParser
-# from pynxtools.dataconverter.readers.em_om.utils.em_nexus_plots \
-#     import em_om_default_plot_generator
-
-from pynxtools_em.subparsers.oasis_config_reader import (
-    NxEmNomadOasisConfigurationParser,
-)
-from pynxtools_em.subparsers.oasis_eln_reader import NxEmNomadOasisElnSchemaParser
-from pynxtools_em.concepts.nxs_concepts import NxEmAppDef
+from pynxtools_em.utils.nx_default_plots import NxEmDefaultPlotResolver
 
 
 class EMReader(BaseReader):
     """Parse content from file formats of the electron microscopy community."""
 
     # pylint: disable=too-few-public-methods
 
@@ -119,38 +117,28 @@
             # nxs_mtex = NxEmNxsMTexSubParser(entry_id, case.dat[0], verbose=False)
             # nxs_mtex.parse(template)
             # TODO::check correct loop through!
 
             nxs_pyxem = NxEmNxsPyxemSubParser(entry_id, case.dat[0], verbose=False)
             nxs_pyxem.parse(template)
 
-            # nxs_nion = NxEmZippedNionProjectSubParser(entry_id, case.dat[0], verbose=False)
-            # nxs_nion.parse(template)
-            # TODO::check correct loop through!
+            nxs_nion = ZipNionProjectSubParser(entry_id, case.dat[0], verbose=False)
+            nxs_nion.parse(template)
 
             # for dat_instance in case.dat_parser_type:
             #     print(f"Process pieces of information in {dat_instance} tech partner file...")
             #    continue
             #    # elif case.dat_parser_type == "zip":
             #    #     zip_parser = NxEmOmZipEbsdParser(case.dat[0], entry_id)
             #    #     zip_parser.parse(template)
-        # em_default_plot_generator(template, 1)
 
-        # run_block = False
-        # if run_block is True:
-        #     nxs_plt = NxEmDefaultPlotResolver()
-        #     # if nxs_mtex is the sub-parser
-        #     resolved_path = nxs_plt.nxs_mtex_get_nxpath_to_default_plot(
-        #         entry_id, file_paths[0]
-        #     )
-        #     # print(f"DEFAULT PLOT IS {resolved_path}")
-        #     if resolved_path != "":
-        #         nxs_plt.annotate_default_plot(template, resolved_path)
+        nxplt = NxEmDefaultPlotResolver()
+        nxplt.priority_select(template)
 
-        debugging = True  # print(template)
+        debugging = False
         if debugging:
             print("Reporting state of template before passing to HDF5 writing...")
             for keyword in template.keys():
                 print(f"{keyword}: {template[keyword]}")
 
         print("Forward instantiated template to the NXS writer...")
         toc = perf_counter_ns()
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_apex.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_apex.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_base.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_base.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_bruker.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_bruker.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_concept.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_concept.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_dreamthreed.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_dreamthreed.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_ebsd.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_ebsd.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_edax.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_edax.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_emsoft.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_emsoft.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/hfive_oxford.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/hfive_oxford.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """(Sub-)parser mapping concepts and content from Oxford Instruments *.h5oina files on NXem."""
 
-import numpy as np
-import h5py
 from typing import Dict
+
+import h5py
+import numpy as np
 from diffpy.structure import Lattice, Structure
 
+from pynxtools_em.examples.ebsd_database import (
+    FLIGHT_PLAN,
+    REGULAR_TILING,
+    SQUARE_GRID,
+)
 from pynxtools_em.subparsers.hfive_base import HdfFiveBaseParser
 from pynxtools_em.utils.hfive_utils import (
-    read_strings_from_dataset,
     format_euler_parameterization,
+    read_strings_from_dataset,
 )
-from pynxtools_em.examples.ebsd_database import (
-    SQUARE_GRID,
-    REGULAR_TILING,
-    FLIGHT_PLAN,
-)  # HEXAGONAL_GRID
 
 
 class HdfFiveOxfordReader(HdfFiveBaseParser):
     """Overwrite constructor of hfive_base reader"""
 
     def __init__(self, file_path: str = ""):
         super().__init__(file_path)
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/image_base.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/image_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Parent class for all tech partner-specific image parsers for mapping on NXem."""
 
-import numpy as np
 from typing import Dict, List
 
+import numpy as np
+
 
 class ImgsBaseParser:
-    def __init__(self, file_path: str = ""):
+    def __init__(self, file_path: str = "", verbose=False):
         # self.supported_version = VERSION_MANAGEMENT
         # self.version = VERSION_MANAGEMENT
         # tech_partner the company which designed this format
         # schema_name the specific name of the family of schemas supported by this reader
         # schema_version the specific version(s) supported by this reader
         # writer_name the specific name of the tech_partner's (typically proprietary) software
         self.prfx = None
         self.tmp: Dict = {}
+        self.verbose = verbose
         if file_path is not None and file_path != "":
             self.file_path = file_path
         else:
             raise ValueError(f"{__name__} needs proper instantiation !")
 
     def init_named_cache(self, ckey: str):
         """Init a new cache for normalized image data if not existent."""
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/image_png_protochips.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/image_png_protochips.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,44 +13,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Subparser for exemplar reading of raw PNG files collected on a TEM with Protochip heating_chip."""
 
+import datetime
 import mmap
 import re
+from typing import Dict, List
+from zipfile import ZipFile
+
+import flatdict as fd
 import numpy as np
 import xmltodict
-import datetime
-import flatdict as fd
-from typing import Dict, List
 from PIL import Image
-from zipfile import ZipFile
 
+from pynxtools_em.concepts.concept_mapper import add_specific_metadata_deprecate
+from pynxtools_em.concepts.mapping_functors import variadic_path_to_specific_path
 from pynxtools_em.config.image_png_protochips_cfg import (
-    specific_to_variadic,
+    AXON_AUX_DYNAMIC_TO_NX_EM,
+    AXON_CHIP_DYNAMIC_TO_NX_EM,
     AXON_DETECTOR_STATIC_TO_NX_EM,
-    AXON_STAGE_STATIC_TO_NX_EM,
     AXON_STAGE_DYNAMIC_TO_NX_EM,
-    AXON_CHIP_DYNAMIC_TO_NX_EM,
-    AXON_AUX_DYNAMIC_TO_NX_EM,
+    AXON_STAGE_STATIC_TO_NX_EM,
     AXON_VARIOUS_DYNAMIC_TO_NX_EM,
-)
-from pynxtools_em.concepts.concept_mapper import (
-    variadic_path_to_specific_path,
-    add_specific_metadata,
+    specific_to_variadic,
 )
 from pynxtools_em.subparsers.image_base import ImgsBaseParser
-from pynxtools_em.utils.xml_utils import flatten_xml_to_dict
 from pynxtools_em.utils.get_file_checksum import (
-    get_sha256_of_file_content,
     DEFAULT_CHECKSUM_ALGORITHM,
+    get_sha256_of_file_content,
 )
 from pynxtools_em.utils.sorting import sort_ascendingly_by_second_argument_iso8601
+from pynxtools_em.utils.xml_utils import flatten_xml_to_dict
 
 
 class ProtochipsPngSetSubParser(ImgsBaseParser):
     def __init__(self, file_path: str = "", entry_id: int = 1, verbose: bool = False):
         super().__init__(file_path)
         self.entry_id = entry_id
         self.event_id = 1
@@ -266,74 +265,74 @@
         print(
             f"Time series end: {events_sorted[-1][1]}, {(events_sorted[-1][1] - time_series_start).total_seconds()} s"
         )
         return events_sorted
 
     def add_detector_static_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_DETECTOR_STATIC_TO_NX_EM,
             self.tmp["meta"][file_name],
             identifier,
             template,
         )
         return template
 
     def add_stage_static_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_STAGE_STATIC_TO_NX_EM,
             self.tmp["meta"][file_name],
             identifier,
             template,
         )
         return template
 
     def add_stage_dynamic_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_STAGE_DYNAMIC_TO_NX_EM,
             self.tmp["meta"][file_name],
             identifier,
             template,
         )
         return template
 
     def add_chip_dynamic_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_CHIP_DYNAMIC_TO_NX_EM,
             self.tmp["meta"][file_name],
             identifier,
             template,
         )
         return template
 
     def add_aux_dynamic_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_AUX_DYNAMIC_TO_NX_EM, self.tmp["meta"][file_name], identifier, template
         )
         return template
 
     def add_various_dynamic_metadata(self, file_name: str, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             AXON_VARIOUS_DYNAMIC_TO_NX_EM,
             self.tmp["meta"][file_name],
             identifier,
             template,
         )
         return template
 
     def process_event_data_em_metadata(self, template: dict) -> dict:
         """Add respective metadata."""
         # contextualization to understand how the image relates to the EM session
         print(
-            f"Mapping some of the Protochips-specific metadata on respective NeXus concept instance"
+            f"Mapping some of the Protochips metadata on respective NeXus concepts..."
         )
         # individual PNGs in self.file_path may include time/date information in the file name
         # surplus eventually AXON-specific identifier it seems useful though to sort these
         # PNGs based on time stamped information directly from the AXON metadata
         # here we sort ascendingly in time the events and associate new event ids
         self.event_sequence = self.sort_event_data_em()
         event_id = self.event_id
@@ -393,18 +392,18 @@
                             "compress": nparr,
                             "strength": 1,
                         }
                         #  0 is y while 1 is x for 2d, 0 is z, 1 is y, while 2 is x for 3d
                         template[f"{trg}/intensity/@long_name"] = f"Signal"
 
                         sxy = {"x": 1.0, "y": 1.0}
-                        scan_unit = {
-                            "x": "px",
-                            "y": "px",
-                        }  # TODO::get AXON image calibration
+                        scan_unit = {"x": "px", "y": "px"}
+                        # TODO::get AXON image calibration
+                        # "ImagerSettings.ImagePhysicalSize.X" / "ImagerSettings.ImagePixels.X"
+                        # "ImagerSettings.ImagePhysicalSize.Y" / "ImagerSettings.ImagePixels.Y"
                         nxy = {"x": np.shape(nparr)[1], "y": np.shape(nparr)[0]}
                         del nparr
                         # TODO::we assume here a very specific coordinate system
                         # see image_tiff_tfs.py parser for further details of the limitations
                         # of this approach
                         for dim in dims:
                             template[f"{trg}/AXISNAME[axis_{dim}]"] = {
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff_tfs.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff_tfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,39 +14,40 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Subparser for harmonizing ThermoFisher-specific content in TIFF files."""
 
 import mmap
-import numpy as np
-import flatdict as fd
 from typing import Dict
+
+import flatdict as fd
+import numpy as np
 from PIL import Image
 from PIL.TiffTags import TAGS
 
-from pynxtools_em.subparsers.image_tiff import TiffSubParser
-from pynxtools_em.subparsers.image_tiff_tfs_concepts import (
-    get_fei_parent_concepts,
-    get_fei_childs,
-)
+from pynxtools_em.concepts.concept_mapper import add_specific_metadata_deprecate
 from pynxtools_em.config.image_tiff_tfs_cfg import (
     TFS_APERTURE_STATIC_TO_NX_EM,
     TFS_DETECTOR_STATIC_TO_NX_EM,
-    TFS_VARIOUS_STATIC_TO_NX_EM,
     TFS_OPTICS_DYNAMIC_TO_NX_EM,
-    TFS_STAGE_DYNAMIC_TO_NX_EM,
     TFS_SCAN_DYNAMIC_TO_NX_EM,
+    TFS_STAGE_DYNAMIC_TO_NX_EM,
     TFS_VARIOUS_DYNAMIC_TO_NX_EM,
+    TFS_VARIOUS_STATIC_TO_NX_EM,
+)
+from pynxtools_em.subparsers.image_tiff import TiffSubParser
+from pynxtools_em.subparsers.image_tiff_tfs_concepts import (
+    get_fei_childs,
+    get_fei_parent_concepts,
 )
 from pynxtools_em.utils.image_utils import (
-    sort_ascendingly_by_second_argument,
     if_str_represents_float,
+    sort_ascendingly_by_second_argument,
 )
-from pynxtools_em.concepts.concept_mapper import add_specific_metadata
 
 
 class TfsTiffSubParser(TiffSubParser):
     def __init__(self, file_path: str = "", entry_id: int = 1):
         super().__init__(file_path)
         self.entry_id = entry_id
         self.event_id = 1
@@ -83,15 +84,15 @@
         else:
             print(
                 f"Parser {self.__class__.__name__} finds no content in {self.file_path} that it supports"
             )
 
     def get_metadata(self):
         """Extract metadata in TFS specific tags if present."""
-        print("Reporting the tags found in this TIFF file...")
+        print("Parsing TIFF tags...")
         # for an overview of tags
         # https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
         # with Image.open(self.file_path, mode="r") as fp:
         #     self.tags = {TAGS[key] : fp.tag[key] for key in fp.tag_v2}
         #     for key, val in self.tags.items():
         #         print(f"{key}, {val}")
         tfs_parent_concepts = get_fei_parent_concepts()
@@ -100,25 +101,27 @@
             tfs_parent_concepts_byte_offset[concept] = None
         with open(self.file_path, "rb", 0) as fp:
             s = mmap.mmap(fp.fileno(), 0, access=mmap.ACCESS_READ)
             for concept in tfs_parent_concepts:
                 pos = s.find(bytes(f"[{concept}]", "utf8"))  # != -1
                 if pos != -1:
                     tfs_parent_concepts_byte_offset[concept] = pos
-                else:
-                    print(f"Instance of concept [{concept}] was not found !")
-            print(tfs_parent_concepts_byte_offset)
+                # else:
+                #     print(f"Instance of concept [{concept}] was not found !")
+            if self.verbose:
+                print(tfs_parent_concepts_byte_offset)
 
             sequence = []  # decide I/O order in which metadata for childs of parent concepts will be read
             for key, value in tfs_parent_concepts_byte_offset.items():
                 if value is not None:
                     sequence.append((key, value))
                     # tuple of parent_concept name and byte offset
             sequence = sort_ascendingly_by_second_argument(sequence)
-            print(sequence)
+            if self.verbose:
+                print(sequence)
 
             idx = 0
             for parent, byte_offset in sequence:
                 pos_s = byte_offset
                 pos_e = None
                 if idx < len(sequence) - 1:
                     pos_e = sequence[idx + 1][1]
@@ -179,15 +182,17 @@
             self.process_event_data_em_metadata(template)
             self.process_event_data_em_data(template)
         return template
 
     def process_event_data_em_data(self, template: dict) -> dict:
         """Add respective heavy data."""
         # default display of the image(s) representing the data collected in this event
-        print(f"Writing TFS/FEI TIFF image as a onto the respective NeXus concept")
+        print(
+            f"Writing TFS/FEI TIFF image data to the respective NeXus concept instances..."
+        )
         # read image in-place
         with Image.open(self.file_path, mode="r") as fp:
             nparr = np.array(fp)
             # print(f"type: {type(nparr)}, dtype: {nparr.dtype}, shape: {np.shape(nparr)}")
             # TODO::discussion points
             # - how do you know we have an image of real space vs. imaginary space (from the metadata?)
             # - how do deal with the (ugly) scale bar that is typically stamped into the TIFF image content?
@@ -224,15 +229,16 @@
             if ("EScan/PixelWidth" in self.tmp["meta"].keys()) and (
                 "EScan/PixelHeight" in self.tmp["meta"].keys()
             ):
                 sxy = {
                     "x": self.tmp["meta"]["EScan/PixelWidth"],
                     "y": self.tmp["meta"]["EScan/PixelHeight"],
                 }
-                scan_unit = {"x": "px", "y": "px"}
+            else:
+                print("WARNING: Assuming pixel width and height unit is meter!")
             nxy = {"x": np.shape(np.array(fp))[1], "y": np.shape(np.array(fp))[0]}
             # TODO::be careful we assume here a very specific coordinate system
             # however the TIFF file gives no clue, TIFF just documents in which order
             # it arranges a bunch of pixels that have stream in into a n-d tiling
             # e.g. a 2D image
             # also we have to be careful because TFS just gives us here
             # typical case of an image without an information without its location
@@ -256,65 +262,65 @@
                     f"Coordinate along {dim}-axis ({scan_unit[dim]})"
                 )
                 template[f"{trg}/AXISNAME[axis_{dim}]/@units"] = f"{scan_unit[dim]}"
         return template
 
     def add_aperture_static_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_APERTURE_STATIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_detector_static_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_DETECTOR_STATIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_various_static_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_VARIOUS_STATIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_optics_dynamic_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_OPTICS_DYNAMIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_stage_dynamic_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_STAGE_DYNAMIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_scan_dynamic_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_SCAN_DYNAMIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def add_various_dynamic_metadata(self, template: dict) -> dict:
         identifier = [self.entry_id, self.event_id, 1]
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             TFS_VARIOUS_DYNAMIC_TO_NX_EM, self.tmp["meta"], identifier, template
         )
         return template
 
     def process_event_data_em_metadata(self, template: dict) -> dict:
         """Add respective metadata."""
         # contextualization to understand how the image relates to the EM session
-        print(f"Mapping some of the TFS/FEI metadata concepts onto NeXus concepts")
+        print(f"Mapping some of the TFS/FEI metadata on respective NeXus concepts...")
         self.add_aperture_static_metadata(template)
         self.add_detector_static_metadata(template)
         self.add_various_static_metadata(template)
         self.add_optics_dynamic_metadata(template)
         self.add_stage_dynamic_metadata(template)
         self.add_scan_dynamic_metadata(template)
         self.add_various_dynamic_metadata(template)
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/image_tiff_tfs_concepts.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/image_tiff_tfs_concepts.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/nxs_imgs.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_imgs.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/nxs_mtex.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_mtex.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/nxs_nion.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_nion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,49 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Parse Nion-specific content in a file containing a zip-compressed nionswift project."""
 
-# pylint: disable=no-member
-
-import mmap
-import yaml
 import json
+import mmap
+from typing import Dict, List
+from zipfile import ZipFile
+
 import flatdict as fd
-import numpy as np
 import h5py
 import nion.swift.model.NDataHandler as nsnd
-from zipfile import ZipFile
-from typing import Dict, List
-
-from pynxtools_em.utils.nion_utils import uuid_to_file_name
+import numpy as np
+import yaml
 
 # from pynxtools_em.utils.swift_generate_dimscale_axes \
 #     import get_list_of_dimension_scale_axes
 # from pynxtools_em.utils.swift_display_items_to_nx \
 #     import nexus_concept_dict, identify_nexus_concept_key
 # from pynxtools_em.concepts.concept_mapper \
 #    import apply_modifier, variadic_path_to_specific_path
 # from pynxtools_em.swift_to_nx_image_real_space \
 #    import NxImageRealSpaceDict
 from pynxtools_em.utils.get_file_checksum import (
-    get_sha256_of_file_content,
     DEFAULT_CHECKSUM_ALGORITHM,
+    get_sha256_of_file_content,
 )
+from pynxtools_em.utils.nion_utils import uuid_to_file_name
 
 
-class NxEmZippedNionProjectSubParser:
+class ZipNionProjectSubParser:
     """Parse zip-compressed archive of a nionswift project with its content."""
 
-    def __init__(self, entry_id: int = 1, input_file_path: str = ""):
+    def __init__(
+        self, entry_id: int = 1, input_file_path: str = "", verbose: bool = True
+    ):
         """Class wrapping swift parser."""
         if input_file_path is not None and input_file_path != "":
             self.file_path = input_file_path
-        else:
-            raise ValueError(f"{__name__} needs proper instantiation !")
         if entry_id > 0:
             self.entry_id = entry_id
         else:
             self.entry_id = 1
         # counters which keep track of how many instances of NXevent_data_em have
         # been instantiated, this implementation currently maps each display_items
         # onto an own NXevent_data_em instance
@@ -68,29 +66,37 @@
         # assure that there is exactly one *.nsproj file only to parse from
         self.ndata_file_dict: Dict = {}
         # just get the *.ndata files irrespective whether parsed later or not
         self.hfive_file_dict: Dict = {}
         # just get the *.h5 files irrespective whether parsed later or not
         self.configure()
         self.supported = False
+        self.verbose = verbose
+        self.check_if_zipped_nionswift_project_file()
 
     def configure(self):
         self.tmp["cfg"]: Dict = {}
         self.tmp["cfg"]["event_data_written"] = False
         self.tmp["cfg"]["event_data_em_id"] = 1
         self.tmp["cfg"]["image_id"] = 1
         self.tmp["cfg"]["spectrum_id"] = 1
         self.tmp["meta"]: Dict = {}
 
-    def check_if_zipped_nionswift_project_file(self, verbose=False):
+    def check_if_zipped_nionswift_project_file(self):
         """Inspect the content of the compressed project file to check if supported."""
+        if not self.file_path.endswith(".zip.nion"):
+            print(
+                f"Parser ZipNionProject finds no content in {self.file_path} that it supports"
+            )
+            return
+
         with open(self.file_path, "rb", 0) as fp:
             s = mmap.mmap(fp.fileno(), 0, access=mmap.ACCESS_READ)
             magic = s.read(8)
-            if verbose is True:
+            if self.verbose:
                 fp.seek(0, 2)
                 eof_byte_offset = fp.tell()
                 print(
                     f"Expecting zip-compressed file: ___{self.file_path}___{magic}___{get_sha256_of_file_content(fp)}___{eof_byte_offset}___"
                 )
             """
             if magic != b'PK\x03\x04':  # https://en.wikipedia.org/wiki/List_of_file_signatures
@@ -103,71 +109,70 @@
                 if (
                     file.endswith(".h5")
                     or file.endswith(".hdf")
                     or file.endswith(".hdf5")
                 ):
                     with zip_file_hdl.open(file) as fp:
                         magic = fp.read(8)
-                        if verbose is True:
+                        if self.verbose:
                             fp.seek(0, 2)
                             eof_byte_offset = fp.tell()
                             print(
                                 f"Expecting hfive: ___{file}___{magic}___{get_sha256_of_file_content(fp)}___{eof_byte_offset}___"
                             )
                         key = file[file.rfind("/") + 1 :].replace(".h5", "")
                         if key not in self.hfive_file_dict:
                             self.hfive_file_dict[key] = file
                 elif file.endswith(".ndata"):
                     with zip_file_hdl.open(file) as fp:
                         magic = fp.read(8)
-                        if verbose is True:
+                        if self.verbose:
                             fp.seek(0, 2)
                             eof_byte_offset = fp.tell()
                             print(
                                 f"Expecting ndata: ___{file}___{magic}___{get_sha256_of_file_content(fp)}___{eof_byte_offset}___"
                             )
                         key = file[file.rfind("/") + 1 :].replace(".ndata", "")
                         if key not in self.ndata_file_dict:
                             self.ndata_file_dict[key] = file
                 elif file.endswith(".nsproj"):
                     with zip_file_hdl.open(file) as fp:
                         magic = fp.read(8)
-                        if verbose is True:
+                        if self.verbose:
                             fp.seek(0, 2)
                             eof_byte_offset = fp.tell()
                             print(
                                 f"Expecting nsproj: ___{file}___{magic}___{get_sha256_of_file_content(fp)}___{eof_byte_offset}___"
                             )
                         key = file[file.rfind("/") + 1 :].replace(".nsproj", "")
                         if key not in self.proj_file_dict:
                             self.proj_file_dict[key] = file
                 else:
                     continue
         if not self.ndata_file_dict.keys().isdisjoint(self.hfive_file_dict.keys()):
             print(
                 "Test 2 failed, UUID keys of *.ndata and *.h5 files in project are not disjoint!"
             )
-            return False
+            return
         if len(self.proj_file_dict.keys()) != 1:
             print(
                 "Test 3 failed, he project contains either no or more than one nsproj file!"
             )
-            return False
+            return
         print(
             f"Content in zip-compressed nionswift project {self.file_path} passed all tests"
         )
         self.supported = True
-        if verbose is True:
+        if self.verbose:
             for key, val in self.proj_file_dict.items():
                 print(f"nsprj: ___{key}___{val}___")
             for key, val in self.ndata_file_dict.items():
                 print(f"ndata: ___{key}___{val}___")
             for key, val in self.hfive_file_dict.items():
                 print(f"hfive: ___{key}___{val}___")
-        return True
 
     def update_event_identifier(self):
         """Advance and reset bookkeeping of event data em and data instances."""
         if self.tmp["cfg"]["event_data_written"] is True:
             self.tmp["cfg"]["event_data_em_id"] += 1
             self.tmp["cfg"]["event_data_written"] = False
         self.tmp["cfg"]["image_id"] = 1
@@ -179,15 +184,15 @@
         return template
 
     def map_to_nexus(self, meta, arr, concept_name, template):
         """Create the actual instance of a specific set of NeXus concepts in template."""
         # TODO::
         return template
 
-    def process_ndata(self, file_hdl, full_path, template, verbose=False):
+    def process_ndata(self, file_hdl, full_path, template):
         """Handle reading and processing of opened *.ndata inside the ZIP file."""
         # assure that we start reading that file_hdl/pointer from the beginning...
         file_hdl.seek(0)
         local_files, dir_files, eocd = nsnd.parse_zip(file_hdl)
         flat_metadata_dict = {}
         """
         data_arr = None
@@ -211,15 +216,15 @@
                 """
                 nx_concept_key = identify_nexus_concept_key(metadata_dict)
                 nx_concept_name = nexus_concept_dict[nx_concept_key]
                 print(f"Display_item {full_path}, concept {nx_concept_key}, maps {nx_concept_name}")
                 """
 
                 flat_metadata_dict = fd.FlatDict(metadata_dict, delimiter="/")
-                if verbose is True:
+                if self.verbose:
                     print(f"Flattened content of this metadata.json")
                     for key, value in flat_metadata_dict.items():
                         print(f"ndata, metadata.json, flat: ___{key}___{value}___")
                 # no break here, because we would like to inspect all content
                 # expect (based on Benedikt's example) to find only one json file
                 # in that *.ndata file pointed to by file_hdl
         if flat_metadata_dict == {}:  # only continue if some metadata were retrieved
@@ -241,23 +246,24 @@
                 # because we expect (based on Benedikt's example) to find only one npy file
                 # in that *.ndata file pointed to by file_hdl
 
         # check on the integriety of the data_arr array that it is not None or empty
         # this should be done more elegantly by just writing the
         # data directly into the template and not creating another copy
         # TODO::only during inspection
-        return template
-
+        """
         self.map_to_nexus(flat_metadata_dict, data_arr, nx_concept_name, template)
         del flat_metadata_dict
         del data_arr
         del nx_concept_name
         return template
+        """
+        return template
 
-    def process_hfive(self, file_hdl, full_path, template: dict, verbose=False):
+    def process_hfive(self, file_hdl, full_path, template: dict):
         """Handle reading and processing of opened *.h5 inside the ZIP file."""
         flat_metadata_dict = {}
         """
         data_arr = None
         nx_concept_name = ""
         """
         file_hdl.seek(0)
@@ -271,15 +277,15 @@
             """
             nx_concept_key = identify_nexus_concept_key(metadata_dict)
             nx_concept_name = nexus_concept_dict[nx_concept_key]
             print(f"Display_item {full_path}, concept {nx_concept_key}, maps {nx_concept_name}")
             """
 
             flat_metadata_dict = fd.FlatDict(metadata_dict, delimiter="/")
-            if verbose is True:
+            if self.verbose:
                 print(f"Flattened content of this metadata.json")
                 for key, value in flat_metadata_dict.items():
                     print(f"hfive, data, flat: ___{key}___{value}___")
 
             if (
                 flat_metadata_dict == {}
             ):  # only continue if some metadata were retrieved
@@ -299,25 +305,25 @@
             self.map_to_nexus(flat_metadata_dict, data_arr, nx_concept_name, template)
             del flat_metadata_dict
             del data_arr
             del nx_concept_name
             """
         return template
 
-    def parse_project_file(self, template: dict, verbose=False) -> dict:
+    def parse_project_file(self, template: dict) -> dict:
         """Parse lazily from compressed NionSwift project (nsproj + directory)."""
         nionswift_proj_mdata = {}
         with ZipFile(self.file_path) as zip_file_hdl:
             for pkey, proj_file_name in self.proj_file_dict.items():
                 with zip_file_hdl.open(proj_file_name) as file_hdl:
                     nionswift_proj_mdata = fd.FlatDict(
                         yaml.safe_load(file_hdl), delimiter="/"
                     )
                     # TODO::inspection phase, maybe with yaml to file?
-                    if verbose is True:
+                    if self.verbose:
                         print(f"Flattened content of {proj_file_name}")
                         for (
                             key,
                             value,
                         ) in nionswift_proj_mdata.items():  # ["display_items"]:
                             print(f"nsprj, flat: ___{key}___{value}___")
         if nionswift_proj_mdata == {}:
@@ -342,38 +348,34 @@
                                 with zip_file_hdl.open(
                                     self.ndata_file_dict[key]
                                 ) as file_hdl:
                                     self.process_ndata(
                                         file_hdl,
                                         self.ndata_file_dict[key],
                                         template,
-                                        verbose,
                                     )
                         elif key in self.hfive_file_dict.keys():
                             print(
                                 f"Key {key} is *.h5 maps to {self.hfive_file_dict[key]}"
                             )
                             with ZipFile(self.file_path) as zip_file_hdl:
                                 print(f"Parsing {self.hfive_file_dict[key]}...")
                                 with zip_file_hdl.open(
                                     self.hfive_file_dict[key]
                                 ) as file_hdl:
                                     self.process_hfive(
                                         file_hdl,
                                         self.hfive_file_dict[key],
                                         template,
-                                        verbose,
                                     )
                         else:
                             print(f"Key {key} has no corresponding data file")
         return template
 
-    def parse(self, template: dict, verbose=False) -> dict:
+    def parse(self, template: dict) -> dict:
         """Parse NOMAD OASIS relevant data and metadata from swift project."""
-        print(
-            "Parsing in-place from zip-compressed nionswift project (nsproj + directory)..."
-        )
-        if self.check_if_zipped_nionswift_project_file(verbose) is False:
-            return template
-
-        self.parse_project_file(template, verbose)
+        if self.supported:
+            print(
+                "Parsing in-place from zip-compressed nionswift project (nsproj + directory)..."
+            )
+            self.parse_project_file(template)
         return template
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/nxs_pyxem.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/nxs_pyxem.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,51 +28,50 @@
 # with offering this parser we also would like to embrace and acknowledge the efforts
 # of other electron microscopists (like the pyxem team, hyperspy etc.) and their work
 # towards software tools which are complementary to the MTex texture toolbox
 # one could have also implemented the HDF5 parsing inside MTex but we leave this as a
 # task for the community and instead focus here on showing a more diverse example
 # towards more interoperability between the different tools in the community
 
+import mmap
 import os
-import numpy as np
 
-from PIL import Image as pil
-from orix import plot
 import matplotlib.pyplot as plt  # in the hope that this closes figures with orix plot
+import numpy as np
+from orix import plot
 from orix.quaternion import Rotation
 from orix.quaternion.symmetry import get_point_group
 from orix.vector import Vector3d
+from PIL import Image as pil
 
+from pynxtools_em.concepts.nxs_image_r_set import NxImageRealSpaceSet
+from pynxtools_em.subparsers.hfive_apex import HdfFiveEdaxApexReader
+from pynxtools_em.subparsers.hfive_bruker import HdfFiveBrukerEspritReader
+from pynxtools_em.subparsers.hfive_dreamthreed import HdfFiveDreamThreedReader
+from pynxtools_em.subparsers.hfive_ebsd import HdfFiveCommunityReader
+from pynxtools_em.subparsers.hfive_edax import HdfFiveEdaxOimAnalysisReader
+from pynxtools_em.subparsers.hfive_emsoft import HdfFiveEmSoftReader
+from pynxtools_em.subparsers.hfive_oxford import HdfFiveOxfordReader
+from pynxtools_em.utils.get_scan_points import (
+    get_scan_point_axis_values,
+    get_scan_point_coords,
+    hexagonal_grid,
+    square_grid,
+    threed,
+)
+from pynxtools_em.utils.get_sqr_grid import (
+    get_scan_points_with_mark_data_discretized_on_sqr_grid,
+)
 from pynxtools_em.utils.hfive_utils import read_strings_from_dataset
 from pynxtools_em.utils.hfive_web_constants import (
-    HFIVE_WEB_MAXIMUM_ROI,
     HFIVE_WEB_MAXIMUM_RGB,
+    HFIVE_WEB_MAXIMUM_ROI,
 )
 from pynxtools_em.utils.hfive_web_utils import hfive_web_decorate_nxdata
 from pynxtools_em.utils.image_processing import thumbnail
-from pynxtools_em.utils.get_sqr_grid import (
-    get_scan_points_with_mark_data_discretized_on_sqr_grid,
-)
-from pynxtools_em.utils.get_scan_points import (
-    square_grid,
-    hexagonal_grid,
-    threed,
-    get_scan_point_axis_values,
-    get_scan_point_coords,
-)
-
-from pynxtools_em.subparsers.hfive_oxford import HdfFiveOxfordReader
-from pynxtools_em.subparsers.hfive_bruker import HdfFiveBrukerEspritReader
-from pynxtools_em.subparsers.hfive_edax import HdfFiveEdaxOimAnalysisReader
-from pynxtools_em.subparsers.hfive_apex import HdfFiveEdaxApexReader
-from pynxtools_em.subparsers.hfive_ebsd import HdfFiveCommunityReader
-from pynxtools_em.subparsers.hfive_emsoft import HdfFiveEmSoftReader
-from pynxtools_em.subparsers.hfive_dreamthreed import HdfFiveDreamThreedReader
-from pynxtools_em.concepts.nxs_image_r_set import NxImageRealSpaceSet
-
 
 PROJECTION_VECTORS = [Vector3d.xvector(), Vector3d.yvector(), Vector3d.zvector()]
 PROJECTION_DIRECTIONS = [
     ("X", Vector3d.xvector().data.flatten()),
     ("Y", Vector3d.yvector().data.flatten()),
     ("Z", Vector3d.zvector().data.flatten()),
 ]
@@ -124,15 +123,17 @@
         }
         self.cache = {"is_filled": False}
         self.verbose = verbose
 
     def parse(self, template: dict) -> dict:
         hfive_parser_type = self.identify_hfive_type()
         if hfive_parser_type is None:
-            print(f"{self.file_path} does not match any of the supported HDF5 formats")
+            print(
+                f"Parser PyXem/NeXus/HDF5 finds that {self.file_path} does not match any of the supported HDF5 formats"
+            )
             return template
         print(
             f"Parsing via {self.__class__.__name__} content type {hfive_parser_type}..."
         )
 
         # ##MK::current implementation pulls all entries into the template
         # before writing them out, this might not fit into main memory
@@ -196,14 +197,19 @@
             self.process_into_template(dreamthreed.tmp, template)
         else:  # none or something unsupported
             return template
         return template
 
     def identify_hfive_type(self):
         """Identify if HDF5 file matches a known format for which a subparser exists."""
+        with open(self.file_path, "rb", 0) as file:
+            s = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
+            magic = s.read(4)
+            if magic != b"\x89HDF":
+                return None
         # tech partner formats used for measurement
         hdf = HdfFiveOxfordReader(self.file_path)
         if hdf.supported is True:
             return "oxford"
         hdf = HdfFiveEdaxOimAnalysisReader(self.file_path)
         if hdf.supported is True:
             return "edax"
@@ -439,16 +445,15 @@
         # for the purpose of showing users a readily consumable default plot
         # to judge for each possible dataset in the same way if the
         # dataset is worthwhile and potentially valuable for ones on research
         n_pts = inp["n_x"] * inp["n_y"]
         n_pts_indexed = np.sum(inp["phase_id"] != 0)
         print(f"n_pts {n_pts}, n_pts_indexed {n_pts_indexed}")
         template[f"{prfx}/number_of_scan_points"] = np.uint32(n_pts)
-        template[f"{prfx}/indexing_rate"] = np.float64(100.0 * n_pts_indexed / n_pts)
-        template[f"{prfx}/indexing_rate/@units"] = f"%"
+        template[f"{prfx}/indexing_rate"] = np.float64(n_pts_indexed / n_pts)
         grp_name = f"{prfx}/phaseID[phase{nxem_phase_id}]"
         template[f"{grp_name}/number_of_scan_points"] = np.uint32(
             np.sum(inp["phase_id"] == 0)
         )
         template[f"{grp_name}/phase_identifier"] = np.uint32(nxem_phase_id)
         template[f"{grp_name}/phase_name"] = f"notIndexed"
 
@@ -609,17 +614,16 @@
                             endpoint=True,
                         ),
                         np.uint32,
                     ),
                     "strength": 1,
                 }
                 template[f"{lgd}/AXISNAME[axis_{dim}]/@long_name"] = (
-                    f"Pixel along {dim[0]}-axis"
+                    f"Pixel coordinate along {dim[0]}-axis"
                 )
-                template[f"{lgd}/AXISNAME[axis_{dim}]/@units"] = "px"
         return template
 
     def onthefly_process_roi_ipfs_phases_threed(
         self, inp: dict, roi_id: int, template: dict
     ) -> dict:
         # this function is almost the same as its twod version we keep it for
         # now an own function until the rediscretization also works for the 3D grid
@@ -628,16 +632,15 @@
         # see comments in twod version of this function
         nxem_phase_id = 0
         prfx = f"/ENTRY[entry{self.entry_id}]/ROI[roi{roi_id}]/ebsd/indexing"
         n_pts = inp["n_x"] * inp["n_y"] * inp["n_z"]
         n_pts_indexed = np.sum(inp["phase_id"] != 0)
         print(f"n_pts {n_pts}, n_pts_indexed {n_pts_indexed}")
         template[f"{prfx}/number_of_scan_points"] = np.uint32(n_pts)
-        template[f"{prfx}/indexing_rate"] = np.float64(100.0 * n_pts_indexed / n_pts)
-        template[f"{prfx}/indexing_rate/@units"] = f"%"
+        template[f"{prfx}/indexing_rate"] = np.float64(n_pts_indexed / n_pts)
         grp_name = f"{prfx}/phaseID[phase{nxem_phase_id}]"
         template[f"{grp_name}/number_of_scan_points"] = np.uint32(
             np.sum(inp["phase_id"] == 0)
         )
         template[f"{grp_name}/phase_identifier"] = np.uint32(nxem_phase_id)
         template[f"{grp_name}/phase_name"] = f"notIndexed"
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/oasis_config_reader.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/oasis_config_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,38 +23,39 @@
 #       "use": list of pair of trg, src endpoint, take the value in src copy into trg
 #       "load": list of single value or pair (trg, src)
 #           if single value this means that the endpoint of trg and src is the same
 #           e.g. in the example below "name" means
 #           ("/ENTRY[entry*]/USER[user*]/name, "load", "name")
 #           if pair load the value pointed to by src and copy into trg
 
+import pathlib
+
 import flatdict as fd
 import yaml
 
-
-from pynxtools_em.config.oasis_cfg import EM_EXAMPLE_CSYS_TO_NEXUS
-from pynxtools_em.concepts.concept_mapper import variadic_path_to_specific_path
+from pynxtools_em.concepts.mapping_functors import add_specific_metadata
+from pynxtools_em.config.oasis_cfg import EM_CSYS_TO_NEXUS
 
 
 class NxEmNomadOasisConfigurationParser:
     """Parse deployment specific configuration."""
 
     def __init__(self, file_path: str, entry_id: int, verbose: bool = False):
         print(
-            f"Extracting data from deployment-specific configuration file: {file_path}"
+            f"Extracting data from deployment-specific configuration file {file_path} ..."
         )
         if (
-            file_path.rsplit("/", 1)[-1].endswith(".oasis.specific.yaml")
-            or file_path.endswith(".oasis.specific.yml")
+            pathlib.Path(file_path).name.endswith(".oasis.specific.yaml")
+            or pathlib.Path(file_path).name.endswith(".oasis.specific.yml")
         ) and entry_id > 0:
             self.entry_id = entry_id
             self.file_path = file_path
             with open(self.file_path, "r", encoding="utf-8") as stream:
                 self.yml = fd.FlatDict(yaml.safe_load(stream), delimiter="/")
-                if verbose is True:
+                if verbose:
                     for key, val in self.yml.items():
                         print(f"key: {key}, val: {val}")
         else:
             self.entry_id = 1
             self.file_path = ""
             self.yml = {}
 
@@ -66,31 +67,20 @@
                 if all(isinstance(entry, dict) for entry in self.yml[src]):
                     csys_id = 1
                     # custom schema delivers a list of dictionaries...
                     for csys_dict in self.yml[src]:
                         if csys_dict == {}:
                             continue
                         identifier = [self.entry_id, csys_id]
-                        variadic_prefix = EM_EXAMPLE_CSYS_TO_NEXUS["prefix"]
-                        for key in csys_dict:
-                            for entry in EM_EXAMPLE_CSYS_TO_NEXUS["load"]:
-                                if isinstance(entry, str):
-                                    if key == entry:
-                                        trg = variadic_path_to_specific_path(
-                                            f"{variadic_prefix}/{entry}", identifier
-                                        )
-                                        template[trg] = csys_dict[entry]
-                                        break
-                                if isinstance(entry, tuple) and len(entry) == 2:
-                                    if key == entry[1]:
-                                        trg = variadic_path_to_specific_path(
-                                            f"{variadic_prefix}/{entry[0]}", identifier
-                                        )
-                                        template[trg] = csys_dict[entry[1]]
-                                        break
+                        add_specific_metadata(
+                            EM_CSYS_TO_NEXUS,
+                            fd.FlatDict(csys_dict),
+                            identifier,
+                            template,
+                        )
                         csys_id += 1
         return template
 
     def report(self, template: dict) -> dict:
         """Copy data from configuration applying mapping functors."""
         self.parse_reference_frames(template)
         return template
```

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_base.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_base.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_bruker.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_bruker.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/subparsers/rsciio_velox.py` & `pynxtools_em-0.1.1/pynxtools_em/subparsers/rsciio_velox.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,47 +13,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """(Sub-)parser for reading content from ThermoFisher Velox *.emd (HDF5) via rosettasciio."""
 
+from datetime import datetime
+from typing import Dict, List
+
 import flatdict as fd
 import numpy as np
 import pytz
-from typing import Dict, List
-from datetime import datetime
-from rsciio import emd
 from ase.data import chemical_symbols
+from rsciio import emd
 
-from pynxtools_em.subparsers.rsciio_base import RsciioBaseParser
-from pynxtools_em.utils.rsciio_hspy_utils import (
-    get_named_axis,
-    get_axes_dims,
-    get_axes_units,
-)
-from pynxtools_em.utils.get_file_checksum import (
-    get_sha256_of_file_content,
-    DEFAULT_CHECKSUM_ALGORITHM,
-)
+from pynxtools_em.concepts.concept_mapper import add_specific_metadata_deprecate
+from pynxtools_em.concepts.mapping_functors import variadic_path_to_specific_path
 from pynxtools_em.config.rsciio_velox_cfg import (
-    VELOX_ENTRY_TO_NX_EM,
+    VELOX_DYNAMIC_TO_NX_EM,
+    VELOX_EBEAM_DYNAMIC_TO_NX_EM,
     VELOX_EBEAM_STATIC_TO_NX_EM,
+    VELOX_ENTRY_TO_NX_EM,
     VELOX_FABRICATION_TO_NX_EM,
-    VELOX_SCAN_TO_NX_EM,
     VELOX_OPTICS_TO_NX_EM,
+    VELOX_SCAN_TO_NX_EM,
     VELOX_STAGE_TO_NX_EM,
-    VELOX_DYNAMIC_TO_NX_EM,
-    VELOX_EBEAM_DYNAMIC_TO_NX_EM,
 )
-from pynxtools_em.utils.string_conversions import string_to_number
-from pynxtools_em.concepts.concept_mapper import (
-    variadic_path_to_specific_path,
-    add_specific_metadata,
+from pynxtools_em.subparsers.rsciio_base import RsciioBaseParser
+from pynxtools_em.utils.get_file_checksum import (
+    DEFAULT_CHECKSUM_ALGORITHM,
+    get_sha256_of_file_content,
 )
+from pynxtools_em.utils.rsciio_hspy_utils import (
+    get_axes_dims,
+    get_axes_units,
+    get_named_axis,
+)
+from pynxtools_em.utils.string_conversions import string_to_number
 
 REAL_SPACE = 0
 COMPLEX_SPACE = 1
 
 
 def all_req_keywords_in_dict(dct: dict, keywords: list) -> bool:
     """Check if dict dct has all keywords in keywords as keys from."""
@@ -262,62 +261,74 @@
 
         return "n/a"
 
     def add_entry_header(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map entry-specific metadata on NXem instance."""
-        add_specific_metadata(VELOX_ENTRY_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_ENTRY_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_ebeam_static(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map em_lab ebeam."""
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             VELOX_EBEAM_STATIC_TO_NX_EM, orgmeta, identifier, template
         )
         return template
 
     def add_fabrication(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map fabrication-specific metadata on NXem instance"""
-        add_specific_metadata(VELOX_FABRICATION_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_FABRICATION_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_scan(self, orgmeta: fd.FlatDict, identifier: list, template: dict) -> dict:
         """Map scan-specific metadata on NXem instance."""
-        add_specific_metadata(VELOX_SCAN_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_SCAN_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_optics(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map optics-specific metadata on NXem instance."""
-        add_specific_metadata(VELOX_OPTICS_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_OPTICS_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_stage(self, orgmeta: fd.FlatDict, identifier: list, template: dict) -> dict:
         """Map optics-specific metadata on NXem instance."""
-        add_specific_metadata(VELOX_STAGE_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_STAGE_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_various_dynamic(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map optics-specific metadata on NXem instance."""
-        add_specific_metadata(VELOX_DYNAMIC_TO_NX_EM, orgmeta, identifier, template)
+        add_specific_metadata_deprecate(
+            VELOX_DYNAMIC_TO_NX_EM, orgmeta, identifier, template
+        )
         return template
 
     def add_ebeam_dynamic(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
         """Map optics-specific metadata on NXem instance."""
-        add_specific_metadata(
+        add_specific_metadata_deprecate(
             VELOX_EBEAM_DYNAMIC_TO_NX_EM, orgmeta, identifier, template
         )
         return template
 
     def add_lens_event_data(
         self, orgmeta: fd.FlatDict, identifier: list, template: dict
     ) -> dict:
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/get_file_checksum.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/get_file_checksum.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/get_gitrepo_commit.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/get_gitrepo_commit.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/get_scan_points.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/get_scan_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Identify likely scan_point_positions for specific EBSD grid types."""
 
-# pylint: disable=no-member
-
 import numpy as np
 
 from pynxtools_em.examples.ebsd_database import (
+    FLIGHT_PLAN,
     HEXAGONAL_GRID,
-    SQUARE_GRID,
     REGULAR_TILING,
-    FLIGHT_PLAN,
+    SQUARE_GRID,
 )
 
 
 def get_scan_point_axis_values(inp: dict, dim_name: str):
     is_threed = False
     if "dimensionality" in inp.keys():
         if inp["dimensionality"] == 3:
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/get_sqr_grid.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/get_sqr_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Discretize point cloud in R^d (d=2, 3) with mark data to square/cube voxel grid."""
 
-# pylint: disable=no-member
-
 import numpy as np
 from scipy.spatial import KDTree
 
 from pynxtools_em.examples.ebsd_database import SQUARE_GRID
-from pynxtools_em.utils.get_scan_points import threed, square_grid, hexagonal_grid
+from pynxtools_em.utils.get_scan_points import hexagonal_grid, square_grid, threed
 
 
 def get_scan_points_with_mark_data_discretized_on_sqr_grid(
     src_grid: dict, max_edge_length: int
 ) -> dict:
-    """Inspect grid_type, dimensionality, point locations, and mark src_grida, map then."""
+    """Inspect grid_type, dimensionality, point locations, and mark src_grid, map then."""
     is_threed = threed(src_grid)
     req_keys = ["grid_type", "tiling", "flight_plan"]
     dims = ["x", "y"]
     if is_threed is True:
         dims.append("z")
     for dim in dims:
         req_keys.append(f"scan_point_{dim}")
@@ -109,25 +107,25 @@
                     * trg_sxy,
                     trg_nxy[0],
                 ),
             )
         )
         # TODO:: if scan_point_{dim} are calibrated this approach
         # here would shift the origin to 0, 0 implicitly which may not be desired
-        print(f"trg_xy {trg_xy}, shape {np.shape(trg_xy)}")
+        print(f"trg_xy np.shape {np.shape(trg_xy)}")
         tree = KDTree(
             np.column_stack((src_grid["scan_point_x"], src_grid["scan_point_y"]))
         )
         d, idx = tree.query(trg_xy, k=1)
         if np.sum(idx == tree.n) > 0:
             raise ValueError(f"kdtree query left some query points without a neighbor!")
         del d
         del tree
 
-        # rebuild src_grid container with only the relevant src_grida selected from src_grid
+        # rebuild src_grid container with only the relevant src_grid selected from src_grid
         for key in src_grid.keys():
             if key == "euler":
                 trg_grid[key] = np.empty((np.shape(trg_xy)[0], 3), np.float32)
                 trg_grid[key].fill(np.nan)
                 trg_grid[key] = src_grid["euler"][idx, :]
                 if np.isnan(trg_grid[key]).any() is True:
                     raise ValueError(
@@ -166,24 +164,24 @@
                 "scan_point_x",
                 "scan_point_y",
                 "scan_point_z",
             ]:
                 trg_grid[key] = src_grid[key]
             #     print(f"WARNING:: src_grid[{key}] is mapped as is on trg_grid[{key}] !")
             #     print(f"final np.shape(trg_grid[{key}]) {np.shape(trg_grid[key])}")
-            else:
-                print(
-                    f"WARNING:: src_grid[{key}] is not yet mapped on trg_grid[{key}] !"
-                )
+            # else:
+            #     print(
+            #         f"WARNING:: src_grid[{key}] is not yet mapped on trg_grid[{key}] !"
+            #     )
             trg_grid["n_x"] = trg_nxy[0]
             trg_grid["n_y"] = trg_nxy[1]
             trg_grid["s_x"] = trg_sxy
             trg_grid["s_y"] = trg_sxy
             trg_grid["scan_point_x"] = trg_xy[0]
             trg_grid["scan_point_y"] = trg_xy[1]
             # TODO::need to update scan_point_{dim}
         return trg_grid
     else:
         raise ValueError(
             f"The 3D discretization is currently not implemented because "
-            f"we do not know of any large enough dataset the test it !"
+            f"we do not know of any large enough dataset to test it !"
         )
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/get_xrayline_iupac_names.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/get_xrayline_iupac_names.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/hfive_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/hfive_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/hfive_web_constants.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/hfive_web_constants.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/hfive_web_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/hfive_web_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/image_processing.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/image_processing.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Resize images so that they display properly in H5Web."""
 
-# pylint: disable=no-member
-
 # f"https://stackoverflow.com/questions/4321290/"
 # f" how-do-i-make-pil-take-into-account-the-shortest-side-when-creating-a-thumbnail"
 
 import numpy as np
 from PIL import Image as pil
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/image_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/io_case_logic.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/io_case_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Utility class to analyze which vendor/community files are passed to apm reader."""
 
-# pylint: disable=no-member,duplicate-code,too-many-branches
-
-from typing import Tuple, Dict, List
+from typing import Dict, List, Tuple
 
 VALID_FILE_NAME_SUFFIX_CONFIG = [".yaml", ".yml"]
 VALID_FILE_NAME_SUFFIX_DATA = [
     ".emd",
     ".tiff",
     ".tif",
     ".zip.axon",
+    ".zip.nion",
     ".edaxh5",
     ".h5",
     ".hdf5",
     ".nxs",
     ".dream3d",
 ]
-# ".dm3", ".dm4", ".mtex", ".nion"]
+# ".dm3", ".dm4", ".mtex"]
 
 
 class EmUseCaseSelector:
     """Decision maker about what needs to be parsed given arbitrary input.
 
     Users might invoke this dataconverter with arbitrary input, no input, or
     too much input. The UseCaseSelector decide what to do in each case.
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/nion_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/nion_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Utility function for mapping nionswift identifier to suffix used for identifying files in project."""
 
-# pylint: disable=no-member
-
 import uuid
 
 # see https://github.com/nion-software/nionswift/blob/e95839c5602d009006ea88a648e5f78dc77c1ea4/
 # nion/swift/model/Profile.py line 146 and following
 
 
 def encode(uuid_: uuid.UUID, alphabet: str) -> str:
```

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/rsciio_hspy_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/rsciio_hspy_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/sorting.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/string_conversions.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/string_conversions.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/string_encoding.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/string_encoding.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em/utils/xml_utils.py` & `pynxtools_em-0.1.1/pynxtools_em/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/pynxtools_em.egg-info/PKG-INFO` & `pynxtools_em-0.1.1/pynxtools_em.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-em
-Version: 0.1
+Version: 0.1.1
 Summary: Make electron microscopy results interoperable via NeXus
 Author-email: Markus Kühbach <markus.kuehbach@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-em
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-em/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,14 +32,17 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: jupyterlab-h5web; extra == "dev"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/pylint.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-em/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/pynxtools-em)
 ![](https://img.shields.io/pypi/l/pynxtools-em)
@@ -83,15 +86,15 @@
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-em.git --branch main --recursive pynxtools_em
 cd pynxtools_em
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
```

### Comparing `pynxtools_em-0.1/pynxtools_em.egg-info/SOURCES.txt` & `pynxtools_em-0.1.1/pynxtools_em.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -35,38 +35,30 @@
 docs/reference/tiff.md
 docs/reference/vemd.md
 docs/stylesheets/extra.css
 docs/tutorial/nexusio.md
 docs/tutorial/oasis.md
 docs/tutorial/standalone.md
 docs/tutorial/media/upload-processing.gif
-examples/README_Ebsd.md
-examples/README_Nion.md
-examples/README_Spctrscpy.md
-examples/Write.NXem_ebsd.Example.1.ipynb
-examples/Write.NXem_nion.Example.1.ipynb
-examples/Write.NXem_spctrscpy.Example.1.ipynb
+examples/HowToUseTutorial.ipynb
+examples/README.md
 examples/eln_data.yaml
-examples/eln_data_em_nion.yaml
-examples/eln_data_em_om.yaml
-examples/eln_data_em_spctrscpy.yaml
 examples/em.oasis.specific.yaml
-examples/image_png_protochips_to_nexus.ods
-examples/image_tiff_tfs_to_nexus.ods
 pynxtools_em/README.md
 pynxtools_em/__init__.py
 pynxtools_em/reader.py
 pynxtools_em.egg-info/PKG-INFO
 pynxtools_em.egg-info/SOURCES.txt
 pynxtools_em.egg-info/dependency_links.txt
 pynxtools_em.egg-info/entry_points.txt
 pynxtools_em.egg-info/requires.txt
 pynxtools_em.egg-info/top_level.txt
 pynxtools_em/concepts/README.md
 pynxtools_em/concepts/concept_mapper.py
+pynxtools_em/concepts/mapping_functors.py
 pynxtools_em/concepts/nxs_concepts.py
 pynxtools_em/concepts/nxs_em_eds_indexing.py
 pynxtools_em/concepts/nxs_image_r_set.py
 pynxtools_em/concepts/nxs_object.py
 pynxtools_em/concepts/nxs_spectrum_set.py
 pynxtools_em/config/README.md
 pynxtools_em/config/eln_cfg.py
@@ -113,21 +105,23 @@
 pynxtools_em/utils/get_sqr_grid.py
 pynxtools_em/utils/get_xrayline_iupac_names.py
 pynxtools_em/utils/hfive_utils.py
 pynxtools_em/utils/hfive_web_constants.py
 pynxtools_em/utils/hfive_web_utils.py
 pynxtools_em/utils/image_processing.py
 pynxtools_em/utils/image_utils.py
+pynxtools_em/utils/interpret_boolean.py
 pynxtools_em/utils/io_case_logic.py
 pynxtools_em/utils/nion_utils.py
 pynxtools_em/utils/nx_default_plots.py
 pynxtools_em/utils/rsciio_hspy_utils.py
 pynxtools_em/utils/sorting.py
 pynxtools_em/utils/string_conversions.py
 pynxtools_em/utils/string_encoding.py
+pynxtools_em/utils/versioning.py
 pynxtools_em/utils/xml_utils.py
 tests/test_reader.py
 tests/data/README.Ebsd.md
 tests/data/README.Spctrscpy.md
 tests/data/README_Nion.md
 tests/data/config_file.json
 tests/data/nomad_oasis_eln_schemes/nxem.ebsd.schema.archive.yaml
```

### Comparing `pynxtools_em-0.1/pyproject.toml` & `pynxtools_em-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 ]
 dev = [
     "mypy",
     "ruff==0.3.4",
     "pytest",
     "types-pyyaml",
     "pip-tools",
+    "jupyter",
+    "jupyterlab",
+    "jupyterlab-h5web"
 ]
 
 [project.entry-points."pynxtools.reader"]
 em = "pynxtools_em.reader:EMReader"
 
 [tool.setuptools_scm]
 version_scheme = "no-guess-dev"
```

### Comparing `pynxtools_em-0.1/rsciio_velox.batch.sh` & `pynxtools_em-0.1.1/rsciio_velox.batch.sh`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/rsciio_velox.ipynb` & `pynxtools_em-0.1.1/rsciio_velox.ipynb`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.ebsd.schema.archive.yaml` & `pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.ebsd.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.nion.schema.archive.yaml` & `pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.nion.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/tests/data/nomad_oasis_eln_schemes/nxem.spctrscpy.schema.archive.yaml` & `pynxtools_em-0.1.1/tests/data/nomad_oasis_eln_schemes/nxem.spctrscpy.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_em-0.1/tests/test_reader.py` & `pynxtools_em-0.1.1/tests/test_reader.py`

 * *Files identical despite different names*

