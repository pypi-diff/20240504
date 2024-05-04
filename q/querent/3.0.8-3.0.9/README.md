# Comparing `tmp/querent-3.0.8.tar.gz` & `tmp/querent-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.8.tar", last modified: Sun Apr 28 02:03:47 2024, max compression
+gzip compressed data, was "querent-3.0.9.tar", last modified: Sat May  4 17:16:42 2024, max compression
```

## Comparing `querent-3.0.8.tar` & `querent-3.0.9.tar`

### file list

```diff
@@ -1,260 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.230068 querent-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-28 01:59:19.000000 querent-3.0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-28 02:03:47.230068 querent-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-28 01:59:19.000000 querent-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.162068 querent-3.0.8/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-28 01:59:19.000000 querent-3.0.8/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.166068 querent-3.0.8/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-28 01:59:19.000000 querent-3.0.8/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 01:59:19.000000 querent-3.0.8/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.166068 querent-3.0.8/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-28 01:59:19.000000 querent-3.0.8/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.166068 querent-3.0.8/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.166068 querent-3.0.8/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.166068 querent-3.0.8/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.170068 querent-3.0.8/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-28 01:59:19.000000 querent-3.0.8/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.174068 querent-3.0.8/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.182068 querent-3.0.8/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 01:59:19.000000 querent-3.0.8/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.182068 querent-3.0.8/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.182068 querent-3.0.8/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.186068 querent-3.0.8/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-28 01:59:19.000000 querent-3.0.8/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-28 01:59:19.000000 querent-3.0.8/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.190068 querent-3.0.8/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.194068 querent-3.0.8/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-28 01:59:19.000000 querent-3.0.8/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.198068 querent-3.0.8/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.198068 querent-3.0.8/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.198068 querent-3.0.8/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.198068 querent-3.0.8/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.198068 querent-3.0.8/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.202068 querent-3.0.8/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.202068 querent-3.0.8/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.202068 querent-3.0.8/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.202068 querent-3.0.8/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.202068 querent-3.0.8/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-28 01:59:19.000000 querent-3.0.8/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.206068 querent-3.0.8/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.210068 querent-3.0.8/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.214068 querent-3.0.8/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-28 01:59:19.000000 querent-3.0.8/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.218068 querent-3.0.8/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 01:59:19.000000 querent-3.0.8/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-28 01:59:19.000000 querent-3.0.8/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 01:59:19.000000 querent-3.0.8/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-28 01:59:19.000000 querent-3.0.8/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.218068 querent-3.0.8/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.222068 querent-3.0.8/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 01:59:19.000000 querent-3.0.8/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.222068 querent-3.0.8/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-28 01:59:19.000000 querent-3.0.8/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-28 01:59:19.000000 querent-3.0.8/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-28 01:59:19.000000 querent-3.0.8/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.226068 querent-3.0.8/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-28 01:59:19.000000 querent-3.0.8/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-28 01:59:19.000000 querent-3.0.8/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-28 01:59:19.000000 querent-3.0.8/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.226068 querent-3.0.8/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-28 01:59:19.000000 querent-3.0.8/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-28 01:59:19.000000 querent-3.0.8/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-28 01:59:19.000000 querent-3.0.8/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-28 01:59:19.000000 querent-3.0.8/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.226068 querent-3.0.8/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-28 01:59:19.000000 querent-3.0.8/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.226068 querent-3.0.8/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:59:19.000000 querent-3.0.8/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-28 01:59:19.000000 querent-3.0.8/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.230068 querent-3.0.8/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 01:59:19.000000 querent-3.0.8/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-28 01:59:19.000000 querent-3.0.8/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-28 01:59:19.000000 querent-3.0.8/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:03:47.230068 querent-3.0.8/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-28 02:03:47.000000 querent-3.0.8/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-28 02:03:47.000000 querent-3.0.8/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:03:47.000000 querent-3.0.8/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-28 02:03:47.000000 querent-3.0.8/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 02:03:47.000000 querent-3.0.8/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:03:47.230068 querent-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-28 01:59:19.000000 querent-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-04 17:12:08.000000 querent-3.0.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-04 17:16:42.203027 querent-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-04 17:12:08.000000 querent-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-04 17:12:08.000000 querent-3.0.9/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-04 17:12:08.000000 querent-3.0.9/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.147027 querent-3.0.9/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.147027 querent-3.0.9/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18047 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18879 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.167027 querent-3.0.9/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.167027 querent-3.0.9/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.183027 querent-3.0.9/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18240 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.187027 querent-3.0.9/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.195027 querent-3.0.9/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-04 17:12:08.000000 querent-3.0.9/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-04 17:12:08.000000 querent-3.0.9/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 17:16:42.203027 querent-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-04 17:12:08.000000 querent-3.0.9/setup.py
```

### Comparing `querent-3.0.8/LICENCE` & `querent-3.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/PKG-INFO` & `querent-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.8
+Version: 3.0.9
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -72,14 +72,15 @@
 Requires-Dist: newsapi-python==0.2.7
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==1.13.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: pdfminer==20191125
+Requires-Dist: pdfplumber==0.10.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: prometheus-client==0.17.1
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pybase64==1.3.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydub==0.25.1
 Requires-Dist: pyjwt==2.4.0
```

### Comparing `querent-3.0.8/README.md` & `querent-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/__init__.py` & `querent-3.0.9/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/callback/event_callback_dispatcher.py` & `querent-3.0.9/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/callback/event_callback_interface.py` & `querent-3.0.9/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/channel/channel_interface.py` & `querent-3.0.9/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/aws/aws_collector.py` & `querent-3.0.9/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/azure/azure_collector.py` & `querent-3.0.9/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/collector_errors.py` & `querent-3.0.9/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/collector_factory.py` & `querent-3.0.9/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/collector_resolver.py` & `querent-3.0.9/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.9/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.9/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/email/email_collector.py` & `querent-3.0.9/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/email/imap.py` & `querent-3.0.9/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/fs/fs_collector.py` & `querent-3.0.9/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.9/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/github/github_collector.py` & `querent-3.0.9/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/jira/jira_collector.py` & `querent-3.0.9/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/news/news_collector.py` & `querent-3.0.9/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/slack/slack_collector.py` & `querent-3.0.9/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.9/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/common_errors.py` & `querent-3.0.9/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/errors/metric_errors.py` & `querent-3.0.9/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/collected_bytes.py` & `querent-3.0.9/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/file_buffer.py` & `querent-3.0.9/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/ingested_code.py` & `querent-3.0.9/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/ingested_images.py` & `querent-3.0.9/querent/common/types/ingested_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class IngestedImages:
     def __init__(
         self,
         file: str,
         image: str,
         image_name: str,
         page_num: int,
-        text: [str],
+        text: [str], # type: ignore
         coordinates: list = [],
         ocr_text: list = [],
         error: str = None,
         doc_source = str,
     ) -> None:
         self.file = file
         self.text = text
```

### Comparing `querent-3.0.8/querent/common/types/ingested_messages.py` & `querent-3.0.9/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/ingested_tokens.py` & `querent-3.0.9/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/types/querent_queue.py` & `querent-3.0.9/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/common/uri.py` & `querent-3.0.9/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/collector/collector_config.py` & `querent-3.0.9/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/config.py` & `querent-3.0.9/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/core/gpt_llm_config.py` & `querent-3.0.9/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/core/llm_config.py` & `querent-3.0.9/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/core/opensource_llm_config.py` & `querent-3.0.9/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/engine/engine_config.py` & `querent-3.0.9/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/graph_config.py` & `querent-3.0.9/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/ingestor/ingestor_config.py` & `querent-3.0.9/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/metric/prometheus.py` & `querent-3.0.9/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/resource/resource_config.py` & `querent-3.0.9/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/config/workflow/workflow_config.py` & `querent-3.0.9/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/core/base_engine.py` & `querent-3.0.9/querent/core/base_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 import asyncio
+import time
 from querent.callback.event_callback_dispatcher import EventCallbackDispatcher
 from querent.callback.event_callback_interface import EventCallbackInterface
 from querent.common.types.ingested_images import IngestedImages
 from querent.common.types.ingested_messages import IngestedMessages
