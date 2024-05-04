# Comparing `tmp/pymmcore_plus-0.9.4.tar.gz` & `tmp/pymmcore_plus-0.9.5.tar.gz`

## Comparing `pymmcore_plus-0.9.4.tar` & `pymmcore_plus-0.9.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/__init__.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/_build.py
--rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/_cli.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/_logger.py
--rw-r--r--   0        0        0    17021 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/_util.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/install.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/py.typed
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/seq_tester.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/__init__.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_adapter.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_config.py
--rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_config_group.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_constants.py
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_device.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_metadata.py
--rw-r--r--   0        0        0    86477 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_mmcore_plus.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_property.py
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_sequencing.py
--rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/_state.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_device_signal_view.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_norm_slot.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_prop_event_mixin.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_protocol.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_psygnal.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_qsignals.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/__init__.py
--rw-r--r--   0        0        0    21084 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_engine.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_protocol.py
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_runner.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_thread_relay.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/__init__.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_protocol.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_psygnal.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_qsignals.py
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_5d_writer_base.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/__init__.py
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_img_sequence_writer.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_ome_tiff_writer.py
--rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_ome_zarr_writer.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_util.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/__init__.py
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_config_file.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_config_group.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_core_device.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_core_link.py
--rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_device.py
--rw-r--r--   0        0        0     9822 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_microscope.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_pixel_size_config.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/src/pymmcore_plus/model/_property.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/conftest.py
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/local_config.cfg
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_adapter_class.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_bench.py
--rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_cli.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_config_group_class.py
--rw-r--r--   0        0        0    20066 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_core.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_device_class.py
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_events.py
--rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_mda.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_misc.py
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_model.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_pixel_config_class.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_property_class.py
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_sequencing.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/test_thread_relay.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/io/test_image_sequence_writer.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/io/test_ome_tiff.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/tests/io/test_ome_zarr.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/LICENSE
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/README.md
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/__init__.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/_build.py
+-rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/_cli.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/_logger.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/_util.py
+-rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/install.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/py.typed
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/seq_tester.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/__init__.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_adapter.py
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_config.py
+-rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_config_group.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_constants.py
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_device.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_metadata.py
+-rw-r--r--   0        0        0    86477 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_mmcore_plus.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_property.py
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_sequencing.py
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/_state.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_device_signal_view.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_norm_slot.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_prop_event_mixin.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_protocol.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_psygnal.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_qsignals.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/__init__.py
+-rw-r--r--   0        0        0    21446 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_engine.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_protocol.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_runner.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_thread_relay.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/__init__.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_protocol.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_psygnal.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_qsignals.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_5d_writer_base.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/__init__.py
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_img_sequence_writer.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_ome_tiff_writer.py
+-rw-r--r--   0        0        0    12131 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_ome_zarr_writer.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_util.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/__init__.py
+-rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_config_file.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_config_group.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_core_device.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_core_link.py
+-rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_device.py
+-rw-r--r--   0        0        0     9822 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_microscope.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_pixel_size_config.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/src/pymmcore_plus/model/_property.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/__init__.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/conftest.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/local_config.cfg
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_adapter_class.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_bench.py
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_cli.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_config_group_class.py
+-rw-r--r--   0        0        0    20066 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_core.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_device_class.py
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_events.py
+-rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_mda.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_misc.py
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_model.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_pixel_config_class.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_property_class.py
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_sequencing.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/test_thread_relay.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/io/test_image_sequence_writer.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/io/test_ome_tiff.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/tests/io/test_ome_zarr.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/LICENSE
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/README.md
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 pymmcore_plus-0.9.5/PKG-INFO
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/__init__.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/_build.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/_build.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/_cli.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/_cli.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/_logger.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 from typing import ClassVar, Iterator
 
 __all__ = ["logger"]
 
 
 logger = logging.getLogger("pymmcore-plus")
 
-
+PYMM_LOG_FILE = os.getenv("PYMM_LOG_FILE", "")
 DEFAULT_LOG_LEVEL: str = os.getenv("PYMM_LOG_LEVEL", "INFO").upper()
-if any(x.endswith("pytest") for x in sys.argv):
+
+if "PYTEST_RUNNING" in os.environ:
     LOG_FILE = None
