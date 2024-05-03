# Comparing `tmp/penzai-0.1.0.tar.gz` & `tmp/penzai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penzai-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "penzai-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `penzai-0.1.0.tar` & `penzai-0.1.1.tar`

### file list

```diff
@@ -1,165 +1,168 @@
--rw-r--r--   0        0        0      731 2024-04-17 19:09:44.663782 penzai-0.1.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0      275 2024-04-18 03:04:49.751435 penzai-0.1.0/.gitignore
--rw-r--r--   0        0        0    14782 2024-04-12 16:02:48.473126 penzai-0.1.0/.pylintrc
--rw-r--r--   0        0        0      552 2024-04-18 03:04:49.751435 penzai-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       65 2024-04-12 16:02:48.473126 penzai-0.1.0/.vscode/extensions.json
--rw-r--r--   0        0        0      868 2024-04-12 16:02:48.473126 penzai-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      335 2024-04-12 16:02:48.473126 penzai-0.1.0/AUTHORS
--rw-r--r--   0        0        0      970 2024-04-12 16:02:48.473126 penzai-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2024-04-12 16:02:48.473126 penzai-0.1.0/LICENSE
--rw-r--r--   0        0        0     4536 2024-04-18 03:04:49.751435 penzai-0.1.0/README.md
--rw-r--r--   0        0        0       23 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/.gitignore
--rw-r--r--   0        0        0      644 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      621 2024-04-14 19:54:03.230332 penzai-0.1.0/docs/_autogen_root.rst
--rw-r--r--   0        0        0     5101 2024-04-18 04:12:25.549193 penzai-0.1.0/docs/_include/_glue_figures.ipynb
--rw-r--r--   0        0        0      638 2024-04-18 03:04:49.751435 penzai-0.1.0/docs/_static/custom.css
--rw-r--r--   0        0        0     2523 2024-04-18 03:04:49.751435 penzai-0.1.0/docs/_static/custom.js
--rw-r--r--   0        0        0      102 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/_templates/pzbase.rst
--rw-r--r--   0        0        0     1889 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/_templates/pzclass.rst
--rw-r--r--   0        0        0      106 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/_templates/pzdata.rst
--rw-r--r--   0        0        0     1294 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/_templates/pzmodule.rst
--rw-r--r--   0        0        0     1298 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/_templates/pzmodule_full.rst
--rw-r--r--   0        0        0     1559 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/api/pz.de.rst
--rw-r--r--   0        0        0     1968 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/api/pz.nn.rst
--rw-r--r--   0        0        0     4241 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/api/pz.rst
--rw-r--r--   0        0        0     1451 2024-04-12 16:02:48.477126 penzai-0.1.0/docs/api/pz.ts.rst
--rw-r--r--   0        0        0     7615 2024-04-18 03:04:49.751435 penzai-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     2003 2024-04-16 03:31:21.126952 penzai-0.1.0/docs/ext/nb_output_cell_to_iframe.py
--rw-r--r--   0        0        0     1370 2024-04-12 16:02:48.481127 penzai-0.1.0/docs/ext/pz_alias_rewrite.py
--rw-r--r--   0        0        0     5570 2024-04-18 03:04:49.751435 penzai-0.1.0/docs/index.rst
--rw-r--r--   0        0        0     3029 2024-04-18 04:12:49.495555 penzai-0.1.0/docs/scripts/readthedocs_fetch_notebook_outputs.sh
--rw-r--r--   0        0        0    71853 2024-04-18 04:12:25.549193 penzai-0.1.0/notebooks/data_effects.ipynb
--rw-r--r--   0        0        0   189024 2024-04-18 05:18:38.910240 penzai-0.1.0/notebooks/gemma_from_scratch.ipynb
--rw-r--r--   0        0        0    51069 2024-04-18 04:12:25.553194 penzai-0.1.0/notebooks/how_to_think_in_penzai.ipynb
--rw-r--r--   0        0        0   142008 2024-04-18 04:12:25.553194 penzai-0.1.0/notebooks/induction_heads.ipynb
--rw-r--r--   0        0        0   144103 2024-04-18 04:12:25.553194 penzai-0.1.0/notebooks/induction_heads_2B.ipynb
--rw-r--r--   0        0        0    47272 2024-04-18 04:12:25.553194 penzai-0.1.0/notebooks/jitting_and_sharding.ipynb
--rw-r--r--   0        0        0    68268 2024-04-18 04:12:25.553194 penzai-0.1.0/notebooks/lora_from_scratch.ipynb
--rw-r--r--   0        0        0    38620 2024-04-18 04:12:25.557194 penzai-0.1.0/notebooks/named_axes.ipynb
--rw-r--r--   0        0        0    42727 2024-04-18 04:12:25.557194 penzai-0.1.0/notebooks/selectors.ipynb
--rw-r--r--   0        0        0    35018 2024-04-18 04:12:25.557194 penzai-0.1.0/notebooks/treescope_arrayviz.ipynb
--rw-r--r--   0        0        0    35468 2024-04-18 04:12:25.557194 penzai-0.1.0/notebooks/treescope_prettyprinting.ipynb
--rw-r--r--   0        0        0      692 2024-04-18 04:44:39.470971 penzai-0.1.0/penzai/__init__.py
--rw-r--r--   0        0        0      929 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/core/__init__.py
--rw-r--r--   0        0        0     6804 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/core/context.py
--rw-r--r--   0        0        0     3802 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/core/dataclass_util.py
--rw-r--r--   0        0        0     2448 2024-04-16 03:31:21.126952 penzai-0.1.0/penzai/core/formatting_util.py
--rw-r--r--   0        0        0     9414 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/core/layer.py
--rw-r--r--   0        0        0    63449 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/core/named_axes.py
--rw-r--r--   0        0        0     5305 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/core/partitioning.py
--rw-r--r--   0        0        0     3782 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/core/random_stream.py
--rw-r--r--   0        0        0    51444 2024-04-16 03:31:21.126952 penzai-0.1.0/penzai/core/selectors.py
--rw-r--r--   0        0        0    43200 2024-04-16 03:31:21.126952 penzai-0.1.0/penzai/core/shapecheck.py
--rw-r--r--   0        0        0    28518 2024-04-13 02:51:15.526660 penzai-0.1.0/penzai/core/struct.py
--rw-r--r--   0        0        0     1117 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/core/syntactic_sugar.py
--rw-r--r--   0        0        0     2384 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/core/tree_util.py
--rw-r--r--   0        0        0      744 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/data_effects/__init__.py
--rw-r--r--   0        0        0    20358 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/data_effects/effect_base.py
--rw-r--r--   0        0        0    24485 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/data_effects/local_state.py
--rw-r--r--   0        0        0    11914 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/data_effects/random.py
--rw-r--r--   0        0        0    14548 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/data_effects/side_input.py
--rw-r--r--   0        0        0     7259 2024-04-17 19:09:44.663782 penzai-0.1.0/penzai/data_effects/side_output.py
--rw-r--r--   0        0        0      735 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/example_models/gemma/__init__.py
--rw-r--r--   0        0        0    23796 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/example_models/gemma/model_core.py
--rw-r--r--   0        0        0    11242 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/example_models/gemma/sampling_mode.py
--rw-r--r--   0        0        0     9496 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/example_models/gemma/simple_decoding_loop.py
--rw-r--r--   0        0        0     2574 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/example_models/simple_mlp.py
--rw-r--r--   0        0        0      867 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/nn/__init__.py
--rw-r--r--   0        0        0    11698 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/nn/attention.py
--rw-r--r--   0        0        0     3276 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/nn/basic_ops.py
--rw-r--r--   0        0        0     4017 2024-04-12 16:02:48.489127 penzai-0.1.0/penzai/nn/combinators.py
--rw-r--r--   0        0        0     5272 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/nn/dropout.py
--rw-r--r--   0        0        0    12857 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/nn/embeddings.py
--rw-r--r--   0        0        0    11637 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/nn/grouping.py
--rw-r--r--   0        0        0    27178 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/nn/linear_and_affine.py
--rw-r--r--   0        0        0    23875 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/nn/parameters.py
--rw-r--r--   0        0        0     6596 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/nn/standardization.py
--rw-r--r--   0        0        0     1879 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/pz/__init__.py
--rw-r--r--   0        0        0     1941 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/pz/de.py
--rw-r--r--   0        0        0     2333 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/pz/nn.py
--rw-r--r--   0        0        0     1811 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/pz/ts.py
--rw-r--r--   0        0        0     5766 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/toolshed/annotate_shapes.py
--rw-r--r--   0        0        0    13543 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/toolshed/basic_training.py
--rw-r--r--   0        0        0     5362 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/toolshed/check_layers_by_tracing.py
--rw-r--r--   0        0        0     6445 2024-04-12 16:02:48.493127 penzai-0.1.0/penzai/toolshed/interleave_intermediates.py
--rw-r--r--   0        0        0    10295 2024-04-12 16:02:48.477126 penzai-0.1.0/penzai/toolshed/isolate_submodel.py
--rw-r--r--   0        0        0     2742 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/toolshed/jit_wrapper.py
--rw-r--r--   0        0        0     4741 2024-04-12 16:02:48.477126 penzai-0.1.0/penzai/toolshed/lora.py
--rw-r--r--   0        0        0    10539 2024-04-14 19:54:54.589795 penzai-0.1.0/penzai/toolshed/model_rewiring.py
--rw-r--r--   0        0        0     2464 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/toolshed/patch_ipdb.py
--rw-r--r--   0        0        0     9120 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/toolshed/sharding_util.py
--rw-r--r--   0        0        0     7271 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/toolshed/token_visualization.py
--rw-r--r--   0        0        0    18431 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/toolshed/unflaxify.py
--rw-r--r--   0        0        0     1522 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/__init__.py
--rw-r--r--   0        0        0      679 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/arrayviz/__init__.py
--rw-r--r--   0        0        0    16626 2024-04-14 19:53:54.821766 penzai-0.1.0/penzai/treescope/arrayviz/array_autovisualizer.py
--rw-r--r--   0        0        0    58879 2024-04-14 19:53:54.821766 penzai-0.1.0/penzai/treescope/arrayviz/arrayviz.py
--rw-r--r--   0        0        0    49417 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/arrayviz/js/arrayviz.js
--rw-r--r--   0        0        0     9447 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/autovisualize.py
--rw-r--r--   0        0        0    21160 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/canonical_aliases.py
--rw-r--r--   0        0        0     3480 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/copypaste_fallback.py
--rw-r--r--   0        0        0    11351 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/default_renderer.py
--rw-r--r--   0        0        0     8599 2024-04-14 19:54:54.589795 penzai-0.1.0/penzai/treescope/figures.py
--rw-r--r--   0        0        0      865 2024-04-12 16:02:48.481127 penzai-0.1.0/penzai/treescope/foldable_representation/__init__.py
--rw-r--r--   0        0        0    41960 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/basic_parts.py
--rw-r--r--   0        0        0    11969 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/common_structures.py
--rw-r--r--   0        0        0    15042 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/common_styles.py
--rw-r--r--   0        0        0     5552 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/embedded_iframe.py
--rw-r--r--   0        0        0    33377 2024-04-16 03:31:21.130952 penzai-0.1.0/penzai/treescope/foldable_representation/foldable_impl.py
--rw-r--r--   0        0        0    10622 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/layout_algorithms.py
--rw-r--r--   0        0        0    14390 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/foldable_representation/part_interface.py
--rw-r--r--   0        0        0     1036 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/__init__.py
--rw-r--r--   0        0        0     5056 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/builtin_atom_handler.py
--rw-r--r--   0        0        0    14612 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/builtin_structure_handler.py
--rw-r--r--   0        0        0     4410 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/canonical_alias_postprocessor.py
--rw-r--r--   0        0        0     4359 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/function_reflection_handlers.py
--rw-r--r--   0        0        0     2970 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/generic_pytree_handler.py
--rw-r--r--   0        0        0     4833 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/generic_repr_handler.py
--rw-r--r--   0        0        0     6123 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/hardcoded_structure_handlers.py
--rw-r--r--   0        0        0     6129 2024-04-14 19:53:54.821766 penzai-0.1.0/penzai/treescope/handlers/ndarray_handler.py
--rw-r--r--   0        0        0      797 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/penzai/__init__.py
--rw-r--r--   0        0        0     6557 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/penzai/data_effects_handlers.py
--rw-r--r--   0        0        0     8745 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/penzai/layer_handler.py
--rw-r--r--   0        0        0     5395 2024-04-14 19:53:54.821766 penzai-0.1.0/penzai/treescope/handlers/penzai/named_axes_handlers.py
--rw-r--r--   0        0        0     6114 2024-04-14 19:53:54.825766 penzai-0.1.0/penzai/treescope/handlers/penzai/shapecheck_handlers.py
--rw-r--r--   0        0        0     5391 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/penzai/struct_handler.py
--rw-r--r--   0        0        0     4247 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/repr_html_postprocessor.py
--rw-r--r--   0        0        0    11707 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/handlers/shared_value_postprocessor.py
--rw-r--r--   0        0        0     5629 2024-04-14 19:53:54.825766 penzai-0.1.0/penzai/treescope/html_compression.py
--rw-r--r--   0        0        0     1879 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/html_escaping.py
--rw-r--r--   0        0        0    19627 2024-04-14 19:53:54.825766 penzai-0.1.0/penzai/treescope/ndarray_summarization.py
--rw-r--r--   0        0        0    15701 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/renderer.py
--rw-r--r--   0        0        0    12009 2024-04-12 16:02:48.485127 penzai-0.1.0/penzai/treescope/selection_rendering.py
--rw-r--r--   0        0        0    13114 2024-04-14 19:54:54.589795 penzai-0.1.0/penzai/treescope/treescope_ipython.py
--rw-r--r--   0        0        0     2370 2024-04-18 03:04:49.759436 penzai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      816 2024-04-12 16:02:48.485127 penzai-0.1.0/run_tests.py
--rw-r--r--   0        0        0     4553 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/core_utils_test.py
--rw-r--r--   0        0        0    11683 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/data_effects/local_state_test.py
--rw-r--r--   0        0        0     3846 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/data_effects/random_test.py
--rw-r--r--   0        0        0     6422 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/data_effects/side_input_test.py
--rw-r--r--   0        0        0     3340 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/data_effects/side_output_test.py
--rw-r--r--   0        0        0     5863 2024-04-14 19:54:54.589795 penzai-0.1.0/tests/example_models/gemma_test.py
--rw-r--r--   0        0        0     2923 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/example_models/simple_mlp_test.py
--rw-r--r--   0        0        0      583 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/fixtures/treescope_examples_fixture.py
--rw-r--r--   0        0        0     2177 2024-04-12 16:02:48.485127 penzai-0.1.0/tests/misc_util_test.py
--rw-r--r--   0        0        0    29342 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/named_axes_test.py
--rw-r--r--   0        0        0     1056 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/basic_ops_test.py
--rw-r--r--   0        0        0     1293 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/embedding_test.py
--rw-r--r--   0        0        0     3403 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/grouping_test.py
--rw-r--r--   0        0        0     3659 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/linear_and_affine_test.py
--rw-r--r--   0        0        0    17014 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/parameters_test.py
--rw-r--r--   0        0        0     1301 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/nn/standardization_test.py
--rw-r--r--   0        0        0     4650 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/partitioning_test.py
--rw-r--r--   0        0        0    30388 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/selectors_test.py
--rw-r--r--   0        0        0    33708 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/shapecheck_test.py
--rw-r--r--   0        0        0    14580 2024-04-13 02:51:15.526660 penzai-0.1.0/tests/struct_pytree_dataclass_test.py
--rw-r--r--   0        0        0     4542 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/toolshed/isolate_submodel_test.py
--rw-r--r--   0        0        0     3625 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/toolshed/lora_test.py
--rw-r--r--   0        0        0     5168 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/toolshed/model_rewiring_test.py
--rw-r--r--   0        0        0    12009 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/toolshed/sharding_util_test.py
--rw-r--r--   0        0        0     4827 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/toolshed/unflaxify_test.py
--rw-r--r--   0        0        0    14189 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/treescope_canonical_aliases_test.py
--rw-r--r--   0        0        0    51923 2024-04-16 03:31:21.130952 penzai-0.1.0/tests/treescope_renderer_test.py
--rw-r--r--   0        0        0    44459 2024-04-12 16:02:48.489127 penzai-0.1.0/tests/treescope_representation_test.py
--rw-r--r--   0        0        0     6584 1970-01-01 00:00:00.000000 penzai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      731 2024-04-17 19:09:44.663782 penzai-0.1.1/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0      275 2024-04-18 15:17:01.802447 penzai-0.1.1/.gitignore
+-rw-r--r--   0        0        0    14782 2024-04-12 16:02:48.473126 penzai-0.1.1/.pylintrc
+-rw-r--r--   0        0        0      552 2024-04-18 15:17:01.802447 penzai-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       65 2024-04-12 16:02:48.473126 penzai-0.1.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      868 2024-04-12 16:02:48.473126 penzai-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      335 2024-04-12 16:02:48.473126 penzai-0.1.1/AUTHORS
+-rw-r--r--   0        0        0      970 2024-04-12 16:02:48.473126 penzai-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2024-04-12 16:02:48.473126 penzai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5370 2024-05-03 20:28:11.057814 penzai-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/.gitignore
+-rw-r--r--   0        0        0      644 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      621 2024-04-14 19:54:03.230332 penzai-0.1.1/docs/_autogen_root.rst
+-rw-r--r--   0        0        0     5101 2024-05-03 22:00:07.040879 penzai-0.1.1/docs/_include/_glue_figures.ipynb
+-rw-r--r--   0        0        0      805 2024-04-19 15:54:51.488782 penzai-0.1.1/docs/_static/custom.css
+-rw-r--r--   0        0        0     2635 2024-05-03 20:28:11.057814 penzai-0.1.1/docs/_static/custom.js
+-rw-r--r--   0        0        0   464137 2024-04-19 15:54:51.492783 penzai-0.1.1/docs/_static/readme_teaser.png
+-rw-r--r--   0        0        0      102 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/_templates/pzbase.rst
+-rw-r--r--   0        0        0     1889 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/_templates/pzclass.rst
+-rw-r--r--   0        0        0      106 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/_templates/pzdata.rst
+-rw-r--r--   0        0        0     1294 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/_templates/pzmodule.rst
+-rw-r--r--   0        0        0     1298 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/_templates/pzmodule_full.rst
+-rw-r--r--   0        0        0     1559 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/api/pz.de.rst
+-rw-r--r--   0        0        0     1968 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/api/pz.nn.rst
+-rw-r--r--   0        0        0     4241 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/api/pz.rst
+-rw-r--r--   0        0        0     1451 2024-04-12 16:02:48.477126 penzai-0.1.1/docs/api/pz.ts.rst
+-rw-r--r--   0        0        0     8256 2024-05-03 20:28:11.057814 penzai-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     2003 2024-04-16 03:31:21.126952 penzai-0.1.1/docs/ext/nb_output_cell_to_iframe.py
+-rw-r--r--   0        0        0     1370 2024-04-12 16:02:48.481127 penzai-0.1.1/docs/ext/pz_alias_rewrite.py
+-rw-r--r--   0        0        0     6263 2024-05-03 20:28:11.061814 penzai-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0     3063 2024-05-03 20:28:11.061814 penzai-0.1.1/docs/scripts/readthedocs_fetch_notebook_outputs.sh
+-rw-r--r--   0        0        0    71854 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/data_effects.ipynb
+-rw-r--r--   0        0        0   189024 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/gemma_from_scratch.ipynb
+-rw-r--r--   0        0        0    51069 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/how_to_think_in_penzai.ipynb
+-rw-r--r--   0        0        0   142008 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/induction_heads.ipynb
+-rw-r--r--   0        0        0   144103 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/induction_heads_2B.ipynb
+-rw-r--r--   0        0        0    47272 2024-05-03 22:00:07.044879 penzai-0.1.1/notebooks/jitting_and_sharding.ipynb
+-rw-r--r--   0        0        0    68268 2024-05-03 22:00:07.048879 penzai-0.1.1/notebooks/lora_from_scratch.ipynb
+-rw-r--r--   0        0        0    38620 2024-05-03 22:00:07.048879 penzai-0.1.1/notebooks/named_axes.ipynb
+-rw-r--r--   0        0        0    42727 2024-05-03 22:00:07.048879 penzai-0.1.1/notebooks/selectors.ipynb
+-rw-r--r--   0        0        0    35018 2024-05-03 22:00:07.048879 penzai-0.1.1/notebooks/treescope_arrayviz.ipynb
+-rw-r--r--   0        0        0    35468 2024-05-03 22:00:07.048879 penzai-0.1.1/notebooks/treescope_prettyprinting.ipynb
+-rw-r--r--   0        0        0      692 2024-05-03 21:49:35.549826 penzai-0.1.1/penzai/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/core/__init__.py
+-rw-r--r--   0        0        0     6804 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/core/context.py
+-rw-r--r--   0        0        0     3802 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/core/dataclass_util.py
+-rw-r--r--   0        0        0     2448 2024-04-16 03:31:21.126952 penzai-0.1.1/penzai/core/formatting_util.py
+-rw-r--r--   0        0        0     9414 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/core/layer.py
+-rw-r--r--   0        0        0    63948 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/core/named_axes.py
+-rw-r--r--   0        0        0     5305 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/core/partitioning.py
+-rw-r--r--   0        0        0     3782 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/core/random_stream.py
+-rw-r--r--   0        0        0    51446 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/core/selectors.py
+-rw-r--r--   0        0        0    43201 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/core/shapecheck.py
+-rw-r--r--   0        0        0    28518 2024-04-13 02:51:15.526660 penzai-0.1.1/penzai/core/struct.py
+-rw-r--r--   0        0        0     1117 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/core/syntactic_sugar.py
+-rw-r--r--   0        0        0     2384 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/core/tree_util.py
+-rw-r--r--   0        0        0      744 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/data_effects/__init__.py
+-rw-r--r--   0        0        0    20359 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/data_effects/effect_base.py
+-rw-r--r--   0        0        0    24485 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/data_effects/local_state.py
+-rw-r--r--   0        0        0    11914 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/data_effects/random.py
+-rw-r--r--   0        0        0    14547 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/data_effects/side_input.py
+-rw-r--r--   0        0        0     7259 2024-04-17 19:09:44.663782 penzai-0.1.1/penzai/data_effects/side_output.py
+-rw-r--r--   0        0        0      735 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/example_models/gemma/__init__.py
+-rw-r--r--   0        0        0    23796 2024-04-16 03:31:21.130952 penzai-0.1.1/penzai/example_models/gemma/model_core.py
+-rw-r--r--   0        0        0    11243 2024-05-03 20:28:11.061814 penzai-0.1.1/penzai/example_models/gemma/sampling_mode.py
+-rw-r--r--   0        0        0     9496 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/example_models/gemma/simple_decoding_loop.py
+-rw-r--r--   0        0        0     2574 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/example_models/simple_mlp.py
+-rw-r--r--   0        0        0      867 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/nn/__init__.py
+-rw-r--r--   0        0        0    11698 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/nn/attention.py
+-rw-r--r--   0        0        0     3276 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/nn/basic_ops.py
+-rw-r--r--   0        0        0     4017 2024-04-12 16:02:48.489127 penzai-0.1.1/penzai/nn/combinators.py
+-rw-r--r--   0        0        0     5272 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/nn/dropout.py
+-rw-r--r--   0        0        0    12857 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/nn/embeddings.py
+-rw-r--r--   0        0        0    11637 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/nn/grouping.py
+-rw-r--r--   0        0        0    27178 2024-04-16 03:31:21.130952 penzai-0.1.1/penzai/nn/linear_and_affine.py
+-rw-r--r--   0        0        0    23875 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/nn/parameters.py
+-rw-r--r--   0        0        0     6596 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/nn/standardization.py
+-rw-r--r--   0        0        0     1879 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/pz/__init__.py
+-rw-r--r--   0        0        0     1941 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/pz/de.py
+-rw-r--r--   0        0        0     2333 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/pz/nn.py
+-rw-r--r--   0        0        0     1811 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/pz/ts.py
+-rw-r--r--   0        0        0     5766 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/toolshed/annotate_shapes.py
+-rw-r--r--   0        0        0     3565 2024-05-03 20:28:11.065814 penzai-0.1.1/penzai/toolshed/auto_nmap.py
+-rw-r--r--   0        0        0    13543 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/toolshed/basic_training.py
+-rw-r--r--   0        0        0     5362 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/toolshed/check_layers_by_tracing.py
+-rw-r--r--   0        0        0     6445 2024-04-12 16:02:48.493127 penzai-0.1.1/penzai/toolshed/interleave_intermediates.py
+-rw-r--r--   0        0        0    10295 2024-04-12 16:02:48.477126 penzai-0.1.1/penzai/toolshed/isolate_submodel.py
+-rw-r--r--   0        0        0     2742 2024-04-16 03:31:21.130952 penzai-0.1.1/penzai/toolshed/jit_wrapper.py
+-rw-r--r--   0        0        0     4741 2024-04-12 16:02:48.477126 penzai-0.1.1/penzai/toolshed/lora.py
+-rw-r--r--   0        0        0    10539 2024-04-14 19:54:54.589795 penzai-0.1.1/penzai/toolshed/model_rewiring.py
+-rw-r--r--   0        0        0     2464 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/toolshed/patch_ipdb.py
+-rw-r--r--   0        0        0     9120 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/toolshed/sharding_util.py
+-rw-r--r--   0        0        0     7271 2024-04-16 03:31:21.130952 penzai-0.1.1/penzai/toolshed/token_visualization.py
+-rw-r--r--   0        0        0    18431 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/toolshed/unflaxify.py
+-rw-r--r--   0        0        0     1522 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/arrayviz/__init__.py
+-rw-r--r--   0        0        0    16626 2024-04-14 19:53:54.821766 penzai-0.1.1/penzai/treescope/arrayviz/array_autovisualizer.py
+-rw-r--r--   0        0        0    58851 2024-05-03 20:28:11.065814 penzai-0.1.1/penzai/treescope/arrayviz/arrayviz.py
+-rw-r--r--   0        0        0    50163 2024-05-03 20:28:11.065814 penzai-0.1.1/penzai/treescope/arrayviz/js/arrayviz.js
+-rw-r--r--   0        0        0     9447 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/autovisualize.py
+-rw-r--r--   0        0        0    21160 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/canonical_aliases.py
+-rw-r--r--   0        0        0     3480 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/copypaste_fallback.py
+-rw-r--r--   0        0        0    11351 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/default_renderer.py
+-rw-r--r--   0        0        0     8599 2024-04-14 19:54:54.589795 penzai-0.1.1/penzai/treescope/figures.py
+-rw-r--r--   0        0        0      865 2024-04-12 16:02:48.481127 penzai-0.1.1/penzai/treescope/foldable_representation/__init__.py
+-rw-r--r--   0        0        0    41960 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/basic_parts.py
+-rw-r--r--   0        0        0    11969 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/common_structures.py
+-rw-r--r--   0        0        0    15042 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/common_styles.py
+-rw-r--r--   0        0        0     5552 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/embedded_iframe.py
+-rw-r--r--   0        0        0    35475 2024-05-03 20:28:11.065814 penzai-0.1.1/penzai/treescope/foldable_representation/foldable_impl.py
+-rw-r--r--   0        0        0    10622 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/layout_algorithms.py
+-rw-r--r--   0        0        0    14390 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/foldable_representation/part_interface.py
+-rw-r--r--   0        0        0     1036 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/__init__.py
+-rw-r--r--   0        0        0     5056 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/builtin_atom_handler.py
+-rw-r--r--   0        0        0    14612 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/builtin_structure_handler.py
+-rw-r--r--   0        0        0     4410 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/canonical_alias_postprocessor.py
+-rw-r--r--   0        0        0     4359 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/function_reflection_handlers.py
+-rw-r--r--   0        0        0     2970 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/generic_pytree_handler.py
+-rw-r--r--   0        0        0     4833 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/generic_repr_handler.py
+-rw-r--r--   0        0        0     6123 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/hardcoded_structure_handlers.py
+-rw-r--r--   0        0        0     6129 2024-04-14 19:53:54.821766 penzai-0.1.1/penzai/treescope/handlers/ndarray_handler.py
+-rw-r--r--   0        0        0      797 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/penzai/__init__.py
+-rw-r--r--   0        0        0     6557 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/penzai/data_effects_handlers.py
+-rw-r--r--   0        0        0     8745 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/penzai/layer_handler.py
+-rw-r--r--   0        0        0     5395 2024-04-14 19:53:54.821766 penzai-0.1.1/penzai/treescope/handlers/penzai/named_axes_handlers.py
+-rw-r--r--   0        0        0     6114 2024-04-14 19:53:54.825766 penzai-0.1.1/penzai/treescope/handlers/penzai/shapecheck_handlers.py
+-rw-r--r--   0        0        0     5391 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/penzai/struct_handler.py
+-rw-r--r--   0        0        0     4247 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/repr_html_postprocessor.py
+-rw-r--r--   0        0        0    11707 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/handlers/shared_value_postprocessor.py
+-rw-r--r--   0        0        0     5629 2024-04-14 19:53:54.825766 penzai-0.1.1/penzai/treescope/html_compression.py
+-rw-r--r--   0        0        0     1879 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/html_escaping.py
+-rw-r--r--   0        0        0    19627 2024-04-14 19:53:54.825766 penzai-0.1.1/penzai/treescope/ndarray_summarization.py
+-rw-r--r--   0        0        0    15701 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/renderer.py
+-rw-r--r--   0        0        0    12009 2024-04-12 16:02:48.485127 penzai-0.1.1/penzai/treescope/selection_rendering.py
+-rw-r--r--   0        0        0    13407 2024-05-03 20:28:11.065814 penzai-0.1.1/penzai/treescope/treescope_ipython.py
+-rw-r--r--   0        0        0     2394 2024-05-03 20:28:11.065814 penzai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      816 2024-04-12 16:02:48.485127 penzai-0.1.1/run_tests.py
+-rw-r--r--   0        0        0     4553 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/core_utils_test.py
+-rw-r--r--   0        0        0    11683 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/data_effects/local_state_test.py
+-rw-r--r--   0        0        0     3846 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/data_effects/random_test.py
+-rw-r--r--   0        0        0     6422 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/data_effects/side_input_test.py
+-rw-r--r--   0        0        0     3340 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/data_effects/side_output_test.py
+-rw-r--r--   0        0        0     5863 2024-04-14 19:54:54.589795 penzai-0.1.1/tests/example_models/gemma_test.py
+-rw-r--r--   0        0        0     2923 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/example_models/simple_mlp_test.py
+-rw-r--r--   0        0        0      583 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/fixtures/treescope_examples_fixture.py
+-rw-r--r--   0        0        0     2177 2024-04-12 16:02:48.485127 penzai-0.1.1/tests/misc_util_test.py
+-rw-r--r--   0        0        0    29797 2024-05-03 20:28:11.065814 penzai-0.1.1/tests/named_axes_test.py
+-rw-r--r--   0        0        0     1056 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/basic_ops_test.py
+-rw-r--r--   0        0        0     1293 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/embedding_test.py
+-rw-r--r--   0        0        0     3403 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/grouping_test.py
+-rw-r--r--   0        0        0     3659 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/linear_and_affine_test.py
+-rw-r--r--   0        0        0    17014 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/parameters_test.py
+-rw-r--r--   0        0        0     1301 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/nn/standardization_test.py
+-rw-r--r--   0        0        0     4650 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/partitioning_test.py
+-rw-r--r--   0        0        0    30388 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/selectors_test.py
+-rw-r--r--   0        0        0    33708 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/shapecheck_test.py
+-rw-r--r--   0        0        0    14580 2024-04-13 02:51:15.526660 penzai-0.1.1/tests/struct_pytree_dataclass_test.py
+-rw-r--r--   0        0        0     2255 2024-05-03 20:28:11.065814 penzai-0.1.1/tests/toolshed/auto_nmap_test.py
+-rw-r--r--   0        0        0     4542 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/toolshed/isolate_submodel_test.py
+-rw-r--r--   0        0        0     3625 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/toolshed/lora_test.py
+-rw-r--r--   0        0        0     5168 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/toolshed/model_rewiring_test.py
+-rw-r--r--   0        0        0    12009 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/toolshed/sharding_util_test.py
+-rw-r--r--   0        0        0     4827 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/toolshed/unflaxify_test.py
+-rw-r--r--   0        0        0    14189 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/treescope_canonical_aliases_test.py
+-rw-r--r--   0        0        0    51923 2024-04-16 03:31:21.130952 penzai-0.1.1/tests/treescope_renderer_test.py
+-rw-r--r--   0        0        0    44459 2024-04-12 16:02:48.489127 penzai-0.1.1/tests/treescope_representation_test.py
+-rw-r--r--   0        0        0     7468 1970-01-01 00:00:00.000000 penzai-0.1.1/PKG-INFO
```