+from querent.common.types.ingested_table import IngestedTables
 from querent.common.types.ingested_tokens import IngestedTokens
 from querent.common.types.ingested_code import IngestedCode
 from querent.common.types.querent_event import EventState, EventType
 from querent.common.types.querent_queue import QuerentQueue
 from querent.config.engine.engine_config import EngineConfig
 from querent.logging.logger import setup_logger
 from querent.common.types.ingested_images import IngestedImages
@@ -117,14 +119,26 @@
         Returns:
             EventState: The state of the event is set with the event type and the timestamp
             of the event and set using `self.set_state(event_state)`.
         """
         raise NotImplementedError
 
     @abstractmethod
+    async def process_tables(self, data: IngestedTables):
+        """
+        Process tables asynchronously.
+        Args:
+            data (IngestedTables): The input data to process.
+        Returns:
+            EventState: The state of the event is set with the event type and the timestamp
+            of the event and set using `self.set_state(event_state)`.
+        """
+        pass
+
+    @abstractmethod
     async def process_images(self, data: IngestedImages):
         """
         Process image files asynchronously.
         Args:
             data (IngestedImage): The input data to process.
         Returns:
             EventState: The state of the event is set with the event type and the timestamp
@@ -173,23 +187,26 @@
         The following methods enables independent processing of tokens and messages.
     """
 
     async def _listen_for_state_changes(self):
         while not self.state_queue.empty() or not self.termination_event.is_set():
             new_state = await self.state_queue.get()
             if isinstance(new_state, EventState):
+                image_id = new_state.image_id
                 if new_state.payload == "Terminate":
                     break
                 new_state = {
                     "event_type": str(new_state.event_type),
                     "timestamp": new_state.timestamp,
                     "payload": new_state.payload,
                     "file": new_state.file,
                     "doc_source": new_state.doc_source,
                 }
+                if image_id is not None:
+                    new_state["image_id"] = image_id
                 await self._notify_subscribers(new_state["event_type"], new_state)
             else:
                 raise Exception(
                     f"Bad state type {type(new_state)} for {self.__class__.__name__}. Supported type: {EventState}"
                 )
             await self.state_queue.task_done()
                 
@@ -228,24 +245,27 @@
                             await self.process_messages(data)
                         elif isinstance(data, IngestedTokens):
                             await self.process_tokens(data)
                         elif isinstance(data, IngestedImages):
                             await self.process_images(data)
                         elif isinstance(data, IngestedCode):
                             await self.process_code(data)
+                        elif isinstance(data, IngestedTables):
+                            continue
+                            # await self.process_tables(data)
                         elif data is None:
                             none_counter += 1
                             if none_counter >= 2:
                                 self.termination_event.set()
-                                current_state = EventState(EventType.Terminate,1.0, "Terminate", "temp.txt")
+                                current_state = EventState(EventType.Terminate,time.time(), "Terminate", "temp.txt")
                                 await self.set_state(new_state=current_state)
 
                         else:
                             raise Exception(
-                                f"Invalid data type {type(data)} for {self.__class__.__name__}. Supported type: {IngestedTokens, IngestedMessages}"
+                                f"Invalid data type {type(data)} for {self.__class__.__name__}. Supported type: {IngestedTokens, IngestedMessages, IngestedTables, IngestedImages}"
                             )
                     except Exception as e:
                         self.logger.error(
                             f"Error processing tokens: {e}. Retrying ({retries}/{self.max_retries})"
                         )
                         retries += 1
```

### Comparing `querent-3.0.8/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.9/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import json
+import re
 from transformers import AutoTokenizer
+import time
+
+import unidecode
+from querent.common.types.ingested_table import IngestedTables
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.common.types.ingested_images import IngestedImages
 from querent.config.core.opensource_llm_config import Opensource_LLM_Config
 from querent.core.transformers.relationship_extraction_llm import RelationExtractor
 from querent.kg.rel_helperfunctions.contextual_predicate import process_data
 from querent.kg.ner_helperfunctions.contextual_embeddings import EntityEmbeddingExtractor
 from querent.kg.ner_helperfunctions.fixed_entities import FixedEntityExtractor
@@ -109,16 +114,85 @@
 
     def validate(self) -> bool:
         return self.ner_model is not None and self.ner_tokenizer is not None
 
     def process_messages(self, data: IngestedMessages):
         return super().process_messages(data)
     
-    def process_images(self, data: IngestedImages):
-        return super().process_images(data)
+    @staticmethod
+    def validate_ingested_images(data: IngestedImages) -> bool:
+        if data.is_error():
+            
+            return False
+
+        return True
+    async def process_images(self, data: IngestedImages):
+        content = ""
+        doc_entity_pairs = []
+        doc_entity_pairs_ocr = []
+        entity_ocr = []
+        results = []
+        blob = data.image
+        try:
+            doc_source = data.doc_source
+            if not BERTLLM.validate_ingested_images(data):
+                self.set_termination_event()                                      
+                return
+            if data.ocr_text:
+                ocr_text = ' '.join(data.ocr_text)
+            if data.text:
+                content = ' '.join(data.text)
+            file = data.file
+            ocr_content = ocr_text
+            if ocr_content or content:
+                (entity_ocr, doc_entity_pairs_ocr) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
+                                                                                                  content=ocr_content,
+                                                                                                  fixed_entities=self.fixed_entities,
+                                                                                                  sample_entities=self.sample_entities)
+                if len(doc_entity_pairs_ocr) >= 1:
+                    results = doc_entity_pairs_ocr
+                elif len(doc_entity_pairs_ocr) == 0:
+                    if content:
+                        if self.fixed_entities:
+                            content = self.entity_context_extractor.find_entity_sentences(content)
+                        (_, doc_entity_pairs) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
+                                                                                                  content=content,
+                                                                                                  fixed_entities=self.fixed_entities,
+                                                                                                  sample_entities=self.sample_entities)
+                        if len(doc_entity_pairs) > 0 and len(entity_ocr) >=1:
+                            results = [self.ner_llm_instance.filter_matching_entities(doc_entity_pairs, entity_ocr)]
+                        elif len(doc_entity_pairs) > 0 and len(entity_ocr) == 0:
+                            results = doc_entity_pairs
+                    else:
+                        return        
+                if len(results) > 0:
+                    doc_entity_pairs = self.ner_llm_instance.remove_duplicates(results)
+                    filtered_triples = process_data(doc_entity_pairs, file)
+                    if self.skip_inferences:
+                        return filtered_triples, file, self.ner_llm_instance
+                    else:
+                        unique_id = str(hash(data.image))
+                        for triple in filtered_triples:
+                            if not self.termination_event.is_set():
+                                updated_tuple = self.ner_llm_instance.final_ingested_images_tuples(triple, create_embeddings=self.create_emb)
+                                graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(updated_tuple))
+                                if graph_json:
+                                    current_state = EventState(event_type=EventType.Graph, timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source, image_id=unique_id)
+                                    await self.set_state(new_state=current_state)
+                                vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(updated_tuple, blob))
+                                if vector_json:
+                                    current_state = EventState(event_type=EventType.Vector, timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source, image_id=unique_id)
+                                    await self.set_state(new_state=current_state)
+            else:
+                return        
+        except Exception as e:
+            self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to process tokens. {e}")
+    
+    async def process_tables(self, data: IngestedTables):
+        return super().process_tables(data)
 
     async def process_code(self, data: IngestedCode):
         return super().process_code(data)
 
     @staticmethod
     def validate_ingested_tokens(data: IngestedTokens) -> bool:
         if data.is_error():
@@ -140,43 +214,40 @@
             self.triple_filter.set_params(**kwargs)
         else:
             self.triple_filter = TripleFilter(**kwargs)
     
     
     async def process_tokens(self, data: IngestedTokens):
         doc_entity_pairs = []
-        number_sentences = 0
         try:
             doc_source = data.doc_source
             if not BERTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
                 single_string = ' '.join(data.data)
-                # clean_text = unidecode(single_string)
                 clean_text = single_string
+                
             else:
                 clean_text = data.data
             if not data.is_token_stream : 
                 file, content = self.file_buffer.add_chunk(
                 data.get_file_path(), clean_text)
             else:
                 content = clean_text
                 file = data.get_file_path()
             if content:
                 if self.fixed_entities:
                     content = self.entity_context_extractor.find_entity_sentences(content)
                 if self.fixed_relationships:
                     content = self.predicate_context_extractor.find_predicate_sentences(content)
-                tokens = self.ner_llm_instance._tokenize_and_chunk(content)
-                for tokenized_sentence, original_sentence, sentence_idx in tokens:
-                    (entities, entity_pairs,) = self.ner_llm_instance.extract_entities_from_sentence(original_sentence, sentence_idx, [s[1] for s in tokens],self.isConfinedSearch, self.fixed_entities, self.sample_entities)
-                    if entity_pairs:
-                        doc_entity_pairs.append(self.ner_llm_instance.transform_entity_pairs(entity_pairs))
-                    number_sentences = number_sentences + 1
+                (_, doc_entity_pairs) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
+                                                                                                  content=content,
+                                                                                                  fixed_entities=self.fixed_entities,
+                                                                                                  sample_entities=self.sample_entities)
             else:
                 return
             if self.sample_entities:
                 doc_entity_pairs = self.entity_context_extractor.process_entity_types(doc_entities=doc_entity_pairs)
             if doc_entity_pairs and any(doc_entity_pairs):
                 doc_entity_pairs = self.ner_llm_instance.remove_duplicates(doc_entity_pairs)
                 pairs_withattn = self.attn_scores_instance.extract_and_append_attention_weights(doc_entity_pairs)
@@ -208,19 +279,19 @@
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
+                                    current_state = EventState(event_type=EventType.Graph, timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                                 if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
+                                    current_state = EventState(event_type=EventType.Vector, timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                             else:
                                 return
                     else:
                         return
                 else:
                     return filtered_triples, file
```

### Comparing `querent-3.0.8/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.9/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 from transformers import AutoTokenizer
+import time
+from querent.common.types.ingested_table import IngestedTables
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.common.types.ingested_images import IngestedImages
 from querent.config.core.opensource_llm_config import Opensource_LLM_Config
 from querent.core.transformers.relationship_extraction_llm import RelationExtractor
 from querent.kg.rel_helperfunctions.contextual_predicate import process_data
 from querent.kg.ner_helperfunctions.fixed_entities import FixedEntityExtractor
 from querent.kg.ner_helperfunctions.ner_llm_transformer import NER_LLM
@@ -89,46 +91,42 @@
 
     def validate(self) -> bool:
         return self.ner_tokenizer is not None
 
     def process_messages(self, data: IngestedMessages):
         return super().process_messages(data)
     
-    def process_images(self, data: IngestedImages):
-        return super().process_images(data)
+    def process_tables(self, data: IngestedTables):
+        pass
+
+    async def process_images(self, data: IngestedImages):
+        pass
 
     async def process_code(self, data: IngestedCode):
         return super().process_code(data)
 
     @staticmethod
     def validate_ingested_tokens(data: IngestedTokens) -> bool:
         if data.is_error():
             
             return False
 
         return True
-
-    def count_entity_pairs(self, doc_entity_pairs):
-        total_pairs = 0
-        for inner_list in doc_entity_pairs:
-            total_pairs += len(inner_list)
-            
-        return total_pairs
     
-    def set_filter_params(self, **kwargs):
-        self.filter_params = kwargs
-        if self.triple_filter:
-            self.triple_filter.set_params(**kwargs)
-        else:
-            self.triple_filter = TripleFilter(**kwargs)
+    @staticmethod
+    def validate_ingested_images(data: IngestedImages) -> bool:
+        if data.is_error():
+            
+            return False
+
+        return True
     
     
     async def process_tokens(self, data: IngestedTokens):
         doc_entity_pairs = []
-        number_sentences = 0
         try:
             doc_source = data.doc_source
             if not Fixed_Entities_LLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
                 single_string = ' '.join(data.data)
@@ -143,20 +141,18 @@
                 content = clean_text
                 file = data.get_file_path()
             if content:
                 if self.fixed_entities:
                     content = self.entity_context_extractor.find_entity_sentences(content)
                 if self.fixed_relationships:
                     content = self.predicate_context_extractor.find_predicate_sentences(content)
-                tokens = self.ner_llm_instance._tokenize_and_chunk(content)
-                for tokenized_sentence, original_sentence, sentence_idx in tokens:
-                    (entities, entity_pairs,) = self.ner_llm_instance.extract_entities_from_sentence(original_sentence, sentence_idx, [s[1] for s in tokens],self.isConfinedSearch, self.fixed_entities, self.sample_entities)
-                    if entity_pairs:
-                        doc_entity_pairs.append(self.ner_llm_instance.transform_entity_pairs(entity_pairs))
-                    number_sentences = number_sentences + 1
+                (_, doc_entity_pairs) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
+                                                                                                  content=content,
+                                                                                                  fixed_entities=self.fixed_entities,
+                                                                                                  sample_entities=self.sample_entities)
             else:
                 return
             if self.sample_entities:
                 doc_entity_pairs = self.entity_context_extractor.process_entity_types(doc_entities=doc_entity_pairs)
             if doc_entity_pairs and any(doc_entity_pairs):
                 doc_entity_pairs = self.ner_llm_instance.remove_duplicates(doc_entity_pairs)
                 filtered_triples = process_data(doc_entity_pairs, file)
@@ -170,19 +166,19 @@
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
+                                    current_state = EventState(event_type=EventType.Graph,timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                                 if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
+                                    current_state = EventState(event_type=EventType.Vector, timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                             else:
                                 return
                     else:
                         return
                 else:
                     return filtered_triples, file
```

### Comparing `querent-3.0.8/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.9/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import json
+import re
+import time
+from querent.common.types.ingested_table import IngestedTables
 from querent.core.transformers.fixed_entities_set_opensourcellm import Fixed_Entities_LLM
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.config.core.gpt_llm_config import GPTConfig
 from querent.core.transformers.bert_ner_opensourcellm import BERTLLM
 from querent.common.types.ingested_images import IngestedImages
 from querent.kg.ner_helperfunctions.ner_llm_transformer import NER_LLM
 from querent.kg.rel_helperfunctions.openai_functions import FunctionRegistry
@@ -73,14 +76,18 @@
             else:
                 self.predicate_context_extractor = None
             self.create_emb = EmbeddingStore()
             if config.is_confined_search:
                 self.llm_instance = Fixed_Entities_LLM(input_queue, llm_config, self.create_emb)
             else :
                 self.llm_instance = BERTLLM(input_queue, llm_config, self.create_emb)
+            if not isinstance (self.llm_instance, BERTLLM):
+                self.process_image_instance = BERTLLM(input_queue, llm_config, self.create_emb)
+            else:
+                self.process_image_instance = self.llm_instance
             self.rel_model_name = config.rel_model_name
             if config.openai_api_key:
                 self.gpt_llm = OpenAI(api_key=config.openai_api_key)
             else:
                 self.gpt_llm = OpenAI()
             self.function_registry = FunctionRegistry()
             
@@ -90,27 +97,61 @@
     
     def validate(self) -> bool:
         return isinstance(self.llm_instance, BERTLLM) or isinstance(self.llm_instance, Fixed_Entities_LLM)
 
     def process_messages(self, data: IngestedMessages):
         return super().process_messages(data)
     
-    def process_images(self, data: IngestedImages):
-        return super().process_messages(data)
+    async def process_images(self, data: IngestedImages):
+        try:
+            if not GPTLLM.validate_ingested_images(data):
+                    self.set_termination_event()                    
+                    return 
+            blob = data.image
+            unique_id = str(hash(data.image))
+            doc_source = data.doc_source
+            result = await self.process_image_instance.process_images(data)  
+            if not result: return 
+            else:
+                filtered_triples, file, ner_instance = result
+                for triple in filtered_triples:
+                    updated_tuple = ner_instance.final_ingested_images_tuples(triple, create_embeddings=self.create_emb)
+                    graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(updated_tuple))
+                    if graph_json:
+                        current_state = EventState(event_type=EventType.Graph, timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source, image_id=unique_id)
+                        await self.set_state(new_state=current_state)
+                    vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(updated_tuple, blob))
+                    if vector_json:
+                        current_state = EventState(event_type=EventType.Vector, timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source, image_id=unique_id)
+                        await self.set_state(new_state=current_state)
+
+        except Exception as e:
+            self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to process tokens. {e}")
 
     async def process_code(self, data: IngestedCode):
         return super().process_messages(data)
+    
+    async def process_tables(self, data: IngestedTables):
+        return super().process_tables(data)
 
     @staticmethod
     def validate_ingested_tokens(data: IngestedTokens) -> bool:
         if data.is_error():
             
             return False
 
         return True
+    
+    @staticmethod
+    def validate_ingested_images(data: IngestedImages) -> bool:
+        if data.is_error():
+            
+            return False
+
+        return True
     def extract_semantic_triples(self, chat_completion):
     # Extract the message content from the ChatCompletion
         message_content = chat_completion.choices[0].message.content.replace('\n', '')
 
         # Parse the JSON content into a Python list
         try:
             triples_list = eval(message_content)
@@ -249,15 +290,14 @@
         return output_tuple
       
     async def process_tokens(self, data: IngestedTokens):
         try:
             if not GPTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                    
                     return 
-            
             doc_source = data.doc_source
             relationships = []
             result = await self.llm_instance.process_tokens(data)
             if not result: return 
             else:
                 filtered_triples, file = result
                 modified_data = GPTLLM.remove_items_from_tuples(filtered_triples)
@@ -270,26 +310,24 @@
                     entity2_nn_chunk = context_data.get("entity2_nn_chunk","")
                     result = await self.process_triples(context, entity1_nn_chunk, entity2_nn_chunk, entity1_label, entity2_label)
                     if result:
                         output_tuple = self.generate_output_tuple(result, context_json)
                         relationships.append(output_tuple)
                 if len(relationships) > 0:
                     embedding_triples = self.create_emb.generate_embeddings(relationships)
-                    if self.sample_relationships:
-                            embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                     for triple in embedding_triples:
                         if not self.termination_event.is_set():
                             graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                             if graph_json:
-                                    current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
-                                    await self.set_state(new_state=current_state)
+                                current_state = EventState(event_type=EventType.Graph,timestamp = time.time(), payload= graph_json, file=file, doc_source=doc_source)
+                                await self.set_state(new_state=current_state)
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                             if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
-                                    await self.set_state(new_state=current_state)
+                                current_state = EventState(event_type=EventType.Vector,timestamp=time.time(), payload = vector_json, file=file, doc_source=doc_source)
+                                await self.set_state(new_state=current_state)
                         else:
                             return
         except Exception as e:
             self.logger.error(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT. {e}")
             raise Exception(f"An error occurred while extracting predicates using GPT: {e}")
 
     async def process_messages(self, data: IngestedMessages):
```

### Comparing `querent-3.0.8/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.9/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 from unidecode import unidecode
+import time
 
 
 import spacy
 from querent.config.core.gpt_llm_config import GPTConfig
 from querent.common.types.ingested_images import IngestedImages
 from querent.kg.rel_helperfunctions.openai_functions import FunctionRegistry
 from querent.common.types.querent_event import EventState, EventType
@@ -242,22 +243,22 @@
                         final_triples.extend(relevant_triples)
                 final_triples = self.remove_duplicate_triplets(final_triples)
                 if len(final_triples) > 0:
                     for triple in final_triples:
                         if not self.termination_event.is_set():
                             graph_json = json.dumps(triple)
                             if graph_json:
-                                current_state = EventState(EventType.Graph,1.0, graph_json, file, doc_source=doc_source)
+                                current_state = EventState(event_type=EventType.Graph,timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source)
                                 await self.set_state(new_state=current_state)
                             context_embeddings = self.create_emb.get_embeddings([triple['sentence']])[0]
                             triple['context_embeddings'] = context_embeddings
                             triple['context'] = triple['sentence']
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson((triple['subject'],json.dumps(triple), triple['object'])))
                             if vector_json:
-                                    current_state = EventState(EventType.Vector,1.0, vector_json, file, doc_source=doc_source)
+                                    current_state = EventState(event_type=EventType.Vector,timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                         else:
                             return
 
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT NER LLM class. {e}")
```

### Comparing `querent-3.0.8/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.9/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/errors.py` & `querent-3.0.9/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/graph.py` & `querent-3.0.9/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/graph_namespace.py` & `querent-3.0.9/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/ontology.py` & `querent-3.0.9/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/schema.py` & `querent-3.0.9/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/shacl.py` & `querent-3.0.9/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/subject.py` & `querent-3.0.9/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/graph/utils.py` & `querent-3.0.9/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.9/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/base_ingestor.py` & `querent-3.0.9/querent/ingestors/base_ingestor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from abc import abstractmethod
+from PIL import Image
+import io
 from typing import AsyncGenerator, List
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common.types.ingested_tokens import IngestedTokens
 from querent.processors.async_processor import AsyncProcessor
 
 
 class BaseIngestor:
@@ -16,7 +18,18 @@
         # Your common ingestion logic here
         raise NotImplementedError
 
     @abstractmethod
     async def process_data(self, text):
         # Your common data processing logic here
         raise NotImplementedError
+
+    async def analyze_image(self, image):
+
+        width, height = image.size
+        min_dimension = 100
+
+        # Check if image meets the criteria
+        if width < min_dimension and height < min_dimension:
+            return False
+        else:
+            return True
```

### Comparing `querent-3.0.8/querent/ingestors/code/code_ingestor.py` & `querent-3.0.9/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.9/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.9/querent/ingestors/doc/doc_ingestor.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from docx import Document
 import pytextract
 import base64
 import pytesseract
 import uuid
 from PIL import Image
+from querent.common.types.ingested_table import IngestedTables
 from querent.processors.async_processor import AsyncProcessor
 from querent.ingestors.ingestor_factory import IngestorFactory
 from querent.ingestors.base_ingestor import BaseIngestor
 from querent.config.ingestor.ingestor_config import IngestorBackend
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common import common_errors
 from querent.common.types.ingested_tokens import IngestedTokens
@@ -93,22 +94,34 @@
                 text += paragraph.text + "\n"
 
             text = await self.process_data(text)
             yield IngestedTokens(
                 file=collected_bytes.file, data=text, error=None, doc_source=doc_source
             )
 
-            # i = 1
-            # for rel in doc.part.rels.values():
-            #     if "image" in rel.reltype:
-            #         image = rel.target_part.blob 
-            #         ocr_text = await self.process_image(image)
-            #         encoded_image = base64.b64encode(image)
-            #         yield IngestedImages(file = collected_bytes.file, image = encoded_image.decode('utf-8'), image_name=str(uuid.uuid4()), page_num=i, text=text, ocr_text=ocr_text, error=None, coordinates=None)
-            #         i += 1
+            i = 1
+            # for table in doc.tables:
+            #     table_data = []
+            #     for row in table.rows:
+            #         row_data = []
+            #         for cell in row.cells:
+            #             row_data.append(cell.text.strip())
+            #         table_data.append(row_data)
+            #     yield IngestedTables(file=collected_bytes.file, table = table_data, page_num = i, text = text, error=None)
+
+            i = 1
+            for rel in doc.part.rels.values():
+                if "image" in rel.reltype:
+                    image = rel.target_part.blob 
+                    ocr_text = await self.process_image(image)
+                    if not ocr_text:
+                        continue
+                    encoded_image = base64.b64encode(image)
+                    yield IngestedImages(file = collected_bytes.file, image = encoded_image.decode('utf-8'), image_name=str(uuid.uuid4()), page_num=i, text=text, ocr_text=[ocr_text], error=None, coordinates=None)
+                    i += 1
 
         elif file_extension == "doc":
             current_doc_text = await self.temp_extract_from(collected_bytes)
             yield IngestedTokens(
                 file=collected_bytes.file, data=current_doc_text, error=None, doc_source=doc_source
             )
         else:
@@ -162,13 +175,17 @@
 
     async def process_image(self, image_blob):
         try:
             image_stream = io.BytesIO(image_blob)
 
             image = Image.open(image_stream)
 
+            image_status = await self.analyze_image(image)
+            if not image_status:
+                return
+
             ocr_text = pytesseract.image_to_string(image)
 
             return ocr_text
         except Exception as e:
             self.logger.error(f"Error during image processing: {e}")
             return ""
```

### Comparing `querent-3.0.8/querent/ingestors/email/email_ingestor.py` & `querent-3.0.9/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/email/email_reader.py` & `querent-3.0.9/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/github/github_ingestor.py` & `querent-3.0.9/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/html/html_ingestor.py` & `querent-3.0.9/querent/ingestors/html/html_ingestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
             for img_tag in soup.find_all('img'):
                 img_src = img_tag.get('src')
                 if img_src and img_src.startswith('data:image'):
                     base64_data = img_src.split(';base64,')[-1]
                     image_data = base64.b64decode(base64_data)
                     image_ocr = await self.process_image(io.BytesIO(image_data))
 
+                    if not image_ocr:
+                        continue
                     yield IngestedImages(file = collected_bytes.file, image = base64_data, image_name = str(uuid.uuid4()), page_num=i, text = soup, ocr_text = image_ocr, coordinates= None, error= None, doc_source=doc_source)
                     i += 1
         except UnicodeDecodeError as exc:
             raise common_errors.UnicodeDecodeError(
                 f"Getting UnicodeDecodeError on this file {collected_bytes.file} as {exc}"
             ) from exc
         except LookupError as exc:
@@ -134,12 +136,15 @@
             return processed_data
         except Exception as e:
             self.logger.error(f"Error while processing text: {e}")
 
     async def process_image(self, image_stream):
         try:
             image = Image.open(image_stream)
+            image_status = await self.analyze_image(image)
+            if not image_status:
+                return
             ocr_text = pytesseract.image_to_string(image)
             return ocr_text
         except Exception as e:
             self.logger.error(f"Error during image processing: {e}")
             return ""
```

### Comparing `querent-3.0.8/querent/ingestors/images/image_ingestor.py` & `querent-3.0.9/querent/ingestors/images/image_ingestor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import List, AsyncGenerator
+import base64
+import uuid
 from querent.common.types.collected_bytes import CollectedBytes
+from querent.common.types.ingested_images import IngestedImages
 from querent.ingestors.base_ingestor import BaseIngestor
 from querent.ingestors.ingestor_factory import IngestorFactory
 from querent.processors.async_processor import AsyncProcessor
 from querent.config.ingestor.ingestor_config import IngestorBackend
 from querent.processors.async_processor import AsyncProcessor
 from querent.common.common_errors import (
     FileNotFoundError,
@@ -48,39 +51,48 @@
                     continue
 
                 if chunk_bytes.file != current_file:
                     if current_file:
                         text = await self.extract_and_process_image(
                             CollectedBytes(file=current_file, data=collected_bytes)
                         )
-                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
-                        yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
+                        if text is not None:
+                            yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
+                            yield IngestedImages(file=current_file, image=base64.b64encode(collected_bytes).decode('utf-8'), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
+                            yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
                     current_file = chunk_bytes.file
                     collected_bytes = b""
 
                 collected_bytes += chunk_bytes.data
 
             if current_file:
                 text = await self.extract_and_process_image(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 )
-                yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
-                yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
+                if text is not None:
+                    yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
+                    yield IngestedImages(file=current_file, image=base64.b64encode(collected_bytes).decode('utf-8'), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
+                    yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
         except Exception as e:
             yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_image(self, collected_bytes: CollectedBytes) -> str:
         text = await self.extract_text_from_image(collected_bytes)
+        if not text:
+            return
         return await self.process_data(text)
 
     async def extract_text_from_image(self, collected_bytes: CollectedBytes) -> str:
         try:
             image = Image.open(io.BytesIO(collected_bytes.data))
+            image_status = await self.analyze_image(image)
+            if not image_status:
+                return
 
         except FileNotFoundError as exc:
             raise FileNotFoundError(
                 f"Given file with name as {collected_bytes.file} not found"
             ) from exc
         except IOError as exc:
             raise IOError(
```

### Comparing `querent-3.0.8/querent/ingestors/ingestor_factory.py` & `querent-3.0.9/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/ingestor_manager.py` & `querent-3.0.9/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/json/json_ingestor.py` & `querent-3.0.9/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.9/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import AsyncGenerator, List
 from io import BytesIO
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common.types.ingested_tokens import IngestedTokens
 from querent.common.types.ingested_images import IngestedImages
+from querent.common.types.ingested_table import IngestedTables
 from querent.config.ingestor.ingestor_config import IngestorBackend
 from querent.ingestors.base_ingestor import BaseIngestor
 from querent.ingestors.ingestor_factory import IngestorFactory
 from querent.logging.logger import setup_logger
 from querent.processors.async_processor import AsyncProcessor
 from querent.common import common_errors
 import uuid
 import fitz
 from PIL import Image
 import io
+import base64
 
 import pybase64
 import pytesseract
+# import pdfplumber
 
 
 class PdfIngestorFactory(IngestorFactory):
     SUPPORTED_EXTENSIONS = {"pdf"}
 
     async def supports(self, file_extension: str) -> bool:
         return file_extension.lower() in self.SUPPORTED_EXTENSIONS
@@ -89,15 +92,14 @@
     async def extract_and_process_pdf(
         self, collected_bytes: CollectedBytes, doc_source: str
     ) -> AsyncGenerator[IngestedTokens, None]:
         try:
             path = BytesIO(collected_bytes.data)
             loader = fitz.open(stream=path.read(), filetype="pdf")
 
-
             for page in loader:
                 text = page.get_text()
                 if not text:
                     continue
 
                 text = text.replace('\"', ' ').replace('\“', '').replace('\”', '')
 
@@ -105,70 +107,100 @@
                 # Yield processed text as IngestedTokens
                 yield IngestedTokens(
                     file=collected_bytes.file,
                     data=processed_text,
                     error=collected_bytes.error,
                     doc_source=doc_source,
                 )
-                # async for image_result in self.extract_images_and_ocr(
-                #     page,
-                #     page_num,
-                #     processed_text,
-                #     collected_bytes.data,
-                #     collected_bytes.file,
-                # ):
-                #     yield image_result
+            
+            # async for table in self.extract_table(collected_bytes):
+            #     yield table
+            
+            async for imgae_data in self.extract_img(loader, collected_bytes.file, collected_bytes.data, doc_source):
+                yield imgae_data
 
         except TypeError as exc:
             self.logger.error(f"Exception while extracting pdf {exc}")
             raise common_errors.TypeError(
                 f"Getting type error on this file {collected_bytes.file}"
             ) from exc
 
         except Exception as exc:
             self.logger.error(f"Exception while extracting pdf {exc}")
             raise common_errors.UnknownError(
                 f"Getting unknown error while handling this file: {collected_bytes.file} error - {exc}"
             ) from exc
+        
+    # async def extract_table(self, data):
+    #     with pdfplumber.open(io.BytesIO(data.data)) as pdf:
+    #         i = 0
+    #         for page in pdf.pages:
+    #             # Extract tables from the current page
+    #             tables = page.extract_tables()
+    #             i += 1
+    #             # for table in tables:
+    #             #     if len(table) <= 1:
+    #             #         continue
+
+    #             #     yield IngestedTables(file= data.file, table = table, text=page.extract_text(), error=None, page_num= i)
+        
+    async def extract_img(self, doc, file_path, data, doc_source):
+        image_page_map = {}
+
+        # Iterate through the pages to fill the map
+        for page_num in range(len(doc)):
+            page = doc.load_page(page_num)
+            image_list = page.get_images(full=True)  # Get full details including xref
+            for img in image_list:
+                xref = img[0]
+                image_page_map[xref] = page_num + 1  # Page numbers are 1-indexed for humans
+
+        # Now we can extract images knowing their page numbers
+        for xref, page_num in image_page_map.items():
+            img = doc.extract_image(xref)
+            if img:  # If image extraction was successful
+                image_data = img["image"]
+                image_ext = img["ext"]
+
+                ocr_text = await self.get_ocr_from_image(image=img["image"])
+                if not ocr_text:
+                    continue
+
+                # Adjust page_num for 0-indexed access and check if it's within range
+                page_index = page_num - 1
+                if page_index < len(doc):
+                    text_content = doc[page_index].get_text()
+                else:
+                    text_content = "Page not in document."
 
-    async def extract_images_and_ocr(self, page, page_num, text, data, file_path):
-        try:
-            for image_path in page.images:
-                ocr = await self.get_ocr_from_image(image_path)
                 yield IngestedImages(
                     file=file_path,
-                    image=pybase64.b64encode(data),
-                    image_name=uuid.uuid4(),
+                    image=base64.b64encode(image_data).decode('utf-8'),
+                    image_name=f"{str(uuid.uuid4())}.{image_ext}",
                     page_num=page_num,
-                    text=text,
+                    text=[text_content],
                     coordinates=None,
-                    ocr_text=ocr,
+                    ocr_text=[ocr_text],
+                    doc_source=doc_source,
                 )
-        except Exception as e:
-            self.logger.error(f"Error extracting images and OCR: {e}")
-            yield IngestedImages(
-                file=file_path,
-                image=pybase64.b64encode(data),
-                image_name=uuid.uuid4(),
-                page_num=page_num,
-                text=text,
-                coordinates=None,
-                ocr_text=None,
-                error=f"Exception:{e}",
-            )
+
 
     async def get_ocr_from_image(self, image):
         """Implement this to return ocr text of the image"""
         try:
-            image = Image.open(io.BytesIO(image.data))
+            image = Image.open(io.BytesIO(image))
+
+            image_status = await self.analyze_image(image)
+            if not image_status:
+                return
             text = pytesseract.image_to_string(image)
         except Exception as e:
             self.logger.error("Exception-{e}")
             raise e
-        return str(text).encode("utf-8").decode("unicode_escape")
+        return str(text).encode("utf-8").decode("utf-8")
 
     async def process_data(self, text: str) -> str:
         if self.processors is None or len(self.processors) == 0:
             return [text]
         try:
             processed_data = text
             for processor in self.processors:
```

### Comparing `querent-3.0.8/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.9/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pptx.enum.shapes import MSO_SHAPE_TYPE
 import io
 from PIL import Image
 import pytesseract
 import pybase64
 import uuid
 
+from querent.common.types.ingested_table import IngestedTables
 from querent.ingestors.ingestor_factory import IngestorFactory
 from querent.processors.async_processor import AsyncProcessor
 from querent.ingestors.base_ingestor import BaseIngestor
 from querent.config.ingestor.ingestor_config import IngestorBackend
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common import common_errors
 from querent.common.types.ingested_tokens import IngestedTokens
@@ -86,17 +87,30 @@
                 presentation = Presentation(ppt_file)
                 i=1
                 for slide in presentation.slides:
                     text = []
                     for shape in slide.shapes:
                         if hasattr(shape, "text"):
                             text.append(shape.text)
-                        # if shape.shape_type == MSO_SHAPE_TYPE.PICTURE or (shape.shape_type in [MSO_SHAPE_TYPE.PLACEHOLDER, MSO_SHAPE_TYPE.AUTO_SHAPE] and hasattr(shape, "image")):
-                        #     ocr_text = await self.process_image(shape)
-                        #     yield IngestedImages(file=collected_bytes.file, image=pybase64.b64encode(shape.image.blob), image_name=str(uuid.uuid4()), page_num=i, text = text, ocr_text=[ocr_text], coordinates=None)
+                        if shape.shape_type == MSO_SHAPE_TYPE.PICTURE or (shape.shape_type in [MSO_SHAPE_TYPE.PLACEHOLDER, MSO_SHAPE_TYPE.AUTO_SHAPE] and hasattr(shape, "image")):
+                            ocr_text = await self.process_image(shape)
+                            if not ocr_text:
+                                continue
+                            yield IngestedImages(file=collected_bytes.file, image=pybase64.b64encode(shape.image.blob), image_name=str(uuid.uuid4()), page_num=i, text = text, ocr_text=[ocr_text], coordinates=None)
+
+                        if shape.has_table:
+                            table = shape.table
+                            
+                            table_data = []
+                            # for row in table.rows:
+                            #     row_data = []
+                            #     for cell in row.cells:
+                            #         row_data.append(cell.text)
+                            #     table_data.append(row_data)
+                            # yield IngestedTables(file= collected_bytes.file, table=table_data, page_num=i, text=text, error=None)
                     slide_text = "\n".join(text)
                     processed_slide_text = await self.process_data(slide_text)
                     yield IngestedTokens(
                         file=collected_bytes.file, data=processed_slide_text, error=None, doc_source=doc_source
                     )
                     i+=1
             elif collected_bytes.extension == "ppt":
@@ -136,14 +150,18 @@
 
     async def process_image(self, shape):
         try:
             # Retrieve image as a BytesIO object
             image_stream = io.BytesIO(shape.image.blob)
             image = Image.open(image_stream)
 
+            image_status = await self.analyze_image(image)
+            if not image_status:
+                return
+
             # Perform OCR using pytesseract
             ocr_text = pytesseract.image_to_string(image)
 
             return ocr_text
         except Exception as e:
             self.logger.error(f"Error during image processing: {e}")
             return ""
```

### Comparing `querent-3.0.8/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.9/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/video/video_ingestor.py` & `querent-3.0.9/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.9/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.9/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.9/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import json
 import spacy
 from transformers import AutoTokenizer, AutoModelForTokenClassification
 import torch
 import nltk
 from nltk.tokenize import sent_tokenize
 from typing import Any, List, Tuple
 from querent.logging.logger import setup_logger
 import os
 from querent.kg.ner_helperfunctions.dependency_parsing import Dependency_Parsing
 from unidecode import unidecode
 import re
+from collections import Counter
+
 
 
 """
     Named Entity Recognition (NER) class for extracting entities and relationships from text.
 
     Attributes:
         ner_tokenizer (Tokenizer): Tokenizer for the NER model.
