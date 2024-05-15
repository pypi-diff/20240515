# Comparing `tmp/nfelib-2.0.5.zip` & `tmp/nfelib-2.0.6.zip`

## zipinfo {}

```diff
@@ -1,704 +1,704 @@
-Zip file size: 1367482 bytes, number of entries: 702
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/
--rw-rw-r--  2.0 unx     1074 b- defN 24-Apr-05 08:24 nfelib-2.0.5/MIT-LICENSE
--rw-rw-r--  2.0 unx       38 b- defN 24-Apr-05 08:24 nfelib-2.0.5/setup.py
--rw-rw-r--  2.0 unx     1493 b- defN 24-May-08 11:09 nfelib-2.0.5/setup.cfg
--rw-rw-r--  2.0 unx     7477 b- defN 24-May-08 10:59 nfelib-2.0.5/README.md
--rw-rw-r--  2.0 unx     8697 b- defN 24-May-08 11:09 nfelib-2.0.5/PKG-INFO
--rw-rw-r--  2.0 unx       64 b- defN 24-Apr-05 08:24 nfelib-2.0.5/MANIFEST.in
--rw-rw-r--  2.0 unx        7 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    30786 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      113 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     8697 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfse/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/mdfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfe_evento_cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cte/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfe/
--rwxrwxr-x  2.0 unx     2534 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/test_fingerprint.py
--rw-rw-r--  2.0 unx    11598 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse.xml
--rw-rw-r--  2.0 unx      632 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/__init__.py
--rw-rw-r--  2.0 unx     1507 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse_dps.xml
--rw-rw-r--  2.0 unx     4370 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_cte.xml
--rw-rw-r--  2.0 unx      453 b- defN 24-May-08 11:08 nfelib-2.0.5/tests/fingerprint.txt
--rw-rw-r--  2.0 unx     1230 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output.xml
--rw-rw-r--  2.0 unx     1207 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_evento_cce.xml
--rw-rw-r--  2.0 unx      224 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_mdfe.xml
--rw-rw-r--  2.0 unx      482 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_inut.xml
--rw-rw-r--  2.0 unx    46226 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_leiaute.xml
--rw-rw-r--  2.0 unx    41634 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/input.xml
--rw-rw-r--  2.0 unx     2549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/test_all.py
--rw-rw-r--  2.0 unx     2608 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfse/test_nfse.py
--rw-rw-r--  2.0 unx     1054 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/mdfe/test_mdfe.py
--rw-rw-r--  2.0 unx     1102 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py
--rw-rw-r--  2.0 unx     1049 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/cte/test_cte.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/v1_00/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/
--rw-rw-r--  2.0 unx     1128 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
--rw-rw-r--  2.0 unx       23 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe/__init__.py
--rw-rw-r--  2.0 unx     4504 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe/test_nfe_legacy.py
--rw-rw-r--  2.0 unx     8764 b- defN 24-Apr-08 21:49 nfelib-2.0.5/tests/nfe/test_nfe.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/v4_00/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/
--rw-rw-r--  2.0 unx     7673 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/samples/v1_0/
--rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
--rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
--rw-rw-r--  2.0 unx      728 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
--rw-rw-r--  2.0 unx    10940 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/bindings/__init__.py
--rw-rw-r--  2.0 unx      516 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
--rw-rw-r--  2.0 unx     5937 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx    36107 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
--rw-rw-r--  2.0 unx      496 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
--rw-rw-r--  2.0 unx   102239 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
--rw-rw-r--  2.0 unx      494 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/dps_v1_00.py
--rw-rw-r--  2.0 unx    16194 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
--rw-rw-r--  2.0 unx      498 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/evento_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/
--rw-rw-r--  2.0 unx    29312 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
--rw-rw-r--  2.0 unx      648 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
--rw-rw-r--  2.0 unx      752 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    78115 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
--rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
--rw-rw-r--  2.0 unx     3406 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
--rw-rw-r--  2.0 unx    57965 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
--rw-rw-r--  2.0 unx      743 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
--rw-rw-r--  2.0 unx    88685 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py
--rw-rw-r--  2.0 unx  1859480 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/__init__.py
--rw-rw-r--  2.0 unx      280 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/README.txt
--rw-rw-r--  2.0 unx   235328 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py
--rw-rw-r--  2.0 unx   231041 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py
--rw-rw-r--  2.0 unx     3387 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py
--rw-rw-r--  2.0 unx   188157 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retInutNFe.py
--rw-rw-r--  2.0 unx   159793 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsCad.py
--rw-rw-r--  2.0 unx    80047 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/distDFeInt.py
--rw-rw-r--  2.0 unx    79013 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py
--rw-rw-r--  2.0 unx  1859541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py
--rw-rw-r--  2.0 unx   239970 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py
--rw-rw-r--  2.0 unx   237200 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py
--rw-rw-r--  2.0 unx   289846 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/
--rw-rw-r--  2.0 unx      947 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
--rw-rw-r--  2.0 unx     1407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx     1816 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
--rw-rw-r--  2.0 unx     3789 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
--rw-rw-r--  2.0 unx     2719 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
--rw-rw-r--  2.0 unx     2057 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
--rw-rw-r--  2.0 unx     3574 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
--rw-rw-r--  2.0 unx      180 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
--rw-rw-r--  2.0 unx      702 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx      732 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx      739 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
--rw-rw-r--  2.0 unx      226 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/__init__.py
--rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     5571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     7084 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py
--rw-rw-r--  2.0 unx      545 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     6239 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     5995 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     7833 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx    11143 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1963 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      546 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      580 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx     5622 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      519 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      538 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    35874 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
--rw-rw-r--  2.0 unx    14799 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     1660 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    10218 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
--rw-rw-r--  2.0 unx      593 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     4353 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     5673 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
--rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx   126107 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      493 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
--rw-rw-r--  2.0 unx     2307 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3231 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
--rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/
--rw-rw-r--  2.0 unx     6549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
--rw-rw-r--  2.0 unx      620 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     1935 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4033 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      673 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    36487 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
--rw-rw-r--  2.0 unx     1564 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      592 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3479 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
--rw-rw-r--  2.0 unx     5523 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
--rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      632 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    10610 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      605 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
--rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      711 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    24229 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3958 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx    99783 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx    10365 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
--rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
--rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4559 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
--rw-rw-r--  2.0 unx     5554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx    10018 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      574 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      622 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     1967 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/__init__.py
--rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1670 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
--rw-rw-r--  2.0 unx    20302 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/
--rw-rw-r--  2.0 unx    15624 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx      598 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1767 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
--rw-rw-r--  2.0 unx     1269 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
--rw-rw-r--  2.0 unx     1755 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
--rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx     1253 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
--rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/
--rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/
--rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/__init__.py
--rw-rw-r--  2.0 unx     5466 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
--rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1010 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1811 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      578 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
--rw-rw-r--  2.0 unx      583 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
--rw-rw-r--  2.0 unx      550 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
--rw-rw-r--  2.0 unx    16741 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
--rw-rw-r--  2.0 unx      566 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/
--rw-rw-r--  2.0 unx      725 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     4651 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
--rw-rw-r--  2.0 unx     4459 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
--rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      601 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    11599 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      596 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    11613 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1774 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
--rw-rw-r--  2.0 unx      617 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    32624 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      634 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      745 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/__init__.py
--rw-rw-r--  2.0 unx     1435 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx    10677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
--rw-rw-r--  2.0 unx    37803 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/
--rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
--rw-rw-r--  2.0 unx     4475 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
--rw-rw-r--  2.0 unx      608 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx    17318 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1782 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      565 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx    17661 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx     5351 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/
--rw-rw-r--  2.0 unx      744 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      615 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      596 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     4424 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
--rw-rw-r--  2.0 unx    11920 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    12382 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      724 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    32624 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     2191 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
--rw-rw-r--  2.0 unx      634 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     4873 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1375 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     5501 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
--rw-rw-r--  2.0 unx     5290 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
--rw-rw-r--  2.0 unx     4141 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
--rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx     4407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     8230 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
--rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     4495 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
--rw-rw-r--  2.0 unx     4933 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/__init__.py
--rw-rw-r--  2.0 unx     1954 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
--rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1773 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx      551 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx    20018 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/
--rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    13952 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
--rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      589 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    32400 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1002 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     1067 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
--rw-rw-r--  2.0 unx     5420 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx     3407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     4283 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     8554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/__init__.py
--rw-rw-r--  2.0 unx     4651 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     4296 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     5551 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
--rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
--rw-rw-r--  2.0 unx      529 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx      539 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
--rw-rw-r--  2.0 unx      472 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
--rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
--rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
--rw-rw-r--  2.0 unx    13972 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx      497 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1915 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
--rw-rw-r--  2.0 unx      599 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1542 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2295 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
--rw-rw-r--  2.0 unx   131130 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/
--rw-rw-r--  2.0 unx      698 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      619 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
--rw-rw-r--  2.0 unx   107163 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx      594 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx    23114 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1411 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      649 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
--rw-rw-r--  2.0 unx     2028 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
--rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     9549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx     1668 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
--rw-rw-r--  2.0 unx      631 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1862 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
--rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx      678 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      582 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      563 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     4106 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     3279 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1028 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      352 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
--rw-rw-r--  2.0 unx      310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
--rw-rw-r--  2.0 unx     5453 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx    22419 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
--rw-rw-r--  2.0 unx     2843 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     4248 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     6807 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/
--rw-rw-r--  2.0 unx     1207 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/__init__.py
--rw-rw-r--  2.0 unx      514 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1705 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
--rw-rw-r--  2.0 unx    22394 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
--rw-rw-r--  2.0 unx     1850 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
--rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
--rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/
--rw-rw-r--  2.0 unx    17276 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
--rw-rw-r--  2.0 unx      657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
--rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     3340 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
--rw-rw-r--  2.0 unx      630 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     2035 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx      573 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx     4481 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
--rw-rw-r--  2.0 unx      557 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx    21825 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/
--rw-rw-r--  2.0 unx      609 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx     3942 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
--rw-rw-r--  2.0 unx    15700 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      618 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx    31796 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/samples/v4_0/
--rw-rw-r--  2.0 unx     3436 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
--rw-rw-r--  2.0 unx     1558 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
--rw-rw-r--  2.0 unx    10117 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
--rw-rw-r--  2.0 unx     3168 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
--rw-rw-r--  2.0 unx     4378 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/bindings/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/bindings/__init__.py
--rw-rw-r--  2.0 unx     1769 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
--rw-rw-r--  2.0 unx      594 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx     3786 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
--rw-rw-r--  2.0 unx     6898 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
--rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     5859 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     8883 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py
--rw-rw-r--  2.0 unx     2303 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
--rw-rw-r--  2.0 unx     5940 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
--rw-rw-r--  2.0 unx      564 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     2294 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
--rw-rw-r--  2.0 unx      534 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     1661 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
--rw-rw-r--  2.0 unx     4686 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
--rw-rw-r--  2.0 unx      478 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_v4_00.py
--rw-rw-r--  2.0 unx      574 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     6926 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
--rw-rw-r--  2.0 unx    18408 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     4334 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
--rw-rw-r--  2.0 unx     1540 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
--rw-rw-r--  2.0 unx      559 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
--rw-rw-r--  2.0 unx     7464 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
--rw-rw-r--  2.0 unx      529 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     8259 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
--rw-rw-r--  2.0 unx    11300 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
--rw-rw-r--  2.0 unx     1780 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
--rw-rw-r--  2.0 unx   424251 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      530 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
--rw-rw-r--  2.0 unx      503 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
--rw-rw-r--  2.0 unx      538 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     5479 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
--rw-rw-r--  2.0 unx      526 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
--rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx      537 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
--rw-rw-r--  2.0 unx     6178 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     1676 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
--rw-rw-r--  2.0 unx      561 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     1684 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
--rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
--rw-rw-r--  2.0 unx    14185 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     2313 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
--rw-rw-r--  2.0 unx      475 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/gtve_v4_00.py
--rw-rw-r--  2.0 unx      507 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
--rw-rw-r--  2.0 unx     8880 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
--rw-rw-r--  2.0 unx    10485 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
--rw-rw-r--  2.0 unx     1773 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/schemas/v4_0/
--rw-rw-r--  2.0 unx     4259 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
--rw-rw-r--  2.0 unx   332786 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx    10576 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
--rw-rw-r--  2.0 unx      700 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     8583 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
--rw-rw-r--  2.0 unx     6338 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      698 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     2213 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
--rw-rw-r--  2.0 unx      706 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
--rw-rw-r--  2.0 unx      702 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
--rw-rw-r--  2.0 unx      699 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     2075 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
--rw-rw-r--  2.0 unx     9313 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      677 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
--rw-rw-r--  2.0 unx     5494 b- defN 23-Mar-09 13:51 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1707 b- defN 23-Feb-27 09:00 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
--rw-rw-r--  2.0 unx      734 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4469 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx    11173 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
--rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
--rw-rw-r--  2.0 unx     6498 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     8005 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
--rw-rw-r--  2.0 unx     1348 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
--rw-rw-r--  2.0 unx    24294 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      651 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
--rw-rw-r--  2.0 unx     1648 b- defN 23-Mar-09 13:52 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
--rw-rw-r--  2.0 unx      834 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      800 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4690 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
--rw-rw-r--  2.0 unx      741 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx    13190 b- defN 23-Apr-28 08:26 nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      677 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
--rw-rw-r--  2.0 unx     4735 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1679 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
--rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      669 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     7868 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
--rw-rw-r--  2.0 unx      656 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
--rw-rw-r--  2.0 unx      695 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      720 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
--rw-rw-r--  2.0 unx     1668 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1516 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1346 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
--rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
--rw-rw-r--  2.0 unx      542 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
--rw-rw-r--  2.0 unx    19324 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/
--rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    14282 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      934 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1504 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py
--rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
--rw-rw-r--  2.0 unx    29843 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
--rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/
--rw-rw-r--  2.0 unx      655 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
--rw-rw-r--  2.0 unx    22200 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
--rw-rw-r--  2.0 unx    29554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      686 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/ws/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/
--rw-rw-r--  2.0 unx    10647 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
--rw-rw-r--  2.0 unx     7180 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
--rw-rw-r--  2.0 unx    37663 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
--rw-rw-r--  2.0 unx    14538 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
--rw-rw-r--  2.0 unx    32177 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
--rw-rw-r--  2.0 unx     9218 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
--rw-rw-r--  2.0 unx    68825 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
--rw-rw-r--  2.0 unx    10834 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
--rw-rw-r--  2.0 unx     9301 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
--rw-rw-r--  2.0 unx    12034 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
--rw-rw-r--  2.0 unx    11802 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
--rw-rw-r--  2.0 unx     9767 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
--rw-rw-r--  2.0 unx    46079 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
--rw-rw-r--  2.0 unx     5549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
--rw-rw-r--  2.0 unx    19459 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
--rw-rw-r--  2.0 unx    46216 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
--rw-rw-r--  2.0 unx      484 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/__init__.py
--rw-rw-r--  2.0 unx    30307 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      512 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     7598 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py
--rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      459 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
--rw-rw-r--  2.0 unx      567 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     2676 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      576 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx    16440 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
--rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx    13133 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      591 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     5962 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx      467 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
--rw-rw-r--  2.0 unx      533 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx   494616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
--rw-rw-r--  2.0 unx      558 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
--rw-rw-r--  2.0 unx       26 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/ws/__init__.py
--rw-rw-r--  2.0 unx     5164 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/
--rw-rw-r--  2.0 unx     3902 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx      628 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
--rw-rw-r--  2.0 unx    20000 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
--rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
--rw-rw-r--  2.0 unx      610 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
--rw-rw-r--  2.0 unx     7801 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx    15469 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
--rw-rw-r--  2.0 unx      617 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      568 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx    21976 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx   334026 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      604 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx    32310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx      602 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
-702 files, 10554408 bytes uncompressed, 1229836 bytes compressed:  88.4%
+Zip file size: 1367695 bytes, number of entries: 702
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/
+-rw-rw-r--  2.0 unx     1074 b- defN 24-Apr-05 08:24 nfelib-2.0.6/MIT-LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 24-Apr-05 08:24 nfelib-2.0.6/setup.py
+-rw-rw-r--  2.0 unx     1493 b- defN 24-May-15 17:08 nfelib-2.0.6/setup.cfg
+-rw-rw-r--  2.0 unx     7477 b- defN 24-May-08 10:59 nfelib-2.0.6/README.md
+-rw-rw-r--  2.0 unx     8697 b- defN 24-May-15 17:08 nfelib-2.0.6/PKG-INFO
+-rw-rw-r--  2.0 unx       64 b- defN 24-Apr-05 08:24 nfelib-2.0.6/MANIFEST.in
+-rw-rw-r--  2.0 unx        7 b- defN 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    30786 b- defN 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      113 b- defN 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     8697 b- defN 24-May-15 17:08 nfelib-2.0.6/nfelib.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/nfse/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/mdfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/nfe_evento_cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/cte/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/nfe/
+-rwxrwxr-x  2.0 unx     2534 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/test_fingerprint.py
+-rw-rw-r--  2.0 unx    11598 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfse.xml
+-rw-rw-r--  2.0 unx      632 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfse_pedRegEvento.xml
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/__init__.py
+-rw-rw-r--  2.0 unx     1507 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfse_dps.xml
+-rw-rw-r--  2.0 unx     4370 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_cte.xml
+-rw-rw-r--  2.0 unx      453 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/fingerprint.txt
+-rw-rw-r--  2.0 unx     1230 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output.xml
+-rw-rw-r--  2.0 unx     1207 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfe_evento_cce.xml
+-rw-rw-r--  2.0 unx      224 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_mdfe.xml
+-rw-rw-r--  2.0 unx      482 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfe_inut.xml
+-rw-rw-r--  2.0 unx    46226 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/output_nfe_leiaute.xml
+-rw-rw-r--  2.0 unx    41634 b- defN 24-May-08 11:10 nfelib-2.0.6/tests/input.xml
+-rw-rw-r--  2.0 unx     2549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/test_all.py
+-rw-rw-r--  2.0 unx     2608 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/nfse/test_nfse.py
+-rw-rw-r--  2.0 unx     1054 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/mdfe/test_mdfe.py
+-rw-rw-r--  2.0 unx     1102 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/nfe_evento_cce/test_cce.py
+-rw-rw-r--  2.0 unx     1049 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/cte/test_cte.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/cce/v1_00/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/tests/cce/v1_00/leiauteCCe/
+-rw-rw-r--  2.0 unx     1128 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+-rw-rw-r--  2.0 unx       23 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/nfe/__init__.py
+-rw-rw-r--  2.0 unx     4504 b- defN 24-Apr-05 08:24 nfelib-2.0.6/tests/nfe/test_nfe_legacy.py
+-rw-rw-r--  2.0 unx     8764 b- defN 24-Apr-08 21:49 nfelib-2.0.6/tests/nfe/test_nfe.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/v4_00/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_mde/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_insucesso/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_epec/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_entrega/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cancel/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/bpe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_ator_interessado/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_generico/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_cons/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/
+-rw-rw-r--  2.0 unx     7673 b- defN 24-May-15 17:05 nfelib-2.0.6/nfelib/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/samples/v1_0/
+-rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
+-rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
+-rw-rw-r--  2.0 unx      728 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
+-rw-rw-r--  2.0 unx    10940 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/bindings/__init__.py
+-rw-rw-r--  2.0 unx      516 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
+-rw-rw-r--  2.0 unx     5937 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx    36107 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
+-rw-rw-r--  2.0 unx      496 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
+-rw-rw-r--  2.0 unx   102239 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
+-rw-rw-r--  2.0 unx      494 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/dps_v1_00.py
+-rw-rw-r--  2.0 unx    16194 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
+-rw-rw-r--  2.0 unx      498 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/nfse/bindings/v1_0/evento_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/
+-rw-rw-r--  2.0 unx    29312 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
+-rw-rw-r--  2.0 unx      648 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
+-rw-rw-r--  2.0 unx      752 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    78115 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
+-rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
+-rw-rw-r--  2.0 unx     3406 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
+-rw-rw-r--  2.0 unx    57965 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
+-rw-rw-r--  2.0 unx      743 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
+-rw-rw-r--  2.0 unx    88685 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retConsStatServ.py
+-rw-rw-r--  2.0 unx  1859480 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retEnviNFe.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/__init__.py
+-rw-rw-r--  2.0 unx      280 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/README.txt
+-rw-rw-r--  2.0 unx   235328 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retEnvConfRecebto.py
+-rw-rw-r--  2.0 unx   231041 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retEnvEvento.py
+-rw-rw-r--  2.0 unx     3387 b- defN 24-Apr-08 21:49 nfelib-2.0.6/nfelib/v4_00/leiauteNFe_sub.py
+-rw-rw-r--  2.0 unx   188157 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retInutNFe.py
+-rw-rw-r--  2.0 unx   159793 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retConsCad.py
+-rw-rw-r--  2.0 unx    80047 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/distDFeInt.py
+-rw-rw-r--  2.0 unx    79013 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retDistDFeInt.py
+-rw-rw-r--  2.0 unx  1859541 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retConsReciNFe.py
+-rw-rw-r--  2.0 unx   239970 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retEnvCCe.py
+-rw-rw-r--  2.0 unx   237200 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retEnvEventoCancNFe.py
+-rw-rw-r--  2.0 unx   289846 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/v4_00/retConsSitNFe.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/
+-rw-rw-r--  2.0 unx      947 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
+-rw-rw-r--  2.0 unx     1407 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx     1816 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
+-rw-rw-r--  2.0 unx     3789 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
+-rw-rw-r--  2.0 unx     2719 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
+-rw-rw-r--  2.0 unx     2057 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
+-rw-rw-r--  2.0 unx     3574 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
+-rw-rw-r--  2.0 unx      180 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
+-rw-rw-r--  2.0 unx      702 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx      732 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx      739 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
+-rw-rw-r--  2.0 unx      226 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     5571 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     7084 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/__init__.py
+-rw-rw-r--  2.0 unx      545 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     6239 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     5995 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     7833 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
+-rw-rw-r--  2.0 unx    11143 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     1963 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      546 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      580 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
+-rw-rw-r--  2.0 unx     5622 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      519 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      538 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx    35874 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
+-rw-rw-r--  2.0 unx    14799 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     1660 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx    10218 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
+-rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     4353 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     5673 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
+-rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx   126107 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      493 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     2307 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     3231 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
+-rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/
+-rw-rw-r--  2.0 unx     6549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
+-rw-rw-r--  2.0 unx      620 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     1935 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4033 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      673 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    36487 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
+-rw-rw-r--  2.0 unx     1564 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      592 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3479 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
+-rw-rw-r--  2.0 unx     5523 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
+-rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      632 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    10610 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      605 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
+-rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      711 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    24229 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3958 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx    99783 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx    10365 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
+-rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4559 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
+-rw-rw-r--  2.0 unx     5554 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4309 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx    10018 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      574 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      622 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     1967 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/__init__.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1670 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
+-rw-rw-r--  2.0 unx    20302 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/
+-rw-rw-r--  2.0 unx    15624 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx      598 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1767 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
+-rw-rw-r--  2.0 unx     1269 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
+-rw-rw-r--  2.0 unx     1755 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx     1253 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
+-rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/
+-rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/
+-rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/__init__.py
+-rw-rw-r--  2.0 unx     5466 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
+-rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1010 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1811 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      578 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      550 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    16741 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      566 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/
+-rw-rw-r--  2.0 unx      725 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4651 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
+-rw-rw-r--  2.0 unx     4459 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    11599 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      596 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    11613 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1774 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
+-rw-rw-r--  2.0 unx      617 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32624 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      634 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      745 b- defN 24-May-08 11:08 nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_epec/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_epec/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1435 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx    10677 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
+-rw-rw-r--  2.0 unx    37803 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/
+-rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx     4475 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
+-rw-rw-r--  2.0 unx      608 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx    17318 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_entrega/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_entrega/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1782 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      565 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    17661 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     5351 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/
+-rw-rw-r--  2.0 unx      744 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      615 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      596 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4424 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
+-rw-rw-r--  2.0 unx    11920 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    12382 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      724 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32624 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     2191 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
+-rw-rw-r--  2.0 unx      634 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     4873 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1375 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     5501 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
+-rw-rw-r--  2.0 unx     5290 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
+-rw-rw-r--  2.0 unx     4141 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx     4407 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     8230 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
+-rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     4495 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
+-rw-rw-r--  2.0 unx     4933 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1954 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
+-rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1773 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      551 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    20018 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    13952 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      589 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32400 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1002 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     1067 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+-rw-rw-r--  2.0 unx     5420 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx     3407 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     4283 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     8554 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/bpe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/bpe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     4651 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     4296 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     5551 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      539 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      472 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
+-rw-rw-r--  2.0 unx    13972 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx      497 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
+-rw-rw-r--  2.0 unx      599 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1542 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2295 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
+-rw-rw-r--  2.0 unx   131130 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/
+-rw-rw-r--  2.0 unx      698 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      619 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx   107163 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx      594 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx    23114 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1411 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1570 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      649 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
+-rw-rw-r--  2.0 unx     2028 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
+-rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     9549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx     1668 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
+-rw-rw-r--  2.0 unx      631 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1862 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
+-rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx      678 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      582 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      563 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4106 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     3279 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1028 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      352 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+-rw-rw-r--  2.0 unx      310 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
+-rw-rw-r--  2.0 unx     5453 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx    22419 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     2843 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     4248 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     6807 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/samples/v1_0/
+-rw-rw-r--  2.0 unx     1207 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/__init__.py
+-rw-rw-r--  2.0 unx      514 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1705 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    22394 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
+-rw-rw-r--  2.0 unx     1850 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
+-rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
+-rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/
+-rw-rw-r--  2.0 unx    17276 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      657 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     3340 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
+-rw-rw-r--  2.0 unx      630 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     2035 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx      573 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx     4481 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
+-rw-rw-r--  2.0 unx      557 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx    21825 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/
+-rw-rw-r--  2.0 unx      609 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx     3942 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
+-rw-rw-r--  2.0 unx    15700 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      618 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx    31796 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/samples/v4_0/
+-rw-rw-r--  2.0 unx     3436 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
+-rw-rw-r--  2.0 unx     1558 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
+-rw-rw-r--  2.0 unx    10117 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
+-rw-rw-r--  2.0 unx     3168 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
+-rw-rw-r--  2.0 unx     4378 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/bindings/v4_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/cte/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1769 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
+-rw-rw-r--  2.0 unx      594 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
+-rw-rw-r--  2.0 unx     3786 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
+-rw-rw-r--  2.0 unx     6898 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
+-rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     5859 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     8883 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/__init__.py
+-rw-rw-r--  2.0 unx     2303 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
+-rw-rw-r--  2.0 unx     5940 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
+-rw-rw-r--  2.0 unx      564 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx     2294 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
+-rw-rw-r--  2.0 unx      534 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1661 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
+-rw-rw-r--  2.0 unx     4686 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
+-rw-rw-r--  2.0 unx      478 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_v4_00.py
+-rw-rw-r--  2.0 unx      574 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
+-rw-rw-r--  2.0 unx     6926 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
+-rw-rw-r--  2.0 unx    18408 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     4334 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1540 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
+-rw-rw-r--  2.0 unx      559 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
+-rw-rw-r--  2.0 unx     7464 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx     8259 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
+-rw-rw-r--  2.0 unx    11300 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
+-rw-rw-r--  2.0 unx     1780 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
+-rw-rw-r--  2.0 unx   424251 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx      530 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx      503 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
+-rw-rw-r--  2.0 unx      538 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx     5479 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
+-rw-rw-r--  2.0 unx      526 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
+-rw-rw-r--  2.0 unx      537 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
+-rw-rw-r--  2.0 unx     6178 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     1676 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1684 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx    14185 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     2313 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
+-rw-rw-r--  2.0 unx      475 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/gtve_v4_00.py
+-rw-rw-r--  2.0 unx      507 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
+-rw-rw-r--  2.0 unx     8880 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
+-rw-rw-r--  2.0 unx    10485 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
+-rw-rw-r--  2.0 unx     1773 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/cte/schemas/v4_0/
+-rw-rw-r--  2.0 unx     4259 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
+-rw-rw-r--  2.0 unx   332786 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx    10576 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
+-rw-rw-r--  2.0 unx      700 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     8583 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
+-rw-rw-r--  2.0 unx     6338 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      698 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     2213 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
+-rw-rw-r--  2.0 unx      706 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
+-rw-rw-r--  2.0 unx      702 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx      699 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     2075 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
+-rw-rw-r--  2.0 unx     9313 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      677 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
+-rw-rw-r--  2.0 unx     5494 b- defN 23-Mar-09 13:51 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1707 b- defN 23-Feb-27 09:00 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
+-rw-rw-r--  2.0 unx      734 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx    11173 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx     6498 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     8005 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
+-rw-rw-r--  2.0 unx    24294 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      651 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1648 b- defN 23-Mar-09 13:52 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
+-rw-rw-r--  2.0 unx      834 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      800 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      741 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx    13190 b- defN 23-Apr-28 08:26 nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      677 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
+-rw-rw-r--  2.0 unx     4735 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1679 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
+-rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      669 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     7868 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
+-rw-rw-r--  2.0 unx      656 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
+-rw-rw-r--  2.0 unx      695 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      720 b- defN 24-May-08 08:07 nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
+-rw-rw-r--  2.0 unx     1668 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1516 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 23-Feb-27 11:40 nfelib-2.0.6/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
+-rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
+-rw-rw-r--  2.0 unx      542 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    19324 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    14282 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_cons/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_cons/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      934 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1504 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/__init__.py
+-rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
+-rw-rw-r--  2.0 unx    29843 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/
+-rw-rw-r--  2.0 unx      655 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
+-rw-rw-r--  2.0 unx    22200 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
+-rw-rw-r--  2.0 unx    29554 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      686 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/ws/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/samples/v4_0/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteInutNFe/
+-rw-rw-r--  2.0 unx    10647 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+-rw-rw-r--  2.0 unx     7180 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+-rw-rw-r--  2.0 unx    37663 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+-rw-rw-r--  2.0 unx    14538 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+-rw-rw-r--  2.0 unx    32177 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+-rw-rw-r--  2.0 unx     9218 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+-rw-rw-r--  2.0 unx    68825 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+-rw-rw-r--  2.0 unx    10834 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+-rw-rw-r--  2.0 unx     9301 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+-rw-rw-r--  2.0 unx    12034 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+-rw-rw-r--  2.0 unx    11802 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+-rw-rw-r--  2.0 unx     9767 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+-rw-rw-r--  2.0 unx    46079 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+-rw-rw-r--  2.0 unx     5549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
+-rw-rw-r--  2.0 unx    19459 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
+-rw-rw-r--  2.0 unx    46216 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
+-rw-rw-r--  2.0 unx      484 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx    30307 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      512 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     7598 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/__init__.py
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      459 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
+-rw-rw-r--  2.0 unx      567 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
+-rw-rw-r--  2.0 unx     2676 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx    16440 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
+-rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx    13133 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      591 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
+-rw-rw-r--  2.0 unx     5962 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      467 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      533 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
+-rw-rw-r--  2.0 unx   494616 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      558 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
+-rw-rw-r--  2.0 unx       26 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/ws/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 24-May-15 17:04 nfelib-2.0.6/nfelib/nfe/ws/edoc_legacy.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-15 17:08 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/
+-rw-rw-r--  2.0 unx     3902 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      628 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
+-rw-rw-r--  2.0 unx    20000 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     7801 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    15469 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
+-rw-rw-r--  2.0 unx      617 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      568 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    21976 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx   334026 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      604 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx    32310 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      602 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.6/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+702 files, 10554921 bytes uncompressed, 1230049 bytes compressed:  88.4%
```

