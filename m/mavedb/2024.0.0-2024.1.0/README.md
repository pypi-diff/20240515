# Comparing `tmp/mavedb-2024.0.0.tar.gz` & `tmp/mavedb-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "mavedb-2024.1.0.tar", max compression
```

## Comparing `mavedb-2024.0.0.tar` & `mavedb-2024.1.0.tar`

### file list

```diff
@@ -1,232 +1,127 @@
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.flake8
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile.test
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile.worker
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic.ini
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mavedb-2024.0.0/docker-compose-local.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mavedb-2024.0.0/requirements.txt
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.github/workflows/run-tests-on-push.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/README
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/alembic_helpers.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/script.py.mako
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/README
--rw-r--r--   0        0        0   489011 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/migrate_target_organism_to_taxonomy.py
--rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/populate_taxonomy_table.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/194cfebabe32_rename_wild_type_sequence.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/22e2d92d602e_add_publication_identifier_metadata_.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/33e99d4b90cc_add_mapped_variants_table.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/44d5c568f64b_simplify_reference_genome_target_.py
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/5cad62af3705_rename_pubmed_identifiers_table_to_publication_identifiers.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/60103ad1cb5b_add_target_sequence_label.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/6fae83d65ee4_taxonomy.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/886e059ad1a8_score_set_processing_errors.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/90e7860964a2_add_target_accession.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/988ca84c701b_.py
--rw-r--r--   0        0        0    24200 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/9d566d915a2c_.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/b3767156e04a_merge_6fae83d65ee4_and_886e059ad1a8.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/c6154dd7d9b9_add_gene_name_column_to_target_.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/da9ba478647d_add_primary_publication.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/f11fd758436e_.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/fecb3e0d181d_make_urns_unique.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/README.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/bioutils/assemblies.pyi
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/assembly_helper.pyi
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/__init__.pyi
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/fasta_seqfetcher.pyi
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/json_data_provider.pyi
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/exceptions.pyi
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/parser.pyi
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/sequencevariant.pyi
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/validator.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/interface.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/seqfetcher.pyi
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/uta.pyi
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/idutils/README.md
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/idutils/__init__.pyi
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/README.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/__init__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/exceptions.pyi
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/position.pyi
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/variant.pyi
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mavedb-2024.0.0/settings/.env.dev
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mavedb-2024.0.0/settings/.env.template
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/__init__.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/deps.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/server_main.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/data_providers/services.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/db/base.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/db/session.py
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/authentication.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/authorization.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/exceptions.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/experiments.py
--rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/identifiers.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/permissions.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/rxiv.py
--rw-r--r--   0        0        0    20708 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/score_sets.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/slack.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/taxonomies.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/temp_urns.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/urns.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/constants.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/hgvs.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/utils.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/variant.py
--rw-r--r--   0        0        0    28991 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/dataframe.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/exceptions.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/identifier.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/keywords.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/publication.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/target.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/urn_re.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/utilities.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/variant.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/conversion.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/general.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/identifier.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/keywords.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/publication.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/target.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/__init__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/access_key.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/doi_identifier.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/ensembl_identifier.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/ensembl_offset.py
--rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment_publication_identifier.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment_set.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/genome_identifier.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/keyword.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/license.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/mapped_variant.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/publication_identifier.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/raw_read_identifier.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/refseq_identifier.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/refseq_offset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/role.py
--rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/score_set.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/score_set_publication_identifier.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_accession.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_gene.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_sequence.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/taxonomy.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/uniprot_identifier.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/uniprot_offset.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/user.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/variant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/enums/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/enums/processing_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_association.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_code.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_nonce.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_partial.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_revision.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/__init__.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/access_keys.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/api_information.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/doi_identifiers.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/experiment_sets.py
--rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/experiments.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/hgvs.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/licenses.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/mapped_variant.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/publication_identifiers.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/raw_read_identifiers.py
--rw-r--r--   0        0        0    33666 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/score_sets.py
--rw-r--r--   0        0        0    14702 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/statistics.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/target_gene_identifiers.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/target_genes.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/taxonomies.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/users.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/access_key.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/api_version.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/doi_identifier.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/experiment.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/experiment_set.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier_offset.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/license.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/mapped_variant.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/publication_identifier.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/raw_read_identifier.py
--rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/score_set.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/search.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_accession.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_gene.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_sequence.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/taxonomy.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/user.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/variant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/base/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/base/base.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/__init__.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/jobs.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/conftest.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/dump_rels.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/constants.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/util.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/data/refseq.NM_001637.3.fasta
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/data/refseq.NM_001637.3.fasta.fai
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/conftest.py
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/test_score_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/__init__.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/conftest.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts.csv
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_different_variants.csv
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_hgvs_nt_and_pro.csv
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_score.csv
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_hgvs_nt_not_match_pro.csv
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_hgvs_pro_has_same_values.csv
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_duplicate_columns.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_hgvs_nt_and_pro.csv
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_nt_prefix.csv
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_pro_prefix.csv
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_nan_column_name.csv
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_string.csv
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_without_hgvs_column.csv
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_without_score_column.csv
--rw-r--r--   0        0        0    18066 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_experiments.py
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_hgvs.py
--rw-r--r--   0        0        0    22111 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_score_set.py
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_statistics.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/counts.csv
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/counts_acc.csv
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/scores.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/scores_acc.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/__init__.py
--rw-r--r--   0        0        0    47206 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_dataframe.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_identifier.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_keywords.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_publication.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_target.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_urn_re.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_utilities.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_variant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_external_gene_identifiers.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_publication_identifier.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_target_gene.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_wild_type_sequence.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/__init__.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/conftest.py
--rw-r--r--   0        0        0    12486 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/test_jobs.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/counts.csv
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/counts_acc.csv
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/scores.csv
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/scores_acc.csv
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 mavedb-2024.0.0/LICENSE
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 mavedb-2024.0.0/README.md
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 mavedb-2024.0.0/pyproject.toml
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 mavedb-2024.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-12-16 18:49:13.425533 mavedb-2024.1.0/LICENSE
+-rw-r--r--   0        0        0     5299 2024-05-15 00:24:52.312848 mavedb-2024.1.0/README.md
+-rw-r--r--   0        0        0     3222 2024-05-15 00:24:52.314475 mavedb-2024.1.0/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-05-15 00:24:52.314775 mavedb-2024.1.0/src/mavedb/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-14 21:37:25.047893 mavedb-2024.1.0/src/mavedb/data_providers/services.py
+-rw-r--r--   0        0        0      426 2024-05-14 21:37:25.048042 mavedb-2024.1.0/src/mavedb/db/base.py
+-rw-r--r--   0        0        0      686 2023-12-16 18:49:13.427672 mavedb-2024.1.0/src/mavedb/db/session.py
+-rw-r--r--   0        0        0      770 2024-05-14 21:37:25.048200 mavedb-2024.1.0/src/mavedb/deps.py
+-rw-r--r--   0        0        0     7601 2024-05-15 00:24:52.314916 mavedb-2024.1.0/src/mavedb/lib/authentication.py
+-rw-r--r--   0        0        0     1948 2024-05-15 00:24:52.315337 mavedb-2024.1.0/src/mavedb/lib/authorization.py
+-rw-r--r--   0        0        0     5230 2024-04-29 17:39:21.853314 mavedb-2024.1.0/src/mavedb/lib/exceptions.py
+-rw-r--r--   0        0        0     3125 2024-05-14 21:37:25.048831 mavedb-2024.1.0/src/mavedb/lib/experiments.py
+-rw-r--r--   0        0        0    17221 2024-05-14 21:37:25.049028 mavedb-2024.1.0/src/mavedb/lib/identifiers.py
+-rw-r--r--   0        0        0     2975 2024-05-15 00:24:52.315465 mavedb-2024.1.0/src/mavedb/lib/logging.py
+-rw-r--r--   0        0        0      391 2023-12-16 18:49:13.428540 mavedb-2024.1.0/src/mavedb/lib/mave/constants.py
+-rw-r--r--   0        0        0     2718 2023-12-16 18:49:13.428718 mavedb-2024.1.0/src/mavedb/lib/mave/hgvs.py
+-rw-r--r--   0        0        0      929 2023-12-16 18:49:13.428782 mavedb-2024.1.0/src/mavedb/lib/mave/utils.py
+-rw-r--r--   0        0        0     2773 2023-12-16 18:49:13.428859 mavedb-2024.1.0/src/mavedb/lib/mave/variant.py
+-rw-r--r--   0        0        0     1057 2024-05-15 00:24:52.315622 mavedb-2024.1.0/src/mavedb/lib/orcid.py
+-rw-r--r--   0        0        0    11222 2024-05-15 00:24:52.315905 mavedb-2024.1.0/src/mavedb/lib/permissions.py
+-rw-r--r--   0        0        0    17811 2023-12-16 18:49:13.429002 mavedb-2024.1.0/src/mavedb/lib/rxiv.py
+-rw-r--r--   0        0        0    25022 2024-05-15 00:24:52.316386 mavedb-2024.1.0/src/mavedb/lib/score_sets.py
+-rw-r--r--   0        0        0      949 2024-05-15 00:24:52.316619 mavedb-2024.1.0/src/mavedb/lib/script_environment.py
+-rw-r--r--   0        0        0     1196 2024-05-14 21:37:25.050298 mavedb-2024.1.0/src/mavedb/lib/slack.py
+-rw-r--r--   0        0        0     2993 2024-05-14 21:37:25.050528 mavedb-2024.1.0/src/mavedb/lib/taxonomies.py
+-rw-r--r--   0        0        0      197 2023-12-16 18:49:13.429177 mavedb-2024.1.0/src/mavedb/lib/temp_urns.py
+-rw-r--r--   0        0        0     5631 2024-05-14 21:37:25.050678 mavedb-2024.1.0/src/mavedb/lib/urns.py
+-rw-r--r--   0        0        0     2068 2023-12-16 18:49:13.429369 mavedb-2024.1.0/src/mavedb/lib/validation/constants/conversion.py
+-rw-r--r--   0        0        0     1390 2024-05-14 21:37:25.050989 mavedb-2024.1.0/src/mavedb/lib/validation/constants/general.py
+-rw-r--r--   0        0        0       49 2023-12-16 18:49:13.429474 mavedb-2024.1.0/src/mavedb/lib/validation/constants/identifier.py
+-rw-r--r--   0        0        0       17 2023-12-16 18:49:13.429523 mavedb-2024.1.0/src/mavedb/lib/validation/constants/keywords.py
+-rw-r--r--   0        0        0       49 2023-12-16 18:49:13.429573 mavedb-2024.1.0/src/mavedb/lib/validation/constants/publication.py
+-rw-r--r--   0        0        0      122 2023-12-16 18:49:13.429624 mavedb-2024.1.0/src/mavedb/lib/validation/constants/target.py
+-rw-r--r--   0        0        0    28991 2024-05-14 21:37:25.051208 mavedb-2024.1.0/src/mavedb/lib/validation/dataframe.py
+-rw-r--r--   0        0        0      277 2024-05-14 21:37:25.051377 mavedb-2024.1.0/src/mavedb/lib/validation/exceptions.py
+-rw-r--r--   0        0        0     5371 2023-12-16 18:49:13.430171 mavedb-2024.1.0/src/mavedb/lib/validation/identifier.py
+-rw-r--r--   0        0        0     1248 2023-12-16 18:49:13.430231 mavedb-2024.1.0/src/mavedb/lib/validation/keywords.py
+-rw-r--r--   0        0        0     6662 2023-12-16 18:49:13.430294 mavedb-2024.1.0/src/mavedb/lib/validation/publication.py
+-rw-r--r--   0        0        0     2311 2023-12-16 18:49:13.430351 mavedb-2024.1.0/src/mavedb/lib/validation/target.py
+-rw-r--r--   0        0        0     1325 2023-12-16 18:49:13.430423 mavedb-2024.1.0/src/mavedb/lib/validation/urn_re.py
+-rw-r--r--   0        0        0    12033 2024-05-14 21:37:25.051783 mavedb-2024.1.0/src/mavedb/lib/validation/utilities.py
+-rw-r--r--   0        0        0     3796 2023-12-16 18:49:13.430588 mavedb-2024.1.0/src/mavedb/lib/validation/variant.py
+-rw-r--r--   0        0        0      484 2024-05-14 21:37:25.051914 mavedb-2024.1.0/src/mavedb/models/__init__.py
+-rw-r--r--   0        0        0     1530 2024-05-15 00:41:42.228431 mavedb-2024.1.0/src/mavedb/models/access_key.py
+-rw-r--r--   0        0        0      567 2024-05-15 00:41:42.228661 mavedb-2024.1.0/src/mavedb/models/doi_identifier.py
+-rw-r--r--   0        0        0      575 2024-05-15 00:41:42.228867 mavedb-2024.1.0/src/mavedb/models/ensembl_identifier.py
+-rw-r--r--   0        0        0      807 2024-05-15 00:41:42.229093 mavedb-2024.1.0/src/mavedb/models/ensembl_offset.py
+-rw-r--r--   0        0        0        0 2023-12-16 18:49:13.431054 mavedb-2024.1.0/src/mavedb/models/enums/__init__.py
+-rw-r--r--   0        0        0      154 2023-12-16 18:49:13.431109 mavedb-2024.1.0/src/mavedb/models/enums/processing_state.py
+-rw-r--r--   0        0        0       61 2024-05-15 00:24:52.316910 mavedb-2024.1.0/src/mavedb/models/enums/user_role.py
+-rw-r--r--   0        0        0     6510 2024-05-15 00:41:42.229346 mavedb-2024.1.0/src/mavedb/models/experiment.py
+-rw-r--r--   0        0        0      926 2024-05-15 00:41:42.229554 mavedb-2024.1.0/src/mavedb/models/experiment_publication_identifier.py
+-rw-r--r--   0        0        0     4053 2024-05-15 00:41:42.229791 mavedb-2024.1.0/src/mavedb/models/experiment_set.py
+-rw-r--r--   0        0        0      573 2024-05-15 00:41:42.229987 mavedb-2024.1.0/src/mavedb/models/genome_identifier.py
+-rw-r--r--   0        0        0      429 2024-05-15 00:41:42.230207 mavedb-2024.1.0/src/mavedb/models/keyword.py
+-rw-r--r--   0        0        0        0 2023-12-16 18:49:13.431559 mavedb-2024.1.0/src/mavedb/models/legacy/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-14 22:34:36.267911 mavedb-2024.1.0/src/mavedb/models/legacy/auth_association.py
+-rw-r--r--   0        0        0      411 2024-05-14 22:34:34.521926 mavedb-2024.1.0/src/mavedb/models/legacy/auth_code.py
+-rw-r--r--   0        0        0      348 2024-05-14 22:34:04.053494 mavedb-2024.1.0/src/mavedb/models/legacy/auth_nonce.py
+-rw-r--r--   0        0        0      465 2024-05-14 22:34:38.074666 mavedb-2024.1.0/src/mavedb/models/legacy/auth_partial.py
+-rw-r--r--   0        0        0      422 2024-05-14 21:37:25.052899 mavedb-2024.1.0/src/mavedb/models/legacy/django_reversion_revision.py
+-rw-r--r--   0        0        0      565 2023-12-16 18:49:13.432008 mavedb-2024.1.0/src/mavedb/models/legacy/django_reversion_version.py
+-rw-r--r--   0        0        0      664 2024-05-15 00:41:42.230398 mavedb-2024.1.0/src/mavedb/models/license.py
+-rw-r--r--   0        0        0      635 2024-05-15 00:41:42.230584 mavedb-2024.1.0/src/mavedb/models/mapped_variant.py
+-rw-r--r--   0        0        0     1074 2024-05-15 00:41:42.230776 mavedb-2024.1.0/src/mavedb/models/publication_identifier.py
+-rw-r--r--   0        0        0      571 2024-05-15 00:41:42.230963 mavedb-2024.1.0/src/mavedb/models/raw_read_identifier.py
+-rw-r--r--   0        0        0      624 2024-05-15 00:41:42.231148 mavedb-2024.1.0/src/mavedb/models/refseq_identifier.py
+-rw-r--r--   0        0        0      784 2024-05-15 00:41:42.231362 mavedb-2024.1.0/src/mavedb/models/refseq_offset.py
+-rw-r--r--   0        0        0      371 2024-05-15 00:24:52.317074 mavedb-2024.1.0/src/mavedb/models/role.py
+-rw-r--r--   0        0        0     7960 2024-05-15 01:16:39.559578 mavedb-2024.1.0/src/mavedb/models/score_set.py
+-rw-r--r--   0        0        0      964 2024-05-15 00:41:42.231953 mavedb-2024.1.0/src/mavedb/models/score_set_publication_identifier.py
+-rw-r--r--   0        0        0      585 2023-12-16 18:49:13.432794 mavedb-2024.1.0/src/mavedb/models/target_accession.py
+-rw-r--r--   0        0        0     2172 2024-05-15 00:41:42.232139 mavedb-2024.1.0/src/mavedb/models/target_gene.py
+-rw-r--r--   0        0        0     1077 2024-05-15 00:41:42.232342 mavedb-2024.1.0/src/mavedb/models/target_sequence.py
+-rw-r--r--   0        0        0     1055 2024-05-15 00:41:42.232557 mavedb-2024.1.0/src/mavedb/models/taxonomy.py
+-rw-r--r--   0        0        0      626 2024-05-15 00:41:42.232767 mavedb-2024.1.0/src/mavedb/models/uniprot_identifier.py
+-rw-r--r--   0        0        0      827 2024-05-15 00:41:42.233171 mavedb-2024.1.0/src/mavedb/models/uniprot_offset.py
+-rw-r--r--   0        0        0     2087 2024-05-15 00:24:52.317221 mavedb-2024.1.0/src/mavedb/models/user.py
+-rw-r--r--   0        0        0     1021 2024-05-15 00:41:42.233368 mavedb-2024.1.0/src/mavedb/models/variant.py
+-rw-r--r--   0        0        0        0 2023-12-16 18:49:13.433162 mavedb-2024.1.0/src/mavedb/routers/__init__.py
+-rw-r--r--   0        0        0     3942 2024-05-15 00:24:52.317406 mavedb-2024.1.0/src/mavedb/routers/access_keys.py
+-rw-r--r--   0        0        0      529 2024-04-29 13:19:41.133875 mavedb-2024.1.0/src/mavedb/routers/api_information.py
+-rw-r--r--   0        0        0     1139 2023-12-16 18:49:13.433340 mavedb-2024.1.0/src/mavedb/routers/doi_identifiers.py
+-rw-r--r--   0        0        0     1141 2023-12-16 18:49:13.433389 mavedb-2024.1.0/src/mavedb/routers/experiment_sets.py
+-rw-r--r--   0        0        0    11972 2024-05-15 00:24:52.317691 mavedb-2024.1.0/src/mavedb/routers/experiments.py
+-rw-r--r--   0        0        0     4267 2024-05-14 21:37:25.055764 mavedb-2024.1.0/src/mavedb/routers/hgvs.py
+-rw-r--r--   0        0        0     1067 2023-12-16 18:49:13.433677 mavedb-2024.1.0/src/mavedb/routers/licenses.py
+-rw-r--r--   0        0        0     1688 2024-04-29 13:20:10.903700 mavedb-2024.1.0/src/mavedb/routers/mapped_variant.py
+-rw-r--r--   0        0        0     2102 2024-05-15 16:22:43.967172 mavedb-2024.1.0/src/mavedb/routers/orcid.py
+-rw-r--r--   0        0        0     6447 2024-05-15 00:24:52.318011 mavedb-2024.1.0/src/mavedb/routers/publication_identifiers.py
+-rw-r--r--   0        0        0     1194 2023-12-16 18:49:13.433867 mavedb-2024.1.0/src/mavedb/routers/raw_read_identifiers.py
+-rw-r--r--   0        0        0    31160 2024-05-15 00:24:52.318195 mavedb-2024.1.0/src/mavedb/routers/score_sets.py
+-rw-r--r--   0        0        0    14702 2024-05-14 21:37:25.056809 mavedb-2024.1.0/src/mavedb/routers/statistics.py
+-rw-r--r--   0        0        0     1362 2024-05-14 21:37:25.056980 mavedb-2024.1.0/src/mavedb/routers/target_gene_identifiers.py
+-rw-r--r--   0        0        0     2619 2024-05-14 21:37:25.057139 mavedb-2024.1.0/src/mavedb/routers/target_genes.py
+-rw-r--r--   0        0        0     3700 2024-05-14 21:37:25.057227 mavedb-2024.1.0/src/mavedb/routers/taxonomies.py
+-rw-r--r--   0        0        0     3812 2024-05-15 00:24:52.318946 mavedb-2024.1.0/src/mavedb/routers/users.py
+-rw-r--r--   0        0        0     6614 2024-05-15 00:24:52.319210 mavedb-2024.1.0/src/mavedb/scripts/export_public_data.py
+-rw-r--r--   0        0        0     7048 2024-05-15 00:24:52.319512 mavedb-2024.1.0/src/mavedb/scripts/resources/CC0_license.txt
+-rw-r--r--   0        0        0     5655 2024-05-15 00:24:52.319954 mavedb-2024.1.0/src/mavedb/server_main.py
+-rw-r--r--   0        0        0     1207 2024-05-14 21:37:25.058287 mavedb-2024.1.0/src/mavedb/view_models/__init__.py
+-rw-r--r--   0        0        0      662 2024-05-15 00:24:52.320226 mavedb-2024.1.0/src/mavedb/view_models/access_key.py
+-rw-r--r--   0        0        0      113 2023-12-16 18:49:13.434665 mavedb-2024.1.0/src/mavedb/view_models/api_version.py
+-rw-r--r--   0        0        0        0 2023-12-16 18:49:13.434724 mavedb-2024.1.0/src/mavedb/view_models/base/__init__.py
+-rw-r--r--   0        0        0      594 2023-12-16 18:49:13.434792 mavedb-2024.1.0/src/mavedb/view_models/base/base.py
+-rw-r--r--   0        0        0      697 2023-12-16 18:49:13.434853 mavedb-2024.1.0/src/mavedb/view_models/doi_identifier.py
+-rw-r--r--   0        0        0     4712 2024-05-15 00:24:52.320904 mavedb-2024.1.0/src/mavedb/view_models/experiment.py
+-rw-r--r--   0        0        0     1477 2024-05-15 00:24:52.321342 mavedb-2024.1.0/src/mavedb/view_models/experiment_set.py
+-rw-r--r--   0        0        0     1190 2023-12-16 18:49:13.435044 mavedb-2024.1.0/src/mavedb/view_models/external_gene_identifier.py
+-rw-r--r--   0        0        0      981 2023-12-16 18:49:13.435105 mavedb-2024.1.0/src/mavedb/view_models/external_gene_identifier_offset.py
+-rw-r--r--   0        0        0      839 2023-12-16 18:49:13.435164 mavedb-2024.1.0/src/mavedb/view_models/license.py
+-rw-r--r--   0        0        0      509 2024-04-29 13:22:13.948950 mavedb-2024.1.0/src/mavedb/view_models/mapped_variant.py
+-rw-r--r--   0        0        0      252 2024-05-15 00:24:52.321479 mavedb-2024.1.0/src/mavedb/view_models/orcid.py
+-rw-r--r--   0        0        0     1440 2023-12-16 18:49:13.435283 mavedb-2024.1.0/src/mavedb/view_models/publication_identifier.py
+-rw-r--r--   0        0        0      448 2023-12-16 18:49:13.435344 mavedb-2024.1.0/src/mavedb/view_models/raw_read_identifier.py
+-rw-r--r--   0        0        0    10990 2024-05-15 01:16:39.559828 mavedb-2024.1.0/src/mavedb/view_models/score_set.py
+-rw-r--r--   0        0        0      788 2023-12-16 18:49:13.435558 mavedb-2024.1.0/src/mavedb/view_models/search.py
+-rw-r--r--   0        0        0     1138 2024-05-14 21:37:25.059698 mavedb-2024.1.0/src/mavedb/view_models/target_accession.py
+-rw-r--r--   0        0        0     5249 2024-05-14 21:37:25.059836 mavedb-2024.1.0/src/mavedb/view_models/target_gene.py
+-rw-r--r--   0        0        0     2782 2024-05-15 16:22:55.676052 mavedb-2024.1.0/src/mavedb/view_models/target_sequence.py
+-rw-r--r--   0        0        0      800 2024-05-14 21:37:25.060201 mavedb-2024.1.0/src/mavedb/view_models/taxonomy.py
+-rw-r--r--   0        0        0     1918 2024-05-15 00:24:52.322258 mavedb-2024.1.0/src/mavedb/view_models/user.py
+-rw-r--r--   0        0        0      724 2023-12-16 18:49:13.435836 mavedb-2024.1.0/src/mavedb/view_models/variant.py
+-rw-r--r--   0        0        0      546 2024-05-14 21:37:25.060808 mavedb-2024.1.0/src/mavedb/worker/__init__.py
+-rw-r--r--   0        0        0     3746 2024-05-14 21:37:25.061003 mavedb-2024.1.0/src/mavedb/worker/jobs.py
+-rw-r--r--   0        0        0     1157 2024-05-14 21:37:25.061083 mavedb-2024.1.0/src/mavedb/worker/settings.py
+-rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 mavedb-2024.1.0/PKG-INFO
```

### Comparing `mavedb-2024.0.0/src/mavedb/deps.py` & `mavedb-2024.1.0/src/mavedb/deps.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/server_main.py` & `mavedb-2024.1.0/src/mavedb/server_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     api_information,
     doi_identifiers,
     experiment_sets,
     experiments,
     hgvs,
     licenses,
     mapped_variant,
