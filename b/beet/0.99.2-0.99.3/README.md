# Comparing `tmp/beet-0.99.2.tar.gz` & `tmp/beet-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beet-0.99.2.tar", max compression
+gzip compressed data, was "beet-0.99.3.tar", max compression
```

## Comparing `beet-0.99.2.tar` & `beet-0.99.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1073 2023-12-02 16:16:04.780528 beet-0.99.2/LICENSE
--rw-r--r--   0        0        0     6048 2023-12-02 16:16:04.780528 beet-0.99.2/README.md
--rw-r--r--   0        0        0      583 2023-12-02 16:16:23.708541 beet-0.99.2/beet/__init__.py
--rw-r--r--   0        0        0       44 2023-12-02 16:16:04.780528 beet-0.99.2/beet/__main__.py
--rw-r--r--   0        0        0        0 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/__init__.py
--rw-r--r--   0        0        0     3265 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/auto_yaml.py
--rw-r--r--   0        0        0     1369 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/autosave.py
--rw-r--r--   0        0        0     2480 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/babelbox.py
--rw-r--r--   0        0        0      574 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/clear.py
--rw-r--r--   0        0        0     3005 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/copy_files.py
--rw-r--r--   0        0        0     8040 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/dbg.py
--rw-r--r--   0        0        0      187 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/default.py
--rw-r--r--   0        0        0     1605 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/dundervar.py
--rw-r--r--   0        0        0      494 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/error_message.py
--rw-r--r--   0        0        0     1046 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/extra_files.py
--rw-r--r--   0        0        0     4280 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/find_replace.py
--rw-r--r--   0        0        0     1472 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/format_json.py
--rw-r--r--   0        0        0      890 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/function_header.py
--rw-r--r--   0        0        0     5701 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/hangman.py
--rw-r--r--   0        0        0     1932 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/inline_function.py
--rw-r--r--   0        0        0     1090 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     3811 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/installation_advancement.py
--rw-r--r--   0        0        0     1774 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/json_log.py
--rw-r--r--   0        0        0     5360 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/json_reporter.py
--rw-r--r--   0        0        0     2871 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/lantern_load.py
--rw-r--r--   0        0        0      816 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/line_endings.py
--rw-r--r--   0        0        0     5916 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/link.py
--rw-r--r--   0        0        0     6740 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/livereload.py
--rw-r--r--   0        0        0     2225 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/load.py
--rw-r--r--   0        0        0     4228 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/load_yaml.py
--rw-r--r--   0        0        0      567 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/log_level.py
--rw-r--r--   0        0        0     1587 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/messages.py
--rw-r--r--   0        0        0      337 2023-12-02 16:16:04.780528 beet-0.99.2/beet/contrib/minify_function.py
--rw-r--r--   0        0        0      235 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/minify_json.py
--rw-r--r--   0        0        0     1590 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/model_merging.py
--rw-r--r--   0        0        0     1591 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/optifine.py
--rw-r--r--   0        0        0      960 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/output.py
--rw-r--r--   0        0        0      956 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/relative_function_path.py
--rw-r--r--   0        0        0     5486 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/rename_files.py
--rw-r--r--   0        0        0     1158 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/render.py
--rw-r--r--   0        0        0      885 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/sandstone.py
--rw-r--r--   0        0        0      889 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/scoreboard.py
--rw-r--r--   0        0        0      811 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/stdin.py
--rw-r--r--   0        0        0     1357 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/strip_final_newlines.py
--rw-r--r--   0        0        0      155 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/template_context.py
--rw-r--r--   0        0        0      229 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/template_sandbox.py
--rw-r--r--   0        0        0      897 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/text_encoding.py
--rw-r--r--   0        0        0      775 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/unknown_files.py
--rw-r--r--   0        0        0     8170 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/vanilla.py
--rw-r--r--   0        0        0     5719 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/worldgen.py
--rw-r--r--   0        0        0     2436 2023-12-02 16:16:04.784528 beet-0.99.2/beet/contrib/yellow_shulker_box.py
--rw-r--r--   0        0        0        0 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/__init__.py
--rw-r--r--   0        0        0    11434 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/cache.py
--rw-r--r--   0        0        0     5956 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/container.py
--rw-r--r--   0        0        0      565 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/error.py
--rw-r--r--   0        0        0    21724 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/file.py
--rw-r--r--   0        0        0     8475 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/utils.py
--rw-r--r--   0        0        0     3711 2023-12-02 16:16:04.784528 beet-0.99.2/beet/core/watch.py
--rw-r--r--   0        0        0        0 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/__init__.py
--rw-r--r--   0        0        0    50474 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/base.py
--rw-r--r--   0        0        0    11769 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/data_pack.py
--rw-r--r--   0        0        0    11939 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/resource_pack.py
--rw-r--r--   0        0        0      529 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/test_utils.py
--rw-r--r--   0        0        0     1952 2023-12-02 16:16:04.784528 beet-0.99.2/beet/library/utils.py
--rw-r--r--   0        0        0       33 2023-12-02 16:16:04.784528 beet-0.99.2/beet/preset_stdin.yml
--rw-r--r--   0        0        0        0 2023-12-02 16:16:04.784528 beet-0.99.2/beet/py.typed
--rw-r--r--   0        0        0     4720 2023-12-02 16:16:04.784528 beet-0.99.2/beet/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/__init__.py
--rw-r--r--   0        0        0     8033 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/cli.py
--rw-r--r--   0        0        0     4600 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/commands.py
--rw-r--r--   0        0        0    15236 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/config.py
--rw-r--r--   0        0        0    10556 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/context.py
--rw-r--r--   0        0        0    11826 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/generator.py
--rw-r--r--   0        0        0     3484 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/helpers.py
--rw-r--r--   0        0        0     4355 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/pipeline.py
--rw-r--r--   0        0        0    13716 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/project.py
--rw-r--r--   0        0        0    24348 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/query.py
--rw-r--r--   0        0        0     6457 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/template.py
--rw-r--r--   0        0        0     3694 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/tree.py
--rw-r--r--   0        0        0     4636 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/utils.py
--rw-r--r--   0        0        0     9695 2023-12-02 16:16:04.784528 beet-0.99.2/beet/toolchain/worker.py
--rw-r--r--   0        0        0     2308 2023-12-02 16:16:23.740541 beet-0.99.2/pyproject.toml
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 beet-0.99.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-12-02 16:32:48.854032 beet-0.99.3/LICENSE
+-rw-r--r--   0        0        0     6048 2023-12-02 16:32:48.854032 beet-0.99.3/README.md
+-rw-r--r--   0        0        0      583 2023-12-02 16:33:11.314285 beet-0.99.3/beet/__init__.py
+-rw-r--r--   0        0        0       44 2023-12-02 16:32:48.854032 beet-0.99.3/beet/__main__.py
+-rw-r--r--   0        0        0        0 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/__init__.py
+-rw-r--r--   0        0        0     3265 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/auto_yaml.py
+-rw-r--r--   0        0        0     1369 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/autosave.py
+-rw-r--r--   0        0        0     2480 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/babelbox.py
+-rw-r--r--   0        0        0      574 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/clear.py
+-rw-r--r--   0        0        0     3005 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/copy_files.py
+-rw-r--r--   0        0        0     8040 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/dbg.py
+-rw-r--r--   0        0        0      187 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/default.py
+-rw-r--r--   0        0        0     1605 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/dundervar.py
+-rw-r--r--   0        0        0      494 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/error_message.py
+-rw-r--r--   0        0        0     1046 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/extra_files.py
+-rw-r--r--   0        0        0     4280 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/find_replace.py
+-rw-r--r--   0        0        0     1472 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/format_json.py
+-rw-r--r--   0        0        0      890 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/function_header.py
+-rw-r--r--   0        0        0     5701 2023-12-02 16:32:48.854032 beet-0.99.3/beet/contrib/hangman.py
+-rw-r--r--   0        0        0     1932 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/inline_function.py
+-rw-r--r--   0        0        0     1090 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     3811 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/installation_advancement.py
+-rw-r--r--   0        0        0     1774 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/json_log.py
+-rw-r--r--   0        0        0     5360 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/json_reporter.py
+-rw-r--r--   0        0        0     2871 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/lantern_load.py
+-rw-r--r--   0        0        0      816 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/line_endings.py
+-rw-r--r--   0        0        0     5916 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/link.py
+-rw-r--r--   0        0        0     6740 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/livereload.py
+-rw-r--r--   0        0        0     2225 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/load.py
+-rw-r--r--   0        0        0     4228 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/load_yaml.py
+-rw-r--r--   0        0        0      567 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/log_level.py
+-rw-r--r--   0        0        0     1587 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/messages.py
+-rw-r--r--   0        0        0      337 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/minify_function.py
+-rw-r--r--   0        0        0      235 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/minify_json.py
+-rw-r--r--   0        0        0     1590 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/model_merging.py
+-rw-r--r--   0        0        0     1591 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/optifine.py
+-rw-r--r--   0        0        0      960 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/output.py
+-rw-r--r--   0        0        0      956 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/relative_function_path.py
+-rw-r--r--   0        0        0     5486 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/rename_files.py
+-rw-r--r--   0        0        0     1158 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/render.py
+-rw-r--r--   0        0        0      885 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/sandstone.py
+-rw-r--r--   0        0        0      889 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/scoreboard.py
+-rw-r--r--   0        0        0      811 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/stdin.py
+-rw-r--r--   0        0        0     1357 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/strip_final_newlines.py
+-rw-r--r--   0        0        0      155 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/template_context.py
+-rw-r--r--   0        0        0      229 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/template_sandbox.py
+-rw-r--r--   0        0        0      897 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/text_encoding.py
+-rw-r--r--   0        0        0      775 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/unknown_files.py
+-rw-r--r--   0        0        0     8170 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/vanilla.py
+-rw-r--r--   0        0        0     5719 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/worldgen.py
+-rw-r--r--   0        0        0     2436 2023-12-02 16:32:48.858032 beet-0.99.3/beet/contrib/yellow_shulker_box.py
+-rw-r--r--   0        0        0        0 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/__init__.py
+-rw-r--r--   0        0        0    11434 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/cache.py
+-rw-r--r--   0        0        0     5956 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/container.py
+-rw-r--r--   0        0        0      565 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/error.py
+-rw-r--r--   0        0        0    21724 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/file.py
+-rw-r--r--   0        0        0     8475 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/utils.py
+-rw-r--r--   0        0        0     3711 2023-12-02 16:32:48.858032 beet-0.99.3/beet/core/watch.py
+-rw-r--r--   0        0        0        0 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/__init__.py
+-rw-r--r--   0        0        0    50474 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/base.py
+-rw-r--r--   0        0        0    11769 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/data_pack.py
+-rw-r--r--   0        0        0    11939 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/resource_pack.py
+-rw-r--r--   0        0        0      529 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/test_utils.py
+-rw-r--r--   0        0        0     1952 2023-12-02 16:32:48.858032 beet-0.99.3/beet/library/utils.py
+-rw-r--r--   0        0        0       33 2023-12-02 16:32:48.858032 beet-0.99.3/beet/preset_stdin.yml
+-rw-r--r--   0        0        0        0 2023-12-02 16:32:48.858032 beet-0.99.3/beet/py.typed
+-rw-r--r--   0        0        0     4720 2023-12-02 16:32:48.858032 beet-0.99.3/beet/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/__init__.py
+-rw-r--r--   0        0        0     8033 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/cli.py
+-rw-r--r--   0        0        0     4600 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/commands.py
+-rw-r--r--   0        0        0    15236 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/config.py
+-rw-r--r--   0        0        0    10556 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/context.py
+-rw-r--r--   0        0        0    11826 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/generator.py
+-rw-r--r--   0        0        0     3484 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/helpers.py
+-rw-r--r--   0        0        0     4355 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/pipeline.py
+-rw-r--r--   0        0        0    13716 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/project.py
+-rw-r--r--   0        0        0    24337 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/query.py
+-rw-r--r--   0        0        0     6457 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/template.py
+-rw-r--r--   0        0        0     3694 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/tree.py
+-rw-r--r--   0        0        0     4636 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/utils.py
+-rw-r--r--   0        0        0     9695 2023-12-02 16:32:48.858032 beet-0.99.3/beet/toolchain/worker.py
+-rw-r--r--   0        0        0     2308 2023-12-02 16:33:11.342285 beet-0.99.3/pyproject.toml
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 beet-0.99.3/PKG-INFO
```

### Comparing `beet-0.99.2/LICENSE` & `beet-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/README.md` & `beet-0.99.3/README.md`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/__init__.py` & `beet-0.99.3/beet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.99.2"
+__version__ = "0.99.3"
 
 
 from .core.cache import *
 from .core.container import *
 from .core.error import *
 from .core.file import *
 from .core.watch import *
```