@@ -263,15 +266,15 @@
                                 "next_sentence": all_sentences[sentence_idx + 1] if sentence_idx < len(all_sentences) - 1 else None
                             }
                             binary_pairs.append((pair, metadata))
         except Exception as e:
             self.logger.error(f"Error extracting binary pairs: {e}")
         return binary_pairs
     
-    def extract_fixed_entities_from_chunk(self, chunk: List[str], fixed_entities: List[str], entity_types: List[str], default_score=1.0):
+    def extract_fixed_entities_from_chunk(self, chunk: List[str], fixed_entities: List[str], entity_types: List[str], default_score=None):
         results = []
         merged_chunk = []  # List to hold merged tokens
         current_word = ""  # String to accumulate current word pieces
 
         # Preprocess chunk to merge tokens
         for token in chunk:
             if token.startswith("##"):
@@ -298,25 +301,41 @@
                         if char_count >= start_pos:
                             start_idx = idx
                             break
                         char_count += len(token) + (1 if idx < len(merged_chunk) - 1 else 0)  # Only add space if not the last token
 
                     if start_idx is not None:
                         label = entity_types[normalized_entities.index(entity)] if normalized_entities.index(entity) < len(entity_types) else 'Unknown'
+                        # Calculate score if not provided
+                        score = default_score if default_score is not None else 1.0  # Example default score calculation
                         results.append({
                             "entity": entity,
                             "label": label,
-                            "score": default_score,
+                            "score": score,
                             "start_idx": start_idx
                         })
         except Exception as e:
             self.logger.error(f"Error extracting fixed entities from merged chunk: {e}")
 
         return sorted(results, key=lambda x: x['start_idx'])
 