+    orcid,
     publication_identifiers,
     target_gene_identifiers,
     taxonomies,
     raw_read_identifiers,
     score_sets,
     statistics,
     target_genes,
@@ -59,14 +60,15 @@
 app.include_router(api_information.router)
 app.include_router(doi_identifiers.router)
 app.include_router(experiment_sets.router)
 app.include_router(experiments.router)
 app.include_router(hgvs.router)
 app.include_router(licenses.router)
 app.include_router(mapped_variant.router)
+app.include_router(orcid.router)
 app.include_router(publication_identifiers.router)
 app.include_router(raw_read_identifiers.router)
 app.include_router(score_sets.router)
 app.include_router(statistics.router)
 app.include_router(target_gene_identifiers.router)
 app.include_router(target_genes.router)
 app.include_router(taxonomies.router)
```

### Comparing `mavedb-2024.0.0/src/mavedb/db/session.py` & `mavedb-2024.1.0/src/mavedb/db/session.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/exceptions.py` & `mavedb-2024.1.0/src/mavedb/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/experiments.py` & `mavedb-2024.1.0/src/mavedb/lib/experiments.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/identifiers.py` & `mavedb-2024.1.0/src/mavedb/lib/identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/rxiv.py` & `mavedb-2024.1.0/src/mavedb/lib/rxiv.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/score_sets.py` & `mavedb-2024.1.0/src/mavedb/lib/score_sets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from typing import BinaryIO, Optional
-
+import csv
+import io
+import re
+from typing import Any, BinaryIO, Iterable, Optional, Sequence
+ 
 import numpy as np
 import pandas as pd
 from pandas.testing import assert_index_equal