### Comparing `beet-0.99.2/beet/contrib/auto_yaml.py` & `beet-0.99.3/beet/contrib/auto_yaml.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/autosave.py` & `beet-0.99.3/beet/contrib/autosave.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/babelbox.py` & `beet-0.99.3/beet/contrib/babelbox.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/clear.py` & `beet-0.99.3/beet/contrib/clear.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/copy_files.py` & `beet-0.99.3/beet/contrib/copy_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/dbg.py` & `beet-0.99.3/beet/contrib/dbg.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/dundervar.py` & `beet-0.99.3/beet/contrib/dundervar.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/extra_files.py` & `beet-0.99.3/beet/contrib/extra_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/find_replace.py` & `beet-0.99.3/beet/contrib/find_replace.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/format_json.py` & `beet-0.99.3/beet/contrib/format_json.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/function_header.py` & `beet-0.99.3/beet/contrib/function_header.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/hangman.py` & `beet-0.99.3/beet/contrib/hangman.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/inline_function.py` & `beet-0.99.3/beet/contrib/inline_function.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/inline_function_tag.py` & `beet-0.99.3/beet/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/installation_advancement.py` & `beet-0.99.3/beet/contrib/installation_advancement.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/json_log.py` & `beet-0.99.3/beet/contrib/json_log.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/json_reporter.py` & `beet-0.99.3/beet/contrib/json_reporter.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/lantern_load.py` & `beet-0.99.3/beet/contrib/lantern_load.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/line_endings.py` & `beet-0.99.3/beet/contrib/line_endings.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/link.py` & `beet-0.99.3/beet/contrib/link.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/livereload.py` & `beet-0.99.3/beet/contrib/livereload.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/load.py` & `beet-0.99.3/beet/contrib/load.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/load_yaml.py` & `beet-0.99.3/beet/contrib/load_yaml.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/log_level.py` & `beet-0.99.3/beet/contrib/log_level.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/messages.py` & `beet-0.99.3/beet/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/model_merging.py` & `beet-0.99.3/beet/contrib/model_merging.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/optifine.py` & `beet-0.99.3/beet/contrib/optifine.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/output.py` & `beet-0.99.3/beet/contrib/output.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/relative_function_path.py` & `beet-0.99.3/beet/contrib/relative_function_path.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/rename_files.py` & `beet-0.99.3/beet/contrib/rename_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/render.py` & `beet-0.99.3/beet/contrib/render.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/sandstone.py` & `beet-0.99.3/beet/contrib/sandstone.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/scoreboard.py` & `beet-0.99.3/beet/contrib/scoreboard.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/stdin.py` & `beet-0.99.3/beet/contrib/stdin.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/strip_final_newlines.py` & `beet-0.99.3/beet/contrib/strip_final_newlines.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/text_encoding.py` & `beet-0.99.3/beet/contrib/text_encoding.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/unknown_files.py` & `beet-0.99.3/beet/contrib/unknown_files.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/vanilla.py` & `beet-0.99.3/beet/contrib/vanilla.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/worldgen.py` & `beet-0.99.3/beet/contrib/worldgen.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/contrib/yellow_shulker_box.py` & `beet-0.99.3/beet/contrib/yellow_shulker_box.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/cache.py` & `beet-0.99.3/beet/core/cache.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/container.py` & `beet-0.99.3/beet/core/container.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/error.py` & `beet-0.99.3/beet/core/error.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/file.py` & `beet-0.99.3/beet/core/file.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/utils.py` & `beet-0.99.3/beet/core/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/core/watch.py` & `beet-0.99.3/beet/core/watch.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/library/base.py` & `beet-0.99.3/beet/library/base.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/library/data_pack.py` & `beet-0.99.3/beet/library/data_pack.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/library/resource_pack.py` & `beet-0.99.3/beet/library/resource_pack.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/library/test_utils.py` & `beet-0.99.3/beet/library/test_utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/library/utils.py` & `beet-0.99.3/beet/library/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/pytest_plugin.py` & `beet-0.99.3/beet/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/cli.py` & `beet-0.99.3/beet/toolchain/cli.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/commands.py` & `beet-0.99.3/beet/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/config.py` & `beet-0.99.3/beet/toolchain/config.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/context.py` & `beet-0.99.3/beet/toolchain/context.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/generator.py` & `beet-0.99.3/beet/toolchain/generator.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/helpers.py` & `beet-0.99.3/beet/toolchain/helpers.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/pipeline.py` & `beet-0.99.3/beet/toolchain/pipeline.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/project.py` & `beet-0.99.3/beet/toolchain/project.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/query.py` & `beet-0.99.3/beet/toolchain/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,24 +30,24 @@
     Any,
     Dict,
     Generic,
     List,
     Literal,
     Mapping,
     Optional,
