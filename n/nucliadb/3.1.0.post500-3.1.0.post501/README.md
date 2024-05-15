# Comparing `tmp/nucliadb-3.1.0.post500-py3-none-any.whl.zip` & `tmp/nucliadb-3.1.0.post501-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,458 +1,462 @@
-Zip file size: 752681 bytes, number of entries: 456
--rw-r--r--  2.0 unx     1135 b- defN 24-May-14 11:08 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-14 11:08 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-14 11:08 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-14 11:08 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-14 11:08 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-14 11:08 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-14 11:08 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-14 11:08 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-14 11:08 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-14 11:08 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-14 11:08 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-14 11:08 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-14 11:08 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-14 11:08 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-14 11:08 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-14 11:08 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-14 11:08 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-14 11:08 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-14 11:08 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-14 11:08 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-14 11:08 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-May-14 11:08 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-14 11:08 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-14 11:08 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-14 11:08 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-May-14 11:08 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-14 11:08 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-14 11:08 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-14 11:08 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-14 11:08 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22097 b- defN 24-May-14 11:08 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8593 b- defN 24-May-14 11:08 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-14 11:08 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2992 b- defN 24-May-14 11:08 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5730 b- defN 24-May-14 11:08 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-14 11:08 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-14 11:08 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-14 11:08 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-14 11:08 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-14 11:08 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-14 11:08 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-14 11:08 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-14 11:08 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-14 11:08 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-14 11:08 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-14 11:08 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-14 11:08 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-14 11:08 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-14 11:08 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-14 11:08 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-14 11:08 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-14 11:08 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-14 11:08 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-14 11:08 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-May-14 11:08 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-14 11:08 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-14 11:08 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-14 11:08 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-14 11:08 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-14 11:08 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-14 11:08 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-14 11:08 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-14 11:08 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-14 11:08 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-14 11:08 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-14 11:08 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-14 11:08 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-May-14 11:08 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-14 11:08 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-May-14 11:08 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-14 11:08 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-14 11:08 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-14 11:08 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-14 11:08 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-14 11:08 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-14 11:08 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-14 11:08 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-14 11:08 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-14 11:08 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-14 11:08 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-14 11:08 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-14 11:08 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-May-14 11:08 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-14 11:08 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-14 11:08 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-14 11:08 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-14 11:08 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-14 11:08 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-14 11:08 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-14 11:08 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-May-14 11:08 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-14 11:08 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-14 11:08 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33196 b- defN 24-May-14 11:08 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-14 11:08 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-14 11:08 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-14 11:08 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27336 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-14 11:08 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     4004 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-14 11:08 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-14 11:08 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-14 11:08 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-14 11:08 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-14 11:08 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-14 11:08 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-14 11:08 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9249 b- defN 24-May-14 11:08 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-14 11:08 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-14 11:08 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-14 11:08 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-14 11:08 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-14 11:08 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-14 11:08 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-14 11:08 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-14 11:08 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-14 11:08 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-14 11:08 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-14 11:08 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-14 11:08 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-May-14 11:08 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13940 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12399 b- defN 24-May-14 11:08 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-14 11:08 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-14 11:08 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-14 11:08 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-14 11:08 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-14 11:08 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-14 11:08 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-14 11:08 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-14 11:08 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-14 11:08 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-14 11:08 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-14 11:08 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    17332 b- defN 24-May-14 11:08 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-14 11:08 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-14 11:08 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-14 11:08 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1222 b- defN 24-May-14 11:08 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9882 b- defN 24-May-14 11:08 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-14 11:08 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8810 b- defN 24-May-14 11:08 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-14 11:08 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-14 11:08 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-14 11:08 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18337 b- defN 24-May-14 11:08 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-14 11:08 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-14 11:08 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-14 11:08 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-14 11:08 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-14 11:08 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-14 11:08 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-14 11:08 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-14 11:08 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-14 11:08 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-14 11:08 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-14 11:08 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-14 11:08 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-14 11:08 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-14 11:08 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-14 11:08 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-14 11:08 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-14 11:08 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-14 11:08 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-14 11:08 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-14 11:08 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-14 11:08 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-14 11:08 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15401 b- defN 24-May-14 11:08 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-14 11:08 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-14 11:08 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-14 11:08 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    13101 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-14 11:08 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-14 11:08 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-14 11:08 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-14 11:08 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-May-14 11:08 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-May-14 11:08 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-14 11:08 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-14 11:08 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-14 11:08 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5415 b- defN 24-May-14 11:08 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-May-14 11:08 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-14 11:08 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-14 11:08 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-14 11:08 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-14 11:08 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-14 11:08 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-14 11:08 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1845 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1587 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-14 11:08 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-14 11:08 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-14 11:08 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-14 11:08 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-14 11:08 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-14 11:08 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-14 11:08 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-14 11:08 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-14 11:08 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-14 11:08 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-14 11:08 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-14 11:08 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-14 11:08 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-14 11:08 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-14 11:08 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-14 11:08 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-14 11:08 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-14 11:08 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-14 11:08 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3093 b- defN 24-May-14 11:08 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-14 11:08 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-14 11:08 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-14 11:08 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-14 11:08 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-14 11:08 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-14 11:08 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-14 11:08 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-14 11:08 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-14 11:08 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-14 11:08 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-14 11:08 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-14 11:08 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-14 11:08 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-14 11:08 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-14 11:08 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-14 11:08 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-14 11:08 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-14 11:08 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-14 11:08 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-14 11:08 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-14 11:08 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-14 11:08 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-14 11:08 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-14 11:08 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-14 11:08 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-14 11:08 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-14 11:08 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-14 11:08 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-14 11:08 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-14 11:08 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-14 11:08 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-14 11:08 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-14 11:08 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-14 11:08 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-14 11:08 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-14 11:08 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-14 11:08 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-14 11:08 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-14 11:08 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-14 11:08 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-14 11:08 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-14 11:08 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-14 11:08 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-14 11:08 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-14 11:08 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-14 11:08 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-14 11:08 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-14 11:08 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-14 11:08 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-14 11:08 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-14 11:08 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-14 11:08 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-14 11:08 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-14 11:08 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-14 11:08 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-14 11:08 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-14 11:08 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-14 11:08 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-14 11:08 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-14 11:08 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-May-14 11:08 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-14 11:08 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-14 11:08 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-14 11:08 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-14 11:08 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-14 11:08 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-14 11:08 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-14 11:08 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10747 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-14 11:08 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-14 11:08 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-14 11:08 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-14 11:08 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-14 11:08 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-14 11:08 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-14 11:08 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-14 11:08 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-14 11:08 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-14 11:08 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-14 11:08 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-14 11:08 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-14 11:08 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-14 11:08 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-14 11:08 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-14 11:08 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-14 11:08 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-14 11:08 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-14 11:08 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-14 11:08 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-14 11:08 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-14 11:08 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4399 b- defN 24-May-14 11:10 nucliadb-3.1.0.post500.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 11:10 nucliadb-3.1.0.post500.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-14 11:10 nucliadb-3.1.0.post500.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-14 11:10 nucliadb-3.1.0.post500.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-14 11:09 nucliadb-3.1.0.post500.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42769 b- defN 24-May-14 11:10 nucliadb-3.1.0.post500.dist-info/RECORD
-456 files, 2223073 bytes uncompressed, 684287 bytes compressed:  69.2%
+Zip file size: 763335 bytes, number of entries: 460
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-14 23:18 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-14 23:18 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-14 23:18 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-14 23:18 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-14 23:18 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-14 23:18 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-14 23:18 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-14 23:18 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-14 23:18 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-14 23:18 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-14 23:18 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-14 23:18 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-14 23:18 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-14 23:18 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-14 23:18 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-14 23:18 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-14 23:18 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-14 23:18 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-14 23:18 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-14 23:18 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-14 23:18 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-14 23:18 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-14 23:18 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-14 23:18 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 23:18 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-14 23:18 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-14 23:18 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-14 23:18 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-14 23:18 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-14 23:18 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22097 b- defN 24-May-14 23:18 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8593 b- defN 24-May-14 23:18 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-14 23:18 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2992 b- defN 24-May-14 23:18 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5730 b- defN 24-May-14 23:18 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-14 23:18 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-14 23:18 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-14 23:18 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-14 23:18 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-14 23:18 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-14 23:18 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-14 23:18 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-14 23:18 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-14 23:18 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-14 23:18 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-14 23:18 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-14 23:18 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-14 23:18 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-14 23:18 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-14 23:18 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-14 23:18 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-14 23:18 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-14 23:18 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-14 23:18 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-14 23:18 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-14 23:18 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-14 23:18 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-14 23:18 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-14 23:18 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-14 23:18 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-14 23:18 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-14 23:18 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-14 23:18 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-14 23:18 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-14 23:18 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-14 23:18 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-14 23:18 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-14 23:18 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-14 23:18 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-14 23:18 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-14 23:18 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-14 23:18 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-14 23:18 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-14 23:18 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-14 23:18 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-14 23:18 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-14 23:18 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-14 23:18 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-14 23:18 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-14 23:18 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-14 23:18 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-14 23:18 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28448 b- defN 24-May-14 23:18 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-14 23:18 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-14 23:18 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-14 23:18 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-14 23:18 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-14 23:18 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-14 23:18 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-14 23:18 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26423 b- defN 24-May-14 23:18 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-14 23:18 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-14 23:18 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33196 b- defN 24-May-14 23:18 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-14 23:18 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-14 23:18 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-14 23:18 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27336 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-14 23:18 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     4004 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-14 23:18 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-14 23:18 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-14 23:18 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-14 23:18 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-14 23:18 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-14 23:18 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-14 23:18 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9249 b- defN 24-May-14 23:18 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-14 23:18 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-14 23:18 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-14 23:18 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-14 23:18 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-14 23:18 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-14 23:18 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-14 23:18 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-14 23:18 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-14 23:18 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-14 23:18 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-14 23:18 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-14 23:18 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-14 23:18 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13940 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-14 23:18 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-14 23:18 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-14 23:18 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-14 23:18 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-14 23:18 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-14 23:18 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-14 23:18 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-14 23:18 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-14 23:18 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-14 23:18 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-14 23:18 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-14 23:18 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-14 23:18 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-14 23:18 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-14 23:18 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-14 23:18 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-14 23:18 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-14 23:18 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9486 b- defN 24-May-14 23:18 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-14 23:18 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8810 b- defN 24-May-14 23:18 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-14 23:18 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-14 23:18 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-14 23:18 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18337 b- defN 24-May-14 23:18 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-14 23:18 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-14 23:18 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-14 23:18 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4066 b- defN 24-May-14 23:18 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-14 23:18 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-14 23:18 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-14 23:18 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-14 23:18 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-14 23:18 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-14 23:18 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-14 23:18 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-14 23:18 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-14 23:18 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-14 23:18 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-14 23:18 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-14 23:18 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-14 23:18 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-14 23:18 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-14 23:18 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-14 23:18 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-14 23:18 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-14 23:18 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-14 23:18 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-14 23:18 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-14 23:18 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-14 23:18 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-14 23:18 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-14 23:18 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-14 23:18 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-14 23:18 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-14 23:18 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-14 23:18 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-14 23:18 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-14 23:18 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-14 23:18 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-14 23:18 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-14 23:18 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5415 b- defN 24-May-14 23:18 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-14 23:18 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-14 23:18 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-14 23:18 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-14 23:18 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-14 23:18 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-14 23:18 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-14 23:18 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1587 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-14 23:18 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-14 23:18 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-14 23:18 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-14 23:18 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-14 23:18 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-14 23:18 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-14 23:18 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-14 23:18 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-14 23:18 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-14 23:18 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-14 23:18 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-14 23:18 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-14 23:18 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-14 23:18 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-14 23:18 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-14 23:18 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-14 23:18 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-14 23:18 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-14 23:18 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3093 b- defN 24-May-14 23:18 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-14 23:18 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-14 23:18 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-14 23:18 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-14 23:18 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-14 23:18 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-14 23:18 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-14 23:18 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-14 23:18 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-14 23:18 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-14 23:18 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-14 23:18 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-14 23:18 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-14 23:18 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-14 23:18 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-14 23:18 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-14 23:18 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-14 23:18 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-14 23:18 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-14 23:18 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-14 23:18 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-14 23:18 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-14 23:18 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-14 23:18 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-14 23:18 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-14 23:18 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-14 23:18 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-14 23:18 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-14 23:18 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-14 23:18 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-14 23:18 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-14 23:18 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-14 23:18 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-14 23:18 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-14 23:18 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-14 23:18 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-14 23:18 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-14 23:18 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-14 23:18 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-14 23:18 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-14 23:18 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-14 23:18 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-14 23:18 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-14 23:18 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-14 23:18 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-14 23:18 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-14 23:18 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-14 23:18 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-14 23:18 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-14 23:18 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-14 23:18 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-14 23:18 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-14 23:18 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-14 23:18 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-14 23:18 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-14 23:18 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-14 23:18 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-14 23:18 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-14 23:18 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-14 23:18 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-14 23:18 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-May-14 23:18 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-14 23:18 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-14 23:18 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-14 23:18 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-14 23:18 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-14 23:18 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-14 23:18 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-14 23:18 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10747 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-14 23:18 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-14 23:18 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-14 23:18 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-14 23:18 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-14 23:18 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-14 23:18 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-14 23:18 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-14 23:18 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-14 23:18 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-14 23:18 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-14 23:18 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-14 23:18 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-14 23:18 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-14 23:18 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-14 23:18 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-14 23:18 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-14 23:18 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-14 23:18 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-14 23:18 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-14 23:18 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-14 23:18 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-14 23:18 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43144 b- defN 24-May-14 23:19 nucliadb-3.1.0.post501.dist-info/RECORD
+460 files, 2259339 bytes uncompressed, 694345 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -618,14 +618,17 @@
 
 Filename: nucliadb/search/api/__init__.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/__init__.py
 Comment: 
 