## zipnote {}

```diff
@@ -1,2107 +1,2107 @@
-Filename: nfelib-2.0.5/
+Filename: nfelib-2.0.6/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/
+Filename: nfelib-2.0.6/nfelib.egg-info/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/
+Filename: nfelib-2.0.6/tests/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/
+Filename: nfelib-2.0.6/nfelib/
 Comment: 
 
-Filename: nfelib-2.0.5/MIT-LICENSE
+Filename: nfelib-2.0.6/MIT-LICENSE
 Comment: 
 
-Filename: nfelib-2.0.5/setup.py
+Filename: nfelib-2.0.6/setup.py
 Comment: 
 
-Filename: nfelib-2.0.5/setup.cfg
+Filename: nfelib-2.0.6/setup.cfg
 Comment: 
 
-Filename: nfelib-2.0.5/README.md
+Filename: nfelib-2.0.6/README.md
 Comment: 
 
-Filename: nfelib-2.0.5/PKG-INFO
+Filename: nfelib-2.0.6/PKG-INFO
 Comment: 
 
-Filename: nfelib-2.0.5/MANIFEST.in
+Filename: nfelib-2.0.6/MANIFEST.in
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/top_level.txt
+Filename: nfelib-2.0.6/nfelib.egg-info/top_level.txt
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/SOURCES.txt
+Filename: nfelib-2.0.6/nfelib.egg-info/SOURCES.txt
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/requires.txt
+Filename: nfelib-2.0.6/nfelib.egg-info/requires.txt
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/dependency_links.txt
+Filename: nfelib-2.0.6/nfelib.egg-info/dependency_links.txt
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib.egg-info/PKG-INFO
+Filename: nfelib-2.0.6/nfelib.egg-info/PKG-INFO
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfse/
+Filename: nfelib-2.0.6/tests/nfse/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/mdfe/
+Filename: nfelib-2.0.6/tests/mdfe/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe_evento_cce/
+Filename: nfelib-2.0.6/tests/nfe_evento_cce/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cte/
+Filename: nfelib-2.0.6/tests/cte/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cce/
+Filename: nfelib-2.0.6/tests/cce/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe/
+Filename: nfelib-2.0.6/tests/nfe/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/test_fingerprint.py
+Filename: nfelib-2.0.6/tests/test_fingerprint.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfse.xml
+Filename: nfelib-2.0.6/tests/output_nfse.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml
+Filename: nfelib-2.0.6/tests/output_nfse_pedRegEvento.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/__init__.py
+Filename: nfelib-2.0.6/tests/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfse_dps.xml
+Filename: nfelib-2.0.6/tests/output_nfse_dps.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_cte.xml
+Filename: nfelib-2.0.6/tests/output_cte.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/fingerprint.txt
+Filename: nfelib-2.0.6/tests/fingerprint.txt
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output.xml
+Filename: nfelib-2.0.6/tests/output.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfe_evento_cce.xml
+Filename: nfelib-2.0.6/tests/output_nfe_evento_cce.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_mdfe.xml
+Filename: nfelib-2.0.6/tests/output_mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfe_inut.xml
+Filename: nfelib-2.0.6/tests/output_nfe_inut.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/output_nfe_leiaute.xml
+Filename: nfelib-2.0.6/tests/output_nfe_leiaute.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/input.xml
+Filename: nfelib-2.0.6/tests/input.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/test_all.py
+Filename: nfelib-2.0.6/tests/test_all.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfse/test_nfse.py
+Filename: nfelib-2.0.6/tests/nfse/test_nfse.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/mdfe/test_mdfe.py
+Filename: nfelib-2.0.6/tests/mdfe/test_mdfe.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py
+Filename: nfelib-2.0.6/tests/nfe_evento_cce/test_cce.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cte/test_cte.py
+Filename: nfelib-2.0.6/tests/cte/test_cte.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cce/v1_00/
+Filename: nfelib-2.0.6/tests/cce/v1_00/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/
+Filename: nfelib-2.0.6/tests/cce/v1_00/leiauteCCe/
 Comment: 
 
-Filename: nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+Filename: nfelib-2.0.6/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe/__init__.py
+Filename: nfelib-2.0.6/tests/nfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe/test_nfe_legacy.py
+Filename: nfelib-2.0.6/tests/nfe/test_nfe_legacy.py
 Comment: 
 
-Filename: nfelib-2.0.5/tests/nfe/test_nfe.py
+Filename: nfelib-2.0.6/tests/nfe/test_nfe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/
+Filename: nfelib-2.0.6/nfelib/nfse/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/
+Filename: nfelib-2.0.6/nfelib/v4_00/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/
+Filename: nfelib-2.0.6/nfelib/mdfe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/
+Filename: nfelib-2.0.6/nfelib/nfe_epec/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/
+Filename: nfelib-2.0.6/nfelib/bpe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/
+Filename: nfelib-2.0.6/nfelib/cte/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/
+Filename: nfelib-2.0.6/nfelib/nfe_cons/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/
+Filename: nfelib-2.0.6/nfelib/nfe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/__init__.py
+Filename: nfelib-2.0.6/nfelib/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/
+Filename: nfelib-2.0.6/nfelib/nfse/samples/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfse/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfse/samples/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
+Filename: nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
+Filename: nfelib-2.0.6/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
+Filename: nfelib-2.0.6/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
+Filename: nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/dps_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/dps_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/evento_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfse/bindings/v1_0/evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retConsStatServ.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retEnviNFe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/__init__.py
+Filename: nfelib-2.0.6/nfelib/v4_00/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/README.txt
+Filename: nfelib-2.0.6/nfelib/v4_00/README.txt
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retEnvConfRecebto.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retEnvEvento.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py
+Filename: nfelib-2.0.6/nfelib/v4_00/leiauteNFe_sub.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retInutNFe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retInutNFe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retConsCad.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retConsCad.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/distDFeInt.py
+Filename: nfelib-2.0.6/nfelib/v4_00/distDFeInt.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retDistDFeInt.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retConsReciNFe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retEnvCCe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retEnvEventoCancNFe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py
+Filename: nfelib-2.0.6/nfelib/v4_00/retConsSitNFe.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
+Filename: nfelib-2.0.6/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_epec/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/__init__.py
+Filename: nfelib-2.0.6/nfelib/bpe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/samples/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/samples/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/
+Filename: nfelib-2.0.6/nfelib/cte/samples/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/
+Filename: nfelib-2.0.6/nfelib/cte/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/
+Filename: nfelib-2.0.6/nfelib/cte/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
+Filename: nfelib-2.0.6/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/gtve_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/
+Filename: nfelib-2.0.6/nfelib/nfe/samples/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/ws/
+Filename: nfelib-2.0.6/nfelib/nfe/ws/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteInutNFe/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
+Filename: nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
+Filename: nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/ws/__init__.py
+Filename: nfelib-2.0.6/nfelib/nfe/ws/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py
+Filename: nfelib-2.0.6/nfelib/nfe/ws/edoc_legacy.py
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.6/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
 Zip file comment:
```