-elif "PYMM_LOG_FILE" in os.environ:
-    if os.environ["PYMM_LOG_FILE"].lower() in ("", "0", "false", "no", "none"):
-        LOG_FILE = None
-    else:
-        LOG_FILE = Path(os.environ["PYMM_LOG_FILE"]).expanduser().resolve()
+elif PYMM_LOG_FILE not in ("", "0", "false", "no", "none"):
+    LOG_FILE = Path(PYMM_LOG_FILE).expanduser().resolve()
 else:
     from ._util import USER_DATA_DIR
 
     LOG_FILE = USER_DATA_DIR / "logs" / "pymmcore-plus.log"
 
 
 class CustomFormatter(logging.Formatter):
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/_util.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,24 +137,29 @@
         logger.debug("using MM path found in applications: %s", pth)
         return str(pth)
     if pth is not None:
         full_list.append(str(pth))
     return full_list
 
 
-def _qt_app_is_running() -> bool:
+def _imported_qt_modules() -> Iterator[str]:
     for modname in {"PyQt5", "PySide2", "PyQt6", "PySide6"}:
         if modname in sys.modules:
-            try:
-                # in broken environments modname can be a namespace package...
-                # and QtWidgets will still be unavailable
-                QtWidgets = importlib.import_module(".QtWidgets", modname)
-            except ImportError:  # pragma: no cover
-                continue
-            return QtWidgets.QApplication.instance() is not None
+            yield modname
+
+
+def _qt_app_is_running() -> bool:
+    for modname in _imported_qt_modules():
+        try:
+            # in broken environments modname can be a namespace package...
+            # and QtWidgets will still be unavailable
+            QtWidgets = importlib.import_module(".QtWidgets", modname)
+        except ImportError:  # pragma: no cover
+            continue
+        return QtWidgets.QApplication.instance() is not None
     return False  # pragma: no cover
 
 
 MMCORE_PLUS_SIGNALS_BACKEND = "MMCORE_PLUS_SIGNALS_BACKEND"
 
 
 def signals_backend() -> Literal["qt", "psygnal"]:
@@ -164,18 +169,19 @@
         warnings.warn(
             f"{MMCORE_PLUS_SIGNALS_BACKEND} must be one of ['qt', 'psygnal', 'auto']. "
             f"not: {env_var!r}. Using 'auto'.",
             stacklevel=1,
         )
         env_var = "auto"
 
+    qt_app_running = _qt_app_is_running()
     if env_var == "auto":
-        return "qt" if _qt_app_is_running() else "psygnal"
+        return "qt" if qt_app_running else "psygnal"
     if env_var == "qt":
-        if _qt_app_is_running():
+        if qt_app_running or list(_imported_qt_modules()):
             return "qt"
         warnings.warn(
             f"{MMCORE_PLUS_SIGNALS_BACKEND} set to 'qt', but no Qt app is running. "
             "Falling back to 'psygnal'.",
             stacklevel=1,
         )
     return "psygnal"
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/install.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         with progress.Progress(
             progress.SpinnerColumn(), progress.TextColumn(f"[{color}]{text}")
         ) as pbar:
             pbar.add_task(description=text, total=None)
             yield pbar
 
 except ImportError:  # pragma: no cover
-    progress = None
+    progress = None  # type: ignore
 
     def _pretty_print(text: str, color: str = "", emoji: str = "") -> None:
         print(text)
 
     @contextmanager
     def _spinner(text: str = "", color: str = "") -> Iterator[None]:
         print(text)
@@ -66,15 +66,15 @@
         content: str = tmp.headers.get("Content-Disposition")
         for part in content.split(";"):
             if "filename=" in part:
                 return part.split("=")[1].strip('"')
     return ""
 
 
-def _get_spinner(log_msg: _MsgLogger) -> Callable[[str], ContextManager[None]]:
+def _get_spinner(log_msg: _MsgLogger) -> Callable[[str], ContextManager]:
     if log_msg is _pretty_print:
         spinner = _spinner
     else:
 
         @contextmanager
         def spinner(msg: str) -> Iterator[None]:
             log_msg(msg)
@@ -173,15 +173,15 @@
 
         def hook(count: float, block_size: float, total_size: float) -> None:
             pbar.update(task_id, total=int(total_size))
             pbar.start_task(task_id)
             pbar.update(task_id, advance=block_size)
 
     else:
