# Comparing `tmp/bloqade-0.8.0.tar.gz` & `tmp/bloqade-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloqade-0.8.0.tar", last modified: Thu Oct 19 21:10:43 2023, max compression
+gzip compressed data, was "bloqade-0.9.0.tar", last modified: Fri Oct 20 18:41:11 2023, max compression
```

## Comparing `bloqade-0.8.0.tar` & `bloqade-0.9.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    10623 2023-10-19 21:10:20.855418 bloqade-0.8.0/LICENSE
--rw-r--r--   0        0        0     9762 2023-10-19 21:10:20.855418 bloqade-0.8.0/README.md
--rw-r--r--   0        0        0     2903 2023-10-19 21:10:43.095476 bloqade-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1158 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/__init__.py
--rw-r--r--   0        0        0      340 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/atom_arrangement.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/__init__.py
--rw-r--r--   0        0        0      562 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/args.py
--rw-r--r--   0        0        0     4960 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/assign.py
--rw-r--r--   0        0        0     1210 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/backend/__init__.py
--rw-r--r--   0        0        0      852 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/backend/bloqade.py
--rw-r--r--   0        0        0     3107 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/backend/braket.py
--rw-r--r--   0        0        0     3043 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/backend/quera.py
--rw-r--r--   0        0        0      367 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/base.py
--rw-r--r--   0        0        0     3163 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/coupling.py
--rw-r--r--   0        0        0     1149 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/drive.py
--rw-r--r--   0        0        0    11476 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/field.py
--rw-r--r--   0        0        0      487 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/parallelize.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/parse/__init__.py
--rw-r--r--   0        0        0     8561 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/parse/builder.py
--rw-r--r--   0        0        0     2399 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/parse/stream.py
--rw-r--r--   0        0        0     1858 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/parse/trait.py
--rw-r--r--   0        0        0     5754 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/pragmas.py
--rw-r--r--   0        0        0      515 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/route.py
--rw-r--r--   0        0        0      311 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/sequence_builder.py
--rw-r--r--   0        0        0     2403 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/spatial.py
--rw-r--r--   0        0        0     2148 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/start.py
--rw-r--r--   0        0        0      264 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/typing.py
--rw-r--r--   0        0        0    50565 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/builder/waveform.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/common/__init__.py
--rw-r--r--   0        0        0    11885 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/common/assign_variables.py
--rw-r--r--   0        0        0    16763 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/common/json.py
--rw-r--r--   0        0        0    13722 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/emulator_ir.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/hardware/__init__.py
--rw-r--r--   0        0        0     7747 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/hardware/piecewise_constant.py
--rw-r--r--   0        0        0     8011 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/hardware/piecewise_linear.py
--rw-r--r--   0        0        0    25215 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/hardware/quera.py
--rw-r--r--   0        0        0     2576 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/codegen/julia/types.py
--rw-r--r--   0        0        0      144 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/constants.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/emulate/__init__.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/emulate/codegen/__init__.py
--rw-r--r--   0        0        0     8014 2023-10-19 21:10:20.891417 bloqade-0.8.0/src/bloqade/emulate/codegen/hamiltonian.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/ir/__init__.py
--rw-r--r--   0        0        0     4883 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/ir/atom_type.py
--rw-r--r--   0        0        0     5315 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/ir/emulator.py
--rw-r--r--   0        0        0     8620 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/ir/space.py
--rw-r--r--   0        0        0    10101 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/ir/state_vector.py
--rw-r--r--   0        0        0     6847 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/emulate/sparse_operator.py
--rw-r--r--   0        0        0     5206 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/factory.py
--rw-r--r--   0        0        0     2099 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/__init__.py
--rw-r--r--   0        0        0     2386 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analog_circuit.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analysis/__init__.py
--rw-r--r--   0        0        0     3590 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analysis/assignment_scan.py
--rw-r--r--   0        0        0     5337 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analysis/is_constant.py
--rw-r--r--   0        0        0      990 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analysis/is_hyperfine.py
--rw-r--r--   0        0        0     9157 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/analysis/scan_variables.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/control/__init__.py
--rw-r--r--   0        0        0     7307 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/control/field.py
--rw-r--r--   0        0        0     4918 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/control/pulse.py
--rw-r--r--   0        0        0     4469 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/control/sequence.py
--rw-r--r--   0        0        0    25153 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/control/waveform.py
--rw-r--r--   0        0        0      492 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/__init__.py
--rw-r--r--   0        0        0     5896 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/base.py
--rw-r--r--   0        0        0    14385 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/bravais.py
--rw-r--r--   0        0        0     2808 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/list.py
--rw-r--r--   0        0        0     3332 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/quera_task_result.py
--rw-r--r--   0        0        0    13351 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/location/transform.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/__init__.py
--rw-r--r--   0        0        0     2144 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/base.py
--rw-r--r--   0        0        0     5961 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/bloqade.py
--rw-r--r--   0        0        0     8805 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/braket.py
--rw-r--r--   0        0        0     1349 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/params.py
--rw-r--r--   0        0        0     4462 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/routine/quera.py
--rw-r--r--   0        0        0    17649 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/scalar.py
--rw-r--r--   0        0        0     6500 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/tree_print.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/visitor/__init__.py
--rw-r--r--   0        0        0     6575 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/visitor/analog_circuit.py
--rw-r--r--   0        0        0     3215 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/visitor/location.py
--rw-r--r--   0        0        0     3097 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/visitor/scalar.py
--rw-r--r--   0        0        0     3686 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/ir/visitor/waveform.py
--rw-r--r--   0        0        0      174 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/juliapkg-release.json
--rw-r--r--   0        0        0      231 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/juliapkg.json
--rw-r--r--   0        0        0     5763 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/serialize.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/__init__.py
--rw-r--r--   0        0        0     1212 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/base.py
--rw-r--r--   0        0        0     2100 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/braket.py
--rw-r--r--   0        0        0      394 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/capabilities.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/__init__.py
--rw-r--r--   0        0        0     4194 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/braket.py
--rw-r--r--   0        0        0     1781 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/capabilities.py
--rw-r--r--   0        0        0     3880 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/parallel.py
--rw-r--r--   0        0        0     2938 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/task_results.py
--rw-r--r--   0        0        0     8282 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/ir/task_specification.py
--rw-r--r--   0        0        0     2332 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/mock.py
--rw-r--r--   0        0        0     2737 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/__init__.py
--rw-r--r--   0        0        0    21088 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/api.py
--rw-r--r--   0        0        0      540 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/aws_login.py
--rw-r--r--   0        0        0      215 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/config/aquila_api_config.json
--rw-r--r--   0        0        0     1738 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/config/capabilities.json
--rw-r--r--   0        0        0      220 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/config/mock_api_config.json
--rw-r--r--   0        0        0      638 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/submission/quera_api_client/load_config.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/task/__init__.py
--rw-r--r--   0        0        0     6736 2023-10-19 21:10:20.895417 bloqade-0.8.0/src/bloqade/task/base.py
--rw-r--r--   0        0        0    19199 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/batch.py
--rw-r--r--   0        0        0     3007 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/bloqade.py
--rw-r--r--   0        0        0     5148 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/braket.py
--rw-r--r--   0        0        0     2037 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/braket_simulator.py
--rw-r--r--   0        0        0     6077 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/json.py
--rw-r--r--   0        0        0     5348 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/task/quera.py
--rw-r--r--   0        0        0     1794 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/__init__.py
--rw-r--r--   0        0        0     2772 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/atom_arragement_visualize.py
--rw-r--r--   0        0        0     4919 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/display.py
--rw-r--r--   0        0        0    10548 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/ir_visualize.py
--rw-r--r--   0        0        0    21227 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/report_visualize.py
--rw-r--r--   0        0        0     5175 2023-10-19 21:10:20.899417 bloqade-0.8.0/src/bloqade/visualization/task_visualize.py
--rw-r--r--   0        0        0        0 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      457 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/_test_issue.py
--rw-r--r--   0        0        0     1670 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/_test_schema.py
--rw-r--r--   0        0        0    14151 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/cassettes/test_quera_internal_api/test_quera_retrieve.yaml
--rw-r--r--   0        0        0     8558 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/cassettes/test_quera_internal_api/test_quera_submit.yaml
--rw-r--r--   0        0        0      220 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/config/submit_quera_api.json
--rw-r--r--   0        0        0     3448 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/list_of_locations_pprint_output.txt
--rw-r--r--   0        0        0     3916 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_defect_count_output.txt
--rw-r--r--   0        0        0     3920 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_defect_density_output.txt
--rw-r--r--   0        0        0     4108 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_output.txt
--rw-r--r--   0        0        0     4242 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_defect_count_output.txt
--rw-r--r--   0        0        0     4196 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_defect_density_output.txt
--rw-r--r--   0        0        0     4496 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_output.txt
--rw-r--r--   0        0        0     4492 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_var_output.txt
--rw-r--r--   0        0        0     1668 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_args.py
--rw-r--r--   0        0        0     3307 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_assign.py
--rw-r--r--   0        0        0     1285 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_batch2.py
--rw-r--r--   0        0        0     2905 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_braket_emulator.py
--rw-r--r--   0        0        0      191 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_braket_ir.py
--rw-r--r--   0        0        0     4994 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_braket_submission_backend.py
--rw-r--r--   0        0        0     4685 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_bravais.py
--rw-r--r--   0        0        0    17088 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_builder.py
--rw-r--r--   0        0        0      306 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_builder_job.py
--rw-r--r--   0        0        0      637 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_builder_old.py
--rw-r--r--   0        0        0      655 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_builder_visual.py
--rw-r--r--   0        0        0     5332 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_codegen_quera.py
--rw-r--r--   0        0        0      112 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_constants.py
--rw-r--r--   0        0        0    11377 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_emulator_codegen.py
--rw-r--r--   0        0        0     4478 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_factory.py
--rw-r--r--   0        0        0     3667 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_field.py
--rw-r--r--   0        0        0    36713 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_hamiltonian_codegen.py
--rw-r--r--   0        0        0    21939 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_hardware_codegen.py
--rw-r--r--   0        0        0     2443 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_ir_visual.py
--rw-r--r--   0        0        0     3201 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_is_constant.py
--rw-r--r--   0        0        0     2201 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_lattice.py
--rw-r--r--   0        0        0     4358 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_lattice_pprint.py
--rw-r--r--   0        0        0      109 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_misc.py
--rw-r--r--   0        0        0      978 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_mock_submit.py
--rw-r--r--   0        0        0     1436 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_parallelize.py
--rw-r--r--   0        0        0     3160 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_printer.py
--rw-r--r--   0        0        0     1982 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_program_visitor.py
--rw-r--r--   0        0        0     6755 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_pulse.py
--rw-r--r--   0        0        0     7225 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_python_emulator.py
--rw-r--r--   0        0        0    19231 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_quera_internal_api.py
--rw-r--r--   0        0        0     6381 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_quera_submission_backend.py
--rw-r--r--   0        0        0     1106 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_report.py
--rw-r--r--   0        0        0      440 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_report_visual.py
--rw-r--r--   0        0        0     9970 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_scalar.py
--rw-r--r--   0        0        0     3080 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_schema_codegen.py
--rw-r--r--   0        0        0     5812 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_sequence.py
--rw-r--r--   0        0        0     2065 2023-10-19 21:10:20.899417 bloqade-0.8.0/tests/test_serialize_decorator.py
--rw-r--r--   0        0        0    23203 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_space.py
--rw-r--r--   0        0        0     3863 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_sparse_operator.py
--rw-r--r--   0        0        0      346 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_submission_base.py
--rw-r--r--   0        0        0     1254 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_task.py
--rw-r--r--   0        0        0     2054 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_task2.py
--rw-r--r--   0        0        0      292 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_types.py
--rw-r--r--   0        0        0     1928 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_variable_scan.py
--rw-r--r--   0        0        0       99 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_version.py
--rw-r--r--   0        0        0    13794 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_waveform.py
--rw-r--r--   0        0        0     2300 2023-10-19 21:10:20.903417 bloqade-0.8.0/tests/test_waveform_visitor.py
--rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 bloqade-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10623 2023-10-20 18:40:49.522775 bloqade-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9762 2023-10-20 18:40:49.522775 bloqade-0.9.0/README.md
+-rw-r--r--   0        0        0     2933 2023-10-20 18:41:11.854870 bloqade-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1158 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/__init__.py
+-rw-r--r--   0        0        0      340 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/atom_arrangement.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/__init__.py
+-rw-r--r--   0        0        0      562 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/args.py
+-rw-r--r--   0        0        0     4960 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/assign.py
+-rw-r--r--   0        0        0     1210 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/backend/__init__.py
+-rw-r--r--   0        0        0      852 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/backend/bloqade.py
+-rw-r--r--   0        0        0     3107 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/backend/braket.py
+-rw-r--r--   0        0        0     3043 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/backend/quera.py
+-rw-r--r--   0        0        0      367 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/base.py
+-rw-r--r--   0        0        0     3163 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/coupling.py
+-rw-r--r--   0        0        0     1149 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/drive.py
+-rw-r--r--   0        0        0    11476 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/field.py
+-rw-r--r--   0        0        0      487 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/parallelize.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/parse/__init__.py
+-rw-r--r--   0        0        0     8561 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/parse/builder.py
+-rw-r--r--   0        0        0     2399 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/parse/stream.py
+-rw-r--r--   0        0        0     1858 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/parse/trait.py
+-rw-r--r--   0        0        0     5754 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/pragmas.py
+-rw-r--r--   0        0        0      515 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/route.py
+-rw-r--r--   0        0        0      311 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/sequence_builder.py
+-rw-r--r--   0        0        0     2403 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/spatial.py
+-rw-r--r--   0        0        0     2148 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/start.py
+-rw-r--r--   0        0        0      264 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/typing.py
+-rw-r--r--   0        0        0    50565 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/builder/waveform.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/codegen/common/__init__.py
+-rw-r--r--   0        0        0    11885 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/codegen/common/assign_variables.py
+-rw-r--r--   0        0        0    16763 2023-10-20 18:40:49.562775 bloqade-0.9.0/src/bloqade/codegen/common/json.py
+-rw-r--r--   0        0        0    13722 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/emulator_ir.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/hardware/__init__.py
+-rw-r--r--   0        0        0     7747 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/hardware/piecewise_constant.py
+-rw-r--r--   0        0        0     8011 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/hardware/piecewise_linear.py
+-rw-r--r--   0        0        0    25215 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/hardware/quera.py
+-rw-r--r--   0        0        0     2576 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/codegen/julia/types.py
+-rw-r--r--   0        0        0      144 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/constants.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/codegen/__init__.py
+-rw-r--r--   0        0        0     8014 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/codegen/hamiltonian.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/ir/__init__.py
+-rw-r--r--   0        0        0     4883 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/ir/atom_type.py
+-rw-r--r--   0        0        0     5315 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/ir/emulator.py
+-rw-r--r--   0        0        0     8620 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/ir/space.py
+-rw-r--r--   0        0        0    10101 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/ir/state_vector.py
+-rw-r--r--   0        0        0     6793 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/emulate/sparse_operator.py
+-rw-r--r--   0        0        0     5206 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/factory.py
+-rw-r--r--   0        0        0     2099 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/__init__.py
+-rw-r--r--   0        0        0     2386 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analog_circuit.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analysis/__init__.py
+-rw-r--r--   0        0        0     3590 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analysis/assignment_scan.py
+-rw-r--r--   0        0        0     5337 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analysis/is_constant.py
+-rw-r--r--   0        0        0      990 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analysis/is_hyperfine.py
+-rw-r--r--   0        0        0     9157 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/analysis/scan_variables.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/control/__init__.py
+-rw-r--r--   0        0        0     7307 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/control/field.py
+-rw-r--r--   0        0        0     4918 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/control/pulse.py
+-rw-r--r--   0        0        0     4469 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/control/sequence.py
+-rw-r--r--   0        0        0    25153 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/control/waveform.py
+-rw-r--r--   0        0        0      492 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/__init__.py
+-rw-r--r--   0        0        0     6910 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/base.py
+-rw-r--r--   0        0        0    14385 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/bravais.py
+-rw-r--r--   0        0        0     2808 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/list.py
+-rw-r--r--   0        0        0     3332 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/quera_task_result.py
+-rw-r--r--   0        0        0    13351 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/location/transform.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/__init__.py
+-rw-r--r--   0        0        0     2144 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/base.py
+-rw-r--r--   0        0        0     5961 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/bloqade.py
+-rw-r--r--   0        0        0     8805 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/braket.py
+-rw-r--r--   0        0        0     1349 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/params.py
+-rw-r--r--   0        0        0     4462 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/routine/quera.py
+-rw-r--r--   0        0        0    17649 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/scalar.py
+-rw-r--r--   0        0        0     6500 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/tree_print.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/visitor/__init__.py
+-rw-r--r--   0        0        0     6575 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/visitor/analog_circuit.py
+-rw-r--r--   0        0        0     3215 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/visitor/location.py
+-rw-r--r--   0        0        0     3097 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/visitor/scalar.py
+-rw-r--r--   0        0        0     3686 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/ir/visitor/waveform.py
+-rw-r--r--   0        0        0      174 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/juliapkg-release.json
+-rw-r--r--   0        0        0      231 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/juliapkg.json
+-rw-r--r--   0        0        0     5763 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/serialize.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/__init__.py
+-rw-r--r--   0        0        0     1212 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/base.py
+-rw-r--r--   0        0        0     2100 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/braket.py
+-rw-r--r--   0        0        0      394 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/capabilities.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/ir/__init__.py
+-rw-r--r--   0        0        0     4194 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/ir/braket.py
+-rw-r--r--   0        0        0     1781 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/ir/capabilities.py
+-rw-r--r--   0        0        0     3880 2023-10-20 18:40:49.566775 bloqade-0.9.0/src/bloqade/submission/ir/parallel.py
+-rw-r--r--   0        0        0     2938 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/ir/task_results.py
+-rw-r--r--   0        0        0     8282 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/ir/task_specification.py
+-rw-r--r--   0        0        0     2332 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/mock.py
+-rw-r--r--   0        0        0     2737 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/__init__.py
+-rw-r--r--   0        0        0    21088 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/api.py
+-rw-r--r--   0        0        0      540 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/aws_login.py
+-rw-r--r--   0        0        0      215 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/config/aquila_api_config.json
+-rw-r--r--   0        0        0     1738 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/config/capabilities.json
+-rw-r--r--   0        0        0      220 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/config/mock_api_config.json
+-rw-r--r--   0        0        0      638 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/submission/quera_api_client/load_config.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/__init__.py
+-rw-r--r--   0        0        0     6736 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/base.py
+-rw-r--r--   0        0        0    19199 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/batch.py
+-rw-r--r--   0        0        0     3007 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/bloqade.py
+-rw-r--r--   0        0        0     5148 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/braket.py
+-rw-r--r--   0        0        0     2037 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/braket_simulator.py
+-rw-r--r--   0        0        0     6077 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/json.py
+-rw-r--r--   0        0        0     5348 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/task/quera.py
+-rw-r--r--   0        0        0     1794 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/__init__.py
+-rw-r--r--   0        0        0     2772 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/atom_arragement_visualize.py
+-rw-r--r--   0        0        0     4919 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/display.py
+-rw-r--r--   0        0        0    10548 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/ir_visualize.py
+-rw-r--r--   0        0        0    21227 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/report_visualize.py
+-rw-r--r--   0        0        0     5175 2023-10-20 18:40:49.570775 bloqade-0.9.0/src/bloqade/visualization/task_visualize.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      457 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/_test_issue.py
+-rw-r--r--   0        0        0     1670 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/_test_schema.py
+-rw-r--r--   0        0        0    14151 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/cassettes/test_quera_internal_api/test_quera_retrieve.yaml
+-rw-r--r--   0        0        0     8558 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/cassettes/test_quera_internal_api/test_quera_submit.yaml
+-rw-r--r--   0        0        0      220 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/config/submit_quera_api.json
+-rw-r--r--   0        0        0     3448 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/list_of_locations_pprint_output.txt
+-rw-r--r--   0        0        0     3916 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_defect_count_output.txt
+-rw-r--r--   0        0        0     3920 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_defect_density_output.txt
+-rw-r--r--   0        0        0     4108 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_output.txt
+-rw-r--r--   0        0        0     4242 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_defect_count_output.txt
+-rw-r--r--   0        0        0     4196 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_defect_density_output.txt
+-rw-r--r--   0        0        0     4496 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_output.txt
+-rw-r--r--   0        0        0     4492 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_var_output.txt
+-rw-r--r--   0        0        0     1668 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_args.py
+-rw-r--r--   0        0        0     3307 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_assign.py
+-rw-r--r--   0        0        0     1285 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_batch2.py
+-rw-r--r--   0        0        0     2905 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_braket_emulator.py
+-rw-r--r--   0        0        0      191 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_braket_ir.py
+-rw-r--r--   0        0        0     4994 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_braket_submission_backend.py
+-rw-r--r--   0        0        0     4685 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_bravais.py
+-rw-r--r--   0        0        0    17088 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_builder.py
+-rw-r--r--   0        0        0      306 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_builder_job.py
+-rw-r--r--   0        0        0      637 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_builder_old.py
+-rw-r--r--   0        0        0      655 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_builder_visual.py
+-rw-r--r--   0        0        0     5332 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_codegen_quera.py
+-rw-r--r--   0        0        0      112 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_constants.py
+-rw-r--r--   0        0        0    11377 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_emulator_codegen.py
+-rw-r--r--   0        0        0     4478 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_factory.py
+-rw-r--r--   0        0        0     3667 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_field.py
+-rw-r--r--   0        0        0    36713 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_hamiltonian_codegen.py
+-rw-r--r--   0        0        0    21939 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_hardware_codegen.py
+-rw-r--r--   0        0        0     2443 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_ir_visual.py
+-rw-r--r--   0        0        0     3201 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_is_constant.py
+-rw-r--r--   0        0        0     2898 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_lattice.py
+-rw-r--r--   0        0        0     4358 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_lattice_pprint.py
+-rw-r--r--   0        0        0      109 2023-10-20 18:40:49.570775 bloqade-0.9.0/tests/test_misc.py
+-rw-r--r--   0        0        0      978 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_mock_submit.py
+-rw-r--r--   0        0        0     1436 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_parallelize.py
+-rw-r--r--   0        0        0     3160 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_printer.py
+-rw-r--r--   0        0        0     1982 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_program_visitor.py
+-rw-r--r--   0        0        0     6755 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_pulse.py
+-rw-r--r--   0        0        0     7225 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_python_emulator.py
+-rw-r--r--   0        0        0    19231 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_quera_internal_api.py
+-rw-r--r--   0        0        0     6381 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_quera_submission_backend.py
+-rw-r--r--   0        0        0     1106 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_report.py
+-rw-r--r--   0        0        0      440 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_report_visual.py
+-rw-r--r--   0        0        0     9970 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_scalar.py
+-rw-r--r--   0        0        0     3080 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_schema_codegen.py
+-rw-r--r--   0        0        0     5812 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_sequence.py
+-rw-r--r--   0        0        0     2065 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_serialize_decorator.py
+-rw-r--r--   0        0        0    23203 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_space.py
+-rw-r--r--   0        0        0     3863 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_sparse_operator.py
+-rw-r--r--   0        0        0      346 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_submission_base.py
+-rw-r--r--   0        0        0     1254 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_task.py
+-rw-r--r--   0        0        0     2054 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_task2.py
+-rw-r--r--   0        0        0      292 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_types.py
+-rw-r--r--   0        0        0     1928 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_variable_scan.py
+-rw-r--r--   0        0        0       99 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_version.py
+-rw-r--r--   0        0        0    13794 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_waveform.py
+-rw-r--r--   0        0        0     2300 2023-10-20 18:40:49.574775 bloqade-0.9.0/tests/test_waveform_visitor.py
+-rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 bloqade-0.9.0/PKG-INFO
```

### Comparing `bloqade-0.8.0/LICENSE` & `bloqade-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/README.md` & `bloqade-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/pyproject.toml` & `bloqade-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bloqade"
-version = "0.8.0"
+version = "0.9.0"
 description = "Neutral atom software development kit"
 authors = [
     { name = "QuEra Computing Inc.", email = "info@quera.com" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
@@ -95,14 +95,15 @@
     "ruff>=0.0.264",
     "pre-commit>=3.3.1",
     "coverage>=7.2.5",
     "jupytext>=1.14.5",
     "pytest-recording>=0.12.2",
     "vcrpy==4.4.0",
     "pyinstrument>=4.5.3",
+    "scikit-optimize>=0.9.0",
 ]
 
 [tool.pdm.scripts]
 upload = "python -m twine upload -r bloqade dist/*"
 
 [tool.pdm.scripts._]
 env_file = "./.env"
```

### Comparing `bloqade-0.8.0/src/bloqade/__init__.py` & `bloqade-0.9.0/src/bloqade/__init__.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/args.py` & `bloqade-0.9.0/src/bloqade/builder/args.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/assign.py` & `bloqade-0.9.0/src/bloqade/builder/assign.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/backend/__init__.py` & `bloqade-0.9.0/src/bloqade/builder/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/backend/bloqade.py` & `bloqade-0.9.0/src/bloqade/builder/backend/bloqade.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/backend/braket.py` & `bloqade-0.9.0/src/bloqade/builder/backend/braket.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/backend/quera.py` & `bloqade-0.9.0/src/bloqade/builder/backend/quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/coupling.py` & `bloqade-0.9.0/src/bloqade/builder/coupling.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/drive.py` & `bloqade-0.9.0/src/bloqade/builder/drive.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/field.py` & `bloqade-0.9.0/src/bloqade/builder/field.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/parse/builder.py` & `bloqade-0.9.0/src/bloqade/builder/parse/builder.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/parse/stream.py` & `bloqade-0.9.0/src/bloqade/builder/parse/stream.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/parse/trait.py` & `bloqade-0.9.0/src/bloqade/builder/parse/trait.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/pragmas.py` & `bloqade-0.9.0/src/bloqade/builder/pragmas.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/route.py` & `bloqade-0.9.0/src/bloqade/builder/route.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/spatial.py` & `bloqade-0.9.0/src/bloqade/builder/spatial.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/start.py` & `bloqade-0.9.0/src/bloqade/builder/start.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/builder/waveform.py` & `bloqade-0.9.0/src/bloqade/builder/waveform.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/common/assign_variables.py` & `bloqade-0.9.0/src/bloqade/codegen/common/assign_variables.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/common/json.py` & `bloqade-0.9.0/src/bloqade/codegen/common/json.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/emulator_ir.py` & `bloqade-0.9.0/src/bloqade/codegen/emulator_ir.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/hardware/piecewise_constant.py` & `bloqade-0.9.0/src/bloqade/codegen/hardware/piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/hardware/piecewise_linear.py` & `bloqade-0.9.0/src/bloqade/codegen/hardware/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/hardware/quera.py` & `bloqade-0.9.0/src/bloqade/codegen/hardware/quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/codegen/julia/types.py` & `bloqade-0.9.0/src/bloqade/codegen/julia/types.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/codegen/hamiltonian.py` & `bloqade-0.9.0/src/bloqade/emulate/codegen/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/ir/atom_type.py` & `bloqade-0.9.0/src/bloqade/emulate/ir/atom_type.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/ir/emulator.py` & `bloqade-0.9.0/src/bloqade/emulate/ir/emulator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/ir/space.py` & `bloqade-0.9.0/src/bloqade/emulate/ir/space.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/ir/state_vector.py` & `bloqade-0.9.0/src/bloqade/emulate/ir/state_vector.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/emulate/sparse_operator.py` & `bloqade-0.9.0/src/bloqade/emulate/sparse_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 
             def _matvec_imp(col_indices, row_indices, scale, input, output):
                 return _index_mapping_row_col_sliced(
                     scale, input[col_indices], output[row_indices]
                 )
 
         elif isinstance(self.col_indices, slice):
-            print(self.col_indices, self.row_indices)
 
             def _matvec_imp(col_indices, row_indices, scale, input, output):
                 return _index_mapping_col_sliced(
                     row_indices, scale, input[col_indices], output
                 )
 
         elif isinstance(self.row_indices, slice):
```

### Comparing `bloqade-0.8.0/src/bloqade/factory.py` & `bloqade-0.9.0/src/bloqade/factory.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/__init__.py` & `bloqade-0.9.0/src/bloqade/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/analog_circuit.py` & `bloqade-0.9.0/src/bloqade/ir/analog_circuit.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/analysis/assignment_scan.py` & `bloqade-0.9.0/src/bloqade/ir/analysis/assignment_scan.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/analysis/is_constant.py` & `bloqade-0.9.0/src/bloqade/ir/analysis/is_constant.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/analysis/is_hyperfine.py` & `bloqade-0.9.0/src/bloqade/ir/analysis/is_hyperfine.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/analysis/scan_variables.py` & `bloqade-0.9.0/src/bloqade/ir/analysis/scan_variables.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/control/field.py` & `bloqade-0.9.0/src/bloqade/ir/control/field.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/control/pulse.py` & `bloqade-0.9.0/src/bloqade/ir/control/pulse.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/control/sequence.py` & `bloqade-0.9.0/src/bloqade/ir/control/sequence.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/control/waveform.py` & `bloqade-0.9.0/src/bloqade/ir/control/waveform.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/location/base.py` & `bloqade-0.9.0/src/bloqade/ir/location/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from pydantic.dataclasses import dataclass
 from beartype.typing import List, Tuple, Generator
 from beartype import beartype
 from enum import Enum
 import plotext as pltxt
 import sys
+import numpy as np
+from numpy.typing import NDArray
 from bloqade.visualization import get_atom_arrangement_figure
 from bloqade.visualization import display_ir
 
 
 class SiteFilling(int, Enum):
     filled = 1
     vacant = 0
@@ -108,14 +110,43 @@
     def figure(self, fig_kwargs=None, **assignments):
         """obtain a figure object from the atom arrangement."""
         return get_atom_arrangement_figure(self, fig_kwargs, **assignments)
 
     def show(self, **assignments) -> None:
         display_ir(self, assignments)
 
+    def rydberg_interaction(self, **assignments) -> NDArray:
+        """calculate the Rydberg interaction matrix.
+
+        Args:
+            **assignments: the values to assign to the variables in the register.
+
+        Returns:
+            NDArray: the Rydberg interaction matrix in the lower triangular form.
+
+        """
+
+        from bloqade.constants import RB_C6
+
+        # calculate the Interaction matrix
+        V_ij = np.zeros((self.n_sites, self.n_sites))
+        for i, site_i in enumerate(self.enumerate()):
+            pos_i = np.array([float(ele(**assignments)) for ele in site_i.position])
+
+            for j, site_j in enumerate(self.enumerate()):
+                if j >= i:
+                    break  # enforce lower triangular form
+
+                pos_j = np.array([float(ele(**assignments)) for ele in site_j.position])
+                r_ij = np.linalg.norm(pos_i - pos_j)
+
+                V_ij[i, j] = RB_C6 / r_ij**6
+
+        return V_ij
+
     @property
     def n_atoms(self) -> int:
         """number of atoms (filled sites) in the register."""
         raise NotImplementedError
 
     @property
     def n_sites(self) -> int:
```

### Comparing `bloqade-0.8.0/src/bloqade/ir/location/bravais.py` & `bloqade-0.9.0/src/bloqade/ir/location/bravais.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/location/list.py` & `bloqade-0.9.0/src/bloqade/ir/location/list.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/location/quera_task_result.py` & `bloqade-0.9.0/src/bloqade/ir/location/quera_task_result.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/location/transform.py` & `bloqade-0.9.0/src/bloqade/ir/location/transform.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/routine/base.py` & `bloqade-0.9.0/src/bloqade/ir/routine/base.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/routine/bloqade.py` & `bloqade-0.9.0/src/bloqade/ir/routine/bloqade.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/routine/braket.py` & `bloqade-0.9.0/src/bloqade/ir/routine/braket.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/routine/params.py` & `bloqade-0.9.0/src/bloqade/ir/routine/params.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/routine/quera.py` & `bloqade-0.9.0/src/bloqade/ir/routine/quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/scalar.py` & `bloqade-0.9.0/src/bloqade/ir/scalar.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/tree_print.py` & `bloqade-0.9.0/src/bloqade/ir/tree_print.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/visitor/analog_circuit.py` & `bloqade-0.9.0/src/bloqade/ir/visitor/analog_circuit.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/visitor/location.py` & `bloqade-0.9.0/src/bloqade/ir/visitor/location.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/visitor/scalar.py` & `bloqade-0.9.0/src/bloqade/ir/visitor/scalar.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/ir/visitor/waveform.py` & `bloqade-0.9.0/src/bloqade/ir/visitor/waveform.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/serialize.py` & `bloqade-0.9.0/src/bloqade/serialize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/base.py` & `bloqade-0.9.0/src/bloqade/submission/base.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/braket.py` & `bloqade-0.9.0/src/bloqade/submission/braket.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/ir/braket.py` & `bloqade-0.9.0/src/bloqade/submission/ir/braket.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/ir/capabilities.py` & `bloqade-0.9.0/src/bloqade/submission/ir/capabilities.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/ir/parallel.py` & `bloqade-0.9.0/src/bloqade/submission/ir/parallel.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/ir/task_results.py` & `bloqade-0.9.0/src/bloqade/submission/ir/task_results.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/ir/task_specification.py` & `bloqade-0.9.0/src/bloqade/submission/ir/task_specification.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/mock.py` & `bloqade-0.9.0/src/bloqade/submission/mock.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/quera.py` & `bloqade-0.9.0/src/bloqade/submission/quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/quera_api_client/api.py` & `bloqade-0.9.0/src/bloqade/submission/quera_api_client/api.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/quera_api_client/aws_login.py` & `bloqade-0.9.0/src/bloqade/submission/quera_api_client/aws_login.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/quera_api_client/config/capabilities.json` & `bloqade-0.9.0/src/bloqade/submission/quera_api_client/config/capabilities.json`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/submission/quera_api_client/load_config.py` & `bloqade-0.9.0/src/bloqade/submission/quera_api_client/load_config.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/base.py` & `bloqade-0.9.0/src/bloqade/task/base.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/batch.py` & `bloqade-0.9.0/src/bloqade/task/batch.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/bloqade.py` & `bloqade-0.9.0/src/bloqade/task/bloqade.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/braket.py` & `bloqade-0.9.0/src/bloqade/task/braket.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/braket_simulator.py` & `bloqade-0.9.0/src/bloqade/task/braket_simulator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/json.py` & `bloqade-0.9.0/src/bloqade/task/json.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/task/quera.py` & `bloqade-0.9.0/src/bloqade/task/quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/__init__.py` & `bloqade-0.9.0/src/bloqade/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/atom_arragement_visualize.py` & `bloqade-0.9.0/src/bloqade/visualization/atom_arragement_visualize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/display.py` & `bloqade-0.9.0/src/bloqade/visualization/display.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/ir_visualize.py` & `bloqade-0.9.0/src/bloqade/visualization/ir_visualize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/report_visualize.py` & `bloqade-0.9.0/src/bloqade/visualization/report_visualize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/src/bloqade/visualization/task_visualize.py` & `bloqade-0.9.0/src/bloqade/visualization/task_visualize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/_test_schema.py` & `bloqade-0.9.0/tests/_test_schema.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/cassettes/test_quera_internal_api/test_quera_retrieve.yaml` & `bloqade-0.9.0/tests/cassettes/test_quera_internal_api/test_quera_retrieve.yaml`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/cassettes/test_quera_internal_api/test_quera_submit.yaml` & `bloqade-0.9.0/tests/cassettes/test_quera_internal_api/test_quera_submit.yaml`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/list_of_locations_pprint_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/list_of_locations_pprint_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_defect_count_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_defect_count_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_defect_density_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_defect_density_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/rectangular_pprint_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/rectangular_pprint_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_defect_count_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_defect_count_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_defect_density_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_defect_density_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/data/expected_pprint_output/square_pprint_var_output.txt` & `bloqade-0.9.0/tests/data/expected_pprint_output/square_pprint_var_output.txt`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_args.py` & `bloqade-0.9.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_assign.py` & `bloqade-0.9.0/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_batch2.py` & `bloqade-0.9.0/tests/test_batch2.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_braket_emulator.py` & `bloqade-0.9.0/tests/test_braket_emulator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_braket_submission_backend.py` & `bloqade-0.9.0/tests/test_braket_submission_backend.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_bravais.py` & `bloqade-0.9.0/tests/test_bravais.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_builder.py` & `bloqade-0.9.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_builder_old.py` & `bloqade-0.9.0/tests/test_builder_old.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_builder_visual.py` & `bloqade-0.9.0/tests/test_builder_visual.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_codegen_quera.py` & `bloqade-0.9.0/tests/test_codegen_quera.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_emulator_codegen.py` & `bloqade-0.9.0/tests/test_emulator_codegen.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_factory.py` & `bloqade-0.9.0/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_field.py` & `bloqade-0.9.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_hamiltonian_codegen.py` & `bloqade-0.9.0/tests/test_hamiltonian_codegen.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_hardware_codegen.py` & `bloqade-0.9.0/tests/test_hardware_codegen.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_ir_visual.py` & `bloqade-0.9.0/tests/test_ir_visual.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_is_constant.py` & `bloqade-0.9.0/tests/test_is_constant.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_lattice_pprint.py` & `bloqade-0.9.0/tests/test_lattice_pprint.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_mock_submit.py` & `bloqade-0.9.0/tests/test_mock_submit.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_parallelize.py` & `bloqade-0.9.0/tests/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_printer.py` & `bloqade-0.9.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_program_visitor.py` & `bloqade-0.9.0/tests/test_program_visitor.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_pulse.py` & `bloqade-0.9.0/tests/test_pulse.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_python_emulator.py` & `bloqade-0.9.0/tests/test_python_emulator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_quera_internal_api.py` & `bloqade-0.9.0/tests/test_quera_internal_api.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_quera_submission_backend.py` & `bloqade-0.9.0/tests/test_quera_submission_backend.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_report.py` & `bloqade-0.9.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_scalar.py` & `bloqade-0.9.0/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_schema_codegen.py` & `bloqade-0.9.0/tests/test_schema_codegen.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_sequence.py` & `bloqade-0.9.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_serialize_decorator.py` & `bloqade-0.9.0/tests/test_serialize_decorator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_space.py` & `bloqade-0.9.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_sparse_operator.py` & `bloqade-0.9.0/tests/test_sparse_operator.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_task.py` & `bloqade-0.9.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_task2.py` & `bloqade-0.9.0/tests/test_task2.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_variable_scan.py` & `bloqade-0.9.0/tests/test_variable_scan.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_waveform.py` & `bloqade-0.9.0/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/tests/test_waveform_visitor.py` & `bloqade-0.9.0/tests/test_waveform_visitor.py`

 * *Files identical despite different names*

### Comparing `bloqade-0.8.0/PKG-INFO` & `bloqade-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloqade
-Version: 0.8.0
+Version: 0.9.0
 Summary: Neutral atom software development kit
 Author-Email: QuEra Computing Inc. <info@quera.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