+    
+    def filter_matching_entities(self, tuples_nested_list, entities_nested_list):
+        matched_tuples = []
+        for entities_list in entities_nested_list:
+            for entity_dict in entities_list:
+                entity_name = entity_dict['entity']
+                for tuples_list in tuples_nested_list:
+                    for tup in tuples_list:
+                        if entity_name in tup[0] or entity_name in tup[2]:
+                            if tup not in matched_tuples:
+                                matched_tuples.append(tup)
+
+        return matched_tuples
+
 
 
 
     def extract_entities_from_sentence(self, sentence: str, sentence_idx: int, all_sentences: List[str], fixed_entities_flag: bool, fixed_entities: List[str],entity_types: List[str]):
         try:
             tokens = self.tokenize_sentence(sentence)
             chunks = self.get_chunks(tokens)
@@ -337,14 +356,39 @@
                     entity['noun_chunk_length'] = len(entity['noun_chunk'].split())
                 entities_withnnchunk = final_entities
             binary_pairs = self.extract_binary_pairs(entities_withnnchunk, tokens, all_sentences, sentence_idx)
             return entities_withnnchunk, binary_pairs
         except Exception as e:
             self.logger.error(f"Error extracting entities from sentence: {e}")
     
+    
+    def get_entity_pairs(self, isConfinedSearch, fixed_entities, sample_entities, content):
+        entity = []
+        doc_entity_pairs = []
+        tokens = self._tokenize_and_chunk(content)
+        for tokenized_sentence, original_sentence, sentence_idx in tokens:
+            (entities, entity_pairs,) = self.extract_entities_from_sentence(original_sentence, sentence_idx, [s[1] for s in tokens],isConfinedSearch, fixed_entities, sample_entities)
+            if entity_pairs:
+                doc_entity_pairs.append(self.transform_entity_pairs(entity_pairs))
+            if entities:
+                entity.append(entities)
+        return (entity, doc_entity_pairs)
+    
+    def final_ingested_images_tuples(self, filtered_triples, create_embeddings):
+        entity, info_json, second_entity = filtered_triples
+        info = json.loads(info_json)
+        info['subject_type'] = info.pop('entity1_label')
+        info['object_type'] = info.pop('entity2_label')
+        info['predicate'] = "has image"
+        info['predicate_type'] = "has image"
+        info['context_embeddings'] = create_embeddings.get_embeddings([info['context']])[0]
+        updated_json = json.dumps(info)
+        updated_tuple = (entity, updated_json, second_entity)
+        return updated_tuple
+    
     def remove_duplicates(self, data):
         seen = set()
         new_data = []
 
         for sublist in data:
             cleaned_sublist = []
             for sub_item in sublist:
```

### Comparing `querent-3.0.8/querent/kg/querent_kg.py` & `querent-3.0.9/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 import json
 from fastembed import TextEmbedding
 from querent.logging.logger import setup_logger
 
+
 class EmbeddingStore:
-    def __init__(self, model_name='sentence-transformers/all-MiniLM-L6-v2'):
+    def __init__(self, model_name="sentence-transformers/all-MiniLM-L6-v2"):
         self.logger = setup_logger("EmbeddingStore_config", "EmbeddingStore")
         try:
             self.model_name = model_name
             self.embeddings = TextEmbedding(model_name=model_name)
         except Exception as e:
-            self.logger.error(f"Invalid {self.__class__.__name__} configuration. Failed to initialize EmbeddingStore: {e}")
+            self.logger.error(
+                f"Invalid {self.__class__.__name__} configuration. Failed to initialize EmbeddingStore: {e}"
+            )
             raise Exception(f"Failed to initialize EmbeddingStore: {e}")
-    
+
     def get_embeddings(self, texts):
         try:
             embeddings = []
             for text in texts:
                 embedding_generator = self.embeddings.embed(text)
                 embedding = list(embedding_generator)[0]
                 embeddings.append(embedding.tolist())
             return embeddings
         except Exception as e:
             self.logger.error(f"Failed to generate embeddings: {e}")
             raise Exception(f"Failed to generate embeddings: {e}")