+Filename: nucliadb/search/api/v1/ask.py
+Comment: 
+
 Filename: nucliadb/search/api/v1/chat.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/feedback.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/find.py
@@ -651,14 +654,17 @@
 
 Filename: nucliadb/search/api/v1/utils.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/resource/__init__.py
 Comment: 
 
+Filename: nucliadb/search/api/v1/resource/ask.py
+Comment: 
+
 Filename: nucliadb/search/api/v1/resource/chat.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/resource/search.py
 Comment: 
 
 Filename: nucliadb/search/requesters/__init__.py
@@ -711,14 +717,17 @@
 
 Filename: nucliadb/search/search/utils.py
 Comment: 
 
 Filename: nucliadb/search/search/chat/__init__.py
 Comment: 
 
+Filename: nucliadb/search/search/chat/ask.py
+Comment: 
+
 Filename: nucliadb/search/search/chat/images.py
 Comment: 
 
 Filename: nucliadb/search/search/chat/prompt.py
 Comment: 
 
 Filename: nucliadb/search/search/chat/query.py
@@ -756,14 +765,17 @@
 
 Filename: nucliadb/search/tests/unit/api/__init__.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/api/v1/__init__.py
 Comment: 
 
+Filename: nucliadb/search/tests/unit/api/v1/test_ask.py
+Comment: 
+
 Filename: nucliadb/search/tests/unit/api/v1/test_chat.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/api/v1/test_summarize.py
