# Comparing `tmp/chik_rs-0.6.1.tar.gz` & `tmp/chik_rs-0.7.0.tar.gz`

## Comparing `chik_rs-0.6.1.tar` & `chik_rs-0.7.0.tar`

### file list

```diff
@@ -1,126 +1,144 @@
--rw-r--r--   0     1001      127      415 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/Cargo.toml
--rw-r--r--   0     1001      127    10152 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/src/from_klvm.rs
--rw-r--r--   0     1001      127     2602 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/src/helpers.rs
--rw-r--r--   0     1001      127      603 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/src/lib.rs
--rw-r--r--   0     1001      127     1217 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/src/macros.rs
--rw-r--r--   0     1001      127     7548 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-derive/src/to_klvm.rs
--rw-r--r--   0     1001      127      625 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/Cargo.toml
--rw-r--r--   0     1001      127      839 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/chik_error.rs
--rw-r--r--   0     1001      127     2346 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/from_json_dict.rs
--rw-r--r--   0     1001      127     2480 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/int.rs
--rw-r--r--   0     1001      127      457 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/lib.rs
--rw-r--r--   0     1001      127    20419 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/streamable.rs
--rw-r--r--   0     1001      127     1892 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-traits/src/to_json_dict.rs
--rw-r--r--   0     1001      127     1134 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/Cargo.toml
--rw-r--r--   0     1001      127     4313 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/README.md
--rw-r--r--   0     1001      127     3186 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/benches/run-generator.rs
--rw-r--r--   0     1001      127     2182 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/benches/tree-hash.rs
--rw-r--r--   0     1001      127      266 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/allocator.rs
--rw-r--r--   0     1001      127     1228 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/error.rs
--rw-r--r--   0     1001      127    17250 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/fast_forward.rs
--rw-r--r--   0     1001      127     3075 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/coin_id.rs
--rw-r--r--   0     1001      127     5714 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      127   189117 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/conditions.rs
--rw-r--r--   0     1001      127     1751 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/flags.rs
--rw-r--r--   0     1001      127     6437 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      127     9639 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/messages.rs
--rw-r--r--   0     1001      127      480 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/mod.rs
--rw-r--r--   0     1001      127    11894 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/opcodes.rs
--rw-r--r--   0     1001      127     6795 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      127     2017 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      127     2944 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      127    10908 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/solution_generator.rs
--rw-r--r--   0     1001      127      471 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/spend_visitor.rs
--rw-r--r--   0     1001      127     9411 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/test_generators.rs
--rw-r--r--   0     1001      127     6371 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/gen/validation_error.rs
--rw-r--r--   0     1001      127     3133 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/generator_rom.rs
--rw-r--r--   0     1001      127      152 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/lib.rs
--rw-r--r--   0     1001      127    22644 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-consensus/src/merkle_set.rs
--rw-r--r--   0     1001      127     1151 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/Cargo.toml
--rw-r--r--   0     1001      127     7024 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/block_record.rs
--rw-r--r--   0     1001      127    17338 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/bytes.rs
--rw-r--r--   0     1001      127     4997 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/chik_protocol.rs
--rw-r--r--   0     1001      127     1208 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/classgroup.rs
--rw-r--r--   0     1001      127     4453 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/coin.rs
--rw-r--r--   0     1001      127      199 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      127      182 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/coin_state.rs
--rw-r--r--   0     1001      127      397 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      127      531 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      127     1983 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/foliage.rs
--rw-r--r--   0     1001      127     3226 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/full_node_protocol.rs
--rw-r--r--   0     1001      127     4342 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/fullblock.rs
--rw-r--r--   0     1001      127     3505 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/header_block.rs
--rw-r--r--   0     1001      127     1406 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/lazy_node.rs
--rw-r--r--   0     1001      127     1455 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/lib.rs
--rw-r--r--   0     1001      127      142 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/peer_info.rs
--rw-r--r--   0     1001      127      195 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/pool_target.rs
--rw-r--r--   0     1001      127    17472 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/program.rs
--rw-r--r--   0     1001      127      319 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      127     1967 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      127     1458 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/slots.rs
--rw-r--r--   0     1001      127     8260 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      127      449 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/sub_epoch_summary.rs
--rw-r--r--   0     1001      127     2343 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/unfinished_block.rs
--rw-r--r--   0     1001      127      338 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/vdf.rs
--rw-r--r--   0     1001      127     4071 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      127     2361 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-protocol/src/weight_proof.rs
--rw-r--r--   0     1001      127      454 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127    13876 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik_py_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127     1267 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/Cargo.toml
--rw-r--r--   0     1001      127     2115 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/README.md
--rw-r--r--   0     1001      127     1389 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/benches/derive_key.rs
--rw-r--r--   0     1001      127     1356 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/benches/parse.rs
--rw-r--r--   0     1001      127      828 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/benches/sign.rs
--rw-r--r--   0     1001      127     1023 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/benches/verify.rs
--rw-r--r--   0     1001      127       78 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/derivable_key.rs
--rw-r--r--   0     1001      127     1500 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/derive_keys.rs
--rw-r--r--   0     1001      127     1114 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/error.rs
--rw-r--r--   0     1001      127     4267 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/gtelement.rs
--rw-r--r--   0     1001      127      565 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/lib.rs
--rw-r--r--   0     1001      127     4484 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/mnemonic.rs
--rw-r--r--   0     1001      127    26579 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/public_key.rs
--rw-r--r--   0     1001      127    19133 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/secret_key.rs
--rw-r--r--   0     1001      127    41458 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-bls/src/signature.rs
--rw-r--r--   0     1001      127      809 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/Cargo.toml
--rw-r--r--   0     1001      127     6975 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/docs/derive_macros.md
--rw-r--r--   0     1001      127     1067 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/error.rs
--rw-r--r--   0     1001      127    10142 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/from_klvm.rs
--rw-r--r--   0     1001      127     1742 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/klvm_decoder.rs
--rw-r--r--   0     1001      127     1518 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/klvm_encoder.rs
--rw-r--r--   0     1001      127     5612 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/lib.rs
--rw-r--r--   0     1001      127     3246 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/macros.rs
--rw-r--r--   0     1001      127     1026 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/match_byte.rs
--rw-r--r--   0     1001      127     8530 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/to_klvm.rs
--rw-r--r--   0     1001      127      670 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-traits/src/wrappers.rs
--rw-r--r--   0     1001      127      759 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/Cargo.toml
--rw-r--r--   0     1001      127     6089 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/derive_synthetic.rs
--rw-r--r--   0     1001      127      114 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/lib.rs
--rw-r--r--   0     1001      127      710 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/proof.rs
--rw-r--r--   0     1001      127    11363 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/cat.rs
--rw-r--r--   0     1001      127     4507 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/did.rs
--rw-r--r--   0     1001      127    13636 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/nft.rs
--rw-r--r--   0     1001      127     2711 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/offer.rs
--rw-r--r--   0     1001      127     4717 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/singleton.rs
--rw-r--r--   0     1001      127     3082 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles/standard.rs
--rw-r--r--   0     1001      127      427 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik-wallet/src/puzzles.rs
--rw-r--r--   0     1001      127      516 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127     9355 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/chik_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127      471 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-utils/Cargo.toml
--rw-r--r--   0     1001      127     2069 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-utils/src/curried_program.rs
--rw-r--r--   0     1001      127     1899 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-utils/src/curry_tree_hash.rs
--rw-r--r--   0     1001      127      806 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-utils/src/lib.rs
--rw-r--r--   0     1001      127     9843 2024-04-15 04:01:23.000000 chik_rs-0.6.1/crates/klvm-utils/src/tree_hash.rs
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 chik_rs-0.6.1/wheel/Cargo.toml
--rw-r--r--   0     1001      127       77 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/README.md
--rw-r--r--   0     1001      127   147712 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/chik_rs.pyi
--rw-r--r--   0     1001      127    15138 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/generate_type_stubs.py
--rw-r--r--   0     1001      127        0 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/py.typed
--rw-r--r--   0     1001      127      364 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/src/adapt_response.rs
--rw-r--r--   0     1001      127    17725 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/src/api.rs
--rw-r--r--   0     1001      127      158 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/src/lib.rs
--rw-r--r--   0     1001      127     8579 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/src/run_generator.rs
--rw-r--r--   0     1001      127     1788 2024-04-15 04:01:23.000000 chik_rs-0.6.1/wheel/src/run_program.rs
--rw-r--r--   0     1001      127    72089 2024-04-15 04:01:23.000000 chik_rs-0.6.1/Cargo.lock
--rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 chik_rs-0.6.1/Cargo.toml
--rw-r--r--   0        0        0      184 1970-01-01 00:00:00.000000 chik_rs-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 chik_rs-0.6.1/PKG-INFO
+-rw-r--r--   0     1001      127      809 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/Cargo.toml
+-rw-r--r--   0     1001      127     6975 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/docs/derive_macros.md
+-rw-r--r--   0     1001      127     1067 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/error.rs
+-rw-r--r--   0     1001      127    10932 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/from_klvm.rs
+-rw-r--r--   0     1001      127     1742 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/klvm_decoder.rs
+-rw-r--r--   0     1001      127     1518 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/klvm_encoder.rs
+-rw-r--r--   0     1001      127     5612 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/lib.rs
+-rw-r--r--   0     1001      127     3246 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/macros.rs
+-rw-r--r--   0     1001      127     1026 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/match_byte.rs
+-rw-r--r--   0     1001      127     8909 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/to_klvm.rs
+-rw-r--r--   0     1001      127      670 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/wrappers.rs
+-rw-r--r--   0     1001      127     1151 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/Cargo.toml
+-rw-r--r--   0     1001      127     7024 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/block_record.rs
+-rw-r--r--   0     1001      127    17317 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/bytes.rs
+-rw-r--r--   0     1001      127     4997 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/chik_protocol.rs
+-rw-r--r--   0     1001      127     1194 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      127     4446 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin.rs
+-rw-r--r--   0     1001      127      199 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      127      182 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      127      397 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      127      531 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      127     1983 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/foliage.rs
+-rw-r--r--   0     1001      127     3226 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/full_node_protocol.rs
+-rw-r--r--   0     1001      127     4342 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      127     4114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/header_block.rs
+-rw-r--r--   0     1001      127     1406 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/lazy_node.rs
+-rw-r--r--   0     1001      127     1380 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/lib.rs
+-rw-r--r--   0     1001      127      142 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/peer_info.rs
+-rw-r--r--   0     1001      127      195 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      127    17472 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/program.rs
+-rw-r--r--   0     1001      127      319 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      127     1967 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      127     1458 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/slots.rs
+-rw-r--r--   0     1001      127     8260 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      127      449 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/sub_epoch_summary.rs
+-rw-r--r--   0     1001      127     2343 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/unfinished_block.rs
+-rw-r--r--   0     1001      127     1856 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/unfinished_header_block.rs
+-rw-r--r--   0     1001      127      338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/vdf.rs
+-rw-r--r--   0     1001      127     4071 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      127     2361 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/weight_proof.rs
+-rw-r--r--   0     1001      127      454 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127    16368 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_py_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127      471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/Cargo.toml
+-rw-r--r--   0     1001      127     2069 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/curried_program.rs
+-rw-r--r--   0     1001      127     1899 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/curry_tree_hash.rs
+-rw-r--r--   0     1001      127      806 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/lib.rs
+-rw-r--r--   0     1001      127     9836 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      127      625 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/Cargo.toml
+-rw-r--r--   0     1001      127      839 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/chik_error.rs
+-rw-r--r--   0     1001      127     2346 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/from_json_dict.rs
+-rw-r--r--   0     1001      127     2484 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/int.rs
+-rw-r--r--   0     1001      127      457 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/lib.rs
+-rw-r--r--   0     1001      127    20419 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/streamable.rs
+-rw-r--r--   0     1001      127     1892 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/to_json_dict.rs
+-rw-r--r--   0     1001      127      415 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/Cargo.toml
+-rw-r--r--   0     1001      127    10152 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/from_klvm.rs
+-rw-r--r--   0     1001      127     2602 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/helpers.rs
+-rw-r--r--   0     1001      127      603 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/lib.rs
+-rw-r--r--   0     1001      127     1217 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/macros.rs
+-rw-r--r--   0     1001      127     7548 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/to_klvm.rs
+-rw-r--r--   0     1001      127      516 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127     9355 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127      759 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/Cargo.toml
+-rw-r--r--   0     1001      127     6089 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/derive_synthetic.rs
+-rw-r--r--   0     1001      127      114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/lib.rs
+-rw-r--r--   0     1001      127      710 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/proof.rs
+-rw-r--r--   0     1001      127    11363 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/cat.rs
+-rw-r--r--   0     1001      127     4507 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/did.rs
+-rw-r--r--   0     1001      127    13636 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/nft.rs
+-rw-r--r--   0     1001      127     2711 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/offer.rs
+-rw-r--r--   0     1001      127     4717 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/singleton.rs
+-rw-r--r--   0     1001      127     3082 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/standard.rs
+-rw-r--r--   0     1001      127      427 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles.rs
+-rw-r--r--   0     1001      127     1471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/Cargo.toml
+-rw-r--r--   0     1001      127     4313 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/README.md
+-rw-r--r--   0     1001      127     2275 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/merkle-set.rs
+-rw-r--r--   0     1001      127     3186 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/run-generator.rs
+-rw-r--r--   0     1001      127     2182 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/tree-hash.rs
+-rw-r--r--   0     1001      127      266 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/allocator.rs
+-rw-r--r--   0     1001      127     4085 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/consensus_constants.rs
+-rw-r--r--   0     1001      127     1228 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/error.rs
+-rw-r--r--   0     1001      127    17250 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/fast_forward.rs
+-rw-r--r--   0     1001      127     3068 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/coin_id.rs
+-rw-r--r--   0     1001      127     5714 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      127   189253 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/conditions.rs
+-rw-r--r--   0     1001      127     1751 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/flags.rs
+-rw-r--r--   0     1001      127     6428 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      127     9647 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/messages.rs
+-rw-r--r--   0     1001      127      506 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/mod.rs
+-rw-r--r--   0     1001      127    11894 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/opcodes.rs
+-rw-r--r--   0     1001      127     5299 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/owned_conditions.rs
+-rw-r--r--   0     1001      127     6795 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      127     2004 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      127     2944 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      127    10908 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/solution_generator.rs
+-rw-r--r--   0     1001      127      471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/spend_visitor.rs
+-rw-r--r--   0     1001      127     9411 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/test_generators.rs
+-rw-r--r--   0     1001      127    14899 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/validation_error.rs
+-rw-r--r--   0     1001      127     3133 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/generator_rom.rs
+-rw-r--r--   0     1001      127      202 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/lib.rs
+-rw-r--r--   0     1001      127    17854 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/merkle_set.rs
+-rw-r--r--   0     1001      127    32196 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/merkle_tree.rs
+-rw-r--r--   0     1001      127     1267 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/Cargo.toml
+-rw-r--r--   0     1001      127     2115 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/README.md
+-rw-r--r--   0     1001      127     1389 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/derive_key.rs
+-rw-r--r--   0     1001      127     1356 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/parse.rs
+-rw-r--r--   0     1001      127      828 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/sign.rs
+-rw-r--r--   0     1001      127     1023 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/verify.rs
+-rw-r--r--   0     1001      127       78 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/derivable_key.rs
+-rw-r--r--   0     1001      127     1500 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/derive_keys.rs
+-rw-r--r--   0     1001      127     1114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/error.rs
+-rw-r--r--   0     1001      127     4267 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/gtelement.rs
+-rw-r--r--   0     1001      127      565 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/lib.rs
+-rw-r--r--   0     1001      127     4484 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/mnemonic.rs
+-rw-r--r--   0     1001      127    26579 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/public_key.rs
+-rw-r--r--   0     1001      127    19133 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/secret_key.rs
+-rw-r--r--   0     1001      127    41458 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/signature.rs
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 chik_rs-0.7.0/wheel/Cargo.toml
+-rw-r--r--   0     1001      127       77 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/README.md
+-rw-r--r--   0     1001      127    15905 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/generate_type_stubs.py
+-rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/py.typed
+-rw-r--r--   0     1001      127       23 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/__init__.py
+-rw-r--r--   0     1001      127   154338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/chik_rs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/py.typed
+-rw-r--r--   0     1001      127     2708 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127      385 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_bytes.py
+-rw-r--r--   0     1001      127     1629 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_ints.py
+-rw-r--r--   0     1001      127     3974 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/struct_stream.py
+-rw-r--r--   0     1001      127      364 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/adapt_response.rs
+-rw-r--r--   0     1001      127    18714 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/api.rs
+-rw-r--r--   0     1001      127      158 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/lib.rs
+-rw-r--r--   0     1001      127     3832 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/run_generator.rs
+-rw-r--r--   0     1001      127     1788 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/run_program.rs
+-rw-r--r--   0     1001      127    70689 2024-05-15 07:54:39.000000 chik_rs-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 chik_rs-0.7.0/Cargo.toml
+-rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 chik_rs-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/py.typed
+-rw-r--r--   0     1001      127     3974 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/struct_stream.py
+-rw-r--r--   0     1001      127      385 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_bytes.py
+-rw-r--r--   0     1001      127       23 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/__init__.py
+-rw-r--r--   0     1001      127     1629 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_ints.py
+-rw-r--r--   0     1001      127     2708 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127   154338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/chik_rs.pyi
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 chik_rs-0.7.0/PKG-INFO
```

### Comparing `chik_rs-0.6.1/crates/klvm-derive/src/from_klvm.rs` & `chik_rs-0.7.0/crates/klvm-derive/src/from_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-derive/src/helpers.rs` & `chik_rs-0.7.0/crates/klvm-derive/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-derive/src/lib.rs` & `chik_rs-0.7.0/crates/klvm-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-derive/src/macros.rs` & `chik_rs-0.7.0/crates/klvm-derive/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-derive/src/to_klvm.rs` & `chik_rs-0.7.0/crates/klvm-derive/src/to_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-traits/Cargo.toml` & `chik_rs-0.7.0/crates/chik-traits/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "chik-traits"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik traits for Streamable types (chik's serialization format)"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods"], optional = true }
-chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
+chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
 chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
 sha2 = "0.10.8"
 hex = "0.4.3"
 thiserror = "1.0.44"
```

### Comparing `chik_rs-0.6.1/crates/chik-traits/src/chik_error.rs` & `chik_rs-0.7.0/crates/chik-traits/src/chik_error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-traits/src/from_json_dict.rs` & `chik_rs-0.7.0/crates/chik-traits/src/from_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-traits/src/int.rs` & `chik_rs-0.7.0/crates/chik-traits/src/int.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::types::PyAny>;
 }
 
 macro_rules! primitive_int {
     ($t:ty, $name:expr) => {
         impl ChikToPython for $t {
             fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
-                let int_module = PyModule::import(py, "chik.util.ints")?;
+                let int_module = PyModule::import(py, "chik_rs.sized_ints")?;
                 let ty = int_module.getattr($name)?;
                 ty.call1((self.into_py(py),))
             }
         }
     };
 }
```

### Comparing `chik_rs-0.6.1/crates/chik-traits/src/streamable.rs` & `chik_rs-0.7.0/crates/chik-traits/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-traits/src/to_json_dict.rs` & `chik_rs-0.7.0/crates/chik-traits/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/Cargo.toml` & `chik_rs-0.7.0/crates/chik-consensus/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 [package]
 name = "chik-consensus"
-version = "0.6.1"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chik blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
-py-bindings = ["dep:pyo3"]
+py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro"]
 
 [dependencies]
 klvmr = "0.6.1"
 hex = "0.4.3"
 pyo3 = { version = ">=0.19.0", optional = true }
-klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
-chik-traits = { version = "0.6.0", path = "../chik-traits" }
-klvm-traits = { version = "0.6.0", path = "../klvm-traits" }
+sha2 = "0.10.8"
+chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
+chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
+klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
+chik-traits = { version = "0.7.0", path = "../chik-traits" }
+klvm-traits = { version = "0.7.0", path = "../klvm-traits" }
 klvm-derive = { version = "0.6.0", path = "../klvm-derive" }
-chik-protocol = { version = "0.6.0", path = "../chik-protocol" }
-chik-wallet = { version = "0.6.0", path = "../chik-wallet" }
+chik-protocol = { version = "0.7.0", path = "../chik-protocol" }
+chik-wallet = { version = "0.7.0", path = "../chik-wallet" }
 hex-literal = "0.4.1"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 num-traits = "0.2.15"
 rstest = "0.16.0"
 text-diff = "0.4.0"
 criterion = "0.5.1"
+rand = { version = "0.8.5", features = [ "small_rng" ] }
 
 [lib]
 bench = false
 
 [[bench]]
 name = "run-generator"
 harness = false
 
 [[bench]]
 name = "tree-hash"
 harness = false
+
+[[bench]]
+name = "merkle-set"
+harness = false
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/README.md` & `chik_rs-0.7.0/crates/chik-consensus/README.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/benches/run-generator.rs` & `chik_rs-0.7.0/crates/chik-consensus/benches/run-generator.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/benches/tree-hash.rs` & `chik_rs-0.7.0/crates/chik-consensus/benches/tree-hash.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/error.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/fast_forward.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/fast_forward.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/coin_id.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/coin_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use chik_protocol::bytes::Bytes32;
+use chik_protocol::Bytes32;
 use klvmr::allocator::{Allocator, NodePtr};
 use klvmr::sha2::{Digest, Sha256};
 
 pub fn compute_coin_id(
     a: &Allocator,
     parent_id: NodePtr,
     puzzle_hash: NodePtr,
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/condition_sanitizers.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/conditions.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/conditions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 use crate::gen::flags::{
     AGG_SIG_ARGS, COND_ARGS_NIL, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
     STRICT_ARGS_COUNT,
 };
 use crate::gen::messages::{Message, SpendId};
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::check_nil;
-use chik_protocol::bytes::Bytes32;
+use chik_protocol::Bytes32;
 use klvmr::allocator::{Allocator, NodePtr, SExp};
 use klvmr::cost::Cost;
 use klvmr::sha2::{Digest, Sha256};
 use std::cmp::{max, min};
 use std::collections::{HashMap, HashSet};
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
@@ -267,15 +267,15 @@
     a: &Allocator,
     mut c: NodePtr,
     op: ConditionOpcode,
     flags: u32,
 ) -> Result<Condition, ValidationErr> {
     match op {
         AGG_SIG_UNSAFE => {
-            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
+            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPublicKey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_UNSAFE takes exactly two parameters
             if (flags & COND_ARGS_NIL) != 0 || (flags & STRICT_ARGS_COUNT) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigUnsafe(pubkey, message))
@@ -287,15 +287,15 @@
                     _ => Ok(Condition::AggSigUnsafe(pubkey, message)),
                 }
             } else {
                 Ok(Condition::AggSigUnsafe(pubkey, message))
             }
         }
         AGG_SIG_ME => {
-            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
+            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPublicKey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_ME takes exactly two parameters
             if (flags & COND_ARGS_NIL) != 0 || (flags & STRICT_ARGS_COUNT) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigMe(pubkey, message))