-        pbar = nullcontext()
+        pbar = nullcontext()  # type: ignore
 
         def hook(count: float, block_size: float, total_size: float) -> None: ...
 
     with pbar:
         urlretrieve(url=url, filename=output_path, reporthook=hook)
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/seq_tester.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/seq_tester.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/__init__.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_adapter.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_adapter.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_config.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_config.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_config_group.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_config_group.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_constants.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_constants.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_device.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_device.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_metadata.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_metadata.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_mmcore_plus.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_mmcore_plus.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_property.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_property.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_sequencing.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_sequencing.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/_state.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/_state.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/__init__.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_device_signal_view.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_device_signal_view.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_norm_slot.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_norm_slot.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_prop_event_mixin.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_prop_event_mixin.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_protocol.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_psygnal.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_psygnal.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/core/events/_qsignals.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/core/events/_qsignals.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_engine.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import time
+from contextlib import suppress
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     Iterable,
     Iterator,
     Mapping,
@@ -306,14 +307,20 @@
         tags = dict(meta) if meta else {}
         for dev, label, val in self._mmc.getSystemStateCache():
             tags[f"{dev}-{label}"] = val
 
         # these are added by AcqEngJ
         # yyyy-MM-dd HH:mm:ss.mmmmmm  # NOTE AcqEngJ omits microseconds
         tags["Time"] = datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")
+        tags["PixelSizeUm"] = self._mmc.getPixelSizeUm(True)  # true == cached
+        with suppress(RuntimeError):
+            tags["XPositionUm"] = self._mmc.getXPosition()
+            tags["YPositionUm"] = self._mmc.getYPosition()
+        with suppress(RuntimeError):
+            tags["ZPositionUm"] = self._mmc.getZPosition()
 
         # used by Runner
         tags["PerfCounter"] = time.perf_counter()
         return tags
 
     def teardown_event(self, event: MDAEvent) -> None:
         """Teardown state of system (hardware, etc.) after `event`."""
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_protocol.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_runner.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_runner.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/_thread_relay.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/_thread_relay.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/__init__.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_protocol.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_psygnal.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_psygnal.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/events/_qsignals.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/events/_qsignals.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_5d_writer_base.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_5d_writer_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from abc import abstractmethod
 from collections import defaultdict
-from typing import TYPE_CHECKING, Generic, Protocol, TypeVar
+from typing import TYPE_CHECKING, Generic, Mapping, Protocol, TypeVar
 
 from ._util import position_sizes
 
 if TYPE_CHECKING:
     import numpy as np
     import useq
 
@@ -68,38 +68,62 @@
         # maps position key to list of frame metadata
         self.frame_metadatas: defaultdict[str, list[dict]] = defaultdict(list)
 
         # set during sequenceStarted and cleared during sequenceFinished
         self.current_sequence: useq.MDASequence | None = None
 
         # list of {dim_name: size} map for each position in the sequence
-        self.position_sizes: list[dict[str, int]] = []
+        self._position_sizes: list[dict[str, int]] = []
+
+        # actual timestamps for each frame
+        self._timestamps: list[float] = []
 
     # The next three methods - `sequenceStarted`, `sequenceFinished`, and `frameReady`
     # are to be connected directly to the MDA's signals, perhaps via listener_connected
 
+    @property
+    def position_sizes(self) -> list[dict[str, int]]:
+        """Return sizes of each dimension for each position in the sequence.
+
+        Will be a list of dicts, where each dict maps dimension names to sizes, and
+        the index in the list corresponds to the stage position index.
+
+        This is the preferred way to access both the dimensions present in each position
+        as well as the sizes of those dimensions.
+
+        The dict is ordered, and the order reflects the order of dimensions in the
+        shape of each position.
+        """
+        return self._position_sizes
+
     def sequenceStarted(self, seq: useq.MDASequence) -> None:
         """On sequence started, simply store the sequence."""
         self.frame_metadatas.clear()
         self.current_sequence = seq
         if seq:
-            self.position_sizes = position_sizes(seq)
+            self._position_sizes = position_sizes(seq)
 
     def sequenceFinished(self, seq: useq.MDASequence) -> None:
         """On sequence finished, clear the current sequence."""
         self.finalize_metadata()
         self.frame_metadatas.clear()
-        self.current_sequence = None
-        self.position_sizes = []
+
+    def get_position_key(self, position_index: int) -> str:
+        """Get the position key for a specific position index.
+
+        This key will be used for subclasses like Zarr that need a directory structure
+        for each position.  And may also be used to index into `self.position_arrays`.
+        """
+        return f"{POS_PREFIX}{position_index}"
 
     def frameReady(self, frame: np.ndarray, event: useq.MDAEvent, meta: dict) -> None:
         """Write frame to the zarr array for the appropriate position."""
         # get the position key to store the array in the group
         p_index = event.index.get("p", 0)