## Comparing `nfelib-2.0.5/MIT-LICENSE` & `nfelib-2.0.6/MIT-LICENSE`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/setup.cfg` & `nfelib-2.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nfelib
-version = 2.0.5
+version = 2.0.6
 description = nfelib: electronic invoicing library for Brazil
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/akretion/nfelib
 author = Raphaël Valyi
 author_email = "raphael.valyi@akretion.com.br"
 license = MIT
```

## Comparing `nfelib-2.0.5/README.md` & `nfelib-2.0.6/README.md`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/PKG-INFO` & `nfelib-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 2.0.5
+Version: 2.0.6
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nfelib Version: 2.0.5 Summary: nfelib: electronic
+Metadata-Version: 2.1 Name: nfelib Version: 2.0.6 Summary: nfelib: electronic
 invoicing library for Brazil Home-page: https://github.com/akretion/nfelib
 Author: RaphaÃ«l Valyi Author-email: "raphael.valyi@akretion.com.br" License:
 MIT Project-URL: Source, https://github.com/akretion/nfelib Keywords: e-
 invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

## Comparing `nfelib-2.0.5/nfelib.egg-info/SOURCES.txt` & `nfelib-2.0.6/nfelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib.egg-info/PKG-INFO` & `nfelib-2.0.6/nfelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 2.0.5
+Version: 2.0.6
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nfelib Version: 2.0.5 Summary: nfelib: electronic
+Metadata-Version: 2.1 Name: nfelib Version: 2.0.6 Summary: nfelib: electronic
 invoicing library for Brazil Home-page: https://github.com/akretion/nfelib
 Author: RaphaÃ«l Valyi Author-email: "raphael.valyi@akretion.com.br" License:
 MIT Project-URL: Source, https://github.com/akretion/nfelib Keywords: e-
 invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