+    Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_origin,
     overload,
 )
 
-from git import Sequence
 from pathspec import PathSpec
 from pathspec.patterns.gitwildmatch import GitWildMatchPattern
 from pydantic.v1 import BaseModel, validator
 
 from beet.core.file import File
 from beet.library.base import NamespaceFile, Pack, create_group_map
```

### Comparing `beet-0.99.2/beet/toolchain/template.py` & `beet-0.99.3/beet/toolchain/template.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/tree.py` & `beet-0.99.3/beet/toolchain/tree.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/utils.py` & `beet-0.99.3/beet/toolchain/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/beet/toolchain/worker.py` & `beet-0.99.3/beet/toolchain/worker.py`

 * *Files identical despite different names*

### Comparing `beet-0.99.2/pyproject.toml` & `beet-0.99.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beet"
-version = "0.99.2"
+version = "0.99.3"
 description = "The Minecraft pack development kit"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/beet"
 repository = "https://github.com/mcbeet/beet"
 documentation = "https://github.com/mcbeet/beet"
```

### Comparing `beet-0.99.2/PKG-INFO` & `beet-0.99.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beet
-Version: 0.99.2
+Version: 0.99.3
 Summary: The Minecraft pack development kit
 Home-page: https://github.com/mcbeet/beet
 License: MIT
 Keywords: beet,minecraft,datapack,resourcepack,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
```