@@ -1344,26 +1356,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/METADATA
+Filename: nucliadb-3.1.0.post501.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/WHEEL
+Filename: nucliadb-3.1.0.post501.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/entry_points.txt
+Filename: nucliadb-3.1.0.post501.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/top_level.txt
+Filename: nucliadb-3.1.0.post501.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/zip-safe
+Filename: nucliadb-3.1.0.post501.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.1.0.post500.dist-info/RECORD
+Filename: nucliadb-3.1.0.post501.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/ingest/orm/brain.py

```diff
@@ -371,14 +371,15 @@
         sentence_pb.metadata.representation.is_a_table = (
             paragraph_pb.metadata.representation.is_a_table
         )
 
         sentence_pb.metadata.position.index = paragraph_pb.metadata.position.index
 
     def delete_vectors(self, field_key: str, vo: VectorObject):
+        # TODO: no need to iterate over all vectors, just delete the whole field
         for subfield, vectors in vo.split_vectors.items():
             for vector in vectors.vectors:
                 self.brain.sentences_to_delete.append(
                     f"{self.rid}/{field_key}/{subfield}/{vector.start}-{vector.end}"
                 )
 
         for vector in vo.vectors.vectors:
```

## nucliadb/search/predict.py

```diff
@@ -16,20 +16,21 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import json
 import os
 from enum import Enum
-from typing import AsyncIterator, Optional
+from typing import Any, AsyncIterator, Literal, Optional, Union
 from unittest.mock import AsyncMock, Mock
 
 import aiohttp
 import backoff
 from nucliadb_protos.utils_pb2 import RelationNode
+from pydantic import BaseModel, Field, ValidationError
 
 from nucliadb.ingest.tests.vectors import Q, Qm2023
 from nucliadb.search import logger
 from nucliadb_models.search import (
     ChatModel,
     FeedbackRequest,
     Ner,
@@ -37,15 +38,15 @@
     RephraseModel,
     SentenceSearch,
     SummarizedResource,
     SummarizedResponse,
     SummarizeModel,
     TokenSearch,
 )
-from nucliadb_telemetry import metrics
+from nucliadb_telemetry import errors, metrics
 from nucliadb_utils import const
 from nucliadb_utils.exceptions import LimitsExceededError
 from nucliadb_utils.settings import nuclia_settings
 from nucliadb_utils.utilities import Utility, has_feature, set_utility
 
 
 class SendToPredictError(Exception):
@@ -110,14 +111,56 @@
 
 
 class AnswerStatusCode(str, Enum):
     SUCCESS = "0"
     ERROR = "-1"
     NO_CONTEXT = "-2"
 
+    def prettify(self) -> str:
+        return {
+            AnswerStatusCode.SUCCESS: "success",
+            AnswerStatusCode.ERROR: "error",
+            AnswerStatusCode.NO_CONTEXT: "no_context",
+        }[self]
+
+
+class TextGenerativeResponse(BaseModel):
+    type: Literal["text"] = "text"
+    text: str
+
+
+class MetaGenerativeResponse(BaseModel):
+    type: Literal["meta"] = "meta"
+    input_tokens: int
+    output_tokens: int
+    timings: dict[str, float]
+
+
+class CitationsGenerativeResponse(BaseModel):
+    type: Literal["citations"] = "citations"
+    citations: dict[str, Any]
+
+
+class StatusGenerativeResponse(BaseModel):
+    type: Literal["status"] = "status"
+    code: str
+    details: Optional[str] = None
+
+
+GenerativeResponse = Union[
+    TextGenerativeResponse,
+    MetaGenerativeResponse,
+    CitationsGenerativeResponse,
+    StatusGenerativeResponse,
+]
+
+
+class GenerativeChunk(BaseModel):
+    chunk: GenerativeResponse = Field(..., discriminator="type")
+
 
 async def start_predict_engine():
     if nuclia_settings.dummy_predict:
         predict_util = DummyPredictEngine()
     else:
         predict_util = PredictEngine(
             nuclia_settings.nuclia_inner_predict_url,
@@ -300,14 +343,44 @@
             headers=self.get_predict_headers(kbid),
             timeout=None,
         )
         await self.check_response(resp, expected_status=200)
         ident = resp.headers.get(NUCLIA_LEARNING_ID_HEADER)
         return ident, get_answer_generator(resp)
 
+    @predict_observer.wrap({"type": "chat_ndjson"})
+    async def chat_query_ndjson(
+        self, kbid: str, item: ChatModel
+    ) -> tuple[str, AsyncIterator[GenerativeChunk]]:
+        """
+        Chat query using the new stream format
+        Format specs: https://github.com/ndjson/ndjson-spec
+        """
+        try:
+            self.check_nua_key_is_configured_for_onprem()
+        except NUAKeyMissingError:
+            error = "Nuclia Service account is not defined so the chat operation could not be performed"
+            logger.warning(error)
+            raise SendToPredictError(error)
+
+        # The ndjson format is triggered by the Accept header
+        headers = self.get_predict_headers(kbid)
+        headers["Accept"] = "application/x-ndjson"
+
+        resp = await self.make_request(
+            "POST",
+            url=self.get_predict_url(CHAT, kbid),
+            json=item.dict(),
+            headers=headers,
+            timeout=None,
+        )
+        await self.check_response(resp, expected_status=200)
+        ident = resp.headers.get(NUCLIA_LEARNING_ID_HEADER)
+        return ident, get_chat_ndjson_generator(resp)
+
     @predict_observer.wrap({"type": "query"})
     async def query(
         self,
         kbid: str,
         sentence: str,
         generative_model: Optional[str] = None,
         rephrase: Optional[bool] = False,
@@ -386,14 +459,20 @@
         self.calls = []
         self.generated_answer = [
             b"valid ",
             b"answer ",
             b" to",
             AnswerStatusCode.SUCCESS.encode(),
         ]
+        self.ndjson_answer = [
+            b'{"chunk": {"type": "text", "text": "valid "}}\n',
+            b'{"chunk": {"type": "text", "text": "answer "}}\n',
+            b'{"chunk": {"type": "text", "text": "to"}}\n',
+            b'{"chunk": {"type": "status", "code": "0"}}\n',
+        ]
         self.max_context = 1000
 
     async def initialize(self):
         pass
 
     async def finalize(self):
         pass
@@ -429,14 +508,25 @@
 
         async def generate():
             for i in self.generated_answer:
                 yield i
 
         return (DUMMY_LEARNING_ID, generate())
 
+    async def chat_query_ndjson(
+        self, kbid: str, item: ChatModel
+    ) -> tuple[str, AsyncIterator[bytes]]:
+        self.calls.append(("chat_query_ndjson", item))
+
+        async def generate():
+            for item in self.ndjson_answer:
+                yield GenerativeChunk.parse_raw(item)
+
+        return (DUMMY_LEARNING_ID, generate())
+
     async def query(
         self,
         kbid: str,
         sentence: str,
         generative_model: Optional[str] = None,
         rephrase: Optional[bool] = False,
     ) -> QueryInfo:
@@ -507,14 +597,30 @@
             if end_of_chunk:
                 yield buffer
                 buffer = b""
 
     return _iter_answer_chunks(response.content.iter_chunks())
 
 
+def get_chat_ndjson_generator(
+    response: aiohttp.ClientResponse,
+) -> AsyncIterator[GenerativeChunk]:
+
+    async def _parse_generative_chunks(gen):
+        async for chunk in gen:
+            try:
+                yield GenerativeChunk.parse_raw(chunk.strip())
+            except ValidationError as ex:
+                errors.capture_exception(ex)
+                logger.error(f"Invalid chunk received: {chunk}")
+                continue
+
+    return _parse_generative_chunks(response.content)
+
+
 async def _parse_rephrase_response(
     resp: aiohttp.ClientResponse,
 ) -> str:
     """
     Predict api is returning a json payload that is a string with the following format:
     <rephrased_query><status_code>
     where status_code is "0" for success, "-1" for error and "-2" for no context
```