-from sqlalchemy import func, or_
+from sqlalchemy import cast, func, Integer, or_, select
 from sqlalchemy.orm import aliased, contains_eager, joinedload, selectinload, Session
 
 from mavedb.lib.exceptions import ValidationError
 from mavedb.lib.mave.constants import (
     HGVS_NT_COLUMN,
     HGVS_PRO_COLUMN,
     HGVS_SPLICE_COLUMN,
@@ -268,14 +271,139 @@
         .filter(*urn_filters)
         .group_by(ScoreSet.id)
         .having(func.count(func.distinct(analyzed_experiment_set.id)) == len(urns))
         .all()
     )
 
 
+def get_score_set_counts_as_csv(
+    db: Session, score_set: ScoreSet, start: Optional[int] = None, limit: Optional[int] = None
+) -> str:
+    assert type(score_set.dataset_columns) is dict
+    count_columns = [str(x) for x in list(score_set.dataset_columns.get("count_columns", []))]
+    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + count_columns
+    type_column = "count_data"
+
+    variants_query = (
+        select(Variant)
+        .where(Variant.score_set_id == score_set.id)
+        .order_by(cast(func.split_part(Variant.urn, "#", 2), Integer))
+    )
+    if start:
+        variants_query = variants_query.offset(start)
+    if limit:
+        variants_query = variants_query.limit(limit)
+    variants = db.scalars(variants_query).all()
+
+    rows_data = variants_to_csv_rows(variants, columns=columns, dtype=type_column)
+    stream = io.StringIO()
+    writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
+    writer.writeheader()
+    writer.writerows(rows_data)
+    return stream.getvalue()
+
+
+def get_score_set_scores_as_csv(
+    db: Session, score_set: ScoreSet, start: Optional[int] = None, limit: Optional[int] = None
+) -> str:
+    assert type(score_set.dataset_columns) is dict
+    score_columns = [str(x) for x in list(score_set.dataset_columns.get("score_columns", []))]
+    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + score_columns
+    type_column = "score_data"
+
+    variants_query = (
+        select(Variant)
+        .where(Variant.score_set_id == score_set.id)
+        .order_by(cast(func.split_part(Variant.urn, "#", 2), Integer))
+    )
+    if start:
+        variants_query = variants_query.offset(start)
+    if limit:
+        variants_query = variants_query.limit(limit)
+    variants = db.scalars(variants_query).all()
+
+    rows_data = variants_to_csv_rows(variants, columns=columns, dtype=type_column)
+    stream = io.StringIO()
+    writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
+    writer.writeheader()
+    writer.writerows(rows_data)
+    return stream.getvalue()
+
+
+null_values_re = re.compile(r"\s+|none|nan|na|undefined|n/a|null|nil", flags=re.IGNORECASE)
+
+
+def is_null(value):
+    """Return True if a string represents a null value."""
+    value = str(value).strip().lower()
+    return null_values_re.fullmatch(value) or not value
+
+
+def variant_to_csv_row(variant: Variant, columns: list[str], dtype: str, na_rep="NA") -> dict[str, Any]:
+    """
+    Format a variant into a containing the keys specified in `columns`.
+
+    Parameters
+    ----------
+    variant : variant.models.Variant
+        List of variants.
+    columns : list[str]
+        Columns to serialize.
+    dtype : str, {'scores', 'counts'}
+        The type of data requested. Either the 'score_data' or 'count_data'.
+    na_rep : str
+        String to represent null values.
+
+    Returns
+    -------
+    dict[str, Any]
+    """
+    row = {}
+    for column_key in columns:
+        if column_key == "hgvs_nt":
+            value = str(variant.hgvs_nt)
+        elif column_key == "hgvs_pro":
+            value = str(variant.hgvs_pro)
+        elif column_key == "hgvs_splice":
+            value = str(variant.hgvs_splice)
+        elif column_key == "accession":
+            value = str(variant.urn)
+        else:
+            parent = variant.data.get(dtype) if variant.data else None
+            value = str(parent.get(column_key)) if parent else na_rep
+        if is_null(value):
+            value = na_rep
+        row[column_key] = value
+    return row
+
+
+def variants_to_csv_rows(
+    variants: Sequence[Variant], columns: list[str], dtype: str, na_rep="NA"
+) -> Iterable[dict[str, Any]]:
+    """
+    Format each variant into a dictionary row containing the keys specified in `columns`.
+
+    Parameters
+    ----------
+    variants : list[variant.models.Variant]
+        List of variants.
+    columns : list[str]
+        Columns to serialize.
+    dtype : str, {'scores', 'counts'}
+        The type of data requested. Either the 'score_data' or 'count_data'.
+    na_rep : str
+        String to represent null values.
+
+    Returns
+    -------
+    list[dict[str, Any]]
+    """
+    return map(lambda v: variant_to_csv_row(v, columns, dtype, na_rep), variants)
+
+
 def find_meta_analyses_for_score_sets(db: Session, urns: list[str]) -> list[ScoreSet]:
     """
     Find all score sets that are meta-analyses for a specified collection of other score sets.
 
     :param db: An active database session.
     :param urns: A list of score set URNS.
     :return: A score set that is a meta-analysis for exactly the collection of score sets specified by urns; or None if
```

### Comparing `mavedb-2024.0.0/src/mavedb/lib/slack.py` & `mavedb-2024.1.0/src/mavedb/lib/slack.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/taxonomies.py` & `mavedb-2024.1.0/src/mavedb/lib/taxonomies.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/urns.py` & `mavedb-2024.1.0/src/mavedb/lib/urns.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/mave/hgvs.py` & `mavedb-2024.1.0/src/mavedb/lib/mave/hgvs.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/mave/utils.py` & `mavedb-2024.1.0/src/mavedb/lib/mave/utils.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/mave/variant.py` & `mavedb-2024.1.0/src/mavedb/lib/mave/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/dataframe.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/dataframe.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/identifier.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/keywords.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/keywords.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/publication.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/publication.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/target.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/target.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/urn_re.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/urn_re.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/utilities.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/utilities.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/variant.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/constants/conversion.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/constants/conversion.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/lib/validation/constants/general.py` & `mavedb-2024.1.0/src/mavedb/lib/validation/constants/general.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/models/doi_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/doi_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 from mavedb.db.base import Base
 
 
 class DoiIdentifier(Base):
     __tablename__ = "doi_identifiers"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False)
     db_name = Column(String, nullable=False)
     db_version = Column(String, nullable=True)
     url = Column(String, nullable=True)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/ensembl_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/refseq_identifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import date
 
 from sqlalchemy import Column, Date, Integer, String
 
 from mavedb.db.base import Base
 
 
-class EnsemblIdentifier(Base):
-    __tablename__ = "ensembl_identifiers"
+class RefseqIdentifier(Base):
+    __tablename__ = "refseq_identifiers"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False)
     db_name = Column(String, nullable=False)
     db_version = Column(String, nullable=True)
     url = Column(String, nullable=True)
+    reference_html = Column(String, nullable=True)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/ensembl_offset.py` & `mavedb-2024.1.0/src/mavedb/models/ensembl_offset.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,12 +6,14 @@
 from mavedb.models.target_gene import TargetGene
 
 
 class EnsemblOffset(Base):
     __tablename__ = "ensembl_offsets"
 
     identifier_id = Column(Integer, ForeignKey("ensembl_identifiers.id"), nullable=False, primary_key=True)
-    identifier : Mapped[EnsemblIdentifier] = relationship("EnsemblIdentifier", backref=backref("target_gene_offsets", uselist=True))
+    identifier: Mapped[EnsemblIdentifier] = relationship(
+        "EnsemblIdentifier", backref=backref("target_gene_offsets", uselist=True)
+    )
     target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
-    target_gene : Mapped[TargetGene] = relationship(back_populates="ensembl_offset")
-   
+    target_gene: Mapped[TargetGene] = relationship(back_populates="ensembl_offset")
+
     offset = Column(Integer, nullable=False)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/experiment.py` & `mavedb-2024.1.0/src/mavedb/models/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Column("sra_identifier_id", ForeignKey("sra_identifiers.id"), primary_key=True),
 )
 
 
 class Experiment(Base):
     __tablename__ = "experiments"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
     urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
     title = Column(String, nullable=False)
     short_description = Column(String, nullable=False)
     abstract_text = Column(String, nullable=False)
     method_text = Column(String, nullable=False)
     extra_metadata = Column(JSONB, nullable=False)
@@ -64,20 +64,20 @@
     published_date = Column(Date, nullable=True)
     processing_state = Column(String, nullable=True)
 
     # TODO Remove this obsolete column.
     num_score_sets = Column("num_scoresets", Integer, nullable=False, default=0)
     score_sets: Mapped[List["ScoreSet"]] = relationship(back_populates="experiment", cascade="all, delete-orphan")
 
-    experiment_set_id = Column(Integer, ForeignKey("experiment_sets.id"), nullable=True)
+    experiment_set_id = Column(Integer, ForeignKey("experiment_sets.id"), index=True, nullable=True)
     experiment_set: Mapped[Optional[ExperimentSet]] = relationship(back_populates="experiments")
 
-    created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    created_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     created_by: Mapped[User] = relationship("User", foreign_keys="Experiment.created_by_id")
-    modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    modified_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     modified_by: Mapped[User] = relationship("User", foreign_keys="Experiment.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
     keyword_objs: Mapped[list[Keyword]] = relationship(
         "Keyword", secondary=experiments_keywords_association_table, backref="experiments"
     )
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/experiment_publication_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/experiment_publication_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from sqlalchemy import Column, Integer, Boolean, ForeignKey
 from sqlalchemy.orm import relationship, Mapped
 
 from mavedb.db.base import Base
 
 # Prevent circular imports
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from mavedb.models.experiment import Experiment
     from mavedb.models.publication_identifier import PublicationIdentifier
 
 
 class ExperimentPublicationIdentifierAssociation(Base):
     __tablename__ = "experiment_publication_identifiers"
 
     experiment_id = Column(Integer, ForeignKey("experiments.id"), primary_key=True)
     publication_identifier_id = Column(Integer, ForeignKey("publication_identifiers.id"), primary_key=True)
     primary = Column(Boolean, nullable=True, default=False)
 
-    experiment : Mapped["Experiment"] = relationship("Experiment", back_populates="publication_identifier_associations")
-    publication : Mapped["PublicationIdentifier"] = relationship("PublicationIdentifier")
+    experiment: Mapped["Experiment"] = relationship("Experiment", back_populates="publication_identifier_associations")
+    publication: Mapped["PublicationIdentifier"] = relationship("PublicationIdentifier")
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/experiment_set.py` & `mavedb-2024.1.0/src/mavedb/models/experiment_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Column("sra_identifier_id", ForeignKey("sra_identifiers.id"), primary_key=True),
 )
 
 
 class ExperimentSet(Base):
     __tablename__ = "experiment_sets"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
     urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
     extra_metadata = Column(JSONB, nullable=False)
 
     private = Column(Boolean, nullable=False, default=True)
     approved = Column(Boolean, nullable=False, default=False)
     published_date = Column(Date, nullable=True)
@@ -62,17 +62,17 @@
 
     # TODO Refactor the way we handle child collections?
     num_experiments = Column(Integer, nullable=False, default=0)
     experiments: Mapped[List["Experiment"]] = relationship(
         back_populates="experiment_set", cascade="all, delete-orphan"
     )
 
-    created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    created_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     created_by: Mapped[User] = relationship("User", foreign_keys="ExperimentSet.created_by_id")
-    modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    modified_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     modified_by: Mapped[User] = relationship("User", foreign_keys="ExperimentSet.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
     keyword_objs: Mapped[list[Keyword]] = relationship(
         "Keyword", secondary=experiment_sets_keywords_association_table, backref="experiment_sets"
     )
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/genome_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/license.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import date
 
 from sqlalchemy import Column, Date, Integer, String
 
 from mavedb.db.base import Base
 
 
-class GenomeIdentifier(Base):
-    __tablename__ = "genome_identifiers"
+class License(Base):
+    __tablename__ = "licenses"
 
-    id = Column(Integer, primary_key=True, index=True)
-    identifier = Column(String, nullable=False)
-    db_name = Column(String, nullable=False)
-    db_version = Column(String, nullable=True)
-    url = Column(String, nullable=True)
+    id = Column(Integer, primary_key=True)
+    long_name = Column(String, nullable=False, unique=True)
+    short_name = Column(String, nullable=False, unique=True)
+    text = Column(String, nullable=False, unique=False)
+    link = Column(String, nullable=True, unique=False)
+    version = Column(String, nullable=True, unique=False)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/license.py` & `mavedb-2024.1.0/src/mavedb/models/publication_identifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from datetime import date
 
 from sqlalchemy import Column, Date, Integer, String
+from sqlalchemy.dialects.postgresql import JSONB
 
 from mavedb.db.base import Base
 
 
-class License(Base):
-    __tablename__ = "licenses"
+class PublicationIdentifier(Base):
+    __tablename__ = "publication_identifiers"
 
-    id = Column(Integer, primary_key=True, index=True)
-    long_name = Column(String, nullable=False, unique=True)
-    short_name = Column(String, nullable=False, unique=True)
-    text = Column(String, nullable=False, unique=False)
-    link = Column(String, nullable=True, unique=False)
-    version = Column(String, nullable=True, unique=False)
+    id = Column(Integer, primary_key=True)
+    identifier = Column(String, nullable=False)
+    db_name = Column(String, nullable=False)
+    db_version = Column(String, nullable=True)
+    title = Column(String, nullable=False)
+    abstract = Column(String, nullable=True)
+    authors = Column(JSONB, nullable=False)
+    publication_doi = Column(String, nullable=True)
+    preprint_doi = Column(String, nullable=True)
+    publication_year = Column(Integer, nullable=True)
+    preprint_date = Column(Date, nullable=True)
+    publication_journal = Column(String, nullable=True)
+    url = Column(String, nullable=True)
+    reference_html = Column(String, nullable=True)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/mapped_variant.py` & `mavedb-2024.1.0/src/mavedb/models/mapped_variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from mavedb.db.base import Base
 from .variant import Variant
 
 
 class MappedVariant(Base):
     __tablename__ = "mapped_variants"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
     pre_mapped = Column(JSONB, nullable=False)
     post_mapped = Column(JSONB, nullable=False)
 
-    variant_id = Column(Integer, ForeignKey("variants.id"), nullable=False)
+    variant_id = Column(Integer, ForeignKey("variants.id"), index=True, nullable=False)
     variant: Mapped[Variant] = relationship("Variant", backref=backref("mapped_variants", cascade="all,delete-orphan"))
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/publication_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/uniprot_identifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 from datetime import date
 
 from sqlalchemy import Column, Date, Integer, String
-from sqlalchemy.dialects.postgresql import JSONB
 
 from mavedb.db.base import Base
 
 
-class PublicationIdentifier(Base):
-    __tablename__ = "publication_identifiers"
+class UniprotIdentifier(Base):
+    __tablename__ = "uniprot_identifiers"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False)
     db_name = Column(String, nullable=False)
     db_version = Column(String, nullable=True)
-    title = Column(String, nullable=False)
-    abstract = Column(String, nullable=True)
-    authors = Column(JSONB, nullable=False)
-    publication_doi = Column(String, nullable=True)
-    preprint_doi = Column(String, nullable=True)
-    publication_year = Column(Integer, nullable=True)
-    preprint_date = Column(Date, nullable=True)
-    publication_journal = Column(String, nullable=True)
     url = Column(String, nullable=True)
     reference_html = Column(String, nullable=True)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/raw_read_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/raw_read_identifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 from mavedb.db.base import Base
 
 
 class RawReadIdentifier(Base):
     __tablename__ = "sra_identifiers"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False)
     db_name = Column(String, nullable=False)
     db_version = Column(String, nullable=True)
     url = Column(String, nullable=True)
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/refseq_offset.py` & `mavedb-2024.1.0/src/mavedb/models/refseq_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 from mavedb.models.target_gene import TargetGene
 
 
 class RefseqOffset(Base):
     __tablename__ = "refseq_offsets"
 
     identifier_id = Column(Integer, ForeignKey("refseq_identifiers.id"), nullable=False, primary_key=True)
-    identifier : Mapped[RefseqIdentifier] = relationship(backref=backref("target_gene_offsets", uselist=True))
+    identifier: Mapped[RefseqIdentifier] = relationship(backref=backref("target_gene_offsets", uselist=True))
     target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
-    target_gene : Mapped[TargetGene] = relationship(back_populates="refseq_offset", single_parent=True)
+    target_gene: Mapped[TargetGene] = relationship(back_populates="refseq_offset", single_parent=True)
     offset = Column(Integer, nullable=False)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/score_set.py` & `mavedb-2024.1.0/src/mavedb/models/score_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     Column("sra_identifier_id", ForeignKey("sra_identifiers.id"), primary_key=True),
 )
 
 
 class ScoreSet(Base):
     __tablename__ = "scoresets"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
-    urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
+    urn = Column(String(64), default=generate_temp_urn, index=True, nullable=True, unique=True)
     title = Column(String, nullable=False)
     method_text = Column(String, nullable=False)
     abstract_text = Column(String, nullable=False)
     short_description = Column(String, nullable=False)
     extra_metadata = Column(JSONB, nullable=False)
     dataset_columns = Column(JSONB, nullable=False, default={})
 
@@ -80,32 +80,31 @@
     processing_state = Column(
         Enum(ProcessingState, create_constraint=True, length=32, native_enum=False, validate_strings=True),
         nullable=True,
     )
     processing_errors = Column(JSONB, nullable=True)
     data_usage_policy = Column(String, nullable=True)
 
-    # TODO Refactor the way we track the number of variants?
     num_variants = Column(Integer, nullable=False, default=0)
     variants: Mapped[list["Variant"]] = relationship(back_populates="score_set", cascade="all, delete-orphan")
 
-    experiment_id = Column(Integer, ForeignKey("experiments.id"), nullable=False)
+    experiment_id = Column(Integer, ForeignKey("experiments.id"), index=True, nullable=False)
     experiment: Mapped["Experiment"] = relationship(back_populates="score_sets")
 
     # TODO Standardize on US or GB spelling for licenc/se.
-    licence_id = Column(Integer, ForeignKey("licenses.id"), nullable=False)
+    licence_id = Column(Integer, ForeignKey("licenses.id"), index=True, nullable=False)
     license: Mapped["License"] = relationship("License")
-    superseded_score_set_id = Column("replaces_id", Integer, ForeignKey("scoresets.id"), nullable=True)  # TODO
+    superseded_score_set_id = Column("replaces_id", Integer, ForeignKey("scoresets.id"), index=True, nullable=True)
     superseded_score_set: Mapped[Optional["ScoreSet"]] = relationship(
         "ScoreSet", uselist=False, remote_side=[id], backref=backref("superseding_score_set", uselist=False)
     )
 
-    created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    created_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     created_by: Mapped["User"] = relationship("User", foreign_keys="ScoreSet.created_by_id")
-    modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
+    modified_by_id = Column(Integer, ForeignKey("users.id"), index=True, nullable=True)
     modified_by: Mapped["User"] = relationship("User", foreign_keys="ScoreSet.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
     keyword_objs: Mapped[list["Keyword"]] = relationship(
         "Keyword", secondary=score_sets_keywords_association_table, backref="score_sets"
     )
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/score_set_publication_identifier.py` & `mavedb-2024.1.0/src/mavedb/models/score_set_publication_identifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from sqlalchemy import Column, Integer, Boolean, ForeignKey
 from sqlalchemy.orm import relationship, Mapped
 
 from mavedb.db.base import Base
 
 # Prevent circular imports
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from mavedb.models.score_set import ScoreSet
     from mavedb.models.publication_identifier import PublicationIdentifier
 
 
 class ScoreSetPublicationIdentifierAssociation(Base):
     __tablename__ = "scoreset_publication_identifiers"
 
     score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), primary_key=True)
     publication_identifier_id = Column(Integer, ForeignKey("publication_identifiers.id"), primary_key=True)
     primary = Column(Boolean, nullable=True, default=False)
 
-    score_set : Mapped["ScoreSet"] = relationship("mavedb.models.score_set.ScoreSet", back_populates="publication_identifier_associations")
-    publication : Mapped["PublicationIdentifier"] = relationship("PublicationIdentifier")
+    score_set: Mapped["ScoreSet"] = relationship(
+        "mavedb.models.score_set.ScoreSet", back_populates="publication_identifier_associations"
+    )
+    publication: Mapped["PublicationIdentifier"] = relationship("PublicationIdentifier")
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/target_accession.py` & `mavedb-2024.1.0/src/mavedb/models/target_accession.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/models/target_gene.py` & `mavedb-2024.1.0/src/mavedb/models/target_gene.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 
 # TODO Reformat code without removing dependencies whose use is not detected.
 
 
 class TargetGene(Base):
     __tablename__ = "target_genes"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
     name = Column(String, nullable=False)
     category = Column(String, nullable=False)
 
-    score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), nullable=False)
-    score_set : Mapped[ScoreSet] = relationship(
-        back_populates="target_genes", single_parent=True, uselist=True
-    )
+    score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), index=True, nullable=False)
+    score_set: Mapped[ScoreSet] = relationship(back_populates="target_genes", single_parent=True, uselist=True)
 
-    target_sequence_id = Column(Integer, ForeignKey("target_sequences.id"), nullable=True)
-    accession_id = Column(Integer, ForeignKey("target_accessions.id"), nullable=True)
-    target_sequence : Mapped[TargetSequence] = relationship(
+    target_sequence_id = Column(Integer, ForeignKey("target_sequences.id"), index=True, nullable=True)
+    accession_id = Column(Integer, ForeignKey("target_accessions.id"), index=True, nullable=True)
+    target_sequence: Mapped[TargetSequence] = relationship(
         back_populates="target_genes", cascade="all,delete-orphan", single_parent=True
     )
-    target_accession : Mapped[TargetAccession] = relationship(
+    target_accession: Mapped[TargetAccession] = relationship(
         "TargetAccession",
         backref=backref("target_genes", single_parent=True, uselist=True),
         cascade="all,delete-orphan",
         single_parent=True,
     )
 
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
-    ensembl_offset : Mapped["EnsemblOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
-    refseq_offset : Mapped["RefseqOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
-    uniprot_offset : Mapped["UniprotOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
+    ensembl_offset: Mapped["EnsemblOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
+    refseq_offset: Mapped["RefseqOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
+    uniprot_offset: Mapped["UniprotOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/target_sequence.py` & `mavedb-2024.1.0/src/mavedb/models/target_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 from .taxonomy import Taxonomy
 
 from mavedb.db.base import Base
 
 if TYPE_CHECKING:
     from mavedb.models.target_gene import TargetGene
 
+
 class TargetSequence(Base):
     __tablename__ = "target_sequences"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     sequence_type = Column(String, nullable=False)
     sequence = Column(String, nullable=False)
     label = Column(String, nullable=True)
-    taxonomy_id = Column("taxonomy_id", Integer, ForeignKey("taxonomies.id"), nullable=True)
-    taxonomy : Mapped[Taxonomy] = relationship(
+    taxonomy_id = Column("taxonomy_id", Integer, ForeignKey("taxonomies.id"), index=True, nullable=True)
+    taxonomy: Mapped[Taxonomy] = relationship(
         "Taxonomy",
         backref=backref("target_sequences", single_parent=True),
     )
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
-    target_genes : Mapped[List["TargetGene"]] = relationship(back_populates="target_sequence")
+    target_genes: Mapped[List["TargetGene"]] = relationship(back_populates="target_sequence")
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/taxonomy.py` & `mavedb-2024.1.0/src/mavedb/models/taxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from mavedb.db.base import Base
 from .genome_identifier import GenomeIdentifier
 
 
 class Taxonomy(Base):
     __tablename__ = "taxonomies"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
     tax_id = Column(Integer, nullable=False)
     organism_name = Column(String, nullable=True)
     common_name = Column(String, nullable=True)
     rank = Column(String, nullable=True)
     has_described_species_name = Column(Boolean, nullable=True)
     url = Column(String, nullable=False)
     article_reference = Column(String, nullable=True)
-    genome_identifier_id = Column(Integer, ForeignKey("genome_identifiers.id"), nullable=True)
-    genome_identifier : Mapped[GenomeIdentifier] = relationship("GenomeIdentifier", backref="taxonomy_genomes")
+    genome_identifier_id = Column(Integer, ForeignKey("genome_identifiers.id"), index=True, nullable=True)
+    genome_identifier: Mapped[GenomeIdentifier] = relationship("GenomeIdentifier", backref="taxonomy_genomes")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/uniprot_offset.py` & `mavedb-2024.1.0/src/mavedb/models/uniprot_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from mavedb.models.target_gene import TargetGene
 
 
 class UniprotOffset(Base):
     __tablename__ = "uniprot_offsets"
 
     identifier_id = Column(Integer, ForeignKey("uniprot_identifiers.id"), nullable=False, primary_key=True)
-    identifier : Mapped[UniprotIdentifier] = relationship(
-        "UniprotIdentifier",
-        backref=backref("target_gene_offsets", uselist=True)
+    identifier: Mapped[UniprotIdentifier] = relationship(
+        "UniprotIdentifier", backref=backref("target_gene_offsets", uselist=True)
     )
     target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
-    target_gene : Mapped[TargetGene] = relationship(back_populates="uniprot_offset", single_parent=True)
+    target_gene: Mapped[TargetGene] = relationship(back_populates="uniprot_offset", single_parent=True)
 
     offset = Column(Integer, nullable=False)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/user.py` & `mavedb-2024.1.0/src/mavedb/models/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from sqlalchemy import Boolean, Column, DateTime, ForeignKey, Integer, String, Table
 from sqlalchemy.orm import relationship, Mapped
-from typing import List, TYPE_CHECKING
+from typing import TYPE_CHECKING
 from mavedb.db.base import Base
 from mavedb.models.role import Role
+from mavedb.models.enums.user_role import UserRole
 
 users_roles_association_table = Table(
     "users_roles",
     Base.metadata,
     Column("user_id", ForeignKey("users.id"), primary_key=True),
     Column("role_id", ForeignKey("roles.id"), primary_key=True),
 )
@@ -24,25 +25,26 @@
     last_name = Column(String, nullable=True)
     email = Column(String, nullable=True)
     is_superuser = Column(Boolean, nullable=False, default=False)
     is_staff = Column(Boolean, nullable=False, default=False)
     is_active = Column(Boolean, nullable=False)
     date_joined = Column(DateTime, nullable=True)
     email = Column(String, nullable=True)
-    role_objs : Mapped[List[Role]] = relationship("Role", secondary=users_roles_association_table, backref="users")
+    role_objs: Mapped[list[Role]] = relationship("Role", secondary=users_roles_association_table, backref="users")
+    is_first_login: Mapped[bool] = Column(Boolean, nullable=False, default=True)
     last_login = Column(DateTime, nullable=True)
 
-    access_keys : Mapped[List["AccessKey"]] = relationship(back_populates="user", cascade="all, delete-orphan")
+    access_keys: Mapped[list["AccessKey"]] = relationship(back_populates="user", cascade="all, delete-orphan")
 
     @property
-    def roles(self) -> list[str]:
+    def roles(self) -> list[UserRole]:
         role_objs = self.role_objs or []
         return [role_obj.name for role_obj in role_objs if role_obj.name is not None]
 
-    async def set_roles(self, db, roles: list[str]):
+    async def set_roles(self, db, roles: list[UserRole]):
         self.role_objs = [await self._find_or_create_role(db, name) for name in roles]
 
     @staticmethod
     async def _find_or_create_role(db, role_name):
         role_obj = db.query(Role).filter(Role.name == role_name).one_or_none()
         if not role_obj:
             role_obj = Role(name=role_name)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/variant.py` & `mavedb-2024.1.0/src/mavedb/models/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from mavedb.db.base import Base
 from .score_set import ScoreSet
 
 
 class Variant(Base):
     __tablename__ = "variants"
 
-    id = Column(Integer, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True)
 
-    urn = Column(String(64), nullable=True, unique=True, index=True)
+    urn = Column(String(64), index=True, nullable=True, unique=True)
     data = Column(JSONB, nullable=False)
 
-    score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), nullable=False)
+    score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), index=True, nullable=False)
     # TODO examine if delete-orphan is necessary, explore cascade
     score_set: Mapped[ScoreSet] = relationship(back_populates="variants")
 
     hgvs_nt = Column(String, nullable=True)
     hgvs_pro = Column(String, nullable=True)
     hgvs_splice = Column(String, nullable=True)
```

### Comparing `mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_version.py` & `mavedb-2024.1.0/src/mavedb/models/legacy/django_reversion_version.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/api_information.py` & `mavedb-2024.1.0/src/mavedb/routers/api_information.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/doi_identifiers.py` & `mavedb-2024.1.0/src/mavedb/routers/doi_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/experiment_sets.py` & `mavedb-2024.1.0/src/mavedb/routers/experiment_sets.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/experiments.py` & `mavedb-2024.1.0/src/mavedb/routers/experiments.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from fastapi import APIRouter, Depends, HTTPException
 from fastapi.encoders import jsonable_encoder
 from sqlalchemy import or_, and_
 from sqlalchemy.orm import Session
 
 from mavedb import deps
+from mavedb.lib.authentication import get_current_user, UserData
 from mavedb.lib.authentication import get_current_user
-from mavedb.lib.authorization import require_current_user
+from mavedb.lib.authorization import require_current_user, require_current_user_with_email
 from mavedb.lib.experiments import search_experiments as _search_experiments
 from mavedb.lib.identifiers import (
     find_or_create_doi_identifier,
     find_or_create_publication_identifier,
     find_or_create_raw_read_identifier,
 )
 from mavedb.lib.permissions import assert_permission, Action
 from mavedb.models.experiment import Experiment
 from mavedb.models.experiment_set import ExperimentSet
 from mavedb.models.score_set import ScoreSet
-from mavedb.models.user import User
 from mavedb.view_models import experiment, score_set
 from mavedb.view_models.search import ExperimentsSearch
 
 import requests
 
 logger = logging.getLogger(__name__)
 
@@ -35,25 +35,27 @@
     "/experiments/", status_code=200, response_model=list[experiment.Experiment], response_model_exclude_none=True
 )
 def list_experiments(
     *,
     editable: Optional[bool] = None,
     q: Optional[str] = None,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: UserData = Depends(get_current_user),
 ) -> list[Experiment]:
     """
     List experiments.
     """
     query = db.query(Experiment)
     if q is not None:
-        if user is None:
+        if user_data.user is None:
             return []
         if len(q) > 0:
-            query = query.filter(Experiment.created_by_id == user.id)  # .filter(Experiment.published_date is None)
+            query = query.filter(
+                Experiment.created_by_id == user_data.user.id
+            )  # .filter(Experiment.published_date is None)
         # else:
         #     query = query.filter(Experiment.created_by_id == user.id).filter(Experiment.published_date is None)
     items = query.order_by(Experiment.urn).all()
     return items
 
 
 @router.post("/experiments/search", status_code=200, response_model=list[experiment.ShortExperiment])
@@ -62,89 +64,94 @@
     Search experiments.
     """
     return _search_experiments(db, None, search)
 
 
 @router.post("/me/experiments/search", status_code=200, response_model=list[experiment.ShortExperiment])
 def search_my_experiments(
-    search: ExperimentsSearch, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
+    search: ExperimentsSearch, db: Session = Depends(deps.get_db), user_data: UserData = Depends(require_current_user)
 ) -> Any:
     """
     Search experiments created by the current user..
     """
