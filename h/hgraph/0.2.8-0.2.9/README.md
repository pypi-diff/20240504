# Comparing `tmp/hgraph-0.2.8.tar.gz` & `tmp/hgraph-0.2.9.tar.gz`

## Comparing `hgraph-0.2.8.tar` & `hgraph-0.2.9.tar`

### file list

```diff
@@ -1,291 +1,298 @@
--rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 hgraph-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.8/ROADMAP.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/dependabot.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/index.md
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/evaluation_clock_uml.png
--rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/evaluation_engine_api.png
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/forward_propagation_graph.md
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_executor_uml.png
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_runtime.md
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/graph_uml.png
--rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/node_uml.png
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/run_mode_uml.png
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/services.md
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/concepts/src_cmpt_snk_diagram.png
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/component_signature.md
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/hg_types.md
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/node_signature.md
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/program_anatomy.md
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/schema_based_types.md
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/python/what_is_1_1.png
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/exception_handling.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/exception_handling.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/feedback.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/feedback.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/generics.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/generics.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/graphs_and_nodes.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/graphs_and_nodes.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/hello_world.md
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/hello_world.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/injectable_attributes.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/injectable_attributes.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/life_cycle.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/life_cycle.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/map_reduce_switch.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/map_reduce_switch.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/node_testing.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/node_testing.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/push_source_node.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/push_source_node.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.8/docs/quick_start/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/__init__.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/monitoring.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/phase_1/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/monitoring/phase_1/monitoring_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/notebook/__init__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/notebook/example_book.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_api/__init__.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_api/web_api.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/__init__.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 hgraph-0.2.8/examples/web_ui/web_ui.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/__about__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/__init__.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_builder.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_graph_builder.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_input_builder.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_node_builder.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_output_builder.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_scalar_builder.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_builder/_ts_builder.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_impl_configuration.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/graph_construction.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_graph_builder.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_map_builder.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_node_builder.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_node_impl_builder.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_reduce_builder.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_service_impl_builder.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_switch_builder.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_try_except_builder.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_builder/_ts_builder.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_common.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_data_writer.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_map_node.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_node.py
--rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_reduce_node.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_service_node_impl.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_switch_node.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_runtime/_try_except_node.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_feature_extension.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_input.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_output.py
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_ref.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_scalar_value.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_signal.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_ts.py
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsb.py
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsd.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tsl.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_impl/_types/_tss.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_constants.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_data_writer.py
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_feedback.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_global_state.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_graph_runner.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_lifecycle.py
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_node.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_runtime/_operators.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_error_type.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_frame_scalar_type_meta_data.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ref_meta_data.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ref_type.py
--rw-r--r--   0        0        0    35974 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_type_meta_data.py
--rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_types.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_scalar_value.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_schema_type.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_time_series_meta_data.py
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_time_series_types.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_meta_data.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_signal_meta_data.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_type.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_ts_type_var_meta_data.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsb_meta_data.py
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsb_type.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsd_meta_data.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsd_type.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsl_meta_data.py
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tsl_type.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tss_meta_data.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_tss_type.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_type_meta_data.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_types/_typing_utils.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0    20255 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_decorators.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_dispatch.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_exception_handling.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_graph_builder.py
--rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_map.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_reduce.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_source_code_details.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_stub_wiring_node.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_switch.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_context.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_errors.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_instance.py
--rw-r--r--   0        0        0    20628 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_signature.py
--rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_port.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_utils.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/__init__.py
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
--rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
--rw-r--r--   0        0        0    24577 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/__init__.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspective.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspetive_publish.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/index_template.html
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/table_template.html
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/adaptors/perspective/workspace_template.html
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_analytical.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_compound_scalar_operators.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_conditional.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_const.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_data_source_polars.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_datetime_operators.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_drop_dups.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_format.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_frame_operators.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_graph.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_logical.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_math.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_null_sink.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_numpy.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_operators.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_pass_through.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_print.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_record.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_replay.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_service_utils.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_set_operators.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_stream_operators.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsb_operators.py
--rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsd_operators.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tsl_operators.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tss_operators.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_tuple_operators.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/nodes/_window_operators.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/NoteBook.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/notebook/_notebook_graph.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/__init__.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/_node_printer.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/_node_unit_tester.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.8/src/hgraph/test/testing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test_wiring.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_feedback.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_complex_types.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_operator_rank.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_data.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_const.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_decorators.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_dispatch.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_error_handling.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_generic_graphs.py
--rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_map.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_overloads.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ref.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_service.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_switch.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tss.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_analytical.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_conditional.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_const.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_data_source_polars.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_drop_dups.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_format.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_frame.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_logical.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_math.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_numpy.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_operators.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_print.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_push_queue.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_recorder.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_replay.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_stream_operators.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsb_operators.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsd_operators.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsl_operators.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tss_operators.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_window_operators.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_wp_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/test_eval_node.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 hgraph-0.2.8/tests/python/unit/hgraph/test/test_node_printer.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.8/LICENSE
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.8/README.md
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 hgraph-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hgraph-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 hgraph-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.9/ROADMAP.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/index.md
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/evaluation_clock_uml.png
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/evaluation_engine_api.png
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/forward_propagation_graph.md
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/graph_executor_uml.png
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/graph_runtime.md
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/graph_uml.png
+-rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/node_uml.png
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/run_mode_uml.png
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/services.md
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/concepts/src_cmpt_snk_diagram.png
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/component_signature.md
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/hg_types.md
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/node_signature.md
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/program_anatomy.md
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/schema_based_types.md
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/python/what_is_1_1.png
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/exception_handling.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/exception_handling.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/feedback.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/feedback.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/generics.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/generics.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/graphs_and_nodes.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/graphs_and_nodes.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/hello_world.md
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/hello_world.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/injectable_attributes.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/injectable_attributes.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/life_cycle.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/life_cycle.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/map_reduce_switch.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/map_reduce_switch.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/node_testing.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/node_testing.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/push_source_node.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/push_source_node.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.9/docs/quick_start/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/monitoring/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/monitoring/monitoring.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/monitoring/phase_1/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/monitoring/phase_1/monitoring_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/notebook/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/notebook/example_book.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/web_api/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/web_api/web_api.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/web_ui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/web_ui/__init__.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 hgraph-0.2.9/examples/web_ui/web_ui.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/__about__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_builder.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_graph_builder.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_input_builder.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_node_builder.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_output_builder.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_scalar_builder.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_impl_configuration.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/graph_construction.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_graph_builder.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_map_builder.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_node_builder.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_node_impl_builder.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_reduce_builder.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_service_impl_builder.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_switch_builder.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_try_except_builder.py
+-rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_common.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_map_node.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_node.py
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_reduce_node.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_service_node_impl.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_switch_node.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_runtime/_try_except_node.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_feature_extension.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_input.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_output.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_ref.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_scalar_value.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_signal.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_ts.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_tsb.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_tsd.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_tsl.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_impl/_types/_tss.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_constants.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_feedback.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_global_state.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_graph.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_graph_runner.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_lifecycle.py
+-rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_node.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_runtime/_operators.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_error_type.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_frame_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ref_meta_data.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ref_type.py
+-rw-r--r--   0        0        0    35974 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_scalar_types.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_scalar_value.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_schema_type.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_time_series_meta_data.py
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_time_series_types.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ts_meta_data.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ts_signal_meta_data.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ts_type.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_ts_type_var_meta_data.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsb_meta_data.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsb_type.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsd_meta_data.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsd_type.py
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsl_meta_data.py
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tsl_type.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tss_meta_data.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_tss_type.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_type_meta_data.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_types/_typing_utils.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0    21228 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_decorators.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_dispatch.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_exception_handling.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_graph_builder.py
+-rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_map.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_reduce.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_source_code_details.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_stub_wiring_node.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_switch.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_context.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_errors.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_instance.py
+-rw-r--r--   0        0        0    20792 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_signature.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_port.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_utils.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/__init__.py
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
+-rw-r--r--   0        0        0    24805 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/data_frame/__init__.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/data_frame/_data_frame_source.py
+-rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/data_frame/_data_source_generators.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/__init__.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/_perspective.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/_perspetive_publish.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/index_template.html
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/table_template.html
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/adaptors/perspective/workspace_template.html
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_analytical.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_compound_scalar_operators.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_conditional.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_const.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_data_source_polars.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_datetime_operators.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_drop_dups.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_format.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_frame_operators.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_graph.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_logical.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_math.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_null_sink.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_numpy.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_operators.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_pass_through.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_print.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_record.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_replay.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_service_utils.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_set_operators.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_stream_operators.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_tsb_operators.py
+-rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_tsd_operators.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_tsl_operators.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_tss_operators.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_tuple_operators.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/nodes/_window_operators.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/notebook/NoteBook.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/notebook/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/notebook/_notebook_graph.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/test/__init__.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/test/_node_printer.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/test/_node_unit_tester.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.9/src/hgraph/test/testing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/test_wiring.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_runtime/test_feedback.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_runtime/test_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_types/test_complex_types.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_types/test_operator_rank.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_types/test_type_meta_data.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_auto_const.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_decorators.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_dispatch.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_error_handling.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_generic_graphs.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_map.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_overloads.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_ref.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_service.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_switch.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tss.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/adaptors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/adaptors/data_frame/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/adaptors/data_frame/test_data_frame_source.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/adaptors/data_frame/test_data_source_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_analytical.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_conditional.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_const.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_data_source_polars.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_drop_dups.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_format.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_frame.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_logical.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_math.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_numpy.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_operators.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_print.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_push_queue.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_recorder.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_replay.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_stream_operators.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsb_operators.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsd_operators.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsl_operators.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tss_operators.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_window_operators.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_wp_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/test/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/test/test_eval_node.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 hgraph-0.2.9/tests/python/unit/hgraph/test/test_node_printer.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.9/README.md
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 hgraph-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 hgraph-0.2.9/PKG-INFO
```