## nucliadb/search/api/v1/__init__.py

```diff
@@ -13,18 +13,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
+from . import ask  # noqa
 from . import chat  # noqa
 from . import feedback  # noqa
 from . import find  # noqa
 from . import knowledgebox  # noqa
 from . import predict_proxy  # noqa
 from . import search  # noqa
 from . import suggest  # noqa
 from . import summarize  # noqa
+from .resource import ask as ask_resource  # noqa
 from .resource import chat as chat_resource  # noqa
 from .resource import search as search_resource  # noqa
 from .router import api  # noqa
```

## nucliadb/search/api/v1/chat.py

```diff
@@ -42,19 +42,19 @@
     InvalidQueryError,
 )
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.search import (
     ChatOptions,
     ChatRequest,
     KnowledgeboxFindResults,
-    MaxTokens,
     NucliaDBClientType,
     PromptContext,
     PromptContextOrder,
     Relations,
+    parse_max_tokens,
 )
 from nucliadb_telemetry.errors import capture_exception
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.exceptions import LimitsExceededError
 
 END_OF_STREAM = "_END_"
 
@@ -173,15 +173,15 @@
             streamed_answer, chat_request.citations
         )
 
         relations_results = None
         if ChatOptions.RELATIONS in chat_request.features:
             # XXX should use query parser here
             relations_results = await get_relations_results(
-                kbid=kbid, chat_request=chat_request, text_answer=answer
+                kbid=kbid, text_answer=answer, target_shard_replicas=chat_request.shards
             )
 
         sync_chat_resp = SyncChatResponse(
             answer=answer,
             relations=relations_results,
             results=chat_result.find_results,
             status=chat_result.status_code.value,
@@ -212,15 +212,17 @@
 
             answer, _ = parse_streamed_answer(streamed_answer, chat_request.citations)
 
             yield END_OF_STREAM.encode()
             if ChatOptions.RELATIONS in chat_request.features:
                 # XXX should use query parser here
                 relations_results = await get_relations_results(
-                    kbid=kbid, chat_request=chat_request, text_answer=answer
+                    kbid=kbid,
+                    text_answer=answer,
+                    target_shard_replicas=chat_request.shards,
                 )
                 yield base64.b64encode(relations_results.json().encode())
 
         return StreamingResponse(
             _streaming_response(),
             media_type="application/octet-stream",
             headers={
@@ -255,18 +257,7 @@
         return text_answer.decode("utf-8"), citations
     except Exception as exc:
         capture_exception(exc)
         logger.exception(
             "Error parsing citations. Returning the answer without citations."
         )
         return text_answer.decode("utf-8"), {}
-
-
-def parse_max_tokens(
-    max_tokens: Optional[Union[int, MaxTokens]]
-) -> Optional[MaxTokens]:
-    if isinstance(max_tokens, int):
-        # If the max_tokens is an integer, it is interpreted as the max_tokens value for the generated answer.
-        # The max tokens for the context is set to None to use the default value for the model (comes in the
-        # NUA's query endpoint response).
-        return MaxTokens(answer=max_tokens, context=None)
-    return max_tokens
```