-    return _search_experiments(db, user, search)
+    return _search_experiments(db, user_data.user, search)
 
 
 @router.get(
     "/experiments/{urn}",
     status_code=200,
     response_model=experiment.Experiment,
     responses={404: {}},
     response_model_exclude_none=True,
 )
 def fetch_experiment(
     *,
     urn: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: Optional[UserData] = Depends(get_current_user),
 ) -> Experiment:
     """
     Fetch a single experiment by URN.
     """
     # item = db.query(Experiment).filter(Experiment.urn == urn).filter(Experiment.private.is_(False)).first()
     item = db.query(Experiment).filter(Experiment.urn == urn).first()
     if not item:
         raise HTTPException(status_code=404, detail=f"Experiment with URN {urn} not found")
-    assert_permission(user, item, Action.READ)
+    assert_permission(user_data, item, Action.READ)
     return item
 
 
 @router.get(
     "/experiments/{urn}/score-sets",
     status_code=200,
     response_model=list[score_set.ScoreSet],
     responses={404: {}},
     response_model_exclude_none=True,
 )
 def get_experiment_score_sets(
     *,
     urn: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: Optional[UserData] = Depends(get_current_user),
 ) -> Any:
     """
     Get all score sets belonging to an experiment.
     """
     experiment = db.query(Experiment).filter(Experiment.urn == urn).first()
     if not experiment:
         raise HTTPException(status_code=404, detail=f"experiment with URN '{urn}' not found")