### Comparing `hgraph-0.2.8/CHANGELOG.md` & `hgraph-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -284,7 +284,11 @@
 Version 0.2.8 (10-04-2024)
 --------------------------
 
 * Add initial notebook support
 * Add perspective adaptor
 * Add support for generic services
 
+Version 0.2.9 (14-04-2024)
+--------------------------
+
+* Add ability to mark nodes as being deprecated.
```

### Comparing `hgraph-0.2.8/ROADMAP.md` & `hgraph-0.2.9/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `hgraph-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `hgraph-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/index.md` & `hgraph-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/evaluation_clock_uml.png` & `hgraph-0.2.9/docs/concepts/evaluation_clock_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/evaluation_engine_api.png` & `hgraph-0.2.9/docs/concepts/evaluation_engine_api.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/forward_propagation_graph.md` & `hgraph-0.2.9/docs/concepts/forward_propagation_graph.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/graph_executor_uml.png` & `hgraph-0.2.9/docs/concepts/graph_executor_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/graph_runtime.md` & `hgraph-0.2.9/docs/concepts/graph_runtime.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/graph_uml.png` & `hgraph-0.2.9/docs/concepts/graph_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/node_uml.png` & `hgraph-0.2.9/docs/concepts/node_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/run_mode_uml.png` & `hgraph-0.2.9/docs/concepts/run_mode_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/services.md` & `hgraph-0.2.9/docs/concepts/services.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/concepts/src_cmpt_snk_diagram.png` & `hgraph-0.2.9/docs/concepts/src_cmpt_snk_diagram.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/component_signature.md` & `hgraph-0.2.9/docs/python/component_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/hg_types.md` & `hgraph-0.2.9/docs/python/hg_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/node_signature.md` & `hgraph-0.2.9/docs/python/node_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/program_anatomy.md` & `hgraph-0.2.9/docs/python/program_anatomy.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/schema_based_types.md` & `hgraph-0.2.9/docs/python/schema_based_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/python/what_is_1_1.png` & `hgraph-0.2.9/docs/python/what_is_1_1.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/exception_handling.md` & `hgraph-0.2.9/docs/quick_start/exception_handling.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/exception_handling.py` & `hgraph-0.2.9/docs/quick_start/exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/feedback.md` & `hgraph-0.2.9/docs/quick_start/feedback.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/generics.md` & `hgraph-0.2.9/docs/quick_start/generics.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/generics.py` & `hgraph-0.2.9/docs/quick_start/generics.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/graphs_and_nodes.md` & `hgraph-0.2.9/docs/quick_start/graphs_and_nodes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/graphs_and_nodes.py` & `hgraph-0.2.9/docs/quick_start/graphs_and_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/hello_world.md` & `hgraph-0.2.9/docs/quick_start/hello_world.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/injectable_attributes.md` & `hgraph-0.2.9/docs/quick_start/injectable_attributes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/injectable_attributes.py` & `hgraph-0.2.9/docs/quick_start/injectable_attributes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/life_cycle.md` & `hgraph-0.2.9/docs/quick_start/life_cycle.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/map_reduce_switch.md` & `hgraph-0.2.9/docs/quick_start/map_reduce_switch.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/map_reduce_switch.py` & `hgraph-0.2.9/docs/quick_start/map_reduce_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/node_testing.md` & `hgraph-0.2.9/docs/quick_start/node_testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/push_source_node.md` & `hgraph-0.2.9/docs/quick_start/push_source_node.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/push_source_node.py` & `hgraph-0.2.9/docs/quick_start/push_source_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/docs/quick_start/quick_start.md` & `hgraph-0.2.9/docs/quick_start/quick_start.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/examples/monitoring/monitoring.md` & `hgraph-0.2.9/examples/monitoring/monitoring.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/examples/monitoring/phase_1/monitoring_api.py` & `hgraph-0.2.9/examples/monitoring/phase_1/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/examples/notebook/example_book.ipynb` & `hgraph-0.2.9/examples/notebook/example_book.ipynb`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/examples/web_api/web_api.py` & `hgraph-0.2.9/examples/web_api/web_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/examples/web_ui/web_ui.py` & `hgraph-0.2.9/examples/web_ui/web_ui.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_graph_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_input_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_input_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_node_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_output_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_output_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_builder/_ts_builder.py` & `hgraph-0.2.9/src/hgraph/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/graph_construction.md` & `hgraph-0.2.9/src/hgraph/_impl/graph_construction.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_graph_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_map_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_map_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_node_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_node_impl_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_node_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_reduce_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_reduce_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_service_impl_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_service_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_switch_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_switch_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_try_except_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_try_except_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_builder/_ts_builder.py` & `hgraph-0.2.9/src/hgraph/_impl/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/__init__.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_common.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_common.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_data_writer.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_clock.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_evaluation_engine.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_executor.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Iterable
 
 from hgraph._impl._runtime._node import SkipEvalDelegate
 from hgraph._runtime._evaluation_clock import EngineEvaluationClock
 from hgraph._runtime._lifecycle import initialise_dispose_context
```

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_graph_recorder.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_map_node.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_map_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_node.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_reduce_node.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_reduce_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_service_node_impl.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_service_node_impl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_switch_node.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_switch_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_runtime/_try_except_node.py` & `hgraph-0.2.9/src/hgraph/_impl/_runtime/_try_except_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_feature_extension.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_feature_extension.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_input.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_input.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_output.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_output.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_ref.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_ref.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_scalar_value.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_signal.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_signal.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_ts.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_ts.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_tsb.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_tsb.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_tsd.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_tsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     @value.setter
     def value(self, v: frozendict | dict | Iterable[tuple[K, SCALAR]] | None):
         if v is None:
             self.invalidate()
             return
         # Expect a mapping of some sort or an iterable of k, v pairs
         for k, v_ in v.items() if isinstance(v, (dict, frozendict)) else v:
-            if v_ in (REMOVE, REMOVE_IF_EXISTS):
+            if v_ is REMOVE or v_ is REMOVE_IF_EXISTS:  # Supporting numpy arrays has its costs (==)
                 if v_ is REMOVE_IF_EXISTS and k not in self._ts_values:  # is check should be faster than contains check
                     continue
                 del self[k]
             else:
                 self.get_or_create(k).value = v_
         if self._removed_items or self._added_keys:
             self.owning_graph.evaluation_engine_api.add_after_evaluation_notification(self._clear_key_changes)
```

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_tsl.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_tsl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_impl/_types/_tss.py` & `hgraph-0.2.9/src/hgraph/_impl/_types/_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/__init__.py` & `hgraph-0.2.9/src/hgraph/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_data_writer.py` & `hgraph-0.2.9/src/hgraph/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_evaluation_clock.py` & `hgraph-0.2.9/src/hgraph/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_evaluation_engine.py` & `hgraph-0.2.9/src/hgraph/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_feedback.py` & `hgraph-0.2.9/src/hgraph/_runtime/_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_global_state.py` & `hgraph-0.2.9/src/hgraph/_runtime/_global_state.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_graph.py` & `hgraph-0.2.9/src/hgraph/_runtime/_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_graph_executor.py` & `hgraph-0.2.9/src/hgraph/_runtime/_graph_executor.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_graph_recorder.py` & `hgraph-0.2.9/src/hgraph/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_graph_runner.py` & `hgraph-0.2.9/src/hgraph/_runtime/_graph_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from dataclasses import dataclass, field
-from dataclasses import dataclass, field
 from datetime import datetime
 from logging import Logger, getLogger, DEBUG, StreamHandler, Formatter
 from typing import Callable, Any
 
 from hgraph._runtime._constants import MIN_ST, MAX_ET, MIN_DT
 from hgraph._runtime._evaluation_engine import EvaluationMode, EvaluationLifeCycleObserver
 from hgraph._runtime._graph_executor import GraphEngineFactory
-from hgraph._runtime._graph_recorder import GraphRecorder
+import warnings
 
 __all__ = ("run_graph", "evaluate_graph", "GraphConfiguration")
 
 from hgraph._runtime._graph_recorder import GraphRecorder
 
 
 def _default_logger() -> Logger:
@@ -24,17 +23,24 @@
         ch.setLevel(DEBUG)
         # create formatter
         formatter = Formatter('%(asctime)s [%(name)s][%(levelname)s] %(message)s')
         # add formatter to ch
         ch.setFormatter(formatter)
         # add ch to logger
         logger.addHandler(ch)
+    warnings.showwarning = warn_with_log
+    warnings.filterwarnings("once", category=DeprecationWarning)
     return logger
 
 
+def warn_with_log(message, category, filename, lineno, file=None, line=None):
+    log = getLogger("hgraph")
+    log.warning(f"{filename}:{lineno}: {category.__name__}: {message}")
+
+
 @dataclass
 class GraphConfiguration:
     run_mode: EvaluationMode = EvaluationMode.SIMULATION
     start_time: datetime = MIN_DT
     end_time: datetime = MAX_ET
     trace: bool = False
     life_cycle_observers: tuple[EvaluationLifeCycleObserver] = tuple()
```

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_lifecycle.py` & `hgraph-0.2.9/src/hgraph/_runtime/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_node.py` & `hgraph-0.2.9/src/hgraph/_runtime/_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_runtime/_operators.py` & `hgraph-0.2.9/src/hgraph/_runtime/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/__init__.py` & `hgraph-0.2.9/src/hgraph/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_error_type.py` & `hgraph-0.2.9/src/hgraph/_types/_error_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_frame_scalar_type_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_frame_scalar_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ref_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_ref_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ref_type.py` & `hgraph-0.2.9/src/hgraph/_types/_ref_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_scalar_type_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_scalar_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_scalar_types.py` & `hgraph-0.2.9/src/hgraph/_types/_scalar_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_scalar_value.py` & `hgraph-0.2.9/src/hgraph/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_schema_type.py` & `hgraph-0.2.9/src/hgraph/_types/_schema_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,14 @@
                 k = parm
                 v = item
             if not isinstance(k, TypeVar):
                 raise ParseError(f"'{cls}' type '{k}' is not an instance of TypeVar as required")
             if k in resolution_dict:
                 raise ParseError(f"'{cls}' has already defined '{k}'")
             if parsed_v := cls._parse_type(v):