## nucliadb/search/search/chat/query.py

```diff
@@ -176,15 +176,15 @@
     )
     if incomplete:
         raise IncompleteFindResultsError()
     return find_results, query_parser
 
 
 async def get_relations_results(
-    *, kbid: str, chat_request: ChatRequest, text_answer: str
+    *, kbid: str, text_answer: str, target_shard_replicas: Optional[list[str]]
 ) -> Relations:
     try:
         predict = get_predict()
         detected_entities = await predict.detect_entities(kbid, text_answer)
         relation_request = RelationSearchRequest()
         relation_request.subgraph.entry_points.extend(detected_entities)
         relation_request.subgraph.depth = 1
@@ -194,15 +194,15 @@
             relations_results,
             _,
             _,
         ) = await node_query(
             kbid,
             Method.RELATIONS,
             relation_request,
-            target_shard_replicas=chat_request.shards,
+            target_shard_replicas=target_shard_replicas,
         )
         return await merge_relations_results(
             relations_results, relation_request.subgraph
         )
     except Exception as exc:
         capture_exception(exc)
         logger.exception("Error getting relations results")
@@ -341,14 +341,15 @@
             duration=time() - start_time,
             user_query=user_query,
             rephrased_query=rephrased_query,
             text_answer=text_answer,
             status_code=status_code.value,
             chat_history=chat_history,
             query_context=prompt_context,
+            query_context_order=prompt_context_order,
             learning_id=nuclia_learning_id,
         )
 
     answer_stream = _wrapped_stream()
     return ChatResult(
         nuclia_learning_id=nuclia_learning_id,
         answer_stream=answer_stream,
@@ -389,32 +390,34 @@
     origin: str,
     duration: float,
     user_query: str,
     rephrased_query: Optional[str],
     text_answer: bytes,
     status_code: Optional[AnswerStatusCode],
     chat_history: list[ChatContextMessage],
-    query_context: list[str],
+    query_context: PromptContext,
+    query_context_order: PromptContextOrder,
     learning_id: str,
 ):
     audit = get_audit()
     if audit is None:
         return
 
     audit_answer = parse_audit_answer(text_answer, status_code)
 
     # Append chat history and query context
     audit_context = [
         audit_pb2.ChatContext(author=message.author, text=message.text)
         for message in chat_history
     ]
+    query_context_paragaph_ids = list(query_context.keys())
     audit_context.append(
         audit_pb2.ChatContext(
             author=Author.NUCLIA,
-            text=AUDIT_TEXT_RESULT_SEP.join(query_context),
+            text=AUDIT_TEXT_RESULT_SEP.join(query_context_paragaph_ids),
         )
     )
     await audit.chat(
         kbid,
         user_id,
         client_type.to_proto(),
         origin,
@@ -442,7 +445,67 @@
     return audit_answer
 
 
 def tokens_to_chars(n_tokens: int) -> int:
     # Multiply by 3 to have a good margin and guess between characters and tokens.
     # This will be properly cut at the NUA predict API.
     return n_tokens * 3
+
+
+class ChatAuditor:
+    def __init__(
+        self,
+        kbid: str,
+        user_id: str,
+        client_type: NucliaDBClientType,
+        origin: str,
+        start_time: float,
+        user_query: str,
+        rephrased_query: Optional[str],
+        chat_history: list[ChatContextMessage],
+        learning_id: Optional[str],
+        query_context: PromptContext,
+        query_context_order: PromptContextOrder,
+    ):
+        self.kbid = kbid
+        self.user_id = user_id
+        self.client_type = client_type
+        self.origin = origin
+        self.start_time = start_time
+        self.user_query = user_query
+        self.rephrased_query = rephrased_query
+        self.chat_history = chat_history
+        self.learning_id = learning_id
+        self.query_context = query_context
+        self.query_context_order = query_context_order
+
+    async def audit(self, text_answer: bytes, status_code: AnswerStatusCode):
+        await maybe_audit_chat(
+            kbid=self.kbid,
+            user_id=self.user_id,
+            client_type=self.client_type,
+            origin=self.origin,
+            duration=time() - self.start_time,
+            user_query=self.user_query,
+            rephrased_query=self.rephrased_query,
+            text_answer=text_answer,
+            status_code=status_code,
+            chat_history=self.chat_history,
+            query_context=self.query_context,
+            query_context_order=self.query_context_order,
+            learning_id=self.learning_id or "unknown",
+        )
+
+
+def sorted_prompt_context_list(
+    context: PromptContext, order: PromptContextOrder
+) -> list[str]:
+    """
+    context = {"x": "foo", "y": "bar"}
+    order = {"y": 1, "x": 0}
+    sorted_prompt_context_list(context, order) == ["foo", "bar"]
+    """
+    sorted_items = sorted(
+        context.items(),
+        key=lambda item: order.get(item[0], float("inf")),
+    )
+    return list(map(lambda item: item[1], sorted_items))
```