-    assert_permission(user, experiment, Action.READ)
+    assert_permission(user_data, experiment, Action.READ)
     # If there is a current user with score sets associated with this experiment, return all of them. Otherwise, only show
     # the public / published score sets.
-    score_sets = (
-        db.query(ScoreSet)
-        .filter(ScoreSet.experiment_id == experiment.id)
-        .filter(or_(ScoreSet.private.is_(False), and_(ScoreSet.private.is_(True), ScoreSet.created_by == user)))
-        .all()
-    )
-    if not score_sets:
+    #
+    # TODO(#182): A side effect of this implementation is that only the user who has created the experiment may view all the Score sets
+    # associated with a given experiment. This could be solved with user impersonation for certain user roles.
+    score_sets = db.query(ScoreSet).filter(ScoreSet.experiment_id == experiment.id)
+    if user_data is not None:
+        score_set_result = score_sets.filter(
+            or_(ScoreSet.private.is_(False), and_(ScoreSet.private.is_(True), ScoreSet.created_by == user_data.user))
+        ).all()
+    else:
+        score_set_result = score_sets.filter(ScoreSet.private.is_(False)).all()
+
+    if not score_set_result:
         raise HTTPException(status_code=404, detail="no associated score sets")
     else:
-        score_sets.sort(key=attrgetter("urn"))
-    return score_sets
+        score_set_result.sort(key=attrgetter("urn"))
+    return score_set_result
 
 
 @router.post(
     "/experiments/", response_model=experiment.Experiment, responses={422: {}}, response_model_exclude_none=True
 )
 async def create_experiment(
     *,
     item_create: experiment.ExperimentCreate,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
+    user_data: UserData = Depends(require_current_user_with_email),
 ) -> Any:
     """
     Create an experiment.
     """
     if item_create is None:
         return None
     experiment_set = None
@@ -152,15 +159,15 @@
         experiment_set = (
             db.query(ExperimentSet).filter(ExperimentSet.urn == item_create.experiment_set_urn).one_or_none()
         )
         if not experiment_set:
             raise HTTPException(
                 status_code=404, detail=f"experiment set with URN '{item_create.experiment_set_urn}' not found."
             )
-        assert_permission(user, experiment_set, Action.ADD_EXPERIMENT)
+        assert_permission(user_data, experiment_set, Action.ADD_EXPERIMENT)
     try:
         doi_identifiers = [
             await find_or_create_doi_identifier(db, identifier.identifier)
             for identifier in item_create.doi_identifiers or []
         ]
         raw_read_identifiers = [
             await find_or_create_raw_read_identifier(db, identifier.identifier)
@@ -198,16 +205,16 @@
                 "raw_read_identifiers",
             },
         ),
         experiment_set=experiment_set,
         doi_identifiers=doi_identifiers,
         publication_identifiers=publication_identifiers,  # an internal association proxy representation
         raw_read_identifiers=raw_read_identifiers,
-        created_by=user,
-        modified_by=user,
+        created_by=user_data.user,
+        modified_by=user_data.user,
     )  # type: ignore
     await item.set_keywords(db, item_create.keywords)
     db.add(item)
     db.commit()
     db.refresh(item)
     return item
 
@@ -216,26 +223,26 @@
     "/experiments/{urn}", response_model=experiment.Experiment, responses={422: {}}, response_model_exclude_none=True
 )
 async def update_experiment(
     *,
     item_update: experiment.ExperimentUpdate,
     urn: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
+    user_data: UserData = Depends(require_current_user_with_email),
 ) -> Any:
     """
     Update an experiment.
     """
     if item_update is None:
         return None
     # item = db.query(Experiment).filter(Experiment.urn == urn).filter(Experiment.private.is_(False)).one_or_none()
     item = db.query(Experiment).filter(Experiment.urn == urn).one_or_none()
     if item is None:
         raise HTTPException(status_code=404, detail=f"experiment with URN {urn} not found")