-                # if not parsed_v.is_resolved:
-                #     raise ParseError(f"'{cls}' type '{k}': '{v}' is an unresolved type, not support")
                 resolution_dict[k] = parsed_v
             else:
                 raise ParseError(f"In '{cls}' type '{k}': '{v}' was unable to parse as a valid type")
         if len(resolution_dict) < len(cls.__parameters__):
             # Only a partial resolution is place
             return cls._create_partial_resolved_class(resolution_dict)
```

### Comparing `hgraph-0.2.8/src/hgraph/_types/_time_series_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_time_series_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_time_series_types.py` & `hgraph-0.2.9/src/hgraph/_types/_time_series_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ts_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_ts_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ts_signal_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_ts_signal_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ts_type.py` & `hgraph-0.2.9/src/hgraph/_types/_ts_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_ts_type_var_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_ts_type_var_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsb_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_tsb_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsb_type.py` & `hgraph-0.2.9/src/hgraph/_types/_tsb_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsd_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_tsd_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsd_type.py` & `hgraph-0.2.9/src/hgraph/_types/_tsd_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsl_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_tsl_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tsl_type.py` & `hgraph-0.2.9/src/hgraph/_types/_tsl_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tss_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_tss_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_tss_type.py` & `hgraph-0.2.9/src/hgraph/_types/_tss_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_type_meta_data.py` & `hgraph-0.2.9/src/hgraph/_types/_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_types/_typing_utils.py` & `hgraph-0.2.9/src/hgraph/_types/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/__init__.py` & `hgraph-0.2.9/src/hgraph/_wiring/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_decorators.py` & `hgraph-0.2.9/src/hgraph/_wiring/_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,72 +24,76 @@
 
 def compute_node(fn: COMPUTE_NODE_SIGNATURE = None, /,
                  node_impl=None,
                  active: Sequence[str] = None,
                  valid: Sequence[str] = None,
                  all_valid: Sequence[str] = None,
                  overloads: "WiringNodeClass" | COMPUTE_NODE_SIGNATURE = None,
-                 resolvers: Mapping[TypeVar, Callable] = None) -> COMPUTE_NODE_SIGNATURE:
+                 resolvers: Mapping[TypeVar, Callable] = None,
+                 deprecated: bool | str = False) -> COMPUTE_NODE_SIGNATURE:
     """
     Used to define a python function to be a compute-node. A compute-node is the worker unit in the graph and
     will be called each time of the inputs to the compute node ticks.
     A compute-node requires inputs and outputs.
 
     :param fn: The function to wrap
     :param node_impl: The node implementation to use (this makes fn a signature only method)
     :param active: Which inputs to mark as being active (by default all are active)
     :param valid: Which inputs to require to be valid (by default all are valid)
     :param all_valid: Which inputs are required to be ``all_valid`` (by default none are all_valid)
     :param overloads: If this node overloads an operator, this is the operator it is designed to overload.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.COMPUTE_NODE, fn, node_impl, active, valid, all_valid, overloads=overloads,
-                           resolvers=resolvers)
+                           resolvers=resolvers, deprecated=deprecated)
 
 
 def pull_source_node(fn: SOURCE_NODE_SIGNATURE = None, /, node_impl=None,
-                     resolvers: Mapping[TypeVar, Callable] = None) -> SOURCE_NODE_SIGNATURE:
+                     resolvers: Mapping[TypeVar, Callable] = None,
+                     deprecated: bool | str = False) -> SOURCE_NODE_SIGNATURE:
     """
     Used to indicate the signature for a source node. For Python source nodes use either the
     generator or source_adapter annotations.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.PULL_SOURCE_NODE, fn, node_impl, resolvers=resolvers)
+    return _node_decorator(WiringNodeType.PULL_SOURCE_NODE, fn, node_impl, resolvers=resolvers, deprecated=deprecated)
 
 
 def push_source_node(fn: SOURCE_NODE_SIGNATURE = None, /, node_impl=None,
-                     resolvers: Mapping[TypeVar, Callable] = None) -> SOURCE_NODE_SIGNATURE:
+                     resolvers: Mapping[TypeVar, Callable] = None,
+                     deprecated: bool | str = False) -> SOURCE_NODE_SIGNATURE:
     """
     Used to indicate the signature for a push source node.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.PUSH_SOURCE_NODE, fn, node_impl, resolvers=resolvers)
+    return _node_decorator(WiringNodeType.PUSH_SOURCE_NODE, fn, node_impl, resolvers=resolvers, deprecated=deprecated)
 
 
 def sink_node(fn: SINK_NODE_SIGNATURE = None, /,
               node_impl=None,
               active: Sequence[str] = None,
               valid: Sequence[str] = None,
               all_valid: Sequence[str] = None,
               overloads: "WiringNodeClass" | SINK_NODE_SIGNATURE = None,
-              resolvers: Mapping[TypeVar, Callable] = None) -> SINK_NODE_SIGNATURE:
+              resolvers: Mapping[TypeVar, Callable] = None,
+              deprecated: bool | str = False) -> SINK_NODE_SIGNATURE:
     """
     Indicates the function definition represents a sink node. This type of node has no return type.
     Other than that it behaves in much the same way as compute node.
 
     :param fn: The function to wrap
     :param node_impl: The node implementation to use (this makes fn a signature only method)
     :param active: Which inputs to mark as being active (by default all are active)
     :param valid: Which inputs to require to be valid (by default all are valid)
     :param all_valid: Which inputs are required to be ``all_valid`` (by default none are all_valid)
     :param overloads: If this node overloads an operator, this is the operator it is designed to overload.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.SINK_NODE, fn, node_impl, active, valid, all_valid, overloads=overloads,