-    
-    
+
     def generate_embeddings(self, payload):
         try:
             triples = payload
             processed_pairs = []
             for entity, json_string, related_entity in triples:
                 try:
                     data = json.loads(json_string)
                     context = data.get("context", "").replace('"', '\\"')
-                    predicate = data.get("predicate","").replace('"', '\\"')
-                    predicate_type = data.get("predicate_type","Unlabeled").replace('"', '\\"')
-                    subject_type = data.get("subject_type","Unlabeled").replace('"', '\\"')
-                    object_type = data.get("object_type","Unlabeled").replace('"', '\\"')
+                    predicate = data.get("predicate", "").replace('"', '\\"')
+                    predicate_type = data.get("predicate_type", "Unlabeled").replace(
+                        '"', '\\"'
+                    )
+                    subject_type = data.get("subject_type", "Unlabeled").replace(
+                        '"', '\\"'
+                    )
+                    object_type = data.get("object_type", "Unlabeled").replace(
+                        '"', '\\"'
+                    )
                     context_embeddings = self.get_embeddings([context])[0]
                     essential_data = {
                         "context": context,
-                        "context_embeddings" : context_embeddings,
+                        "context_embeddings": context_embeddings,
                         "predicate_type": predicate_type,
-                        "predicate" : predicate,
+                        "predicate": predicate,
                         "subject_type": subject_type,
-                        "object_type": object_type
+                        "object_type": object_type,
                     }
                     updated_json_string = json.dumps(essential_data)