-        key = f"{POS_PREFIX}{p_index}"
+        key = self.get_position_key(p_index)
         pos_sizes = self.position_sizes[p_index]
         if key in self.position_arrays:
             ary = self.position_arrays[key]
         else:
             # this is the first time we've seen this position
             # create a new array in the group for it
             if not self.current_sequence:
@@ -113,14 +137,17 @@
             # create the new array, getting XY chunksize from the frame
             # and total shape from the sequence.
             sizes = pos_sizes.copy()
             sizes["y"], sizes["x"] = frame.shape[-2:]
             self.position_arrays[key] = ary = self.new_array(key, frame.dtype, sizes)
 
         index = tuple(event.index[k] for k in pos_sizes)
+        t = event.index.get("t", 0)
+        if t >= len(self._timestamps) and "ElapsedTime-ms" in meta:
+            self._timestamps.append(meta["ElapsedTime-ms"])
         self.write_frame(ary, index, frame)
         self.store_frame_metadata(key, event, meta)
 
     @abstractmethod
     def new_array(
         self, position_key: str, dtype: np.dtype, dim_sizes: dict[str, int]
     ) -> T:
@@ -190,7 +217,57 @@
 
     def finalize_metadata(self) -> None:
         """Called during sequenceFinished before clearing sequence metadata.
 
         Subclasses may override this method to flush any accumulated frame metadata to
         disk at the end of the sequence.
         """
+
+    # This syntax is intentionally the same as xarray's isel method.  It's possible
+    # we will use xarray in the future, and this will make it easier to switch.
+    def isel(
+        self,
+        indexers: Mapping[str, int | slice] | None = None,
+        **indexers_kwargs: int | slice,
+    ) -> np.ndarray:
+        """Select data from the array.
+
+        This is a convenience method to select data from the array for a given position
+        key.  It will call the appropriate `__getitem__` method on the array with the
+        given indexers.
+
+        Parameters
+        ----------
+        indexers : Mapping[str, int | slice] | None
+            Mapping of dimension names to indices or slices.  If None, will return the
+            full array.
+        **indexers_kwargs : int | slice
+            Keyword arguments of dimension names to indices or slices.  These will be
+            merged with `indexers`, and allows for a nicer syntax.
+
+        Returns
+        -------
+        np.ndarray
+            The selected data from the array.
+
+        Examples
+        --------
+        >>> data = writer.isel(t=0, z=1, c=0, x=slice(128, 256))
+        """
+        indexers = dict(indexers or {})
+        indexers.update(indexers_kwargs)
+
+        p_index = indexers.get("p", 0)
+        if isinstance(p_index, slice):
+            raise NotImplementedError("Cannot slice over position index")  # TODO
+
+        try:
+            sizes = [*list(self.position_sizes[p_index]), "y", "x"]
+        except IndexError as e:
+            raise IndexError(
+                f"Position index {p_index} out of range for {len(self.position_sizes)}"
+            ) from e
+
+        data = self.position_arrays[self.get_position_key(p_index)]
+        full = slice(None, None)
+        index = tuple(indexers.get(k, full) for k in sizes)
+        return data[index]  # type: ignore
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_img_sequence_writer.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_img_sequence_writer.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_ome_tiff_writer.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_ome_tiff_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     def sequenceStarted(self, seq: useq.MDASequence) -> None:
         super().sequenceStarted(seq)
         # Non-OME (ImageJ) hyperstack axes MUST be in TZCYXS order
         # so we reorder the ordered position_sizes dicts.  This will ensure
         # that the array indices created from event.index are in the correct order.
         if not self._is_ome:
-            self.position_sizes = [
+            self._position_sizes = [
                 {k: x[k] for k in IMAGEJ_AXIS_ORDER if k.lower() in x}
                 for x in self.position_sizes
             ]
 
     def write_frame(
         self, ary: np.memmap, index: tuple[int, ...], frame: np.ndarray
     ) -> None:
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_ome_zarr_writer.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_ome_zarr_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import atexit
 import json
 import os.path
 import shutil
 import tempfile
+from contextlib import suppress
 from typing import TYPE_CHECKING, Any, Literal, MutableMapping, Protocol
 
+import numpy as np
+
 from ._5d_writer_base import _5DWriterBase
 
 if TYPE_CHECKING:
     from os import PathLike
     from typing import ContextManager, Sequence, TypedDict
 
-    import numpy as np
+    import xarray as xr
     import zarr
     from fsspec import FSMap
     from numcodecs.abc import Codec
 
     class ZarrSynchronizer(Protocol):
         def __getitem__(self, key: str) -> ContextManager: ...
 
@@ -182,22 +185,82 @@
     def group(self) -> zarr.Group:
         """Read-only access to the zarr group."""
         return self._group
 
     def finalize_metadata(self) -> None:
         """Called by superclass in sequenceFinished.  Flush metadata to disk."""
         # flush frame metadata to disk
+        self._populate_xarray_coords()
         while self.frame_metadatas:
             key, metas = self.frame_metadatas.popitem()
             if key in self.position_arrays:
                 self.position_arrays[key].attrs["frame_meta"] = metas
 
         if self._minify_metadata:
             self._minify_zattrs_metadata()
 
+    def _populate_xarray_coords(self) -> None:
+        # FIXME:
+        # This provides support for xarray coordinates... but it's not obvious
+        # how we should deal with positions that have different shapes, etc...
+        # Also: this whole thing should be generalized to support any kind of
+        # dimension, and should be better about populating the coords as the experiment
+        # progresses.  And it's rather ugly...
+        if not (seq := self.current_sequence):
+            return
+
+        sizes = {**seq.sizes}
+        px = 1
+        if self.frame_metadatas:
+            key, metas = next(iter(self.frame_metadatas.items()))
+            if key in self.position_arrays:
+                shape = self.position_arrays[key].shape
+                px = metas[-1].get("PixelSizeUm", 1)
+                with suppress(IndexError):
+                    sizes.update(y=shape[-2], x=shape[-1])
+
+        for dim, size in sizes.items():
+            if size == 0:
+                continue
+
+            # TODO: this could be much cleaner
+            attrs: dict = {"_ARRAY_DIMENSIONS": [dim]}
+            if dim == "t":
+                if self._timestamps:
+                    coords: Any = list(self._timestamps)
+                elif seq.time_plan:
+                    coords = np.arange(seq.time_plan.num_timepoints(), dtype="float")
+                else:
+                    continue
+                attrs["units"] = "ms"
+            elif dim == "p":
+                # coords = [(p.x, p.y, p.z) for p in seq.stage_positions]
+                coords = np.arange(size)
+            elif dim == "c":
+                coords = [c.config for c in seq.channels]
+            elif dim == "z":
+                coords = list(seq.z_plan) if seq.z_plan else [0]
+                attrs["units"] = "um"
+            elif dim in "yx":
+                coords = np.arange(size, dtype="float") * px
+                attrs["units"] = "um"
+            elif dim == "g":
+                coords = np.arange(size)
+                # TODO
+            else:
+                continue
+
+            # fill_value=None is important to avoid nan where coords == 0
+            if dim in self._group:
+                ds = self._group[dim]
+                ds[:] = coords
+            else:
+                ds = self._group.create_dataset(dim, data=coords, fill_value=None)
+            ds.attrs.update(attrs)
+
     def new_array(self, key: str, dtype: np.dtype, sizes: dict[str, int]) -> zarr.Array:
         """Create a new array in the group, under `key`."""
         dims, shape = zip(*sizes.items())
         ary: zarr.Array = self._group.create(
             key,
             shape=shape,
             chunks=(1,) * len(shape[:-2]) + shape[-2:],  # single XY plane chunks
@@ -246,14 +309,19 @@
         store = self._group.store
         for key in store.keys():
             if key.endswith(".zattrs"):
                 data = json_loads(store[key])
                 # dump minified data back to disk
                 store[key] = json.dumps(data, separators=(",", ":")).encode("ascii")
 
+    def as_xarray(self) -> xr.Dataset:
+        import xarray as xr
+
+        return xr.open_zarr(self.group.store, consolidated=False)
+
 
 # https://ngff.openmicroscopy.org/0.4/index.html#axes-md
 AXTYPE = {
     "x": "space",
     "y": "space",
     "z": "space",
     "c": "channel",
```

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/mda/handlers/_util.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/mda/handlers/_util.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_config_file.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_config_file.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_config_group.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_config_group.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_core_device.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_core_device.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_core_link.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_core_link.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_device.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_device.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_microscope.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_microscope.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_pixel_size_config.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_pixel_size_config.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/src/pymmcore_plus/model/_property.py` & `pymmcore_plus-0.9.5/src/pymmcore_plus/model/_property.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/conftest.py` & `pymmcore_plus-0.9.5/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
+import os
 from unittest.mock import patch
 
-import pymmcore_plus
-import pytest
-from pymmcore_plus._logger import logger
-from pymmcore_plus.core.events import CMMCoreSignaler
-from pymmcore_plus.mda.events import MDASignaler
+os.environ["PYTEST_RUNNING"] = "1"
+
+import pymmcore_plus  # noqa: E402
+import pytest  # noqa: E402
+from pymmcore_plus._logger import logger  # noqa: E402
+from pymmcore_plus.core.events import CMMCoreSignaler  # noqa: E402
+from pymmcore_plus.mda.events import MDASignaler  # noqa: E402
 
 try:
     from pymmcore_plus.core.events import QCoreSignaler
     from pymmcore_plus.mda.events import QMDASignaler
 
     PARAMS = ["QSignal", "psygnal"]
 except ImportError:
```

### Comparing `pymmcore_plus-0.9.4/tests/local_config.cfg` & `pymmcore_plus-0.9.5/tests/local_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_adapter_class.py` & `pymmcore_plus-0.9.5/tests/test_adapter_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_bench.py` & `pymmcore_plus-0.9.5/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_cli.py` & `pymmcore_plus-0.9.5/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,19 +245,14 @@
 
     Timer(0.2, lambda: kill(getpid(), SIGINT)).start()
     result = runner.invoke(app, ["logs", "--tail"], input="ctrl-c")
     q.put(result.output)
 
 
 def test_cli_logs(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> None:
-    # at first there should be no logs
-    result = runner.invoke(app, ["logs"])
-    assert result.exit_code == 0
-    assert "No log file" in result.stdout
-
     # create mock log file
     TEST_LOG = tmp_path / "test.log"
     monkeypatch.setattr(_logger, "LOG_FILE", TEST_LOG)
     _logger.configure_logging(file=TEST_LOG)
     assert _logger.current_logfile(_logger.logger) == TEST_LOG
     assert TEST_LOG.exists()
```

### Comparing `pymmcore_plus-0.9.4/tests/test_config_group_class.py` & `pymmcore_plus-0.9.5/tests/test_config_group_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_core.py` & `pymmcore_plus-0.9.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_device_class.py` & `pymmcore_plus-0.9.5/tests/test_device_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_events.py` & `pymmcore_plus-0.9.5/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_mda.py` & `pymmcore_plus-0.9.5/tests/test_mda.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_misc.py` & `pymmcore_plus-0.9.5/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_model.py` & `pymmcore_plus-0.9.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_pixel_config_class.py` & `pymmcore_plus-0.9.5/tests/test_pixel_config_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_property_class.py` & `pymmcore_plus-0.9.5/tests/test_property_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_sequencing.py` & `pymmcore_plus-0.9.5/tests/test_sequencing.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/test_thread_relay.py` & `pymmcore_plus-0.9.5/tests/test_thread_relay.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/io/test_image_sequence_writer.py` & `pymmcore_plus-0.9.5/tests/io/test_image_sequence_writer.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/io/test_ome_tiff.py` & `pymmcore_plus-0.9.5/tests/io/test_ome_tiff.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/tests/io/test_ome_zarr.py` & `pymmcore_plus-0.9.5/tests/io/test_ome_zarr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+import numpy as np
 import pytest
 import useq
 from pymmcore_plus.mda.handlers import OMEZarrWriter
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     import zarr
     from pymmcore_plus import CMMCorePlus
 else:
     zarr = pytest.importorskip("zarr")
 
+try:
+    import xarray as xr
+except ImportError:
+    xr = None
+
 
 SIMPLE_MDA = useq.MDASequence(
     channels=["Cy5", "FITC"],
     time_plan={"interval": 0.1, "loops": 2},
     axis_order="tpcz",
 )
 SIMPLE_EXPECTATION = {"p0": {"t": 2, "c": 2, "y": 512, "x": 512}}
@@ -86,24 +92,39 @@
         writer = OMEZarrWriter(tmp_path / store)
 
     core.mda.run(mda, output=writer)
 
     if store:
         # ensure that non-memory stores were written to disk
         data = zarr.open(writer.group.store.path)
-        for _, ary in data.arrays():
-            # ensure real data was written
-            assert ary.nchunks_initialized > 0
-            assert ary[0, 0].mean() > ary.fill_value
+        for k, ary in data.arrays():
+            if k in writer.position_arrays:
+                # ensure real data was written
+                assert ary.nchunks_initialized > 0
+                assert ary[0, 0].mean() > ary.fill_value
     else:
         data = writer.group
 
     # check that arrays have expected shape and dimensions
-    actual_shapes = {
-        k: dict(zip(v.attrs["_ARRAY_DIMENSIONS"], v.shape)) for k, v in data.arrays()
-    }
-    assert actual_shapes == expected_shapes
+    for k, v in data.arrays():
+        if k not in writer.position_arrays:
+            continue  # not a position array
+
+        actual_shape = dict(zip(v.attrs["_ARRAY_DIMENSIONS"], v.shape))
+        assert expected_shapes[k] == actual_shape
 
-    # check that the MDASequence was stored
-    for _, v in data.arrays():
+        # check that the MDASequence was stored
         stored_seq = useq.MDASequence.parse_obj(v.attrs["useq_MDASequence"])
         assert stored_seq == mda
+
+        if xr is not None:
+            # check that the xarray was written
+            ds = writer.as_xarray()
+            assert isinstance(ds, xr.Dataset)
+            assert ds[k].sizes == expected_shapes[k]
+            # check that *most* dimensions have coordinates
+            for dim_name in ds.dims:
+                if dim_name != "g":
+                    assert dim_name in ds.coords
+
+    # smoke test the isel method
+    assert isinstance(writer.isel(p=0, t=0, x=slice(0, 100)), np.ndarray)
```

### Comparing `pymmcore_plus-0.9.4/.gitignore` & `pymmcore_plus-0.9.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -140,9 +140,9 @@
 Micro-Manager-*
 .vscode
 
 docs/_includes/_cmmcore_members.md
 docs/_includes/_cmmcore_table.md
 docs/_includes/_cmmcoreplus_members.md
 
-example_*.ome.tiff
+example_*.some.tiff
 example.zarr
```

### Comparing `pymmcore_plus-0.9.4/LICENSE` & `pymmcore_plus-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/README.md` & `pymmcore_plus-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.9.4/pyproject.toml` & `pymmcore_plus-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "pytest-qt >=4",
     "pytest >=7.3.2",
     "qtpy >=2",
     "rich",
     "typer >=0.4.2",
     "tifffile >=2021.6.14",
     "zarr >=2.2",
+    "xarray",
 ]
 dev = ["ipython", "mypy", "pdbpp", "pre-commit", "ruff"]
 docs = [
     "mkdocs >=1.4",
     "mkdocs-material",
     "mkdocstrings ==0.22.0",
     "mkdocstrings-python ==1.1.2",
```

### Comparing `pymmcore_plus-0.9.4/PKG-INFO` & `pymmcore_plus-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pymmcore-plus
-Version: 0.9.4
+Version: 0.9.5
 Summary: pymmcore superset providing improved APIs, event handling, and a pure python acquisition engine
 Project-URL: Source, https://github.com/pymmcore-plus/pymmcore-plus
 Project-URL: Tracker, https://github.com/pymmcore-plus/pymmcore-plus/issues
 Project-URL: Documentation, https://pymmcore-plus.github.io/pymmcore-plus
 Author-email: Talley Lambert <talley.lambert@gmail.com>, Federico Gasparoli <federico.gasparoli@gmail.com>, Ian Hunt-Isaak <ianhuntisaak@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -56,14 +56,15 @@
 Requires-Dist: pytest-cov>=4; extra == 'test'
 Requires-Dist: pytest-qt>=4; extra == 'test'
 Requires-Dist: pytest>=7.3.2; extra == 'test'
 Requires-Dist: qtpy>=2; extra == 'test'
 Requires-Dist: rich; extra == 'test'
 Requires-Dist: tifffile>=2021.6.14; extra == 'test'
 Requires-Dist: typer>=0.4.2; extra == 'test'
+Requires-Dist: xarray; extra == 'test'
 Requires-Dist: zarr>=2.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pymmcore-plus
 
 [![License](https://img.shields.io/pypi/l/pymmcore-plus.svg?color=green)](https://github.com/pymmcore-plus/pymmcore-plus/raw/master/LICENSE)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymmcore-plus)](https://pypi.org/project/pymmcore-plus)
```