@@ -312,15 +312,15 @@
         }
         AGG_SIG_PUZZLE
         | AGG_SIG_PUZZLE_AMOUNT
         | AGG_SIG_PARENT
         | AGG_SIG_AMOUNT
         | AGG_SIG_PARENT_PUZZLE
         | AGG_SIG_PARENT_AMOUNT => {
-            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
+            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPublicKey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_* take two parameters
 
             if (flags & STRICT_ARGS_COUNT) != 0 {
                 check_nil(a, rest(a, c)?)?;
             }
@@ -338,18 +338,18 @@
         }
         CREATE_COIN => {
             let puzzle_hash = sanitize_hash(a, first(a, c)?, 32, ErrorCode::InvalidPuzzleHash)?;
             c = rest(a, c)?;
             let node = first(a, c)?;
             let amount = match sanitize_uint(a, node, 8, ErrorCode::InvalidCoinAmount)? {
                 SanitizedUint::PositiveOverflow => {
-                    return Err(ValidationErr(node, ErrorCode::AmountExceedsMaximum));
+                    return Err(ValidationErr(node, ErrorCode::CoinAmountExceedsMaximum));
                 }
                 SanitizedUint::NegativeOverflow => {
-                    return Err(ValidationErr(node, ErrorCode::NegativeAmount));
+                    return Err(ValidationErr(node, ErrorCode::CoinAmountNegative));
                 }
                 SanitizedUint::Ok(amount) => amount,
             };
             // CREATE_COIN takes an optional 3rd parameter, which is a list of
             // byte buffers (typically a 32 byte hash). We only pull out the
             // first element for now, but may support more in the future.
             // If we find anything else, that's still OK, since garbage is
@@ -448,15 +448,15 @@
         ASSERT_MY_PARENT_ID => {
             maybe_check_args_terminator(a, c, flags)?;
             let id = sanitize_hash(a, first(a, c)?, 32, ErrorCode::AssertMyParentIdFailed)?;
             Ok(Condition::AssertMyParentId(id))
         }
         ASSERT_MY_PUZZLEHASH => {
             maybe_check_args_terminator(a, c, flags)?;
-            let id = sanitize_hash(a, first(a, c)?, 32, ErrorCode::AssertMyPuzzlehashFailed)?;
+            let id = sanitize_hash(a, first(a, c)?, 32, ErrorCode::AssertMyPuzzleHashFailed)?;
             Ok(Condition::AssertMyPuzzlehash(id))
         }
         ASSERT_MY_AMOUNT => {
             maybe_check_args_terminator(a, c, flags)?;
             let amount = parse_amount(a, first(a, c)?, ErrorCode::AssertMyAmountFailed)?;
             Ok(Condition::AssertMyAmount(amount))
         }
@@ -486,86 +486,86 @@
                 check_nil(a, c)?;
             }
             Ok(Condition::AssertEphemeral)
         }
         ASSERT_SECONDS_RELATIVE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertSecondsRelative;
+            let code = ErrorCode::AssertSecondsRelativeFailed;
             match sanitize_uint(a, node, 8, code)? {
                 SanitizedUint::PositiveOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::NegativeOverflow => Ok(Condition::SkipRelativeCondition),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertSecondsRelative(r)),
             }
         }
         ASSERT_SECONDS_ABSOLUTE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertSecondsAbsolute;
+            let code = ErrorCode::AssertSecondsAbsoluteFailed;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::NegativeOverflow => Ok(Condition::Skip),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertSecondsAbsolute(r)),
             }
         }
         ASSERT_HEIGHT_RELATIVE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertHeightRelative;
+            let code = ErrorCode::AssertHeightRelativeFailed;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::NegativeOverflow => Ok(Condition::SkipRelativeCondition),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertHeightRelative(r as u32)),
             }
         }
         ASSERT_HEIGHT_ABSOLUTE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertHeightAbsolute;
+            let code = ErrorCode::AssertHeightAbsoluteFailed;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::NegativeOverflow => Ok(Condition::Skip),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertHeightAbsolute(r as u32)),
             }
         }
         ASSERT_BEFORE_SECONDS_RELATIVE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertBeforeSecondsRelative;
+            let code = ErrorCode::AssertBeforeSecondsRelativeFailed;
             match sanitize_uint(a, node, 8, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::SkipRelativeCondition),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeSecondsRelative(r)),
             }
         }
         ASSERT_BEFORE_SECONDS_ABSOLUTE => {
             maybe_check_args_terminator(a, c, flags)?;
 
             let node = first(a, c)?;
-            let code = ErrorCode::AssertBeforeSecondsAbsolute;
+            let code = ErrorCode::AssertBeforeSecondsAbsoluteFailed;
             match sanitize_uint(a, node, 8, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::Skip),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeSecondsAbsolute(r)),
             }
         }
         ASSERT_BEFORE_HEIGHT_RELATIVE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertBeforeHeightRelative;
+            let code = ErrorCode::AssertBeforeHeightRelativeFailed;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::SkipRelativeCondition),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeHeightRelative(r as u32)),
             }
         }
         ASSERT_BEFORE_HEIGHT_ABSOLUTE => {
             maybe_check_args_terminator(a, c, flags)?;
             let node = first(a, c)?;
-            let code = ErrorCode::AssertBeforeHeightAbsolute;
+            let code = ErrorCode::AssertBeforeHeightAbsoluteFailed;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::Skip),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeHeightAbsolute(r as u32)),
             }
         }
         SEND_MESSAGE => {
@@ -1100,15 +1100,15 @@
             Condition::AssertMyParentId(id) => {
                 if a.atom(id).as_ref() != a.atom(spend.parent_id).as_ref() {
                     return Err(ValidationErr(c, ErrorCode::AssertMyParentIdFailed));
                 }
             }
             Condition::AssertMyPuzzlehash(hash) => {
                 if a.atom(hash).as_ref() != a.atom(spend.puzzle_hash).as_ref() {
-                    return Err(ValidationErr(c, ErrorCode::AssertMyPuzzlehashFailed));
+                    return Err(ValidationErr(c, ErrorCode::AssertMyPuzzleHashFailed));
                 }
             }
             Condition::CreateCoinAnnouncement(msg) => {
                 decrement(&mut announce_countdown, msg)?;
                 state.announce_coin.insert((spend.coin_id.clone(), msg));
             }
             Condition::CreatePuzzleAnnouncement(msg) => {
@@ -2091,60 +2091,60 @@
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(
     ASSERT_SECONDS_ABSOLUTE,
     "0x010000000000000000",
-    ErrorCode::AssertSecondsAbsolute
+    ErrorCode::AssertSecondsAbsoluteFailed
 )]
 #[case(
     ASSERT_SECONDS_RELATIVE,
     "0x010000000000000000",
-    ErrorCode::AssertSecondsRelative
+    ErrorCode::AssertSecondsRelativeFailed
 )]
 #[case(
     ASSERT_HEIGHT_ABSOLUTE,
     "0x0100000000",
-    ErrorCode::AssertHeightAbsolute
+    ErrorCode::AssertHeightAbsoluteFailed
 )]
 #[case(
     ASSERT_HEIGHT_RELATIVE,
     "0x0100000000",
-    ErrorCode::AssertHeightRelative
+    ErrorCode::AssertHeightRelativeFailed
 )]
 #[case(
     ASSERT_BEFORE_SECONDS_ABSOLUTE,
     "-1",
-    ErrorCode::AssertBeforeSecondsAbsolute
+    ErrorCode::AssertBeforeSecondsAbsoluteFailed
 )]
 #[case(
     ASSERT_BEFORE_SECONDS_ABSOLUTE,
     "0",
     ErrorCode::ImpossibleSecondsAbsoluteConstraints
 )]
 #[case(
     ASSERT_BEFORE_SECONDS_RELATIVE,
     "-1",
-    ErrorCode::AssertBeforeSecondsRelative
+    ErrorCode::AssertBeforeSecondsRelativeFailed
 )]
 #[case(
     ASSERT_BEFORE_HEIGHT_ABSOLUTE,
     "-1",
-    ErrorCode::AssertBeforeHeightAbsolute
+    ErrorCode::AssertBeforeHeightAbsoluteFailed
 )]
 #[case(
     ASSERT_BEFORE_HEIGHT_ABSOLUTE,
     "0",
     ErrorCode::ImpossibleHeightAbsoluteConstraints
 )]
 #[case(
     ASSERT_BEFORE_HEIGHT_RELATIVE,
     "-1",
-    ErrorCode::AssertBeforeHeightRelative
+    ErrorCode::AssertBeforeHeightRelativeFailed
 )]
 #[case(ASSERT_MY_BIRTH_HEIGHT, "-1", ErrorCode::AssertMyBirthHeightFailed)]
 #[case(
     ASSERT_MY_BIRTH_HEIGHT,
     "0x0100000000",
     ErrorCode::AssertMyBirthHeightFailed
 )]
@@ -2585,27 +2585,27 @@
 #[test]
 fn test_single_assert_my_puzzle_hash_mismatch() {
     // ASSERT_MY_PUZZLEHASH
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((72 ({h1} )))))")
             .unwrap_err()
             .1,
-        ErrorCode::AssertMyPuzzlehashFailed
+        ErrorCode::AssertMyPuzzleHashFailed
     );
 }
 
 #[test]
 fn test_single_invalid_assert_my_puzzle_hash() {
     // ASSERT_MY_PUZZLEHASH
     // the parent ID in the condition is 33 bytes long
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((72 ({long} )))))")
             .unwrap_err()
             .1,
-        ErrorCode::AssertMyPuzzlehashFailed
+        ErrorCode::AssertMyPuzzleHashFailed
     );
 }
 
 #[test]
 fn test_single_create_coin() {
     // CREATE_COIN
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((51 ({h2} (42 )))))").unwrap();
@@ -2664,26 +2664,26 @@
 #[test]
 fn test_create_coin_amount_exceeds_max() {
     // CREATE_COIN
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((51 ({h2} (0x010000000000000000 )))))")
             .unwrap_err()
             .1,
-        ErrorCode::AmountExceedsMaximum
+        ErrorCode::CoinAmountExceedsMaximum
     );
 }
 
 #[test]
 fn test_create_coin_negative_amount() {
     // CREATE_COIN
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((51 ({h2} (-1 )))))")
             .unwrap_err()
             .1,
-        ErrorCode::NegativeAmount
+        ErrorCode::CoinAmountNegative
     );
 }
 
 #[test]
 fn test_create_coin_invalid_puzzlehash() {
     // CREATE_COIN
     assert_eq!(
@@ -3098,15 +3098,15 @@
                 "((({{h1}} ({{h2}} (123 ((({} ({{h2}} ({{msg1}} )))))",
                 condition as u8
             ),
             ENABLE_SOFTFORK_CONDITION | mempool
         )
         .unwrap_err()
         .1,
-        ErrorCode::InvalidPubkey
+        ErrorCode::InvalidPublicKey
     );
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(AGG_SIG_ME)]
 #[case(AGG_SIG_PARENT)]
@@ -3413,15 +3413,15 @@
 #[test]
 fn test_agg_sig_unsafe_invalid_pubkey() {
     // AGG_SIG_UNSAFE
     assert_eq!(
         cond_test("((({h1} ({h2} (123 (((49 ({h2} ({msg1} )))))")
             .unwrap_err()
             .1,
-        ErrorCode::InvalidPubkey
+        ErrorCode::InvalidPublicKey
     );
 }
 
 #[test]
 fn test_agg_sig_unsafe_invalid_msg() {
     // AGG_SIG_UNSAFE
     assert_eq!(
@@ -4829,23 +4829,23 @@
 #[case("(66 (0x3c ({msg2} ({msg1} )", ErrorCode::InvalidParentId)]
 #[case("(66 (0x3a ({long} ({msg1} )", ErrorCode::InvalidPuzzleHash)]
 #[case("(66 (0x3a ({msg2} ({msg1} )", ErrorCode::InvalidPuzzleHash)]
 #[case("(66 (0x3f ({long} ({msg1} )", ErrorCode::InvalidCoinId)]
 #[case("(66 (0x3f ({msg2} ({msg1} )", ErrorCode::InvalidCoinId)]
 #[case(
     "(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} (-1 )",
-    ErrorCode::NegativeAmount
+    ErrorCode::CoinAmountNegative
 )]
 #[case(
     "(66 (0x08 ({msg1} ) ((67 (0x08 ({msg1} )",
     ErrorCode::InvalidCondition
 )]
 #[case(
     "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} )",
-    ErrorCode::NegativeAmount
+    ErrorCode::CoinAmountNegative
 )]
 #[case(
     "(66 (0x01 ({msg1} ) ((67 (0x01 ({msg1} )",
     ErrorCode::InvalidCondition
 )]
 #[case(
     "(66 (0x02 ({msg1} ({msg2} ) ((67 (0x02 ({msg1} )",
@@ -4921,19 +4921,19 @@
 #[case(
     "(66 (0x01 ({msg1} (0x00 ) ((67 (0x01 ({msg1} (123 )",
     ErrorCode::InvalidCoinAmount
 )]
 // coin amounts can't be negative
 #[case(
     "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} (123 )",
-    ErrorCode::NegativeAmount
+    ErrorCode::CoinAmountNegative
 )]
 #[case(
     "(66 (0x01 ({msg1} (-1 ) ((67 (0x01 ({msg1} (123 )",