-    assert_permission(user, item, Action.UPDATE)
+    assert_permission(user_data, item, Action.UPDATE)
 
     pairs = {
         k: v
         for k, v in vars(item_update).items()
         if k
         not in [
             "doi_identifiers",
@@ -272,28 +279,29 @@
         setattr(publication, "primary", publication.identifier in primary_identifiers)
 
     item.doi_identifiers = doi_identifiers
     item.publication_identifiers = publication_identifiers
     item.raw_read_identifiers = raw_read_identifiers
 
     await item.set_keywords(db, item_update.keywords)
-    item.modified_by = user
+    item.modified_by = user_data.user
 
     db.add(item)
     db.commit()
     db.refresh(item)
     return item
 
 
-@router.delete(
-    "/experiments/{urn}", response_model=experiment.Experiment, responses={422: {}}, response_model_exclude_none=True
-)
+@router.delete("/experiments/{urn}", response_model=None, responses={422: {}})
 async def delete_experiment(
-    *, urn: str, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
-) -> Any:
+    *,
+    urn: str,
+    db: Session = Depends(deps.get_db),
+    user_data: UserData = Depends(require_current_user),
+) -> None:
     """
     Delete a experiment .
 
     Raises
 
     Returns
     _______
@@ -302,11 +310,11 @@
     or
     communitcate to client whether the operation succeeded
     204 if successful but not returning content - likely going with this
     """
     item = db.query(Experiment).filter(Experiment.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"experiment with URN '{urn}' not found.")
-    assert_permission(user, item, Action.DELETE)
+    assert_permission(user_data, item, Action.DELETE)
 
     db.delete(item)
     db.commit()
```

### Comparing `mavedb-2024.0.0/src/mavedb/routers/hgvs.py` & `mavedb-2024.1.0/src/mavedb/routers/hgvs.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/licenses.py` & `mavedb-2024.1.0/src/mavedb/routers/licenses.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/mapped_variant.py` & `mavedb-2024.1.0/src/mavedb/routers/mapped_variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/publication_identifiers.py` & `mavedb-2024.1.0/src/mavedb/routers/publication_identifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-from typing import Any, List, Optional
+from typing import Any, List
 
 from fastapi import APIRouter, Depends, HTTPException
 from sqlalchemy import func
 from sqlalchemy.exc import MultipleResultsFound
 from sqlalchemy.orm import Session
 
 from mavedb import deps
-from mavedb.lib.authentication import get_current_user
 from mavedb.lib.identifiers import find_generic_article
 from mavedb.models.publication_identifier import PublicationIdentifier
-from mavedb.models.user import User
 from mavedb.view_models import publication_identifier
 from mavedb.view_models.search import TextSearch
 
 router = APIRouter(
     prefix="/api/v1/publication-identifiers",
     tags=["publication identifiers"],
     responses={404: {"description": "Not found"}},
 )
 
 
 @router.get("/", status_code=200, response_model=list[publication_identifier.PublicationIdentifier])
-def list_publications(
-    *,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> Any:
+def list_publications(*, db: Session = Depends(deps.get_db)) -> Any:
     """
     List stored all stored publications.
     """
     items = db.query(PublicationIdentifier).all()
     return items
 
 
 @router.get(
     "/{identifier}",
     status_code=200,
     response_model=publication_identifier.PublicationIdentifier,
     responses={404: {}},
 )
-def fetch_publication_by_identifier(
-    *,
-    identifier: str,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> PublicationIdentifier:
+def fetch_publication_by_identifier(*, identifier: str, db: Session = Depends(deps.get_db)) -> PublicationIdentifier:
     """
     Fetch a single publication by identifier.
     """
     try:
         item = db.query(PublicationIdentifier).filter(PublicationIdentifier.identifier == identifier).one_or_none()
     except MultipleResultsFound:
         raise HTTPException(
@@ -68,15 +57,14 @@
     responses={404: {}},
 )
 def fetch_publication_by_dbname_and_identifier(
     *,
     db_name: str,
     identifier: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
 ) -> PublicationIdentifier:
     """
     Fetch a single publication by db name and identifier.
     """
     try:
         item = (
             db.query(PublicationIdentifier)
@@ -93,49 +81,37 @@
             status_code=404,
             detail=f"No publication with identifier {identifier} and database name {db_name} were found.",
         )
     return item
 
 
 @router.get("/journals", status_code=200, response_model=list[str], responses={404: {}})
-def list_publication_journal_names(
-    *,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> Any:
+def list_publication_journal_names(*, db: Session = Depends(deps.get_db)) -> Any:
     """
     List distinct journal names, in alphabetical order.
     """
 
     items = db.query(PublicationIdentifier).all()
     journals = map(lambda item: item.publication_journal, items)
     return sorted(list(set(journals)))
 
 
 @router.get("/databases", status_code=200, response_model=list[str], responses={404: {}})
-def list_publication_database_names(
-    *,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> Any:
+def list_publication_database_names(*, db: Session = Depends(deps.get_db)) -> Any:
     """
     List distinct database names, in alphabetical order.
     """
 
     items = db.query(PublicationIdentifier).all()
     databases = map(lambda item: item.db_name, items)
     return sorted(list(set(databases)))
 
 
 @router.post("/search", status_code=200, response_model=list[publication_identifier.PublicationIdentifier])
-def search_publication_identifiers(
-    search: TextSearch,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> Any:
+def search_publication_identifiers(search: TextSearch, db: Session = Depends(deps.get_db)) -> Any:
     """
     Search publication identifiers via a TextSearch query.
     """
 
     query = db.query(PublicationIdentifier)
 
     if search.text and len(search.text.strip()) > 0:
@@ -152,17 +128,15 @@
 
 @router.get(
     "/search/{identifier}",
     status_code=200,
     response_model=publication_identifier.PublicationIdentifier,
     responses={404: {}, 500: {}},
 )
-async def search_publications_by_identifier(
-    *, identifier: str, db: Session = Depends(deps.get_db), user: User = Depends(get_current_user)
-) -> Any:
+async def search_publications_by_identifier(*, identifier: str, db: Session = Depends(deps.get_db)) -> Any:
     """
     Search publication identifiers via their identifier.
     """
     query = db.query(PublicationIdentifier).filter(PublicationIdentifier.identifier == identifier).all()
 
     if not query:
         raise HTTPException(status_code=404, detail=f"No publications with identifier {identifier} were found.")
@@ -176,15 +150,14 @@
     responses={404: {}, 500: {}},
 )
 async def search_publications_by_identifier_and_db(
     *,
     identifier: str,
     db_name: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
 ) -> Any:
     """
     Search publication identifiers via their identifier and database.
     """
     query = (
         db.query(PublicationIdentifier)
         .filter(PublicationIdentifier.identifier == identifier and PublicationIdentifier.db_name == db_name)
@@ -198,19 +171,15 @@
         )
     return query
 
 
 @router.post(
     "/search-external", status_code=200, response_model=List[publication_identifier.ExternalPublicationIdentifier]
 )
-async def search_external_publication_identifiers(
-    search: TextSearch,
-    db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
-) -> Any:
+async def search_external_publication_identifiers(search: TextSearch, db: Session = Depends(deps.get_db)) -> Any:
     """
     Search external publication identifiers via a TextSearch query.
     Technically, this should be some sort of accepted publication identifier.
     """
 
     if search.text and len(search.text.strip()) > 0:
         lower_search_text = search.text.strip().lower()
```

### Comparing `mavedb-2024.0.0/src/mavedb/routers/raw_read_identifiers.py` & `mavedb-2024.1.0/src/mavedb/routers/raw_read_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/score_sets.py` & `mavedb-2024.1.0/src/mavedb/routers/score_sets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,134 +1,119 @@
-import csv
-import io
 import logging
-import re
 from datetime import date
 from typing import Any, List, Optional
 
-import numpy as np
 import pandas as pd
 from arq import ArqRedis
-from cdot.hgvs.dataproviders import RESTDataProvider
 from fastapi import APIRouter, Depends, File, status, UploadFile, Query
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import HTTPException
 from fastapi.responses import StreamingResponse
 from sqlalchemy import or_
 from sqlalchemy.orm import Session
 from sqlalchemy.exc import MultipleResultsFound
 
 from mavedb import deps
-from mavedb.lib.authorization import get_current_user, require_current_user
+from mavedb.lib.authentication import UserData
+from mavedb.lib.authorization import get_current_user, require_current_user, require_current_user_with_email
 from mavedb.lib.identifiers import (
     create_external_gene_identifier_offset,
     find_or_create_doi_identifier,
     find_or_create_publication_identifier,
 )
+from mavedb.lib.logging import LoggedRoute
 from mavedb.lib.permissions import Action, assert_permission
 from mavedb.lib.score_sets import (
     find_meta_analyses_for_experiment_sets,
+    get_score_set_counts_as_csv,
+    get_score_set_scores_as_csv,
     search_score_sets as _search_score_sets,
-    HGVSColumns,
     csv_data_to_df,
+    variants_to_csv_rows,
 )
 from mavedb.lib.taxonomies import find_or_create_taxonomy
 from mavedb.lib.urns import generate_experiment_set_urn, generate_experiment_urn, generate_score_set_urn
 from mavedb.lib.exceptions import MixedTargetError
 from mavedb.models.enums.processing_state import ProcessingState
 from mavedb.models.experiment import Experiment
 from mavedb.models.license import License
 from mavedb.models.mapped_variant import MappedVariant
 from mavedb.models.score_set import ScoreSet
 from mavedb.models.target_gene import TargetGene
 from mavedb.models.target_accession import TargetAccession
-from mavedb.models.taxonomy import Taxonomy
 from mavedb.models.user import User
 from mavedb.models.variant import Variant
 from mavedb.models.target_sequence import TargetSequence
 from mavedb.view_models import mapped_variant
 from mavedb.view_models import score_set
 from mavedb.view_models.search import ScoreSetsSearch
 
 logger = logging.getLogger(__name__)
 
-null_values_re = re.compile(r"\s+|none|nan|na|undefined|n/a|null|nil", flags=re.IGNORECASE)
 
-
-async def fetch_score_set_by_urn(db, urn: str, owner: Optional[User]) -> Optional[ScoreSet]:
+async def fetch_score_set_by_urn(db, urn: str, owner: Optional[UserData]) -> Optional[ScoreSet]:
     """
     Fetch one score set by URN, ensuring that it is either published or owned by a specified user.
 
     :param db: An active database session.
     :param urn: The score set URN.
     :param owner: A user whose private score sets may be included in the search. If None, then the score set will only
         be returned if it is public.
     :return: The score set, or None if the URL was not found or refers to a private score set not owned by the specified
         user.
     """
     try:
-        if owner is not None:
-            permission_filter = or_(
-                ScoreSet.private.is_(False),
-                ScoreSet.created_by_id == owner.id,
-            )
-        else:
-            permission_filter = ScoreSet.private.is_(False)
-        item = db.query(ScoreSet).filter(ScoreSet.urn == urn).filter(permission_filter).one_or_none()
+        item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     except MultipleResultsFound:
         raise HTTPException(status_code=500, detail=f"multiple score sets with URN '{urn}' were found")
+
+    assert_permission(owner, item, Action.READ)
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
     return item
 
 
-def is_null(value):
-    """Return True if a string represents a null value."""
-    value = str(value).strip().lower()
-    return null_values_re.fullmatch(value) or not value
-
-
-router = APIRouter(prefix="/api/v1", tags=["score sets"], responses={404: {"description": "not found"}})
+router = APIRouter(prefix="/api/v1", tags=["score sets"], responses={404: {"description": "not found"}}, route_class=LoggedRoute)
 
 
 @router.post("/score-sets/search", status_code=200, response_model=list[score_set.ShortScoreSet])
 def search_score_sets(search: ScoreSetsSearch, db: Session = Depends(deps.get_db)) -> Any:  # = Body(..., embed=True),
     """
     Search score sets.
     """
     return _search_score_sets(db, None, search)
 
 
 @router.post("/me/score-sets/search", status_code=200, response_model=list[score_set.ShortScoreSet])
 def search_my_score_sets(
     search: ScoreSetsSearch,  # = Body(..., embed=True),
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
+    user_data: UserData = Depends(require_current_user),
 ) -> Any:
     """
     Search score sets created by the current user..
     """
-    return _search_score_sets(db, user, search)
+    return _search_score_sets(db, user_data.user, search)
 
 
 @router.get(
     "/score-sets/{urn}",
     status_code=200,
     response_model=score_set.ScoreSet,
     responses={404: {}, 500: {}},
     response_model_exclude_none=True,
 )
 async def show_score_set(
-    *, urn: str, db: Session = Depends(deps.get_db), user: User = Depends(get_current_user)
+    *, urn: str, db: Session = Depends(deps.get_db), user_data: UserData = Depends(get_current_user)
 ) -> Any:
     """
     Fetch a single score set by URN.
     """
 
-    return await fetch_score_set_by_urn(db, urn, user)
+    return await fetch_score_set_by_urn(db, urn, user_data)
 
 
 @router.get(
     "/score-sets/{urn}/scores",
     status_code=200,
     responses={
         200: {
@@ -140,15 +125,15 @@
 )
 def get_score_set_scores_csv(
     *,
     urn: str,
     start: int = Query(default=None, description="Start index for pagination"),
     limit: int = Query(default=None, description="Number of variants to return"),
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: Optional[UserData] = Depends(get_current_user),
 ) -> Any:
     """
     Return scores from a score set, identified by URN, in CSV format.
     If no start and limit, all of variants of this score set will be returned.
     Example path:
     /score-sets/{urn}/scores
     /score-sets/{urn}/scores?start=0&limit=100
@@ -158,33 +143,18 @@
         raise HTTPException(status_code=400, detail="Start index must be non-negative")
     if limit != None and limit <= 0:
         raise HTTPException(status_code=400, detail="Limit must be positive")
 
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    assert_permission(user, score_set, Action.READ)
+    assert_permission(user_data, score_set, Action.READ)
 
-    assert type(score_set.dataset_columns) is dict
-    score_columns = [str(x) for x in list(score_set.dataset_columns.get("score_columns", []))]
-    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + score_columns
-    type_column = "score_data"
-    variants = score_set.variants
-
-    if start:
-        variants = variants[start:]
-    if limit:
-        variants = variants[:limit]
-
-    rows_data = get_csv_rows_data(variants, columns=columns, dtype=type_column)
-    stream = io.StringIO()
-    writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
-    writer.writeheader()
-    writer.writerows(rows_data)
-    return StreamingResponse(iter([stream.getvalue()]), media_type="text/csv")
+    csv_str = get_score_set_scores_as_csv(db, score_set, start, limit)
+    return StreamingResponse(iter([csv_str]), media_type="text/csv")
 
 
 @router.get(
     "/score-sets/{urn}/counts",
     status_code=200,
     responses={
         200: {
@@ -196,15 +166,15 @@
 )
 async def get_score_set_counts_csv(
     *,
     urn: str,
     start: int = Query(default=None, description="Start index for pagination"),
     limit: int = Query(default=None, description="Number of variants to return"),
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: Optional[UserData] = Depends(get_current_user),
 ) -> Any:
     """
     Return counts from a score set, identified by URN, in CSV format.
     If no start and limit, all of variants of this score set will be returned.
     Example path:
     /score-sets/{urn}/counts
     /score-sets/{urn}/counts?start=0&limit=100
@@ -214,49 +184,34 @@
         raise HTTPException(status_code=400, detail="Start index must be non-negative")
     if limit != None and limit <= 0:
         raise HTTPException(status_code=400, detail="Limit must be positive")
 
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN {urn} not found")
-    assert_permission(user, score_set, Action.READ)
+    assert_permission(user_data, score_set, Action.READ)
 
-    assert type(score_set.dataset_columns) is dict
-    count_columns = [str(x) for x in list(score_set.dataset_columns.get("count_columns", []))]
-    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + count_columns
-    type_column = "count_data"
-    variants = score_set.variants
-
-    if start:
-        variants = variants[start:]
-    if limit:
-        variants = variants[:limit]
-
-    rows_data = get_csv_rows_data(variants, columns=columns, dtype=type_column)
-    stream = io.StringIO()
-    writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
-    writer.writeheader()
-    writer.writerows(rows_data)
-    return StreamingResponse(iter([stream.getvalue()]), media_type="text/csv")
+    csv_str = get_score_set_counts_as_csv(db, score_set, start, limit)
+    return StreamingResponse(iter([csv_str]), media_type="text/csv")
 
 
 @router.get("/score-sets/{urn}/mapped-variants", status_code=200, response_model=list[mapped_variant.MappedVariant])
 def get_score_set_mapped_variants(
     *,
     urn: str,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(get_current_user),
+    user_data: Optional[UserData] = Depends(get_current_user),
 ) -> Any:
     """
     Return mapped variants from a score set, identified by URN.
     """
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN {urn} not found")
-    assert_permission(user, score_set, Action.READ)
+    assert_permission(user_data, score_set, Action.READ)
 
     mapped_variants = (
         db.query(MappedVariant)
         .filter(ScoreSet.urn == urn)
         .filter(ScoreSet.id == Variant.score_set_id)
         .filter(Variant.id == MappedVariant.variant_id)
         .all()
@@ -269,38 +224,38 @@
 
 
 @router.post("/score-sets/", response_model=score_set.ScoreSet, responses={422: {}}, response_model_exclude_none=True)
 async def create_score_set(
     *,
     item_create: score_set.ScoreSetCreate,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
+    user_data: UserData = Depends(require_current_user_with_email),
 ) -> Any:
     """
     Create a score set.
     """
 
-    # TODO Confirm that the experiment is editable by this user.
-
     if item_create is None:
         return None
 
     experiment: Optional[Experiment] = None
     if item_create.experiment_urn is not None:
         experiment = db.query(Experiment).filter(Experiment.urn == item_create.experiment_urn).one_or_none()
         if not experiment:
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown experiment")
-        assert_permission(user, experiment, Action.ADD_SCORE_SET)
+
+        assert_permission(user_data, experiment, Action.UPDATE)
+        assert_permission(user_data, experiment, Action.ADD_SCORE_SET)
 
     license_ = db.query(License).filter(License.id == item_create.license_id).one_or_none()
     if not license_:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown license")
 
     if item_create.superseded_score_set_urn is not None:
-        superseded_score_set = await fetch_score_set_by_urn(db, item_create.superseded_score_set_urn, user)
+        superseded_score_set = await fetch_score_set_by_urn(db, item_create.superseded_score_set_urn, user_data)
         if superseded_score_set is None:
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown superseded score set")
     else:
         superseded_score_set = None
 
     distinct_meta_analyzes_score_set_urns = list(set(item_create.meta_analyzes_score_set_urns or []))
     meta_analyzes_score_sets = [
@@ -341,26 +296,26 @@
             experiment = Experiment(
                 experiment_set=meta_analyzes_experiment_set,
                 title=item_create.title,
                 short_description=item_create.short_description,
                 abstract_text=item_create.abstract_text,
                 method_text=item_create.method_text,
                 extra_metadata={},
-                created_by=user,
-                modified_by=user,
+                created_by=user_data.user,
+                modified_by=user_data.user,
             )
         else:
             experiment = Experiment(
                 title=item_create.title,
                 short_description=item_create.short_description,
                 abstract_text=item_create.abstract_text,
                 method_text=item_create.method_text,
                 extra_metadata={},
-                created_by=user,
-                modified_by=user,
+                created_by=user_data.user,
+                modified_by=user_data.user,
             )
 
     doi_identifiers = [
         await find_or_create_doi_identifier(db, identifier.identifier)
         for identifier in item_create.doi_identifiers or []
     ]
     primary_publication_identifiers = [
@@ -458,16 +413,16 @@
         license=license_,
         superseded_score_set=superseded_score_set,
         meta_analyzes_score_sets=meta_analyzes_score_sets,
         target_genes=targets,
         doi_identifiers=doi_identifiers,
         publication_identifiers=publication_identifiers,
         processing_state=ProcessingState.incomplete,
-        created_by=user,
-        modified_by=user,
+        created_by=user_data.user,
+        modified_by=user_data.user,
     )  # type: ignore
     if item_create.keywords is not None:
         await item.set_keywords(db, item_create.keywords)
     db.add(item)
     db.commit()
     db.refresh(item)
     return item
@@ -481,29 +436,29 @@
 )
 async def upload_score_set_variant_data(
     *,
     urn: str,
     counts_file: Optional[UploadFile] = File(None),
     scores_file: UploadFile = File(...),
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
+    user_data: UserData = Depends(require_current_user_with_email),
     worker: ArqRedis = Depends(deps.get_worker),
 ) -> Any:
     """
     Upload scores and variant count files for a score set, and initiate processing these files to
     create variants.
     """
 
-    # TODO Confirm access.
-
     # item = db.query(ScoreSet).filter(ScoreSet.urn == urn).filter(ScoreSet.private.is_(False)).one_or_none()
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item or not item.urn or not scores_file:
         return None
-    assert_permission(user, item, Action.SET_SCORES)
+
+    assert_permission(user_data, item, Action.UPDATE)
+    assert_permission(user_data, item, Action.SET_SCORES)
 
     # Mark the score set as being processed and delete the old variants so that uploading new scores and counts won't accumulate the old ones.
     item.processing_state = ProcessingState.processing
     db.query(Variant).filter(Variant.score_set_id == item.id).delete()
     db.add(item)
     db.commit()
     db.refresh(item)
@@ -511,40 +466,39 @@
     scores_df = csv_data_to_df(scores_file.file)
     counts_df = None
     if counts_file and counts_file.filename:
         counts_df = csv_data_to_df(counts_file.file)
 
     if scores_file:
         # await the insertion of this job into the worker queue, not the job itself.
-        await worker.enqueue_job("create_variants_for_score_set", item.urn, user.id, scores_df, counts_df)
+        await worker.enqueue_job("create_variants_for_score_set", item.urn, user_data.user.id, scores_df, counts_df)
 
     return item
 
 
 @router.put("/score-sets/{urn}", response_model=score_set.ScoreSet, responses={422: {}})
 async def update_score_set(
     *,
     urn: str,
     item_update: score_set.ScoreSetUpdate,
     db: Session = Depends(deps.get_db),
-    user: User = Depends(require_current_user),
-    hdp: RESTDataProvider = Depends(deps.hgvs_data_provider),  # TODO - remove.
+    user_data: UserData = Depends(require_current_user_with_email),
     worker: ArqRedis = Depends(deps.get_worker),
 ) -> Any:
     """
     Update a score set.
     """
 
     if not item_update:
         raise HTTPException(status_code=400, detail="The request contained no updated item.")
 
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    assert_permission(user, item, Action.UPDATE)
+    assert_permission(user_data, item, Action.UPDATE)
 
     # Editing unpublished score set
     if item.private is True:
         license_ = None
         if item_update.license_id is not None:
             license_ = db.query(License).filter(License.id == item_update.license_id).one_or_none()
             if not license_:
@@ -662,22 +616,24 @@
 
         # re-validate existing variants and clear them if they do not pass validation
         if item.variants:
             assert item.dataset_columns is not None
             score_columns = ["hgvs_nt", "hgvs_splice", "hgvs_pro"] + item.dataset_columns["score_columns"]
             count_columns = ["hgvs_nt", "hgvs_splice", "hgvs_pro"] + item.dataset_columns["count_columns"]
             scores_data = pd.DataFrame(
-                get_csv_rows_data(item.variants, columns=score_columns, dtype="score_data")
+                variants_to_csv_rows(item.variants, columns=score_columns, dtype="score_data")
             ).replace("NA", pd.NA)
             count_data = pd.DataFrame(
-                get_csv_rows_data(item.variants, columns=count_columns, dtype="count_data")
+                variants_to_csv_rows(item.variants, columns=count_columns, dtype="count_data")
             ).replace("NA", pd.NA)
 
             # await the insertion of this job into the worker queue, not the job itself.
-            await worker.enqueue_job("create_variants_for_score_set", item.urn, user.id, scores_data, count_data)
+            await worker.enqueue_job(
+                "create_variants_for_score_set", item.urn, user_data.user.id, scores_data, count_data
+            )
 
         for var, value in vars(item_update).items():
             if var not in [
                 "keywords",
                 "doi_identifiers",
                 "experiment_urn",
                 "primary_publication_identifiers",
@@ -696,15 +652,18 @@
     db.commit()
     db.refresh(item)
     return item
 
 
 @router.delete("/score-sets/{urn}", responses={422: {}})
 async def delete_score_set(
-    *, urn: str, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
+    *,
+    urn: str,
+    db: Session = Depends(deps.get_db),
+    user_data: UserData = Depends(require_current_user),
 ) -> Any:
     """
     Delete a score set.
 
     Raises
 
     Returns
@@ -714,32 +673,35 @@
     or
     communitcate to client whether the operation succeeded
     204 if successful but not returning content - likely going with this
     """
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    assert_permission(user, item, Action.DELETE)
+    assert_permission(user_data, item, Action.DELETE)
     db.delete(item)
     db.commit()
 
 
 @router.post(
     "/score-sets/{urn}/publish", status_code=200, response_model=score_set.ScoreSet, response_model_exclude_none=True
 )
 def publish_score_set(
-    *, urn: str, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
+    *,
+    urn: str,
+    db: Session = Depends(deps.get_db),
+    user_data: UserData = Depends(require_current_user),
 ) -> Any:
     """
     Publish a score set.
     """
     item: Optional[ScoreSet] = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    assert_permission(user, item, Action.UPDATE)
+    assert_permission(user_data, item, Action.PUBLISH)
 
     if not item.experiment:
         raise HTTPException(
             status_code=500, detail="This score set does not belong to an experiment and cannot be published."
         )
     if not item.experiment.experiment_set:
         raise HTTPException(
@@ -776,48 +738,7 @@
     item.private = False
     item.published_date = published_date
     db.add(item)
 
     db.commit()
     db.refresh(item)
     return item
-
-
-def get_csv_rows_data(variants, columns, dtype, na_rep="NA"):
-    """
-    Format each variant into a dictionary row containing the keys specified
-    in `columns`.
-
-    Parameters
-    ----------
-    variants : list[variant.models.Variant`]
-        List of variants.
-    columns : list[str]
-        Columns to serialize.
-    dtype : str, {'scores', 'counts'}
-        The type of data requested. Either the 'score_data' or 'count_data'.
-    na_rep : str
-        String to represent null values.
-
-    Returns
-    -------
-    list[dict]
-    """
-    row_dicts = []
-    for variant in variants:
-        data = {}
-        for column_key in columns:
-            if column_key == "hgvs_nt":
-                value = str(variant.hgvs_nt)
-            elif column_key == "hgvs_pro":
-                value = str(variant.hgvs_pro)
-            elif column_key == "hgvs_splice":
-                value = str(variant.hgvs_splice)
-            elif column_key == "accession":
-                value = str(variant.urn)
-            else:
-                value = str(variant.data[dtype][column_key])
-            if is_null(value):
-                value = na_rep
-            data[column_key] = value
-        row_dicts.append(data)
-    return row_dicts
```

### Comparing `mavedb-2024.0.0/src/mavedb/routers/statistics.py` & `mavedb-2024.1.0/src/mavedb/routers/statistics.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/target_gene_identifiers.py` & `mavedb-2024.1.0/src/mavedb/routers/target_gene_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/target_genes.py` & `mavedb-2024.1.0/src/mavedb/routers/target_genes.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/routers/taxonomies.py` & `mavedb-2024.1.0/src/mavedb/routers/taxonomies.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/__init__.py` & `mavedb-2024.1.0/src/mavedb/view_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/access_key.py` & `mavedb-2024.1.0/src/mavedb/view_models/access_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from datetime import date
 from typing import Optional
 
 from mavedb.view_models.base.base import BaseModel
+from mavedb.models.enums.user_role import UserRole
 
 
 class AccessKeyBase(BaseModel):
     key_id: str
     name: Optional[str]
     expiration_date: Optional[date]
     created_at: Optional[str]
 
 
 # Properties shared by models stored in DB
 class SavedAccessKey(AccessKeyBase):
     class Config:
         orm_mode = True
 
+    role: Optional[UserRole]
+
 
 # Properties to return to non-admin clients
 class AccessKey(SavedAccessKey):
     pass
 
 
 # Properties to return when an access key has just been created
```

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/doi_identifier.py` & `mavedb-2024.1.0/src/mavedb/view_models/doi_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/experiment.py` & `mavedb-2024.1.0/src/mavedb/view_models/experiment.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,20 +86,18 @@
     urn: str
     created_by: SavedUser
     modified_by: SavedUser
     creation_date: date
     modification_date: date
     published_date: Optional[date]
     experiment_set_urn: str
-    score_set_urns: list[str]
     doi_identifiers: Sequence[SavedDoiIdentifier]
     primary_publication_identifiers: Sequence[SavedPublicationIdentifier]
     secondary_publication_identifiers: Sequence[SavedPublicationIdentifier]
     raw_read_identifiers: Sequence[SavedRawReadIdentifier]
-    processing_state: Optional[str]
     keywords: list[str]
 
     class Config:
         orm_mode = True
         getter_dict = ExperimentGetter
 
     # Association proxy objects return an untyped _AssocitionList object.
@@ -108,22 +106,36 @@
     def publication_identifiers_validator(cls, value, values, field) -> list[PublicationIdentifier]:
         assert isinstance(value, Collection), f"{field.name} must be a collection, not {type(value)}"
         return list(value)  # Re-cast into proper list-like type
 
 
 # Properties to return to non-admin clients
 class Experiment(SavedExperiment):
+    score_set_urns: list[str]
+    processing_state: Optional[str]
     doi_identifiers: Sequence[DoiIdentifier]
     primary_publication_identifiers: Sequence[PublicationIdentifier]
     secondary_publication_identifiers: Sequence[PublicationIdentifier]
     raw_read_identifiers: Sequence[RawReadIdentifier]
     created_by: User
     modified_by: User
 
 
 class ShortExperiment(SavedExperiment):
-    pass
+    score_set_urns: list[str]
+    processing_state: Optional[str]
 
 
 # Properties to return to admin clients
-class AdminExperiment(SavedExperiment):
+class AdminExperiment(Experiment):
+    score_set_urns: list[str]
+    processing_state: Optional[str]
     approved: bool
+
+
+# Properties to include in a dump of all published data.
+class ExperimentPublicDump(SavedExperiment):
+    score_sets: "Sequence[ScoreSetPublicDump]"
+
+
+from mavedb.view_models.score_set import ScoreSetPublicDump
+ExperimentPublicDump.update_forward_refs()
```

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/experiment_set.py` & `mavedb-2024.1.0/src/mavedb/view_models/experiment_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import date
 from typing import List, Sequence
 
 from pydantic.types import Optional
 
 from mavedb.view_models.base.base import BaseModel
-from mavedb.view_models.experiment import Experiment, SavedExperiment
+from mavedb.view_models.experiment import Experiment, ExperimentPublicDump, SavedExperiment
 from mavedb.view_models.user import SavedUser, User
 
 
 class ExperimentSetBase(BaseModel):
     urn: str
     published_date: Optional[date]
 
@@ -45,7 +45,14 @@
 class AdminExperimentSet(SavedExperimentSet):
     private: bool
     approved: bool
     processing_state: Optional[str]
     created_by: Optional[User]
     modified_by: Optional[User]
     experiments: Sequence[Experiment]
+
+
+# Properties to include in a dump of all published data.
+class ExperimentSetPublicDump(SavedExperimentSet):
+    experiments: Sequence[ExperimentPublicDump]
+    created_by: Optional[User]
+    modified_by: Optional[User]
```

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier.py` & `mavedb-2024.1.0/src/mavedb/view_models/external_gene_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier_offset.py` & `mavedb-2024.1.0/src/mavedb/view_models/external_gene_identifier_offset.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/license.py` & `mavedb-2024.1.0/src/mavedb/view_models/license.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/publication_identifier.py` & `mavedb-2024.1.0/src/mavedb/view_models/publication_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/score_set.py` & `mavedb-2024.1.0/src/mavedb/view_models/score_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,28 +84,37 @@
 
         return field_value
 
     # Validate nested label fields are not identical
     @validator("target_genes")
     def target_labels_are_unique(cls, field_value, values):
         # Labels are only used on target sequence instances.
-        if len(field_value) > 1 and all([isinstance(target, TargetSequence) for target in field_value]):
+        if len(field_value) > 1 and all([target.target_sequence is not None for target in field_value]):
+            # Labels have already been sanitized by the TargetSequence validator.
             labels = [target.target_sequence.label for target in field_value]
             dup_indices = [idx for idx, item in enumerate(labels) if item in labels[:idx]]
             if dup_indices:
                 # TODO: surface the error for the each duplicated index. the way these pydantic validators are
                 # implemented would require additional customization to surface each duplicate, so surfacing
                 # just one for now seems fine.
                 raise ValidationError(
                     "Target sequence labels cannot be duplicated.",
                     custom_loc=["body", "targetGene", dup_indices[-1], "targetSequence", "label"],
                 )
 
         return field_value
 
+    # Validate that this score set contains at least one target attached to it
+    @validator("target_genes")
+    def at_least_one_target_gene_exists(cls, field_value, values):
+        if len(field_value) < 1:
+            raise ValidationError("Score sets should define at least one target.")
+
+        return field_value
+
     @validator("keywords")
     def validate_keywords(cls, v):
         keywords.validate_keywords(v)
         return v
 
 
 class ScoreSetCreate(ScoreSetModify):
@@ -192,15 +201,14 @@
 
 
 class SavedScoreSet(ScoreSetBase):
     """Base class for score set view models representing saved records."""
 
     urn: str
     num_variants: int
-    experiment: SavedExperiment
     license: ShortLicense
     superseded_score_set_urn: Optional[str]
     superseding_score_set_urn: Optional[str]
     meta_analyzes_score_set_urns: list[str]
     meta_analyzed_by_score_set_urns: list[str]
     doi_identifiers: Sequence[SavedDoiIdentifier]
     primary_publication_identifiers: Sequence[SavedPublicationIdentifier]
@@ -256,7 +264,21 @@
 
 
 class AdminScoreSet(ScoreSet):
     """Score set view model containing properties to return to admin clients."""
 
     normalised: bool
     approved: bool
+
+
+class ScoreSetPublicDump(SavedScoreSet):
+    """Score set view model containing properties to include in a dump of all published data."""
+
+    doi_identifiers: Sequence[DoiIdentifier]
+    primary_publication_identifiers: Sequence[PublicationIdentifier]
+    secondary_publication_identifiers: Sequence[PublicationIdentifier]
+    created_by: Optional[User]
+    modified_by: Optional[User]
+    target_genes: Sequence[TargetGene]
+    private: bool
+    processing_state: Optional[ProcessingState]
+    processing_errors: Optional[dict]
```

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/search.py` & `mavedb-2024.1.0/src/mavedb/view_models/search.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/target_accession.py` & `mavedb-2024.1.0/src/mavedb/view_models/target_accession.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/target_gene.py` & `mavedb-2024.1.0/src/mavedb/view_models/target_gene.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/target_sequence.py` & `mavedb-2024.1.0/src/mavedb/view_models/target_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from mavedb.view_models.taxonomy import AdminTaxonomy, SavedTaxonomy, Taxonomy, TaxonomyCreate
 from mavedb.lib.validation import target
 from mavedb.lib.validation.exceptions import ValidationError
 
 from fqfa import infer_sequence_type
 
 
+def sanitize_target_sequence_label(label: str):
+    return label.strip().replace(" ", "_")
+
+
 class TargetSequenceBase(BaseModel):
     sequence_type: str
     sequence: str
     label: Optional[str]
 
 
 class TargetSequenceModify(TargetSequenceBase):
@@ -36,21 +40,23 @@
             # field_value is sequence
             target.validate_target_sequence(field_value, sequence_type)
         else:
             raise ValueError("sequence_type is invalid")
         return field_value
 
     @validator("label")
-    def check_alphanumeric(cls, field_value, values, field, config) -> str:
+    def label_does_not_include_colon(cls, field_value, values, field, config) -> str:
         if isinstance(field_value, str):
-            is_alphanumeric = field_value.replace("_", "").isalnum()
-            if not is_alphanumeric:
-                raise ValidationError(
-                    f"Target sequence label `{field_value}` can contain only letters, numbers, and underscores."
-                )
+            if ":" in field_value:
+                raise ValidationError(f"Target sequence label `{field_value}` may not contain a colon.")
+
+            # Sanitize the label by stripping leading/trailing whitespace and replacing any internal whitespace with
+            # underscores. Fully qualified variants should never contain whitespace.
+            return sanitize_target_sequence_label(field_value)
+
         return field_value
 
 
 class TargetSequenceCreate(TargetSequenceModify):
     taxonomy: TaxonomyCreate
```

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/taxonomy.py` & `mavedb-2024.1.0/src/mavedb/view_models/taxonomy.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/variant.py` & `mavedb-2024.1.0/src/mavedb/view_models/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/view_models/base/base.py` & `mavedb-2024.1.0/src/mavedb/view_models/base/base.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/worker/__init__.py` & `mavedb-2024.1.0/src/mavedb/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/worker/jobs.py` & `mavedb-2024.1.0/src/mavedb/worker/jobs.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/src/mavedb/worker/settings.py` & `mavedb-2024.1.0/src/mavedb/worker/settings.py`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/LICENSE` & `mavedb-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mavedb-2024.0.0/README.md` & `mavedb-2024.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,31 +22,36 @@
 
 ## Building and running mavedb-api
 
 ### Prerequisites
 
 - Python 3.9 or later
 - PIP
-- [build](https://github.com/pypa/hatch) for building distributions. This can be installed with `pip install build`.
-- [hatch](https://github.com/pypa/hatch) for building distributions. This can be installed with `pip install hatch`.
+- [Poetry](https://python-poetry.org/) for building and publishing distributions. For details on installing poetry, consult its [documentation](https://python-poetry.org/docs/#installation).
 
 ### Building distribution packages
 
 To build the source distribution and wheel, run
 
 ```
-python -m build
+poetry build
 ```
 
-The build utility will look at `pyproject.toml` and invoke Hatchling to build the distributions.
+The build utility will look at `pyproject.toml` and invoke Poetry to build the distributions. Note that it will output build artifacts to `./dist` by default.
 
-The distribution can be uploaded to PyPI using [twine](https://twine.readthedocs.io/en/stable/).
+The distribution can be uploaded to PyPI using Poetry as well. After building the packaged, simply invoke
+
+```
+poetry publish -r pypi -u <username> -p <password>
+```
+
+To build and publish the package in one go, just pass the `--build` flag to the publish command.
 
 For use as a server, this distribution includes an optional set of dependencies, which are only invoked if the package
-is installed with `pip install mavedb[server]`.
+is installed with `poetry install mavedb --extras server`.
 
 ### Running a local version of the API server
 
 First build the application's Docker image:
 ```
 docker build --tag mavedb-api/mavedb-api .
 ```
```