## Comparing `nfelib-2.0.5/tests/test_fingerprint.py` & `nfelib-2.0.6/tests/test_fingerprint.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_nfse.xml` & `nfelib-2.0.6/tests/output_nfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml` & `nfelib-2.0.6/tests/output_nfse_pedRegEvento.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_nfse_dps.xml` & `nfelib-2.0.6/tests/output_nfse_dps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_cte.xml` & `nfelib-2.0.6/tests/output_cte.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output.xml` & `nfelib-2.0.6/tests/output.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_nfe_evento_cce.xml` & `nfelib-2.0.6/tests/output_nfe_evento_cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/output_nfe_leiaute.xml` & `nfelib-2.0.6/tests/output_nfe_leiaute.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/input.xml` & `nfelib-2.0.6/tests/input.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/test_all.py` & `nfelib-2.0.6/tests/test_all.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/nfse/test_nfse.py` & `nfelib-2.0.6/tests/nfse/test_nfse.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/mdfe/test_mdfe.py` & `nfelib-2.0.6/tests/mdfe/test_mdfe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py` & `nfelib-2.0.6/tests/nfe_evento_cce/test_cce.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/cte/test_cte.py` & `nfelib-2.0.6/tests/cte/test_cte.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml` & `nfelib-2.0.6/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/nfe/test_nfe_legacy.py` & `nfelib-2.0.6/tests/nfe/test_nfe_legacy.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/tests/nfe/test_nfe.py` & `nfelib-2.0.6/tests/nfe/test_nfe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/__init__.py` & `nfelib-2.0.6/nfelib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import xsdata
 from lxml import etree
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 class CommonMixin:
     """Generic helper class. Can be overriden for specific documents."""
 
     schema_path = None
     namespace = None