-    ErrorCode::NegativeAmount
+    ErrorCode::CoinAmountNegative
 )]
 fn test_message_conditions_failures(#[case] test_case: &str, #[case] expect: ErrorCode) {
     for flags in [ENABLE_MESSAGE_CONDITIONS, MEMPOOL_MODE] {
         let ret = cond_test_flag(&format!("((({{h1}} ({{h2}} (123 (({test_case}))))"), flags);
 
         let Err(ValidationErr(_, code)) = ret else {
             panic!("expected failure: {expect:?}");
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/flags.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/flags.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::gen::validation_error::{atom, check_nil, first, next, rest, ErrorCode, ValidationErr};
-use ::chik_protocol::bytes::Bytes32;
+use chik_protocol::Bytes32;
 use klvm_utils::tree_hash;
 use klvmr::allocator::{Allocator, Atom, NodePtr};
 use klvmr::op_utils::u64_from_bytes;
 
 // returns parent-coin ID, amount, puzzle-reveal and solution
 pub fn parse_coin_spend(
     a: &Allocator,
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/messages.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/messages.rs`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,18 @@
             NodePtr::NIL
         };
 
         let amount = if (mode & AMOUNT) != 0 {
             let amount = match sanitize_uint(a, first(a, *args)?, 8, ErrorCode::InvalidCoinAmount)?
             {
                 SanitizedUint::PositiveOverflow => {
-                    return Err(ValidationErr(*args, ErrorCode::AmountExceedsMaximum));
+                    return Err(ValidationErr(*args, ErrorCode::CoinAmountExceedsMaximum));
                 }
                 SanitizedUint::NegativeOverflow => {
-                    return Err(ValidationErr(*args, ErrorCode::NegativeAmount));
+                    return Err(ValidationErr(*args, ErrorCode::CoinAmountNegative));
                 }
                 SanitizedUint::Ok(amount) => amount,
             };
             *args = rest(a, *args)?;
             amount
         } else {
             0
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/opcodes.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/opcodes.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/run_block_generator.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/run_block_generator.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/run_puzzle.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/run_puzzle.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::gen::conditions::{parse_conditions, ParseState, Spend, SpendBundleConditions};
 use crate::gen::flags::ALLOW_BACKREFS;
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::ValidationErr;
-use chik_protocol::bytes::Bytes32;
-use chik_protocol::coin::Coin;
+use chik_protocol::Bytes32;
+use chik_protocol::Coin;
 use klvm_utils::tree_hash;
 use klvmr::allocator::Allocator;
 use klvmr::chik_dialect::ChikDialect;
 use klvmr::reduction::Reduction;
 use klvmr::run_program::run_program;
 use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
 use std::sync::Arc;
```

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/sanitize_int.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/solution_generator.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/solution_generator.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/gen/test_generators.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/gen/test_generators.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-consensus/src/generator_rom.rs` & `chik_rs-0.7.0/crates/chik-consensus/src/generator_rom.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/Cargo.toml` & `chik_rs-0.7.0/crates/chik-protocol/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chik-protocol"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik network protocol message types"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
@@ -12,20 +12,20 @@
 py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro", "chik-traits/py-bindings", "chik-bls/py-bindings"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods", "num-bigint"], optional = true }
 sha2 = "0.10.8"
 hex = "0.4.3"
 chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
-chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
+chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
 klvmr = "0.6.1"
-chik-traits = { version = "0.6.0", path = "../chik-traits" }
-klvm-traits = { version = "0.6.0", path = "../klvm-traits", features = ["derive"] }
-klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
-chik-bls = { version = "0.6.0", path = "../chik-bls" }
+chik-traits = { version = "0.7.0", path = "../chik-traits" }
+klvm-traits = { version = "0.7.0", path = "../klvm-traits", features = ["derive"] }
+klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
+chik-bls = { version = "0.7.0", path = "../chik-bls" }
 arbitrary = { version = "1.3.0", features = ["derive"] }
 
 [dev-dependencies]
 rstest = "0.17.0"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/block_record.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/block_record.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/bytes.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/bytes.rs`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     }
 }
 
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> ChikToPython for BytesImpl<N> {
     fn to_python<'a>(&self, py: Python<'a>) -> PyResult<&'a PyAny> {
         if N == 32 {
-            let bytes_module = PyModule::import(py, "chik.types.blockchain_format.sized_bytes")?;
+            let bytes_module = PyModule::import(py, "chik_rs.sized_bytes")?;
             let ty = bytes_module.getattr("bytes32")?;
             ty.call1((self.0.into_py(py),))
         } else {
             Ok(PyBytes::new(py, &self.0).into())
         }
     }
 }
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/chik_protocol.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/chik_protocol.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/classgroup.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/classgroup.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 use crate::Bytes100;
 use chik_streamable_macro::streamable;
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
 #[streamable]
+#[derive(Copy)]
 pub struct ClassgroupElement {
     data: Bytes100,
 }
 
-impl ClassgroupElement {
-    pub fn get_default_element() -> ClassgroupElement {
+impl Default for ClassgroupElement {
+    fn default() -> Self {
         let mut data = [0_u8; 100];
         data[0] = 0x08;
-        ClassgroupElement { data: data.into() }
+        Self { data: data.into() }
     }
+}
 
-    pub fn get_size() -> i32 {
-        100
-    }
+impl ClassgroupElement {
+    pub const SIZE: usize = 100;
 }
 
 #[cfg(feature = "py-bindings")]
 #[pymethods]
 impl ClassgroupElement {
     #[staticmethod]
     pub fn create(bytes: &[u8]) -> ClassgroupElement {
@@ -37,16 +38,16 @@
             ClassgroupElement { data: data.into() }
         }
     }
 
     #[staticmethod]
     #[pyo3(name = "get_default_element")]
     pub fn py_get_default_element() -> ClassgroupElement {
-        Self::get_default_element()
+        Self::default()
     }
 
     #[staticmethod]
     #[pyo3(name = "get_size")]
     pub fn py_get_size() -> i32 {
-        Self::get_size()
+        Self::SIZE as i32
     }
 }
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/coin.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/coin.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{bytes::Bytes32, BytesImpl};
+use crate::{Bytes32, BytesImpl};
 use chik_streamable_macro::streamable;
 use klvm_traits::{
     destructure_list, klvm_list, match_list, FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder,
     ToKlvm, ToKlvmError,
 };
 use sha2::{Digest, Sha256};
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/fee_estimate.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/foliage.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/full_node_protocol.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/full_node_protocol.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/fullblock.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/fullblock.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/header_block.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/header_block.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use chik_streamable_macro::streamable;
 
+use crate::unfinished_header_block::UnfinishedHeaderBlock;
 use crate::Bytes;
 use crate::Bytes32;
 use crate::EndOfSubSlotBundle;
 use crate::RewardChainBlock;
 use crate::VDFProof;
 use crate::{Foliage, FoliageTransactionBlock, TransactionsInfo};
 use chik_traits::Streamable;
@@ -68,14 +69,26 @@
     pub fn is_transaction_block(&self) -> bool {
         self.reward_chain_block.is_transaction_block
     }
 
     pub fn first_in_sub_slot(&self) -> bool {
         !self.finished_sub_slots.is_empty()
     }
+
+    pub fn into_unfinished_header_block(self) -> UnfinishedHeaderBlock {
+        UnfinishedHeaderBlock {
+            finished_sub_slots: self.finished_sub_slots,
+            reward_chain_block: self.reward_chain_block.get_unfinished(),
+            challenge_chain_sp_proof: self.challenge_chain_sp_proof,
+            reward_chain_sp_proof: self.reward_chain_sp_proof,
+            foliage: self.foliage,
+            foliage_transaction_block: self.foliage_transaction_block,
+            transactions_filter: self.transactions_filter,
+        }
+    }
 }
 
 #[cfg(feature = "py-bindings")]
 use chik_traits::ChikToPython;
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/lazy_node.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/lazy_node.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/lib.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-pub mod block_record;
-pub mod bytes;
-pub mod chik_protocol;
-pub mod classgroup;
-pub mod coin;
-pub mod coin_spend;
-pub mod coin_state;
-pub mod end_of_sub_slot_bundle;
-pub mod fee_estimate;
-pub mod foliage;
-pub mod full_node_protocol;
-pub mod fullblock;
-pub mod header_block;
-pub mod peer_info;
-pub mod pool_target;
-pub mod program;
-pub mod proof_of_space;
-pub mod reward_chain_block;
-pub mod slots;
-pub mod spend_bundle;
-pub mod sub_epoch_summary;
-pub mod unfinished_block;
-pub mod vdf;
-pub mod wallet_protocol;
-pub mod weight_proof;
+mod block_record;
+mod bytes;
+mod chik_protocol;
+mod classgroup;
+mod coin;
+mod coin_spend;
+mod coin_state;
+mod end_of_sub_slot_bundle;
+mod fee_estimate;
+mod foliage;
+mod full_node_protocol;
+mod fullblock;
+mod header_block;
+mod peer_info;
+mod pool_target;
+mod program;
+mod proof_of_space;
+mod reward_chain_block;
+mod slots;
+mod spend_bundle;
+mod sub_epoch_summary;
+mod unfinished_block;
+mod unfinished_header_block;
+mod vdf;
+mod wallet_protocol;
+mod weight_proof;
 
 #[cfg(feature = "py-bindings")]
-pub mod lazy_node;
+mod lazy_node;
 
 // export shorter names
 pub use crate::block_record::*;
 pub use crate::bytes::*;
 pub use crate::chik_protocol::*;
 pub use crate::classgroup::*;
 pub use crate::coin::*;
```

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/program.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/reward_chain_block.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/slots.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/spend_bundle.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/spend_bundle.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/unfinished_block.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/unfinished_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/wallet_protocol.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/wallet_protocol.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-protocol/src/weight_proof.rs` & `chik_rs-0.7.0/crates/chik-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik_py_streamable_macro/src/lib.rs` & `chik_rs-0.7.0/crates/chik_py_streamable_macro/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 extern crate proc_macro;
 
 use proc_macro2::{Ident, Span};
 use proc_macro_crate::{crate_name, FoundCrate};
 use quote::quote;
 use syn::{parse_macro_input, DeriveInput, FieldsNamed, FieldsUnnamed};
 
-#[proc_macro_derive(PyStreamable)]
+fn maybe_upper_fields(py_uppercase: bool, fnames: Vec<syn::Ident>) -> Vec<syn::Ident> {
+    if py_uppercase {
+        fnames
+            .into_iter()
+            .map(|f| syn::Ident::new(&f.to_string().to_uppercase(), Span::call_site()))
+            .collect()
+    } else {
+        fnames
+    }
+}
+
+#[proc_macro_derive(PyStreamable, attributes(py_uppercase, py_pickle))]
 pub fn py_streamable_macro(input: proc_macro::TokenStream) -> proc_macro::TokenStream {
     let found_crate = crate_name("chik-traits").expect("chik-traits is present in `Cargo.toml`");
 
     let crate_name = match found_crate {
         FoundCrate::Itself => quote!(crate),
         FoundCrate::Name(name) => {
             let ident = Ident::new(&name, Span::call_site());
             quote!(#ident)
         }
     };
 
-    let DeriveInput { ident, data, .. } = parse_macro_input!(input);
+    let DeriveInput {
+        ident, data, attrs, ..
+    } = parse_macro_input!(input);
+
+    let mut py_uppercase = false;
+    let mut py_pickle = false;
+    for attr in attrs.iter() {
+        if attr.path().is_ident("py_uppercase") {
+            py_uppercase = true;
+        } else if attr.path().is_ident("py_pickle") {
+            py_pickle = true;
+        }
+    }
 
     let fields = match data {
         syn::Data::Struct(s) => s.fields,
         syn::Data::Enum(_) => {
             return quote! {
                 impl<'a> pyo3::conversion::FromPyObject<'a> for #ident {
                     fn extract(ob: &'a pyo3::PyAny) -> pyo3::PyResult<Self> {
@@ -76,31 +99,34 @@
         impl #crate_name::ChikToPython for #ident {
             fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
                 Ok(pyo3::IntoPy::into_py(self.clone(), py).into_ref(py))
             }
         }
     };
 
+    let mut fnames = Vec::<syn::Ident>::new();
+    let mut ftypes = Vec::<syn::Type>::new();
+
     match fields {
         syn::Fields::Named(FieldsNamed { named, .. }) => {
-            let mut fnames = Vec::<syn::Ident>::new();
-            let mut ftypes = Vec::<syn::Type>::new();
             for f in named.iter() {
                 fnames.push(f.ident.as_ref().unwrap().clone());
                 ftypes.push(f.ty.clone());
             }
 
+            let fnames_maybe_upper = maybe_upper_fields(py_uppercase, fnames.clone());
+
             py_protocol.extend(quote! {
                 #[pyo3::pymethods]
                 impl #ident {
                     #[allow(too_many_arguments)]
                     #[new]
-                    #[pyo3(signature = (#(#fnames),*))]
-                    pub fn py_new ( #(#fnames : #ftypes),* ) -> Self {
-                        Self { #(#fnames),* }
+                    #[pyo3(signature = (#(#fnames_maybe_upper),*))]
+                    pub fn py_new ( #(#fnames_maybe_upper : #ftypes),* ) -> Self {
+                        Self { #(#fnames: #fnames_maybe_upper),* }
                     }
                 }
             });
 
             py_protocol.extend(quote! {
                 #[pyo3::pymethods]
                 impl #ident {
@@ -108,15 +134,15 @@
                     fn replace(&self, kwargs: Option<&pyo3::types::PyDict>) -> pyo3::PyResult<Self> {
                         let mut ret = self.clone();
                         if let Some(kwargs) = kwargs {
                             let iter: pyo3::types::iter::PyDictIterator = kwargs.iter();
                             for (field, value) in iter {
                                 let field = field.extract::<String>()?;
                                 match field.as_str() {
-                                    #(stringify!(#fnames) => {
+                                    #(stringify!(#fnames_maybe_upper) => {
                                         ret.#fnames = value.extract()?;
                                     }),*
                                     _ => { return Err(pyo3::exceptions::PyKeyError::new_err(format!("unknown field {field}"))); }
                                 }
                             }
                         }
                         Ok(ret)
@@ -216,30 +242,72 @@
 
             pub fn __copy__<'p>(&self) -> pyo3::PyResult<Self> {
                 Ok(self.clone())
             }
         }
     };
     py_protocol.extend(streamable);
+
+    if py_pickle {
+        let pickle = quote! {
+            #[pyo3::pymethods]
+            impl #ident {
+                pub fn __setstate__(
+                    &mut self,
+                    state: &pyo3::types::PyBytes,
+                ) -> pyo3::PyResult<()> {
+                    use chik_traits::Streamable;
+
+                    *self = Self::parse::<true>(&mut std::io::Cursor::new(state.as_bytes()))?;
+
+                    Ok(())
+                }
+
+                pub fn __getstate__<'py>(
+                    &self,
+                    py: pyo3::Python<'py>,
+                ) -> pyo3::PyResult<&'py pyo3::types::PyBytes> {
+                    self.py_to_bytes(py)
+                }
+
+                pub fn __getnewargs__<'py>(&self, py: pyo3::Python<'py>) -> pyo3::PyResult<&'py pyo3::types::PyTuple> {
+                    let mut args = Vec::new();
+                    #( args.push(#crate_name::ChikToPython::to_python(&self.#fnames, py)?); )*
+                    Ok(pyo3::types::PyTuple::new(py, args))
+                }
+            }
+        };
+        py_protocol.extend(pickle);
+    }
+
     py_protocol.into()
 }
 
-#[proc_macro_derive(PyJsonDict)]
+#[proc_macro_derive(PyJsonDict, attributes(py_uppercase))]
 pub fn py_json_dict_macro(input: proc_macro::TokenStream) -> proc_macro::TokenStream {
     let found_crate = crate_name("chik-traits").expect("chik-traits is present in `Cargo.toml`");
 
     let crate_name = match found_crate {
         FoundCrate::Itself => quote!(crate),
         FoundCrate::Name(name) => {
             let ident = Ident::new(&name, Span::call_site());
             quote!(#ident)
         }
     };
 
-    let DeriveInput { ident, data, .. } = parse_macro_input!(input);
+    let DeriveInput {
+        ident, data, attrs, ..
+    } = parse_macro_input!(input);
+
+    let mut py_uppercase = false;
+    for attr in attrs.iter() {
+        if attr.path().is_ident("py_uppercase") {
+            py_uppercase = true;
+        }
+    }
 
     let fields = match data {
         syn::Data::Struct(s) => s.fields,
         syn::Data::Enum(_) => {
             return quote! {
                 impl #crate_name::to_json_dict::ToJsonDict for #ident {
                     fn to_json_dict(&self, py: pyo3::Python) -> pyo3::PyResult<pyo3::PyObject> {
@@ -268,44 +336,55 @@
             let mut fnames = Vec::<syn::Ident>::new();
             let mut ftypes = Vec::<syn::Type>::new();
             for f in named.iter() {
                 fnames.push(f.ident.as_ref().unwrap().clone());
                 ftypes.push(f.ty.clone());
             }
 
+            let fnames_maybe_upper = maybe_upper_fields(py_uppercase, fnames.clone());
+
             py_protocol.extend( quote! {
 
                 impl #crate_name::to_json_dict::ToJsonDict for #ident {
                     fn to_json_dict(&self, py: pyo3::Python) -> pyo3::PyResult<pyo3::PyObject> {
                         let ret = pyo3::types::PyDict::new(py);
-                        #(ret.set_item(stringify!(#fnames), self.#fnames.to_json_dict(py)?)?);*;
+                        #(ret.set_item(stringify!(#fnames_maybe_upper), self.#fnames.to_json_dict(py)?)?);*;
                         Ok(ret.into())
                     }
                 }
 
                 impl #crate_name::from_json_dict::FromJsonDict for #ident {
                     fn from_json_dict(o: &pyo3::PyAny) -> pyo3::PyResult<Self> {
                         Ok(Self{
-                            #(#fnames: <#ftypes as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(o.get_item(stringify!(#fnames))?)?,)*
+                            #(#fnames: <#ftypes as #crate_name::from_json_dict::FromJsonDict>::from_json_dict(o.get_item(stringify!(#fnames_maybe_upper))?)?,)*
                         })
                     }
                 }
             });
         }
         _ => {
             panic!("PyJsonDict only supports structs");
         }
     }
 
     py_protocol.into()
 }
 
-#[proc_macro_derive(PyGetters)]
+#[proc_macro_derive(PyGetters, attributes(py_uppercase))]
 pub fn py_getters_macro(input: proc_macro::TokenStream) -> proc_macro::TokenStream {
-    let DeriveInput { ident, data, .. } = parse_macro_input!(input);
+    let DeriveInput {
+        ident, data, attrs, ..
+    } = parse_macro_input!(input);
+
+    let mut py_uppercase = false;
+    for attr in attrs.iter() {
+        if attr.path().is_ident("py_uppercase") {
+            py_uppercase = true;
+        }
+    }
 
     let syn::Data::Struct(s) = data else {
         panic!("python binding only support struct");
     };
 
     let syn::Fields::Named(FieldsNamed { named, .. }) = s.fields else {
         panic!("python binding only support struct");
@@ -324,20 +403,22 @@
     let mut fnames = Vec::<syn::Ident>::new();
     let mut ftypes = Vec::<syn::Type>::new();
     for f in named.into_iter() {
         fnames.push(f.ident.unwrap());
         ftypes.push(f.ty);
     }
 
+    let fnames_maybe_upper = maybe_upper_fields(py_uppercase, fnames.clone());
+
     let ret = quote! {
         #[pyo3::pymethods]
         impl #ident {
             #(
             #[getter]
-            fn #fnames<'a> (&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
+            fn #fnames_maybe_upper<'a> (&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
                 #crate_name::ChikToPython::to_python(&self.#fnames, py)
             }
             )*
         }
     };
 
     ret.into()
```

### Comparing `chik_rs-0.6.1/crates/chik-bls/Cargo.toml` & `chik_rs-0.7.0/crates/chik-bls/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "chik-bls"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "BLS signature, verification and aggregation funcions for the Chik blockchain"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "chik_py_streamable_macro", "chik-traits/py-bindings"]
 
 [dependencies]
-chik-traits = { version = "0.6.0", path = "../chik-traits" }
-chik_py_streamable_macro = { version = "0.6.0", path = "../chik_py_streamable_macro", optional = true }
+chik-traits = { version = "0.7.0", path = "../chik-traits" }
+chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
 tiny-bip39 = "1.0.0"
 anyhow = "1.0.71"
 sha2 = "0.10.8"
 hkdf = "0.12.0"
 blst = { version = "0.3.11", git = "https://github.com/supranational/blst.git", rev = "0d46eefa45fc1e57aceb42bba0e84eab3a7a9725", features = ["portable"] }
 hex = "0.4.3"
 thiserror = "1.0.44"
```

### Comparing `chik_rs-0.6.1/crates/chik-bls/README.md` & `chik_rs-0.7.0/crates/chik-bls/README.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/benches/derive_key.rs` & `chik_rs-0.7.0/crates/chik-bls/benches/derive_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/benches/parse.rs` & `chik_rs-0.7.0/crates/chik-bls/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/benches/sign.rs` & `chik_rs-0.7.0/crates/chik-bls/benches/sign.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/benches/verify.rs` & `chik_rs-0.7.0/crates/chik-bls/benches/verify.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/derive_keys.rs` & `chik_rs-0.7.0/crates/chik-bls/src/derive_keys.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/error.rs` & `chik_rs-0.7.0/crates/chik-bls/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/gtelement.rs` & `chik_rs-0.7.0/crates/chik-bls/src/gtelement.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/lib.rs` & `chik_rs-0.7.0/crates/chik-bls/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/mnemonic.rs` & `chik_rs-0.7.0/crates/chik-bls/src/mnemonic.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/public_key.rs` & `chik_rs-0.7.0/crates/chik-bls/src/public_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/secret_key.rs` & `chik_rs-0.7.0/crates/chik-bls/src/secret_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-bls/src/signature.rs` & `chik_rs-0.7.0/crates/chik-bls/src/signature.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/Cargo.toml` & `chik_rs-0.7.0/crates/klvm-traits/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "klvm-traits"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Traits for encoding and decoding KLVM objects."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
@@ -16,14 +16,14 @@
 chik-bls = ["dep:chik-bls"]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
 pyo3 = { version = ">=0.19.0", optional = true }
 klvmr = "0.6.1"
 klvm-derive = { version = "0.6.0", path = "../klvm-derive", optional = true }
-chik-bls = { version = "0.6.0", path = "../chik-bls", optional = true }
+chik-bls = { version = "0.7.0", path = "../chik-bls", optional = true }
 num-bigint = "0.4.3"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 hex = "0.4.3"
 hex-literal = "0.4.1"
```

### Comparing `chik_rs-0.6.1/crates/klvm-traits/docs/derive_macros.md` & `chik_rs-0.7.0/crates/klvm-traits/docs/derive_macros.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/error.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/from_klvm.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/from_klvm.rs`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,27 @@
 klvm_primitive!(u64);
 klvm_primitive!(i64);
 klvm_primitive!(u128);
 klvm_primitive!(i128);
 klvm_primitive!(usize);
 klvm_primitive!(isize);
 
+impl<N> FromKlvm<N> for bool {
+    fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
+        let atom = decoder.decode_atom(&node)?;
+        match atom.as_ref() {
+            [] => Ok(false),
+            [1] => Ok(true),
+            _ => Err(FromKlvmError::Custom(
+                "expected boolean value of either `()` or `1`".to_string(),
+            )),
+        }
+    }
+}
+
 impl<N, A, B> FromKlvm<N> for (A, B)
 where
     A: FromKlvm<N>,
     B: FromKlvm<N>,
 {
     fn from_klvm(decoder: &impl KlvmDecoder<Node = N>, node: N) -> Result<Self, FromKlvmError> {
         let (first, rest) = decoder.decode_pair(&node)?;
@@ -208,14 +221,27 @@
         assert_eq!(decode(a, "05"), Ok(5i32));
         assert_eq!(decode(a, "81e5"), Ok(-27i32));
         assert_eq!(decode(a, "80"), Ok(-0));
         assert_eq!(decode(a, "8180"), Ok(-128i8));
     }
 
     #[test]
+    fn test_bool() {
+        let a = &mut Allocator::new();
+        assert_eq!(decode(a, "80"), Ok(false));
+        assert_eq!(decode(a, "01"), Ok(true));
+        assert_eq!(
+            decode::<bool>(a, "05"),
+            Err(FromKlvmError::Custom(
+                "expected boolean value of either `()` or `1`".to_string(),
+            ))
+        )
+    }
+
+    #[test]
     fn test_pair() {
         let a = &mut Allocator::new();
         assert_eq!(decode(a, "ff0502"), Ok((5, 2)));
         assert_eq!(decode(a, "ff81b8ff8301600980"), Ok((-72, (90121, ()))));
         assert_eq!(
             decode(a, "ffff80ff80ff80ffff80ff80ff80808080"),
             Ok((((), ((), ((), (((), ((), ((), ()))), ())))), ()))
```

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/klvm_decoder.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/klvm_decoder.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/klvm_encoder.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/klvm_encoder.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/lib.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/macros.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/match_byte.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/match_byte.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/to_klvm.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/to_klvm.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 klvm_primitive!(u64);
 klvm_primitive!(i64);
 klvm_primitive!(u128);
 klvm_primitive!(i128);
 klvm_primitive!(usize);
 klvm_primitive!(isize);
 
+impl<N> ToKlvm<N> for bool {
+    fn to_klvm(&self, encoder: &mut impl KlvmEncoder<Node = N>) -> Result<N, ToKlvmError> {
+        (if *self { 1 } else { 0 }).to_klvm(encoder)
+    }
+}
+
 impl<N, T> ToKlvm<N> for &T
 where
     T: ToKlvm<N>,
 {
     fn to_klvm(&self, encoder: &mut impl KlvmEncoder<Node = N>) -> Result<N, ToKlvmError> {
         T::to_klvm(*self, encoder)
     }
@@ -170,14 +176,21 @@
         assert_eq!(encode(a, 5i32), Ok("05".to_owned()));
         assert_eq!(encode(a, -27i32), Ok("81e5".to_owned()));
         assert_eq!(encode(a, -0), Ok("80".to_owned()));
         assert_eq!(encode(a, -128i8), Ok("8180".to_owned()));
     }
 
     #[test]
+    fn test_bool() {
+        let a = &mut Allocator::new();
+        assert_eq!(encode(a, true), Ok("01".to_owned()));
+        assert_eq!(encode(a, false), Ok("80".to_owned()));
+    }
+
+    #[test]
     fn test_reference() {
         let a = &mut Allocator::new();
         assert_eq!(encode(a, [1, 2, 3]), encode(a, [1, 2, 3]));
         assert_eq!(encode(a, Some(42)), encode(a, Some(42)));
         assert_eq!(encode(a, Some(&42)), encode(a, Some(42)));
         assert_eq!(encode(a, Some(&42)), encode(a, Some(42)));
     }
```

### Comparing `chik_rs-0.6.1/crates/klvm-traits/src/wrappers.rs` & `chik_rs-0.7.0/crates/klvm-traits/src/wrappers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/Cargo.toml` & `chik_rs-0.7.0/crates/chik-wallet/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [package]
 name = "chik-wallet"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik primitives needed for building wallets."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [dependencies]
 klvmr = "0.6.1"
 sha2 = "0.10.8"
 num-bigint = "0.4.3"
 hex-literal = "0.4.1"
-klvm-utils = { version = "0.6.0", path = "../klvm-utils" }
-klvm-traits = { version = "0.6.0", path = "../klvm-traits", features = ["chik-bls"] }
-chik-bls = { version = "0.6.0", path = "../chik-bls" }
-chik-protocol = { version = "0.6.0", path = "../chik-protocol" }
+klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
+klvm-traits = { version = "0.7.0", path = "../klvm-traits", features = ["chik-bls"] }
+chik-bls = { version = "0.7.0", path = "../chik-bls" }
+chik-protocol = { version = "0.7.0", path = "../chik-protocol" }
 arbitrary = "1.3.0"
 
 [dev-dependencies]
 hex = "0.4.3"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/derive_synthetic.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/derive_synthetic.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/proof.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/proof.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/cat.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/cat.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/did.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/did.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/nft.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/nft.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/offer.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/offer.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/singleton.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/singleton.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik-wallet/src/puzzles/standard.rs` & `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/standard.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik_streamable_macro/Cargo.toml` & `chik_rs-0.7.0/crates/chik_streamable_macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/chik_streamable_macro/src/lib.rs` & `chik_rs-0.7.0/crates/chik_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-utils/src/curried_program.rs` & `chik_rs-0.7.0/crates/klvm-utils/src/curried_program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-utils/src/curry_tree_hash.rs` & `chik_rs-0.7.0/crates/klvm-utils/src/curry_tree_hash.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-utils/src/lib.rs` & `chik_rs-0.7.0/crates/klvm-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/crates/klvm-utils/src/tree_hash.rs` & `chik_rs-0.7.0/crates/klvm-utils/src/tree_hash.rs`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         node_from_bytes_backrefs, node_from_bytes_backrefs_record, node_to_bytes_backrefs,
     };
     use std::fs::read_to_string;
 
     let filename = format!("../../generator-tests/{name}.txt");
     println!("file: {filename}",);
     let test_file = read_to_string(filename).expect("test file not found");
-    let (generator, _) = test_file.split_once('\n').expect("invalid test file");
+    let generator = test_file.lines().next().expect("invalid test file");
     let generator = hex::decode(generator).expect("invalid hex encoded generator");
 
     let generator = if compressed {
         let mut a = Allocator::new();
         let node = node_from_bytes_backrefs(&mut a, &generator).expect("node_from_bytes_backrefs");
         node_to_bytes_backrefs(&a, node).expect("node_to_bytes_backrefs")
     } else {
```

### Comparing `chik_rs-0.6.1/wheel/Cargo.toml` & `chik_rs-0.7.0/wheel/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chik_rs"
-version = "0.6.1"
+version = "0.7.0"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Code useful for implementing chik consensus."
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 readme = "README.md"
@@ -15,15 +15,15 @@
 path = "src/lib.rs"
 
 [dependencies]
 klvmr = "0.6.1"
 hex = "0.4.3"
 sha2 = "0.10.8"
 pyo3 = { version = "=0.19.0", features = ["multiple-pymethods"] }