## nucliadb/search/tests/unit/test_predict.py

```diff
@@ -14,29 +14,36 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import asyncio
+from unittest import mock
 from unittest.mock import AsyncMock, MagicMock, Mock
 
 import aiohttp
 import pytest
 from yarl import URL
 
 from nucliadb.search.predict import (
+    CitationsGenerativeResponse,
     DummyPredictEngine,
+    GenerativeChunk,
+    MetaGenerativeResponse,
     PredictEngine,
     ProxiedPredictAPIError,
     RephraseError,
     RephraseMissingContextError,
     SendToPredictError,
+    StatusGenerativeResponse,
+    TextGenerativeResponse,
     _parse_rephrase_response,
     get_answer_generator,
+    get_chat_ndjson_generator,
 )
 from nucliadb.tests.utils.aiohttp_session import get_mocked_session
 from nucliadb_models.search import (
     ChatModel,
     FeedbackRequest,
     FeedbackTasks,
     RephraseModel,
@@ -442,7 +449,77 @@
 
     resp = Mock()
     resp.content.iter_chunks = Mock(return_value=_iter_chunks())
     get_answer_generator(resp)
 
     answer_chunks = [chunk async for chunk in get_answer_generator(resp)]
     assert answer_chunks == [b"foobar", b"baz"]
+
+
+async def test_get_chat_ndjson_generator():
+    streamed_elements = [
+        TextGenerativeResponse(text="foo"),
+        MetaGenerativeResponse(input_tokens=1, output_tokens=1, timings={"foo": 1}),
+        CitationsGenerativeResponse(citations={"foo": "bar"}),
+        StatusGenerativeResponse(code="-1", details="foo"),
+    ]
+
+    async def _content():
+        for element in streamed_elements:
+            gen_chunk = GenerativeChunk(chunk=element)
+            yield gen_chunk.json() + "\n"
+        # yield an unknown chunk, to make sure it is ignored
+        yield '{"unknown": "chunk"}\n'
+
+    response = mock.Mock()
+    response.content = _content()
+
+    gen = get_chat_ndjson_generator(response)
+
+    parsed = [line async for line in gen]
+    assert len(parsed) == 4
+    assert parsed[0].chunk == TextGenerativeResponse(text="foo")
+    assert parsed[1].chunk == MetaGenerativeResponse(
+        input_tokens=1, output_tokens=1, timings={"foo": 1}
+    )
+    assert parsed[2].chunk == CitationsGenerativeResponse(citations={"foo": "bar"})
+    assert parsed[3].chunk == StatusGenerativeResponse(code="-1", details="foo")
+
+
+async def test_chat_query_ndjson():
+    pe = PredictEngine(
+        "cluster",
+        "public-{zone}",
+        zone="europe1",
+        onprem=False,
+    )
+    streamed_elements = [
+        TextGenerativeResponse(text="foo"),
+        StatusGenerativeResponse(code="-1", details="foo"),
+    ]
+
+    async def _content():
+        for element in streamed_elements:
+            gen_chunk = GenerativeChunk(chunk=element)
+            yield gen_chunk.json() + "\n"
+
+    chat_query_response = Mock()
+    chat_query_response.status = 200
+    chat_query_response.headers = {"NUCLIA-LEARNING-ID": "learning-id"}
+    chat_query_response.content = _content()
+    pe.session = mock.Mock()
+    pe.session.post = AsyncMock(return_value=chat_query_response)
+
+    item = ChatModel(question="foo", user_id="bar")
+
+    learning_id, generator = await pe.chat_query_ndjson("kbid", item)
+
+    assert learning_id == "learning-id"
+    parsed = [line async for line in generator]
+    assert len(parsed) == 2
+    assert parsed[0].chunk == TextGenerativeResponse(text="foo")
+    assert parsed[1].chunk == StatusGenerativeResponse(code="-1", details="foo")
+
+    # Make sure the request was made with the correct headers
+    pe.session.post.call_args_list[0].kwargs["headers"][
+        "Accept"
+    ] == "application/ndjson"
```