-                    processed_pairs.append((entity, updated_json_string, related_entity))
+                    processed_pairs.append(
+                        (entity, updated_json_string, related_entity)
+                    )
                 except json.JSONDecodeError as e:
-                    self.logger.debug(f"JSON parsing error: {e} in string: {json_string}")
+                    self.logger.debug(
+                        f"JSON parsing error: {e} in string: {json_string}"
+                    )
 
             return processed_pairs
 
         except Exception as e:
             self.logger.error(f"Error in extracting embeddings: {e}")
-
-
```

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.9/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,28 +48,29 @@
             }
 
             return json_object
         except Exception as e:
             raise Exception(f"Error in convert_graphjson: {e}")
 
     @staticmethod
-    def convert_vectorjson(triple):
+    def convert_vectorjson(triple, blob = None):
         try:
             subject, json_str, object_ = triple
             data = TripleToJsonConverter._parse_json_str(json_str)
             if data is None:
                 return {}
 
             id_format = f"{TripleToJsonConverter._normalize_text(subject)}-{TripleToJsonConverter._normalize_text(data.get('predicate', ''))}-{TripleToJsonConverter._normalize_text(object_)}"
             json_object = {
                 "id": TripleToJsonConverter._normalize_text(id_format,replace_space=True).replace(",","_"),
                 "embeddings": data.get("context_embeddings", []),
                 "size": len(data.get("context_embeddings", [])),
                 "namespace": TripleToJsonConverter._normalize_text(data.get("predicate", ""),replace_space=True),
-                "sentence": data.get("context", "").lower()
+                "sentence": data.get("context", "").lower(),
+                "blob": blob,
             }
 
             return json_object
         except Exception as e:
             raise Exception(f"Error in convert_vectorjson: {e}")
```