-                           resolvers=resolvers)
+                           resolvers=resolvers, deprecated=deprecated)
 
 
 def graph(fn: GRAPH_SIGNATURE = None,
           overloads: "WiringNodeClass" | GRAPH_SIGNATURE = None,
           resolvers: Mapping[TypeVar, Callable] = None) -> GRAPH_SIGNATURE:
     """
     Wraps a wiring function. The function can take the form of a function that looks like a compute_node,
@@ -98,15 +102,16 @@
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.GRAPH, fn, overloads=overloads, resolvers=resolvers)
 
 
 def generator(fn: SOURCE_NODE_SIGNATURE = None,
               overloads: "WiringNodeClass" | GRAPH_SIGNATURE = None,
-              resolvers: Mapping[TypeVar, Callable] = None) -> SOURCE_NODE_SIGNATURE:
+              resolvers: Mapping[TypeVar, Callable] = None,
+              deprecated: bool | str = False) -> SOURCE_NODE_SIGNATURE:
     """
     Creates a pull source node that supports generating a sequence of ticks that will be fed into the
     graph. The generator wraps a function that is implemented as a python generator which returns a tuple of
     time (or timedelta) and value.
 
     For example:
     ```Python
@@ -123,20 +128,21 @@
     The generator will fetch the first tick during the start life-cycle of the node. If no tick is returned, the
     generator WILL do NOTHING.
 
     """
     from hgraph._wiring._wiring_node_class._python_wiring_node_classes import PythonGeneratorWiringNodeClass
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.PULL_SOURCE_NODE, fn, overloads=overloads,
-                           node_class=PythonGeneratorWiringNodeClass, resolvers=resolvers)
+                           node_class=PythonGeneratorWiringNodeClass, resolvers=resolvers, deprecated=deprecated)
 
 
 def push_queue(tp: type[TIME_SERIES_TYPE],
                overloads: "WiringNodeClass" | SOURCE_NODE_SIGNATURE = None,
-               resolvers: Mapping[TypeVar, Callable] = None
+               resolvers: Mapping[TypeVar, Callable] = None,
+               deprecated: bool | str = False
                ):
     """
     Creates a push source node that supports injecting values into the graph asynchronously.
     The function that is wrapped by this decorator will be called as a start lifecycle method.
     The function must take as its first parameter the sender callable.
     It is possible to take additional scalar values that will be provided as kwargs.
 
@@ -155,15 +161,16 @@
         sig = signature(fn)
         sender_arg = next(iter(sig.parameters.keys()))
         annotations = {k: v.annotation for k, v in sig.parameters.items() if k != sender_arg}
         defaults = {k: v.default for k, v in sig.parameters.items() if k != sender_arg}
 
         node = _create_node(_create_node_signature(fn.__name__,
                                                    annotations, tp, defaults=defaults,
-                                                   node_type=WiringNodeType.PUSH_SOURCE_NODE),
+                                                   node_type=WiringNodeType.PUSH_SOURCE_NODE,
+                                                   deprecated=deprecated),
                             impl_fn=fn, node_type=WiringNodeType.PUSH_SOURCE_NODE,
                             node_class=PythonPushQueueWiringNodeClass)
 
         if resolvers is not None:
             node = node[tuple(slice(k, v) for k, v in resolvers.items())]
 
         if overloads is not None:
@@ -246,20 +253,22 @@
 
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
     return _node_decorator(WiringNodeType.REQ_REP_SVC, fn, resolvers=resolvers)
 
 
 def service_impl(*, interfaces: Sequence[SERVICE_DEFINITION] | SERVICE_DEFINITION = None,
-                 resolvers: Mapping[TypeVar, Callable] = None):
+                 resolvers: Mapping[TypeVar, Callable] = None,
+                 deprecated: bool | str = False):
     """
     Wraps a service implementation. The service is defined to implement the declared interface.
     """
     from hgraph._wiring._wiring_node_signature import WiringNodeType
-    return _node_decorator(WiringNodeType.SVC_IMPL, None, interfaces=interfaces, resolvers=resolvers)
+    return _node_decorator(WiringNodeType.SVC_IMPL, None, interfaces=interfaces, resolvers=resolvers,
+                           deprecated=deprecated)
 
 
 def register_service(path: str, implementation, resolution_dict=None, **kwargs):
     """
     Binds the implementation of the interface to the path provided. The additional kwargs
     are passed to the implementation. These should be defined on the implementation and are independent of the
     attributes defined in the service.
@@ -309,27 +318,29 @@
     """
 
 
 def _node_decorator(node_type: "WiringNodeType", impl_fn, node_impl=None, active: Sequence[str] = None,
                     valid: Sequence[str] = None, all_valid: Sequence[str] = None,
                     node_class: Type["WiringNodeClass"] = None,
                     overloads: "WiringNodeClass" = None, interfaces=None,
-                    resolvers: Mapping[TypeVar, Callable] = None) -> Callable:
+                    resolvers: Mapping[TypeVar, Callable] = None,
+                    deprecated: bool | str = False) -> Callable:
     from hgraph._wiring._wiring_node_class._wiring_node_class import WiringNodeClass
     from hgraph._wiring._wiring_node_class._node_impl_wiring_node_class import NodeImplWiringNodeClass
     from hgraph._wiring._wiring_node_class._graph_wiring_node_class import GraphWiringNodeClass
     from hgraph._wiring._wiring_node_class._python_wiring_node_classes import PythonWiringNodeClass
     from hgraph._wiring._wiring_node_signature import WiringNodeType
 
     kwargs = dict(node_type=node_type,
                   node_class=PythonWiringNodeClass if node_class is None else node_class,
                   active=active,
                   valid=valid,
                   all_valid=all_valid,
-                  interfaces=interfaces)
+                  interfaces=interfaces,
+                  deprecated=deprecated, )
     if node_impl is not None:
         if isinstance(node_impl, type) and issubclass(node_impl, WiringNodeClass):
             kwargs["node_class"] = node_impl
         else:
             kwargs['node_class'] = NodeImplWiringNodeClass
             kwargs['impl_fn'] = node_impl
 
@@ -383,40 +394,47 @@
         raise ValueError(f"{label} do not support ticked")
     if kwargs.get("valid") is not None:
         raise ValueError(f"{label} do not support valid")
     if kwargs.get("all_valid") is not None:
         raise ValueError(f"{label} do not support all_valid")
 
 
-def _create_node(signature_fn, impl_fn=None, node_type: "WiringNodeType" = None,
-                 node_class: Type["WiringNodeClass"] = None, active: Sequence[str] = None, valid: Sequence[str] = None,
-                 all_valid: Sequence[str] = None, interfaces=None, resolver=None) -> "WiringNodeClass":
+def _create_node(signature_fn, impl_fn=None,
+                 node_type: "WiringNodeType" = None,
+                 node_class: Type["WiringNodeClass"] = None,
+                 active: Sequence[str] = None,
+                 valid: Sequence[str] = None,
+                 all_valid: Sequence[str] = None,
+                 interfaces=None,
+                 resolver=None,
+                 deprecated: bool | str = False) -> "WiringNodeClass":
     """
     Create the wiring node using the supplied node_type and impl_fn, for non-cpp types the impl_fn is assumed to be
     the signature fn as well.
     """
     from hgraph._wiring._wiring_node_signature import extract_signature
     if impl_fn is None:
         impl_fn = signature_fn
     from hgraph._wiring._wiring_node_signature import WiringNodeSignature
     active_inputs = frozenset(active) if active is not None else None
     valid_inputs = frozenset(valid) if valid is not None else None
     all_valid_inputs = frozenset(all_valid) if all_valid is not None else None
     signature = signature_fn if isinstance(signature_fn, WiringNodeSignature) else \
         extract_signature(signature_fn, node_type, active_inputs=active_inputs, valid_inputs=valid_inputs,
-                          all_valid_inputs=all_valid_inputs)
+                          all_valid_inputs=all_valid_inputs, deprecated=deprecated)
     if interfaces is None:
         return node_class(signature, impl_fn)
     else:
         return node_class(signature, impl_fn, interfaces=interfaces)
 
 
 def _create_node_signature(name: str, kwargs: dict[str, Type], ret_type: Type, node_type: "WiringNodeType",
                            active_inputs: frozenset[str] = None, valid_inputs: frozenset[str] = None,
-                           all_valid_inputs: frozenset[str] = None, defaults: dict[str, Any] = None) -> Callable:
+                           all_valid_inputs: frozenset[str] = None, defaults: dict[str, Any] = None,
+                           deprecated: bool | str = False) -> Callable:
     """
     Create a function that takes the kwargs and returns the kwargs. This is used to create a function that
     can be used to create a signature.
     """
     from hgraph._wiring._wiring_node_class._wiring_node_class import WiringNodeSignature
     from hgraph import HgScalarTypeMetaData, HgTimeSeriesTypeMetaData
 
@@ -431,10 +449,14 @@
         output_type=HgTimeSeriesTypeMetaData.parse_type(ret_type) if ret_type is not None else None,
         src_location=SourceCodeDetails(Path(), 0),  # TODO: make this point to a real place in code.
         active_inputs=active_inputs,
         valid_inputs=valid_inputs,
         all_valid_inputs=all_valid_inputs,
         unresolved_args=frozenset(),
         time_series_args=frozenset(),
-        injectable_inputs=extract_injectable_inputs(**kwargs)
+        injectable_inputs=extract_injectable_inputs(**kwargs),
+        deprecated=deprecated
     )
     return signature
+
+
+CALLABLE = TypeVar("CALLABLE", bound=Callable)
```

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_dispatch.py` & `hgraph-0.2.9/src/hgraph/_wiring/_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_exception_handling.py` & `hgraph-0.2.9/src/hgraph/_wiring/_exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_graph_builder.py` & `hgraph-0.2.9/src/hgraph/_wiring/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_map.py` & `hgraph-0.2.9/src/hgraph/_wiring/_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_reduce.py` & `hgraph-0.2.9/src/hgraph/_wiring/_reduce.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_stub_wiring_node.py` & `hgraph-0.2.9/src/hgraph/_wiring/_stub_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_switch.py` & `hgraph-0.2.9/src/hgraph/_wiring/_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_context.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_context.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_errors.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_errors.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_instance.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_instance.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_signature.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     unresolved_args: frozenset[str]
     time_series_args: frozenset[str]
     injectable_inputs: InjectableTypes = InjectableTypes(0)
     # It is not possible to have an unresolved output with un-resolved inputs as we resolve output using information
     # supplied via inputs
     label: str | None = None  # A label if provided, this can help to disambiguate the node
     record_and_replay_id: str | None = None