```

## Comparing `nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml` & `nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml` & `nfelib-2.0.6/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml` & `nfelib-2.0.6/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml` & `nfelib-2.0.6/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py` & `nfelib-2.0.6/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py` & `nfelib-2.0.6/nfelib/v4_00/retConsStatServ.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py` & `nfelib-2.0.6/nfelib/v4_00/retEnviNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py` & `nfelib-2.0.6/nfelib/v4_00/retEnvConfRecebto.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py` & `nfelib-2.0.6/nfelib/v4_00/retEnvEvento.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py` & `nfelib-2.0.6/nfelib/v4_00/leiauteNFe_sub.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retInutNFe.py` & `nfelib-2.0.6/nfelib/v4_00/retInutNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retConsCad.py` & `nfelib-2.0.6/nfelib/v4_00/retConsCad.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/distDFeInt.py` & `nfelib-2.0.6/nfelib/v4_00/distDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py` & `nfelib-2.0.6/nfelib/v4_00/retDistDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py` & `nfelib-2.0.6/nfelib/v4_00/retConsReciNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py` & `nfelib-2.0.6/nfelib/v4_00/retEnvCCe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py` & `nfelib-2.0.6/nfelib/v4_00/retEnvEventoCancNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py` & `nfelib-2.0.6/nfelib/v4_00/retConsSitNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml` & `nfelib-2.0.6/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py` & `nfelib-2.0.6/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd` & `nfelib-2.0.6/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py` & `nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py` & `nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py` & `nfelib-2.0.6/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd` & `nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd` & `nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py` & `nfelib-2.0.6/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.6/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml` & `nfelib-2.0.6/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML` & `nfelib-2.0.6/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml` & `nfelib-2.0.6/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml` & `nfelib-2.0.6/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml` & `nfelib-2.0.6/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml` & `nfelib-2.0.6/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py` & `nfelib-2.0.6/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/cte_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py` & `nfelib-2.0.6/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py` & `nfelib-2.0.6/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd` & `nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd` & `nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd` & `nfelib-2.0.6/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml` & `nfelib-2.0.6/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py` & `nfelib-2.0.6/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py` & `nfelib-2.0.6/nfelib/nfe/ws/edoc_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,27 +104,39 @@
     def consulta_documento(self, chave):
         raiz = ConsSitNfe(
             versao=self.versao,
             tpAmb=self.ambiente,
             xServ="CONSULTAR",
             chNFe=chave,
         )
-        return self._post(
-            raiz=raiz,
-            url=localizar_url(
+
+        # Check if the method ´_get_ws_endpoint´ exists to ensure compatibility 
+        # with different versions of the erpbrasil.edoc library.
+        if hasattr(self, '_get_ws_endpoint'):
+            url = self._get_ws_endpoint(WS_NFE_CONSULTA)
+        else:
+            # TODO: Remove this fallback in the next few months.
+            # The following block is a temporary solution to support older versions.
+            # After transitioning, remove the localizar_url method call.
+            url = localizar_url(
                 WS_NFE_CONSULTA,
                 str(self.uf),
                 self.mod,
                 int(self.ambiente)
-            ),
+            )
+
+        return self._post(
+            raiz=raiz,
+            url=url,
             operacao="nfeConsultaNF",
             classe=RetConsSitNfe,
         )
 
 
+
 class NFCeAdapter(DocumentoElectronicoAdapter, NFCe):
     pass
 
 
 class MDeAdapter(DocumentoElectronicoAdapter, MDe):
     pass
```

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.6/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