### Comparing `querent-3.0.8/querent/logging/filters.py` & `querent-3.0.9/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/logging/handlers.py` & `querent-3.0.9/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/logging/logger.py` & `querent-3.0.9/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.9/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/metric/metric_logging_handler.py` & `querent-3.0.9/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/metric/metric_registry.py` & `querent-3.0.9/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/processors/text_cleanup_processor.py` & `querent-3.0.9/querent/processors/text_cleanup_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,10 @@
         self.logger = setup_logger(__name__, "TextCleanupProcessor")
 
     async def process_text(self, data: str) -> str:
         data = data.replace("\"", "").replace('\“', '').replace('\”', '')
         data = data.replace("\\n", " ").replace("\\t", " ")
         data = re.sub(r'\\x[0-9a-fA-F]{2}', '', data)
         data = data.replace("\n", " ").replace("\r", " ").replace("\t", " ")
+        data = re.sub(r'[\x00-\x08\x0b\x0c\x0e-\x1f]+', '', data)
 
         return data
```

### Comparing `querent-3.0.8/querent/processors/text_processor.py` & `querent-3.0.9/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/querent/auto_scaler.py` & `querent-3.0.9/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/querent/querent.py` & `querent-3.0.9/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/querent/resource_manager.py` & `querent-3.0.9/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/storage/gcs_query.py` & `querent-3.0.9/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.9/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.9/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.9/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/tools/web_page_extractor.py` & `querent-3.0.9/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/utils/webpage_extractor.py` & `querent-3.0.9/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent/workflow/_helpers.py` & `querent-3.0.9/querent/workflow/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,19 +99,19 @@
         receive_token_feeder(
             resource_manager=resource_manager,
             config=config,
             result_queue=result_queue,
         )
     )
 
-    # check_message_states_task = asyncio.create_task(
-    #     check_message_states(config, resource_manager, [querent_task, token_feeder])
-    # )
+    check_message_states_task = asyncio.create_task(
+        check_message_states(config, resource_manager, [querent_task, token_feeder])
+    )
 
-    await asyncio.gather(querent_task, token_feeder)
+    await asyncio.gather(querent_task, token_feeder, check_message_states_task)
 
 
 async def start_gpt_workflow(
     resource_manager: ResourceManager, config: Config, result_queue: QuerentQueue
 ):
     search_directory = os.getenv('MODEL_PATH', '/model/')
     setup_nltk_and_spacy_paths(config, search_directory)
```

### Comparing `querent-3.0.8/querent/workflow/workflow.py` & `querent-3.0.9/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.8/querent.egg-info/PKG-INFO` & `querent-3.0.9/querent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.8
+Version: 3.0.9
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -72,14 +72,15 @@
 Requires-Dist: newsapi-python==0.2.7
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==1.13.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: pdfminer==20191125
+Requires-Dist: pdfplumber==0.10.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: prometheus-client==0.17.1
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pybase64==1.3.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydub==0.25.1
 Requires-Dist: pyjwt==2.4.0
```

### Comparing `querent-3.0.8/querent.egg-info/SOURCES.txt` & `querent-3.0.9/querent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 querent/common/types/collector_config_keys.py
 querent/common/types/config_keys.py
 querent/common/types/engine_config_keys.py
 querent/common/types/file_buffer.py
 querent/common/types/ingested_code.py
 querent/common/types/ingested_images.py
 querent/common/types/ingested_messages.py
+querent/common/types/ingested_table.py
 querent/common/types/ingested_tokens.py
 querent/common/types/querent_event.py
 querent/common/types/querent_queue.py
 querent/common/types/resource_config_keys.py
 querent/common/types/workflow_config_keys.py
 querent/config/__init__.py
 querent/config/config.py
```

### Comparing `querent-3.0.8/querent.egg-info/requires.txt` & `querent-3.0.9/querent.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 newsapi-python==0.2.7
 nltk==3.8.1
 numpy==1.24.3
 openai==1.13.3
 openpyxl==3.1.2
 pandas==2.1.4
 pdfminer==20191125
+pdfplumber==0.10.0
 pillow==10.3.0
 prometheus-client==0.17.1
 psutil==5.9.8
 pybase64==1.3.1
 pydantic==2.6.4
 pydub==0.25.1
 pyjwt==2.4.0
```

### Comparing `querent-3.0.8/setup.py` & `querent-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "newsapi-python==0.2.7",
     "nltk==3.8.1",
     "numpy==1.24.3",
     "openai==1.13.3",
     "openpyxl==3.1.2",
     "pandas==2.1.4",
     "pdfminer==20191125",
+    "pdfplumber==0.10.0",
     "pillow==10.3.0",
     "prometheus-client==0.17.1",
     "psutil==5.9.8",
     "pybase64==1.3.1",
     "pydantic==2.6.4",
     "pydub==0.25.1",
     "pyjwt==2.4.0",
@@ -74,15 +75,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.8",
+    version="3.0.9",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