+    deprecated: str  | bool = False
 
     @property
     def uses_scheduler(self) -> bool:
         return InjectableTypes.SCHEDULER in self.injectable_inputs
 
     @property
     def uses_clock(self) -> bool:
@@ -111,15 +112,16 @@
     def as_dict(self) -> dict:
         return dict(node_type=self.node_type, name=self.name, args=self.args, defaults=self.defaults,
                     input_types=self.input_types, output_type=self.output_type, src_location=self.src_location,
                     active_inputs=self.active_inputs, valid_inputs=self.valid_inputs,
                     all_valid_inputs=self.all_valid_inputs,
                     unresolved_args=self.unresolved_args, time_series_args=self.time_series_args,
                     injectable_inputs=self.injectable_inputs, label=self.label,
-                    record_and_replay_id=self.record_and_replay_id)
+                    record_and_replay_id=self.record_and_replay_id,
+                    deprecated=self.deprecated)
 
     def copy_with(self, **kwargs: Any) -> "WiringNodeSignature":
         kwargs_ = self.as_dict() | kwargs
         return WiringNodeSignature(**kwargs_)
 
     @property
     def signature(self) -> str:
@@ -314,18 +316,20 @@
             if isinstance(kwargs[k], WiringPort):
                 if not v.dereference().matches(kwargs[k].output_type.dereference()):
                     raise IncorrectTypeBinding(v, kwarg_types[k])
             else:
                 if not v.dereference().matches(kwarg_types[k].dereference()):
                     raise IncorrectTypeBinding(v, kwarg_types[k])
 
+
 def extract_signature(fn, wiring_node_type: WiringNodeType,
                       active_inputs: frozenset[str] | None = None,
                       valid_inputs: frozenset[str] | None = None,
-                      all_valid_inputs: frozenset[str] | None = None) -> WiringNodeSignature:
+                      all_valid_inputs: frozenset[str] | None = None,
+                      deprecated: bool = False) -> WiringNodeSignature:
     """
     Performs signature extract that will work for python 3.9 (and possibly above)
     :param fn:
     :return:
     """
     name = fn.__name__
     annotations = get_type_hints(fn)
@@ -391,15 +395,16 @@
         valid_inputs=valid_inputs,
         all_valid_inputs=all_valid_inputs,
         src_location=SourceCodeDetails(file=filename, start_line=first_line),
         unresolved_args=unresolved_inputs,
         time_series_args=time_series_inputs,
         injectable_inputs=injectable_inputs,
         label=None,