## Comparing `nucliadb-3.1.0.post500.dist-info/METADATA` & `nucliadb-3.1.0.post501.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.1.0.post500
+Version: 3.1.0.post501
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post500
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post500
-Requires-Dist: nucliadb-protos >=3.1.0.post500
-Requires-Dist: nucliadb-models >=3.1.0.post500
+Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post501
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post501
+Requires-Dist: nucliadb-protos >=3.1.0.post501
+Requires-Dist: nucliadb-models >=3.1.0.post501
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.1.0.post500.dist-info/entry_points.txt` & `nucliadb-3.1.0.post501.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.1.0.post500.dist-info/RECORD` & `nucliadb-3.1.0.post501.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 nucliadb/ingest/fields/file.py,sha256=RtLlnDuT3bueO7V0gnm_i_P1lUCG9l6CZFky0fFCCgg,5159
 nucliadb/ingest/fields/generic.py,sha256=elgtqv15aJUq3zY7X_g0bli_2BpcwPArVvzhe54Y4Ig,1547
 nucliadb/ingest/fields/keywordset.py,sha256=mLpitqGiSH3IilHCEo2ZGg3laTOMoZ5qc_DVbV3UECA,1235
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=SUVp5MqMW9LN4Wx7vB23SsSAmEAn8eug4qdPnkdxEyM,4531
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/orm/brain.py,sha256=Hq8c0TpHlJ2rT5oig3QX3xmSQZiB8YFURws5xj3-iuk,28367
+nucliadb/ingest/orm/brain.py,sha256=VeOdXmlqYVWQnB4iL934d1QI2t7__KWz8gcfP4QSnTQ,28448
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
 nucliadb/ingest/orm/knowledgebox.py,sha256=urKMAL8Rj0Unen5AZ4Au-Z-176Vk1mOiXTUF4PnqMMs,17167
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=gmmVw8tkAcH8oYQdfuxSrRhD8KZ4mh0oPs3SML2RGtY,60444
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
@@ -196,31 +196,33 @@
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
 nucliadb/search/__init__.py,sha256=fwzdF6p7p9uDCtE38gTUxrRVIdbEDVQTAXWUMVKgSBM,1535
 nucliadb/search/app.py,sha256=azMj8BiaFr03pYQKcWSr2YqjB0FopJDeVKE2wwuj6pU,4905
 nucliadb/search/lifecycle.py,sha256=s6If2a78dcv4_71d-Q_uA6b9TaJCQOASUhqa2HcxfIw,1956
 nucliadb/search/openapi.py,sha256=t3Wo_4baTrfPftg2BHsyLWNZ1MYn7ZRdW7ht-wFOgRs,1016
-nucliadb/search/predict.py,sha256=SOzMErnplx-jDTdKya1hr4LKbQt956THyzN_vVc1iiY,17332
+nucliadb/search/predict.py,sha256=F-EuRp00Q2wb5Ut1srXeomoY_JW_y-LEB0aKPU8Cf-Y,20665
 nucliadb/search/run.py,sha256=aFb-CXRi_C8YMpP_ivNj8KW1BYhADj88y8K9Lr_nUPI,1402
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/api/v1/__init__.py,sha256=tusthakDVkeiAgU-eNjLsO183KXs8Js3fdPAF3JTXP0,1222
-nucliadb/search/api/v1/chat.py,sha256=6rFou6kpEPiRBw0DTpDkrud8tYhpyfrOiAifmETSzp8,9882
+nucliadb/search/api/v1/__init__.py,sha256=FR4pbt1XyWQAS3TAiAhvOQb0kWSsZpmzL87JJMcAoMc,1298
+nucliadb/search/api/v1/ask.py,sha256=JRHdcMnOOSfB6nWY2TnVes0FXriumbT30_wI1IbfCyE,3534
+nucliadb/search/api/v1/chat.py,sha256=y1z74bwwypb1FFaQrDegFXTixe-9W44-1PXjlqQYvPM,9486
 nucliadb/search/api/v1/feedback.py,sha256=SFXKzqgn31TDudUYPmp8845EBwLSJtWImG-7tTc9WQM,2668
 nucliadb/search/api/v1/find.py,sha256=oHfavVeX56ipsEiTUNVyBoFu-E5-dWwP_iyaHaUqz5c,8810
 nucliadb/search/api/v1/knowledgebox.py,sha256=hQ0wdBlHJVTwiRZgVCeNVwW_6f2bay88Hs9JMHgnx9M,6938
 nucliadb/search/api/v1/predict_proxy.py,sha256=QrGzo0hKjtmyGZ6pjlJHYAh4hxwVUIOTcVcerRCw7eE,3047
 nucliadb/search/api/v1/router.py,sha256=mtT07rBZcVfpa49doaw9b1tj3sdi3qLH0gn9Io6NYM0,988
 nucliadb/search/api/v1/search.py,sha256=GbCmp_WzG-wA8oVZkXGo9TwVLOHDBE2rhPWptHplje4,18337
 nucliadb/search/api/v1/suggest.py,sha256=3Mz34gxxTtyWG45CpfXQFJ54WS7cHUVwwz7oAtmtM28,5970
 nucliadb/search/api/v1/summarize.py,sha256=VAHJvE6V3xUgEBfqNKhgoxmDqCvh30RnrEIBVhMcNLU,2499
 nucliadb/search/api/v1/utils.py,sha256=5Ve-frn7LAE2jqAgB85F8RSeqxDlyA08--gS-AdOLS4,1434
 nucliadb/search/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