-chik-consensus = { version = "=0.6.1", path = "../crates/chik-consensus", features = ["py-bindings"] }
-chik-bls = { version = "=0.6.0", path = "../crates/chik-bls", features = ["py-bindings"]  }
-chik-protocol = { version = "=0.6.0", path = "../crates/chik-protocol", features = ["py-bindings"]  }
-chik-traits = { version = "=0.6.0", path = "../crates/chik-traits", features = ["py-bindings"]  }
-klvm-traits = { version = "=0.6.0", path = "../crates/klvm-traits", features = ["derive", "py-bindings"] }
-klvm-utils = { version = "=0.6.0", path = "../crates/klvm-utils" }
-chik_py_streamable_macro = { version = "=0.6.0", path = "../crates/chik_py_streamable_macro" }
+chik-consensus = { version = "0.7.0", path = "../crates/chik-consensus", features = ["py-bindings"] }
+chik-bls = { version = "0.7.0", path = "../crates/chik-bls", features = ["py-bindings"]  }
+chik-protocol = { version = "0.7.0", path = "../crates/chik-protocol", features = ["py-bindings"]  }
+chik-traits = { version = "0.7.0", path = "../crates/chik-traits", features = ["py-bindings"]  }
+klvm-traits = { version = "0.7.0", path = "../crates/klvm-traits", features = ["derive", "py-bindings"] }
+klvm-utils = { version = "0.7.0", path = "../crates/klvm-utils" }
+chik_py_streamable_macro = { version = "0.7.0", path = "../crates/chik_py_streamable_macro" }
 chik_streamable_macro = { version = "=0.6.0", path = "../crates/chik_streamable_macro" }
```

### Comparing `chik_rs-0.6.1/wheel/chik_rs.pyi` & `chik_rs-0.7.0/wheel/python/chik_rs/chik_rs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 #
 # this file is generated by generate_type_stubs.py
 #
 
-from typing import List, Optional, Sequence, Tuple
-from chik.types.blockchain_format.sized_bytes import bytes32
-from chik.util.ints import uint8, uint16, uint32, uint64, uint128, int8, int16, int32, int64, int128
+from typing import List, Optional, Sequence, Tuple, Union, Dict, Any, ClassVar
+from .sized_bytes import bytes32, bytes100
+from .sized_ints import uint8, uint16, uint32, uint64, uint128, int8, int16, int32, int64
 from chik.types.blockchain_format.program import Program as ChikProgram
-from chik.consensus.constants import ConsensusConstants
 
 ReadableBuffer = Union[bytes, bytearray, memoryview]
 
 class _Unspec:
     pass
 
 def solution_generator(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
@@ -30,14 +29,30 @@
     program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
+def deserialize_proof(
+    proof: bytes
+) -> MerkleSet: ...
+
+def confirm_included_already_hashed(
+    root: bytes32,
+    item: bytes32,
+    proof: bytes,
+) -> bool: ...
+
+def confirm_not_included_already_hashed(
+    root: bytes32,
+    item: bytes32,
+    proof: bytes,
+) -> bool: ...
+
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
 ENABLE_MESSAGE_CONDITIONS: int = ...
@@ -52,27 +67,27 @@
 ELIGIBLE_FOR_DEDUP: int = ...
 ELIGIBLE_FOR_FF: int = ...
 
 NO_UNKNOWN_OPS: int = ...
 
 def run_chik_program(
     program: bytes, args: bytes, max_cost: int, flags: int
-) -> Pair[int, LazyNode]: ...
+) -> Tuple[int, LazyNode]: ...
 
 class LazyNode:
-    def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
-    def atom() -> bytes: ...
+    pair: Optional[Tuple[LazyNode, LazyNode]]
+    atom: Optional[bytes]
 
 def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class AugSchemeMPL:
     @staticmethod
-    def sign(pk: PrivateKey, msg: bytes, prepend_pk: G1Element = None) -> G2Element: ...
+    def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
     def verify(pk: G1Element, msg: bytes, sig: G2Element) -> bool: ...
     @staticmethod
     def aggregate_verify(pks: Sequence[G1Element], msgs: Sequence[bytes], sig: G2Element) -> bool: ...
     @staticmethod
@@ -82,25 +97,30 @@
     @staticmethod
     def derive_child_sk(pk: PrivateKey, index: int) -> PrivateKey: ...
     @staticmethod
     def derive_child_sk_unhardened(pk: PrivateKey, index: int) -> PrivateKey: ...
     @staticmethod
     def derive_child_pk_unhardened(pk: G1Element, index: int) -> G1Element: ...
 
+class MerkleSet:
+    def get_root(self) -> bytes32: ...
+    def is_included_already_hashed(self, to_check: bytes) -> Tuple[bool, bytes]: ...
+    def __init__(
+        self,
+        leafs: List[bytes32],
+    ) -> None: ...
+
 class G1Element:
     SIZE: ClassVar[int] = ...
     def __new__(cls) -> G1Element: ...
     def get_fingerprint(self) -> int: ...
     def pair(self, other: G2Element) -> GTElement: ...
     @staticmethod