-        record_and_replay_id=None
+        record_and_replay_id=None,
+        deprecated=deprecated
     )
 
 
 def extract_injectable_inputs(**kwargs) -> InjectableTypes:
     return reduce(or_,
                   ({
                        HgSchedulerType: InjectableTypes.SCHEDULER,
```

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_port.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_port.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_utils.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/__init__.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py` & `hgraph-0.2.9/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import inspect
 from dataclasses import replace
-from types import GenericAlias
 from typing import Callable, Any, TypeVar, _GenericAlias, Mapping, TYPE_CHECKING, Tuple, List
 
 from frozendict import frozendict
 
-from hgraph._types._scalar_type_meta_data import HgTypeOfTypeMetaData, HgScalarTypeMetaData
 from hgraph._types._time_series_meta_data import HgTimeSeriesTypeMetaData
 from hgraph._types._tsb_meta_data import HgTSBTypeMetaData, HgTimeSeriesSchemaTypeMetaData
-from hgraph._types._type_meta_data import HgTypeMetaData, ParseError, AUTO_RESOLVE
+from hgraph._types._type_meta_data import HgTypeMetaData, AUTO_RESOLVE
 from hgraph._wiring._wiring_context import WiringContext
-from hgraph._wiring._wiring_errors import WiringError, IncorrectTypeBinding, MissingInputsError, \
+from hgraph._wiring._wiring_errors import WiringError, MissingInputsError, \
     CustomMessageWiringError, WiringFailureError
 from hgraph._wiring._wiring_node_instance import WiringNodeInstance, create_wiring_node_instance
 from hgraph._wiring._wiring_node_signature import WiringNodeSignature, WiringNodeType
 from hgraph._wiring._wiring_port import _wiring_port_for, WiringPort
 
 if TYPE_CHECKING:
     from hgraph._builder._node_builder import NodeBuilder
@@ -169,16 +167,16 @@
         """
         kwargs_ = prepare_kwargs(self.signature, *args, **kwargs)
         return kwargs_
 
     def resolve_signature(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None,
                           **kwargs) -> "WiringNodeSignature":
         _, resolved_signature, _ = self._validate_and_resolve_signature(*args,
-                                                                     __pre_resolved_types__=__pre_resolved_types__,
-                                                                     **kwargs)
+                                                                        __pre_resolved_types__=__pre_resolved_types__,
+                                                                        **kwargs)
         return resolved_signature
 
     def _validate_and_resolve_signature(self, *args,
                                         __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable],
                                         __enforce_output_type__: bool = True,
                                         **kwargs) \
             -> tuple[dict[str, Any], WiringNodeSignature, dict[TypeVar, HgTypeMetaData]]:
@@ -256,30 +254,35 @@
         if found_overload:
             return r
 
         # TODO: Capture the call site information (line number / file etc.) for better error reporting.
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
             # Now validate types and resolve any un-resolved types and provide an updated signature.
             kwargs_, resolved_signature, _ = self._validate_and_resolve_signature(*args,
-                                                                               __pre_resolved_types__=__pre_resolved_types__,
-                                                                               **kwargs)
+                                                                                  __pre_resolved_types__=__pre_resolved_types__,
+                                                                                  **kwargs)
 
             # TODO: This mechanism to work out rank may fail when using a delayed binding?
             match resolved_signature.node_type:
                 case WiringNodeType.PUSH_SOURCE_NODE:
                     rank = 0
                 case WiringNodeType.PULL_SOURCE_NODE | WiringNodeType.REF_SVC:
                     rank = 1
                 case WiringNodeType.COMPUTE_NODE | WiringNodeType.SINK_NODE | WiringNodeType.SUBS_SVC:
                     rank = max(v.rank for k, v in kwargs_.items() if
                                v is not None and k in self.signature.time_series_args) + 1024  # leave enough space of all services
                 case _:
                     raise CustomMessageWiringError(
                         f"Wiring type: {resolved_signature.node_type} is not supported as a wiring node class")
-
+            if self.signature.deprecated:
+                import warnings
+                warnings.warn(
+                    f"{self.signature.signature} is deprecated and will be removed in a future version."
+                    f"{(' ' + self.signature.deprecated) if type(self.signature.deprecated) is str else ''}",
+                    DeprecationWarning, stacklevel=3)
             wiring_node_instance = create_wiring_node_instance(self, resolved_signature, frozendict(kwargs_), rank=rank)
             # Select the correct wiring port for the TS type! That we can provide useful wiring syntax
             # to support this like out.p1 on a bundle or out.s1 on a ComplexScalar, etc.
 
             if resolved_signature.node_type is WiringNodeType.SINK_NODE:
                 from hgraph._wiring._wiring_node_class._graph_wiring_node_class import WiringGraphContext
                 WiringGraphContext.instance().add_sink_node(wiring_node_instance)
```

### Comparing `hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspective.py` & `hgraph-0.2.9/src/hgraph/adaptors/perspective/_perspective.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/adaptors/perspective/_perspetive_publish.py` & `hgraph-0.2.9/src/hgraph/adaptors/perspective/_perspetive_publish.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/adaptors/perspective/index_template.html` & `hgraph-0.2.9/src/hgraph/adaptors/perspective/index_template.html`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/adaptors/perspective/table_template.html` & `hgraph-0.2.9/src/hgraph/adaptors/perspective/table_template.html`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/adaptors/perspective/workspace_template.html` & `hgraph-0.2.9/src/hgraph/adaptors/perspective/workspace_template.html`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/__init__.py` & `hgraph-0.2.9/src/hgraph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_analytical.py` & `hgraph-0.2.9/src/hgraph/nodes/_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_compound_scalar_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_const.py` & `hgraph-0.2.9/src/hgraph/nodes/_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_data_source_polars.py` & `hgraph-0.2.9/src/hgraph/nodes/_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_datetime_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_datetime_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_format.py` & `hgraph-0.2.9/src/hgraph/nodes/_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_frame_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_frame_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_math.py` & `hgraph-0.2.9/src/hgraph/nodes/_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_numpy.py` & `hgraph-0.2.9/src/hgraph/nodes/_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_print.py` & `hgraph-0.2.9/src/hgraph/nodes/_print.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_record.py` & `hgraph-0.2.9/src/hgraph/nodes/_record.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_replay.py` & `hgraph-0.2.9/src/hgraph/nodes/_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_service_utils.py` & `hgraph-0.2.9/src/hgraph/nodes/_service_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_set_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_set_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_stream_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_stream_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_tsb_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_tsd_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_tsd_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_tsl_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_tss_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_tuple_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_tuple_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/nodes/_window_operators.py` & `hgraph-0.2.9/src/hgraph/nodes/_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/notebook/NoteBook.md` & `hgraph-0.2.9/src/hgraph/notebook/NoteBook.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/notebook/_notebook_graph.py` & `hgraph-0.2.9/src/hgraph/notebook/_notebook_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/test/_node_printer.py` & `hgraph-0.2.9/src/hgraph/test/_node_printer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/test/_node_unit_tester.py` & `hgraph-0.2.9/src/hgraph/test/_node_unit_tester.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/src/hgraph/test/testing.md` & `hgraph-0.2.9/src/hgraph/test/testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/test_wiring.py` & `hgraph-0.2.9/tests/python/unit/hgraph/test_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_feedback.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_runtime/test_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_runtime/test_scheduler.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_runtime/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_complex_types.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_types/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_operator_rank.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_types/test_operator_rank.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_data.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_types/test_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_types/test_type_meta_resolve.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_types/test_type_meta_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_const.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_auto_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_auto_resolve.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_auto_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_decorators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_dispatch.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_error_handling.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_generic_graphs.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_generic_graphs.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_map.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_overloads.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_overloads.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_ref.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_ref.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from typing import cast
 
 from hgraph import TIME_SERIES_TYPE, compute_node, REF, TS, TSL, Size, SIZE, graph, TSS, TSD, REMOVE, \
-    PythonTimeSeriesReference, Removed, K, KEYABLE_SCALAR
+    Removed, K, KEYABLE_SCALAR
 from hgraph.nodes import tss_contains
+from hgraph.nodes._conditional import route_ref
 from hgraph.test import eval_node
 
 
 @compute_node
 def create_ref(ts: REF[TIME_SERIES_TYPE]) -> REF[TIME_SERIES_TYPE]:
     return ts.value
 
 
 def test_ref():
     assert eval_node(create_ref[TIME_SERIES_TYPE: TS[int]], ts=[1, 2]) == [1, 2]
 
 
-@compute_node
-def route_ref(condition: TS[bool], ts: REF[TIME_SERIES_TYPE]) -> TSL[REF[TIME_SERIES_TYPE], Size[2]]:
-    return cast(TSL,
-                (ts.value, PythonTimeSeriesReference()) if condition.value else (PythonTimeSeriesReference(), ts.value))
-
-
 def test_route_ref():
     assert eval_node(route_ref[TIME_SERIES_TYPE: TS[int]], condition=[True, None, False, None], ts=[1, 2, None, 4]) == [
         {0: 1}, {0: 2}, {1: 2}, {1: 4}]
 
 
 @compute_node
 def merge_ref(index: TS[int], ts: TSL[REF[TIME_SERIES_TYPE], SIZE]) -> REF[TIME_SERIES_TYPE]:
```

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_service.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_service.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_switch.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from typing import Generic
+
 import pytest
 
-from hgraph import TSB, TimeSeriesSchema, TS, compute_node, graph, IncorrectTypeBinding, ParseError
+from hgraph import TSB, TimeSeriesSchema, TS, compute_node, graph, IncorrectTypeBinding, ParseError, TIME_SERIES_TYPE, \
+    SCALAR, SCALAR_1
 from hgraph.test import eval_node
 
 
 class MyTsb(TimeSeriesSchema):
     p1: TS[int]
     p2: TS[str]
 
@@ -78,7 +81,24 @@
     try:
         @graph
         def tsb_bad_return_type() -> MyTsb:
             ...
         assert False, "Should have raised an exception"
     except ParseError:
         ...
+
+
+def test_generic_tsb():
+    from frozendict import frozendict as fd
+
+    class GenericTSB(TimeSeriesSchema, Generic[SCALAR]):
+        p1: TS[SCALAR]
+
+    @compute_node
+    def tsb_multi_type(ts: TSB[GenericTSB[SCALAR]], v: TS[SCALAR_1]) -> TSB[GenericTSB[SCALAR_1]]:
+        return {"p1": v.value}
+
+    @graph
+    def g(ts1: TS[int], ts2: TS[str]) -> TSB[GenericTSB[str]]:
+        return tsb_multi_type(TSB[GenericTSB[int]].from_ts(p1=ts1), ts2)
+
+    assert eval_node(g, [1, 2], ["a", "b"]) == [fd({"p1": "a"}), fd({"p1": "b"})]
```

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_tss.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py` & `hgraph-0.2.9/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_analytical.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_const.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_data_source_polars.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_format.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_frame.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_frame.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_math.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_numpy.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_push_queue.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_push_queue.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_recorder.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsb_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsd_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsd_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tsl_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_tss_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_window_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/nodes/test_wp_operators.py` & `hgraph-0.2.9/tests/python/unit/hgraph/nodes/test_wp_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/tests/python/unit/hgraph/test/test_node_printer.py` & `hgraph-0.2.9/tests/python/unit/hgraph/test/test_node_printer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/LICENSE` & `hgraph-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/README.md` & `hgraph-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.8/pyproject.toml` & `hgraph-0.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 name = "hgraph"
 dynamic = ["version"]
 dependencies = [
     "frozendict>=2.3.10",
     "sortedcontainers>=2.4.0",
     "ordered-set>=4.1.0",
     "numpy>=1.23",
-    "polars>=0.20.15",
+    "polars>=0.20.18",
+    "sqlalchemy>=2.0.29",
+    "duckdb>=0.10.1",
+    "pyarrow>=15.0.2"
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "Howard Henson", email = "howard@henson.me.uk" },
 ]
 maintainers = [
 ]
```

### Comparing `hgraph-0.2.8/PKG-INFO` & `hgraph-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: hgraph
-Version: 0.2.8
+Version: 0.2.9
 Summary: A functional reactive engine
 Project-URL: Homepage, https://github.com/hhenson/hgraph
 Project-URL: Repository, https://github.com/hhenson/hgraph.git
 Author-email: Howard Henson <howard@henson.me.uk>
 License: MIT License
         
         Copyright (c) 2023 Howard Henson
@@ -29,19 +29,22 @@
 License-File: LICENSE
 Keywords: forward propogating graph,fpg,functional reactive programming,graph,reactive,time series
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
+Requires-Dist: duckdb>=0.10.1
 Requires-Dist: frozendict>=2.3.10
 Requires-Dist: numpy>=1.23
 Requires-Dist: ordered-set>=4.1.0
-Requires-Dist: polars>=0.20.15
+Requires-Dist: polars>=0.20.18
+Requires-Dist: pyarrow>=15.0.2
 Requires-Dist: sortedcontainers>=2.4.0
+Requires-Dist: sqlalchemy>=2.0.29
 Description-Content-Type: text/markdown
 
 # hgraph
 A functional reactive programming engine with a Python front-end.
 
 This provides a DSL and runtime to support the computation of results over time, featuring
 a graph based directed acyclic dependency graph and the concept of time-series properties.
```