+nucliadb/search/api/v1/resource/ask.py,sha256=sKf9gdpMabwjXaMoi22b1iFoILshLiqclrM6tjz8SVs,4066
 nucliadb/search/api/v1/resource/chat.py,sha256=OaU3_yivCtdF2QLosGOiCngyzp4v4cCmbSMzCDxSpog,5821
 nucliadb/search/api/v1/resource/search.py,sha256=C6Do2x0dq0lUyUg67hFYxHMJ8xtaAtJj5yPnmrGTONo,5303
 nucliadb/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/requesters/utils.py,sha256=P2OIPXs9klQ-Nnu7TjS3rVEp91Q3dCtf92mQa2StXdw,9111
 nucliadb/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/cache.py,sha256=86WwnknDYI00bd-kFf5MhN8TVFS2tfHzgobUHv_fAIA,2746
 nucliadb/search/search/exceptions.py,sha256=mbToQ-ghrv8ukLEv8S_-EZrgweWaIZZ5SIpoeuGDk6s,1154
@@ -233,29 +235,31 @@
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
 nucliadb/search/search/query.py,sha256=cq6BFwnLdfAfrcGhJfW3DNlVvY1Vk7JGoO2TVFgJ8sU,31127
 nucliadb/search/search/shards.py,sha256=0p_BWLEVrK87htqhavZ2ixA2l253FPQnre3RpThtZco,3018
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
+nucliadb/search/search/chat/ask.py,sha256=4yLOqeIJDKt5zVl78knppDqfgeMqZjRUEIiEbQxfDkM,16676
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
-nucliadb/search/search/chat/query.py,sha256=6NKMtilwo6CUcjchf6u9Z8ieCaDTK8gD3MWAAQ_b9JE,15401
+nucliadb/search/search/chat/query.py,sha256=_ZwdkNCbT77NQyrVVEi3J_sabiP6KB2YK-C3CNyKF9k,17543
 nucliadb/search/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/conftest.py,sha256=BhVEPbrIm7GKDHtnS7tc7WqCRReIL4MzzTjLQUWrLJY,1295
 nucliadb/search/tests/fixtures.py,sha256=a0q-mh15uvr97ebGTStcdONWx4AQ8rdkH772azMwMMg,6578
 nucliadb/search/tests/node.py,sha256=QInxf97DUUi-afzBPZDboCH8D-E02A3R-XFwFpUrvCc,15480
 nucliadb/search/tests/unit/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/test_app.py,sha256=3wr6_DTLdwhpk7Sske7EEqmGbaJSG4OH9Olw_KVszPw,2649
 nucliadb/search/tests/unit/test_find_merge.py,sha256=z_qLcXG8qdUegGkaEloG7wXXwoZyppeOnzUCcHAVq3w,3374
 nucliadb/search/tests/unit/test_merge.py,sha256=1uCdn3MZbUWs2WKFGJSJZgpm4xTtn5nvgurbo37l5B8,1400
-nucliadb/search/tests/unit/test_predict.py,sha256=QRM2KhJtsaWUOzXv36LQ5hazuN9ViFsmvrgwdGZI3_I,13101
+nucliadb/search/tests/unit/test_predict.py,sha256=5m_J0k3ESL4A1HPw-qoru9p6IAqJnaKgJInCS8t4UMU,15721
 nucliadb/search/tests/unit/test_run.py,sha256=ui8Ucm_mDpCcewm2xiGT9GFG2XtNezrRnnSpaNuBmjk,1328
 nucliadb/search/tests/unit/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
+nucliadb/search/tests/unit/api/v1/test_ask.py,sha256=uMIX-hrZZKaH0mtSVlGIz9osknQtQorOx_xxeO4RABs,3759
 nucliadb/search/tests/unit/api/v1/test_chat.py,sha256=Ud6MDM7gLUV6PZQeCDA5vBcJ40Sf4fqNeWBwYWUOi-E,2966
 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py,sha256=CuouBrldS3mpBZe3FlpkaW3R_cI8Db8o6bSFPW0ifmA,2865
 nucliadb/search/tests/unit/api/v1/test_summarize.py,sha256=4VQm-fegHLeBNBoNuoKbKM5FiqAML9m9QT7XNY3n2n4,2901
 nucliadb/search/tests/unit/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/resource/test_chat.py,sha256=p91CJTfjmPfVpMt6B1Rzee2yK1Dy4vNQeXgqxTXRWCk,3040
 nucliadb/search/tests/unit/search/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/search/test_chat_prompt.py,sha256=FKjGgBpTFmpvB2BUdHhriWWKSznBoYV1K5IHD5YOqU8,8586
@@ -444,13 +448,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.1.0.post500.dist-info/METADATA,sha256=8M4IXDAkD-5m0Ul7Qsg7IJRWn16zZl1l1f9AwIGcDbs,4399
-nucliadb-3.1.0.post500.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.1.0.post500.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.1.0.post500.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.1.0.post500.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.1.0.post500.dist-info/RECORD,,
+nucliadb-3.1.0.post501.dist-info/METADATA,sha256=7q__eHrSbOYrBu-8pXvMZrHfvusOh_xcldvc5wFJnIw,4399
+nucliadb-3.1.0.post501.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.1.0.post501.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.1.0.post501.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.1.0.post501.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.1.0.post501.dist-info/RECORD,,
```