### Comparing `penzai-0.1.0/.github/workflows/unittests.yml` & `penzai-0.1.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/.pylintrc` & `penzai-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/.readthedocs.yaml` & `penzai-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/.vscode/settings.json` & `penzai-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/CONTRIBUTING.md` & `penzai-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/LICENSE` & `penzai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/README.md` & `penzai-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 structures, along with tools for visualizing, modifying, and analyzing them.
 Penzai focuses on **making it easy to do stuff with models after they have been
 trained**, making it a great choice for research involving reverse-engineering
 or ablating model components, inspecting and probing internal activations,
 performing model surgery, debugging architectures, and more. (But if you just
 want to build and train a model, you can do that too!)
 
+With Penzai, your neural networks could look like this:
+
+![Screenshot of the Gemma model in Penzai](docs/_static/readme_teaser.png)
+
 Penzai is structured as a collection of modular tools, designed together but
 each useable independently:
 
 * `penzai.nn` (`pz.nn`): A declarative combinator-based neural network
   library and an alternative to other neural network libraries like Flax, Haiku,
   Keras, or Equinox, which exposes the full structure of your model's
   forward pass in the model pytree. This means you can see everything your model
@@ -42,67 +46,80 @@
 * `penzai.data_effects` (`pz.de`): An opt-in system for side arguments, random
   numbers, and state variables that is built on pytree traversal and puts you
   in control, without getting in the way of writing or using your model.
 
 Documentation on Penzai can be found at
 [https://penzai.readthedocs.io](https://penzai.readthedocs.io).
 
+> [!WARNING]
+> Penzai's API is currently unstable and may change in future releases.
+>
+> In particular, the way Penzai handles parameter initialization, parameter
+> sharing, and local mutable state in `penzai.nn` and
+> `penzai.data_effects` is likely to be simplified in the future.
+> Some internal details of the `treescope` pretty-printer intermediate
+> representation may also change to make it easier to extend and configure.
+>
+> Projects that use Penzai's neural network components or model implementations,
+> or that define their own handlers for `treescope`, are encouraged to pin the
+> `0.1.x` release series (e.g. `penzai>=0.1,<0.2`) to avoid breaking changes.
+
 
 ## Getting Started
 
 If you haven't already installed JAX, you should do that first, since the
 installation process depends on your platform. You can find instructions in the
 [JAX documentation](https://jax.readthedocs.io/en/latest/installation.html).
 Afterward, you can install Penzai using
 
-```
+```python
 pip install penzai
 ```
 
 and import it using
 
-```
+```python
 import penzai
 from penzai import pz
 ```
 
 (`penzai.pz` is an *alias namespace*, which makes it easier to reference
 common Penzai objects.)
 
 When working in an Colab or IPython notebook, we recommend also configuring
 Penzai as the default pretty printer, and enabling some utilities for
 interactive use:
 
-```
+```python
 pz.ts.register_as_default()
 pz.ts.register_autovisualize_magic()
 pz.enable_interactive_context()
 
 # Optional: enables automatic array visualization
 pz.ts.active_autovisualizer.set_interactive(pz.ts.ArrayAutovisualizer())
 ```
 
 Here's how you could initialize and visualize a simple neural network:
 
-```
+```python
 from penzai.example_models import simple_mlp
 mlp = pz.nn.initialize_parameters(
     simple_mlp.MLP.from_config([8, 32, 32, 8]),
     jax.random.key(42),
 )
 
 # Models and arrays are visualized automatically when you output them from a
 # Colab/IPython notebook cell:
 mlp
 ```
 
 Here's how you could capture and extract the activations after the elementwise
 nonlinearities:
 
-```
+```python
 mlp_with_captured_activations = pz.de.CollectingSideOutputs.handling(
     pz.select(mlp)
     .at_instances_of(pz.nn.Elementwise)
     .insert_after(pz.de.TellIntermediate())
 )
 
 output, intermediates = mlp_with_captured_activations(
```

### Comparing `penzai-0.1.0/docs/Makefile` & `penzai-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/_autogen_root.rst` & `penzai-0.1.1/docs/_autogen_root.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/_include/_glue_figures.ipynb` & `penzai-0.1.1/docs/_include/_glue_figures.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/_static/custom.js` & `penzai-0.1.1/docs/_static/custom.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -23,30 +23,33 @@
         frame.classList.add('cell_output_frame');
         frame.sandbox = [
             'allow-downloads', 'allow-forms', 'allow-pointer-lock', 'allow-popups',
             'allow-same-origin', 'allow-scripts',
             'allow-storage-access-by-user-activation',
             'allow-popups-to-escape-sandbox'
         ].join(' ');
-        frameTpl.parentNode.replaceChild(frame, frameTpl);
-        frame.contentDocument.body.appendChild(frameTpl.content.cloneNode(true));
-        frame.contentDocument.body.style.height = 'fit-content';
-        frame.contentDocument.body.style.margin = '0';
-        frame.contentDocument.body.style.padding = '0.5em 1ch 0.5em 1ch';
-        const observer = new ResizeObserver(() => {
-            const frameBounds = frame.getBoundingClientRect();
-            const bounds = frame.contentDocument.body.getBoundingClientRect();
-            if (frame.contentDocument.body.scrollWidth > frameBounds.width) {
-                // Make room for the scrollbar.
-                frame.style.height = `calc(1em + ${bounds.height}px)`;
-            } else {
-                frame.style.height = `${bounds.height}px`;
-            }
+        frame.addEventListener("load", () => {
+            frame.contentDocument.body.appendChild(frameTpl.content.cloneNode(true));
+            frame.contentDocument.body.style.height = 'fit-content';
+            frame.contentDocument.body.style.margin = '0';
+            frame.contentDocument.body.style.padding = '0.5em 1ch 0.5em 1ch';
+            const observer = new ResizeObserver(() => {
+                const frameBounds = frame.getBoundingClientRect();
+                const bounds = frame.contentDocument.body.getBoundingClientRect();
+                if (frame.contentDocument.body.scrollWidth > frameBounds.width) {
+                    // Make room for the scrollbar.
+                    frame.style.height = `calc(1em + ${bounds.height}px)`;
+                } else {
+                    frame.style.height = `${bounds.height}px`;
+                }
+            });
+            observer.observe(frame.contentDocument.body);
         });
-        observer.observe(frame.contentDocument.body);
+        frame.src = "about:blank";
+        frameTpl.parentNode.replaceChild(frame, frameTpl);
     }
 
     // Add zero-width spaces to sidebar identifiers to improve word breaking.
     const sidebarNodes = document.querySelectorAll(
         '.bd-docs-nav .reference, .bd-docs-nav .reference *');
     for (let parent of sidebarNodes) {
         for (let elt of parent.childNodes) {
```

### Comparing `penzai-0.1.0/docs/_templates/pzclass.rst` & `penzai-0.1.1/docs/_templates/pzclass.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/_templates/pzmodule.rst` & `penzai-0.1.1/docs/_templates/pzmodule.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/_templates/pzmodule_full.rst` & `penzai-0.1.1/docs/_templates/pzmodule_full.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/api/pz.de.rst` & `penzai-0.1.1/docs/api/pz.de.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/api/pz.nn.rst` & `penzai-0.1.1/docs/api/pz.nn.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/api/pz.rst` & `penzai-0.1.1/docs/api/pz.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/api/pz.ts.rst` & `penzai-0.1.1/docs/api/pz.ts.rst`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/conf.py` & `penzai-0.1.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 # pylint: disable=g-bad-import-order
 # pylint: disable=g-import-not-at-top
 import inspect
 import logging
 import os
+import subprocess
 import sys
 import typing
 
 import penzai.core
 import penzai.data_effects
 import penzai.nn
 import penzai.treescope
@@ -75,14 +76,21 @@
       return True
 
 
 sphinx_logging.getLogger('sphinx.highlighting').logger.addFilter(
     IgnoreBangWarningFilter()
 )
 
+try:
+  # Look up the current git hash so we can link to it.
+  git_hash_bytes = subprocess.check_output(['git', 'rev-parse', 'HEAD'])
+  source_git_hash = git_hash_bytes.decode().strip()
+except Exception:  # pylint: disable=broad-exception-caught
+  source_git_hash = None
+
 # -- Project information -----------------------------------------------------
 
 project = 'Penzai'
 copyright = '2024, The Penzai Authors'  # pylint: disable=redefined-builtin
 author = 'the Penzai Authors'
 
 # -- General configuration ---------------------------------------------------
@@ -102,14 +110,15 @@
     'sphinx.ext.napoleon',
     'sphinxcontrib.katex',
     'myst_nb',
     'sphinxcontrib.collections',
     'sphinx_contributors',
     'pz_alias_rewrite',
     'nb_output_cell_to_iframe',
+    'hoverxref.extension',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -196,14 +205,24 @@
 # Translate LaTeX macros to KaTeX and add to options for HTML builder
 katex_macros = katex.latex_defs_to_katex_macros(latex_macros)
 katex_options = 'macros: {' + katex_macros + '}'
 
 # Add LaTeX macros for LATEX builder
 latex_elements = {'preamble': latex_macros}
 
+# -- Hover cross-references ----------------------------------------------------
+
+hoverxref_domains = [
+    'py',
+]
+hoverxref_role_types = {
+    'obj': 'tooltip',
+    'class': 'tooltip',
+}
+
 # -- Source code links -------------------------------------------------------
 
 
 def linkcode_resolve(domain, info):
   """Resolve a GitHub URL corresponding to Python object."""
   if domain != 'py':
     return None
@@ -228,18 +247,22 @@
     return None
 
   try:
     source, lineno = inspect.getsourcelines(obj)
   except OSError:
     return None
 
-  return 'https://github.com/deepmind/penzai/tree/master/penzai/%s#L%d#L%d' % (
-      os.path.relpath(filename, start=os.path.dirname(penzai.__file__)),
-      lineno,
-      lineno + len(source) - 1,
+  if source_git_hash is not None:
+    git_identifier = source_git_hash
+  else:
+    git_identifier = 'main'
+  relpath = os.path.relpath(filename, start=os.path.dirname(penzai.__file__))
+  return (
+      f'https://github.com/google-deepmind/penzai/blob/{git_identifier}/penzai/'
+      f'{relpath}#L{lineno}#L{lineno + len(source) - 1}'
   )
 
 
 # -- Intersphinx configuration -----------------------------------------------
 
 intersphinx_mapping = {
     'jax': ('https://jax.readthedocs.io/en/latest/', None),
```

### Comparing `penzai-0.1.0/docs/ext/nb_output_cell_to_iframe.py` & `penzai-0.1.1/docs/ext/nb_output_cell_to_iframe.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/ext/pz_alias_rewrite.py` & `penzai-0.1.1/docs/ext/pz_alias_rewrite.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/docs/index.rst` & `penzai-0.1.1/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,28 @@
 * `penzai.data_effects` (``pz.de``): An opt-in system for side arguments, random
   numbers, and state variables that is built on pytree traversal and puts you
   in control, without getting in the way of writing or using your model.
 
 These components are described in more detail in the guides in the left
 sidebar.
 
+.. warning::
+   Penzai's API is currently unstable and may change in future releases.
+
+   In particular, the way Penzai handles parameter initialization, parameter
+   sharing, and local mutable state in `penzai.nn` and
+   `penzai.data_effects` is likely to be simplified in the future.
+   Some internal details of the `penzai.treescope` pretty-printer intermediate
+   representation may also change to make it easier to extend and configure.
+
+   Projects that use Penzai's neural network components or model
+   implementations, or that define their own handlers for ``treescope``, are
+   encouraged to pin the ``0.1.x`` release series (e.g. ``penzai>=0.1,<0.2``)
+   to avoid breaking changes.
+
 Getting Started
 ---------------
 
 If you haven't already installed JAX, you should do that first, since the
 installation process depends on your platform. You can find instructions in the
 `JAX documentation <https://jax.readthedocs.io/en/latest/installation.html>`_.
 Afterward, you can install Penzai using
@@ -107,15 +121,15 @@
   # Colab/IPython notebook cell:
   mlp
 
 To learn more about how to build and manipulate neural networks with Penzai,
 we recommend starting with the
 :doc:`"How to Think in Penzai" <notebooks/how_to_think_in_penzai>`
 notebook, which gives a high-level overview of how to think about and use Penzai
-models. Afterward, you coould:
+models. Afterward, you could:
 
 * Take a look at one of the example notebooks to see how you can use Penzai to
   visualize and modify pretrained models.
 * Or, read through the guides in the left sidebar to learn more about each of
   Penzai's components.
```

### Comparing `penzai-0.1.0/docs/scripts/readthedocs_fetch_notebook_outputs.sh` & `penzai-0.1.1/docs/scripts/readthedocs_fetch_notebook_outputs.sh`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 set -e
 set -x
 
 # Figure out where we are, likely a branch or tag.
 # - When building a tag, this will produce something like "tags/tagname^0"
 # - When building a branch, it will be like "remotes/origin/branchname"
-curref=$(git name-rev --name-only --no-undefined HEAD || true)
+curref=$(git name-rev --name-only --no-undefined --exclude='main' --exclude='HEAD' HEAD || true)
 
 if [[ "${curref}" =~ ^tags/(.*)"^0"$ ]]; then
   # Looks like a tag.
   tagname="${BASH_REMATCH[1]}"
   notebook_ref=${tagname}+notebook_outputs
   missing_message="ERROR: Missing notebook outputs ref ${notebook_ref} for tag ${tagname}"
   required="true"
```

### Comparing `penzai-0.1.0/notebooks/data_effects.ipynb` & `penzai-0.1.1/notebooks/data_effects.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999821937321938%*

 * *Differences: {"'cells'": "{47: {'source': {insert: [(8, 'This means the wrapper object looks just like an "*

 * *            'ordinary Penzai model to JAX, since it has a normal PyTree structure, and produces a '*

 * *            "pure functional output without accessing global state.\\n')], delete: [8]}}}"}*

```diff
@@ -660,15 +660,15 @@
                 "- We can identify where a side effect should happen by inserting some node into the model tree with a special type (`ReplaceMeWithAnAppendFunction`).\n",
                 "- We can then wrap the model tree in a wrapper object (`CaptureIntermediatesWhereRequested`) that handles the effect by\n",
                 "  - creating its own temporary local mutable Python variables,\n",
                 "  - substituting them into the model,\n",
                 "  - running the model,\n",
                 "  - and then putting together a pure result.\n",
                 "\n",
-                "This means the wrapper object looks just like an ordinary Penzai model to JAX, since it has a normal PyTree strucure, and produces a pure functional output without accessing global state.\n",
+                "This means the wrapper object looks just like an ordinary Penzai model to JAX, since it has a normal PyTree structure, and produces a pure functional output without accessing global state.\n",
                 "\n",
                 "Next, we'll describe the full data effects system, which abstracts this approach into a more general pattern, and imposes a few more rules to make it easier to understand in the presence of multiple effects."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
```

### Comparing `penzai-0.1.0/notebooks/gemma_from_scratch.ipynb` & `penzai-0.1.1/notebooks/gemma_from_scratch.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999942121590961%*

 * *Differences: {"'cells'": "{74: {'source': {insert: [(0, 'This approach makes Flax a great choice for quickly "*

 * *            'writing neural networks in JAX, especially if you are already familiar with stateful '*

 * *            "neural network libraries and object-oriented programming.\\n')], delete: [0]}}}"}*

```diff
@@ -919,15 +919,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "CGxxn3-VvdOr"
             },
             "source": [
-                "This approach makes Flax a great choice for quickly writing neural networks in JAX, expecially if you are already familiar with stateful neural network libraries and object-oriented programming.\n",
+                "This approach makes Flax a great choice for quickly writing neural networks in JAX, especially if you are already familiar with stateful neural network libraries and object-oriented programming.\n",
                 "\n",
                 "However, since this representation was designed for *writing* model architectures, it's not necessarily the best choice for *analyzing* or *patching* those models. Indeed, any such analysis must be designed to work around the transformation from stateful object-oriented modules to functional JAX-compatible method calls.\n",
                 "\n",
                 "Penzai, on the other hand, prioritizes **analysis**, **visualization**, and **patchability**. One of the primary design goals for Penzai's neural net library `penzai.nn` is to be a *declarative* system where \"*what you see is what you get*\": you should be able to immediately see what your model is going to do when you call it, and you should be able to \"reach in\" and change what it does. This leads to a number of concrete differences:\n",
                 "\n",
                 "- Parameters:\n",
                 "  - In Flax, you define parameters by calling `self.param`, and you can define other mutable variables using `self.variable`. This variable is implicitly inserted into a parameter dictionary and retrieved when a module is functionalized.\n",
```

### Comparing `penzai-0.1.0/notebooks/how_to_think_in_penzai.ipynb` & `penzai-0.1.1/notebooks/how_to_think_in_penzai.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/induction_heads.ipynb` & `penzai-0.1.1/notebooks/induction_heads.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/induction_heads_2B.ipynb` & `penzai-0.1.1/notebooks/induction_heads_2B.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/jitting_and_sharding.ipynb` & `penzai-0.1.1/notebooks/jitting_and_sharding.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/lora_from_scratch.ipynb` & `penzai-0.1.1/notebooks/lora_from_scratch.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/named_axes.ipynb` & `penzai-0.1.1/notebooks/named_axes.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/selectors.ipynb` & `penzai-0.1.1/notebooks/selectors.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/treescope_arrayviz.ipynb` & `penzai-0.1.1/notebooks/treescope_arrayviz.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/notebooks/treescope_prettyprinting.ipynb` & `penzai-0.1.1/notebooks/treescope_prettyprinting.ipynb`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/__init__.py` & `penzai-0.1.1/penzai/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A JAX research toolkit for building, editing, and visualizing neural networks."""
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

### Comparing `penzai-0.1.0/penzai/core/__init__.py` & `penzai-0.1.1/penzai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/context.py` & `penzai-0.1.1/penzai/core/context.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/dataclass_util.py` & `penzai-0.1.1/penzai/core/dataclass_util.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/formatting_util.py` & `penzai-0.1.1/penzai/core/formatting_util.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/layer.py` & `penzai-0.1.1/penzai/core/layer.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/named_axes.py` & `penzai-0.1.1/penzai/core/named_axes.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A lightweight and minimal implementation of named axes.
 
 As argued by "Tensors Considered Harmful", relying on axis indices for complex
-tensor operations can be brittile and difficult to read. This has led to a
+tensor operations can be brittle and difficult to read. This has led to a
 number of proposals for indexing axes by name instead of by position. However,
 due to the large API surface for NDArray manipulation, building a fully-featured
 named axis implementation requires making named-axis versions of many individual
 operations.
 
 This module provides a lightweight implementation of named axes using a
 "locally positional" style. The key idea is to reuse positional-axis operations
@@ -763,15 +763,15 @@
     If they do have positional axes, those positional axes can be indexed into
     using ordinary Numpy-style indexing. Indexing operations will be
     automatically vectorized over all of the named axes. For instance, an
     embedding lookup could look something like::
 
       embedding_table.untag("vocab")[token_ids]
 
-    which first untagss the "vocab" named axis as positional, then indexes into
+    which first untags the "vocab" named axis as positional, then indexes into
     that axis using another array (which can be a `NamedArray` or an ordinary
     array).
 
     If they do NOT have positional axes, the named axes can be sliced directly
     using dictionaries mapping names to indices or slices, e.g.::
 
       my_array[{"position": 1, "feature": pz.slice[2:5]}]
@@ -863,25 +863,37 @@
           index_thunks.append(_DynamicThunk(c))
         elif isinstance(c, slice):
           index_thunks.append(_SliceThunk(c.start, c.stop, c.step))
         else:
           index_thunks.append(_StaticThunk(c))
       return _jitted_nmapped_getitem(self, tuple(index_thunks))
 
-  # Array conversion operator
+  # Array conversion operators
   def __array__(self, *args, **kwargs):
+    """Converts a named array with no named axes to a Numpy array."""
     if self.named_shape:
       raise ValueError(
           "Only NamedArray(View)s with no named axes can be converted to numpy"
           " arrays. Use `unwrap` or `untag` to assign positions to named axes"
           " first, or use `penzai.named_axes.nmap` with a JAX function instead."
       )
     else:
       return np.array(self.unwrap(), *args, **kwargs)
 
+  def __jax_array__(self):
+    """Converts a named array with no named axes to a JAX array."""
+    if self.named_shape:
+      raise ValueError(
+          "Only NamedArray(View)s with no named axes can be converted to JAX"
+          " arrays. Use `unwrap` or `untag` to assign positions to named axes"
+          " first, or use `penzai.named_axes.nmap` with a JAX function instead."
+      )
+    else:
+      return self.unwrap()
+
   # Iteration. Note that we *must* implement this to avoid Python simply trying
   # to run __getitem__ until it raises IndexError, because we won't raise
   # IndexError (since JAX clips array indices).
   def __iter__(self):
     if not self.positional_shape:
       raise ValueError("Cannot iterate over an array with no positional axes!")
     for i in range(self.positional_shape[0]):
@@ -1083,15 +1095,15 @@
       *names: Optional names for the axes of the array. If provided, must be the
         same length as the array's shape. This is a convenience wrapper so that
         you can call ``wrap(array, "foo", "bar")`` instead of
         ``wrap(array).tag("foo", "bar")``.
 
     Returns:
       An equivalent ``NamedArray`` for the given array. If ``names`` is
-      provided, the resuling array will have those names assigned to the
+      provided, the resulting array will have those names assigned to the
       corresponding axes. Otherwise, the resulting array will have a positional
       shape.
     """
     wrapped = NamedArray(
         named_axes=collections.OrderedDict(), data_array=jnp.asarray(array)
     )
     if names:
@@ -1520,15 +1532,15 @@
   """Convenience function to create a range along a named axis.
 
   This is shorthand for ``wrap(jnp.arange(...)).tag(name)``.
 
   Args:
     name: Name for the resulting axis.
     start: Start of the range. If ``stop`` is not provided, this is instead
-      interpreted as ``stop``, with ``start`` implicity set to 0, following
+      interpreted as ``stop``, with ``start`` implicitly set to 0, following
       `jnp.arange`.
     stop: End of the range.
     step: Step size (defaults to 1).
     dtype: Optional dtype for the result.
 
   Returns:
     `NamedArray` with a single named axis containing a range of integers.
```

### Comparing `penzai-0.1.0/penzai/core/partitioning.py` & `penzai-0.1.1/penzai/core/partitioning.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/random_stream.py` & `penzai-0.1.1/penzai/core/random_stream.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/selectors.py` & `penzai-0.1.1/penzai/core/selectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,15 +833,15 @@
       .at_subtrees_where(lambda subtree: template == subtree)
 
     but also skips `jax.Array`, `np.ndarray`, and
     `penzai.core.named_axes.NamedArray`, since they override ``==`` to return
     arrays.
 
     Args:
-      template: The object to select occurences of.
+      template: The object to select occurrences of.
 
     Returns:
       A refined selection that selects instances of this class that compare
       equal to this object (with other on the left).
     """
     # Lazy import to avoid circular dependencies
     import penzai.core.named_axes  # pylint: disable=g-import-not-at-top
@@ -1352,15 +1352,15 @@
     tree_with_boundary: A PyTree, with `_InProgressSelectionBoundary` nodes
       wrapping the subtrees that we wish to select. An unchecked requirement is
       that no `_InProgressSelectionBoundary` node should contain another
       `_InProgressSelectionBoundary` node; if this happens the boundary nodes
       will leak back into the returned selection.
 
   Returns:
-    A selection, such that each occurence of `_InProgressSelectionBoundary` is
+    A selection, such that each occurrence of `_InProgressSelectionBoundary` is
     transformed into a selected subtree.
   """
   selected_by_path = collections.OrderedDict()
 
   def process_selected(keypath, leaf):
     """Process PyTree leaves or subtrees where _is_hole_or_quote is True."""
     if isinstance(leaf, _InProgressSelectionBoundary):
```

### Comparing `penzai-0.1.0/penzai/core/shapecheck.py` & `penzai-0.1.1/penzai/core/shapecheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
               f"\n  {constraint.value} =="
               f" {_summarize_pattern(constraint.pattern)} from"
               f" root{jax.tree_util.keystr(keypath)}"
               for (keypath, constraint) in unsolved_variable_constraints
           )
       )
 
-  # No more constraints, which means this was a sucessful match. We need to
+  # No more constraints, which means this was a successful match. We need to
   # re-associate any variables whose values were tuples.
   final_matches = {}
   match_errors = []
   for name, binding in solutions.items():
     if isinstance(name, tuple):
       if name[0] in solutions:
         # Redundant! We already have this in our solution.
@@ -1061,15 +1061,15 @@
 
   DimensionVariableSubstitution can be used to inspect and modify the dimension
   variables appearing in an unknown structure. It is intended to be used as
   part of transformations that inspect the input or output structures of layers.
 
   The substitutions are allowed to contain other dimension variables. For
   instance, you can set `mapping_variables["foo"] = {"bar":1, **var("baz")}` to
-  map the original unpacked mapping varialbe "foo" to the new composite mapping.
+  map the original unpacked mapping variable "foo" to the new composite mapping.
   This can be used to e.g. rename variables.
 
   Attributes:
     size_variables: A map from dimension variable names to their sizes.
     sequence_variables: A map from sequence variable names to their sequence of
       sizes.
     mapping_variables: A map from mapping variable names to their mappings from
```

### Comparing `penzai-0.1.0/penzai/core/struct.py` & `penzai-0.1.1/penzai/core/struct.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/syntactic_sugar.py` & `penzai-0.1.1/penzai/core/syntactic_sugar.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/core/tree_util.py` & `penzai-0.1.1/penzai/core/tree_util.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/data_effects/__init__.py` & `penzai-0.1.1/penzai/data_effects/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/data_effects/effect_base.py` & `penzai-0.1.1/penzai/data_effects/effect_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
 
 
 class EffectRuntimeImpl(abc.ABC):
   """Base class for runtime effect implementations.
 
   Subclasses of ``EffectRuntimeImpl`` are created by effect handlers and are
   inserted into any layer that needs access to the effect while the model is
-  actually being called at runtime. They are reponsible for providing the
+  actually being called at runtime. They are responsible for providing the
   implementation of the effect protocol according to the handler's
   configuration.
 
   ``EffectRuntimeImpl`` should not usually be kept around outside of the
   handler's ``__call__`` method, as they may contain mutable state that is
   incompatible with JAX. In some cases they can be used temporarily outside of
   their handler, but models containing ``EffectRuntimeImpl`` should never be the
```

### Comparing `penzai-0.1.0/penzai/data_effects/local_state.py` & `penzai-0.1.1/penzai/data_effects/local_state.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/data_effects/random.py` & `penzai-0.1.1/penzai/data_effects/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 @struct.pytree_dataclass
 class WithFrozenRandomState(effect_base.EffectHandler):
   """`RandomEffect` handler that uses a fixed random state.
 
   ``WithFrozenRandomState`` can be used to freeze the random state of a model
   at a given point in time, allowing it to be deterministic and reproducible.
   It is most useful for debugging the behavior of a stochastic model while
-  holding the random seed constent.
+  holding the random seed constant.
 
   Attributes:
     handler_id: The ID of this handler.
     body: The layer that this handler wraps.
     random_key: The constant random key to use.
     starting_offset: The starting offset at which to generate random numbers
       using the random key. This can be used to advance the random stream as if
```

### Comparing `penzai-0.1.0/penzai/data_effects/side_input.py` & `penzai-0.1.1/penzai/data_effects/side_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
   instance of this is shared parameters, which can be represented in Penzai as
   side inputs with a constant value provided by a `WithConstantSideInputs`
   handler. If you want to extract a layer that uses shared parameters, you can
   first hoist out the constant values of all shared parameters, extract the
   submodel you want, and then re-bind the shared parameters of that subtree
   alone.
 
-  Calling `hoist_constant_side_inputs` on a layer and then immediatelly calling
+  Calling `hoist_constant_side_inputs` on a layer and then immediately calling
   `WithConstantSideInputs.handling` on the results will usually produce a layer
   with the same observable behavior, although the tree structure may differ.
   However, if ``scoped`` is False, it is possible that this function will raise
   an error due to tag conflicts.
 
   Args:
     tree: A tree to hoist constant side inputs from. Usually will contain
```

### Comparing `penzai-0.1.0/penzai/data_effects/side_output.py` & `penzai-0.1.1/penzai/data_effects/side_output.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/example_models/gemma/__init__.py` & `penzai-0.1.1/penzai/example_models/gemma/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/example_models/gemma/model_core.py` & `penzai-0.1.1/penzai/example_models/gemma/model_core.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/example_models/gemma/sampling_mode.py` & `penzai-0.1.1/penzai/example_models/gemma/sampling_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     This can be used to process inputs that do not need advanced position or
     attention mask handling, and which just consist of ordinary sequences that
     are not packed together or padded. It augments the tokens with a standard
     position array and causal attention mask, adjusted by the current cache
     offset.
 
     Args:
-      tokens: Subsquence of tokens, as an integer named array with a "seq" axis
+      tokens: Subsequence of tokens, as an integer named array with a "seq" axis
         and possibly batch axes. When pre-filling, the "seq" axis can be the
         length of the prompt. When sampling, the "seq" instance will usually
         have length 1.
       sampling_state: Current sampling state, containing key-value caches.
 
     Returns:
       A full input structure containing the provided tokens, along with a simple
```

### Comparing `penzai-0.1.0/penzai/example_models/gemma/simple_decoding_loop.py` & `penzai-0.1.1/penzai/example_models/gemma/simple_decoding_loop.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/example_models/simple_mlp.py` & `penzai-0.1.1/penzai/example_models/simple_mlp.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/__init__.py` & `penzai-0.1.1/penzai/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/attention.py` & `penzai-0.1.1/penzai/nn/attention.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/basic_ops.py` & `penzai-0.1.1/penzai/nn/basic_ops.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/combinators.py` & `penzai-0.1.1/penzai/nn/combinators.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/dropout.py` & `penzai-0.1.1/penzai/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/embeddings.py` & `penzai-0.1.1/penzai/nn/embeddings.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/grouping.py` & `penzai-0.1.1/penzai/nn/grouping.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/linear_and_affine.py` & `penzai-0.1.1/penzai/nn/linear_and_affine.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/parameters.py` & `penzai-0.1.1/penzai/nn/parameters.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/nn/standardization.py` & `penzai-0.1.1/penzai/nn/standardization.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/pz/__init__.py` & `penzai-0.1.1/penzai/pz/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/pz/de.py` & `penzai-0.1.1/penzai/pz/de.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/pz/nn.py` & `penzai-0.1.1/penzai/pz/nn.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/pz/ts.py` & `penzai-0.1.1/penzai/pz/ts.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/annotate_shapes.py` & `penzai-0.1.1/penzai/toolshed/annotate_shapes.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/basic_training.py` & `penzai-0.1.1/penzai/toolshed/basic_training.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/check_layers_by_tracing.py` & `penzai-0.1.1/penzai/toolshed/check_layers_by_tracing.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/interleave_intermediates.py` & `penzai-0.1.1/penzai/toolshed/interleave_intermediates.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/isolate_submodel.py` & `penzai-0.1.1/penzai/toolshed/isolate_submodel.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/jit_wrapper.py` & `penzai-0.1.1/penzai/toolshed/jit_wrapper.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/lora.py` & `penzai-0.1.1/penzai/toolshed/lora.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/model_rewiring.py` & `penzai-0.1.1/penzai/toolshed/model_rewiring.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/patch_ipdb.py` & `penzai-0.1.1/penzai/toolshed/patch_ipdb.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/sharding_util.py` & `penzai-0.1.1/penzai/toolshed/sharding_util.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/token_visualization.py` & `penzai-0.1.1/penzai/toolshed/token_visualization.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/toolshed/unflaxify.py` & `penzai-0.1.1/penzai/toolshed/unflaxify.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/__init__.py` & `penzai-0.1.1/penzai/treescope/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/arrayviz/__init__.py` & `penzai-0.1.1/penzai/treescope/arrayviz/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/arrayviz/array_autovisualizer.py` & `penzai-0.1.1/penzai/treescope/arrayviz/array_autovisualizer.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/arrayviz/arrayviz.py` & `penzai-0.1.1/penzai/treescope/arrayviz/arrayviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1472,22 +1472,22 @@
     label_bottom = str(value)
 
   fresh_id = "arrayviz" + uuid.uuid4().hex
   render_args = json.dumps({
       "value": value,
       "labelTop": label_top,
       "labelBottom": label_bottom,
+      "destinationId": fresh_id,
   })
   size_attr = html_escaping.escape_html_attribute(size)
   src = (
       f'<span id="{fresh_id}" class="inline_digitbox"'
       f' style="font-size: {size_attr}"></span>'
       '<template class="treescope_run_soon">'
-      f'<script>document.querySelector("#{fresh_id}").appendChild('
-      f"arrayviz.renderOneDigitbox({render_args}));</script></template>"
+      f"<script>arrayviz.renderOneDigitbox({render_args});</script></template>"
   )
   return ArrayvizRendering(src)
 
 
 @dataclasses.dataclass(frozen=True)
 class ValueColoredTextbox(
     figures.RendersAsRootInIPython, basic_parts.DeferringToChild
```

### Comparing `penzai-0.1.0/penzai/treescope/arrayviz/js/arrayviz.js` & `penzai-0.1.1/penzai/treescope/arrayviz/js/arrayviz.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -552,14 +552,34 @@
      * Configuration for a named axis. Start is inclusive, end exclusive.
      * Name is the label for each axis internally; label is the label we should
      * use as the annotation of the axis in the figure.
      * @typedef {{name: string, label: string, start: number, end: number}}
      */
     let AxisSpec;
 
+    /* Delays an action until a destination element becomes visible. */
+    function _delayUntilVisible(destinationId, action) {
+        // Trigger rendering as soon as the destination becomes visible.
+        const destination = /** @type {!Element} */
+            (document.getElementById(destinationId));
+        const visiblityObserver = new IntersectionObserver((entries) => {
+            if (entries[0].intersectionRatio > 0) {
+                const loadingMarkers = destination.querySelectorAll('.loading_message');
+                action();
+                for (let elt of loadingMarkers) {
+                    elt.remove();
+                }
+                visiblityObserver.disconnect();
+            }
+        }, {});
+        requestAnimationFrame(() => {
+            visiblityObserver.observe(destination);
+        });
+    }
+
     /**
      * Renders an array to a destination object.
      *  config.destinationId: ID of the HTML element to render into.
      *  config.info: Info for the figure; drawn on the bottom.
      *  config.arrayBase64: Base64-encoded array of either float32 or int32 data.
      *  config.arrayDtype: Either "float32" or "int32".
      *  config.validMaskBase64: Base64-encoded array of uint8-encoded boolean
@@ -590,28 +610,16 @@
      *    yAxisSpecs: !Array<!AxisSpec>,
      *    slicedAxisSpecs: !Array<!AxisSpec>,
      *    colormapConfig: !ColormapConfig,
      *    valueFormattingInstructions: !Array<?>,
      * }} config Configuration for the setup.
      */
     function buildArrayvizFigure(config) {
-        // Trigger rendering as soon as the destination becomes visible.
-        const destination = /** @type {!Element} */
-            (document.getElementById(config.destinationId));
-        const visiblityObserver = new IntersectionObserver((entries) => {
-            if (entries[0].intersectionRatio > 0) {
-                _buildArrayvizFigure(config);
-                for (let elt of destination.querySelectorAll('.loading_message')) {
-                    elt.remove();
-                }
-                visiblityObserver.disconnect();
-            }
-        }, {});
-        requestAnimationFrame(() => {
-            visiblityObserver.observe(destination);
+        _delayUntilVisible(config.destinationId, () => {
+            _buildArrayvizFigure(config);
         });
     }
 
     function _buildArrayvizFigure(config) {
         const destinationId = config.destinationId;
         const info = config.info;
         const arrayBase64 = config.arrayBase64;
@@ -871,21 +879,24 @@
             const row = Math.floor((y - 1) / cellSize) - 1;
 
             if (col < 0 || row < 0 || col >= colWidths[colWidths.length - 1] ||
                 row >= rowHeights[rowHeights.length - 1]) {
                 return null;
             }
 
+            // Compute positions along each named axis and the overall offset into
+            // the data array. We handle slider offsets first, then column and row
+            // offsets starting from the outermost in the rendering.
             const result = {};
+            let dataIndex = 0;
             for (const spec of slicedAxisSpecs) {
-                result[spec.name] = spec.start + activeSliceOffsets[spec.name];
+                const index = spec.start + activeSliceOffsets[spec.name];
+                result[spec.name] = index;
+                dataIndex += dataStrides[spec.name] * index;
             }
-            // Compute positions along each named axis, starting with the outermost
-            // in the rendering.
-            let dataIndex = 0;
             let colRemainder = col;
             for (let i = xAxisSpecs.length - 1; i >= 0; i--) {
                 const spec = xAxisSpecs[i];
                 const stride = colWidths[i] + seps[i];
                 const modulus = colWidths[i + 1] + seps[i + 1];
                 colRemainder = colRemainder % modulus;
                 const coord = Math.floor(colRemainder / stride);
@@ -1265,91 +1276,94 @@
     }
 
     /**
      * Renders a single cell representing an integer digit.
      *  config.value: Integer value to render.
      *  config.labelTop: Label to draw above the box.
      *  config.labelBottom: Label to draw below the box.
+     *  config.destinationId: ID of the element to render into.
      * @param {{
      *    value: number,
      *    labelTop: string,
      *    labelBottom: string,
+     *    destinationId: string,
      * }} config Configuration for the digitbox.
-     * @returns {!HTMLElement} The rendered element.
      */
     function renderOneDigitbox(config) {
-        const value = config.value;
-        const labelTop = config.labelTop;
-        const labelBottom = config.labelBottom;
-
-        const canvas =
-            /** @type {!HTMLCanvasElement} */
-            (document.createElement('canvas'));
-        canvas.width = cellSize;
-        canvas.height = cellSize;
-        const ctx =
-            /** @type {!CanvasRenderingContext2D} */
-            (canvas.getContext('2d'));
-        drawOneCell(ctx, 0, 0, value, true, {
-            type: 'digitbox'
-        }, null);
-
-        const container =
-            /** @type {!HTMLDivElement} */
-            (document.createElement('div'));
-        container.style.width = '1cap';
-        container.style.height = '1cap';
-        container.style.marginTop = '0.75em';
-        container.style.display = 'inline-block';
-        container.style.position = 'relative';
-        container.style.overflow = 'visible';
-        container.style.fontFamily = 'monospace';
-        container.style.whiteSpace = 'pre';
-        container.style.lineHeight = '2.5';
-        container.style.setProperty('image-rendering', 'pixelated');
+        _delayUntilVisible(config.destinationId, () => {
+            const destination = document.getElementById(config.destinationId);
+            const value = config.value;
+            const labelTop = config.labelTop;
+            const labelBottom = config.labelBottom;
+
+            const canvas =
+                /** @type {!HTMLCanvasElement} */
+                (document.createElement('canvas'));
+            canvas.width = cellSize;
+            canvas.height = cellSize;
+            const ctx =
+                /** @type {!CanvasRenderingContext2D} */
+                (canvas.getContext('2d'));
+            drawOneCell(ctx, 0, 0, value, true, {
+                type: 'digitbox'
+            }, null);
 
-        container.style.outline = '1px solid black';
-
-        container.appendChild(canvas);
-        canvas.style.width = '1cap';
-        canvas.style.height = '1cap';
-        canvas.style.position = 'absolute';
-
-        if (labelTop) {
-            const labelElt =
-                /** @type {!HTMLDivElement} */
-                (document.createElement('div'));
-            container.appendChild(labelElt);
-            labelElt.style.width = '200%';
-            labelElt.style.fontSize =
-                `${0.75 * Math.min(1, 3.5 / labelTop.length)}em`;
-            labelElt.style.position = 'absolute';
-            labelElt.style.left = '-50%';
-            labelElt.style.bottom = '110%';
-            labelElt.style.textAlign = 'center';
-            labelElt.style.lineHeight = '1';
-            labelElt.textContent = labelTop;
-        }
-        if (labelBottom) {
-            const labelElt =
+            const container =
                 /** @type {!HTMLDivElement} */
                 (document.createElement('div'));
-            container.appendChild(labelElt);
-            labelElt.style.width = '200%';
-            labelElt.style.fontSize =
-                `${0.75 * Math.min(1, 3.5 / labelBottom.length)}em`;
-            labelElt.style.position = 'absolute';
-            labelElt.style.left = '-50%';
-            labelElt.style.top = '110%';
-            labelElt.style.textAlign = 'center';
-            labelElt.style.lineHeight = '1';
-            labelElt.textContent = labelBottom;
-        }
-
-        return container;
+            container.style.width = '1cap';
+            container.style.height = '1cap';
+            container.style.marginTop = '0.75em';
+            container.style.display = 'inline-block';
+            container.style.position = 'relative';
+            container.style.overflow = 'visible';
+            container.style.fontFamily = 'monospace';
+            container.style.whiteSpace = 'pre';
+            container.style.lineHeight = '2.5';
+            container.style.setProperty('image-rendering', 'pixelated');
+
+            container.style.outline = '1px solid black';
+
+            container.appendChild(canvas);
+            canvas.style.width = '1cap';
+            canvas.style.height = '1cap';
+            canvas.style.position = 'absolute';
+
+            if (labelTop) {
+                const labelElt =
+                    /** @type {!HTMLDivElement} */
+                    (document.createElement('div'));
+                container.appendChild(labelElt);
+                labelElt.style.width = '200%';
+                labelElt.style.fontSize =
+                    `${0.75 * Math.min(1, 3.5 / labelTop.length)}em`;
+                labelElt.style.position = 'absolute';
+                labelElt.style.left = '-50%';
+                labelElt.style.bottom = '110%';
+                labelElt.style.textAlign = 'center';
+                labelElt.style.lineHeight = '1';
+                labelElt.textContent = labelTop;
+            }
+            if (labelBottom) {
+                const labelElt =
+                    /** @type {!HTMLDivElement} */
+                    (document.createElement('div'));
+                container.appendChild(labelElt);
+                labelElt.style.width = '200%';
+                labelElt.style.fontSize =
+                    `${0.75 * Math.min(1, 3.5 / labelBottom.length)}em`;
+                labelElt.style.position = 'absolute';
+                labelElt.style.left = '-50%';
+                labelElt.style.top = '110%';
+                labelElt.style.textAlign = 'center';
+                labelElt.style.lineHeight = '1';
+                labelElt.textContent = labelBottom;
+            }
+            destination.appendChild(container);
+        });
     }
 
     return {
         renderOneDigitbox: renderOneDigitbox,
         buildArrayvizFigure: buildArrayvizFigure,
     };
 })();
```

### Comparing `penzai-0.1.0/penzai/treescope/autovisualize.py` & `penzai-0.1.1/penzai/treescope/autovisualize.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/canonical_aliases.py` & `penzai-0.1.1/penzai/treescope/canonical_aliases.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/copypaste_fallback.py` & `penzai-0.1.1/penzai/treescope/copypaste_fallback.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/default_renderer.py` & `penzai-0.1.1/penzai/treescope/default_renderer.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/figures.py` & `penzai-0.1.1/penzai/treescope/figures.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/__init__.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/basic_parts.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/basic_parts.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/common_structures.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/common_structures.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/common_styles.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/common_styles.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/embedded_iframe.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/embedded_iframe.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/foldable_impl.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/foldable_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,20 +133,20 @@
         {{
             color: darkseagreen;
         }}
 
         .foldable_node:not({setup_context.collapsed_selector} *)
           > label:has(>.foldable_node_toggle:checked)::before
         {{
-            content: '▼';
+            content: '\\25bc';
         }}
         .foldable_node:not({setup_context.collapsed_selector} *)
           > label:has(>.foldable_node_toggle:not(:checked))::before
         {{
-            content: '▶';
+            content: '\\25b6';
         }}
 
         .foldable_node:not({setup_context.collapsed_selector} *) > label:hover
         {{
             cursor: pointer;
         }}
         .foldable_node:is({setup_context.collapsed_selector} *) > label
@@ -303,25 +303,14 @@
 
   def html_setup_parts(
       self, setup_context: HtmlContextForSetup
   ) -> set[CSSStyleRule | JavaScriptDefn]:
     rules = {
         JavaScriptDefn(html_escaping.without_repeated_whitespace("""
         (()=>{
-          const _get_root = (relative_to) => {
-            /* Look for the root node. */
-            let root = relative_to;
-            while (
-              root != document.body
-              && !root.classList.contains("treescope_root")
-            ) {
-              root = root.parentElement;
-            }
-            return root;
-          };
           const _get_target = (root, target_path) => {
             /* Look for the requested path string. */
             let target = root.querySelector(
                 `[data-keypath="${CSS.escape(target_path)}"]`
             );
             return target;
           };
@@ -329,15 +318,15 @@
               /* Try to jump to the label. */
               const possible = target.querySelector(":scope > label");
               return possible ? possible : target;
           };
 
           window.treescope.expand_and_scroll_to = (
             (linkelement, target_path) => {
-              const root = _get_root(linkelement);
+              const root = window.treescope.get_treescope_root(linkelement);
               const target = _get_target(root, target_path);
               /* Expand all of its parents. */
               let may_need_expand = target.parentElement;
               while (may_need_expand != root) {
                 if (may_need_expand.classList.contains("foldable_node")) {
                   const checkbox = may_need_expand.querySelector(
                       ":scope > label > .foldable_node_toggle");
@@ -359,15 +348,15 @@
                 }, 1200);
               }
             }
           );
 
           window.treescope.handle_hyperlink_mouse = (
             (linkelement, event, target_path) => {
-              const root = _get_root(linkelement);
+              const root = window.treescope.get_treescope_root(linkelement);
               const target = _get_target(root, target_path);
               if (event.type == "mouseover") {
                 target.classList.add("hyperlink_remote_hover");
               } else {
                 target.classList.remove("hyperlink_remote_hover");
               }
             }
@@ -483,14 +472,16 @@
   ):
     # Doesn't render at all in text mode.
     pass
 
   def html_setup_parts(
       self, setup_context: HtmlContextForSetup
   ) -> set[CSSStyleRule | JavaScriptDefn]:
+    # https://github.com/google/material-design-icons/blob/master/symbols/web/content_copy/materialsymbolsoutlined/content_copy_grad200_20px.svg
+    font_data_url = "data:font/woff2;base64,d09GMgABAAAAAAIQAAoAAAAABRwAAAHFAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAABmAAgkoKdIEBCwYAATYCJAMIBCAFgxIHLhtsBMieg3FDX2LI6YvSpuiPM5T1JXIRVMvWMztPyFFC+WgkTiBD0hiDQuJEdGj0Hb/fvIdpqK6hqWiiQuMnGhHfUtAU6BNr4AFInkE6cUuun+R5qcskwvfFl/qxgEo8gbJwG81HA/nAR5LrrJ1R+gz0Rd0AJf1gN7CwGj2g0oyuR77mE16wHX9OggpeTky4eIbz5cbrOGtaAgQINwDasysQuIIXWEFwAPQpIYdU//+g7T7X3t0fKPqAv52g0LAN7AMwAmgzRS+uZSeEXx2f6czN4RHy5uBAKzBjpFp3iHQCE0ZuP4S7nfBLEHFMmAi+8vE2hn1h7+bVwXjwHrvDGUCnjfEEgt+OcZll759CJwB8h94MMGS3GZAgmI5jBQ9tTGeH9EBBIG3Dg4R/YcybAGEAAVK/AQGaAeMClAHzEOgZtg6BPgOOIDBkiQ5eFBXCBFci0phropnQAApZED1z1kSfCfthyKnHdaFsHf0NmGEN6BdAqVVpatsSZmddai92fz94Uijq6pmr6OoYCSirGmvJG3SWS3FE2cBQfT+HlopG4Fsw5agq68iZeSNlpWnBHIedMreuWqGCm1WFrkSSx526WWswAQAA"
     rules = {
         JavaScriptDefn(html_escaping.without_repeated_whitespace("""
           window.treescope.handle_copy_click = async (button) => {
             const dataToCopy = button.dataset.copy;
             try {
               await navigator.clipboard.writeText(dataToCopy);
               button.classList.add("was_clicked");
@@ -503,37 +494,32 @@
                   "  # Failed to copy! Copy manually instead: " + dataToCopy
               );
             }
           };
         """)),
         CSSStyleRule(html_escaping.without_repeated_whitespace(f"""
           @font-face {{
-              font-family: 'Material Symbols Outlined';
+              font-family: 'Material Symbols Outlined Content Copy';
               font-style: normal;
-              font-weight: 100 700;
-              src: url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v114/kJEhBvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oFsLjBuVY.woff2) format('woff2');
+              font-weight: 400;
+              src: url({font_data_url}) format('woff2');
           }}
           {setup_context.collapsed_selector} .copybutton {{
               display: none;
           }}
+          .copybutton::before {{
+              content: " ";
+          }}
           .copybutton > span::before {{
-              content: " content_copy";
-              font-family: 'Material Symbols Outlined';
-              -webkit-font-feature-settings: 'liga';
+              content: "\\e14d";
+              font-family: 'Material Symbols Outlined Content Copy';
               -webkit-font-smoothing: antialiased;
-              font-variation-settings:
-                'FILL' 0,
-                'wght' 400,
-                'GRAD' 200,
-                'opsz' 20;
-              position: relative;
-              top: 0.1em;
               color: #e0e0e0;
               cursor: pointer;
-              font-size: 0.8em;
+              font-size: 0.9em;
           }}
           .copybutton:hover > span::before {{
               color: darkseagreen;
           }}
           .copybutton.was_clicked > span::after {{
               color: #cccccc;
           }}
@@ -823,14 +809,25 @@
   # the content is loaded, avoiding locking up the browser rendering process.
   stream.write(html_escaping.without_repeated_whitespace("""
   <script>
     if (window.treescope === undefined) {
       window.treescope = {};
       window.treescope._pendingActions = [];
       window.treescope._pendingActionHandle = null;
+      window.treescope.get_treescope_root = (relative_to) => {
+        /* Look for the root node. */
+        let root = relative_to;
+        while (
+          root != document.body
+          && !root.classList.contains("treescope_root")
+        ) {
+          root = root.parentElement;
+        }
+        return root;
+      };
       window.treescope.runSoon = (work) => {
           const doWork = () => {
               const tick = performance.now();
               while (performance.now() - tick < 32) {
                 if (window.treescope._pendingActions.length == 0) {
                     window.treescope._pendingActionHandle = null;
                     return;
@@ -910,20 +907,25 @@
       )
       stream.write("</span></div>")
 
     stream.write("<script>(() => {")
     all_ids = [deferred.placeholder.replacement_id for deferred in deferreds]
     stream.write(f"const targetIds = {json.dumps(all_ids)};")
     stream.write(html_escaping.without_repeated_whitespace("""
+        const root = window.treescope.get_treescope_root(
+            document.getElementById(targetIds[0]));
+        const fragment = document.createDocumentFragment();
+        const rootClone = fragment.appendChild(root.cloneNode(true));
         for (let i = 0; i < targetIds.length; i++) {
-            let target = document.getElementById(targetIds[i]);
+            let target = fragment.getElementById(targetIds[i]);
             let sourceDiv = document.getElementById("for_" + targetIds[i]);
-            target.parentNode.replaceChild(sourceDiv.firstElementChild, target);
+            target.replaceWith(sourceDiv.firstElementChild);
             sourceDiv.remove();
         }
+        root.replaceWith(rootClone);
       })();
       </script>
     """))
     stream.write("<script>window.treescope.enqueueDeferredTemplates()</script>")
     yield stream.getvalue()
 
 
@@ -956,30 +958,55 @@
 
 
 def display_streaming_as_root(
     root_node: RenderableTreePart,
     deferreds: Sequence[DeferredWithThunk],
     roundtrip: bool = False,
     compressed: bool = True,
-):
+    stealable: bool = False,
+) -> str | None:
   """Displays a root node in an IPython notebook in a streaming fashion.
 
   Args:
     root_node: The root node to render.
     deferreds: Deferred objects to render and splice in.
     roundtrip: Whether to render in roundtrip mode.
     compressed: Whether to compress the HTML for display.
+    stealable: Whether to return an extra HTML snippet that allows the streaming
+      rendering to be relocated after it is shown.
+
+  Returns:
+    If ``stealable`` is True, a final HTML snippet which, if inserted into a
+    document, will "steal" the root node rendering, moving the DOM nodes for it
+    into itself. In particular, using this as the HTML rendering of the root
+    node during pretty printing will correctly associate the rendering with the
+    IPython "cell output", which is visible in some IPython backends (e.g.
+    JupyterLab). If ``stealable`` is False, returns None.
   """
   import IPython.display  # pylint: disable=g-import-not-at-top
 
   render_iterator = _render_to_html_as_root_streaming(
       root_node, roundtrip, deferreds
   )
+  steal_id = uuid.uuid4().hex
   for i, step in enumerate(render_iterator):
     if compressed:
       if i == 0:
         step = html_compression.compress_html(
             step, include_preamble=True, loading_message="(Loading...)"
         )
+        if stealable:
+          step = f'<div id="output_{steal_id}">{step}</div>'
       else:
         step = html_compression.compress_html(step, include_preamble=False)
     IPython.display.display(IPython.display.HTML(step))
+
+  if stealable:
+    return html_escaping.without_repeated_whitespace(
+        """<div id="output_dest_{__STEAL_ID__}"><script>
+        (()=>{
+          const output = document.getElementById("output_{__STEAL_ID__}");
+          const dest = document.getElementById("output_dest_{__STEAL_ID__}");
+          dest.parentNode.replaceChild(output, dest);
+        })();
+        </script></div>""".replace("{__STEAL_ID__}", steal_id)
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/layout_algorithms.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/layout_algorithms.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/foldable_representation/part_interface.py` & `penzai-0.1.1/penzai/treescope/foldable_representation/part_interface.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/__init__.py` & `penzai-0.1.1/penzai/treescope/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/builtin_atom_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/builtin_atom_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/builtin_structure_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/builtin_structure_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/canonical_alias_postprocessor.py` & `penzai-0.1.1/penzai/treescope/handlers/canonical_alias_postprocessor.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/function_reflection_handlers.py` & `penzai-0.1.1/penzai/treescope/handlers/function_reflection_handlers.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/generic_pytree_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/generic_pytree_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/generic_repr_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/generic_repr_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/hardcoded_structure_handlers.py` & `penzai-0.1.1/penzai/treescope/handlers/hardcoded_structure_handlers.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/ndarray_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/ndarray_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/__init__.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/data_effects_handlers.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/data_effects_handlers.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/layer_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/layer_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/named_axes_handlers.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/named_axes_handlers.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/shapecheck_handlers.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/shapecheck_handlers.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/penzai/struct_handler.py` & `penzai-0.1.1/penzai/treescope/handlers/penzai/struct_handler.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/repr_html_postprocessor.py` & `penzai-0.1.1/penzai/treescope/handlers/repr_html_postprocessor.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/handlers/shared_value_postprocessor.py` & `penzai-0.1.1/penzai/treescope/handlers/shared_value_postprocessor.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/html_compression.py` & `penzai-0.1.1/penzai/treescope/html_compression.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/html_escaping.py` & `penzai-0.1.1/penzai/treescope/html_escaping.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/ndarray_summarization.py` & `penzai-0.1.1/penzai/treescope/ndarray_summarization.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/renderer.py` & `penzai-0.1.1/penzai/treescope/renderer.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/selection_rendering.py` & `penzai-0.1.1/penzai/treescope/selection_rendering.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/penzai/treescope/treescope_ipython.py` & `penzai-0.1.1/penzai/treescope/treescope_ipython.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,23 +175,27 @@
         else:
           foldable_ir = basic_parts.build_full_line_with_annotations(
               default_renderer.build_foldable_representation(
                   value, ignore_exceptions=True
               )
           )
         if streaming:
-          foldable_impl.display_streaming_as_root(
+          output_stealer = foldable_impl.display_streaming_as_root(
               foldable_ir,
               deferreds,
               roundtrip=False,
               compressed=compress_html,
+              stealable=True,
           )
-          # Once we get here, we've displayed everything already so there's
-          # nothing else to render.
-          return ""
+          # Executing the above call will have already displayed the output,
+          # but it may be in the wrong place (e.g. it may appear before the
+          # actual "Out" marker in JupyterLab). By returning `output_stealer`
+          # as the rendering of the object, we can ensure that the output is
+          # moved to the right place.
+          return output_stealer
         else:
           assert deferreds is None
           return foldable_impl.render_to_html_as_root(
               foldable_ir,
               roundtrip=False,
               compressed=compress_html,
           )
```

### Comparing `penzai-0.1.0/pyproject.toml` & `penzai-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "sphinx-book-theme>=1.0.1",
     "sphinxcontrib-katex",
     "ipython>=8.8.0",
     "myst-nb>=1.0.0",
     "matplotlib>=3.5.0",
     "sphinx-collections>=0.0.1",
     "sphinx_contributors",
+    "sphinx-hoverxref",
     "jax[cpu]>=0.4.23",
 ]
 
 [tool.pyink]
 # Formatting configuration to follow Google style-guide
 line-length = 80
 unstable = true
```

### Comparing `penzai-0.1.0/run_tests.py` & `penzai-0.1.1/run_tests.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/core_utils_test.py` & `penzai-0.1.1/tests/core_utils_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/data_effects/local_state_test.py` & `penzai-0.1.1/tests/data_effects/local_state_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/data_effects/random_test.py` & `penzai-0.1.1/tests/data_effects/random_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/data_effects/side_input_test.py` & `penzai-0.1.1/tests/data_effects/side_input_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/data_effects/side_output_test.py` & `penzai-0.1.1/tests/data_effects/side_output_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/example_models/gemma_test.py` & `penzai-0.1.1/tests/example_models/gemma_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/example_models/simple_mlp_test.py` & `penzai-0.1.1/tests/example_models/simple_mlp_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/fixtures/__init__.py` & `penzai-0.1.1/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/fixtures/treescope_examples_fixture.py` & `penzai-0.1.1/tests/fixtures/treescope_examples_fixture.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/misc_util_test.py` & `penzai-0.1.1/tests/misc_util_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/named_axes_test.py` & `penzai-0.1.1/tests/named_axes_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,24 +639,38 @@
   def test_named_array_conversion(self):
     array_a = named_axes.wrap(jnp.arange(6))
 
     with self.subTest("convert_positional_to_numpy"):
       array_a_as_np = np.array(array_a)
       self.assertEqual(array_a_as_np.shape, (6,))
 
+    with self.subTest("convert_positional_to_jax"):
+      array_a_as_jax = jnp.array(array_a)
+      self.assertEqual(array_a_as_jax.shape, (6,))
+
     with self.subTest("conversion_failure_with_names"):
       with self.assertRaisesRegex(
           ValueError,
           re.escape(
               "Only NamedArray(View)s with no named axes can be converted to"
               " numpy arrays"
           ),
       ):
         _ = np.array(array_a.tag("foo"))
 
+    with self.subTest("conversion_failure_with_names_jax"):
+      with self.assertRaisesRegex(
+          ValueError,
+          re.escape(
+              "Only NamedArray(View)s with no named axes can be converted to"
+              " JAX arrays"
+          ),
+      ):
+        _ = jnp.array(array_a.tag("foo"))
+
   def test_convenience_constructors(self):
     with self.subTest("zeros"):
       chex.assert_trees_all_equal(
           named_axes.zeros({"foo": 2, "bar": 3}, jnp.int32),
           named_axes.wrap(jnp.zeros((2, 3))).tag("foo", "bar"),
       )
     with self.subTest("ones"):
```

### Comparing `penzai-0.1.0/tests/nn/basic_ops_test.py` & `penzai-0.1.1/tests/nn/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/nn/embedding_test.py` & `penzai-0.1.1/tests/nn/embedding_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/nn/grouping_test.py` & `penzai-0.1.1/tests/nn/grouping_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/nn/linear_and_affine_test.py` & `penzai-0.1.1/tests/nn/linear_and_affine_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/nn/parameters_test.py` & `penzai-0.1.1/tests/nn/parameters_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/nn/standardization_test.py` & `penzai-0.1.1/tests/nn/standardization_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/partitioning_test.py` & `penzai-0.1.1/tests/partitioning_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/selectors_test.py` & `penzai-0.1.1/tests/selectors_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/shapecheck_test.py` & `penzai-0.1.1/tests/shapecheck_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/struct_pytree_dataclass_test.py` & `penzai-0.1.1/tests/struct_pytree_dataclass_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/toolshed/isolate_submodel_test.py` & `penzai-0.1.1/tests/toolshed/isolate_submodel_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/toolshed/lora_test.py` & `penzai-0.1.1/tests/toolshed/lora_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/toolshed/model_rewiring_test.py` & `penzai-0.1.1/tests/toolshed/model_rewiring_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/toolshed/sharding_util_test.py` & `penzai-0.1.1/tests/toolshed/sharding_util_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/toolshed/unflaxify_test.py` & `penzai-0.1.1/tests/toolshed/unflaxify_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/treescope_canonical_aliases_test.py` & `penzai-0.1.1/tests/treescope_canonical_aliases_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/treescope_renderer_test.py` & `penzai-0.1.1/tests/treescope_renderer_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/tests/treescope_representation_test.py` & `penzai-0.1.1/tests/treescope_representation_test.py`

 * *Files identical despite different names*

### Comparing `penzai-0.1.0/PKG-INFO` & `penzai-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penzai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Penzai: A JAX research toolkit for building, editing, and visualizing neural networks.
 Keywords: 
 Author-email: The Penzai Authors <penzai-dev@google.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -27,14 +27,15 @@
 Requires-Dist: sphinx-book-theme>=1.0.1 ; extra == "docs"
 Requires-Dist: sphinxcontrib-katex ; extra == "docs"
 Requires-Dist: ipython>=8.8.0 ; extra == "docs"
 Requires-Dist: myst-nb>=1.0.0 ; extra == "docs"
 Requires-Dist: matplotlib>=3.5.0 ; extra == "docs"
 Requires-Dist: sphinx-collections>=0.0.1 ; extra == "docs"
 Requires-Dist: sphinx_contributors ; extra == "docs"
+Requires-Dist: sphinx-hoverxref ; extra == "docs"
 Requires-Dist: jax[cpu]>=0.4.23 ; extra == "docs"
 Requires-Dist: ipython ; extra == "extras"
 Requires-Dist: flax>=0.8.2 ; extra == "extras"
 Requires-Dist: optax ; extra == "extras"
 Requires-Dist: ipython ; extra == "notebook"
 Requires-Dist: flax>=0.8.2 ; extra == "notebook"
 Requires-Dist: optax ; extra == "notebook"
@@ -57,14 +58,18 @@
 structures, along with tools for visualizing, modifying, and analyzing them.
 Penzai focuses on **making it easy to do stuff with models after they have been
 trained**, making it a great choice for research involving reverse-engineering
 or ablating model components, inspecting and probing internal activations,
 performing model surgery, debugging architectures, and more. (But if you just
 want to build and train a model, you can do that too!)
 
+With Penzai, your neural networks could look like this:
+
+![Screenshot of the Gemma model in Penzai](docs/_static/readme_teaser.png)
+
 Penzai is structured as a collection of modular tools, designed together but
 each useable independently:
 
 * `penzai.nn` (`pz.nn`): A declarative combinator-based neural network
   library and an alternative to other neural network libraries like Flax, Haiku,
   Keras, or Equinox, which exposes the full structure of your model's
   forward pass in the model pytree. This means you can see everything your model
@@ -91,67 +96,80 @@
 * `penzai.data_effects` (`pz.de`): An opt-in system for side arguments, random
   numbers, and state variables that is built on pytree traversal and puts you
   in control, without getting in the way of writing or using your model.
 
 Documentation on Penzai can be found at
 [https://penzai.readthedocs.io](https://penzai.readthedocs.io).
 
+> [!WARNING]
+> Penzai's API is currently unstable and may change in future releases.
+>
+> In particular, the way Penzai handles parameter initialization, parameter
+> sharing, and local mutable state in `penzai.nn` and
+> `penzai.data_effects` is likely to be simplified in the future.
+> Some internal details of the `treescope` pretty-printer intermediate
+> representation may also change to make it easier to extend and configure.
+>
+> Projects that use Penzai's neural network components or model implementations,
+> or that define their own handlers for `treescope`, are encouraged to pin the
+> `0.1.x` release series (e.g. `penzai>=0.1,<0.2`) to avoid breaking changes.
+
 
 ## Getting Started
 
 If you haven't already installed JAX, you should do that first, since the
 installation process depends on your platform. You can find instructions in the
 [JAX documentation](https://jax.readthedocs.io/en/latest/installation.html).
 Afterward, you can install Penzai using
 
-```
+```python
 pip install penzai
 ```
 
 and import it using
 
-```
+```python
 import penzai
 from penzai import pz
 ```
 
 (`penzai.pz` is an *alias namespace*, which makes it easier to reference
 common Penzai objects.)
 
 When working in an Colab or IPython notebook, we recommend also configuring
 Penzai as the default pretty printer, and enabling some utilities for
 interactive use:
 
-```
+```python
 pz.ts.register_as_default()
 pz.ts.register_autovisualize_magic()
 pz.enable_interactive_context()
 
 # Optional: enables automatic array visualization
 pz.ts.active_autovisualizer.set_interactive(pz.ts.ArrayAutovisualizer())
 ```
 
 Here's how you could initialize and visualize a simple neural network:
 
-```
+```python
 from penzai.example_models import simple_mlp
 mlp = pz.nn.initialize_parameters(
     simple_mlp.MLP.from_config([8, 32, 32, 8]),
     jax.random.key(42),
 )
 
 # Models and arrays are visualized automatically when you output them from a
 # Colab/IPython notebook cell:
 mlp
 ```
 
 Here's how you could capture and extract the activations after the elementwise
 nonlinearities:
 
-```
+```python
 mlp_with_captured_activations = pz.de.CollectingSideOutputs.handling(
     pz.select(mlp)
     .at_instances_of(pz.nn.Elementwise)
     .insert_after(pz.de.TellIntermediate())
 )
 
 output, intermediates = mlp_with_captured_activations(
```