-    def from_bytes_unchecked(b: bytes) -> G1Element: ...
-    @staticmethod
     def generator() -> G1Element: ...
     def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
     def __add__(self, other: G1Element) -> G1Element: ...
     def __iadd__(self, other: G1Element) -> G1Element: ...
     def __init__(
         self
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
@@ -113,28 +133,25 @@
     def from_bytes_unchecked(bytes) -> G1Element: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[G1Element, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> G1Element: ...
+    def from_json_dict(json_dict: Any) -> G1Element: ...
 
 class G2Element:
     SIZE: ClassVar[int] = ...
     def __new__(cls) -> G2Element: ...
-    @staticmethod
-    def from_bytes_unchecked(b: bytes) -> G2Element: ...
     def pair(self, other: G1Element) -> GTElement: ...
     @staticmethod
     def generator() -> G2Element: ...
     def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
     def __add__(self, other: G2Element) -> G2Element: ...
     def __iadd__(self, other: G2Element) -> G2Element: ...
     def __init__(
         self
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
@@ -147,24 +164,21 @@
     def from_bytes_unchecked(bytes) -> G2Element: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[G2Element, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> G2Element: ...
+    def from_json_dict(json_dict: Any) -> G2Element: ...
 
 class GTElement:
     SIZE: ClassVar[int] = ...
-    @staticmethod
-    def from_bytes_unchecked(b: bytes) -> GTElement: ...
     def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
     def __mul__(self, rhs: GTElement) -> GTElement: ...
     def __imul__(self, rhs: GTElement) -> GTElement : ...
     def __init__(
         self
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
@@ -177,24 +191,23 @@
     def from_bytes_unchecked(bytes) -> GTElement: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[GTElement, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> GTElement: ...
+    def from_json_dict(json_dict: Any) -> GTElement: ...
 
 class PrivateKey:
     PRIVATE_KEY_SIZE: ClassVar[int] = ...
     def sign_g2(self, msg: bytes, dst: bytes) -> G2Element: ...
     def get_g1(self) -> G1Element: ...
     def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
     def __init__(
         self
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> PrivateKey: ...
@@ -205,17 +218,17 @@
     def from_bytes_unchecked(bytes) -> PrivateKey: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[PrivateKey, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> PrivateKey: ...
+    def from_json_dict(json_dict: Any) -> PrivateKey: ...
 
 class Spend:
     coin_id: bytes
     parent_id: bytes
     puzzle_hash: bytes
     coin_amount: int
     height_relative: Optional[int]
@@ -266,17 +279,17 @@
     def from_bytes_unchecked(bytes) -> Spend: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Spend, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Spend: ...
+    def from_json_dict(json_dict: Any) -> Spend: ...
     def replace(self, *, coin_id: Union[ bytes, _Unspec] = _Unspec(),
         parent_id: Union[ bytes, _Unspec] = _Unspec(),
         puzzle_hash: Union[ bytes, _Unspec] = _Unspec(),
         coin_amount: Union[ int, _Unspec] = _Unspec(),
         height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         seconds_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         before_height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
@@ -328,17 +341,17 @@
     def from_bytes_unchecked(bytes) -> SpendBundleConditions: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SpendBundleConditions, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SpendBundleConditions: ...
+    def from_json_dict(json_dict: Any) -> SpendBundleConditions: ...
     def replace(self, *, spends: Union[ List[Spend], _Unspec] = _Unspec(),
         reserve_fee: Union[ int, _Unspec] = _Unspec(),
         height_absolute: Union[ int, _Unspec] = _Unspec(),
         seconds_absolute: Union[ int, _Unspec] = _Unspec(),
         before_height_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
         before_seconds_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
         agg_sig_unsafe: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
@@ -419,17 +432,17 @@
     def from_bytes_unchecked(bytes) -> BlockRecord: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[BlockRecord, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> BlockRecord: ...
+    def from_json_dict(json_dict: Any) -> BlockRecord: ...
     def replace(self, *, header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         prev_hash: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec(),
         weight: Union[ uint128, _Unspec] = _Unspec(),
         total_iters: Union[ uint128, _Unspec] = _Unspec(),
         signage_point_index: Union[ uint8, _Unspec] = _Unspec(),
         challenge_vdf_output: Union[ ClassgroupElement, _Unspec] = _Unspec(),
@@ -473,36 +486,36 @@
     def from_bytes_unchecked(bytes) -> Message: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Message, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Message: ...
+    def from_json_dict(json_dict: Any) -> Message: ...
     def replace(self, *, msg_type: Union[ int, _Unspec] = _Unspec(),
         id: Union[ Optional[uint16], _Unspec] = _Unspec(),
         data: Union[ bytes, _Unspec] = _Unspec()) -> Message: ...
 
 class Handshake:
-    network_id: String
-    protocol_version: String
-    software_version: String
+    network_id: str
+    protocol_version: str
+    software_version: str
     server_port: uint16
     node_type: int
-    capabilities: List[(uint16, String)]
+    capabilities: List[Tuple[uint16, str]]
     def __init__(
         self,
-        network_id: String,
-        protocol_version: String,
-        software_version: String,
+        network_id: str,
+        protocol_version: str,
+        software_version: str,
         server_port: uint16,
         node_type: int,
-        capabilities: Sequence[(uint16, String)]
+        capabilities: Sequence[Tuple[uint16, str]]
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> Handshake: ...
     def __copy__(self) -> Handshake: ...
     @staticmethod
@@ -511,23 +524,23 @@
     def from_bytes_unchecked(bytes) -> Handshake: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Handshake, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Handshake: ...
-    def replace(self, *, network_id: Union[ String, _Unspec] = _Unspec(),
-        protocol_version: Union[ String, _Unspec] = _Unspec(),
-        software_version: Union[ String, _Unspec] = _Unspec(),
+    def from_json_dict(json_dict: Any) -> Handshake: ...
+    def replace(self, *, network_id: Union[ str, _Unspec] = _Unspec(),
+        protocol_version: Union[ str, _Unspec] = _Unspec(),
+        software_version: Union[ str, _Unspec] = _Unspec(),
         server_port: Union[ uint16, _Unspec] = _Unspec(),
         node_type: Union[ int, _Unspec] = _Unspec(),
-        capabilities: Union[ List[(uint16, String)], _Unspec] = _Unspec()) -> Handshake: ...
+        capabilities: Union[ List[Tuple[uint16, str]], _Unspec] = _Unspec()) -> Handshake: ...
 
 class ClassgroupElement:
     data: bytes100
     @staticmethod
     def create(bytes) -> ClassgroupElement: ...
     @staticmethod
     def get_default_element() -> ClassgroupElement: ...
@@ -548,17 +561,17 @@
     def from_bytes_unchecked(bytes) -> ClassgroupElement: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[ClassgroupElement, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> ClassgroupElement: ...
+    def from_json_dict(json_dict: Any) -> ClassgroupElement: ...
     def replace(self, *, data: Union[ bytes100, _Unspec] = _Unspec()) -> ClassgroupElement: ...
 
 class Coin:
     parent_coin_info: bytes32
     puzzle_hash: bytes32
     amount: uint64
     def name(self) -> bytes32: ...
@@ -579,17 +592,17 @@
     def from_bytes_unchecked(bytes) -> Coin: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Coin, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Coin: ...
+    def from_json_dict(json_dict: Any) -> Coin: ...
     def replace(self, *, parent_coin_info: Union[ bytes32, _Unspec] = _Unspec(),
         puzzle_hash: Union[ bytes32, _Unspec] = _Unspec(),
         amount: Union[ uint64, _Unspec] = _Unspec()) -> Coin: ...
 
 class CoinSpend:
     coin: Coin
     puzzle_reveal: Program
@@ -611,17 +624,17 @@
     def from_bytes_unchecked(bytes) -> CoinSpend: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[CoinSpend, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> CoinSpend: ...
+    def from_json_dict(json_dict: Any) -> CoinSpend: ...
     def replace(self, *, coin: Union[ Coin, _Unspec] = _Unspec(),
         puzzle_reveal: Union[ Program, _Unspec] = _Unspec(),
         solution: Union[ Program, _Unspec] = _Unspec()) -> CoinSpend: ...
 
 class CoinState:
     coin: Coin
     spent_height: Optional[uint32]
@@ -643,17 +656,17 @@
     def from_bytes_unchecked(bytes) -> CoinState: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[CoinState, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> CoinState: ...
+    def from_json_dict(json_dict: Any) -> CoinState: ...
     def replace(self, *, coin: Union[ Coin, _Unspec] = _Unspec(),
         spent_height: Union[ Optional[uint32], _Unspec] = _Unspec(),
         created_height: Union[ Optional[uint32], _Unspec] = _Unspec()) -> CoinState: ...
 
 class EndOfSubSlotBundle:
     challenge_chain: ChallengeChainSubSlot
     infused_challenge_chain: Optional[InfusedChallengeChainSubSlot]
@@ -677,17 +690,17 @@
     def from_bytes_unchecked(bytes) -> EndOfSubSlotBundle: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[EndOfSubSlotBundle, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> EndOfSubSlotBundle: ...
+    def from_json_dict(json_dict: Any) -> EndOfSubSlotBundle: ...
     def replace(self, *, challenge_chain: Union[ ChallengeChainSubSlot, _Unspec] = _Unspec(),
         infused_challenge_chain: Union[ Optional[InfusedChallengeChainSubSlot], _Unspec] = _Unspec(),
         reward_chain: Union[ RewardChainSubSlot, _Unspec] = _Unspec(),
         proofs: Union[ SubSlotProofs, _Unspec] = _Unspec()) -> EndOfSubSlotBundle: ...
 
 class FeeRate:
     mojos_per_klvm_cost: uint64
@@ -706,26 +719,26 @@
     def from_bytes_unchecked(bytes) -> FeeRate: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FeeRate, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FeeRate: ...
+    def from_json_dict(json_dict: Any) -> FeeRate: ...
     def replace(self, *, mojos_per_klvm_cost: Union[ uint64, _Unspec] = _Unspec()) -> FeeRate: ...
 
 class FeeEstimate:
-    error: Optional[String]
+    error: Optional[str]
     time_target: uint64
     estimated_fee_rate: FeeRate
     def __init__(
         self,
-        error: Optional[String],
+        error: Optional[str],
         time_target: uint64,
         estimated_fee_rate: FeeRate
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> FeeEstimate: ...
@@ -736,27 +749,27 @@
     def from_bytes_unchecked(bytes) -> FeeEstimate: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FeeEstimate, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FeeEstimate: ...
-    def replace(self, *, error: Union[ Optional[String], _Unspec] = _Unspec(),
+    def from_json_dict(json_dict: Any) -> FeeEstimate: ...
+    def replace(self, *, error: Union[ Optional[str], _Unspec] = _Unspec(),
         time_target: Union[ uint64, _Unspec] = _Unspec(),
         estimated_fee_rate: Union[ FeeRate, _Unspec] = _Unspec()) -> FeeEstimate: ...
 
 class FeeEstimateGroup:
-    error: Optional[String]
+    error: Optional[str]
     estimates: List[FeeEstimate]
     def __init__(
         self,
-        error: Optional[String],
+        error: Optional[str],
         estimates: Sequence[FeeEstimate]
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> FeeEstimateGroup: ...
     def __copy__(self) -> FeeEstimateGroup: ...
@@ -766,18 +779,18 @@
     def from_bytes_unchecked(bytes) -> FeeEstimateGroup: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FeeEstimateGroup, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FeeEstimateGroup: ...
-    def replace(self, *, error: Union[ Optional[String], _Unspec] = _Unspec(),
+    def from_json_dict(json_dict: Any) -> FeeEstimateGroup: ...
+    def replace(self, *, error: Union[ Optional[str], _Unspec] = _Unspec(),
         estimates: Union[ List[FeeEstimate], _Unspec] = _Unspec()) -> FeeEstimateGroup: ...
 
 class TransactionsInfo:
     generator_root: bytes32
     generator_refs_root: bytes32
     aggregated_signature: G2Element
     fees: uint64
@@ -803,17 +816,17 @@
     def from_bytes_unchecked(bytes) -> TransactionsInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[TransactionsInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> TransactionsInfo: ...
+    def from_json_dict(json_dict: Any) -> TransactionsInfo: ...
     def replace(self, *, generator_root: Union[ bytes32, _Unspec] = _Unspec(),
         generator_refs_root: Union[ bytes32, _Unspec] = _Unspec(),
         aggregated_signature: Union[ G2Element, _Unspec] = _Unspec(),
         fees: Union[ uint64, _Unspec] = _Unspec(),
         cost: Union[ uint64, _Unspec] = _Unspec(),
         reward_claims_incorporated: Union[ List[Coin], _Unspec] = _Unspec()) -> TransactionsInfo: ...
 
@@ -844,17 +857,17 @@
     def from_bytes_unchecked(bytes) -> FoliageTransactionBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FoliageTransactionBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FoliageTransactionBlock: ...
+    def from_json_dict(json_dict: Any) -> FoliageTransactionBlock: ...
     def replace(self, *, prev_transaction_block_hash: Union[ bytes32, _Unspec] = _Unspec(),
         timestamp: Union[ uint64, _Unspec] = _Unspec(),
         filter_hash: Union[ bytes32, _Unspec] = _Unspec(),
         additions_root: Union[ bytes32, _Unspec] = _Unspec(),
         removals_root: Union[ bytes32, _Unspec] = _Unspec(),
         transactions_info_hash: Union[ bytes32, _Unspec] = _Unspec()) -> FoliageTransactionBlock: ...
 
@@ -883,17 +896,17 @@
     def from_bytes_unchecked(bytes) -> FoliageBlockData: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FoliageBlockData, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FoliageBlockData: ...
+    def from_json_dict(json_dict: Any) -> FoliageBlockData: ...
     def replace(self, *, unfinished_reward_block_hash: Union[ bytes32, _Unspec] = _Unspec(),
         pool_target: Union[ PoolTarget, _Unspec] = _Unspec(),
         pool_signature: Union[ Optional[G2Element], _Unspec] = _Unspec(),
         farmer_reward_puzzle_hash: Union[ bytes32, _Unspec] = _Unspec(),
         extension_data: Union[ bytes32, _Unspec] = _Unspec()) -> FoliageBlockData: ...
 
 class Foliage:
@@ -923,17 +936,17 @@
     def from_bytes_unchecked(bytes) -> Foliage: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Foliage, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Foliage: ...
+    def from_json_dict(json_dict: Any) -> Foliage: ...
     def replace(self, *, prev_block_hash: Union[ bytes32, _Unspec] = _Unspec(),
         reward_block_hash: Union[ bytes32, _Unspec] = _Unspec(),
         foliage_block_data: Union[ FoliageBlockData, _Unspec] = _Unspec(),
         foliage_block_data_signature: Union[ G2Element, _Unspec] = _Unspec(),
         foliage_transaction_block_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         foliage_transaction_block_signature: Union[ Optional[G2Element], _Unspec] = _Unspec()) -> Foliage: ...
 
@@ -962,17 +975,17 @@
     def from_bytes_unchecked(bytes) -> NewPeak: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewPeak, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewPeak: ...
+    def from_json_dict(json_dict: Any) -> NewPeak: ...
     def replace(self, *, header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec(),
         weight: Union[ uint128, _Unspec] = _Unspec(),
         fork_point_with_previous_peak: Union[ uint32, _Unspec] = _Unspec(),
         unfinished_reward_block_hash: Union[ bytes32, _Unspec] = _Unspec()) -> NewPeak: ...
 
 class NewTransaction:
@@ -996,17 +1009,17 @@
     def from_bytes_unchecked(bytes) -> NewTransaction: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewTransaction, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewTransaction: ...
+    def from_json_dict(json_dict: Any) -> NewTransaction: ...
     def replace(self, *, transaction_id: Union[ bytes32, _Unspec] = _Unspec(),
         cost: Union[ uint64, _Unspec] = _Unspec(),
         fees: Union[ uint64, _Unspec] = _Unspec()) -> NewTransaction: ...
 
 class RequestTransaction:
     transaction_id: bytes32
     def __init__(
@@ -1024,17 +1037,17 @@
     def from_bytes_unchecked(bytes) -> RequestTransaction: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestTransaction, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestTransaction: ...
+    def from_json_dict(json_dict: Any) -> RequestTransaction: ...
     def replace(self, *, transaction_id: Union[ bytes32, _Unspec] = _Unspec()) -> RequestTransaction: ...
 
 class RespondTransaction:
     transaction: SpendBundle
     def __init__(
         self,
         transaction: SpendBundle
@@ -1050,17 +1063,17 @@
     def from_bytes_unchecked(bytes) -> RespondTransaction: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondTransaction, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondTransaction: ...
+    def from_json_dict(json_dict: Any) -> RespondTransaction: ...
     def replace(self, *, transaction: Union[ SpendBundle, _Unspec] = _Unspec()) -> RespondTransaction: ...
 
 class RequestProofOfWeight:
     total_number_of_blocks: uint32
     tip: bytes32
     def __init__(
         self,
@@ -1078,17 +1091,17 @@
     def from_bytes_unchecked(bytes) -> RequestProofOfWeight: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestProofOfWeight, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestProofOfWeight: ...
+    def from_json_dict(json_dict: Any) -> RequestProofOfWeight: ...
     def replace(self, *, total_number_of_blocks: Union[ uint32, _Unspec] = _Unspec(),
         tip: Union[ bytes32, _Unspec] = _Unspec()) -> RequestProofOfWeight: ...
 
 class RespondProofOfWeight:
     wp: WeightProof
     tip: bytes32
     def __init__(
@@ -1107,17 +1120,17 @@
     def from_bytes_unchecked(bytes) -> RespondProofOfWeight: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondProofOfWeight, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondProofOfWeight: ...
+    def from_json_dict(json_dict: Any) -> RespondProofOfWeight: ...
     def replace(self, *, wp: Union[ WeightProof, _Unspec] = _Unspec(),
         tip: Union[ bytes32, _Unspec] = _Unspec()) -> RespondProofOfWeight: ...
 
 class RequestBlock:
     height: uint32
     include_transaction_block: bool
     def __init__(
@@ -1136,17 +1149,17 @@
     def from_bytes_unchecked(bytes) -> RequestBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestBlock: ...
+    def from_json_dict(json_dict: Any) -> RequestBlock: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         include_transaction_block: Union[ bool, _Unspec] = _Unspec()) -> RequestBlock: ...
 
 class RejectBlock:
     height: uint32
     def __init__(
         self,
@@ -1163,17 +1176,17 @@
     def from_bytes_unchecked(bytes) -> RejectBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectBlock: ...
+    def from_json_dict(json_dict: Any) -> RejectBlock: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec()) -> RejectBlock: ...
 
 class RequestBlocks:
     start_height: uint32
     end_height: uint32
     include_transaction_block: bool
     def __init__(
@@ -1193,17 +1206,17 @@
     def from_bytes_unchecked(bytes) -> RequestBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestBlocks: ...
+    def from_json_dict(json_dict: Any) -> RequestBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec(),
         include_transaction_block: Union[ bool, _Unspec] = _Unspec()) -> RequestBlocks: ...
 
 class RespondBlocks:
     start_height: uint32
     end_height: uint32
@@ -1225,17 +1238,17 @@
     def from_bytes_unchecked(bytes) -> RespondBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondBlocks: ...
+    def from_json_dict(json_dict: Any) -> RespondBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec(),
         blocks: Union[ List[FullBlock], _Unspec] = _Unspec()) -> RespondBlocks: ...
 
 class RejectBlocks:
     start_height: uint32
     end_height: uint32
@@ -1255,17 +1268,17 @@
     def from_bytes_unchecked(bytes) -> RejectBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectBlocks: ...
+    def from_json_dict(json_dict: Any) -> RejectBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec()) -> RejectBlocks: ...
 
 class RespondBlock:
     block: FullBlock
     def __init__(
         self,
@@ -1282,17 +1295,17 @@
     def from_bytes_unchecked(bytes) -> RespondBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondBlock: ...
+    def from_json_dict(json_dict: Any) -> RespondBlock: ...
     def replace(self, *, block: Union[ FullBlock, _Unspec] = _Unspec()) -> RespondBlock: ...
 
 class NewUnfinishedBlock:
     unfinished_reward_hash: bytes32
     def __init__(
         self,
         unfinished_reward_hash: bytes
@@ -1308,17 +1321,17 @@
     def from_bytes_unchecked(bytes) -> NewUnfinishedBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewUnfinishedBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewUnfinishedBlock: ...
+    def from_json_dict(json_dict: Any) -> NewUnfinishedBlock: ...
     def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec()) -> NewUnfinishedBlock: ...
 
 class RequestUnfinishedBlock:
     unfinished_reward_hash: bytes32
     def __init__(
         self,
         unfinished_reward_hash: bytes
@@ -1334,17 +1347,17 @@
     def from_bytes_unchecked(bytes) -> RequestUnfinishedBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestUnfinishedBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestUnfinishedBlock: ...
+    def from_json_dict(json_dict: Any) -> RequestUnfinishedBlock: ...
     def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec()) -> RequestUnfinishedBlock: ...
 
 class RespondUnfinishedBlock:
     unfinished_block: UnfinishedBlock
     def __init__(
         self,
         unfinished_block: UnfinishedBlock
@@ -1360,17 +1373,17 @@
     def from_bytes_unchecked(bytes) -> RespondUnfinishedBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondUnfinishedBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondUnfinishedBlock: ...
+    def from_json_dict(json_dict: Any) -> RespondUnfinishedBlock: ...
     def replace(self, *, unfinished_block: Union[ UnfinishedBlock, _Unspec] = _Unspec()) -> RespondUnfinishedBlock: ...
 
 class NewSignagePointOrEndOfSubSlot:
     prev_challenge_hash: Optional[bytes32]
     challenge_hash: bytes32
     index_from_challenge: uint8
     last_rc_infusion: bytes32
@@ -1392,17 +1405,17 @@
     def from_bytes_unchecked(bytes) -> NewSignagePointOrEndOfSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewSignagePointOrEndOfSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewSignagePointOrEndOfSubSlot: ...
+    def from_json_dict(json_dict: Any) -> NewSignagePointOrEndOfSubSlot: ...
     def replace(self, *, prev_challenge_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         challenge_hash: Union[ bytes32, _Unspec] = _Unspec(),
         index_from_challenge: Union[ uint8, _Unspec] = _Unspec(),
         last_rc_infusion: Union[ bytes32, _Unspec] = _Unspec()) -> NewSignagePointOrEndOfSubSlot: ...
 
 class RequestSignagePointOrEndOfSubSlot:
     challenge_hash: bytes32
@@ -1425,17 +1438,17 @@
     def from_bytes_unchecked(bytes) -> RequestSignagePointOrEndOfSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestSignagePointOrEndOfSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestSignagePointOrEndOfSubSlot: ...
+    def from_json_dict(json_dict: Any) -> RequestSignagePointOrEndOfSubSlot: ...
     def replace(self, *, challenge_hash: Union[ bytes32, _Unspec] = _Unspec(),
         index_from_challenge: Union[ uint8, _Unspec] = _Unspec(),
         last_rc_infusion: Union[ bytes32, _Unspec] = _Unspec()) -> RequestSignagePointOrEndOfSubSlot: ...
 
 class RespondSignagePoint:
     index_from_challenge: uint8
     challenge_chain_vdf: VDFInfo
@@ -1461,17 +1474,17 @@
     def from_bytes_unchecked(bytes) -> RespondSignagePoint: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondSignagePoint, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondSignagePoint: ...
+    def from_json_dict(json_dict: Any) -> RespondSignagePoint: ...
     def replace(self, *, index_from_challenge: Union[ uint8, _Unspec] = _Unspec(),
         challenge_chain_vdf: Union[ VDFInfo, _Unspec] = _Unspec(),
         challenge_chain_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         reward_chain_vdf: Union[ VDFInfo, _Unspec] = _Unspec(),
         reward_chain_proof: Union[ VDFProof, _Unspec] = _Unspec()) -> RespondSignagePoint: ...
 
 class RespondEndOfSubSlot:
@@ -1491,17 +1504,17 @@
     def from_bytes_unchecked(bytes) -> RespondEndOfSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondEndOfSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondEndOfSubSlot: ...
+    def from_json_dict(json_dict: Any) -> RespondEndOfSubSlot: ...
     def replace(self, *, end_of_slot_bundle: Union[ EndOfSubSlotBundle, _Unspec] = _Unspec()) -> RespondEndOfSubSlot: ...
 
 class RequestMempoolTransactions:
     filter: bytes
     def __init__(
         self,
         filter: bytes
@@ -1517,17 +1530,17 @@
     def from_bytes_unchecked(bytes) -> RequestMempoolTransactions: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestMempoolTransactions, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestMempoolTransactions: ...
+    def from_json_dict(json_dict: Any) -> RequestMempoolTransactions: ...
     def replace(self, *, filter: Union[ bytes, _Unspec] = _Unspec()) -> RequestMempoolTransactions: ...
 
 class NewCompactVDF:
     height: uint32
     header_hash: bytes32
     field_vdf: uint8
     vdf_info: VDFInfo
@@ -1549,17 +1562,17 @@
     def from_bytes_unchecked(bytes) -> NewCompactVDF: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewCompactVDF, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewCompactVDF: ...
+    def from_json_dict(json_dict: Any) -> NewCompactVDF: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         field_vdf: Union[ uint8, _Unspec] = _Unspec(),
         vdf_info: Union[ VDFInfo, _Unspec] = _Unspec()) -> NewCompactVDF: ...
 
 class RequestCompactVDF:
     height: uint32
@@ -1584,17 +1597,17 @@
     def from_bytes_unchecked(bytes) -> RequestCompactVDF: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestCompactVDF, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestCompactVDF: ...
+    def from_json_dict(json_dict: Any) -> RequestCompactVDF: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         field_vdf: Union[ uint8, _Unspec] = _Unspec(),
         vdf_info: Union[ VDFInfo, _Unspec] = _Unspec()) -> RequestCompactVDF: ...
 
 class RespondCompactVDF:
     height: uint32
@@ -1621,17 +1634,17 @@
     def from_bytes_unchecked(bytes) -> RespondCompactVDF: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondCompactVDF, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondCompactVDF: ...
+    def from_json_dict(json_dict: Any) -> RespondCompactVDF: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         field_vdf: Union[ uint8, _Unspec] = _Unspec(),
         vdf_info: Union[ VDFInfo, _Unspec] = _Unspec(),
         vdf_proof: Union[ VDFProof, _Unspec] = _Unspec()) -> RespondCompactVDF: ...
 
 class RequestPeers:
@@ -1649,17 +1662,17 @@
     def from_bytes_unchecked(bytes) -> RequestPeers: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestPeers, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestPeers: ...
+    def from_json_dict(json_dict: Any) -> RequestPeers: ...
 
 class RespondPeers:
     peer_list: List[TimestampedPeerInfo]
     def __init__(
         self,
         peer_list: Sequence[TimestampedPeerInfo]
     ) -> None: ...
@@ -1674,17 +1687,17 @@
     def from_bytes_unchecked(bytes) -> RespondPeers: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondPeers, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondPeers: ...
+    def from_json_dict(json_dict: Any) -> RespondPeers: ...
     def replace(self, *, peer_list: Union[ List[TimestampedPeerInfo], _Unspec] = _Unspec()) -> RespondPeers: ...
 
 class FullBlock:
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlock
     challenge_chain_sp_proof: Optional[VDFProof]
     challenge_chain_ip_proof: VDFProof
@@ -1730,17 +1743,17 @@
     def from_bytes_unchecked(bytes) -> FullBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[FullBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> FullBlock: ...
+    def from_json_dict(json_dict: Any) -> FullBlock: ...
     def replace(self, *, finished_sub_slots: Union[ List[EndOfSubSlotBundle], _Unspec] = _Unspec(),
         reward_chain_block: Union[ RewardChainBlock, _Unspec] = _Unspec(),
         challenge_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         challenge_chain_ip_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         reward_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         reward_chain_ip_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         infused_challenge_chain_ip_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
@@ -1796,36 +1809,36 @@
     def from_bytes_unchecked(bytes) -> HeaderBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[HeaderBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> HeaderBlock: ...
+    def from_json_dict(json_dict: Any) -> HeaderBlock: ...
     def replace(self, *, finished_sub_slots: Union[ List[EndOfSubSlotBundle], _Unspec] = _Unspec(),
         reward_chain_block: Union[ RewardChainBlock, _Unspec] = _Unspec(),
         challenge_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         challenge_chain_ip_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         reward_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         reward_chain_ip_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         infused_challenge_chain_ip_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         foliage: Union[ Foliage, _Unspec] = _Unspec(),
         foliage_transaction_block: Union[ Optional[FoliageTransactionBlock], _Unspec] = _Unspec(),
         transactions_filter: Union[ bytes, _Unspec] = _Unspec(),
         transactions_info: Union[ Optional[TransactionsInfo], _Unspec] = _Unspec()) -> HeaderBlock: ...
 
 class TimestampedPeerInfo:
-    host: String
+    host: str
     port: uint16
     timestamp: uint64
     def __init__(
         self,
-        host: String,
+        host: str,
         port: uint16,
         timestamp: uint64
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> TimestampedPeerInfo: ...
@@ -1836,18 +1849,18 @@
     def from_bytes_unchecked(bytes) -> TimestampedPeerInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[TimestampedPeerInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> TimestampedPeerInfo: ...
-    def replace(self, *, host: Union[ String, _Unspec] = _Unspec(),
+    def from_json_dict(json_dict: Any) -> TimestampedPeerInfo: ...
+    def replace(self, *, host: Union[ str, _Unspec] = _Unspec(),
         port: Union[ uint16, _Unspec] = _Unspec(),
         timestamp: Union[ uint64, _Unspec] = _Unspec()) -> TimestampedPeerInfo: ...
 
 class PoolTarget:
     puzzle_hash: bytes32
     max_height: uint32
     def __init__(
@@ -1866,17 +1879,17 @@
     def from_bytes_unchecked(bytes) -> PoolTarget: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[PoolTarget, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> PoolTarget: ...
+    def from_json_dict(json_dict: Any) -> PoolTarget: ...
     def replace(self, *, puzzle_hash: Union[ bytes32, _Unspec] = _Unspec(),
         max_height: Union[ uint32, _Unspec] = _Unspec()) -> PoolTarget: ...
 
 class Program:
     a0: bytes
     def get_tree_hash(self) -> bytes32: ...
     @staticmethod
@@ -1907,17 +1920,17 @@
     def from_bytes_unchecked(bytes) -> Program: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[Program, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> Program: ...
+    def from_json_dict(json_dict: Any) -> Program: ...
     def replace(self, *, a0: Union[ bytes, _Unspec] = _Unspec()) -> Program: ...
 
 class ProofOfSpace:
     challenge: bytes32
     pool_public_key: Optional[G1Element]
     pool_contract_puzzle_hash: Optional[bytes32]
     plot_public_key: G1Element
@@ -1943,17 +1956,17 @@
     def from_bytes_unchecked(bytes) -> ProofOfSpace: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[ProofOfSpace, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> ProofOfSpace: ...
+    def from_json_dict(json_dict: Any) -> ProofOfSpace: ...
     def replace(self, *, challenge: Union[ bytes32, _Unspec] = _Unspec(),
         pool_public_key: Union[ Optional[G1Element], _Unspec] = _Unspec(),
         pool_contract_puzzle_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         plot_public_key: Union[ G1Element, _Unspec] = _Unspec(),
         size: Union[ uint8, _Unspec] = _Unspec(),
         proof: Union[ bytes, _Unspec] = _Unspec()) -> ProofOfSpace: ...
 
@@ -1988,17 +2001,17 @@
     def from_bytes_unchecked(bytes) -> RewardChainBlockUnfinished: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RewardChainBlockUnfinished, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RewardChainBlockUnfinished: ...
+    def from_json_dict(json_dict: Any) -> RewardChainBlockUnfinished: ...
     def replace(self, *, total_iters: Union[ uint128, _Unspec] = _Unspec(),
         signage_point_index: Union[ uint8, _Unspec] = _Unspec(),
         pos_ss_cc_challenge_hash: Union[ bytes32, _Unspec] = _Unspec(),
         proof_of_space: Union[ ProofOfSpace, _Unspec] = _Unspec(),
         challenge_chain_sp_vdf: Union[ Optional[VDFInfo], _Unspec] = _Unspec(),
         challenge_chain_sp_signature: Union[ G2Element, _Unspec] = _Unspec(),
         reward_chain_sp_vdf: Union[ Optional[VDFInfo], _Unspec] = _Unspec(),
@@ -2048,17 +2061,17 @@
     def from_bytes_unchecked(bytes) -> RewardChainBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RewardChainBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RewardChainBlock: ...
+    def from_json_dict(json_dict: Any) -> RewardChainBlock: ...
     def replace(self, *, weight: Union[ uint128, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec(),
         total_iters: Union[ uint128, _Unspec] = _Unspec(),
         signage_point_index: Union[ uint8, _Unspec] = _Unspec(),
         pos_ss_cc_challenge_hash: Union[ bytes32, _Unspec] = _Unspec(),
         proof_of_space: Union[ ProofOfSpace, _Unspec] = _Unspec(),
         challenge_chain_sp_vdf: Union[ Optional[VDFInfo], _Unspec] = _Unspec(),
@@ -2093,17 +2106,17 @@
     def from_bytes_unchecked(bytes) -> ChallengeBlockInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[ChallengeBlockInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> ChallengeBlockInfo: ...
+    def from_json_dict(json_dict: Any) -> ChallengeBlockInfo: ...
     def replace(self, *, proof_of_space: Union[ ProofOfSpace, _Unspec] = _Unspec(),
         challenge_chain_sp_vdf: Union[ Optional[VDFInfo], _Unspec] = _Unspec(),
         challenge_chain_sp_signature: Union[ G2Element, _Unspec] = _Unspec(),
         challenge_chain_ip_vdf: Union[ VDFInfo, _Unspec] = _Unspec()) -> ChallengeBlockInfo: ...
 
 class ChallengeChainSubSlot:
     challenge_chain_end_of_slot_vdf: VDFInfo
@@ -2130,17 +2143,17 @@
     def from_bytes_unchecked(bytes) -> ChallengeChainSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[ChallengeChainSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> ChallengeChainSubSlot: ...
+    def from_json_dict(json_dict: Any) -> ChallengeChainSubSlot: ...
     def replace(self, *, challenge_chain_end_of_slot_vdf: Union[ VDFInfo, _Unspec] = _Unspec(),
         infused_challenge_chain_sub_slot_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         subepoch_summary_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         new_sub_slot_iters: Union[ Optional[uint64], _Unspec] = _Unspec(),
         new_difficulty: Union[ Optional[uint64], _Unspec] = _Unspec()) -> ChallengeChainSubSlot: ...
 
 class InfusedChallengeChainSubSlot:
@@ -2160,17 +2173,17 @@
     def from_bytes_unchecked(bytes) -> InfusedChallengeChainSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[InfusedChallengeChainSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> InfusedChallengeChainSubSlot: ...
+    def from_json_dict(json_dict: Any) -> InfusedChallengeChainSubSlot: ...
     def replace(self, *, infused_challenge_chain_end_of_slot_vdf: Union[ VDFInfo, _Unspec] = _Unspec()) -> InfusedChallengeChainSubSlot: ...
 
 class RewardChainSubSlot:
     end_of_slot_vdf: VDFInfo
     challenge_chain_sub_slot_hash: bytes32
     infused_challenge_chain_sub_slot_hash: Optional[bytes32]
     deficit: uint8
@@ -2192,17 +2205,17 @@
     def from_bytes_unchecked(bytes) -> RewardChainSubSlot: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RewardChainSubSlot, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RewardChainSubSlot: ...
+    def from_json_dict(json_dict: Any) -> RewardChainSubSlot: ...
     def replace(self, *, end_of_slot_vdf: Union[ VDFInfo, _Unspec] = _Unspec(),
         challenge_chain_sub_slot_hash: Union[ bytes32, _Unspec] = _Unspec(),
         infused_challenge_chain_sub_slot_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         deficit: Union[ uint8, _Unspec] = _Unspec()) -> RewardChainSubSlot: ...
 
 class SubSlotProofs:
     challenge_chain_slot_proof: VDFProof
@@ -2225,17 +2238,17 @@
     def from_bytes_unchecked(bytes) -> SubSlotProofs: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubSlotProofs, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubSlotProofs: ...
+    def from_json_dict(json_dict: Any) -> SubSlotProofs: ...
     def replace(self, *, challenge_chain_slot_proof: Union[ VDFProof, _Unspec] = _Unspec(),
         infused_challenge_chain_slot_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         reward_chain_slot_proof: Union[ VDFProof, _Unspec] = _Unspec()) -> SubSlotProofs: ...
 
 class SpendBundle:
     coin_spends: List[CoinSpend]
     aggregated_signature: G2Element
@@ -2261,17 +2274,17 @@
     def from_bytes_unchecked(bytes) -> SpendBundle: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SpendBundle, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SpendBundle: ...
+    def from_json_dict(json_dict: Any) -> SpendBundle: ...
     def replace(self, *, coin_spends: Union[ List[CoinSpend], _Unspec] = _Unspec(),
         aggregated_signature: Union[ G2Element, _Unspec] = _Unspec()) -> SpendBundle: ...
 
 class SubEpochSummary:
     prev_subepoch_summary_hash: bytes32
     reward_chain_hash: bytes32
     num_blocks_overflow: uint8
@@ -2296,17 +2309,17 @@
     def from_bytes_unchecked(bytes) -> SubEpochSummary: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubEpochSummary, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubEpochSummary: ...
+    def from_json_dict(json_dict: Any) -> SubEpochSummary: ...
     def replace(self, *, prev_subepoch_summary_hash: Union[ bytes32, _Unspec] = _Unspec(),
         reward_chain_hash: Union[ bytes32, _Unspec] = _Unspec(),
         num_blocks_overflow: Union[ uint8, _Unspec] = _Unspec(),
         new_difficulty: Union[ Optional[uint64], _Unspec] = _Unspec(),
         new_sub_slot_iters: Union[ Optional[uint64], _Unspec] = _Unspec()) -> SubEpochSummary: ...
 
 class UnfinishedBlock:
@@ -2346,27 +2359,71 @@
     def from_bytes_unchecked(bytes) -> UnfinishedBlock: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[UnfinishedBlock, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> UnfinishedBlock: ...
+    def from_json_dict(json_dict: Any) -> UnfinishedBlock: ...
     def replace(self, *, finished_sub_slots: Union[ List[EndOfSubSlotBundle], _Unspec] = _Unspec(),
         reward_chain_block: Union[ RewardChainBlockUnfinished, _Unspec] = _Unspec(),
         challenge_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         reward_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         foliage: Union[ Foliage, _Unspec] = _Unspec(),
         foliage_transaction_block: Union[ Optional[FoliageTransactionBlock], _Unspec] = _Unspec(),
         transactions_info: Union[ Optional[TransactionsInfo], _Unspec] = _Unspec(),
         transactions_generator: Union[ Optional[Program], _Unspec] = _Unspec(),
         transactions_generator_ref_list: Union[ List[uint32], _Unspec] = _Unspec()) -> UnfinishedBlock: ...
 
+class UnfinishedHeaderBlock:
+    finished_sub_slots: List[EndOfSubSlotBundle]
+    reward_chain_block: RewardChainBlockUnfinished
+    challenge_chain_sp_proof: Optional[VDFProof]
+    reward_chain_sp_proof: Optional[VDFProof]
+    foliage: Foliage
+    foliage_transaction_block: Optional[FoliageTransactionBlock]
+    transactions_filter: bytes
+    def __init__(
+        self,
+        finished_sub_slots: Sequence[EndOfSubSlotBundle],
+        reward_chain_block: RewardChainBlockUnfinished,
+        challenge_chain_sp_proof: Optional[VDFProof],
+        reward_chain_sp_proof: Optional[VDFProof],
+        foliage: Foliage,
+        foliage_transaction_block: Optional[FoliageTransactionBlock],
+        transactions_filter: bytes
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> UnfinishedHeaderBlock: ...
+    def __copy__(self) -> UnfinishedHeaderBlock: ...
+    @staticmethod
+    def from_bytes(bytes) -> UnfinishedHeaderBlock: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> UnfinishedHeaderBlock: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[UnfinishedHeaderBlock, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> UnfinishedHeaderBlock: ...
+    def replace(self, *, finished_sub_slots: Union[ List[EndOfSubSlotBundle], _Unspec] = _Unspec(),
+        reward_chain_block: Union[ RewardChainBlockUnfinished, _Unspec] = _Unspec(),
+        challenge_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
+        reward_chain_sp_proof: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
+        foliage: Union[ Foliage, _Unspec] = _Unspec(),
+        foliage_transaction_block: Union[ Optional[FoliageTransactionBlock], _Unspec] = _Unspec(),
+        transactions_filter: Union[ bytes, _Unspec] = _Unspec()) -> UnfinishedHeaderBlock: ...
+
 class VDFInfo:
     challenge: bytes32
     number_of_iterations: uint64
     output: ClassgroupElement
     def __init__(
         self,
         challenge: bytes,
@@ -2384,17 +2441,17 @@
     def from_bytes_unchecked(bytes) -> VDFInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[VDFInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> VDFInfo: ...
+    def from_json_dict(json_dict: Any) -> VDFInfo: ...
     def replace(self, *, challenge: Union[ bytes32, _Unspec] = _Unspec(),
         number_of_iterations: Union[ uint64, _Unspec] = _Unspec(),
         output: Union[ ClassgroupElement, _Unspec] = _Unspec()) -> VDFInfo: ...
 
 class VDFProof:
     witness_type: uint8
     witness: bytes
@@ -2416,17 +2473,17 @@
     def from_bytes_unchecked(bytes) -> VDFProof: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[VDFProof, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> VDFProof: ...
+    def from_json_dict(json_dict: Any) -> VDFProof: ...
     def replace(self, *, witness_type: Union[ uint8, _Unspec] = _Unspec(),
         witness: Union[ bytes, _Unspec] = _Unspec(),
         normalized_to_identity: Union[ bool, _Unspec] = _Unspec()) -> VDFProof: ...
 
 class RequestPuzzleSolution:
     coin_name: bytes32
     height: uint32
@@ -2446,17 +2503,17 @@
     def from_bytes_unchecked(bytes) -> RequestPuzzleSolution: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestPuzzleSolution, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestPuzzleSolution: ...
+    def from_json_dict(json_dict: Any) -> RequestPuzzleSolution: ...
     def replace(self, *, coin_name: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec()) -> RequestPuzzleSolution: ...
 
 class PuzzleSolutionResponse:
     coin_name: bytes32
     height: uint32
     puzzle: Program
@@ -2479,17 +2536,17 @@
     def from_bytes_unchecked(bytes) -> PuzzleSolutionResponse: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[PuzzleSolutionResponse, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> PuzzleSolutionResponse: ...
+    def from_json_dict(json_dict: Any) -> PuzzleSolutionResponse: ...
     def replace(self, *, coin_name: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec(),
         puzzle: Union[ Program, _Unspec] = _Unspec(),
         solution: Union[ Program, _Unspec] = _Unspec()) -> PuzzleSolutionResponse: ...
 
 class RespondPuzzleSolution:
     response: PuzzleSolutionResponse
@@ -2508,17 +2565,17 @@
     def from_bytes_unchecked(bytes) -> RespondPuzzleSolution: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondPuzzleSolution, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondPuzzleSolution: ...
+    def from_json_dict(json_dict: Any) -> RespondPuzzleSolution: ...
     def replace(self, *, response: Union[ PuzzleSolutionResponse, _Unspec] = _Unspec()) -> RespondPuzzleSolution: ...
 
 class RejectPuzzleSolution:
     coin_name: bytes32
     height: uint32
     def __init__(
         self,
@@ -2536,17 +2593,17 @@
     def from_bytes_unchecked(bytes) -> RejectPuzzleSolution: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectPuzzleSolution, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectPuzzleSolution: ...
+    def from_json_dict(json_dict: Any) -> RejectPuzzleSolution: ...
     def replace(self, *, coin_name: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec()) -> RejectPuzzleSolution: ...
 
 class SendTransaction:
     transaction: SpendBundle
     def __init__(
         self,
@@ -2563,28 +2620,28 @@
     def from_bytes_unchecked(bytes) -> SendTransaction: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SendTransaction, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SendTransaction: ...
+    def from_json_dict(json_dict: Any) -> SendTransaction: ...
     def replace(self, *, transaction: Union[ SpendBundle, _Unspec] = _Unspec()) -> SendTransaction: ...
 
 class TransactionAck:
     txid: bytes32
     status: uint8
-    error: Optional[String]
+    error: Optional[str]
     def __init__(
         self,
         txid: bytes,
         status: uint8,
-        error: Optional[String]
+        error: Optional[str]
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> TransactionAck: ...
     def __copy__(self) -> TransactionAck: ...
     @staticmethod
@@ -2593,20 +2650,20 @@
     def from_bytes_unchecked(bytes) -> TransactionAck: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[TransactionAck, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> TransactionAck: ...
+    def from_json_dict(json_dict: Any) -> TransactionAck: ...
     def replace(self, *, txid: Union[ bytes32, _Unspec] = _Unspec(),
         status: Union[ uint8, _Unspec] = _Unspec(),
-        error: Union[ Optional[String], _Unspec] = _Unspec()) -> TransactionAck: ...
+        error: Union[ Optional[str], _Unspec] = _Unspec()) -> TransactionAck: ...
 
 class NewPeakWallet:
     header_hash: bytes32
     height: uint32
     weight: uint128
     fork_point_with_previous_peak: uint32
     def __init__(
@@ -2627,17 +2684,17 @@
     def from_bytes_unchecked(bytes) -> NewPeakWallet: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewPeakWallet, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> NewPeakWallet: ...
+    def from_json_dict(json_dict: Any) -> NewPeakWallet: ...
     def replace(self, *, header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         height: Union[ uint32, _Unspec] = _Unspec(),
         weight: Union[ uint128, _Unspec] = _Unspec(),
         fork_point_with_previous_peak: Union[ uint32, _Unspec] = _Unspec()) -> NewPeakWallet: ...
 
 class RequestBlockHeader:
     height: uint32
@@ -2656,17 +2713,17 @@
     def from_bytes_unchecked(bytes) -> RequestBlockHeader: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestBlockHeader, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestBlockHeader: ...
+    def from_json_dict(json_dict: Any) -> RequestBlockHeader: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec()) -> RequestBlockHeader: ...
 
 class RespondBlockHeader:
     header_block: HeaderBlock
     def __init__(
         self,
         header_block: HeaderBlock
@@ -2682,17 +2739,17 @@
     def from_bytes_unchecked(bytes) -> RespondBlockHeader: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondBlockHeader, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondBlockHeader: ...
+    def from_json_dict(json_dict: Any) -> RespondBlockHeader: ...
     def replace(self, *, header_block: Union[ HeaderBlock, _Unspec] = _Unspec()) -> RespondBlockHeader: ...
 
 class RejectHeaderRequest:
     height: uint32
     def __init__(
         self,
         height: uint32
@@ -2708,17 +2765,17 @@
     def from_bytes_unchecked(bytes) -> RejectHeaderRequest: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectHeaderRequest, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectHeaderRequest: ...
+    def from_json_dict(json_dict: Any) -> RejectHeaderRequest: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec()) -> RejectHeaderRequest: ...
 
 class RequestRemovals:
     height: uint32
     header_hash: bytes32
     coin_names: Optional[List[bytes32]]
     def __init__(
@@ -2738,32 +2795,32 @@
     def from_bytes_unchecked(bytes) -> RequestRemovals: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestRemovals, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestRemovals: ...
+    def from_json_dict(json_dict: Any) -> RequestRemovals: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
         coin_names: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestRemovals: ...
 
 class RespondRemovals:
     height: uint32
     header_hash: bytes32
-    coins: List[(bytes32, Optional[Coin])]
-    proofs: Optional[List[(bytes32, bytes)]]
+    coins: List[Tuple[bytes32, Optional[Coin]]]
+    proofs: Optional[List[Tuple[bytes32, bytes]]]
     def __init__(
         self,
         height: uint32,
         header_hash: bytes,
-        coins: Sequence[(bytes32, Optional[Coin])],
-        proofs: Optional[Sequence[(bytes32, bytes)]]
+        coins: Sequence[Tuple[bytes32, Optional[Coin]]],
+        proofs: Optional[Sequence[Tuple[bytes32, bytes]]]
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> RespondRemovals: ...
     def __copy__(self) -> RespondRemovals: ...
     @staticmethod
@@ -2772,21 +2829,21 @@
     def from_bytes_unchecked(bytes) -> RespondRemovals: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondRemovals, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondRemovals: ...
+    def from_json_dict(json_dict: Any) -> RespondRemovals: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
-        coins: Union[ List[(bytes32, Optional[Coin])], _Unspec] = _Unspec(),
-        proofs: Union[ Optional[List[(bytes32, bytes)]], _Unspec] = _Unspec()) -> RespondRemovals: ...
+        coins: Union[ List[Tuple[bytes32, Optional[Coin]]], _Unspec] = _Unspec(),
+        proofs: Union[ Optional[List[Tuple[bytes32, bytes]]], _Unspec] = _Unspec()) -> RespondRemovals: ...
 
 class RejectRemovalsRequest:
     height: uint32
     header_hash: bytes32
     def __init__(
         self,
         height: uint32,
@@ -2803,17 +2860,17 @@
     def from_bytes_unchecked(bytes) -> RejectRemovalsRequest: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectRemovalsRequest, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectRemovalsRequest: ...
+    def from_json_dict(json_dict: Any) -> RejectRemovalsRequest: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec()) -> RejectRemovalsRequest: ...
 
 class RequestAdditions:
     height: uint32
     header_hash: Optional[bytes32]
     puzzle_hashes: Optional[List[bytes32]]
@@ -2834,32 +2891,32 @@
     def from_bytes_unchecked(bytes) -> RequestAdditions: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestAdditions, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestAdditions: ...
+    def from_json_dict(json_dict: Any) -> RequestAdditions: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ Optional[bytes32], _Unspec] = _Unspec(),
         puzzle_hashes: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestAdditions: ...
 
 class RespondAdditions:
     height: uint32
     header_hash: bytes32
-    coins: List[(bytes32, List[Coin])]
-    proofs: Optional[List[(bytes32, bytes, Optional[bytes])]]
+    coins: List[Tuple[bytes32, List[Coin]]]
+    proofs: Optional[List[Tuple[bytes32, bytes, Optional[bytes]]]]
     def __init__(
         self,
         height: uint32,
         header_hash: bytes,
-        coins: Sequence[(bytes32, Sequence[Coin])],
-        proofs: Optional[Sequence[(bytes32, bytes, Optional[bytes])]]
+        coins: Sequence[Tuple[bytes32, Sequence[Coin]]],
+        proofs: Optional[Sequence[Tuple[bytes32, bytes, Optional[bytes]]]]
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> RespondAdditions: ...
     def __copy__(self) -> RespondAdditions: ...
     @staticmethod
@@ -2868,21 +2925,21 @@
     def from_bytes_unchecked(bytes) -> RespondAdditions: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondAdditions, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondAdditions: ...
+    def from_json_dict(json_dict: Any) -> RespondAdditions: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec(),
-        coins: Union[ List[(bytes32, List[Coin])], _Unspec] = _Unspec(),
-        proofs: Union[ Optional[List[(bytes32, bytes, Optional[bytes])]], _Unspec] = _Unspec()) -> RespondAdditions: ...
+        coins: Union[ List[Tuple[bytes32, List[Coin]]], _Unspec] = _Unspec(),
+        proofs: Union[ Optional[List[Tuple[bytes32, bytes, Optional[bytes]]]], _Unspec] = _Unspec()) -> RespondAdditions: ...
 
 class RejectAdditionsRequest:
     height: uint32
     header_hash: bytes32
     def __init__(
         self,
         height: uint32,
@@ -2899,17 +2956,17 @@
     def from_bytes_unchecked(bytes) -> RejectAdditionsRequest: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectAdditionsRequest, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectAdditionsRequest: ...
+    def from_json_dict(json_dict: Any) -> RejectAdditionsRequest: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         header_hash: Union[ bytes32, _Unspec] = _Unspec()) -> RejectAdditionsRequest: ...
 
 class RespondBlockHeaders:
     start_height: uint32
     end_height: uint32
     header_blocks: List[HeaderBlock]
@@ -2930,17 +2987,17 @@
     def from_bytes_unchecked(bytes) -> RespondBlockHeaders: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondBlockHeaders, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondBlockHeaders: ...
+    def from_json_dict(json_dict: Any) -> RespondBlockHeaders: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec(),
         header_blocks: Union[ List[HeaderBlock], _Unspec] = _Unspec()) -> RespondBlockHeaders: ...
 
 class RejectBlockHeaders:
     start_height: uint32
     end_height: uint32
@@ -2960,17 +3017,17 @@
     def from_bytes_unchecked(bytes) -> RejectBlockHeaders: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectBlockHeaders, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectBlockHeaders: ...
+    def from_json_dict(json_dict: Any) -> RejectBlockHeaders: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec()) -> RejectBlockHeaders: ...
 
 class RequestBlockHeaders:
     start_height: uint32
     end_height: uint32
     return_filter: bool
@@ -2991,17 +3048,17 @@
     def from_bytes_unchecked(bytes) -> RequestBlockHeaders: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestBlockHeaders, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestBlockHeaders: ...
+    def from_json_dict(json_dict: Any) -> RequestBlockHeaders: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec(),
         return_filter: Union[ bool, _Unspec] = _Unspec()) -> RequestBlockHeaders: ...
 
 class RequestHeaderBlocks:
     start_height: uint32
     end_height: uint32
@@ -3021,17 +3078,17 @@
     def from_bytes_unchecked(bytes) -> RequestHeaderBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestHeaderBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestHeaderBlocks: ...
+    def from_json_dict(json_dict: Any) -> RequestHeaderBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec()) -> RequestHeaderBlocks: ...
 
 class RejectHeaderBlocks:
     start_height: uint32
     end_height: uint32
     def __init__(
@@ -3050,17 +3107,17 @@
     def from_bytes_unchecked(bytes) -> RejectHeaderBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectHeaderBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RejectHeaderBlocks: ...
+    def from_json_dict(json_dict: Any) -> RejectHeaderBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec()) -> RejectHeaderBlocks: ...
 
 class RespondHeaderBlocks:
     start_height: uint32
     end_height: uint32
     header_blocks: List[HeaderBlock]
@@ -3081,17 +3138,17 @@
     def from_bytes_unchecked(bytes) -> RespondHeaderBlocks: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondHeaderBlocks, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondHeaderBlocks: ...
+    def from_json_dict(json_dict: Any) -> RespondHeaderBlocks: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec(),
         header_blocks: Union[ List[HeaderBlock], _Unspec] = _Unspec()) -> RespondHeaderBlocks: ...
 
 class RegisterForPhUpdates:
     puzzle_hashes: List[bytes32]
     min_height: uint32
@@ -3111,17 +3168,17 @@
     def from_bytes_unchecked(bytes) -> RegisterForPhUpdates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RegisterForPhUpdates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RegisterForPhUpdates: ...
+    def from_json_dict(json_dict: Any) -> RegisterForPhUpdates: ...
     def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
         min_height: Union[ uint32, _Unspec] = _Unspec()) -> RegisterForPhUpdates: ...
 
 class RespondToPhUpdates:
     puzzle_hashes: List[bytes32]
     min_height: uint32
     coin_states: List[CoinState]
@@ -3142,17 +3199,17 @@
     def from_bytes_unchecked(bytes) -> RespondToPhUpdates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondToPhUpdates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondToPhUpdates: ...
+    def from_json_dict(json_dict: Any) -> RespondToPhUpdates: ...
     def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
         min_height: Union[ uint32, _Unspec] = _Unspec(),
         coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondToPhUpdates: ...
 
 class RegisterForCoinUpdates:
     coin_ids: List[bytes32]
     min_height: uint32
@@ -3172,17 +3229,17 @@
     def from_bytes_unchecked(bytes) -> RegisterForCoinUpdates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RegisterForCoinUpdates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RegisterForCoinUpdates: ...
+    def from_json_dict(json_dict: Any) -> RegisterForCoinUpdates: ...
     def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
         min_height: Union[ uint32, _Unspec] = _Unspec()) -> RegisterForCoinUpdates: ...
 
 class RespondToCoinUpdates:
     coin_ids: List[bytes32]
     min_height: uint32
     coin_states: List[CoinState]
@@ -3203,17 +3260,17 @@
     def from_bytes_unchecked(bytes) -> RespondToCoinUpdates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondToCoinUpdates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondToCoinUpdates: ...
+    def from_json_dict(json_dict: Any) -> RespondToCoinUpdates: ...
     def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
         min_height: Union[ uint32, _Unspec] = _Unspec(),
         coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondToCoinUpdates: ...
 
 class CoinStateUpdate:
     height: uint32
     fork_height: uint32
@@ -3237,17 +3294,17 @@
     def from_bytes_unchecked(bytes) -> CoinStateUpdate: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[CoinStateUpdate, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> CoinStateUpdate: ...
+    def from_json_dict(json_dict: Any) -> CoinStateUpdate: ...
     def replace(self, *, height: Union[ uint32, _Unspec] = _Unspec(),
         fork_height: Union[ uint32, _Unspec] = _Unspec(),
         peak_hash: Union[ bytes32, _Unspec] = _Unspec(),
         items: Union[ List[CoinState], _Unspec] = _Unspec()) -> CoinStateUpdate: ...
 
 class RequestChildren:
     coin_name: bytes32
@@ -3266,17 +3323,17 @@
     def from_bytes_unchecked(bytes) -> RequestChildren: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestChildren, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestChildren: ...
+    def from_json_dict(json_dict: Any) -> RequestChildren: ...
     def replace(self, *, coin_name: Union[ bytes32, _Unspec] = _Unspec()) -> RequestChildren: ...
 
 class RespondChildren:
     coin_states: List[CoinState]
     def __init__(
         self,
         coin_states: Sequence[CoinState]
@@ -3292,17 +3349,17 @@
     def from_bytes_unchecked(bytes) -> RespondChildren: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondChildren, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondChildren: ...
+    def from_json_dict(json_dict: Any) -> RespondChildren: ...
     def replace(self, *, coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondChildren: ...
 
 class RequestSesInfo:
     start_height: uint32
     end_height: uint32
     def __init__(
         self,
@@ -3320,17 +3377,17 @@
     def from_bytes_unchecked(bytes) -> RequestSesInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestSesInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestSesInfo: ...
+    def from_json_dict(json_dict: Any) -> RequestSesInfo: ...
     def replace(self, *, start_height: Union[ uint32, _Unspec] = _Unspec(),
         end_height: Union[ uint32, _Unspec] = _Unspec()) -> RequestSesInfo: ...
 
 class RespondSesInfo:
     reward_chain_hash: List[bytes32]
     heights: List[List[uint32]]
     def __init__(
@@ -3349,17 +3406,17 @@
     def from_bytes_unchecked(bytes) -> RespondSesInfo: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondSesInfo, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondSesInfo: ...
+    def from_json_dict(json_dict: Any) -> RespondSesInfo: ...
     def replace(self, *, reward_chain_hash: Union[ List[bytes32], _Unspec] = _Unspec(),
         heights: Union[ List[List[uint32]], _Unspec] = _Unspec()) -> RespondSesInfo: ...
 
 class RequestFeeEstimates:
     time_targets: List[uint64]
     def __init__(
         self,
@@ -3376,17 +3433,17 @@
     def from_bytes_unchecked(bytes) -> RequestFeeEstimates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestFeeEstimates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RequestFeeEstimates: ...
+    def from_json_dict(json_dict: Any) -> RequestFeeEstimates: ...
     def replace(self, *, time_targets: Union[ List[uint64], _Unspec] = _Unspec()) -> RequestFeeEstimates: ...
 
 class RespondFeeEstimates:
     estimates: FeeEstimateGroup
     def __init__(
         self,
         estimates: FeeEstimateGroup
@@ -3402,17 +3459,17 @@
     def from_bytes_unchecked(bytes) -> RespondFeeEstimates: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondFeeEstimates, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RespondFeeEstimates: ...
+    def from_json_dict(json_dict: Any) -> RespondFeeEstimates: ...
     def replace(self, *, estimates: Union[ FeeEstimateGroup, _Unspec] = _Unspec()) -> RespondFeeEstimates: ...
 
 class SubEpochData:
     reward_chain_hash: bytes32
     num_blocks_overflow: uint8
     new_sub_slot_iters: Optional[uint64]
     new_difficulty: Optional[uint64]
@@ -3434,17 +3491,17 @@
     def from_bytes_unchecked(bytes) -> SubEpochData: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubEpochData, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubEpochData: ...
+    def from_json_dict(json_dict: Any) -> SubEpochData: ...
     def replace(self, *, reward_chain_hash: Union[ bytes32, _Unspec] = _Unspec(),
         num_blocks_overflow: Union[ uint8, _Unspec] = _Unspec(),
         new_sub_slot_iters: Union[ Optional[uint64], _Unspec] = _Unspec(),
         new_difficulty: Union[ Optional[uint64], _Unspec] = _Unspec()) -> SubEpochData: ...
 
 class SubSlotData:
     proof_of_space: Optional[ProofOfSpace]
@@ -3489,17 +3546,17 @@
     def from_bytes_unchecked(bytes) -> SubSlotData: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubSlotData, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubSlotData: ...
+    def from_json_dict(json_dict: Any) -> SubSlotData: ...
     def replace(self, *, proof_of_space: Union[ Optional[ProofOfSpace], _Unspec] = _Unspec(),
         cc_signage_point: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         cc_infusion_point: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         icc_infusion_point: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
         cc_sp_vdf_info: Union[ Optional[VDFInfo], _Unspec] = _Unspec(),
         signage_point_index: Union[ Optional[uint8], _Unspec] = _Unspec(),
         cc_slot_end: Union[ Optional[VDFProof], _Unspec] = _Unspec(),
@@ -3531,17 +3588,17 @@
     def from_bytes_unchecked(bytes) -> SubEpochChallengeSegment: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubEpochChallengeSegment, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubEpochChallengeSegment: ...
+    def from_json_dict(json_dict: Any) -> SubEpochChallengeSegment: ...
     def replace(self, *, sub_epoch_n: Union[ uint32, _Unspec] = _Unspec(),
         sub_slots: Union[ List[SubSlotData], _Unspec] = _Unspec(),
         rc_slot_end_info: Union[ Optional[VDFInfo], _Unspec] = _Unspec()) -> SubEpochChallengeSegment: ...
 
 class SubEpochSegments:
     challenge_segments: List[SubEpochChallengeSegment]
     def __init__(
@@ -3559,17 +3616,17 @@
     def from_bytes_unchecked(bytes) -> SubEpochSegments: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[SubEpochSegments, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> SubEpochSegments: ...
+    def from_json_dict(json_dict: Any) -> SubEpochSegments: ...
     def replace(self, *, challenge_segments: Union[ List[SubEpochChallengeSegment], _Unspec] = _Unspec()) -> SubEpochSegments: ...
 
 class RecentChainData:
     recent_chain_data: List[HeaderBlock]
     def __init__(
         self,
         recent_chain_data: Sequence[HeaderBlock]
@@ -3585,17 +3642,17 @@
     def from_bytes_unchecked(bytes) -> RecentChainData: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[RecentChainData, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> RecentChainData: ...
+    def from_json_dict(json_dict: Any) -> RecentChainData: ...
     def replace(self, *, recent_chain_data: Union[ List[HeaderBlock], _Unspec] = _Unspec()) -> RecentChainData: ...
 
 class ProofBlockHeader:
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlock
     def __init__(
         self,
@@ -3613,17 +3670,17 @@
     def from_bytes_unchecked(bytes) -> ProofBlockHeader: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[ProofBlockHeader, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> ProofBlockHeader: ...
+    def from_json_dict(json_dict: Any) -> ProofBlockHeader: ...
     def replace(self, *, finished_sub_slots: Union[ List[EndOfSubSlotBundle], _Unspec] = _Unspec(),
         reward_chain_block: Union[ RewardChainBlock, _Unspec] = _Unspec()) -> ProofBlockHeader: ...
 
 class WeightProof:
     sub_epochs: List[SubEpochData]
     sub_epoch_segments: List[SubEpochChallengeSegment]
     recent_chain_data: List[HeaderBlock]
@@ -3644,13 +3701,162 @@
     def from_bytes_unchecked(bytes) -> WeightProof: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[WeightProof, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> WeightProof: ...
+    def from_json_dict(json_dict: Any) -> WeightProof: ...
     def replace(self, *, sub_epochs: Union[ List[SubEpochData], _Unspec] = _Unspec(),
         sub_epoch_segments: Union[ List[SubEpochChallengeSegment], _Unspec] = _Unspec(),
         recent_chain_data: Union[ List[HeaderBlock], _Unspec] = _Unspec()) -> WeightProof: ...
+
+class ConsensusConstants:
+    SLOT_BLOCKS_TARGET: uint32
+    MIN_BLOCKS_PER_CHALLENGE_BLOCK: uint8
+    MAX_SUB_SLOT_BLOCKS: uint32
+    NUM_SPS_SUB_SLOT: uint32
+    SUB_SLOT_ITERS_STARTING: uint64
+    DIFFICULTY_CONSTANT_FACTOR: uint128
+    DIFFICULTY_STARTING: uint64
+    DIFFICULTY_CHANGE_MAX_FACTOR: uint32
+    SUB_EPOCH_BLOCKS: uint32
+    EPOCH_BLOCKS: uint32
+    SIGNIFICANT_BITS: uint8
+    DISCRIMINANT_SIZE_BITS: uint16
+    NUMBER_ZERO_BITS_PLOT_FILTER: uint8
+    MIN_PLOT_SIZE: uint8
+    MAX_PLOT_SIZE: uint8
+    SUB_SLOT_TIME_TARGET: uint16
+    NUM_SP_INTERVALS_EXTRA: uint8
+    MAX_FUTURE_TIME2: uint32
+    NUMBER_OF_TIMESTAMPS: uint8
+    GENESIS_CHALLENGE: bytes32
+    AGG_SIG_ME_ADDITIONAL_DATA: bytes32
+    GENESIS_PRE_FARM_POOL_PUZZLE_HASH: bytes32
+    GENESIS_PRE_FARM_FARMER_PUZZLE_HASH: bytes32
+    MAX_VDF_WITNESS_SIZE: uint8
+    MEMPOOL_BLOCK_BUFFER: uint8
+    MAX_COIN_AMOUNT: uint64
+    MAX_BLOCK_COST_KLVM: uint64
+    COST_PER_BYTE: uint64
+    WEIGHT_PROOF_THRESHOLD: uint8
+    WEIGHT_PROOF_RECENT_BLOCKS: uint32
+    MAX_BLOCK_COUNT_PER_REQUESTS: uint32
+    BLOCKS_CACHE_SIZE: uint32
+    MAX_GENERATOR_SIZE: uint32
+    MAX_GENERATOR_REF_LIST_SIZE: uint32
+    POOL_SUB_SLOT_ITERS: uint64
+    SOFT_FORK2_HEIGHT: uint32
+    SOFT_FORK4_HEIGHT: uint32
+    HARD_FORK_HEIGHT: uint32
+    HARD_FORK_FIX_HEIGHT: uint32
+    PLOT_FILTER_128_HEIGHT: uint32
+    PLOT_FILTER_64_HEIGHT: uint32
+    PLOT_FILTER_32_HEIGHT: uint32
+    def __init__(
+        self,
+        SLOT_BLOCKS_TARGET: uint32,
+        MIN_BLOCKS_PER_CHALLENGE_BLOCK: uint8,
+        MAX_SUB_SLOT_BLOCKS: uint32,
+        NUM_SPS_SUB_SLOT: uint32,
+        SUB_SLOT_ITERS_STARTING: uint64,
+        DIFFICULTY_CONSTANT_FACTOR: uint128,
+        DIFFICULTY_STARTING: uint64,
+        DIFFICULTY_CHANGE_MAX_FACTOR: uint32,
+        SUB_EPOCH_BLOCKS: uint32,
+        EPOCH_BLOCKS: uint32,
+        SIGNIFICANT_BITS: uint8,
+        DISCRIMINANT_SIZE_BITS: uint16,
+        NUMBER_ZERO_BITS_PLOT_FILTER: uint8,
+        MIN_PLOT_SIZE: uint8,
+        MAX_PLOT_SIZE: uint8,
+        SUB_SLOT_TIME_TARGET: uint16,
+        NUM_SP_INTERVALS_EXTRA: uint8,
+        MAX_FUTURE_TIME2: uint32,
+        NUMBER_OF_TIMESTAMPS: uint8,
+        GENESIS_CHALLENGE: bytes,
+        AGG_SIG_ME_ADDITIONAL_DATA: bytes,
+        GENESIS_PRE_FARM_POOL_PUZZLE_HASH: bytes,
+        GENESIS_PRE_FARM_FARMER_PUZZLE_HASH: bytes,
+        MAX_VDF_WITNESS_SIZE: uint8,
+        MEMPOOL_BLOCK_BUFFER: uint8,
+        MAX_COIN_AMOUNT: uint64,
+        MAX_BLOCK_COST_KLVM: uint64,
+        COST_PER_BYTE: uint64,
+        WEIGHT_PROOF_THRESHOLD: uint8,
+        WEIGHT_PROOF_RECENT_BLOCKS: uint32,
+        MAX_BLOCK_COUNT_PER_REQUESTS: uint32,
+        BLOCKS_CACHE_SIZE: uint32,
+        MAX_GENERATOR_SIZE: uint32,
+        MAX_GENERATOR_REF_LIST_SIZE: uint32,
+        POOL_SUB_SLOT_ITERS: uint64,
+        SOFT_FORK2_HEIGHT: uint32,
+        SOFT_FORK4_HEIGHT: uint32,
+        HARD_FORK_HEIGHT: uint32,
+        HARD_FORK_FIX_HEIGHT: uint32,
+        PLOT_FILTER_128_HEIGHT: uint32,
+        PLOT_FILTER_64_HEIGHT: uint32,
+        PLOT_FILTER_32_HEIGHT: uint32
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> ConsensusConstants: ...
+    def __copy__(self) -> ConsensusConstants: ...
+    @staticmethod
+    def from_bytes(bytes) -> ConsensusConstants: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> ConsensusConstants: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[ConsensusConstants, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> ConsensusConstants: ...
+    def replace(self, *, SLOT_BLOCKS_TARGET: Union[ uint32, _Unspec] = _Unspec(),
+        MIN_BLOCKS_PER_CHALLENGE_BLOCK: Union[ uint8, _Unspec] = _Unspec(),
+        MAX_SUB_SLOT_BLOCKS: Union[ uint32, _Unspec] = _Unspec(),
+        NUM_SPS_SUB_SLOT: Union[ uint32, _Unspec] = _Unspec(),
+        SUB_SLOT_ITERS_STARTING: Union[ uint64, _Unspec] = _Unspec(),
+        DIFFICULTY_CONSTANT_FACTOR: Union[ uint128, _Unspec] = _Unspec(),
+        DIFFICULTY_STARTING: Union[ uint64, _Unspec] = _Unspec(),
+        DIFFICULTY_CHANGE_MAX_FACTOR: Union[ uint32, _Unspec] = _Unspec(),
+        SUB_EPOCH_BLOCKS: Union[ uint32, _Unspec] = _Unspec(),
+        EPOCH_BLOCKS: Union[ uint32, _Unspec] = _Unspec(),
+        SIGNIFICANT_BITS: Union[ uint8, _Unspec] = _Unspec(),
+        DISCRIMINANT_SIZE_BITS: Union[ uint16, _Unspec] = _Unspec(),
+        NUMBER_ZERO_BITS_PLOT_FILTER: Union[ uint8, _Unspec] = _Unspec(),
+        MIN_PLOT_SIZE: Union[ uint8, _Unspec] = _Unspec(),
+        MAX_PLOT_SIZE: Union[ uint8, _Unspec] = _Unspec(),
+        SUB_SLOT_TIME_TARGET: Union[ uint16, _Unspec] = _Unspec(),
+        NUM_SP_INTERVALS_EXTRA: Union[ uint8, _Unspec] = _Unspec(),
+        MAX_FUTURE_TIME2: Union[ uint32, _Unspec] = _Unspec(),
+        NUMBER_OF_TIMESTAMPS: Union[ uint8, _Unspec] = _Unspec(),
+        GENESIS_CHALLENGE: Union[ bytes32, _Unspec] = _Unspec(),
+        AGG_SIG_ME_ADDITIONAL_DATA: Union[ bytes32, _Unspec] = _Unspec(),
+        GENESIS_PRE_FARM_POOL_PUZZLE_HASH: Union[ bytes32, _Unspec] = _Unspec(),
+        GENESIS_PRE_FARM_FARMER_PUZZLE_HASH: Union[ bytes32, _Unspec] = _Unspec(),
+        MAX_VDF_WITNESS_SIZE: Union[ uint8, _Unspec] = _Unspec(),
+        MEMPOOL_BLOCK_BUFFER: Union[ uint8, _Unspec] = _Unspec(),
+        MAX_COIN_AMOUNT: Union[ uint64, _Unspec] = _Unspec(),
+        MAX_BLOCK_COST_KLVM: Union[ uint64, _Unspec] = _Unspec(),
+        COST_PER_BYTE: Union[ uint64, _Unspec] = _Unspec(),
+        WEIGHT_PROOF_THRESHOLD: Union[ uint8, _Unspec] = _Unspec(),
+        WEIGHT_PROOF_RECENT_BLOCKS: Union[ uint32, _Unspec] = _Unspec(),
+        MAX_BLOCK_COUNT_PER_REQUESTS: Union[ uint32, _Unspec] = _Unspec(),
+        BLOCKS_CACHE_SIZE: Union[ uint32, _Unspec] = _Unspec(),
+        MAX_GENERATOR_SIZE: Union[ uint32, _Unspec] = _Unspec(),
+        MAX_GENERATOR_REF_LIST_SIZE: Union[ uint32, _Unspec] = _Unspec(),
+        POOL_SUB_SLOT_ITERS: Union[ uint64, _Unspec] = _Unspec(),
+        SOFT_FORK2_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        SOFT_FORK4_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        HARD_FORK_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        HARD_FORK_FIX_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        PLOT_FILTER_128_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        PLOT_FILTER_64_HEIGHT: Union[ uint32, _Unspec] = _Unspec(),
+        PLOT_FILTER_32_HEIGHT: Union[ uint32, _Unspec] = _Unspec()) -> ConsensusConstants: ...
```

### Comparing `chik_rs-0.6.1/wheel/generate_type_stubs.py` & `chik_rs-0.7.0/wheel/generate_type_stubs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from pathlib import Path
-from typing import Any, List, Optional, Tuple
+from typing import List, Optional, Tuple, TextIO
 from glob import glob
 
-output_file = Path(__file__).parent.resolve() / "chik_rs.pyi"
-input_dir = Path(__file__).parent.parent.resolve() / "crates" / "chik-protocol" / "src"
+output_file = Path(__file__).parent.resolve() / "python" / "chik_rs" / "chik_rs.pyi"
+crates_dir = Path(__file__).parent.parent.resolve() / "crates"
+input_dir = crates_dir / "chik-protocol" / "src"
 
 # enums are exposed to python as int
 enums = set(["NodeType", "ProtocolMessageTypes"])
 
+
 def transform_type(m: str) -> str:
     n, t = m.split(":")
     if "List[" in t:
         t = t.replace("List[", "Sequence[")
     elif "bytes32" == t.strip():
         t = " bytes"
     elif t.strip() in enums:
         t = " int"
     return f"{n}:{t}"
 
 
-def print_class(f: Any, name: str, members: List[str], extra: Optional[List[str]] = None):
+def print_class(
+    file: TextIO, name: str, members: List[str], extra: Optional[List[str]] = None
+):
 
     # f-strings don't allow backslashes, which makes it a bit tricky to
     # manipulate strings with newlines
     nl = "\n"
-    def add_indent(x):
-        return '\n    ' + x
 
-    init_args = ''.join([(',\n        ' + transform_type(x)) for x in members])
+    def add_indent(x: str):
+        return "\n    " + x
+
+    init_args = "".join([(",\n        " + transform_type(x)) for x in members])
 
     all_replace_parameters = []
     for m in members:
-        replace_param_name, replace_type = m.split(':')
-        all_replace_parameters.append(f"{replace_param_name}: Union[{replace_type}, _Unspec] = _Unspec()")
+        replace_param_name, replace_type = m.split(":")
+        all_replace_parameters.append(
+            f"{replace_param_name}: Union[{replace_type}, _Unspec] = _Unspec()"
+        )
 
     if extra is not None:
         members.extend(extra)
-    members = ''.join(map(add_indent, members));
 
-    f.write(
+    file.write(
         f"""
-class {name}:{members}
+class {name}:{"".join(map(add_indent, members))}
     def __init__(
         self{init_args}
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> {name}: ...
@@ -55,34 +61,38 @@
     def from_bytes_unchecked(bytes) -> {name}: ...
     @staticmethod
     def parse_rust(ReadableBuffer, bool = False) -> Tuple[{name}, int]: ...
     def to_bytes(self) -> bytes: ...
     def __bytes__(self) -> bytes: ...
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
-    def to_json_dict(self) -> Dict[str, Any]: ...
+    def to_json_dict(self) -> Any: ...
     @staticmethod
-    def from_json_dict(json_dict: Dict[str, Any]) -> {name}: ...
+    def from_json_dict(json_dict: Any) -> {name}: ...
 """
     )
 
     if len(all_replace_parameters) > 0:
         indent = ",\n        "
-        f.write(
+        file.write(
             f"""    def replace(self, *, {indent.join(all_replace_parameters)}) -> {name}: ...
-""")
+"""
+        )
 
 
 def rust_type_to_python(t: str) -> str:
     ret = (
         t.replace("<", "[")
         .replace(">", "]")
+        .replace("(", "Tuple[")
+        .replace(")", "]")
         .replace("Vec", "List")
         .replace("Option", "Optional")
         .replace("Bytes", "bytes")
+        .replace("String", "str")
         .replace("u8", "uint8")
         .replace("u16", "uint16")
         .replace("u32", "uint32")
         .replace("u64", "uint64")
         .replace("u128", "uint128")
         .replace("i8", "int8")
         .replace("i16", "int16")
@@ -92,16 +102,16 @@
         .strip()
     )
     if ret in enums:
         ret = "int"
     return ret
 
 
-def parse_rust_source(filename: str) -> List[Tuple[str, List[str]]]:
-    ret: List[Tuple[str], List[str]] = []
+def parse_rust_source(filename: str, upper_case: bool) -> List[Tuple[str, List[str]]]:
+    ret: List[Tuple[str, List[str]]] = []
     in_struct: Optional[str] = None
     members: List[str] = []
     with open(filename) as f:
         for line in f:
             if not in_struct:
                 if line.startswith("pub struct ") and "{" in line:
                     in_struct = line.split("pub struct ")[1].split("{")[0].strip()
@@ -125,33 +135,32 @@
 
             # we're parsing members
             # ignore macros
             if line.strip().startswith("#"):
                 continue
 
             # a field
-            if ":" in line:
+            if ":" in line and "///" not in line:
                 name, rust_type = line.split("//")[0].strip().split(":")
                 # members are separated by , in rust. Strip that off
                 try:
-                    rust_type, line = rust_type.rsplit(",",1)
+                    rust_type, line = rust_type.rsplit(",", 1)
                 except:
-                    rust_type, line = rust_type.rsplit("}",1)
+                    rust_type, line = rust_type.rsplit("}", 1)
                     line = "}" + line
                 py_type = rust_type_to_python(rust_type)
-                members.append(f"{name}: {py_type}")
+                members.append(f"{name.upper() if upper_case else name}: {py_type}")
 
             # did we reach the end?
             if "}" in line:
                 ret.append((in_struct, members))
                 members = []
                 in_struct = None
                 continue
 
-
     assert in_struct is None
     return ret
 
 
 extra_members = {
     "Coin": [
         "def name(self) -> bytes32: ...",
@@ -223,31 +232,37 @@
         "def sp_iters(self, constants: ConsensusConstants) -> uint64: ...",
         "def ip_iters(self, constants: ConsensusConstants) -> uint64: ...",
         "def sp_total_iters(self, constants: ConsensusConstants) -> uint128: ...",
     ],
 }
 
 classes = []
-for f in sorted(glob(str(input_dir / "*.rs"))):
-    if f.endswith("bytes.rs") or f.endswith("lazy_node.rs"):
+for filepath in sorted(glob(str(input_dir / "*.rs"))):
+    if filepath.endswith("bytes.rs") or filepath.endswith("lazy_node.rs"):
         continue
-    classes.extend(parse_rust_source(f))
+    classes.extend(parse_rust_source(filepath, upper_case=False))
+
+classes.extend(
+    parse_rust_source(
+        str(crates_dir / "chik-consensus" / "src" / "consensus_constants.rs"),
+        upper_case=True,
+    )
+)
 
-with open(output_file, "w") as f:
-    f.write(
+with open(output_file, "w") as file:
+    file.write(
         """
 #
 # this file is generated by generate_type_stubs.py
 #
 
-from typing import List, Optional, Sequence, Tuple
-from chik.types.blockchain_format.sized_bytes import bytes32
-from chik.util.ints import uint8, uint16, uint32, uint64, uint128, int8, int16, int32, int64, int128
+from typing import List, Optional, Sequence, Tuple, Union, Dict, Any, ClassVar
+from .sized_bytes import bytes32, bytes100
+from .sized_ints import uint8, uint16, uint32, uint64, uint128, int8, int16, int32, int64
 from chik.types.blockchain_format.program import Program as ChikProgram
-from chik.consensus.constants import ConsensusConstants
 
 ReadableBuffer = Union[bytes, bytearray, memoryview]
 
 class _Unspec:
     pass
 
 def solution_generator(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
@@ -266,14 +281,30 @@
     program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
+def deserialize_proof(
+    proof: bytes
+) -> MerkleSet: ...
+
+def confirm_included_already_hashed(
+    root: bytes32,
+    item: bytes32,
+    proof: bytes,
+) -> bool: ...
+
+def confirm_not_included_already_hashed(
+    root: bytes32,
+    item: bytes32,
+    proof: bytes,
+) -> bool: ...
+
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
 AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
 ENABLE_SOFTFORK_CONDITION: int = ...
 ENABLE_MESSAGE_CONDITIONS: int = ...
@@ -288,27 +319,27 @@
 ELIGIBLE_FOR_DEDUP: int = ...
 ELIGIBLE_FOR_FF: int = ...
 
 NO_UNKNOWN_OPS: int = ...
 
 def run_chik_program(
     program: bytes, args: bytes, max_cost: int, flags: int
-) -> Pair[int, LazyNode]: ...
+) -> Tuple[int, LazyNode]: ...
 
 class LazyNode:
-    def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
-    def atom() -> bytes: ...
+    pair: Optional[Tuple[LazyNode, LazyNode]]
+    atom: Optional[bytes]
 
 def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class AugSchemeMPL:
     @staticmethod
-    def sign(pk: PrivateKey, msg: bytes, prepend_pk: G1Element = None) -> G2Element: ...
+    def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
     def verify(pk: G1Element, msg: bytes, sig: G2Element) -> bool: ...
     @staticmethod
     def aggregate_verify(pks: Sequence[G1Element], msgs: Sequence[bytes], sig: G2Element) -> bool: ...
     @staticmethod
@@ -317,62 +348,82 @@
     def g2_from_message(msg: bytes) -> G2Element: ...
     @staticmethod
     def derive_child_sk(pk: PrivateKey, index: int) -> PrivateKey: ...
     @staticmethod
     def derive_child_sk_unhardened(pk: PrivateKey, index: int) -> PrivateKey: ...
     @staticmethod
     def derive_child_pk_unhardened(pk: G1Element, index: int) -> G1Element: ...
+
+class MerkleSet:
+    def get_root(self) -> bytes32: ...
+    def is_included_already_hashed(self, to_check: bytes) -> Tuple[bool, bytes]: ...
+    def __init__(
+        self,
+        leafs: List[bytes32],
+    ) -> None: ...
 """
     )
 
-    print_class(f, "G1Element", [], [
-        "SIZE: ClassVar[int] = ...",
-        "def __new__(cls) -> G1Element: ...",
-        "def get_fingerprint(self) -> int: ...",
-        "def pair(self, other: G2Element) -> GTElement: ...",
-        "@staticmethod",
-        "def from_bytes_unchecked(b: bytes) -> G1Element: ...",
-        "@staticmethod",
-        "def generator() -> G1Element: ...",
-        "def __str__(self) -> str: ...",
-        "def __repr__(self) -> str: ...",
-        "def __add__(self, other: G1Element) -> G1Element: ...",
-        "def __iadd__(self, other: G1Element) -> G1Element: ...",
-    ])
-    print_class(f, "G2Element", [], [
-        "SIZE: ClassVar[int] = ...",
-        "def __new__(cls) -> G2Element: ...",
-        "@staticmethod",
-        "def from_bytes_unchecked(b: bytes) -> G2Element: ...",
-        "def pair(self, other: G1Element) -> GTElement: ...",
-        "@staticmethod",
-        "def generator() -> G2Element: ...",
-        "def __str__(self) -> str: ...",
-        "def __repr__(self) -> str: ...",
-        "def __add__(self, other: G2Element) -> G2Element: ...",
-        "def __iadd__(self, other: G2Element) -> G2Element: ...",
-        ])
-    print_class(f, "GTElement", [], [
-        "SIZE: ClassVar[int] = ...",
-        "@staticmethod",
-        "def from_bytes_unchecked(b: bytes) -> GTElement: ...",
-        "def __str__(self) -> str: ...",
-        "def __repr__(self) -> str: ...",
-        "def __mul__(self, rhs: GTElement) -> GTElement: ...",
-        "def __imul__(self, rhs: GTElement) -> GTElement : ...",
-        ])
-    print_class(f, "PrivateKey", [], [
-        "PRIVATE_KEY_SIZE: ClassVar[int] = ...",
-        "def sign_g2(self, msg: bytes, dst: bytes) -> G2Element: ...",
-        "def get_g1(self) -> G1Element: ...",
-        "def __str__(self) -> str: ...",
-        "def __repr__(self) -> str: ...",
-        ])
+    print_class(
+        file,
+        "G1Element",
+        [],
+        [
+            "SIZE: ClassVar[int] = ...",
+            "def __new__(cls) -> G1Element: ...",
+            "def get_fingerprint(self) -> int: ...",
+            "def pair(self, other: G2Element) -> GTElement: ...",
+            "@staticmethod",
+            "def generator() -> G1Element: ...",
+            "def __str__(self) -> str: ...",
+            "def __add__(self, other: G1Element) -> G1Element: ...",
+            "def __iadd__(self, other: G1Element) -> G1Element: ...",
+        ],
+    )
+    print_class(
+        file,
+        "G2Element",
+        [],
+        [
+            "SIZE: ClassVar[int] = ...",
+            "def __new__(cls) -> G2Element: ...",
+            "def pair(self, other: G1Element) -> GTElement: ...",
+            "@staticmethod",
+            "def generator() -> G2Element: ...",
+            "def __str__(self) -> str: ...",
+            "def __add__(self, other: G2Element) -> G2Element: ...",
+            "def __iadd__(self, other: G2Element) -> G2Element: ...",
+        ],
+    )
+    print_class(
+        file,
+        "GTElement",
+        [],
+        [
+            "SIZE: ClassVar[int] = ...",
+            "def __str__(self) -> str: ...",
+            "def __mul__(self, rhs: GTElement) -> GTElement: ...",
+            "def __imul__(self, rhs: GTElement) -> GTElement : ...",
+        ],
+    )
+    print_class(
+        file,
+        "PrivateKey",
+        [],
+        [
+            "PRIVATE_KEY_SIZE: ClassVar[int] = ...",
+            "def sign_g2(self, msg: bytes, dst: bytes) -> G2Element: ...",
+            "def get_g1(self) -> G1Element: ...",
+            "def __str__(self) -> str: ...",
+        ],
+    )
 
-    print_class(f, "Spend",
+    print_class(
+        file,
+        "Spend",
         [
             "coin_id: bytes",
             "parent_id: bytes",
             "puzzle_hash: bytes",
             "coin_amount: int",
             "height_relative: Optional[int]",
             "seconds_relative: Optional[int]",
@@ -388,24 +439,26 @@
             "agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]",
             "agg_sig_parent_amount: List[Tuple[bytes, bytes]]",
             "agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]",
             "flags: int",
         ],
     )
 
-    print_class(f, "SpendBundleConditions",
+    print_class(
+        file,
+        "SpendBundleConditions",
         [
             "spends: List[Spend]",
             "reserve_fee: int",
             "height_absolute: int",
             "seconds_absolute: int",
             "before_height_absolute: Optional[int]",
             "before_seconds_absolute: Optional[int]",
             "agg_sig_unsafe: List[Tuple[bytes, bytes]]",
             "cost: int",
             "removal_amount: int",
             "addition_amount: int",
         ],
     )
 
-    for c in classes:
-        print_class(f, c[0], c[1], extra_members.get(c[0]))
+    for item in classes:
+        print_class(file, item[0], item[1], extra_members.get(item[0]))
```

### Comparing `chik_rs-0.6.1/wheel/src/api.rs` & `chik_rs-0.7.0/wheel/src/api.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-use crate::run_generator::{
-    convert_spend_bundle_conds, run_block_generator, run_block_generator2, PySpend,
-    PySpendBundleConditions,
-};
+use crate::run_generator::{run_block_generator, run_block_generator2};
 use chik_consensus::allocator::make_allocator;
+use chik_consensus::consensus_constants::ConsensusConstants;
 use chik_consensus::gen::conditions::MempoolVisitor;
 use chik_consensus::gen::flags::{
     AGG_SIG_ARGS, ALLOW_BACKREFS, ANALYZE_SPENDS, COND_ARGS_NIL, ENABLE_MESSAGE_CONDITIONS,
     ENABLE_SOFTFORK_CONDITION, MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL, NO_UNKNOWN_CONDS,
     STRICT_ARGS_COUNT,
 };
+use chik_consensus::gen::owned_conditions::{OwnedSpend, OwnedSpendBundleConditions};
 use chik_consensus::gen::run_puzzle::run_puzzle as native_run_puzzle;
 use chik_consensus::gen::solution_generator::solution_generator as native_solution_generator;
 use chik_consensus::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
 use chik_consensus::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
+use chik_consensus::merkle_tree::{validate_merkle_proof, MerkleSet};
 use chik_protocol::{
     BlockRecord, Bytes32, ChallengeBlockInfo, ChallengeChainSubSlot, ClassgroupElement, Coin,
     CoinSpend, CoinState, CoinStateUpdate, EndOfSubSlotBundle, Foliage, FoliageBlockData,
     FoliageTransactionBlock, FullBlock, HeaderBlock, InfusedChallengeChainSubSlot, NewCompactVDF,
     NewPeak, NewPeakWallet, NewSignagePointOrEndOfSubSlot, NewTransaction, NewUnfinishedBlock,
     PoolTarget, Program, ProofBlockHeader, ProofOfSpace, PuzzleSolutionResponse, RecentChainData,
     RegisterForCoinUpdates, RegisterForPhUpdates, RejectAdditionsRequest, RejectBlock,
@@ -34,15 +34,15 @@
     RewardChainSubSlot, SendTransaction, SpendBundle, SubEpochChallengeSegment, SubEpochData,
     SubEpochSegments, SubEpochSummary, SubSlotData, SubSlotProofs, TimestampedPeerInfo,
     TransactionAck, TransactionsInfo, UnfinishedBlock, VDFInfo, VDFProof, WeightProof,
 };
 use klvm_utils::tree_hash_from_bytes;
 use klvmr::{ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, LIMIT_HEAP, NO_UNKNOWN_OPS};
 use pyo3::buffer::PyBuffer;
-use pyo3::exceptions::PyRuntimeError;
+use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 use pyo3::types::PyList;
 use pyo3::types::PyTuple;
 use pyo3::wrap_pyfunction;
 use std::iter::zip;
 
@@ -74,14 +74,35 @@
     for b in values {
         buffer.push(b.as_bytes().try_into()?);
     }
     Ok(PyBytes::new(py, &compute_merkle_root_impl(&mut buffer)))
 }
 
 #[pyfunction]
+pub fn confirm_included_already_hashed(
+    root: Bytes32,
+    item: Bytes32,
+    proof: &[u8],
+) -> PyResult<bool> {
+    validate_merkle_proof(proof, (&item).into(), (&root).into())
+        .map_err(|_| PyValueError::new_err("Invalid proof"))
+}
+
+#[pyfunction]
+pub fn confirm_not_included_already_hashed(
+    root: Bytes32,
+    item: Bytes32,
+    proof: &[u8],
+) -> PyResult<bool> {
+    validate_merkle_proof(proof, (&item).into(), (&root).into())
+        .map_err(|_| PyValueError::new_err("Invalid proof"))
+        .map(|r| !r)
+}
+
+#[pyfunction]
 pub fn tree_hash(py: Python, blob: PyBuffer<u8>) -> PyResult<&PyBytes> {
     if !blob.is_c_contiguous() {
         panic!("tree_hash() must be called with a contiguous buffer");
     }
     let slice =
         unsafe { std::slice::from_raw_parts(blob.buf_ptr() as *const u8, blob.len_bytes()) };
     Ok(PyBytes::new(py, &tree_hash_from_bytes(slice)?))
@@ -152,20 +173,20 @@
 fn run_puzzle(
     puzzle: &[u8],
     solution: &[u8],
     parent_id: &[u8],
     amount: u64,
     max_cost: Cost,
     flags: u32,
-) -> PyResult<PySpendBundleConditions> {
+) -> PyResult<OwnedSpendBundleConditions> {
     let mut a = make_allocator(LIMIT_HEAP);
     let conds = native_run_puzzle::<MempoolVisitor>(
         &mut a, puzzle, solution, parent_id, amount, max_cost, flags,
     )?;
-    Ok(convert_spend_bundle_conds(&a, conds))
+    Ok(OwnedSpendBundleConditions::from(&a, conds))
 }
 
 // this is like a CoinSpend but with references to the puzzle and solution,
 // rather than owning them
 type CoinSpendRef<'a> = (Coin, &'a [u8], &'a [u8]);
 
 fn convert_list_of_tuples(spends: &PyAny) -> PyResult<Vec<CoinSpendRef>> {
@@ -332,24 +353,32 @@
     m.add_function(wrap_pyfunction!(run_block_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_block_generator2, m)?)?;
     m.add_function(wrap_pyfunction!(run_puzzle, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator, m)?)?;
     m.add_function(wrap_pyfunction!(solution_generator_backrefs, m)?)?;
     m.add_function(wrap_pyfunction!(supports_fast_forward, m)?)?;
     m.add_function(wrap_pyfunction!(fast_forward_singleton, m)?)?;
-    m.add_class::<PySpendBundleConditions>()?;
+    m.add_class::<OwnedSpendBundleConditions>()?;
     m.add(
         "ELIGIBLE_FOR_DEDUP",
         chik_consensus::gen::conditions::ELIGIBLE_FOR_DEDUP,
     )?;
     m.add(
         "ELIGIBLE_FOR_FF",
         chik_consensus::gen::conditions::ELIGIBLE_FOR_FF,
     )?;
-    m.add_class::<PySpend>()?;
+    m.add_class::<OwnedSpend>()?;
+
+    // constants
+    m.add_class::<ConsensusConstants>()?;
+
+    // merkle tree
+    m.add_class::<MerkleSet>()?;
+    m.add_function(wrap_pyfunction!(confirm_included_already_hashed, m)?)?;
+    m.add_function(wrap_pyfunction!(confirm_not_included_already_hashed, m)?)?;
 
     // klvm functions
     m.add("COND_ARGS_NIL", COND_ARGS_NIL)?;
     m.add("NO_UNKNOWN_CONDS", NO_UNKNOWN_CONDS)?;
     m.add("STRICT_ARGS_COUNT", STRICT_ARGS_COUNT)?;
     m.add("AGG_SIG_ARGS", AGG_SIG_ARGS)?;
     m.add("ENABLE_FIXED_DIV", ENABLE_FIXED_DIV)?;
```

### Comparing `chik_rs-0.6.1/wheel/src/run_program.rs` & `chik_rs-0.7.0/wheel/src/run_program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.6.1/Cargo.lock` & `chik_rs-0.7.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -272,22 +272,22 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chik"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "chik-client",
  "chik-consensus",
  "chik-protocol",
  "chik-ssl",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "chik-wallet",
  "klvm-traits",
  "klvm-utils",
 ]
 
 [[package]]
 name = "chik-bls"
@@ -304,20 +304,20 @@
  "sha2",
  "thiserror",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chik-bls"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "anyhow",
  "arbitrary",
  "blst",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "chik_py_streamable_macro",
  "criterion",
  "hex",
  "hkdf",
  "pyo3",
  "rand",
  "rstest 0.17.0",
@@ -326,74 +326,78 @@
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chik-bls-fuzz"
 version = "0.0.0"
 dependencies = [
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "libfuzzer-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "chik-client"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "futures-util",
  "thiserror",
  "tokio",
  "tokio-tungstenite",
  "tungstenite",
 ]
 
 [[package]]
 name = "chik-consensus"
-version = "0.6.1"
+version = "0.7.0"
 dependencies = [
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "chik-wallet",
+ "chik_py_streamable_macro",
+ "chik_streamable_macro 0.6.0",
  "criterion",
  "hex",
  "hex-literal",
  "klvm-derive",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "num-traits",
  "pyo3",
+ "rand",
  "rstest 0.16.0",
+ "sha2",
  "text-diff",
  "thiserror",
 ]
 
 [[package]]
 name = "chik-fuzz"
 version = "0.6.0"
 dependencies = [
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "hex-literal",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "libfuzzer-sys",
 ]
 
 [[package]]
 name = "chik-protocol"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "arbitrary",
- "chik-bls 0.6.0",
- "chik-traits 0.6.0",
+ "chik-bls 0.7.0",
+ "chik-traits 0.7.0",
  "chik_py_streamable_macro",
  "chik_streamable_macro 0.6.0",
  "hex",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "pyo3",
@@ -403,44 +407,43 @@
 
 [[package]]
 name = "chik-protocol-fuzz"
 version = "0.0.0"
 dependencies = [
  "arbitrary",
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "hex",
  "klvm-traits",
  "klvmr",
  "libfuzzer-sys",
  "sha2",
 ]
 
 [[package]]
 name = "chik-ssl"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "lazy_static",
  "rand",
  "rcgen",
  "rsa",
- "rustls",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "chik-tools"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "blocking-threadpool",
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "chik-wallet",
  "clap",
  "hex",
  "hex-literal",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
@@ -458,30 +461,30 @@
  "hex",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "chik-traits"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "chik_py_streamable_macro",
  "chik_streamable_macro 0.6.0",
  "hex",
  "pyo3",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "chik-wallet"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "arbitrary",
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "chik-protocol",
  "hex",
  "hex-literal",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "num-bigint",
@@ -497,30 +500,30 @@
  "klvmr",
  "libfuzzer-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "chik_py_streamable_macro"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 2.0.40",
 ]
 
 [[package]]
 name = "chik_rs"
-version = "0.6.1"
+version = "0.7.0"
 dependencies = [
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.6.0",
+ "chik-traits 0.7.0",
  "chik_py_streamable_macro",
  "chik_streamable_macro 0.6.0",
  "hex",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "pyo3",
@@ -1266,29 +1269,29 @@
  "proc-macro2",
  "quote",
  "syn 2.0.40",
 ]
 
 [[package]]
 name = "klvm-traits"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
- "chik-bls 0.6.0",
+ "chik-bls 0.7.0",
  "hex",
  "hex-literal",
  "klvm-derive",
  "klvmr",
  "num-bigint",
  "pyo3",
  "thiserror",
 ]
 
 [[package]]
 name = "klvm-utils"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "hex",
  "klvm-traits",
  "klvmr",
  "rstest 0.16.0",
 ]
 
@@ -1323,15 +1326,15 @@
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
- "spin 0.5.2",
+ "spin",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.151"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
@@ -1836,15 +1839,15 @@
 [[package]]
 name = "rcgen"
 version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52c4f3084aa3bc7dfbba4eff4fab2a54db4324965d8872ab933565e6fbd83bc6"
 dependencies = [
  "pem",
- "ring 0.16.20",
+ "ring",
  "time",
  "x509-parser",
  "yasna",
 ]
 
 [[package]]
 name = "redox_syscall"
@@ -1899,35 +1902,21 @@
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
  "cc",
  "libc",
  "once_cell",
- "spin 0.5.2",
- "untrusted 0.7.1",
+ "spin",
+ "untrusted",
  "web-sys",
  "winapi 0.3.9",
 ]
 
 [[package]]
-name = "ring"
-version = "0.17.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "688c63d65483050968b2a8937f7995f443e27041a0f7700aa59b0822aedebb74"
-dependencies = [
- "cc",
- "getrandom",
- "libc",
- "spin 0.9.8",
- "untrusted 0.9.0",
- "windows-sys 0.48.0",
-]
-
-[[package]]
 name = "rsa"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d0e5124fcb30e76a7e79bfee683a2746db83784b86289f6251b54b7950a0dfc"
 dependencies = [
  "const-oid",
  "digest",
@@ -2049,36 +2038,14 @@
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "rustls"
-version = "0.21.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
-dependencies = [
- "log",
- "ring 0.17.7",
- "rustls-webpki",
- "sct",
-]
-
-[[package]]
-name = "rustls-webpki"
-version = "0.101.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
-dependencies = [
- "ring 0.17.7",
- "untrusted 0.9.0",
-]
-
-[[package]]
 name = "ryu"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "same-file"
@@ -2098,24 +2065,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "sct"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
-dependencies = [
- "ring 0.17.7",
- "untrusted 0.9.0",
-]
-
-[[package]]
 name = "sec1"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3e97a565f76233a6003f9f5c54be1d9c5bdfa3eccfb189469f11ec4901c47dc"
 dependencies = [
  "base16ct",
  "der",
@@ -2222,20 +2179,14 @@
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
-name = "spin"
-version = "0.9.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
-
-[[package]]
 name = "spki"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d91ed6c858b01f942cd56b37a94b3e0a1798290327d1236e4d9cf4eaca44d29d"
 dependencies = [
  "base64ct",
  "der",
@@ -2526,20 +2477,14 @@
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
-name = "untrusted"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
-
-[[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
@@ -2878,15 +2823,15 @@
 dependencies = [
  "asn1-rs",
  "data-encoding",
  "der-parser",
  "lazy_static",
  "nom",
  "oid-registry",
- "ring 0.16.20",
+ "ring",
  "rusticata-macros",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "yasna"
```

### Comparing `chik_rs-0.6.1/Cargo.toml` & `chik_rs-0.7.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["wheel"]
 
 [package]
 name = "chik"
-version = "0.6.0"
+version = "0.7.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "A meta-crate that exports all of the Chik crates in the workspace."
 authors = [
     "Richard Kiss <him@richardkiss.com>",
     "Arvid Norberg <arvid@chiknetwork.com>",
     "Brandon Haggstrom <b.haggstrom@chiknetwork.com>"
@@ -35,23 +35,23 @@
 ssl = ["dep:chik-ssl"]
 traits = ["dep:chik-traits"]
 wallet = ["dep:chik-wallet"]
 klvm-traits = ["dep:klvm-traits"]
 klvm-utils = ["dep:klvm-utils"]
 
 [dependencies]
-chik-bls = { path = "./crates/chik-bls", version = "0.6.0", optional = true }
-chik-client = { path = "./crates/chik-client", version = "0.6.0", optional = true }
-chik-consensus = { path = "./crates/chik-consensus", version = "0.6.1", optional = true }
-chik-protocol = { path = "./crates/chik-protocol", version = "0.6.0", optional = true }
-chik-ssl = { path = "./crates/chik-ssl", version = "0.6.0", optional = true }
-chik-traits = { path = "./crates/chik-traits", version = "0.6.0", optional = true }
-chik-wallet = { path = "./crates/chik-wallet", version = "0.6.0", optional = true }
-klvm-traits = { path = "./crates/klvm-traits", version = "0.6.0", optional = true }
-klvm-utils = { path = "./crates/klvm-utils", version = "0.6.0", optional = true }
+chik-bls = { path = "./crates/chik-bls", version = "0.7.0", optional = true }
+chik-client = { path = "./crates/chik-client", version = "0.7.0", optional = true }
+chik-consensus = { path = "./crates/chik-consensus", version = "0.7.0", optional = true }
+chik-protocol = { path = "./crates/chik-protocol", version = "0.7.0", optional = true }
+chik-ssl = { path = "./crates/chik-ssl", version = "0.7.0", optional = true }
+chik-traits = { path = "./crates/chik-traits", version = "0.7.0", optional = true }
+chik-wallet = { path = "./crates/chik-wallet", version = "0.7.0", optional = true }
+klvm-traits = { path = "./crates/klvm-traits", version = "0.7.0", optional = true }
+klvm-utils = { path = "./crates/klvm-utils", version = "0.7.0", optional = true }
 
 [profile.release]
 lto = "thin"
 
 # This is also necessary in `wheel/Cargo.toml` to make sure the `wheel` crate builds as well.
 # Pin the `blst` dependency to the correct revision, since the fix has not been properly released yet.
 [patch.crates-io]
```

